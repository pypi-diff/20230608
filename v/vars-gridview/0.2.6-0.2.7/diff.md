# Comparing `tmp/vars_gridview-0.2.6.tar.gz` & `tmp/vars_gridview-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vars_gridview-0.2.6.tar", max compression
+gzip compressed data, was "vars_gridview-0.2.7.tar", max compression
```

## Comparing `vars_gridview-0.2.6.tar` & `vars_gridview-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1104 2022-11-08 18:34:42.170730 vars_gridview-0.2.6/LICENSE
--rw-r--r--   0        0        0     1194 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/README.md
--rw-r--r--   0        0        0      862 2023-06-08 20:06:01.342538 vars_gridview-0.2.6/pyproject.toml
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.6/vars_gridview/__init__.py
--rw-r--r--   0        0        0      865 2023-03-24 17:40:22.606615 vars_gridview-0.2.6/vars_gridview/assets/base_query.sql
--rw-r--r--   0        0        0    24010 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/assets/gridview.ui
--rw-r--r--   0        0        0    31829 2022-11-08 18:34:42.170730 vars_gridview-0.2.6/vars_gridview/assets/style/dark.qss
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.162730 vars_gridview-0.2.6/vars_gridview/lib/__init__.py
--rw-r--r--   0        0        0     4963 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/annotation.py
--rw-r--r--   0        0        0     6242 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/boxes.py
--rw-r--r--   0        0        0      633 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/constants.py
--rw-r--r--   0        0        0    27011 2023-06-08 20:01:57.048947 vars_gridview-0.2.6/vars_gridview/lib/image_mosaic.py
--rw-r--r--   0        0        0     1733 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/log.py
--rw-r--r--   0        0        0     1680 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/m3/__init__.py
--rw-r--r--   0        0        0     5174 2023-06-08 19:33:40.306607 vars_gridview-0.2.6/vars_gridview/lib/m3/clients.py
--rw-r--r--   0        0        0     7188 2023-06-08 19:33:17.850773 vars_gridview-0.2.6/vars_gridview/lib/m3/operations.py
--rw-r--r--   0        0        0      729 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/raziel.py
--rw-r--r--   0        0        0     2645 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/settings.py
--rw-r--r--   0        0        0     3815 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/sort_methods.py
--rw-r--r--   0        0        0     3008 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/sql.py
--rw-r--r--   0        0        0     1887 2023-06-08 20:01:35.469166 vars_gridview-0.2.6/vars_gridview/lib/util.py
--rw-r--r--   0        0        0    10153 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/lib/widgets.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.170730 vars_gridview-0.2.6/vars_gridview/scripts/__init__.py
--rw-r--r--   0        0        0    22676 2023-06-08 20:04:03.911683 vars_gridview-0.2.6/vars_gridview/scripts/run.py
--rw-r--r--   0        0        0     2932 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/ui/LoginDialog.py
--rw-r--r--   0        0        0    16306 2023-03-24 17:40:22.606615 vars_gridview-0.2.6/vars_gridview/ui/QueryDialog.py
--rw-r--r--   0        0        0        0 2023-03-13 18:20:05.325704 vars_gridview-0.2.6/vars_gridview/ui/__init__.py
--rw-r--r--   0        0        0     2790 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/SettingsDialog.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.6/vars_gridview/ui/settings/__init__.py
--rw-r--r--   0        0        0      822 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
--rw-r--r--   0        0        0      710 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/M3Tab.py
--rw-r--r--   0        0        0     2004 2023-03-13 18:20:05.329704 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/SQLTab.py
--rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/__init__.py
--rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1104 2022-11-08 18:34:42.170730 vars_gridview-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1194 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/README.md
+-rw-r--r--   0        0        0      862 2023-06-08 21:20:02.027612 vars_gridview-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.7/vars_gridview/__init__.py
+-rw-r--r--   0        0        0      865 2023-03-24 17:40:22.606615 vars_gridview-0.2.7/vars_gridview/assets/base_query.sql
+-rw-r--r--   0        0        0    24010 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/assets/gridview.ui
+-rw-r--r--   0        0        0    31829 2022-11-08 18:34:42.170730 vars_gridview-0.2.7/vars_gridview/assets/style/dark.qss
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.162730 vars_gridview-0.2.7/vars_gridview/lib/__init__.py
+-rw-r--r--   0        0        0     4963 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/annotation.py
+-rw-r--r--   0        0        0     6242 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/boxes.py
+-rw-r--r--   0        0        0      633 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/constants.py
+-rw-r--r--   0        0        0    27206 2023-06-08 21:20:02.027612 vars_gridview-0.2.7/vars_gridview/lib/image_mosaic.py
+-rw-r--r--   0        0        0     1733 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/log.py
+-rw-r--r--   0        0        0     1680 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/m3/__init__.py
+-rw-r--r--   0        0        0     5174 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/lib/m3/clients.py
+-rw-r--r--   0        0        0     7188 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/lib/m3/operations.py
+-rw-r--r--   0        0        0      729 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/raziel.py
+-rw-r--r--   0        0        0     2645 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/settings.py
+-rw-r--r--   0        0        0     3815 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/sort_methods.py
+-rw-r--r--   0        0        0     3008 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/sql.py
+-rw-r--r--   0        0        0     1887 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/lib/util.py
+-rw-r--r--   0        0        0    10153 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/lib/widgets.py
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.170730 vars_gridview-0.2.7/vars_gridview/scripts/__init__.py
+-rw-r--r--   0        0        0    22676 2023-06-08 20:06:35.210212 vars_gridview-0.2.7/vars_gridview/scripts/run.py
+-rw-r--r--   0        0        0     2932 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/ui/LoginDialog.py
+-rw-r--r--   0        0        0    16306 2023-03-24 17:40:22.606615 vars_gridview-0.2.7/vars_gridview/ui/QueryDialog.py
+-rw-r--r--   0        0        0        0 2023-03-13 18:20:05.325704 vars_gridview-0.2.7/vars_gridview/ui/__init__.py
+-rw-r--r--   0        0        0     2790 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/SettingsDialog.py
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.7/vars_gridview/ui/settings/__init__.py
+-rw-r--r--   0        0        0      822 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py
+-rw-r--r--   0        0        0      710 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/M3Tab.py
+-rw-r--r--   0        0        0     2004 2023-03-13 18:20:05.329704 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/SQLTab.py
+-rw-r--r--   0        0        0        0 2022-11-08 18:34:42.158730 vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/__init__.py
+-rw-r--r--   0        0        0     2256 1970-01-01 00:00:00.000000 vars_gridview-0.2.7/PKG-INFO
```

### Comparing `vars_gridview-0.2.6/LICENSE` & `vars_gridview-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/README.md` & `vars_gridview-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/pyproject.toml` & `vars_gridview-0.2.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "vars-gridview"
-version = "0.2.6"
+version = "0.2.7"
 description = "VARS GridView is a tool for reviewing and correcting VARS localizations in bulk."
 authors = [
     "Kevin Barnard <kbarnard@mbari.org>",
     "Paul Roberts <proberts@mbari.org>"
 ]
 readme = "README.md"
 repository = "https://github.com/mbari-org/vars-gridview"
