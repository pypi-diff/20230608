# Comparing `tmp/lidia-0.8.1.tar.gz` & `tmp/lidia-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lidia-0.8.1.tar", last modified: Mon Apr 17 19:46:17 2023, max compression
+gzip compressed data, was "lidia-0.9.0.tar", last modified: Thu Jun  8 10:16:07 2023, max compression
```

## Comparing `lidia-0.8.1.tar` & `lidia-0.9.0.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.486624 lidia-0.8.1/
--rw-rw-rw-   0        0        0     1097 2023-02-17 08:50:04.000000 lidia-0.8.1/LICENSE.txt
--rw-rw-rw-   0        0        0      114 2023-03-01 12:02:42.000000 lidia-0.8.1/MANIFEST.in
--rw-rw-rw-   0        0        0     2519 2023-04-17 19:46:17.487624 lidia-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0     2052 2023-03-01 12:02:42.000000 lidia-0.8.1/README.md
--rw-rw-rw-   0        0        0       88 2022-12-15 16:52:24.000000 lidia-0.8.1/pyproject.toml
--rw-rw-rw-   0        0        0      858 2023-04-17 19:46:17.492624 lidia-0.8.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:16.543715 lidia-0.8.1/src/
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:16.955289 lidia-0.8.1/src/lidia/
--rw-rw-rw-   0        0        0       23 2023-04-17 19:44:25.000000 lidia-0.8.1/src/lidia/__init__.py
--rw-rw-rw-   0        0        0       35 2022-06-02 23:11:14.000000 lidia-0.8.1/src/lidia/__main__.py
--rw-rw-rw-   0        0        0    12690 2023-04-17 19:44:25.000000 lidia-0.8.1/src/lidia/aircraft.py
--rw-rw-rw-   0        0        0     3584 2023-02-17 08:50:04.000000 lidia-0.8.1/src/lidia/approach.html
--rw-rw-rw-   0        0        0     5293 2023-02-17 08:50:04.000000 lidia-0.8.1/src/lidia/cas.html
--rw-rw-rw-   0        0        0     3821 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/config.py
--rw-rw-rw-   0        0        0     1061 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/info.html
--rw-rw-rw-   0        0        0     5165 2023-03-01 12:02:42.000000 lidia-0.8.1/src/lidia/lidia.py
--rw-rw-rw-   0        0        0     2540 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/mytypes.py
--rw-rw-rw-   0        0        0    27835 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/pfd.html
--rw-rw-rw-   0        0        0    15774 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/rpctask.html
--rw-rw-rw-   0        0        0     2312 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/server.py
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.131388 lidia-0.8.1/src/lidia/sources/
--rw-rw-rw-   0        0        0        0 2022-06-13 10:57:36.000000 lidia-0.8.1/src/lidia/sources/__init__.py
--rw-rw-rw-   0        0        0     2236 2022-12-19 19:16:52.000000 lidia-0.8.1/src/lidia/sources/approach.py
--rw-rw-rw-   0        0        0     1551 2023-02-17 08:50:04.000000 lidia-0.8.1/src/lidia/sources/confighelp.md
--rw-rw-rw-   0        0        0     2416 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/confighelp.py
--rw-rw-rw-   0        0        0     5204 2023-04-17 19:44:25.000000 lidia-0.8.1/src/lidia/sources/demo.py
--rw-rw-rw-   0        0        0     2937 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/flightgear.py
--rw-rw-rw-   0        0        0     6600 2022-12-19 19:16:52.000000 lidia-0.8.1/src/lidia/sources/mytypes.py
--rw-rw-rw-   0        0        0     3623 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/rpctask.py
--rw-rw-rw-   0        0        0     2112 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/sources/smol.py
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.370196 lidia-0.8.1/src/lidia/static/
--rw-rw-rw-   0        0        0     1761 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/LICENSE.txt
--rw-rw-rw-   0        0        0    87008 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Bold.ttf
--rw-rw-rw-   0        0        0    87788 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-ExtraLight.ttf
--rw-rw-rw-   0        0        0    87592 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Light.ttf
--rw-rw-rw-   0        0        0    86820 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Medium.ttf
--rw-rw-rw-   0        0        0    86908 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Regular.ttf
--rw-rw-rw-   0        0        0    87076 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-SemiBold.ttf
--rw-rw-rw-   0        0        0    87872 2022-11-28 17:12:51.000000 lidia-0.8.1/src/lidia/static/RobotoMono-Thin.ttf
--rw-rw-rw-   0        0        0     7073 2022-12-09 17:51:17.000000 lidia-0.8.1/src/lidia/static/controls.js
--rw-rw-rw-   0        0        0   121824 2022-06-02 22:10:07.000000 lidia-0.8.1/src/lidia/static/socket.io.js
--rw-rw-rw-   0        0        0     1853 2023-03-01 11:21:48.000000 lidia-0.8.1/src/lidia/static/style.css
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.484624 lidia-0.8.1/src/lidia/utils/
--rw-rw-rw-   0        0        0     3654 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/utils/pack_lidia.m
--rw-rw-rw-   0        0        0    22361 2023-04-17 19:44:22.000000 lidia-0.8.1/src/lidia/utils/pack_maker.py
-drwxrwxrwx   0        0        0        0 2023-04-17 19:46:17.011333 lidia-0.8.1/src/lidia.egg-info/
--rw-rw-rw-   0        0        0     2519 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1224 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       97 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-17 19:46:16.000000 lidia-0.8.1/src/lidia.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.518508 lidia-0.9.0/
+-rw-rw-rw-   0        0        0     1097 2023-02-17 08:50:04.000000 lidia-0.9.0/LICENSE.txt
+-rw-rw-rw-   0        0        0      114 2023-03-01 12:02:42.000000 lidia-0.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2519 2023-06-08 10:16:07.519630 lidia-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2052 2023-03-01 12:02:42.000000 lidia-0.9.0/README.md
+-rw-rw-rw-   0        0        0       88 2022-12-15 16:52:24.000000 lidia-0.9.0/pyproject.toml
+-rw-rw-rw-   0        0        0      858 2023-06-08 10:16:07.523604 lidia-0.9.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.140566 lidia-0.9.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.399006 lidia-0.9.0/src/lidia/
+-rw-rw-rw-   0        0        0       23 2023-06-08 10:14:52.000000 lidia-0.9.0/src/lidia/__init__.py
+-rw-rw-rw-   0        0        0       35 2022-06-02 23:11:14.000000 lidia-0.9.0/src/lidia/__main__.py
+-rw-rw-rw-   0        0        0    14247 2023-06-08 10:14:52.000000 lidia-0.9.0/src/lidia/aircraft.py
+-rw-rw-rw-   0        0        0     3584 2023-02-17 08:50:04.000000 lidia-0.9.0/src/lidia/approach.html
+-rw-rw-rw-   0        0        0     5293 2023-02-17 08:50:04.000000 lidia-0.9.0/src/lidia/cas.html
+-rw-rw-rw-   0        0        0     4862 2023-06-08 10:14:52.000000 lidia-0.9.0/src/lidia/config.py
+-rw-rw-rw-   0        0        0     1061 2023-04-17 19:44:22.000000 lidia-0.9.0/src/lidia/info.html
+-rw-rw-rw-   0        0        0     5165 2023-03-01 12:02:42.000000 lidia-0.9.0/src/lidia/lidia.py
+-rw-rw-rw-   0        0        0     2540 2023-04-17 19:44:22.000000 lidia-0.9.0/src/lidia/mytypes.py
+-rw-rw-rw-   0        0        0    38852 2023-06-08 10:14:52.000000 lidia-0.9.0/src/lidia/pfd.html
+-rw-rw-rw-   0        0        0    15774 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/rpctask.html
+-rw-rw-rw-   0        0        0     2312 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/server.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.480520 lidia-0.9.0/src/lidia/sources/
+-rw-rw-rw-   0        0        0        0 2022-06-13 10:57:36.000000 lidia-0.9.0/src/lidia/sources/__init__.py
+-rw-rw-rw-   0        0        0     2236 2022-12-19 19:16:52.000000 lidia-0.9.0/src/lidia/sources/approach.py
+-rw-rw-rw-   0        0        0     1551 2023-02-17 08:50:04.000000 lidia-0.9.0/src/lidia/sources/confighelp.md
+-rw-rw-rw-   0        0        0     2416 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/sources/confighelp.py
+-rw-rw-rw-   0        0        0     6390 2023-06-08 10:14:52.000000 lidia-0.9.0/src/lidia/sources/demo.py
+-rw-rw-rw-   0        0        0     2937 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/sources/flightgear.py
+-rw-rw-rw-   0        0        0     6600 2022-12-19 19:16:52.000000 lidia-0.9.0/src/lidia/sources/mytypes.py
+-rw-rw-rw-   0        0        0     3623 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/sources/rpctask.py
+-rw-rw-rw-   0        0        0     2112 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/sources/smol.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.511512 lidia-0.9.0/src/lidia/static/
+-rw-rw-rw-   0        0        0     1761 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/LICENSE.txt
+-rw-rw-rw-   0        0        0    87008 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-Bold.ttf
+-rw-rw-rw-   0        0        0    87788 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-ExtraLight.ttf
+-rw-rw-rw-   0        0        0    87592 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-Light.ttf
+-rw-rw-rw-   0        0        0    86820 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-Medium.ttf
+-rw-rw-rw-   0        0        0    86908 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-Regular.ttf
+-rw-rw-rw-   0        0        0    87076 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-SemiBold.ttf
+-rw-rw-rw-   0        0        0    87872 2022-11-28 17:12:51.000000 lidia-0.9.0/src/lidia/static/RobotoMono-Thin.ttf
+-rw-rw-rw-   0        0        0     7073 2022-12-09 17:51:17.000000 lidia-0.9.0/src/lidia/static/controls.js
+-rw-rw-rw-   0        0        0   121824 2022-06-02 22:10:07.000000 lidia-0.9.0/src/lidia/static/socket.io.js
+-rw-rw-rw-   0        0        0     1853 2023-03-01 11:21:48.000000 lidia-0.9.0/src/lidia/static/style.css
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.516524 lidia-0.9.0/src/lidia/utils/
+-rw-rw-rw-   0        0        0     3654 2023-04-17 19:44:22.000000 lidia-0.9.0/src/lidia/utils/pack_lidia.m
+-rw-rw-rw-   0        0        0    22361 2023-04-17 19:44:22.000000 lidia-0.9.0/src/lidia/utils/pack_maker.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:16:07.457507 lidia-0.9.0/src/lidia.egg-info/
+-rw-rw-rw-   0        0        0     2519 2023-06-08 10:16:07.000000 lidia-0.9.0/src/lidia.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1224 2023-06-08 10:16:07.000000 lidia-0.9.0/src/lidia.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:16:07.000000 lidia-0.9.0/src/lidia.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-06-08 10:16:07.000000 lidia-0.9.0/src/lidia.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       97 2023-06-08 10:16:07.000000 lidia-0.9.0/src/lidia.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 10:16:07.000000 lidia-0.9.0/src/lidia.egg-info/top_level.txt
```

### Comparing `lidia-0.8.1/LICENSE.txt` & `lidia-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/PKG-INFO` & `lidia-0.9.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidia
-Version: 0.8.1
+Version: 0.9.0
 Summary: serve an aircraft instruments panel as a web page
 Home-page: https://gitlab.com/Maarrk/lidia
 Author: Marek S. Lukasiewicz
 Author-email: marek@lukasiewicz.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lidia-0.8.1/README.md` & `lidia-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/setup.cfg` & `lidia-0.9.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/aircraft.py` & `lidia-0.9.0/src/lidia/aircraft.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from enum import Enum
 import json
 from math import cos, sin, sqrt
 from time import time
 from pydantic import BaseModel
 from typing import Any, Dict, List, Optional, Sequence
 
 from .config import Config as LidiaConfig
