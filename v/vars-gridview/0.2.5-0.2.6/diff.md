# Comparing `tmp/vars_gridview-0.2.5.tar.gz` & `tmp/vars_gridview-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.2.5.tar", max compression
+gzip compressed data, was "vars_gridview-0.2.6.tar", max compression
```

## Comparing `vars_gridview-0.2.5.tar` & `vars_gridview-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0     1104 2022-11-08 18:34:42.170730 vars_gridview-0.2.5/LICENSE
--rw-r--r--   0        0        0     1194 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/README.md
--rw-r--r--   0        0        0      862 2023-03-24 18:20:23.292837 vars_gridview-0.2.5/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.5/vars_gridview/__init__.py
--rw-r--r--   0        0        0      865 2023-03-24 17:40:22.606615 vars_gridview-0.2.5/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    24010 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0    31829 2022-11-08 18:34:42.170730 vars_gridview-0.2.5/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.162730 vars_gridview-0.2.5/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     4963 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     6242 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0      633 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    26200 2023-03-24 17:40:22.606615 vars_gridview-0.2.5/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1733 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     1680 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5039 2023-03-24 17:40:22.606615 vars_gridview-0.2.5/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0     6880 2023-03-24 17:40:22.606615 vars_gridview-0.2.5/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2645 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     3815 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3008 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0    10153 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.170730 vars_gridview-0.2.5/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    22392 2023-03-24 18:20:23.292837 vars_gridview-0.2.5/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     2932 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    16306 2023-03-24 17:40:22.606615 vars_gridview-0.2.5/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0        0 2023-03-13 18:20:05.325704 vars_gridview-0.2.5/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     2790 2023-03-13 18:20:05.329704 vars_gridview-0.2.5/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.5/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-03-13 18:20:05.329704 vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0      710 2023-03-13 18:20:05.329704 vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2004 2023-03-13 18:20:05.329704 vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0     1104 2022-11-08 18:34:42.170730 vars_gridview-0.2.6/LICENSE
+-rw-r--r--   0        0        0     1194 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/README.md
+-rw-r--r--   0        0        0      862 2023-06-08 20:06:01.342538 vars_gridview-0.2.6/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.6/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-24 17:40:22.606615 vars_gridview-0.2.6/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    24010 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0    31829 2022-11-08 18:34:42.170730 vars_gridview-0.2.6/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.162730 vars_gridview-0.2.6/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     4963 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     6242 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0      633 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    27011 2023-06-08 20:01:57.048947 vars_gridview-0.2.6/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1733 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     1680 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5174 2023-06-08 19:33:40.306607 vars_gridview-0.2.6/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0     7188 2023-06-08 19:33:17.850773 vars_gridview-0.2.6/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2645 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     3815 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3008 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     1887 2023-06-08 20:01:35.469166 vars_gridview-0.2.6/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    10153 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.170730 vars_gridview-0.2.6/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    22676 2023-06-08 20:04:03.911683 vars_gridview-0.2.6/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     2932 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    16306 2023-03-24 17:40:22.606615 vars_gridview-0.2.6/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0        0 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     2790 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.6/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0      710 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2004 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.6/PKG-INFO
```

### Comparing `vars_gridview-0.2.5/LICENSE` & `vars_gridview-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/README.md` & `vars_gridview-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/pyproject.toml` & `vars_gridview-0.2.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.2.5"
+version = "0.2.6"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
```

### Comparing `vars_gridview-0.2.5/vars_gridview/assets/base_query.sql` & `vars_gridview-0.2.6/vars_gridview/assets/base_query.sql`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/assets/gridview.ui` & `vars_gridview-0.2.6/vars_gridview/assets/gridview.ui`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.2.6/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/annotation.py` & `vars_gridview-0.2.6/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/boxes.py` & `vars_gridview-0.2.6/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/constants.py` & `vars_gridview-0.2.6/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.2.6/vars_gridview/lib/image_mosaic.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,29 @@
 """
 image_mosaic.py -- A set of classes to extend widgets from pyqtgraph and pyqt for annotation purposes
 Copyright 2020  Monterey Bay Aquarium Research Institute
 Distributed under MIT license. See license.txt for more infomation.
 
 """
 
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import List, Optional
 from uuid import UUID
 
 import cv2
 import numpy as np
 import pyqtgraph as pg
 import requests
 from PyQt6 import QtCore, QtWidgets
 
 from vars_gridview.lib.annotation import VARSLocalization
 from vars_gridview.lib.log import LOGGER
 from vars_gridview.lib.m3 import operations
 from vars_gridview.lib.sort_methods import SortMethod