```

### Comparing `vars_gridview-0.2.6/vars_gridview/assets/base_query.sql` & `vars_gridview-0.2.7/vars_gridview/assets/base_query.sql`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/assets/gridview.ui` & `vars_gridview-0.2.7/vars_gridview/assets/gridview.ui`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/assets/style/dark.qss` & `vars_gridview-0.2.7/vars_gridview/assets/style/dark.qss`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/annotation.py` & `vars_gridview-0.2.7/vars_gridview/lib/annotation.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/boxes.py` & `vars_gridview-0.2.7/vars_gridview/lib/boxes.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/constants.py` & `vars_gridview-0.2.7/vars_gridview/lib/constants.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/image_mosaic.py` & `vars_gridview-0.2.7/vars_gridview/lib/image_mosaic.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,14 +164,17 @@
                 annotation_timestamp = get_timestamp(original_video_start_timestamp, recorded_timestamp, elapsed_time_millis, timecode)
                 
                 if annotation_timestamp is not None and video_reference_uuid is not None and video_reference_uuid not in self.video_reference_uuid_to_mp4_video_reference:
                     try:
                         video_sequence = operations.get_video_sequence_by_name(video_sequence_name)
                         for video in video_sequence["videos"]:
                             # Extract video time bounds
+                            if "start_timestamp" not in video or "duration_millis" not in video:  # invalid video, can't use
+                                continue
+                            
                             video_start_timestamp = parse_iso(video["start_timestamp"])
                             video_end_timestamp = video_start_timestamp + timedelta(milliseconds=video["duration_millis"])
                             
                             if not (video_start_timestamp <= annotation_timestamp <= video_end_timestamp):  # Annotation is not in this video
                                 continue
                             
                             for video_reference in video["video_references"]:
```

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/log.py` & `vars_gridview-0.2.7/vars_gridview/lib/log.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/m3/__init__.py` & `vars_gridview-0.2.7/vars_gridview/lib/m3/__init__.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/m3/clients.py` & `vars_gridview-0.2.7/vars_gridview/lib/m3/clients.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/m3/operations.py` & `vars_gridview-0.2.7/vars_gridview/lib/m3/operations.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/raziel.py` & `vars_gridview-0.2.7/vars_gridview/lib/raziel.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/settings.py` & `vars_gridview-0.2.7/vars_gridview/lib/settings.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/sort_methods.py` & `vars_gridview-0.2.7/vars_gridview/lib/sort_methods.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/sql.py` & `vars_gridview-0.2.7/vars_gridview/lib/sql.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/util.py` & `vars_gridview-0.2.7/vars_gridview/lib/util.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/lib/widgets.py` & `vars_gridview-0.2.7/vars_gridview/lib/widgets.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/scripts/run.py` & `vars_gridview-0.2.7/vars_gridview/scripts/run.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/ui/LoginDialog.py` & `vars_gridview-0.2.7/vars_gridview/ui/LoginDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/ui/QueryDialog.py` & `vars_gridview-0.2.7/vars_gridview/ui/QueryDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/ui/settings/SettingsDialog.py` & `vars_gridview-0.2.7/vars_gridview/ui/settings/SettingsDialog.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py` & `vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/AbstractSettingsTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/M3Tab.py` & `vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/M3Tab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/vars_gridview/ui/settings/tabs/SQLTab.py` & `vars_gridview-0.2.7/vars_gridview/ui/settings/tabs/SQLTab.py`

 * *Files identical despite different names*

### Comparing `vars_gridview-0.2.6/PKG-INFO` & `vars_gridview-0.2.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vars-gridview
-Version: 0.2.6
+Version: 0.2.7
 Summary: VARS GridView is a tool for reviewing and correcting VARS localizations in bulk.
 Home-page: https://github.com/mbari-org/vars-gridview
 License: MIT
 Keywords: VARS,localization,annotation
 Author: Kevin Barnard
 Author-email: kbarnard@mbari.org
 Requires-Python: >=3.8,<4.0
```

