# Comparing `tmp/flet_ivid_hks-1.0.tar.gz` & `tmp/flet_ivid_hks-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flet_ivid_hks-1.0.tar", last modified: Wed Jun  7 08:44:15 2023, max compression
+gzip compressed data, was "flet_ivid_hks-1.1.tar", last modified: Thu Jun  8 02:58:43 2023, max compression
```

## Comparing `flet_ivid_hks-1.0.tar` & `flet_ivid_hks-1.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 08:44:15.686812 flet_ivid_hks-1.0/
--rw-rw-rw-   0        0        0     1081 2023-06-05 11:51:13.000000 flet_ivid_hks-1.0/LICENSE
--rw-rw-rw-   0        0        0       18 2023-06-05 11:51:13.000000 flet_ivid_hks-1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2227 2023-06-07 08:44:15.686812 flet_ivid_hks-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1798 2023-06-05 11:51:13.000000 flet_ivid_hks-1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 08:44:15.680309 flet_ivid_hks-1.0/example/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:56:27.000000 flet_ivid_hks-1.0/example/__init__.py
--rw-rw-rw-   0        0        0     3794 2023-06-06 18:02:59.000000 flet_ivid_hks-1.0/example/video_grid.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:44:15.681309 flet_ivid_hks-1.0/flet_ivid/
--rw-rw-rw-   0        0        0       45 2023-06-05 11:51:13.000000 flet_ivid_hks-1.0/flet_ivid/__init__.py
--rw-rw-rw-   0        0        0    10232 2023-06-06 03:41:06.000000 flet_ivid_hks-1.0/flet_ivid/video_container.py
-drwxrwxrwx   0        0        0        0 2023-06-07 08:44:15.685812 flet_ivid_hks-1.0/flet_ivid_hks.egg-info/
--rw-rw-rw-   0        0        0     2227 2023-06-07 08:44:15.000000 flet_ivid_hks-1.0/flet_ivid_hks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      330 2023-06-07 08:44:15.000000 flet_ivid_hks-1.0/flet_ivid_hks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 08:44:15.000000 flet_ivid_hks-1.0/flet_ivid_hks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-06-07 08:44:15.000000 flet_ivid_hks-1.0/flet_ivid_hks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-06-07 08:44:15.000000 flet_ivid_hks-1.0/flet_ivid_hks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      108 2023-06-05 11:51:13.000000 flet_ivid_hks-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 08:44:15.686812 flet_ivid_hks-1.0/setup.cfg
--rw-rw-rw-   0        0        0      689 2023-06-07 08:43:53.000000 flet_ivid_hks-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:58:43.301208 flet_ivid_hks-1.1/
+-rw-rw-rw-   0        0        0     1081 2023-06-05 11:51:13.000000 flet_ivid_hks-1.1/LICENSE
+-rw-rw-rw-   0        0        0       18 2023-06-05 11:51:13.000000 flet_ivid_hks-1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1491 2023-06-08 02:58:43.301208 flet_ivid_hks-1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1062 2023-06-08 02:55:17.000000 flet_ivid_hks-1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 02:58:43.293880 flet_ivid_hks-1.1/example/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:56:27.000000 flet_ivid_hks-1.1/example/__init__.py
+-rw-rw-rw-   0        0        0     4811 2023-06-08 02:56:59.000000 flet_ivid_hks-1.1/example/video_grid.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:58:43.295880 flet_ivid_hks-1.1/flet_ivid_hks/
+-rw-rw-rw-   0        0        0       45 2023-06-05 11:51:13.000000 flet_ivid_hks-1.1/flet_ivid_hks/__init__.py
+-rw-rw-rw-   0        0        0    11887 2023-06-08 02:53:31.000000 flet_ivid_hks-1.1/flet_ivid_hks/video_container.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:58:43.300207 flet_ivid_hks-1.1/flet_ivid_hks.egg-info/
+-rw-rw-rw-   0        0        0     1491 2023-06-08 02:58:43.000000 flet_ivid_hks-1.1/flet_ivid_hks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2023-06-08 02:58:43.000000 flet_ivid_hks-1.1/flet_ivid_hks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:58:43.000000 flet_ivid_hks-1.1/flet_ivid_hks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-08 02:58:43.000000 flet_ivid_hks-1.1/flet_ivid_hks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-08 02:58:43.000000 flet_ivid_hks-1.1/flet_ivid_hks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      108 2023-06-05 11:51:13.000000 flet_ivid_hks-1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:58:43.301208 flet_ivid_hks-1.1/setup.cfg
+-rw-rw-rw-   0        0        0      689 2023-06-08 02:57:26.000000 flet_ivid_hks-1.1/setup.py
```

### Comparing `flet_ivid_hks-1.0/LICENSE` & `flet_ivid_hks-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flet_ivid_hks-1.0/PKG-INFO` & `flet_ivid_hks-1.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,45 @@
 Metadata-Version: 2.1
 Name: flet_ivid_hks