+from vars_gridview.lib.util import get_timestamp, parse_iso
 from vars_gridview.lib.widgets import RectWidget
 from vars_gridview.lib.constants import IMAGE_TYPE
 
 
 class ImageMosaic(QtCore.QObject):
     """
     Manager of the image mosaic widget
@@ -133,36 +134,59 @@
                     for k in (  # Video data keys
                         "index_elapsed_time_millis",
                         "index_timecode",
                         "index_recorded_timestamp",
                         "video_start_timestamp",
                         "video_uri",
                         "video_container",
-                        "video_reference_uuid"
+                        "video_reference_uuid",
+                        "video_sequence_name"
                     )
                 }
 
                 # Tag in video data where appropriate
                 if video_data.get("video_uri", None) is not None:  # valid video
                     if imaged_moment_uuid not in self.moment_video_data:
                         self.moment_video_data[imaged_moment_uuid] = video_data
 
                 # Find the corresponding MP4 video reference for this video reference, if there is one
                 video_reference_uuid = query_item["video_reference_uuid"]
-                if video_reference_uuid is not None and video_reference_uuid not in self.video_reference_uuid_to_mp4_video_reference:
+                video_sequence_name = query_item["video_sequence_name"]
+                
+                original_video_start_timestamp = video_data["video_start_timestamp"]
+                    
+                elapsed_time_millis = video_data.get(
+                    "index_elapsed_time_millis", None
+                )
+                timecode = video_data.get("index_timecode", None)
+                recorded_timestamp = video_data.get("index_recorded_timestamp", None)
+
+                # Get annotation video time index
+                annotation_timestamp = get_timestamp(original_video_start_timestamp, recorded_timestamp, elapsed_time_millis, timecode)
+                
+                if annotation_timestamp is not None and video_reference_uuid is not None and video_reference_uuid not in self.video_reference_uuid_to_mp4_video_reference:
                     try:
-                        video_data = operations.get_video_by_video_reference_uuid(video_reference_uuid)
-                        for video_reference in video_data["video_references"]:
-                            if video_reference.get("container", None) == "video/mp4":
-                                self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = video_reference
-                                break
-                        else:
-                            self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = None
+                        video_sequence = operations.get_video_sequence_by_name(video_sequence_name)
+                        for video in video_sequence["videos"]:
+                            # Extract video time bounds
+                            video_start_timestamp = parse_iso(video["start_timestamp"])
+                            video_end_timestamp = video_start_timestamp + timedelta(milliseconds=video["duration_millis"])
+                            
+                            if not (video_start_timestamp <= annotation_timestamp <= video_end_timestamp):  # Annotation is not in this video
+                                continue
+                            
+                            for video_reference in video["video_references"]:
+                                if video_reference.get("container", None) == "video/mp4":
+                                    self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = video_reference
+                                    video_data["proxy_mp4"] = video
+                                    break
+                            else:
+                                self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = None
                     except requests.exceptions.HTTPError as e:
-                        LOGGER.error(f"Could not get video data for video reference {video_reference_uuid}: {e}")
+                        LOGGER.error(f"Could not get video sequence data for name {video_sequence_name}: {e}")
                         self.video_reference_uuid_to_mp4_video_reference[video_reference_uuid] = None
 
                 # Collect bounding boxes
                 if link_name == "bounding box":
                     if association_uuid in seen_associations:
                         continue
                     seen_associations.add(association_uuid)
@@ -221,48 +245,36 @@
                             LOGGER.warning(
                                 "No web video available for capture for moment: {}, skipping".format(
                                     imaged_moment_uuid
                                 )
                             )
                             continue
 
-                    # Compute the elapsed time in milliseconds of the annotation into the video
-                    elapsed_time_millis = None
+                    video_start_timestamp = original_video_data["video_start_timestamp"]  # TODO check this
                     
-                    video_start_datetime = original_video_data["video_start_timestamp"]
                     elapsed_time_millis = original_video_data.get(
                         "index_elapsed_time_millis", None
                     )
                     timecode = original_video_data.get("index_timecode", None)
                     recorded_timestamp = original_video_data.get("index_recorded_timestamp", None)
 
                     # Get annotation video time index
-                    annotation_datetime = None
-                    if recorded_timestamp is not None:
-                        annotation_datetime = recorded_timestamp
-                    elif elapsed_time_millis is not None:
-                        annotation_datetime = video_start_datetime + datetime.timedelta(
-                            milliseconds=int(elapsed_time_millis)
-                        )
-                    elif timecode is not None:
-                        hours, minutes, seconds, frames = map(int, timecode.split(":"))
-                        annotation_datetime = video_start_datetime + datetime.timedelta(
-                            hours=hours, minutes=minutes, seconds=seconds
-                        )
-                    else:
+                    annotation_timestamp = get_timestamp(video_start_timestamp, recorded_timestamp, elapsed_time_millis, timecode)
+                    
+                    if annotation_timestamp is None:
                         LOGGER.error(
                             "No time index available for moment: {}, skipping".format(
                                 imaged_moment_uuid
                             )
                         )
                         continue
 
                     # Compute the elapsed time in milliseconds
                     elapsed_time_millis = round(
-                        (annotation_datetime - video_start_datetime).total_seconds()
+                        (annotation_timestamp - video_start_timestamp).total_seconds()
                         * 1000
                     )
                     
                     # Get the capture from beholder
                     LOGGER.debug(f"Getting capture from beholder for moment: {imaged_moment_uuid} ({video_uri} @ {elapsed_time_millis} ms)")
                     try:
                         res = requests.post(
```

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/log.py` & `vars_gridview-0.2.6/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.2.6/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.2.6/vars_gridview/lib/m3/clients.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,14 +153,17 @@
         return self.get(f"/videos/timestamp/{timestamp}")
     
     def get_video_by_video_reference_uuid(self, video_reference_uuid: str) -> requests.Response:
         return self.get(f"/videos/videoreference/{video_reference_uuid}")
     
     def get_video_sequence_names(self) -> requests.Response:
         return self.get("/videosequences/names")
+    
+    def get_video_sequence_by_name(self, name: str) -> requests.Response:
+        return self.get(f"/videosequences/name/{name}")
 
 
 class VARSUserServerClient(M3Client):
     """
     VARS user server (v1) client.
     """
```

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.2.6/vars_gridview/lib/m3/operations.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 M3 operations. Make use of the clients defined in __init__.py.
 """
 
 import json
 from datetime import datetime
