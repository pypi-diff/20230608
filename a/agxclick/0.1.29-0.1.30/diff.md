# Comparing `tmp/agxclick-0.1.29.tar.gz` & `tmp/agxclick-0.1.30.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agxclick-0.1.29.tar", max compression
+gzip compressed data, was "agxclick-0.1.30.tar", max compression
```

## Comparing `agxclick-0.1.29.tar` & `agxclick-0.1.30.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    10433 2023-06-07 08:50:39.313818 agxclick-0.1.29/README.md
--rw-r--r--   0        0        0      495 2023-06-07 09:26:12.304609 agxclick-0.1.29/pyproject.toml
--rw-r--r--   0        0        0      649 2022-06-02 06:39:22.620436 agxclick-0.1.29/src/agxclick/__init__.py
--rw-r--r--   0        0        0     2348 2022-06-02 06:39:22.622000 agxclick-0.1.29/src/agxclick/agx_application.py
--rw-r--r--   0        0        0      264 2022-06-16 12:35:01.202788 agxclick-0.1.29/src/agxclick/application_step_listener.py
--rw-r--r--   0        0        0     1647 2023-06-07 07:32:08.110496 agxclick-0.1.29/src/agxclick/brick_reader.py
--rw-r--r--   0        0        0     2379 2022-06-02 06:39:22.625681 agxclick-0.1.29/src/agxclick/brick_utils.py
--rw-r--r--   0        0        0    10140 2023-06-07 07:32:08.110706 agxclick-0.1.29/src/agxclick/click_application.py
--rw-r--r--   0        0        0     9778 2023-06-07 07:32:08.110907 agxclick-0.1.29/src/agxclick/click_event_listener.py
--rw-r--r--   0        0        0    10192 2023-06-07 07:32:08.111099 agxclick-0.1.29/src/agxclick/click_robot.py
--rw-r--r--   0        0        0      736 2022-06-02 06:39:22.629400 agxclick-0.1.29/src/agxclick/graphics_throttler.py
--rw-r--r--   0        0        0     1319 2021-11-17 10:51:45.931702 agxclick-0.1.29/src/agxclick/keyboard_listener.py
--rw-r--r--   0        0        0    10279 2023-06-07 07:32:08.111672 agxclick-0.1.29/src/agxclick/message_factory.py
--rw-r--r--   0        0        0     1230 2023-06-07 07:32:08.111855 agxclick-0.1.29/src/agxclick/reset_batch_listener.py
--rw-r--r--   0        0        0      348 2022-06-02 06:39:22.631892 agxclick-0.1.29/src/agxclick/wallclock.py
--rw-r--r--   0        0        0    11081 1970-01-01 00:00:00.000000 agxclick-0.1.29/PKG-INFO
+-rw-r--r--   0        0        0     1324 2023-06-08 07:28:16.340888 agxclick-0.1.30/README-pypi.md
+-rw-r--r--   0        0        0      560 2023-06-08 07:33:35.344826 agxclick-0.1.30/pyproject.toml
+-rw-r--r--   0        0        0      649 2023-06-07 13:56:58.281738 agxclick-0.1.30/src/agxclick/__init__.py
+-rw-r--r--   0        0        0     2348 2022-06-02 06:39:22.622000 agxclick-0.1.30/src/agxclick/agx_application.py
+-rw-r--r--   0        0        0      264 2022-06-16 12:35:01.202788 agxclick-0.1.30/src/agxclick/application_step_listener.py
+-rw-r--r--   0        0        0     1647 2023-06-07 13:56:58.282251 agxclick-0.1.30/src/agxclick/brick_reader.py
+-rw-r--r--   0        0        0     2379 2022-06-02 06:39:22.625681 agxclick-0.1.30/src/agxclick/brick_utils.py
+-rw-r--r--   0        0        0    10140 2023-06-07 13:56:58.281157 agxclick-0.1.30/src/agxclick/click_application.py
+-rw-r--r--   0        0        0     9778 2023-06-07 13:56:58.281087 agxclick-0.1.30/src/agxclick/click_event_listener.py
+-rw-r--r--   0        0        0    10192 2023-06-07 13:56:58.281650 agxclick-0.1.30/src/agxclick/click_robot.py
+-rw-r--r--   0        0        0      736 2023-06-07 13:56:58.281768 agxclick-0.1.30/src/agxclick/graphics_throttler.py
+-rw-r--r--   0        0        0     1319 2021-11-17 10:51:45.931702 agxclick-0.1.30/src/agxclick/keyboard_listener.py
+-rw-r--r--   0        0        0    10279 2023-06-07 13:56:58.281698 agxclick-0.1.30/src/agxclick/message_factory.py
+-rw-r--r--   0        0        0     1230 2023-06-07 13:56:58.281034 agxclick-0.1.30/src/agxclick/reset_batch_listener.py
+-rw-r--r--   0        0        0      348 2022-06-02 06:39:22.631892 agxclick-0.1.30/src/agxclick/wallclock.py
+-rw-r--r--   0        0        0     1973 1970-01-01 00:00:00.000000 agxclick-0.1.30/PKG-INFO
```

### Comparing `agxclick-0.1.29/src/agxclick/__init__.py` & `agxclick-0.1.30/src/agxclick/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from agxClick.brick_utils import BrickUtils
-from agxClick.click_robot import ClickRobot, ClickObject
-from agxClick.brick_reader import find_robots_in_scene, get_click_configuration, has_click_configuration
-from agxClick.message_factory import MessageFactory, update_robots_from_message
-from agxClick.application_step_listener import ApplicationStepListener, noop
-from agxClick.reset_batch_listener import ResetBatchListener
-from agxClick.click_event_listener import ClickFrameListener
-from agxClick.keyboard_listener import KeyboardListener
-from agxClick.agx_application import AgxApplication
-from agxClick.click_application import ClickApplication
+from agxclick.brick_utils import BrickUtils
+from agxclick.click_robot import ClickRobot, ClickObject
+from agxclick.brick_reader import find_robots_in_scene, get_click_configuration, has_click_configuration
+from agxclick.message_factory import MessageFactory, update_robots_from_message
+from agxclick.application_step_listener import ApplicationStepListener, noop
+from agxclick.reset_batch_listener import ResetBatchListener
+from agxclick.click_event_listener import ClickFrameListener
+from agxclick.keyboard_listener import KeyboardListener
+from agxclick.agx_application import AgxApplication
+from agxclick.click_application import ClickApplication
```

### Comparing `agxclick-0.1.29/src/agxclick/agx_application.py` & `agxclick-0.1.30/src/agxclick/agx_application.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.29/src/agxclick/brick_reader.py` & `agxclick-0.1.30/src/agxclick/brick_reader.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List
-from agxClick import ClickObject, ClickRobot, BrickUtils
+from agxclick import ClickObject, ClickRobot, BrickUtils
 
 
 def has_click_configuration(scene_positioninput) -> bool:
     return BrickUtils.get_component_attribute(scene_positioninput, "clickobjects") is not None
 
 
 def get_click_configuration(click_scene) -> List[ClickRobot]:
```

### Comparing `agxclick-0.1.29/src/agxclick/brick_utils.py` & `agxclick-0.1.30/src/agxclick/brick_utils.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.29/src/agxclick/click_application.py` & `agxclick-0.1.30/src/agxclick/click_application.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from agxClick import KeyboardListener, AgxApplication, ClickFrameListener, ApplicationStepListener, ResetBatchListener
-from pClick import Server
-from pClick.server import SizeCollector, SizeCollectorChanges
+from agxclick import KeyboardListener, AgxApplication, ClickFrameListener, ApplicationStepListener, ResetBatchListener
+from pclick import Server
+from pclick.server import SizeCollector, SizeCollectorChanges
 from typing import Any, Callable, List
 import logging
-from agxClick.wallclock import WallClock
-from agxClick.graphics_throttler import GraphicsThrottler
+from agxclick.wallclock import WallClock
+from agxclick.graphics_throttler import GraphicsThrottler
 
 
 class ClickApplication(AgxApplication):
 
     def __init__(self, args: List[str]):
         super().__init__(args)
         self._logger = logging.getLogger(__file__)
```

### Comparing `agxclick-0.1.29/src/agxclick/click_event_listener.py` & `agxclick-0.1.30/src/agxclick/click_event_listener.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import queue
 import agxSDK
 from typing import List, Callable
