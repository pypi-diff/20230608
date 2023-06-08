# Comparing `tmp/pclick-0.1.29.tar.gz` & `tmp/pclick-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pclick-0.1.29.tar", max compression
+gzip compressed data, was "pclick-0.1.30.tar", max compression
```

## Comparing `pclick-0.1.29.tar` & `pclick-0.1.30.tar`

### file list

```diff
@@ -1,20 +1,11 @@
--rw-r--r--   0        0        0     1070 2021-10-20 11:00:43.860801 pclick-0.1.29/README.md
--rw-r--r--   0        0        0      476 2023-06-07 09:25:24.359356 pclick-0.1.29/pyproject.toml
--rw-r--r--   0        0        0    10259 2023-06-07 07:32:08.130569 pclick-0.1.29/src/pclick/Messaging_pb2.py
--rw-r--r--   0        0        0      527 2022-12-20 09:23:53.909558 pclick-0.1.29/src/pclick/__init__.py
--rw-r--r--   0        0        0     1087 2022-09-09 16:13:16.831909 pclick-0.1.29/src/pclick/client.py
--rw-r--r--   0        0        0        0 2021-10-15 12:09:20.013250 pclick-0.1.29/src/pclick/demo/__init__.py
--rw-r--r--   0        0        0      159 2022-10-24 11:54:24.274468 pclick-0.1.29/src/pclick/demo/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      157 2022-06-20 06:44:26.841227 pclick-0.1.29/src/pclick/demo/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0        0        0     3457 2023-05-31 11:34:14.381785 pclick-0.1.29/src/pclick/demo/__pycache__/client.cpython-310.pyc
--rw-r--r--   0        0        0     3461 2023-05-22 14:26:39.207729 pclick-0.1.29/src/pclick/demo/__pycache__/client.cpython-39.pyc
--rw-r--r--   0        0        0     2898 2022-09-13 13:14:55.794124 pclick-0.1.29/src/pclick/demo/__pycache__/client_shared.cpython-39.pyc
--rw-r--r--   0        0        0     2990 2022-09-12 15:08:46.858446 pclick-0.1.29/src/pclick/demo/__pycache__/pub_demo_server.cpython-39.pyc
--rw-r--r--   0        0        0     3081 2023-05-31 09:24:47.280850 pclick-0.1.29/src/pclick/demo/__pycache__/server.cpython-310.pyc
--rw-r--r--   0        0        0     3076 2023-05-22 14:12:21.319547 pclick-0.1.29/src/pclick/demo/__pycache__/server.cpython-39.pyc
--rw-r--r--   0        0        0     1652 2022-09-13 13:14:55.791524 pclick-0.1.29/src/pclick/demo/__pycache__/sub_demo_client.cpython-39.pyc
--rw-r--r--   0        0        0     4566 2023-06-07 07:32:08.131103 pclick-0.1.29/src/pclick/demo/client.py
--rw-r--r--   0        0        0     3767 2023-06-07 07:32:08.131614 pclick-0.1.29/src/pclick/demo/server.py
--rw-r--r--   0        0        0     2014 2021-10-20 09:58:12.229791 pclick-0.1.29/src/pclick/message_proto_helpers.py
--rw-r--r--   0        0        0     2537 2023-06-07 07:32:08.132121 pclick-0.1.29/src/pclick/server.py
--rw-r--r--   0        0        0     1754 1970-01-01 00:00:00.000000 pclick-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0     1116 2023-06-08 07:31:57.421043 pclick-0.1.30/README.md
+-rw-r--r--   0        0        0      533 2023-06-08 07:32:36.363867 pclick-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0    10259 2023-06-07 07:32:08.130569 pclick-0.1.30/src/pclick/Messaging_pb2.py
+-rw-r--r--   0        0        0      527 2023-06-07 13:56:45.585922 pclick-0.1.30/src/pclick/__init__.py
+-rw-r--r--   0        0        0     1087 2023-06-07 13:56:45.595713 pclick-0.1.30/src/pclick/client.py
+-rw-r--r--   0        0        0        0 2021-10-15 12:09:20.013250 pclick-0.1.30/src/pclick/demo/__init__.py
+-rw-r--r--   0        0        0     4566 2023-06-07 13:56:45.585972 pclick-0.1.30/src/pclick/demo/client.py
+-rw-r--r--   0        0        0     3767 2023-06-07 13:56:58.282284 pclick-0.1.30/src/pclick/demo/server.py
+-rw-r--r--   0        0        0     2014 2023-06-07 13:56:45.587181 pclick-0.1.30/src/pclick/message_proto_helpers.py
+-rw-r--r--   0        0        0     2537 2023-06-07 13:56:45.585944 pclick-0.1.30/src/pclick/server.py
+-rw-r--r--   0        0        0     1800 1970-01-01 00:00:00.000000 pclick-0.1.30/PKG-INFO
```

### Comparing `pclick-0.1.29/README.md` & `pclick-0.1.30/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -16,18 +16,22 @@
 1. Client controller connects and sends HandshakeInit
 2. Server responds with Handshake
 3. Client receives Handshake and validates the setup.
 4. Client sends Controls
 5. Server responds with Sensors
 6. The loop 4-5 is repeated.
 
-## Run demo server
+## Run demo
 
 ```bash
-python3 -m pClick.demo.server
+python3.9 -m pclick.demo.server --trace
+```
+
+```bash
+python3 -m pclick.demo.client
 ```
 
 ## Use
 
 ```python
-import pClick
+import pclick
 ```