-from typing import List
+from typing import List, Optional
 
 import requests
 
 from vars_gridview.lib import m3
 from vars_gridview.lib.log import LOGGER
 
 KB_CONCEPTS = None
@@ -210,14 +210,25 @@
         video_reference_uuid
     )
 
     response.raise_for_status()
     return response.json()
 
 
+def get_video_sequence_by_name(name: str) -> dict:
+    """
+    Get a video sequence by name.
+    """
+    LOGGER.debug(f"Getting video sequence by name {name}")
+    response = m3.VAMPIRE_SQUID_CLIENT.get_video_sequence_by_name(name)
+    
+    response.raise_for_status()
+    return response.json()
+
+
 def get_vars_imaged_moment(image_reference_uuid: str) -> dict:
     """
     Get MBARI VARS imaged moment by UUID.
     This will not work unless you are connected to the MBARI network!
     """
     LOGGER.debug(f"Getting VARS imaged moment {image_reference_uuid}")
     response = requests.get(
```

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/raziel.py` & `vars_gridview-0.2.6/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/settings.py` & `vars_gridview-0.2.6/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.2.6/vars_gridview/lib/sort_methods.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/sql.py` & `vars_gridview-0.2.6/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/lib/widgets.py` & `vars_gridview-0.2.6/vars_gridview/lib/widgets.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/scripts/run.py` & `vars_gridview-0.2.6/vars_gridview/scripts/run.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     MeanHueSort,
     MeanIntensitySort,
     ObservationUUIDSort,
     RecordedTimestampSort,
     RegionMeanHueSort,
     WidthSort,
 )
+from vars_gridview.lib.util import parse_iso
 from vars_gridview.lib.widgets import RectWidget
 from vars_gridview.ui.LoginDialog import LoginDialog
 from vars_gridview.ui.QueryDialog import QueryDialog
 from vars_gridview.ui.settings.SettingsDialog import SettingsDialog
 
 # Define main window class from template
 CWD = Path(__file__).parent
@@ -537,15 +538,22 @@
             return
 
         # Get the annotation recorded datetime
         annotation_datetime = self.last_selected_rect.annotation_datetime()
         
         # Get the annotation video reference UUID and start timestamp
         video_reference_uuid = self.last_selected_rect.video_data.get("video_reference_uuid", None)
-        video_start_datetime = self.last_selected_rect.video_data.get("video_start_timestamp", None)
+        proxy_mp4 = self.last_selected_rect.video_data.get("proxy_mp4", None)
+        if proxy_mp4 is None:
+            QtWidgets.QMessageBox.warning(
+                self, "Missing Video", "ROI lacks MP4 video."
+            )
+            return
+            
+        video_start_datetime = proxy_mp4.get("start_timestamp", None)
         
         # Exit if we don't have what we need
         if annotation_datetime is None or video_reference_uuid is None or video_start_datetime is None:
             QtWidgets.QMessageBox.warning(
                 self, "Missing Info", "ROI lacks necessary information to link video."
             )
             return
@@ -557,15 +565,15 @@
                 self, "Missing Video", "ROI lacks MP4 video."
             )
             return
 
         mp4_video_url = mp4_video_reference.get("uri", None)
 
         # Compute the timedelta between the annotation and video start
-        annotation_timedelta = annotation_datetime - video_start_datetime
+        annotation_timedelta = annotation_datetime - parse_iso(video_start_datetime)
 
         # Open the MP4 video at the computed timedelta (in seconds)
         annotation_seconds = max(annotation_timedelta.total_seconds(), 0)
         url = mp4_video_url + "#t={},{}".format(
             annotation_seconds, annotation_seconds + 1e-3
         )  # "pause" at the annotation
         webbrowser.open(url)
```

### Comparing `vars_gridview-0.2.5/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.2.6/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.2.6/vars_gridview/ui/QueryDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.2.6/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.5/PKG-INFO` & `vars_gridview-0.2.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.2.5
+Version: 0.2.6
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
```