-Version: 1.0
+Version: 1.1
 Summary: A package tool that provide basic video player for flet.
 Home-page: https://github.com/Uni-Gal/fork-flet_ived
 Author: SKbarbon, Hocassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# flet_ived
+# flet_ivid_hks
 A package tool that provide basic video player for flet. Its super easy to use, its built to be used as a normal `flet` control.
 
 ## installation
 To install, just type:
 
 ```
-pip install flet_ivid --upgrade
+pip install flet_ivid_hks --upgrade
 ```
 
 ## usage
 
 To start show your video inside your `flet` app, you can just import the `VideoContainer` control and use its properties, for example:
 
 ```python
-from flet_ivid import VideoContainer # import the package
+from flet_ivid_hks import VideoContainer # import the package
 import flet
 
 
 def main (page:flet.Page):
     page.bgcolor = "black"
     vc = VideoContainer("yourvideo.mp4", border_radius=18, expand=True) # This is a VideoContainer
     page.add(flet.Row([vc], alignment="center"))
 
     vc.play() # call `play` function to make the video start playing.
 
     # Call `vc.pause()` to stop the video from playing.
 
 flet.app(target=main)
-```
-
-### ⚠️ If your device is old!
-This package can load the video from file source while show the video at the same time. But this is not so with old devices or the devices that have a weak performance, So you must set `play_after_loading` to true. For example:
-
-```python
-from flet_ivid import VideoContainer # import the package
-import flet
-
-
-def main (page:flet.Page):
-    page.bgcolor = "black"
-    vc = VideoContainer("yourvideo.mp4", play_after_loading=True, border_radius=18, expand=True) # This is a VideoContainer
-    page.add(flet.Row([vc], alignment="center"))
-
-    vc.play() # call `play` function to make the video start playing.
-
-    # Call `vc.pause()` to stop the video from playing.
-
-flet.app(target=main)
 ```
 
 ## Note
 `Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, if you do so it will be a RAM consuming and slow for biger videos..**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flet_ivid_hks-1.0/README.md` & `flet_ivid_hks-1.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,33 @@
-# flet_ived
+# flet_ivid_hks
 A package tool that provide basic video player for flet. Its super easy to use, its built to be used as a normal `flet` control.
 
 ## installation
 To install, just type:
 
 ```
-pip install flet_ivid --upgrade
+pip install flet_ivid_hks --upgrade
 ```
 
 ## usage
 
 To start show your video inside your `flet` app, you can just import the `VideoContainer` control and use its properties, for example:
 
 ```python
-from flet_ivid import VideoContainer # import the package
+from flet_ivid_hks import VideoContainer # import the package
 import flet
 
 
 def main (page:flet.Page):
     page.bgcolor = "black"
     vc = VideoContainer("yourvideo.mp4", border_radius=18, expand=True) # This is a VideoContainer
     page.add(flet.Row([vc], alignment="center"))
 
     vc.play() # call `play` function to make the video start playing.
 
     # Call `vc.pause()` to stop the video from playing.
 
 flet.app(target=main)
