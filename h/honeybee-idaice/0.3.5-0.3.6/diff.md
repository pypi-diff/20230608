# Comparing `tmp/honeybee-idaice-0.3.5.tar.gz` & `tmp/honeybee-idaice-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/honeybee-idaice-0.3.5.tar", last modified: Thu Jun  1 20:50:21 2023, max compression
+gzip compressed data, was "dist/honeybee-idaice-0.3.6.tar", last modified: Thu Jun  8 20:30:55 2023, max compression
```

## Comparing `honeybee-idaice-0.3.5.tar` & `honeybee-idaice-0.3.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/_extend_honeybee.py
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/archive.py
--rw-r--r--   0 runner    (1001) docker     (123)    10534 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/bldgbody.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/cli/translate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/face.py
--rw-r--r--   0 runner    (1001) docker     (123)     4896 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/geometry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/shade.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/
--rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/ahu.idc
--rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/ahu.idm
--rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/building.idm
--rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/plant.idc
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/plant.idm
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/templates/room.idm
--rw-r--r--   0 runner    (1001) docker     (123)    11033 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/honeybee_idaice/writer_obj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/honeybee_idaice.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 20:50:21.000000 honeybee-idaice-0.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-01 20:48:56.000000 honeybee-idaice-0.3.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/_extend_honeybee.py
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/archive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/bldgbody.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/cli/translate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/face.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9028 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/geometry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4672 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/shade.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)    10761 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/ahu.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     6144 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/ahu.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    20327 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/building.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    13552 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/plant.idc
+-rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/plant.idm
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/templates/room.idm
+-rw-r--r--   0 runner    (1001) docker     (123)    11427 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4506 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/honeybee_idaice/writer_obj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/honeybee_idaice.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 20:30:55.000000 honeybee-idaice-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-08 20:29:45.000000 honeybee-idaice-0.3.6/setup.py
```

### Comparing `honeybee-idaice-0.3.5/LICENSE` & `honeybee-idaice-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/PKG-INFO` & `honeybee-idaice-0.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.5
+Version: 0.3.6
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.5/README.md` & `honeybee-idaice-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/archive.py` & `honeybee-idaice-0.3.6/honeybee_idaice/archive.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/bldgbody.py` & `honeybee-idaice-0.3.6/honeybee_idaice/bldgbody.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """A module for functions related to IDM building-bodies."""
 from typing import List
 from ladybug_geometry.bounding import bounding_box
 from ladybug_geometry.geometry2d import Polygon2D, Point2D
-from ladybug_geometry.geometry3d import Plane, LineSegment3D, Face3D
+from ladybug_geometry.geometry3d import Plane, LineSegment3D
 
 from honeybee.room import Room
-from honeybee.facetype import RoofCeiling, Floor
+from honeybee.facetype import Floor
 
 from .geometry_utils import get_floor_boundary, get_rooms_boundary
 
 
 def _section_to_idm_protected(rooms: List[Room]):
     if not rooms:
         return ''
```

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/cli/translate.py` & `honeybee-idaice-0.3.6/honeybee_idaice/cli/translate.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/face.py` & `honeybee-idaice-0.3.6/honeybee_idaice/face.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import math
 from typing import Union
 
 from honeybee.model import Face, Aperture, Door
 from ladybug_geometry.geometry3d import Point3D, Vector3D, Plane, Face3D
 
+from .geometry_utils import prepare_apertures
+
 
 def opening_to_idm(opening: Union[Aperture, Door], is_aperture=True) -> str:
     """Translate a HBJSON aperture to an IDM Window."""
     # name = opening.display_name
     name = opening.identifier
 
     # IDA-ICE looks to apertures from inside the room
@@ -65,15 +67,18 @@
     count = len(vertices)
     vertices_idm = ' '.join((
         f'({v.x - origin.x} {v.y - origin.y} {v.z - origin.z})' for v in vertices
     ))
 
     # add apertures
     windows = ['']
-    for aperture in face.apertures:
+    apertures = prepare_apertures(face.apertures)
+    for aperture in apertures:
+        if aperture.user_data and aperture.user_data.get('_idm_ignore', False):
+            continue
         windows.append(opening_to_idm(aperture))
 
     windows = ''.join(windows)
 
     # add doors
     doors = ['']
     for door in face.doors:
```

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/shade.py` & `honeybee-idaice-0.3.6/honeybee_idaice/shade.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/templates/ahu.idc` & `honeybee-idaice-0.3.6/honeybee_idaice/templates/ahu.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/templates/ahu.idm` & `honeybee-idaice-0.3.6/honeybee_idaice/templates/ahu.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/templates/building.idm` & `honeybee-idaice-0.3.6/honeybee_idaice/templates/building.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/templates/plant.idc` & `honeybee-idaice-0.3.6/honeybee_idaice/templates/plant.idc`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/templates/plant.idm` & `honeybee-idaice-0.3.6/honeybee_idaice/templates/plant.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/templates/room.idm` & `honeybee-idaice-0.3.6/honeybee_idaice/templates/room.idm`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/writer.py` & `honeybee-idaice-0.3.6/honeybee_idaice/writer.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from typing import List
 
 from honeybee.model import Model, Room, Face
 from honeybee.facetype import RoofCeiling, Wall, Floor
 from ladybug_geometry.geometry3d import Point3D
 
 from .archive import zip_folder_to_idm
