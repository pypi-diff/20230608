# Comparing `tmp/citros-23.23.1.tar.gz` & `tmp/citros-23.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.23.1.tar", last modified: Thu Jun  8 14:53:45 2023, max compression
+gzip compressed data, was "citros-23.23.2.tar", last modified: Thu Jun  8 15:43:42 2023, max compression
```

## Comparing `citros-23.23.1.tar` & `citros-23.23.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 14:53:26.000000 citros-23.23.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 14:53:45.167378 citros-23.23.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 14:53:26.000000 citros-23.23.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-08 14:53:26.000000 citros-23.23.1/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 14:53:26.000000 citros-23.23.1/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 14:53:26.000000 citros-23.23.1/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-08 14:53:26.000000 citros-23.23.1/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 14:53:26.000000 citros-23.23.1/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 14:53:26.000000 citros-23.23.1/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 14:53:26.000000 citros-23.23.1/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 14:53:26.000000 citros-23.23.1/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 14:53:26.000000 citros-23.23.1/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 14:53:26.000000 citros-23.23.1/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 14:53:26.000000 citros-23.23.1/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:53:45.167378 citros-23.23.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 14:53:26.000000 citros-23.23.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 14:53:26.000000 citros-23.23.1/tests/test_parse_makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 14:53:26.000000 citros-23.23.1/tests/test_parse_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 14:53:26.000000 citros-23.23.1/tests/test_parse_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.808278 citros-23.23.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 15:43:23.000000 citros-23.23.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 15:43:42.808278 citros-23.23.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 15:43:23.000000 citros-23.23.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-08 15:43:23.000000 citros-23.23.2/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 15:43:23.000000 citros-23.23.2/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 15:43:23.000000 citros-23.23.2/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-08 15:43:23.000000 citros-23.23.2/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 15:43:23.000000 citros-23.23.2/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 15:43:23.000000 citros-23.23.2/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 15:43:23.000000 citros-23.23.2/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 15:43:23.000000 citros-23.23.2/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 15:43:23.000000 citros-23.23.2/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 15:43:23.000000 citros-23.23.2/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.808278 citros-23.23.2/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 15:43:23.000000 citros-23.23.2/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:43:42.808278 citros-23.23.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 15:43:23.000000 citros-23.23.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.808278 citros-23.23.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 15:43:23.000000 citros-23.23.2/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 15:43:23.000000 citros-23.23.2/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 15:43:23.000000 citros-23.23.2/tests/test_parse_xml.py
```

### Comparing `citros-23.23.1/LICENSE` & `citros-23.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/PKG-INFO` & `citros-23.23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.1
+Version: 23.23.2
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.1/README.md` & `citros-23.23.2/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/bin/citros` & `citros-23.23.2/bin/citros`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/__init__.py` & `citros-23.23.2/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/citros.py` & `citros-23.23.2/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/citros_bag.py` & `citros-23.23.2/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/citros_batch.py` & `citros-23.23.2/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/citros_events.py` & `citros-23.23.2/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/citros_integration.py` & `citros-23.23.2/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/citros_params.py` & `citros-23.23.2/citros/citros_params.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import yaml
 import json
 import os
 import numpy as np
 from pathlib import Path
 from decouple import config
-from ament_index_python.packages import get_package_share_directory
 
 
 class citros_params():
     def __init__(self, citros):
         self.citros = citros
         self.log = citros.log
         self.CONFIG_FOLDER = config("CONFIG_FOLDER", 'tmp/config')
@@ -134,15 +133,18 @@
                     paramValue = paramValues.get(str(parameter["id"]))
                     if paramValue:
                         value = paramValue
                     config[package["name"]][node["name"]]["ros__parameters"][parameter['name']] = value                                                             
         return config   
     
 
-    def save_config(self, config):     
+    def save_config(self, config):  
+        # callback running inside ROS workspace context.   
+        from ament_index_python.packages import get_package_share_directory
+
         Path(self.CONFIG_FOLDER).mkdir(exist_ok=True, parents=True)
                 
         for package_name, citros_config in config.items():     
             self.log.debug(f"Saving config for [{package_name}]")
 
             # TODO: add other method to get the package path
             path_to_package = None
```

### Comparing `citros-23.23.1/citros/citros_utils.py` & `citros-23.23.2/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/launches/__init__.py` & `citros-23.23.2/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/launches/launch.py` & `citros-23.23.2/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/logger/__init__.py` & `citros-23.23.2/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/logger/logger.py` & `citros-23.23.2/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/logger/logger_pg_handler.py` & `citros-23.23.2/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/parsers/__init__.py` & `citros-23.23.2/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/parsers/parser_ros2.py` & `citros-23.23.2/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/rosbag/__init__.py` & `citros-23.23.2/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/rosbag/reader_base.py` & `citros-23.23.2/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/rosbag/reader_mcap.py` & `citros-23.23.2/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros/rosbag/reader_sqlite.py` & `citros-23.23.2/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/citros.egg-info/PKG-INFO` & `citros-23.23.2/citros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.1
+Version: 23.23.2
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.1/citros.egg-info/SOURCES.txt` & `citros-23.23.2/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/setup.py` & `citros-23.23.2/setup.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/tests/test_parse_makefile.py` & `citros-23.23.2/tests/test_parse_makefile.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/tests/test_parse_setup_py.py` & `citros-23.23.2/tests/test_parse_setup_py.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.1/tests/test_parse_xml.py` & `citros-23.23.2/tests/test_parse_xml.py`

 * *Files identical despite different names*

