# Comparing `tmp/citros-23.23.3.tar.gz` & `tmp/citros-23.23.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.23.3.tar", last modified: Thu Jun  8 16:06:56 2023, max compression
+gzip compressed data, was "citros-23.23.4.tar", last modified: Thu Jun  8 16:17:26 2023, max compression
```

## Comparing `citros-23.23.3.tar` & `citros-23.23.4.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 16:06:41.000000 citros-23.23.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 16:06:56.751634 citros-23.23.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 16:06:41.000000 citros-23.23.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.747634 citros-23.23.3/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-08 16:06:41.000000 citros-23.23.3/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.747634 citros-23.23.3/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 16:06:41.000000 citros-23.23.3/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 16:06:41.000000 citros-23.23.3/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-08 16:06:41.000000 citros-23.23.3/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 16:06:41.000000 citros-23.23.3/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 16:06:41.000000 citros-23.23.3/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 16:06:41.000000 citros-23.23.3/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 16:06:41.000000 citros-23.23.3/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 16:06:41.000000 citros-23.23.3/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 16:06:41.000000 citros-23.23.3/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.747634 citros-23.23.3/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 16:06:41.000000 citros-23.23.3/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:06:56.751634 citros-23.23.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 16:06:41.000000 citros-23.23.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 16:06:41.000000 citros-23.23.3/tests/test_parse_makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 16:06:41.000000 citros-23.23.3/tests/test_parse_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 16:06:41.000000 citros-23.23.3/tests/test_parse_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.787917 citros-23.23.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 16:17:09.000000 citros-23.23.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 16:17:26.787917 citros-23.23.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 16:17:09.000000 citros-23.23.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.783916 citros-23.23.4/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-08 16:17:09.000000 citros-23.23.4/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.783916 citros-23.23.4/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 16:17:09.000000 citros-23.23.4/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 16:17:09.000000 citros-23.23.4/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.783916 citros-23.23.4/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 16:17:09.000000 citros-23.23.4/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12271 2023-06-08 16:17:09.000000 citros-23.23.4/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.787917 citros-23.23.4/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 16:17:09.000000 citros-23.23.4/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 16:17:09.000000 citros-23.23.4/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 16:17:09.000000 citros-23.23.4/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.787917 citros-23.23.4/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 16:17:09.000000 citros-23.23.4/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 16:17:09.000000 citros-23.23.4/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 16:17:09.000000 citros-23.23.4/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.787917 citros-23.23.4/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 16:17:09.000000 citros-23.23.4/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 16:17:09.000000 citros-23.23.4/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 16:17:09.000000 citros-23.23.4/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 16:17:09.000000 citros-23.23.4/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.783916 citros-23.23.4/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 16:17:26.000000 citros-23.23.4/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 16:17:26.000000 citros-23.23.4/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:17:26.000000 citros-23.23.4/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 16:17:26.000000 citros-23.23.4/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 16:17:26.000000 citros-23.23.4/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 16:17:09.000000 citros-23.23.4/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:17:26.787917 citros-23.23.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 16:17:09.000000 citros-23.23.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:17:26.787917 citros-23.23.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 16:17:09.000000 citros-23.23.4/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 16:17:09.000000 citros-23.23.4/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 16:17:09.000000 citros-23.23.4/tests/test_parse_xml.py
```

### Comparing `citros-23.23.3/LICENSE` & `citros-23.23.4/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/PKG-INFO` & `citros-23.23.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.3
+Version: 23.23.4
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.3/README.md` & `citros-23.23.4/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/bin/citros` & `citros-23.23.4/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/__init__.py` & `citros-23.23.4/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros.py` & `citros-23.23.4/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros_bag.py` & `citros-23.23.4/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros_batch.py` & `citros-23.23.4/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros_events.py` & `citros-23.23.4/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros_integration.py` & `citros-23.23.4/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros_params.py` & `citros-23.23.4/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/citros_utils.py` & `citros-23.23.4/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/launches/__init__.py` & `citros-23.23.4/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/launches/launch.py` & `citros-23.23.4/citros/launches/launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,12 @@
 import os
 import shutil
 from datetime import datetime
 from typing import cast
-from ament_index_python.packages import get_package_share_directory
-from launch import LaunchDescription, Event
-from launch.actions import EmitEvent, ExecuteProcess, IncludeLaunchDescription, DeclareLaunchArgument, OpaqueFunction, RegisterEventHandler, LogInfo, TimerAction
-from launch.launch_description_sources import PythonLaunchDescriptionSource
-from launch_ros.actions import Node
-from launch.substitutions import LaunchConfiguration, LocalSubstitution, TextSubstitution
-from launch.event_handlers import (OnExecutionComplete, OnProcessExit,
-                                OnProcessIO, OnProcessStart, OnShutdown)
-from launch.events import Shutdown, process
-from launch.actions import SetLaunchConfiguration
+
 from citros import Citros
 
 ################################
 # Entrypoint        
 ################################
 def generate_launch_description(citros : Citros, timeout):
     """
@@ -24,14 +15,26 @@
     Args:
         citros (Citros): An instance of Citros class which manages interaction with the CiTROS service.
         timeout (int): The time limit for the simulation run.
 
     Returns:
         launch.LaunchDescription: A launch description that ROS2 can execute.
     """
+    # running inside ROS workspace context.  
+    from ament_index_python.packages import get_package_share_directory
+    from launch import LaunchDescription, Event
+    from launch.actions import EmitEvent, ExecuteProcess, IncludeLaunchDescription, DeclareLaunchArgument, OpaqueFunction, RegisterEventHandler, LogInfo, TimerAction
+    from launch.launch_description_sources import PythonLaunchDescriptionSource
+    from launch_ros.actions import Node
+    from launch.substitutions import LaunchConfiguration, LocalSubstitution, TextSubstitution
+    from launch.event_handlers import (OnExecutionComplete, OnProcessExit,
+                                    OnProcessIO, OnProcessStart, OnShutdown)
+    from launch.events import Shutdown, process
+    from launch.actions import SetLaunchConfiguration
+
     batch_run_id = str(citros.batch_run_id)    
     simulation_run_id = str(citros.simulation_run_id)    
     timeout = str(timeout)    
     
     citros.log.debug("+ generate_launch_description()")
     citros.log.debug(f"batch_run_id: {batch_run_id}")
     citros.log.debug(f"simulation_run_id: {simulation_run_id}")
```

### Comparing `citros-23.23.3/citros/logger/__init__.py` & `citros-23.23.4/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/logger/logger.py` & `citros-23.23.4/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/logger/logger_pg_handler.py` & `citros-23.23.4/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/parsers/__init__.py` & `citros-23.23.4/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/parsers/parser_ros2.py` & `citros-23.23.4/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/rosbag/__init__.py` & `citros-23.23.4/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/rosbag/reader_base.py` & `citros-23.23.4/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/rosbag/reader_mcap.py` & `citros-23.23.4/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros/rosbag/reader_sqlite.py` & `citros-23.23.4/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/citros.egg-info/PKG-INFO` & `citros-23.23.4/citros.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.3
+Version: 23.23.4
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.3/citros.egg-info/SOURCES.txt` & `citros-23.23.4/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/setup.py` & `citros-23.23.4/setup.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/tests/test_parse_makefile.py` & `citros-23.23.4/tests/test_parse_makefile.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/tests/test_parse_setup_py.py` & `citros-23.23.4/tests/test_parse_setup_py.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.3/tests/test_parse_xml.py` & `citros-23.23.4/tests/test_parse_xml.py`

 * *Files identical despite different names*