-from .geometry_utils import get_floor_boundary, get_ceiling_boundary
+from .geometry_utils import get_floor_boundary, get_ceiling_boundary, prepare_apertures
 from .bldgbody import section_to_idm
 from .shade import shades_to_idm
 from .face import face_to_idm, opening_to_idm
 
 
 def ceilings_to_idm(faces: List[Face], origin: Point3D):
     """Translate a collection of ceilings face to an IDM ENCLOSING-ELEMENT."""
@@ -43,15 +43,16 @@
         count = len(vertices)
         vertices_idm = ' '.join((
             f'({v.x - origin.x} {v.y - origin.y} {v.z - origin.z})' for v in vertices
         ))
 
         # add apertures
         windows = ['']
-        for aperture in face.apertures:
+        apertures = prepare_apertures(face.apertures)
+        for aperture in apertures:
             windows.append(opening_to_idm(aperture))
 
         windows = ''.join(windows)
 
         cp = f' ((ENCLOSING-ELEMENT :N "{name}" :T CEILING-PART :INDEX {-1001 - fc})\n' \
             '  ((AGGREGATE :N GEOMETRY)\n' \
             f'   (:PAR :N CORNERS :DIM ({count} 3) :SP ({count} 3) :V #2A({vertices_idm}))\n' \
@@ -185,16 +186,19 @@
     model.convert_to_units(units='Meters')
 
     room_names = {}
     grouped_rooms, _ = Room.group_by_floor_height(model.rooms, min_difference=0.2)
     tolerance = 0.75  # assuming the door centers are not closer than this dist
     for grouped_room in grouped_rooms:
         door_tracker = []
+        aperture_tracker = []
         for room in grouped_room:
             # check the display name and change it if it is not unique
+            room.display_name = \
+                room.display_name.replace('/', '-').replace('\\', '-').replace('\n', ' ')
             if room.display_name in room_names:
                 original_name = room.display_name
                 room.display_name = \
                     f'{room.display_name}_{room_names[original_name]}'
                 room_names[original_name] += 1
             else:
                 room_names[room.display_name] = 1
@@ -203,15 +207,23 @@
                 for door in face.doors:
                     center = door.geometry.center
                     for pt in door_tracker:
                         if pt.distance_to_point(center) <= tolerance:
                             door.user_data = {'_idm_ignore': True}
                             break
                     door_tracker.append(center)
-
+                for aperture in face.apertures:
+                    center = aperture.geometry.center
+                    normal = aperture.geometry.normal
+                    for data in aperture_tracker:
+                        c, n = data
+                        if c.distance_to_point(center) <= tolerance \
+                                and abs(n.angle(normal) - 3.14159) < 0.1:
+                            aperture.user_data = {'_idm_ignore': True}
+                    aperture_tracker.append((center, normal))
     return model
 
 
 def model_to_idm(model: Model, out_folder: pathlib.Path, name: str = None,
                  debug: bool = True):
     """Translate a Honeybee model to an IDM file."""
 
@@ -244,23 +256,15 @@
             bldg.write(line)
 
         # create a building section for each floor
         sections = section_to_idm(model.rooms)
         bldg.write(sections)
 
         # add rooms as zones
-        room_names = {}
         for room in model.rooms:
-            if room.display_name in room_names:
-                original_name = room.display_name
-                room.display_name = \
-                    f'{room.display_name}_{room_names[original_name]}'
-                room_names[original_name] += 1
-            else:
-                room_names[room.display_name] = 1
             bldg.write(f'((CE-ZONE :N "{room.display_name}" :T ZONE))\n')
 
         # collect all the shades from room
         shades_idm = shades_to_idm(model.shades)
         bldg.write(shades_idm)
         bldg.write(f'\n;[end of {bldg_name}.idm]\n')
```

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice/writer_obj.py` & `honeybee-idaice-0.3.6/honeybee_idaice/writer_obj.py`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice.egg-info/PKG-INFO` & `honeybee-idaice-0.3.6/honeybee_idaice.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: honeybee-idaice
-Version: 0.3.5
+Version: 0.3.6
 Summary: Honeybee extension for translating HBJSON files to IDA-ICE IDM.
 Home-page: https://github.com/ladybug-tools/honeybee-idaice
 Author: Ladybug Tools
 Author-email: info@ladybug.tools
 License: AGPL-3.0
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
```

### Comparing `honeybee-idaice-0.3.5/honeybee_idaice.egg-info/SOURCES.txt` & `honeybee-idaice-0.3.6/honeybee_idaice.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `honeybee-idaice-0.3.5/setup.py` & `honeybee-idaice-0.3.6/setup.py`

 * *Files identical despite different names*