-```
-
-### ⚠️ If your device is old!
-This package can load the video from file source while show the video at the same time. But this is not so with old devices or the devices that have a weak performance, So you must set `play_after_loading` to true. For example:
-
-```python
-from flet_ivid import VideoContainer # import the package
-import flet
-
-
-def main (page:flet.Page):
-    page.bgcolor = "black"
-    vc = VideoContainer("yourvideo.mp4", play_after_loading=True, border_radius=18, expand=True) # This is a VideoContainer
-    page.add(flet.Row([vc], alignment="center"))
-
-    vc.play() # call `play` function to make the video start playing.
-
-    # Call `vc.pause()` to stop the video from playing.
-
-flet.app(target=main)
 ```
 
 ## Note
 `Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, if you do so it will be a RAM consuming and slow for biger videos..**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flet_ivid_hks-1.0/flet_ivid/video_container.py` & `flet_ivid_hks-1.1/flet_ivid_hks/video_container.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,77 @@
 import base64
 import time
 
 
 class VideoContainer(Container):
     """This will show a video you choose."""
 
-    def __init__(self, video_path: str, play_after_loading=False, video_frame_fit_type: flet.ImageFit = None,
-                 video_progress_bar=True, video_play_button=False, content=None, ref=None, key=None, width=None,
-                 height=None, left=None,
-                 top=None, right=None, bottom=None, expand=None, col=None, opacity=None, rotate=None, scale=None,
-                 offset=None, aspect_ratio=None, animate_opacity=None, animate_size=None, animate_position=None,
-                 animate_rotation=None, animate_scale=None, animate_offset=None, on_animation_end=None, tooltip=None,
-                 visible=None, disabled=None, data=None, padding=None, margin=None, alignment=None, bgcolor=None,
-                 gradient=None, blend_mode=BlendMode.NONE, border=None, border_radius=None, image_src=None,
-                 image_src_base64=None, image_repeat=None, image_fit=None, image_opacity: OptionalNumber = None,
-                 shape=None, clip_behavior=None, ink=None, animate=None, blur=None, shadow=None, url=None,
-                 url_target=None, theme=None, theme_mode=None, on_click=None, on_long_press=None, on_hover=None):
+    def __init__(
+            self,
+            video_path: str,
+            play_after_loading=False,
+            video_frame_fit_type: flet.ImageFit = None,
+            video_progress_bar=True,
+            video_play_button=False,
+            exec_after_full_loaded=None,
+            only_show_cover=False,
+            content=None,
+            ref=None,
+            key=None,
+            width=None,
+            height=None,
+            left=None,
+            top=None,
+            right=None,
+            bottom=None,
+            expand=None,
+            col=None,
+            opacity=None,
+            rotate=None,
+            scale=None,
+            offset=None,
+            aspect_ratio=None,
+            animate_opacity=None,
+            animate_size=None,
+            animate_position=None,
+            animate_rotation=None,
+            animate_scale=None,
+            animate_offset=None,
+            on_animation_end=None,
+            tooltip=None,
+            visible=None,
+            disabled=None,
+            data=None,
+            padding=None,
+            margin=None,
+            alignment=None,
+            bgcolor=None,
+            gradient=None,
+            blend_mode=BlendMode.NONE,
+            border=None,
+            border_radius=None,
+            image_src=None,
+            image_src_base64=None,
+            image_repeat=None,
+            image_fit=None,
+            image_opacity: OptionalNumber = None,
+            shape=None,
+            clip_behavior=None,
+            ink=None,
+            animate=None,
+            blur=None,
+            shadow=None,
+            url=None,
+            url_target=None,
+            theme=None,
+            theme_mode=None,
+            on_click=None,
+            on_long_press=None,
+            on_hover=None
+    ):
         super().__init__(content, ref, key, width, height, left, top, right, bottom, expand, col, opacity, rotate,
                          scale, offset, aspect_ratio, animate_opacity, animate_size, animate_position, animate_rotation,
                          animate_scale, animate_offset, on_animation_end, tooltip, visible, disabled, data, padding,
                          margin, alignment, bgcolor, gradient, blend_mode, border, border_radius, image_src,
                          image_src_base64, image_repeat, image_fit, image_opacity, shape, clip_behavior, ink, animate,
                          blur, shadow, url, url_target, theme, theme_mode, on_click, on_long_press, on_hover)
 
