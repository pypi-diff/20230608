# Comparing `tmp/dariusVision-0.0.4.tar.gz` & `tmp/dariusVision-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dariusVision-0.0.4.tar", last modified: Thu Jun  1 07:54:15 2023, max compression
+gzip compressed data, was "dariusVision-0.0.5.tar", last modified: Thu Jun  8 11:49:32 2023, max compression
```

## Comparing `dariusVision-0.0.4.tar` & `dariusVision-0.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-06-01 07:54:15.981321 dariusVision-0.0.4/
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)    35149 2023-04-07 04:46:45.000000 dariusVision-0.0.4/LICENSE
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      445 2023-06-01 07:54:15.981321 dariusVision-0.0.4/PKG-INFO
-drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-06-01 07:54:15.977321 dariusVision-0.0.4/dariusVision/
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      423 2023-06-01 07:48:43.000000 dariusVision-0.0.4/dariusVision/__init__.py
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     3265 2023-04-07 01:35:34.000000 dariusVision-0.0.4/dariusVision/cam.py
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)    10315 2023-06-01 07:50:31.000000 dariusVision-0.0.4/dariusVision/realsense2.py
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)     2011 2023-04-07 04:29:23.000000 dariusVision-0.0.4/dariusVision/utils.py
-drwxrwxr-x   0 gbox3d    (1000) gbox3d    (1000)        0 2023-06-01 07:54:15.981321 dariusVision-0.0.4/dariusVision.egg-info/
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      445 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/PKG-INFO
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      289 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/SOURCES.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)        1 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/dependency_links.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       33 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/requires.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       13 2023-06-01 07:54:15.000000 dariusVision-0.0.4/dariusVision.egg-info/top_level.txt
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)       38 2023-06-01 07:54:15.981321 dariusVision-0.0.4/setup.cfg
--rw-rw-r--   0 gbox3d    (1000) gbox3d    (1000)      644 2023-06-01 07:54:12.000000 dariusVision-0.0.4/setup.py
+drwxr-xr-x   0 gbox3d     (501) staff       (20)        0 2023-06-08 11:49:32.570355 dariusVision-0.0.5/
+-rw-r--r--   0 gbox3d     (501) staff       (20)    35149 2023-06-01 07:21:31.000000 dariusVision-0.0.5/LICENSE
+-rw-r--r--   0 gbox3d     (501) staff       (20)      445 2023-06-08 11:49:32.570229 dariusVision-0.0.5/PKG-INFO
+drwxr-xr-x   0 gbox3d     (501) staff       (20)        0 2023-06-08 11:49:32.569455 dariusVision-0.0.5/dariusVision/
+-rw-r--r--   0 gbox3d     (501) staff       (20)      423 2023-06-08 11:31:03.000000 dariusVision-0.0.5/dariusVision/__init__.py
+-rw-r--r--   0 gbox3d     (501) staff       (20)     3326 2023-06-08 11:46:33.000000 dariusVision-0.0.5/dariusVision/cam.py
+-rw-r--r--   0 gbox3d     (501) staff       (20)    10474 2023-06-08 11:30:22.000000 dariusVision-0.0.5/dariusVision/realsense2.py
+-rw-r--r--   0 gbox3d     (501) staff       (20)     2011 2023-06-01 07:21:31.000000 dariusVision-0.0.5/dariusVision/utils.py
+drwxr-xr-x   0 gbox3d     (501) staff       (20)        0 2023-06-08 11:49:32.570039 dariusVision-0.0.5/dariusVision.egg-info/
+-rw-r--r--   0 gbox3d     (501) staff       (20)      445 2023-06-08 11:49:32.000000 dariusVision-0.0.5/dariusVision.egg-info/PKG-INFO
+-rw-r--r--   0 gbox3d     (501) staff       (20)      289 2023-06-08 11:49:32.000000 dariusVision-0.0.5/dariusVision.egg-info/SOURCES.txt
+-rw-r--r--   0 gbox3d     (501) staff       (20)        1 2023-06-08 11:49:32.000000 dariusVision-0.0.5/dariusVision.egg-info/dependency_links.txt
+-rw-r--r--   0 gbox3d     (501) staff       (20)       33 2023-06-08 11:49:32.000000 dariusVision-0.0.5/dariusVision.egg-info/requires.txt
+-rw-r--r--   0 gbox3d     (501) staff       (20)       13 2023-06-08 11:49:32.000000 dariusVision-0.0.5/dariusVision.egg-info/top_level.txt
+-rw-r--r--   0 gbox3d     (501) staff       (20)       38 2023-06-08 11:49:32.570400 dariusVision-0.0.5/setup.cfg
+-rw-r--r--   0 gbox3d     (501) staff       (20)      644 2023-06-08 11:30:22.000000 dariusVision-0.0.5/setup.py
```

### Comparing `dariusVision-0.0.4/LICENSE` & `dariusVision-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.4/dariusVision/cam.py` & `dariusVision-0.0.5/dariusVision/cam.py`

 * *Files 8% similar despite different names*

```diff
@@ -49,21 +49,22 @@
         self.cap.release()
         self.cap = cv.VideoCapture(vid_src)
         self.bPause = False
         
 
     def read(self) :
         with self._critical_Section :
