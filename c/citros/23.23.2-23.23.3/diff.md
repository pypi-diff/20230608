# Comparing `tmp/citros-23.23.2.tar.gz` & `tmp/citros-23.23.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.23.2.tar", last modified: Thu Jun  8 15:43:42 2023, max compression
+gzip compressed data, was "citros-23.23.3.tar", last modified: Thu Jun  8 16:06:56 2023, max compression
```

## Comparing `citros-23.23.2.tar` & `citros-23.23.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.808278 citros-23.23.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 15:43:23.000000 citros-23.23.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 15:43:42.808278 citros-23.23.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 15:43:23.000000 citros-23.23.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-08 15:43:23.000000 citros-23.23.2/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 15:43:23.000000 citros-23.23.2/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 15:43:23.000000 citros-23.23.2/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 15:43:23.000000 citros-23.23.2/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-08 15:43:23.000000 citros-23.23.2/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 15:43:23.000000 citros-23.23.2/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 15:43:23.000000 citros-23.23.2/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 15:43:23.000000 citros-23.23.2/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 15:43:23.000000 citros-23.23.2/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 15:43:23.000000 citros-23.23.2/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 15:43:23.000000 citros-23.23.2/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.808278 citros-23.23.2/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 15:43:23.000000 citros-23.23.2/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.804278 citros-23.23.2/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 15:43:42.000000 citros-23.23.2/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 15:43:23.000000 citros-23.23.2/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:43:42.808278 citros-23.23.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 15:43:23.000000 citros-23.23.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:43:42.808278 citros-23.23.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 15:43:23.000000 citros-23.23.2/tests/test_parse_makefile.py
--rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 15:43:23.000000 citros-23.23.2/tests/test_parse_setup_py.py
--rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 15:43:23.000000 citros-23.23.2/tests/test_parse_xml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 16:06:41.000000 citros-23.23.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 16:06:56.751634 citros-23.23.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 16:06:41.000000 citros-23.23.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.747634 citros-23.23.3/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17385 2023-06-08 16:06:41.000000 citros-23.23.3/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.747634 citros-23.23.3/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 16:06:41.000000 citros-23.23.3/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8429 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 16:06:41.000000 citros-23.23.3/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 16:06:41.000000 citros-23.23.3/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-08 16:06:41.000000 citros-23.23.3/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 16:06:41.000000 citros-23.23.3/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 16:06:41.000000 citros-23.23.3/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 16:06:41.000000 citros-23.23.3/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 16:06:41.000000 citros-23.23.3/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 16:06:41.000000 citros-23.23.3/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 16:06:41.000000 citros-23.23.3/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 16:06:41.000000 citros-23.23.3/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.747634 citros-23.23.3/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 16:06:56.000000 citros-23.23.3/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 16:06:41.000000 citros-23.23.3/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:06:56.751634 citros-23.23.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 16:06:41.000000 citros-23.23.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:06:56.751634 citros-23.23.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 16:06:41.000000 citros-23.23.3/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 16:06:41.000000 citros-23.23.3/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 16:06:41.000000 citros-23.23.3/tests/test_parse_xml.py
```

### Comparing `citros-23.23.2/LICENSE` & `citros-23.23.3/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/PKG-INFO` & `citros-23.23.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.2
+Version: 23.23.3
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.2/README.md` & `citros-23.23.3/README.md`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/bin/citros` & `citros-23.23.3/bin/citros`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 import sys        
 import traceback
 from decouple import config
 
 from InquirerPy import prompt
 from prompt_toolkit.validation import Validator, ValidationError
 
-from launch import LaunchService 
 from citros.launches import generate_launch_description  
 
 # in seconds
 DEFAULT_SIMULATION_TIMEOUT = 10*60
 
 
 class NumberValidator(Validator):
@@ -212,15 +211,18 @@
             print (e)
             traceback.print_exc()
             print("------------------------")
             continue
     print(f" - Finished [{batch_run_id}] batch.")    
 
 
-def single_simulation_run(batch_id, sid, timeout):    
+def single_simulation_run(batch_id, sid, timeout):   
+    # running inside ROS workspace context.  
+    from launch import LaunchService 
+
     print(f" + + running simulation [{sid}]")  
     
     # create a new instance of citros so that a new logger will be created 
     # and mapped according to batch_id, simulation_run_id. Very inelegant.
     # TODO: find a simple way to map the loggers without instantiating Citros. 
     with Citros(batch_id, sid) as citros:
         launch_description = generate_launch_description(citros, str(timeout))
```

### Comparing `citros-23.23.2/citros/__init__.py` & `citros-23.23.3/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros.py` & `citros-23.23.3/citros/citros.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros_bag.py` & `citros-23.23.3/citros/citros_bag.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros_batch.py` & `citros-23.23.3/citros/citros_batch.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros_events.py` & `citros-23.23.3/citros/citros_events.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros_integration.py` & `citros-23.23.3/citros/citros_integration.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros_params.py` & `citros-23.23.3/citros/citros_params.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/citros_utils.py` & `citros-23.23.3/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/launches/__init__.py` & `citros-23.23.3/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/launches/launch.py` & `citros-23.23.3/citros/launches/launch.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/logger/__init__.py` & `citros-23.23.3/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/logger/logger.py` & `citros-23.23.3/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/logger/logger_pg_handler.py` & `citros-23.23.3/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/parsers/__init__.py` & `citros-23.23.3/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/parsers/parser_ros2.py` & `citros-23.23.3/citros/parsers/parser_ros2.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/rosbag/__init__.py` & `citros-23.23.3/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/rosbag/reader_base.py` & `citros-23.23.3/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/rosbag/reader_mcap.py` & `citros-23.23.3/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros/rosbag/reader_sqlite.py` & `citros-23.23.3/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/citros.egg-info/PKG-INFO` & `citros-23.23.3/citros.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.23.2
+Version: 23.23.3
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `citros-23.23.2/citros.egg-info/SOURCES.txt` & `citros-23.23.3/citros.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/setup.py` & `citros-23.23.3/setup.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/tests/test_parse_makefile.py` & `citros-23.23.3/tests/test_parse_makefile.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/tests/test_parse_setup_py.py` & `citros-23.23.3/tests/test_parse_setup_py.py`

 * *Files identical despite different names*

### Comparing `citros-23.23.2/tests/test_parse_xml.py` & `citros-23.23.3/tests/test_parse_xml.py`

 * *Files identical despite different names*