```

### Comparing `pclick-0.1.29/src/pclick/Messaging_pb2.py` & `pclick-0.1.30/src/pclick/Messaging_pb2.py`

 * *Files identical despite different names*

### Comparing `pclick-0.1.29/src/pclick/client.py` & `pclick-0.1.30/src/pclick/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import zmq
-from pClick.message_proto_helpers import MessageSerializer, Message
+from pclick.message_proto_helpers import MessageSerializer, Message
 
 
 class Client:
     def __init__(self):
         self.context = zmq.Context()
         self.socket = self.context.socket(zmq.REQ)
```

### Comparing `pclick-0.1.29/src/pclick/demo/client.py` & `pclick-0.1.30/src/pclick/demo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #
 #   click client in Python
 #   Connects REQ socket to tcp://localhost:5555
 #   Sends "HandshakeInit" to server, expects "Handshake" back
 #
 
-from pClick import Client
-from pClick import MessageFactory
+from pclick import Client
+from pclick import MessageFactory
 from argparse import ArgumentParser
 
-from pClick.Messaging_pb2 import SensorMessageType
+from pclick.Messaging_pb2 import SensorMessageType
 from time import time
 
 def parse_args():
     parser = ArgumentParser(description='Demo client connecting to click server')
     parser.add_argument('--host', metavar='<host>', type=str, default="localhost",
                         help=f'server to connect to, default is localhost')
     parser.add_argument('--port', metavar='<port>', type=str, default="5555",
```

### Comparing `pclick-0.1.29/src/pclick/demo/server.py` & `pclick-0.1.30/src/pclick/demo/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #
 #   Click server in Python
 #   Binds REP socket to tcp://*:5555
 #   Expects Message from client, replies with Message
 #
 
-from pClick import Server, MessageFactory, ControlMessageType, HandshakeInitMessageType, ValueType
-from pClick.server import SizeCollectorChanges
+from pclick import Server, MessageFactory, ControlMessageType, HandshakeInitMessageType, ValueType
+from pclick.server import SizeCollectorChanges
 from argparse import ArgumentParser
 
 
 def parse_args():
     parser = ArgumentParser(description='Demo client connecting to click server')
     parser.add_argument('--host', metavar='<host>', type=str, default="*",
                         help=f'server to connect to, default is *')
@@ -29,15 +29,15 @@
     addr = f"tcp://{args.host}:{args.port}"
     if args.addr:
         addr = args.addr
     server = Server(addr)
     if args.trace_sizes:
         server.size_collector = SizeCollectorChanges()
 
-    # Note: Below code uses the protobuf API directly, we recommend using the higher level agxClick ClickObject and ClickRobot instead
+    # Note: Below code uses the protobuf API directly, we recommend using the higher level agxclick ClickObject and ClickRobot instead
     # if possible - to protect client code from future protocol changes.
     while True:
 
         request = server.recv()
         if request is None:
             continue
         if args.trace:
```

### Comparing `pclick-0.1.29/src/pclick/message_proto_helpers.py` & `pclick-0.1.30/src/pclick/message_proto_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-from pClick.Messaging_pb2 import CURRENT_VERSION, Message, ErrorMessage, HandshakeMessage, SensorMessage, ControlMessage, ResetMessage, HandshakeInitMessage, SensorRequestMessage
-from pClick.Messaging_pb2 import HandshakeInitMessageType, ErrorMessageType, HandshakeMessageType, SensorMessageType, ControlMessageType, ResetMessageType, SensorRequestMessageType
+from pclick.Messaging_pb2 import CURRENT_VERSION, Message, ErrorMessage, HandshakeMessage, SensorMessage, ControlMessage, ResetMessage, HandshakeInitMessage, SensorRequestMessage
+from pclick.Messaging_pb2 import HandshakeInitMessageType, ErrorMessageType, HandshakeMessageType, SensorMessageType, ControlMessageType, ResetMessageType, SensorRequestMessageType
 
 
 class MessageFactory:
     _mdict = {HandshakeInitMessageType: HandshakeInitMessage,
               HandshakeMessageType: HandshakeMessage,
               ControlMessageType: ControlMessage,
               SensorMessageType: SensorMessage,
```

### Comparing `pclick-0.1.29/src/pclick/server.py` & `pclick-0.1.30/src/pclick/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import zmq
-from pClick.message_proto_helpers import MessageSerializer, Message
+from pclick.message_proto_helpers import MessageSerializer, Message
 from abc import abstractmethod
 
 
 class SizeCollector:
     """
     A no operation SizeCollector.
     """
```

### Comparing `pclick-0.1.29/PKG-INFO` & `pclick-0.1.30/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: pclick
-Version: 0.1.29
+Version: 0.1.30
 Summary: Controller to AGX messaging
 Home-page: https://github.com/algoryx/click-mirror
 License: Apache-2.0
 Author: Algoryx Simulation
 Author-email: contact@algoryx.se
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Dist: protobuf (==3.17.1)
+Requires-Dist: protobuf (==3.20.3)
 Requires-Dist: pyzmq (==22.3.0)
 Project-URL: Repository, https://github.com/algoryx/click-mirror
 Description-Content-Type: text/markdown
 
 # Click
 
 The main idea behind click is to enable a non-Brick controller talking to a Brick enabled AGX Simulation in way configurable by Brick.
@@ -35,19 +35,23 @@
 1. Client controller connects and sends HandshakeInit
 2. Server responds with Handshake
 3. Client receives Handshake and validates the setup.
 4. Client sends Controls
 5. Server responds with Sensors
 6. The loop 4-5 is repeated.
 
-## Run demo server
+## Run demo
 
 ```bash
-python3 -m pClick.demo.server
+python3.9 -m pclick.demo.server --trace
+```
+
+```bash
+python3 -m pclick.demo.client
 ```
 
 ## Use
 
 ```python
-import pClick
+import pclick
 ```
```