-            return (self.frame_status,self.frame.copy())
+            return self.frame_status,self.frame.copy()
         
     def getFrame(self) :
         if self.running == True :
-            return self.read()
+            status,frame = self.read()
+            return status,None,frame
         else :
-            return self.cap.read()
+            return self.running,None,self.cap.read()
         
     def startCamera(self) :
         self.cap = cv.VideoCapture(self.vid_src)
         self.cap.set(cv.CAP_PROP_FRAME_WIDTH, self.width)
         self.cap.set(cv.CAP_PROP_FRAME_HEIGHT, self.height)  
         
         if self.cap.isOpened():
```

### Comparing `dariusVision-0.0.4/dariusVision/realsense2.py` & `dariusVision-0.0.5/dariusVision/realsense2.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,26 +156,27 @@
         self.pipeline = None
         self.frame_status = False
     def getFrame(self) :
         
         if self._critical_Section is not None :
             with self._critical_Section : 
                 if self.frame_status :
-                    return True, self.depth_frame, self.color_frame
+                    #return True, self.depth_frame, self.color_frame
+                    return True,np.asanyarray(self.depth_frame.get_data()), np.asanyarray(self.color_frame.get_data())
                 else :
                     return False, None, None
         else :
             # frames = pipeline.wait_for_frames()
             frames = self.pipeline.wait_for_frames()
             aligned_frames = self.align.process(frames)
             self.depth_frame = aligned_frames.get_depth_frame()
             self.color_frame = aligned_frames.get_color_frame()
             self.frame_status = True # frame is ready
-            
-            return True, np.asanyarray(self.color_frame.get_data())
+            return True,np.asanyarray(self.depth_frame.get_data()), np.asanyarray(self.color_frame.get_data())
+        
     def getDepthFrame(self) :
         return True,self.depth_frame    
     
     def _getPoint3d(self, x, y) :
         if self.frame_status :
             depth = self.depth_frame.get_distance(x, y)
             # 2D 이미지 좌표를 3D 좌표계로 변환
```

### Comparing `dariusVision-0.0.4/dariusVision/utils.py` & `dariusVision-0.0.5/dariusVision/utils.py`

 * *Files identical despite different names*

### Comparing `dariusVision-0.0.4/setup.py` & `dariusVision-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='dariusVision',
-    version='0.0.4',
+    version='0.0.5',
     description='camera utilities to get last frame',
     long_description='camera utilities to get last frame',
     packages=['dariusVision'],
     install_requires=[
         'numpy',
         'opencv-python',
         'pyrealsense2',
```

