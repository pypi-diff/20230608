# Comparing `tmp/osef-2.8.0.tar.gz` & `tmp/osef-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osef-2.8.0.tar", last modified: Thu Mar  9 13:17:03 2023, max compression
+gzip compressed data, was "osef-2.8.1.tar", last modified: Thu Jun  8 13:59:12 2023, max compression
```

## Comparing `osef-2.8.0.tar` & `osef-2.8.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:17:03.023094 osef-2.8.0/
--rw-rw-rw-   0 root         (0) root         (0)     1064 2023-02-22 15:05:39.000000 osef-2.8.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-09 13:17:03.023094 osef-2.8.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2882 2023-02-22 15:05:39.000000 osef-2.8.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:17:03.019094 osef-2.8.0/osef/
--rw-rw-rw-   0 root         (0) root         (0)      381 2023-02-22 15:05:39.000000 osef-2.8.0/osef/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-02-22 15:05:39.000000 osef-2.8.0/osef/_logger.py
--rw-rw-rw-   0 root         (0) root         (0)     3064 2023-02-22 15:05:39.000000 osef-2.8.0/osef/_packers.py
--rw-rw-rw-   0 root         (0) root         (0)     5155 2023-02-22 15:05:39.000000 osef-2.8.0/osef/_unpackers.py
--rw-rw-rw-   0 root         (0) root         (0)      173 2023-02-22 15:05:39.000000 osef-2.8.0/osef/_version.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-02-22 15:05:39.000000 osef-2.8.0/osef/constants.py
--rw-rw-rw-   0 root         (0) root         (0)     9950 2023-02-22 15:05:39.000000 osef-2.8.0/osef/multi_streamer.py
--rw-rw-rw-   0 root         (0) root         (0)    23874 2023-02-22 15:05:39.000000 osef-2.8.0/osef/osef_frame.py
--rw-rw-rw-   0 root         (0) root         (0)    46589 2023-03-08 14:42:34.000000 osef-2.8.0/osef/osef_types.py
--rw-rw-rw-   0 root         (0) root         (0)     2973 2023-02-22 15:05:39.000000 osef-2.8.0/osef/packer.py
--rwxrwxrwx   0 root         (0) root         (0)    11795 2023-02-22 15:05:39.000000 osef-2.8.0/osef/parser.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2023-02-22 15:05:39.000000 osef-2.8.0/osef/precise_timer.py
--rw-rw-rw-   0 root         (0) root         (0)     1689 2023-02-22 15:05:39.000000 osef-2.8.0/osef/saver.py
--rw-rw-rw-   0 root         (0) root         (0)     2546 2023-02-22 15:05:39.000000 osef-2.8.0/osef/scanner.py
--rw-rw-rw-   0 root         (0) root         (0)     2387 2023-02-22 15:05:39.000000 osef-2.8.0/osef/streamer.py
--rw-rw-rw-   0 root         (0) root         (0)    20992 2023-03-08 14:42:34.000000 osef-2.8.0/osef/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:17:03.023094 osef-2.8.0/osef.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3259 2023-03-09 13:17:03.000000 osef-2.8.0/osef.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      633 2023-03-09 13:17:03.000000 osef-2.8.0/osef.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-09 13:17:03.000000 osef-2.8.0/osef.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-09 13:17:03.000000 osef-2.8.0/osef.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-09 13:17:03.000000 osef-2.8.0/osef.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      103 2023-02-22 15:05:39.000000 osef-2.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-09 13:17:03.023094 osef-2.8.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      798 2023-02-22 15:05:39.000000 osef-2.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-09 13:17:03.023094 osef-2.8.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)    15933 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_frame.py
--rw-rw-rw-   0 root         (0) root         (0)     2340 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_packer.py
--rw-rw-rw-   0 root         (0) root         (0)     3394 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_parser.py
--rw-rw-rw-   0 root         (0) root         (0)      581 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_private_types.py
--rw-rw-rw-   0 root         (0) root         (0)     1604 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_scanner.py
--rw-rw-rw-   0 root         (0) root         (0)     2730 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_streamer.py
--rw-rw-rw-   0 root         (0) root         (0)     3070 2023-02-22 15:05:39.000000 osef-2.8.0/tests/test_types.py
--rw-rw-rw-   0 root         (0) root         (0)     3556 2023-03-08 14:42:34.000000 osef-2.8.0/tests/tests_base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:59:12.512502 osef-2.8.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1064 2023-06-08 13:59:00.000000 osef-2.8.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-08 13:59:12.512502 osef-2.8.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2882 2023-06-08 13:59:00.000000 osef-2.8.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:59:12.512502 osef-2.8.1/osef/
+-rw-rw-rw-   0 root         (0) root         (0)      381 2023-06-08 13:59:00.000000 osef-2.8.1/osef/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      128 2023-06-08 13:59:00.000000 osef-2.8.1/osef/_logger.py
+-rw-rw-rw-   0 root         (0) root         (0)     3036 2023-06-08 13:59:00.000000 osef-2.8.1/osef/_packers.py
+-rw-rw-rw-   0 root         (0) root         (0)     5155 2023-06-08 13:59:00.000000 osef-2.8.1/osef/_unpackers.py
+-rw-rw-rw-   0 root         (0) root         (0)      173 2023-06-08 13:59:00.000000 osef-2.8.1/osef/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-06-08 13:59:00.000000 osef-2.8.1/osef/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)     9950 2023-06-08 13:59:00.000000 osef-2.8.1/osef/multi_streamer.py
+-rw-rw-rw-   0 root         (0) root         (0)    23874 2023-06-08 13:59:00.000000 osef-2.8.1/osef/osef_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)    46592 2023-06-08 13:59:00.000000 osef-2.8.1/osef/osef_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     2973 2023-06-08 13:59:00.000000 osef-2.8.1/osef/packer.py
+-rwxrwxrwx   0 root         (0) root         (0)    11816 2023-06-08 13:59:00.000000 osef-2.8.1/osef/parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2023-06-08 13:59:00.000000 osef-2.8.1/osef/precise_timer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1689 2023-06-08 13:59:00.000000 osef-2.8.1/osef/saver.py
+-rw-rw-rw-   0 root         (0) root         (0)     2546 2023-06-08 13:59:00.000000 osef-2.8.1/osef/scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2387 2023-06-08 13:59:00.000000 osef-2.8.1/osef/streamer.py
+-rw-rw-rw-   0 root         (0) root         (0)    20992 2023-06-08 13:59:00.000000 osef-2.8.1/osef/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:59:12.512502 osef-2.8.1/osef.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3259 2023-06-08 13:59:12.000000 osef-2.8.1/osef.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      633 2023-06-08 13:59:12.000000 osef-2.8.1/osef.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 13:59:12.000000 osef-2.8.1/osef.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-08 13:59:12.000000 osef-2.8.1/osef.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-08 13:59:12.000000 osef-2.8.1/osef.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      103 2023-06-08 13:59:00.000000 osef-2.8.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 13:59:12.512502 osef-2.8.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      798 2023-06-08 13:59:00.000000 osef-2.8.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 13:59:12.512502 osef-2.8.1/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    15933 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)     2340 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_packer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3394 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)      581 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_private_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     1604 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_scanner.py
+-rw-rw-rw-   0 root         (0) root         (0)     2730 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_streamer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3070 2023-06-08 13:59:00.000000 osef-2.8.1/tests/test_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3556 2023-06-08 13:59:00.000000 osef-2.8.1/tests/tests_base.py
```

### Comparing `osef-2.8.0/LICENSE` & `osef-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/PKG-INFO` & `osef-2.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osef
-Version: 2.8.0
+Version: 2.8.1
 Summary: Osef file/stream tools.
 Author: Outsight Developers
 Author-email: support@outsight.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `osef-2.8.0/README.md` & `osef-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/_packers.py` & `osef-2.8.1/osef/_packers.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,17 +52,17 @@
     """Values to parse: tx ty tz Vxx Vyx Vzx Vxy Vyy Vzy Vxz Vyz Vzz
 
     Where rotation matrices should be at the end:
         | Vxx Vxy Vxz |
     R = | Vyx Vyy Vyz |
         | Vzx Vzy Vzz |
     """
-    translation = value["translation"]
-    rotation = np.ravel(value["rotation"].transpose())
-    t_r = np.hstack((translation, rotation)).astype(np.float32)
+    t_r = np.zeros(12, dtype=np.float32)
+    t_r[:3] = value["translation"]
+    t_r[3:] = value["rotation"].transpose().flatten()
     return t_r.tobytes()
 
 
 def _pose_array_packer(value: List) -> bytes:
     if len(value) == 0:
         return np.array([]).tobytes()
     out = bytes()
```