@@ -44,14 +45,21 @@
     """Engine power input, between 0 and 1"""
     pedals_right: float = 0
     """Pedals input to yaw right, between -1 and 1"""
     collective_up: float = 0
     """Collective input to increase lift, between 0 and 1"""
 
 
+class HelicopterRPM(VectorModel):
+    rotor: float = 0
+    """Rotor RPM, relative to nominal"""
+    engine: float = 0
+    """Engine RPM, relative to nominal"""
+
+
 class Borders(BaseModel):
     low = Controls.from_list([-1, -1, 0, -1, 0])
     high = Controls.from_list([1, 1, 1, 1, 1])
 
     def smol(self) -> Dict[str, Any]:
         return {
             'low': self.low.smol(),
@@ -60,35 +68,62 @@
 
 
 class Buttons(IntFlagModel):
     cyc_ftr: bool = False
     coll_ftr: bool = False
 
 
+class CASMessage(BaseModel):
+    msg_id: int
+    blinking: bool
+
+
+class CAS(BaseModel):
+    """Crew Alerting System state"""
+    msgs: List[CASMessage]
+
+
+class TrafficVolume(Enum):
+    OTHER_TRAFFIC = 0
+    """No collision threat, fits in entire surveillance range; hollow white diamond"""
+    PROXIMATE_TRAFFIC = 1
+    """No collision threat, intruder in a specified range; filled white diamond"""
+    TRAFFIC_ADVISORY = 2
+    """Possible threat of collision in 40 seconds; filled amber circle"""
+    RESOLUTION_ADVISORY = 3
+    """Real threat of collision in 25 seconds; filled red square"""
+
+
+class TrafficObject(BaseModel):
+    """Object displayed on TCAS view"""
+    vol: TrafficVolume = TrafficVolume.OTHER_TRAFFIC
+    """Type of traffic advisory issued"""
+    brg: float = 0
+    """Relative bearing to right, in radians"""
+    dist: float = 0
+    """Distance to intruder, in meters"""
+    alt: float = 0
+    """Altitude difference positive for intruder higher, in meters"""
+    vsi: int = 0
+    """Intruder vertical speed indicator, positive for climb"""
+
+
 class Instruments(BaseModel):
     ias: float = 0
     """Indicated airspeed"""
     gs: Optional[float] = None
     """Groundspeed"""
     alt: float = 0
     """Barometric altitude"""
     qnh: Optional[float] = 1013
     """Altimeter setting, None for STD"""
     ralt: Optional[float] = None
     """Radio altimeter"""
-
-
-class CASMessage(BaseModel):
-    msg_id: int
-    blinking: bool
-
-
-class CAS(BaseModel):
-    """Crew Alerting System state"""
-    msgs: List[CASMessage]
+    tcas: Optional[List[TrafficObject]] = None
+    """Traffic objects"""
 
 
 class Transforms:
     @staticmethod
     def _matmul(matrix: Sequence[float], multiplicand: Sequence[float]) -> List[float]:
         """Multiply 3x3 matrix by 3-element vector or 3x3 matrix"""
         assert len(matrix) == 9
@@ -162,14 +197,16 @@
     """Velocity in local horizon coordinate system, in meters per second"""
     a_body: Optional[XYZ] = None
     """Acceleration measured (with gravity) in body frame, in meters per second squared"""
     a_ned: Optional[NED] = None
     """Acceleration measured in local horizon coordinate system, in meters per second squared"""
     ctrl: Optional[Controls] = None
     """Control inceptors position, normalized by max deflection"""
+    hrpm: Optional[HelicopterRPM] = None
+    """RPM value, normalized to nominal"""
     brdr: Optional[Borders] = None
     """Task borders for inceptors"""
     btn: Optional[Buttons] = None
     """Pressed buttons"""
     instr: Optional[Instruments] = None
     """Instrument values"""
     t_boot: Optional[int] = None
@@ -186,32 +223,37 @@
         """Return self as dictionary with SMOL-defined keys"""
         # HACK: JSON roundtrip is required, because there is no encoder configuration for .dict()
         return json.loads(self.json(models_as_dict=False, exclude={f for f in self.__fields__ if (getattr(self, f) is None or f in ['trgt', 'trim'])}))
 
     @classmethod
     def from_smol(cls, smol: dict) -> 'AircraftData':
         state = cls()
-        for name in ['ned', 'v_ned', 'a_ned']:
-            if name in smol:
-                setattr(state, name, NED.from_list(smol[name]))
-        if 'att' in smol:
-            state.att = Attitude.from_list(smol['att'])
-        for name in ['v_body', 'a_body']:
+        for VectorType, name in [
+            (NED, 'ned'),
+            (NED, 'v_ned'),
+            (NED, 'a_ned'),
+            (Attitude, 'att'),
+            (XYZ, 'v_body'),
+            (XYZ, 'a_body'),
+            (Controls, 'ctrl'),
+            (HelicopterRPM, 'hrpm'),
+        ]:
             if name in smol:
-                setattr(state, name, XYZ.from_list(smol[name]))
-        if 'ctrl' in smol:
-            state.ctrl = Controls.from_list(smol['ctrl'])
+                setattr(state, name, VectorType.from_list(smol[name]))
         # TODO: Borders
         if 'btn' in smol:
             state.btn = Buttons.from_list(smol['btn'])
         if 'instr' in smol:
             state.instr = Instruments()
-            for name in ['ias', 'gs', 'alt', 'qnh', 'alt']:
+            for name in ['ias', 'gs', 'alt', 'qnh', 'ralt']:
                 if name in smol['instr']:
                     setattr(state.instr, name, smol['instr'][name])
+            if 'tcas' in smol['instr']:
+                state.instr.tcas = [
+                    TrafficObject(**t) for t in smol['instr']['tcas']]
         if 't_boot' in smol:
             state.t_boot = smol['t_boot']
 
         return state
 
     def xyz2ned(self, vec: XYZ) -> NED:
         """Transform from body frame vector to outside frame coordinates
@@ -336,14 +378,19 @@
     state.a_body = XYZ.from_list([0.0, 0.0, 0.0])
     state.a_ned = NED.from_list([0.0, 0.0, 0.0])
     state.ctrl = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
     state.trgt = AircraftData()
     state.trgt.ctrl = Controls.from_list([0.0, 0.0, 0.0, 0.0, 0.0])
     state.t_boot = 0x10000000
     state.model_instruments(config)
+    state.instr.tcas = []
+    state.instr.tcas.append(TrafficObject(
+        vol=TrafficVolume.PROXIMATE_TRAFFIC,
+        brg=0.5, dist=5000.0, alt=10.0, vsi=0
+    ))
     print(state.smol())
     import msgpack
     packer = msgpack.Packer(use_single_float=False)
     data_double = packer.pack(state.smol())
     packer = msgpack.Packer(use_single_float=True)
     data_float = packer.pack(state.smol())
     data = data_double[:0x21] + data_float[0x15:]
```

### Comparing `lidia-0.8.1/src/lidia/approach.html` & `lidia-0.9.0/src/lidia/approach.html`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/cas.html` & `lidia-0.9.0/src/lidia/cas.html`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/info.html` & `lidia-0.9.0/src/lidia/info.html`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/lidia.py` & `lidia-0.9.0/src/lidia/lidia.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/mytypes.py` & `lidia-0.9.0/src/lidia/mytypes.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/pfd.html` & `lidia-0.9.0/src/lidia/pfd.html`

 * *Files 19% similar despite different names*

```diff
@@ -28,14 +28,35 @@
         stroke-linecap="round" fill="none" />
       <path id="flightpathVector" d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M -2,0 h-3.5 M 2,0 h3.5 M 0,-2 v-1.5"
         stroke-linecap="square" fill="none" />
       <g id="flightpathRetrograde" stroke-linecap="square" fill="none">
         <path d="M -2,0 a 2,2 0 0,0 4,0 a 2,2 0 0,0 -4,0 M 0,-2 v-2 M -1.73, 1 l -1.73, 1 M 1.73, 1 l 1.73, 1" />
         <path d="M -2.82,-2.82 L 2.82,2.82 M -2.82,2.82 L 2.82,-2.82" transform="scale(0.5)" />
       </g>
+      <!-- Duplication of label code, because the <use> element creates a closed shadow root, inaccessible to outside JS -->
+      <g id="trafficOT">
+        <polygon points="-10,0 0,12 10,0 0,-12" fill="none" stroke-width="3" />
+        <text x="15" y="-25" text-anchor="end" dominant-baseline="central" font-size="25" stroke="none">+00</text>
+        <path d="M 20,13 v-17 h5 l-5,-8 l-5,8 h5" stroke-width="3" transform="scale(1,1)" />
+      </g>
+      <g id="trafficPD">
+        <polygon points="-10,0 0,12 10,0 0,-12" />
+        <text x="15" y="-25" text-anchor="end" dominant-baseline="central" font-size="25" stroke="none">+00</text>
+        <path d="M 20,13 v-17 h5 l-5,-8 l-5,8 h5" stroke-width="3" transform="scale(1,1)" />
+      </g>
+      <g id="trafficTA">
+        <circle cx="0" cy="0" r="10" stroke="none" />
+        <text x="15" y="-25" text-anchor="end" dominant-baseline="central" font-size="25" stroke="none">+00</text>
+        <path d="M 20,13 v-17 h5 l-5,-8 l-5,8 h5" stroke-width="3" transform="scale(1,1)" />
+      </g>
+      <g id="trafficRA">
+        <rect x="-9" y="-9" width="18" height="18" />
+        <text x="15" y="-25" text-anchor="end" dominant-baseline="central" font-size="25" stroke="none">+00</text>
+        <path d="M 20,13 v-17 h5 l-5,-8 l-5,8 h5" stroke-width="3" transform="scale(1,1)" />
+      </g>
     </defs>
     <g id="autopilotRegion" data-extents="0 1325 30 775">
       <path id="PIC" d="M1050 15 v5 h15 v 10 l15 -15 l-15 -15 v10 h-15 z" fill="var(--pfdGreen)" stroke="none" />
     </g>
 
     <g id="adiRegion" data-extents="35 1325 585 775">
       <g transform="translate(1050 310)">
@@ -126,14 +147,18 @@
         <g id="vsiText" fill="white" font-size="40" dominant-baseline="central" transform="translate(420)">
           <text y="-240">2</text>
           <text y="-180">1</text>
           <text y="180">1</text>
           <text y="240">2</text>
         </g>
         <line id="vsiIndicator" x1="320" y1="0" x2="370" y2="0" stroke="var(--pfdGreen)" stroke-width="8" />
+        <line id="vsiTargetIndicatorContour" x1="378" y1="0" x2="417" y2="0" stroke="black" stroke-width="12"
+          display="none" />
+        <line id="vsiTargetIndicator" x1="380" y1="0" x2="415" y2="0" stroke="var(--pfdMagenta)" stroke-width="8"
+          display="none" />
       </g>
     </g>
 
     <g id="vsidialRegionIgnored" display="none" data-extents="25 2080 585 1520">
       <g transform="translate(1800 310)">
         <circle cx="0" cy="0" r="275" fill="black" stroke="white" stroke-width="5" />
         <g id="vsidialDial" text-anchor="middle" dominant-baseline="central" fill="white" stroke="white" font-size="50"
@@ -224,23 +249,24 @@
           <use href="#iasBackground" />
         </clipPath>
 
         <g clip-path="url(#iasClip)">
           <g transform="scale(6)">
             <g id="iasTape" transform="translate(0 0)" fill="white" font-size="6" text-anchor="end"
               dominant-baseline="central" stroke="white" stroke-width="1">
-              <g id="iasVne" transform="translate(0 -167)">
-                <path d="m0 0 h-30 " stroke="var(--pfdRed)" stroke-width="2" />
+              <path id="iasVne" transform="translate(0 -167)" d="m0 0 h-30 " stroke="var(--pfdRed)" stroke-width="2" />
+              <g id="iasTapeTicks">
+                <path d="m0 10 h-10" />
+                <path d="m0 20 h-10" />
+                <path d="m0 30 h-10" />
+                <path d="m0 40 h-10" />
+                <!-- Other ticks generated with script -->
               </g>
-
-              <path d="m0 10 h-10" />
-              <path d="m0 20 h-10" />
-              <path d="m0 30 h-10" />
-              <path d="m0 40 h-10" />
-              <!-- Other ticks generated with script -->
+              <path id="iasTargetIndicator" transform="translate(0 -0)" d="m0 0 l -4 -4 v-2 h4 v12 h-4 v-2 z"
+                fill="var(--pfdMagenta)" stroke-width="0.4" stroke="black" display="none" />
             </g>
           </g>
         </g>
         <use href="#iasBackground" class="tapeContour" />
         <g id="iasReadout">
           <path id="iasReadoutBackground" d="m-5 0 l-30 -30 h-135 v60 h135 z" />
           <clipPath id="iasReadoutClip">
@@ -296,18 +322,55 @@
         </g>
         <path d="M250 0 v-25 h-150 l-50 25 l50 25 h150 z" stroke="white" stroke-width="5" />
         <text id="rhtValue" x="245" y="0" fill="var(--pfdAmber)" font-size="48" text-anchor="end"
           dominant-baseline="central">---</text>
       </g>
     </g>
 
+    <g id="rpmRegion" data-extents="660 755 1220 575">
+      <g transform="translate(750 940)">
+        <rect id="rpmBackground" x="-170" y="-275" height="550" width="170" />
+        <use href="#rpmBackground" class="tapeContour" />
+        <g text-anchor="middle" font-size="50" fill="white" transform="translate(-85)">
+          <text id="rpmEName" x="-30" y="-200">E</text>
+          <text id="rpmRName" x="30" y="-200">R</text>
+          <g font-size="30" text-anchor="end">
+            <text id="rpmEReadout" x="-5" y="240">00%</text>
+            <text id="rpmRReadout" x="80" y="240">00%</text>
+          </g>
+        </g>
+        <g transform="translate(-85 180) rotate(-90) scale(3)">
+          <!-- Engine RPM -->
+          <g transform="translate(0 -10)">
+            <rect id="rpmEBackground" y="-4.5" x="-1.5" height="9" width="123" fill="var(--pfdRed)" />
+            <rect id="rpmEFillLow" y="-3" x="0" height="6" width="100" fill="var(--pfdRed)" />
+            <rect id="rpmEFillHigh" y="-3" x="100" height="6" width="20" fill="black" />
+            <rect id="rpmETapeWarn" y="-4.5" x="97" height="9" width="6" fill="var(--pfdAmber)" />
+            <rect id="rpmETapeGood" y="-4.5" x="97" height="9" width="6" fill="var(--pfdGreen)" />
+            <path id="rpmEIndicator" d="M0 -4.5 l5 -10 h-10 z" fill="var(--pfdRed)" transform="translate(0)" />
+          </g>
+          <!-- Rotor RPM -->
+          <g transform="translate(0 10)">
+            <rect id="rpmRBackground" y=" -4.5" x="-1.5" height="9" width="123" fill="var(--pfdRed)" />
+            <rect id="rpmRFillLow" y="-3" x="0" height="6" width="100" fill="var(--pfdRed)" />
+            <rect id="rpmRFillHigh" y="-3" x="100" height="6" width="20" fill="black" />
+            <rect id="rpmRTapeWarn" y="-4.5" x="90" height="9" width="20" fill="var(--pfdAmber)" />
+            <rect id="rpmRTapeGood" y="-4.5" x="97" height="9" width="6" fill="var(--pfdGreen)" />
+            <path id="rpmRIndicator" d="M0 4.5 l5 10 h-10 z" fill="var(--pfdRed)" transform="translate(0)" />
+          </g>
+        </g>
+      </g>
+    </g>
+
     <g id="hsiRegion" data-extents="595 1325 1180 775">
       <g transform="translate(1050 900)">
         <circle cx="0" cy="0" r="275" fill="black" stroke="none" />
-        <circle cx="0" cy="0" r="137.5" fill="none" stroke="white" stroke-dasharray="3" stroke-width="3" />
+        <circle cx="0" cy="0" r="80" fill="none" stroke="gray" stroke-dasharray="3,9" stroke-width="3" />
+        <circle id="hsiTrafficPerimeter" cx="0" cy="0" r="160" fill="none" stroke="gray" stroke-dasharray="3,6"
+          stroke-width="3" />
         <path d="M0 -280 l20 -20 h-40 z" stroke="white" stroke-width="5" />
         <g id="hsiWheel" text-anchor="middle" dominant-baseline="hanging" fill="white" font-size="40" font-weight="600">
           <text x="0" y="-225">N</text>
           <text x="0" y="-225" transform="rotate(30)">3</text>
           <text x="0" y="-225" transform="rotate(60)">6</text>
           <text x="0" y="-225" transform="rotate(90)">E</text>
           <text x="0" y="-225" transform="rotate(120)">12</text>
@@ -317,15 +380,25 @@
           <text x="0" y="-225" transform="rotate(240)">24</text>
           <text x="0" y="-225" transform="rotate(270)">W</text>
           <text x="0" y="-225" transform="rotate(300)">30</text>
           <text x="0" y="-225" transform="rotate(330)">33</text>
 
           <!-- Ticks generated with script -->
         </g>
-        <g id="hsiHeli">
+        <g id="hsiTraffic">
+          <g id="hsiTrafficOT" fill="white" stroke="white">
+          </g>
+          <g id="hsiTrafficPD" fill="white" stroke="white">
+          </g>
+          <g id="hsiTrafficTA" fill="var(--pfdAmber)" stroke="var(--pfdAmber)">
+          </g>
+          <g id="hsiTrafficRA" fill="var(--pfdRed)" stroke="var(--pfdRed)">
+          </g>
+        </g>
+        <g id="hsiHeli" transform="scale(0.75)">
           <ellipse cx="0" cy="0" rx="12" ry="30" fill="white" />
           <path d="M0 0 v60 M-7 50 h15" stroke-width="5" stroke="white" />
           <path d="M-32 -32 l64 64 M-32 32 l64 -64" stroke-width="8" stroke="white" />
         </g>
       </g>
     </g>
 
@@ -412,16 +485,16 @@
 
     let iasTapeHTML = [];
     for (let ias = 0; ias <= 400; ias += 10) {
       iasTapeHTML.push(`
         <path d="m0 ${-ias} h-10" />
         <text x="-12" y="${-ias}" stroke="none">${ias}</text>`);
     }
-    let iasTape = document.getElementById("iasTape");
-    iasTape.innerHTML = iasTape.innerHTML + iasTapeHTML.join("");
+    let iasTapeTicks = document.getElementById("iasTapeTicks");
+    iasTapeTicks.innerHTML = iasTapeTicks.innerHTML + iasTapeHTML.join("");
 
     let pitchHTML = [];
     for (let pitch = -50; pitch <= 50; pitch += 10) {
       if (pitch == 0) continue;
 
       pitchHTML.push(`
         <text x="-13" y="${-pitch}" text-anchor="end" stroke="none">${Math.abs(pitch)}</text>
@@ -459,22 +532,33 @@
     hsiWheel.innerHTML = hsiWheel.innerHTML + hsiWheelHTML.join("");
   </script>
 
   <script type="text/javascript">
     var socket = io();
     var config = {
       ias_never_exceed: 167,
+      show_ias_target: true,
+      show_vsi_target: true,
       rotate_adi_target: true,
       show_adi_target: true,
       adi_target_roll: true,
       adi_target_yaw: false,
       show_flightpath: true,
       show_retrograde: false,
       move_roll_ticks: false,
       sideslip_max: 15,
+      rpm_e_good_low: 0.97,
+      rpm_e_good_high: 1.03,
+      rpm_e_warn_low: 0.97,
+      rpm_e_warn_high: 1.03,
+      rpm_r_good_low: 0.97,
+      rpm_r_good_high: 1.03,
+      rpm_r_warn_low: 0.90,
+      rpm_r_warn_high: 1.10,
+      traffic_range: 18520,
     };
 
     function updateOptional(value, element, decimal = 0, width = 1) {
       if (value !== null && isFinite(value)) {
         element.textContent = value.toFixed(decimal).padStart(width, "0");
         element.setAttribute("fill", "white");
       } else {
@@ -547,22 +631,25 @@
         qnhValue.setAttribute("fill", "white");
       }
     }
 
     const vsiIndicator = document.getElementById("vsiIndicator");
     const vsiX1 = parseFloat(vsiIndicator.getAttribute("x1"));
     const vsiX2 = parseFloat(vsiIndicator.getAttribute("x2"));
-    function updateVSI(verticalSpeed) {
+    function vsiAngleRadians(verticalSpeed) {
       let direction = Math.sign(verticalSpeed);
       let value = Math.abs(verticalSpeed);
       const maxAngleDeg = 37;
       let angleDeg = (value <= 10) ? (value / 10 * 25) : // first 10 hft/min is 25 degrees
         (value - 10 + 25); // above 10 it's 10 deg per 10 hft/min
       angleDeg = Math.min(angleDeg, maxAngleDeg); // limit to maximum angle
-      let angle = radians(angleDeg) * direction;
+      return radians(angleDeg) * direction;
+    }
+    function updateVSI(verticalSpeed) {
+      let angle = vsiAngleRadians(verticalSpeed);
 
       // positive vertical speed is lower y in svg
       vsiIndicator.setAttribute("y1", -Math.sin(angle) * vsiX1);
       vsiIndicator.setAttribute("y2", -Math.sin(angle) * vsiX2);
 
       let dialAngle = Math.max(-170, Math.min(170, verticalSpeed * 8));
       document.getElementById("vsidialIndicator").setAttribute("transform", `rotate(${dialAngle})`);
@@ -573,19 +660,111 @@
       if (rht !== null && isFinite(rht)) {
         document.getElementById("rhtTape").setAttribute("transform", `translate(0 ${rht})`);
       } else {
         document.getElementById("rhtTape").setAttribute("transform", `translate(0 0)`);
       }
     }
 
+    const trafficVolumeNames = ["OT", "PD", "TA", "RA"];
+    const trafficPerimeterRadius = document.getElementById("hsiTrafficPerimeter").getAttribute("r");
+    function updateTCAS(tcas) {
+      let counts = [0, 0, 0, 0];
+      for (const t of tcas) {
+        if (t.dist <= config.traffic_range) {
+          counts[t.vol] += 1;
+        }
+      }
+      for (let volumeIndex = 0; volumeIndex < 4; volumeIndex++) {
+        const volume = trafficVolumeNames[volumeIndex]
+        const volumeGroup = document.getElementById("hsiTraffic" + volume);
+        const count = counts[volumeIndex];
+        if (volumeGroup.childElementCount > count) {
+          for (let i = volumeGroup.childElementCount - count; i > 0; i--) {
+            volumeGroup.lastChild.remove();
+          }
+        } else if (volumeGroup.childElementCount < count) {
+          for (let i = count - volumeGroup.childElementCount; i > 0; i--) {
+            let clone = document.getElementById("traffic" + volume).cloneNode(true);
+            volumeGroup.appendChild(clone);
+          }
+        }
+      }
+
+      let nextChildIndex = [0, 0, 0, 0];
+      for (const t of tcas) {
+        if (t.dist <= config.traffic_range) {
+          const group = document.getElementById("hsiTraffic" + trafficVolumeNames[t.vol]);
+          let blip = group.children[nextChildIndex[t.vol]];
+          nextChildIndex[t.vol] += 1;
+
+          let r = t.dist / config.traffic_range * trafficPerimeterRadius;
+          let y = -Math.cos(t.brg) * r;
+          let x = Math.sin(t.brg) * r;
+          blip.setAttribute("transform", `translate(${x}, ${y})`);
+
+          // TODO: handle altitude text, position and arrow orientation
+          let hectofeet = Math.round(feet(t.alt) / 100.0);
+          let sign = hectofeet > 0 ? "+" : hectofeet < 0 ? "-" : "";
+          let altText = sign + Math.abs(hectofeet).toString().padStart(2, "0");
+          let textElement = blip.querySelector("text");
+          textElement.innerHTML = altText;
+          let ty = parseFloat(textElement.getAttribute("y"));
+          textElement.setAttribute("y", (hectofeet >= 0 ? -1 : 1) * Math.abs(ty));
+          blip.querySelector("path").setAttribute("transform", `scale(1, ${Math.sign(t.vsi)})`)
+        }
+      }
+    }
+
     function updateHSI(hdg) {
       document.getElementById("hsiWheel").setAttribute("transform", `rotate(${hdg})`);
     }
 
+    function updateRPM(rpmE, rpmR) {
+      for (const part of [[rpmE, "E"], [rpmR, "R"]]) {
+        const rpm = part[0];
+        const P = part[1];
+        const p = P.toLowerCase();
+
+        const x = Math.max(0, Math.min(120, rpm * 100));
+        const indicator = document.getElementById(`rpm${P}Indicator`);
+        const fillLow = document.getElementById(`rpm${P}FillLow`);
+        const fillHigh = document.getElementById(`rpm${P}FillHigh`);
+        const name = document.getElementById(`rpm${P}Name`);
+        const readout = document.getElementById(`rpm${P}Readout`);
+
+        indicator.setAttribute("transform", `translate(${x})`);
+        fillLow.setAttribute("fill", "black");
+        fillHigh.setAttribute("fill", "black");
+        name.setAttribute("fill", "white");
+        if (rpm >= config[`rpm_${p}_good_low`] && rpm <= config[`rpm_${p}_good_high`]) {
+          indicator.setAttribute("fill", "var(--pfdGreen)");
+        } else if (rpm >= config[`rpm_${p}_warn_low`] && rpm <= config[`rpm_${p}_warn_high`]) {
+          indicator.setAttribute("fill", "var(--pfdAmber)");
+        } else {
+          indicator.setAttribute("fill", "var(--pfdRed)");
+          if (rpm > 1.0) {
+            fillHigh.setAttribute("fill", "var(--pfdRed)");
+          } else {
+            fillLow.setAttribute("fill", "var(--pfdRed)");
+          }
+          name.setAttribute("fill", "var(--pfdRed)");
+        }
+
+        readout.textContent = `${Math.round(rpm * 100)}%`;
+      }
+    }
+
     const adiTargetIndicator = document.getElementById("adiTargetIndicator");
+    const iasTargetIndicator = document.getElementById("iasTargetIndicator");
+    const vsiTargetIndicator = document.getElementById("vsiTargetIndicator");
+    const vsiTargetX1 = parseFloat(vsiTargetIndicator.getAttribute("x1"));
+    const vsiTargetX2 = parseFloat(vsiTargetIndicator.getAttribute("x2"));
+    const vsiTargetIndicatorContour = document.getElementById("vsiTargetIndicatorContour");
+    const vsiTargetContourX1 = parseFloat(vsiTargetIndicator.getAttribute("x1"));
+    const vsiTargetContourX2 = parseFloat(vsiTargetIndicator.getAttribute("x2"));
     function updateTarget(s) {
       if ("att" in s.trgt && "att" in s) {
         const roll = degrees(s.att[0]);
         const pitch = degrees(s.att[1]);
         const yaw = degrees(s.att[2]);
         const targetRoll = degrees(s.trgt.att[0]);
         const targetPitch = degrees(s.trgt.att[1]);
@@ -597,18 +776,50 @@
           targetTransform = targetTransform + ` translate(${targetYaw - yaw})`;
         }
         if (config.adi_target_roll) {
           targetTransform = targetTransform + ` rotate(${targetRoll})`
         }
         adiTargetIndicator.setAttribute("transform", targetTransform);
       }
+      if ("v_ned" in s.trgt) {
+        vsiTargetIndicator.setAttribute("display", config.show_ias_target ? "block" : "none");
+        vsiTargetIndicatorContour.setAttribute("display", config.show_ias_target ? "block" : "none");
+
+        let angle = vsiAngleRadians(feet(s.trgt.v_ned[2]) * -0.6); // from m/s down to 100ft/min up
+
+        // positive vertical speed is lower y in svg
+        vsiTargetIndicator.setAttribute("y1", -Math.sin(angle) * vsiTargetX1);
+        vsiTargetIndicator.setAttribute("y2", -Math.sin(angle) * vsiTargetX2);
+        vsiTargetIndicatorContour.setAttribute("y1", -Math.sin(angle) * vsiTargetContourX1);
+        vsiTargetIndicatorContour.setAttribute("y2", -Math.sin(angle) * vsiTargetContourX2);
+      }
+      if ("instr" in s.trgt) {
+        if ("ias" in s.trgt.instr) {
+          iasTargetIndicator.setAttribute("display", config.show_ias_target ? "block" : "none");
+          iasTargetIndicator.setAttribute("transform", `translate(0 ${-s.trgt.instr.ias})`);
+        }
+      }
     }
 
     function updateLimits() {
       document.getElementById("iasVne").setAttribute("transform", `translate(0 ${-config.ias_never_exceed})`);
+      for (const P of ["E", "R"]) {
+        const p = P.toLowerCase();
+
+        for (const Area of ["Good", "Warn"]) {
+          const area = Area.toLowerCase();
+
+          const tape = document.getElementById(`rpm${P}Tape${Area}`);
+          const low = config[`rpm_${p}_${area}_low`];
+          const high = config[`rpm_${p}_${area}_high`];
+
+          tape.setAttribute("x", 100 * low);
+          tape.setAttribute("width", 100 * (high - low));
+        }
+      }
     }
 
     socket.on("smol", (s) => {
       if ("att" in s) {
         updateADI(degrees(s.att[0]), degrees(s.att[1]));
         updateHSI(degrees(s.att[2]));
       }
@@ -617,20 +828,24 @@
       }
       if ("v_body" in s) {
         updateFPV(s.v_body[0], s.v_body[1], s.v_body[2]); // units irrelevant
       }
       if ("a_body" in s) {
         updateSlip(s.a_body[1], s.a_body[2]); // units irrelevant
       }
+      if ("hrpm" in s) {
+        updateRPM(s.hrpm[1], s.hrpm[0]);
+      }
       if ("instr" in s) {
         if ("ias" in s.instr) updateIAS(s.instr.ias);
         if ("gs" in s.instr) updateGS(s.instr.gs);
         if ("alt" in s.instr) updateALT(s.instr.alt);
         if ("qnh" in s.instr) updateQNH(s.instr.qnh);
         if ("ralt" in s.instr) updateRHT(s.instr.ralt);
+        if ("tcas" in s.instr) updateTCAS(s.instr.tcas);
       }
       if ("trgt" in s) {
         updateTarget(s);
       }
     });
     socket.on("config", (s) => {
       if ("pfd" in s) {
@@ -638,8 +853,8 @@
         updateLimits();
       }
     });
     socket.emit("config_request", {});
   </script>
 </body>
 
-</html>
+</html>
```

#### html2text {}

```diff
@@ -1,6 +1,7 @@
 
-
-2 1 1 2         VSI  x100 FT/MIN UP DN                               00   40 20
-00 80 60 40 20 00 20 40 60 80 00 20 40       NEG     STD
-00   0 9 8 7 6 5 4 3 2 1 0 9       GS ---                       ---         N 3
-6 E 12 15 S 21 24 W 30 33              0    OAT 15 Â°C   No Ovly
+           +00     +00     +00     +00
+2 1 1 2           VSI  x100 FT/MIN UP DN                               00   40
+20 00 80 60 40 20 00 20 40 60 80 00 20 40       NEG     STD
+00   0 9 8 7 6 5 4 3 2 1 0 9       GS ---                       ---        E R
+00% 00%                                N 3 6 E 12 15 S 21 24 W 30 33
+0    OAT 15 Â°C   No Ovly
```

### Comparing `lidia-0.8.1/src/lidia/rpctask.html` & `lidia-0.9.0/src/lidia/rpctask.html`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/server.py` & `lidia-0.9.0/src/lidia/server.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/approach.py` & `lidia-0.9.0/src/lidia/sources/approach.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/confighelp.md` & `lidia-0.9.0/src/lidia/sources/confighelp.md`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/confighelp.py` & `lidia-0.9.0/src/lidia/sources/confighelp.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/flightgear.py` & `lidia-0.9.0/src/lidia/sources/flightgear.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/mytypes.py` & `lidia-0.9.0/src/lidia/sources/mytypes.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/rpctask.py` & `lidia-0.9.0/src/lidia/sources/rpctask.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/sources/smol.py` & `lidia-0.9.0/src/lidia/sources/smol.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/LICENSE.txt` & `lidia-0.9.0/src/lidia/static/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-Bold.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-ExtraLight.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-Light.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-Light.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-Medium.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-Medium.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-Regular.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-Regular.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-SemiBold.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-SemiBold.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/RobotoMono-Thin.ttf` & `lidia-0.9.0/src/lidia/static/RobotoMono-Thin.ttf`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/controls.js` & `lidia-0.9.0/src/lidia/static/controls.js`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/socket.io.js` & `lidia-0.9.0/src/lidia/static/socket.io.js`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/static/style.css` & `lidia-0.9.0/src/lidia/static/style.css`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/utils/pack_lidia.m` & `lidia-0.9.0/src/lidia/utils/pack_lidia.m`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia/utils/pack_maker.py` & `lidia-0.9.0/src/lidia/utils/pack_maker.py`

 * *Files identical despite different names*

### Comparing `lidia-0.8.1/src/lidia.egg-info/PKG-INFO` & `lidia-0.9.0/src/lidia.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lidia
-Version: 0.8.1
+Version: 0.9.0
 Summary: serve an aircraft instruments panel as a web page
 Home-page: https://gitlab.com/Maarrk/lidia
 Author: Marek S. Lukasiewicz
 Author-email: marek@lukasiewicz.tech
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `lidia-0.8.1/src/lidia.egg-info/SOURCES.txt` & `lidia-0.9.0/src/lidia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

