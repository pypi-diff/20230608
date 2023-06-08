# Comparing `tmp/rendersrt-0.0.5.tar.gz` & `tmp/rendersrt-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rendersrt-0.0.5.tar", last modified: Wed Jun  7 15:14:09 2023, max compression
+gzip compressed data, was "rendersrt-0.0.6.tar", last modified: Thu Jun  8 00:50:45 2023, max compression
```

## Comparing `rendersrt-0.0.5.tar` & `rendersrt-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:14:09.179800 rendersrt-0.0.5/
--rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     1563 2023-06-07 15:14:09.180549 rendersrt-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 15:14:09.122926 rendersrt-0.0.5/rendersrt/
--rw-rw-rw-   0        0        0    58233 2023-06-07 15:12:20.000000 rendersrt-0.0.5/rendersrt/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:14:09.177552 rendersrt-0.0.5/rendersrt.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      270 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       34 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-07 15:14:08.000000 rendersrt-0.0.5/rendersrt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      147 2023-06-07 15:14:09.184851 rendersrt-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:50:45.879198 rendersrt-0.0.6/
+-rw-rw-rw-   0        0        0     1087 2023-01-06 18:50:17.000000 rendersrt-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0       34 2023-01-06 18:50:17.000000 rendersrt-0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0     1563 2023-06-08 00:50:45.879198 rendersrt-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     3055 2023-05-25 12:05:46.000000 rendersrt-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 00:50:45.784274 rendersrt-0.0.6/rendersrt/
+-rw-rw-rw-   0        0        0    58891 2023-06-08 00:48:12.000000 rendersrt-0.0.6/rendersrt/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:50:45.876202 rendersrt-0.0.6/rendersrt.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       34 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-08 00:50:45.000000 rendersrt-0.0.6/rendersrt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      147 2023-06-08 00:50:45.883696 rendersrt-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1362 2023-06-07 15:11:16.000000 rendersrt-0.0.6/setup.py
```

### Comparing `rendersrt-0.0.5/LICENSE` & `rendersrt-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.5/PKG-INFO` & `rendersrt-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.5
+Version: 0.0.6
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.5/README.md` & `rendersrt-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `rendersrt-0.0.5/rendersrt/__init__.py` & `rendersrt-0.0.6/rendersrt/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import shlex
 import json
 import pysrt
 from pathlib import Path
 from datetime import datetime, timedelta
 
 
-VERSION = "0.0.5"
+VERSION = "0.0.6"
 
 
 class Language:
     def __init__(self):
         self.list_codes = []
         self.list_codes.append("af")
         self.list_codes.append("sq")
@@ -937,21 +937,36 @@
             if self.error_messages_callback:
                 self.error_messages_callback("ffmpeg: Executable not found on machine.")
             else:
                 print("ffmpeg: Executable not found on machine.")
                 raise Exception("Dependency not found: ffmpeg")
 
         try:
+            '''
             ffmpeg_command = [
                                 "ffmpeg",
                                 "-y",
                                 "-i", media_filepath,
                                 "-vf", f"subtitles={shlex.quote(self.subtitle_path)}",
                                 "-y", self.output_path
                              ]
+            '''
+
+            scale_switch = "'trunc(iw/2)*2':'trunc(ih/2)*2'"
+            ffmpeg_command = [
+                                "ffmpeg",
+                                "-y",
+                                "-i", media_filepath,
+                                "-vf", f"subtitles={shlex.quote(self.subtitle_path)},scale={scale_switch}",
+                                "-c:v", "libx264",
+                                "-crf", "23",
+                                "-preset", "medium",
+                                "-c:a", "copy",
+                                self.output_path
+                             ]
 
             ffprobe_command = f'ffprobe -v error -show_entries format=duration -of default=noprint_wrappers=1:nokey=1 "{media_filepath}"'
 
             if sys.platform == "win32":
                 ffprobe_process = subprocess.Popen(ffprobe_command, shell=True, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
             else:
                 ffprobe_process = subprocess.Popen(ffprobe_command, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
@@ -1297,15 +1312,14 @@
                 if ffmpeg_src_language_code in subtitle_stream_parser.languages():
                     print("Is '%s' subtitle stream exist       : Yes" %(ffmpeg_src_language_code.center(3)))
                 else:
                     print("Is '%s' subtitle stream exist       : No" %(ffmpeg_src_language_code.center(3)))
 
                     #result = render_subtitle_to_media(media_filepaths[0], media_type, valid_subtitle_paths[0], language_code, output_path, error_messages_callback=None)
 
-
                     widgets = [f"Rendering \'{language_code}\' subtitles with {media_type} : ", Percentage(), ' ', Bar(marker="#"), ' ', ETA()]
                     pbar = ProgressBar(widgets=widgets, maxval=100).start()
                     subtitle_renderer = MediaSubtitleRenderer(subtitle_path=valid_subtitle_paths[0], language=language_code, output_path=output_path, progress_callback=show_progress, error_messages_callback=show_error_messages)
                     result = subtitle_renderer(media_filepaths[0])
                     pbar.finish()
```

### Comparing `rendersrt-0.0.5/rendersrt.egg-info/PKG-INFO` & `rendersrt-0.0.6/rendersrt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rendersrt
-Version: 0.0.5
+Version: 0.0.6
 Summary: a utility for rendering subtitle file into video file
 Home-page: https://github.com/botbahlul/rendersrt
 Author: Bot Bahlul
 Author-email: bot.bahlul@gmail.com
 License: MIT License
         
         Copyright (c) 2022 botbahlul
```

### Comparing `rendersrt-0.0.5/setup.py` & `rendersrt-0.0.6/setup.py`

 * *Files identical despite different names*