### Comparing `osef-2.8.0/osef/_unpackers.py` & `osef-2.8.1/osef/_unpackers.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/constants.py` & `osef-2.8.1/osef/constants.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/multi_streamer.py` & `osef-2.8.1/osef/multi_streamer.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/osef_frame.py` & `osef-2.8.1/osef/osef_frame.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/osef_types.py` & `osef-2.8.1/osef/osef_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """OSEF private types definition."""
-__version__ = "1.11.0"
+__version__ = "1.11.1"
 
 # Standard imports
 from enum import Enum, IntEnum
 
 # !!! Warning !!!
 # !!! This file has been auto generated, do not attempt to edit it !!!
 # Important: all words use little-endian representation, unless specified otherwise
@@ -149,15 +149,15 @@
     * distance : meters, range [ 0.0 ..  +inf ]
     """
     SPHERICAL_COORDINATES = "spherical_coordinates"
 
     """
     Reflectivities
     **Output when**: Augmented Cloud is enabled.
-    **Format**: list of unsigned 8-bits integers.
+    **Format**: List of unsigned 8-bits integers.
     **Purpose**: Contains list of reflectivity values.
     Diffuse reflectors report values from 0 to 100 for reflectivities from 0% to 100%.
     Retroreflectors report values from 101 to 255, where 255 represents an ideal reflection.
     """
     REFLECTIVITIES = "reflectivities"
 
     """