-from agxClick import MessageFactory, ApplicationStepListener, update_robots_from_message, find_robots_in_scene, has_click_configuration, ClickObject, noop
-from pClick import Server, HandshakeInitMessageType, ControlMessageType, ResetMessageType, SensorRequestMessageType, ErrorMessageType
-from pClick import ControlMessage, MessageFactory as ProtoMessageFactory
+from agxclick import MessageFactory, ApplicationStepListener, update_robots_from_message, find_robots_in_scene, has_click_configuration, ClickObject, noop
+from pclick import Server, HandshakeInitMessageType, ControlMessageType, ResetMessageType, SensorRequestMessageType, ErrorMessageType
+from pclick import ControlMessage, MessageFactory as ProtoMessageFactory
 import logging
 from queue import SimpleQueue
 from enum import Enum, auto
 
-from agxClick import get_click_configuration
+from agxclick import get_click_configuration
 
 
 class States(Enum):
     INVALID = auto()
 
     RECV_HANDSHAKE = auto()
     RECV = auto()
```

### Comparing `agxclick-0.1.29/src/agxclick/click_robot.py` & `agxclick-0.1.30/src/agxclick/click_robot.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, List, Tuple, Dict
-from agxClick import BrickUtils
+from agxclick import BrickUtils
 import logging
 import itertools
-from pClick import ValueType
+from pclick import ValueType
 
 
 class ClickObject():
     def __init__(self, component):
         """
         component is a Brick.Component
         """
```

### Comparing `agxclick-0.1.29/src/agxclick/graphics_throttler.py` & `agxclick-0.1.30/src/agxclick/graphics_throttler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from agxClick.wallclock import WallClock
+from agxclick.wallclock import WallClock
 
 class GraphicsThrottler:
 
     def __init__(self, framerate: int):
         """
         If framerate is 0 or negative -> render_graphics always returns True
         """
```

### Comparing `agxclick-0.1.29/src/agxclick/keyboard_listener.py` & `agxclick-0.1.30/src/agxclick/keyboard_listener.py`

 * *Files identical despite different names*

### Comparing `agxclick-0.1.29/src/agxclick/message_factory.py` & `agxclick-0.1.30/src/agxclick/message_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import List, Any
-from agxClick import ClickRobot, BrickUtils
-from agxClick.click_robot import ClickObject
-from pClick import HandshakeMessage, SensorMessage, ValueType, MessageFactory as ProtoMessageFactory
+from agxclick import ClickRobot, BrickUtils
+from agxclick.click_robot import ClickObject
+from pclick import HandshakeMessage, SensorMessage, ValueType, MessageFactory as ProtoMessageFactory
 import math
 
 
 def _identity(x):
     return x
```

### Comparing `agxclick-0.1.29/src/agxclick/reset_batch_listener.py` & `agxclick-0.1.30/src/agxclick/reset_batch_listener.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from agxClick import ApplicationStepListener, noop
+from agxclick import ApplicationStepListener, noop
 from typing import Callable
 
 
 class ResetBatchListener(ApplicationStepListener):
     def __init__(self, scene, batch_time: float, on_batch_end: Callable[[], None] = noop) -> None:
         super().__init__()
         self._scene = scene
```