@@ -39,29 +91,34 @@
         self.__video_pause_button = None
         self.__video_play_button = None
         self.__video_is_play = False
         self.vid_duration = None
         self.fps = 0
         self.__video_is_full_loaded = None
         self.video_frames = None
+        self.exec_after_full_loaded = exec_after_full_loaded
 
         if not os.path.isfile(video_path):
             raise FileNotFoundError("Cannot find the video at the path you set.")
 
-        self.__all_frames_of_video = []
+        self.all_frames_of_video = []
         self.__video_played = False
         self.video_progress_bar = video_progress_bar
         self.video_play_button = video_play_button
 
         if video_frame_fit_type is None:
             self.video_frame_fit_type = flet.ImageFit.CONTAIN
 
         # generate the UI
         self.__ui()
 
+        if only_show_cover:
+            self.read_video_cover(video_path)
+            return
+
         # start a video reader.
         if play_after_loading:
             print("Please wait the video is loading..\nThis will take a time based on your video size...")
             self.read_the_video(video_path)
         else:
             threading.Thread(target=self.read_the_video, args=[video_path], daemon=True).start()
 
@@ -181,17 +238,17 @@
         self.__video_played = True
         threading.Thread(target=self.__play, daemon=True).start()
 
     def __play(self):
         self.image_frames_viewer.visible = True
 
         num = self.__cur_play_frame
-        video_frames_len = len(self.__all_frames_of_video)
+        video_frames_len = len(self.all_frames_of_video)
 
-        for index, i in enumerate(self.__all_frames_of_video[self.__cur_play_frame:-1]):
+        for index, i in enumerate(self.all_frames_of_video[self.__cur_play_frame:-1]):
             if not self.__video_played:
                 self.__cur_play_frame = self.__cur_play_frame + index
                 break
             if index + self.__cur_play_frame == video_frames_len - 2:
                 self.__cur_play_frame = 0
 
             # update video progress bar
@@ -212,14 +269,31 @@
             num += 1
 
         self.show_play()
 
     def pause(self):
         self.__video_played = False
 
+    def read_video_cover(self, video_path):
+        video = cv2.VideoCapture(video_path)
+        frame_count = video.get(cv2.CAP_PROP_FRAME_COUNT)
+        slice_frame_num = frame_count / 2
+        video.set(cv2.CAP_PROP_POS_FRAMES, slice_frame_num)
+        success, frame = video.read()
+        _, buffer = cv2.imencode('.jpg', frame)
+        encoded_frame = base64.b64encode(buffer).decode('utf-8')
+
+        if self.image_frames_viewer.src_base64 is None:
+            self.image_frames_viewer.src_base64 = encoded_frame
+            self.image_frames_viewer.visible = True
+            if self.image_frames_viewer.page is not None:
+                self.image_frames_viewer.update()
+
+        video.release()
+
     def read_the_video(self, video_path):
         # Open the video file
         video = cv2.VideoCapture(video_path)
 
         # Iterate over each frame and encode it
         success, frame = video.read()
 
@@ -227,30 +301,33 @@
             # Encode the frame as JPEG
             _, buffer = cv2.imencode('.jpg', frame)
 
             # Base64 encode the buffer
             encoded_frame = base64.b64encode(buffer).decode('utf-8')
 
             # Store the base64-encoded frame in the list