@@ -216,15 +216,15 @@
     """
     _IMAGE_DIMENSION = "image_dimension"
 
     """
     Number of Objects
     **Output when**: Tracking is enabled.
     **Purpose**: Number of tracked objects.
-    **Format**: unsigned 32-bits integer, range [ 0 .. 2^32 [
+    **Format**: Unsigned 32-bits integer, range [ 0 .. 2^32 [
     """
     NUMBER_OF_OBJECTS = "number_of_objects"
 
     """
     Cloud Frame
     Contains following sub-TLVs:
     - exactly one:     Augmented Cloud                (AUGMENTED_CLOUD)
@@ -287,15 +287,15 @@
     * y_max : percentage of the image size, 32-bits floating-point, range [ 0 .. 1 ]
     """
     _BOUNDING_BOXES_ARRAY = "bounding_boxes_array"
 
     """
     Class ID Array
     **Output when**: Tracking is enabled.
-    **Format**: list of signed 32 bits integers, using enum CLASS ID.
+    **Format**: List of signed 32 bits integers, using enum CLASS ID.
     **Purpose**: Contains list of class IDs. For further details, see:
     [Classification](https://docs.outsight.ai/software/understanding-osef-data/object-tracking-data#classification)
     """
     CLASS_ID_ARRAY = "class_id_array"
 
     """
     Confidence Array
@@ -552,17 +552,17 @@
     * Byte [0,3]: UNIX time in seconds,   unsigned 32-bits integer, range [ 0 .. 2^32 [
     * Byte [4,7]: remaining microseconds, unsigned 32-bits integer, range [ 0 .. 1000000 [
     * Acceleration vector
     * Byte [8,11] x : meters / second^2, 32 bits float, range [ -inf .. +inf ]
     * Byte [12,15] y : meters / second^2, 32 bits float, range [ -inf .. +inf ]
     * Byte [16,19] z : meters / second^2, 32 bits float, range [ -inf .. +inf ]
     * Angular velocity vector
-    * Byte [20,23] x : degrees / second, 32 bits float, range [ -inf .. +inf ]
-    * Byte [24,27] x : degrees / second, 32 bits float, range [ -inf .. +inf ]
-    * Byte [28,31] x : degrees / second, 32 bits float, range [ -inf .. +inf ]
+    * Byte [20,23] x : radians / second, 32 bits float, range [ -inf .. +inf ]
+    * Byte [24,27] x : radians / second, 32 bits float, range [ -inf .. +inf ]
+    * Byte [28,31] x : radians / second, 32 bits float, range [ -inf .. +inf ]
     """
     _IMU_PACKET = "imu_packet"
 
     """
     Timestamp Lidar Velodyne
     Describes a timestamp with microsecond precision. This timestamp is in the lidar reference system, and uses the
     Velodyne format. This means that this timestamp is the time spent since the beginning of the hour.
@@ -648,15 +648,15 @@
 
     """
     Object ID 32 Bits
     **Output when**: Tracking is enabled.
     **Format**: Array of unsigned 32-bits integers. Each element of the array is an Object ID.
     **Purpose**: Give a unique identifier (ID) to each detected object.
     Optionally, this ID can also be used to establish a link between detected objects
-    and the defined Zones, or the points of a Augmented Cloud.
+    and the defined Zones, or the points from an Augmented Cloud.
     When used as leaf of Tracked Objects:
     - The number of elements of the array is equal to the Number of Objects (type 10).
     - Each ID represents a distinct detected object.
     - The affectation of an ID to an object is arbitrary and permanent,
       it remains the same throughout the tracking phase.
     When used as leaf of Augmented Cloud:
     - The number of elements of the array is equal to the Number of Points (type 2).
@@ -805,15 +805,15 @@
     A Response made by a device.
     """
     _INTERACTIVE_RESPONSE = "interactive_response"
 
     """
     Interactive Request ID
     An ID to identify to which request is associated the response.
-    **Format**: unsigned 32-bits integer.
+    **Format**: Unsigned 32-bits integer.
     """
     _INTERACTIVE_REQUEST_ID = "interactive_request_id"
 
     """
     Interactive Request Background Header
     Request background header.
     """
@@ -836,15 +836,15 @@
     Response background data.
     """
     _INTERACTIVE_RESPONSE_BACKGROUND_DATA = "interactive_response_background_data"
 
     """
     Interactive Request PingPong
     Request pingpong.
-    **Format**: binary payload
+    **Format**: Binary payload
     """
     _INTERACTIVE_REQUEST_PINGPONG = "interactive_request_pingpong"
 
     """
     Interactive Response PingPong
     Response pingpong.
     **Format**: The same binary payload as in the request
@@ -890,68 +890,68 @@
     - 1 means SLAM algorithm seems to have diverged, the associated pose is not trustworthy.
     """
     DIVERGENCE_INDICATOR = "divergence_indicator"
 
     """
     Carla Tag Array
     **Output when**: generated by Carla Scenario Generator.
-    **Format**: list of unsigned 8-bits integers, using enum Carla Tag enum.
-    **Purpose**: keeps the tag value, attributed by the Carla Simulator, to each point of the pointcloud.
+    **Format**: List of unsigned 8-bits integers, using enum Carla Tag enum.
+    **Purpose**: keeps the tag value, attributed by the Carla Simulator, to each point of the point cloud.
     """
     _CARLA_TAG_ARRAY = "carla_tag_array"
 
     """
     Background Scene Params
     **Output when**: Multi-LiDARS Tracking is enabled, in the background stream between edge and fusion.
     **Purpose**: All params to initialize the background scene and be able to interpret Background Stream Fragment
     (type 76) packets
     """
     _BACKGROUND_SCENE_PARAMS = "background_scene_params"
 
     """
     Background Scene Params General
     **Output when**: Multi-LiDARS Tracking is enabled, in the background stream between edge and fusion.
-    **Format**: the following concatenated values:
+    **Format**: The following concatenated values:
       * width: 32-bits unsigned integer, number of columns of the background scene array
       * height: 32-bits unsigned integer, number of rows of the background scene array
       * first azimuth: single-precision float, azimuth of the first column of the background scene array, in degrees
       * azimuth step: single-precision float, difference between the azimuths of two consecutive columns of the
     background scene array, in degrees
     """
     _BACKGROUND_SCENE_PARAMS_GENERAL = "background_scene_params_general"
 
     """
     Background Scene Params Elevations
     **Output when**: generated by Carla Scenario Generator.
-    **Format**: list of single precision floats, each one representing the elevation of a row in the background scene
+    **Format**: List of single precision floats, each one representing the elevation of a row in the background scene
     array, in degrees
     """
     _BACKGROUND_SCENE_PARAMS_ELEVATIONS = "background_scene_params_elevations"
 
     """
     Background Scene Fragment
     **Output when**: Multi-LiDARS Tracking is enabled, in the background stream between edge and fusion.
     **Purpose**: A fragment of the background scene array
     """
     _BACKGROUND_SCENE_FRAGMENT = "background_scene_fragment"
 
     """
     Background Scene Fragment Info
     **Output when**: in background stream between edge and fusion, in tracking mode
-    **Format**: the following concatenated values:
+    **Format**: The following concatenated values:
       * first_index: 32-bites unsigned integer, index of the first cell in background scene array, computed as x *
     height + y, the second cell index is first_index+1, etc., with a rollover on width * height
       * cells_number: 32-bites unsigned integer, number of cells contained in the fragment
     """
     _BACKGROUND_SCENE_FRAGMENT_INFO = "background_scene_fragment_info"
 
     """
     Background Scene Fragment Distances
     **Output when**: Multi-LiDARS Tracking is enabled, in the background stream between edge and fusion.
-    **Format**: list of single precision floats, each one representing the farthest background distance for the
+    **Format**: List of single precision floats, each one representing the farthest background distance for the
     corresponding cell
     """
     _BACKGROUND_SCENE_FRAGMENT_DISTANCES = "background_scene_fragment_distances"
 
     """
     Geographic Pose Array
     **Output when**: Tracking is enabled and georeferencing is activated.
@@ -1021,15 +1021,15 @@
     """
     _FILTERED_ROTATION_SPEED = "filtered_rotation_speed"
 
     """
     Reference Map Bits
     **Output when**: SLAM is enabled and its mapping module is enabled.
     **Purpose**: SLAM identifies potential points of interest within the point cloud, and the mapping module selects
-    some of them to build the map. Theses bits identify the points that are selected to generate the output map.
+    some of them to build the map. These bits identify the points that are selected to generate the output map.
     **Format**: Padded list of bits, 1 bit per point of the cloud. If the bit is set, the point is part of the
     reference map.
     """
     REFERENCE_MAP_BITS = "reference_map_bits"
 
     """
     Cartesian covariance
```

### Comparing `osef-2.8.0/osef/packer.py` & `osef-2.8.1/osef/packer.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/parser.py` & `osef-2.8.1/osef/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import time
 import traceback
 from collections import deque
 from itertools import islice
 from struct import Struct
 from typing import Any, Iterable, Optional, Tuple, Iterator, Union
 from urllib.parse import urlparse
+import errno
 
 from osef import types
 from osef._logger import osef_logger
 from osef.constants import _Tlv, _TreeNode, _STRUCT_FORMAT
 from osef import precise_timer
 from osef.osef_types import OsefKeys
 
@@ -67,21 +68,21 @@
 
         return self._io_stream.read(size)
 
     def open_socket(self, auto_reconnect: bool = True):
         """Open tcp socket on provided path.
         Tries to connect again if the connection fails
         """
-        tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
 
         # Count the retries, to avoid flooding the log
         retry = 0
 
         while True:
             try:
+                tcp_socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
                 tcp_socket.settimeout(TCP_TIMEOUT)
                 tcp_socket.connect(
                     (self._parsed_path.hostname, self._parsed_path.port or 11120)
                 )
                 osef_logger.warning(
                     "Connected to %s:%d",
                     self._parsed_path.hostname,
```

### Comparing `osef-2.8.0/osef/saver.py` & `osef-2.8.1/osef/saver.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/scanner.py` & `osef-2.8.1/osef/scanner.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/streamer.py` & `osef-2.8.1/osef/streamer.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef/types.py` & `osef-2.8.1/osef/types.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/osef.egg-info/PKG-INFO` & `osef-2.8.1/osef.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osef
-Version: 2.8.0
+Version: 2.8.1
 Summary: Osef file/stream tools.
 Author: Outsight Developers
 Author-email: support@outsight.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `osef-2.8.0/osef.egg-info/SOURCES.txt` & `osef-2.8.1/osef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/setup.py` & `osef-2.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_frame.py` & `osef-2.8.1/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_packer.py` & `osef-2.8.1/tests/test_packer.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_parser.py` & `osef-2.8.1/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_private_types.py` & `osef-2.8.1/tests/test_private_types.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_scanner.py` & `osef-2.8.1/tests/test_scanner.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_streamer.py` & `osef-2.8.1/tests/test_streamer.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/test_types.py` & `osef-2.8.1/tests/test_types.py`

 * *Files identical despite different names*

### Comparing `osef-2.8.0/tests/tests_base.py` & `osef-2.8.1/tests/tests_base.py`

 * *Files identical despite different names*