-            self.__all_frames_of_video.append(encoded_frame)
+            self.all_frames_of_video.append(encoded_frame)
 
             # check if the image is shown
             if self.image_frames_viewer.src_base64 is None:
                 self.image_frames_viewer.src_base64 = encoded_frame
                 self.image_frames_viewer.visible = True
                 if self.image_frames_viewer.page is not None:
                     self.image_frames_viewer.update()
 
             success, frame = video.read()
 
         # Release the video object
         video.release()
 
         self.__video_is_full_loaded = True
-        return self.__all_frames_of_video
+        # exec callback
+        if self.exec_after_full_loaded:
+            self.exec_after_full_loaded()
+        return self.all_frames_of_video
 
     def get_video_duration(self, video_path):
         cap = cv2.VideoCapture(video_path)
         if not cap.isOpened():
             print("Error opening video file")
             return
```

### Comparing `flet_ivid_hks-1.0/flet_ivid_hks.egg-info/PKG-INFO` & `flet_ivid_hks-1.1/flet_ivid_hks.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,65 +1,45 @@
 Metadata-Version: 2.1
 Name: flet-ivid-hks
-Version: 1.0
+Version: 1.1
 Summary: A package tool that provide basic video player for flet.
 Home-page: https://github.com/Uni-Gal/fork-flet_ived
 Author: SKbarbon, Hocassian
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# flet_ived
+# flet_ivid_hks
 A package tool that provide basic video player for flet. Its super easy to use, its built to be used as a normal `flet` control.
 
 ## installation
 To install, just type:
 
 ```
-pip install flet_ivid --upgrade
+pip install flet_ivid_hks --upgrade
 ```
 
 ## usage
 
 To start show your video inside your `flet` app, you can just import the `VideoContainer` control and use its properties, for example:
 
 ```python
-from flet_ivid import VideoContainer # import the package
+from flet_ivid_hks import VideoContainer # import the package
 import flet
 
 
 def main (page:flet.Page):
     page.bgcolor = "black"
     vc = VideoContainer("yourvideo.mp4", border_radius=18, expand=True) # This is a VideoContainer
     page.add(flet.Row([vc], alignment="center"))
 
     vc.play() # call `play` function to make the video start playing.
 
     # Call `vc.pause()` to stop the video from playing.
 
 flet.app(target=main)
-```
-
-### ⚠️ If your device is old!
-This package can load the video from file source while show the video at the same time. But this is not so with old devices or the devices that have a weak performance, So you must set `play_after_loading` to true. For example:
-
-```python
-from flet_ivid import VideoContainer # import the package
-import flet
-
-
-def main (page:flet.Page):
-    page.bgcolor = "black"
-    vc = VideoContainer("yourvideo.mp4", play_after_loading=True, border_radius=18, expand=True) # This is a VideoContainer
-    page.add(flet.Row([vc], alignment="center"))
-
-    vc.play() # call `play` function to make the video start playing.
-
-    # Call `vc.pause()` to stop the video from playing.
-
-flet.app(target=main)
 ```
 
 ## Note
 `Note`: **You should know that this built to be used for basic small or normal usage, its can NOT be used for big production cases, if you do so it will be a RAM consuming and slow for biger videos..**
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `flet_ivid_hks-1.0/setup.py` & `flet_ivid_hks-1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", encoding="utf-8") as f:
     long_des = str(f.read())
 
 setup(
     name='flet_ivid_hks',
-    version='1.0',
+    version='1.1',
     author='SKbarbon, Hocassian',
     description='A package tool that provide basic video player for flet.',
     long_description=long_des,
     long_description_content_type='text/markdown',
     url='https://github.com/Uni-Gal/fork-flet_ived',
     install_requires=["flet", "opencv-python"],
     packages=find_packages(),
```

