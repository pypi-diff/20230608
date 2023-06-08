# Comparing `tmp/faceshine-1.0.3-py3-none-any.whl.zip` & `tmp/faceshine-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 23265 bytes, number of entries: 35
--rw-rw-r--  2.0 unx      239 b- defN 23-Jun-07 23:46 faceshine/__init__.py
+Zip file size: 23261 bytes, number of entries: 35
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jun-08 00:05 faceshine/__init__.py
 -rw-rw-r--  2.0 unx      602 b- defN 23-Jun-02 05:58 faceshine/__main__.py
 -rw-rw-r--  2.0 unx     2857 b- defN 23-Jun-07 07:04 faceshine/app.py
 -rw-rw-r--  2.0 unx      992 b- defN 23-Jun-05 22:49 faceshine/utils.py
 -rw-rw-r--  2.0 unx      276 b- defN 23-Jun-06 23:44 faceshine/tasks/__init__.py
 -rw-rw-r--  2.0 unx      131 b- defN 23-Jun-05 22:42 faceshine/tasks/base/__init__.py
 -rw-rw-r--  2.0 unx      380 b- defN 23-Apr-20 16:29 faceshine/tasks/base/ai_enhancer.py
 -rw-rw-r--  2.0 unx      367 b- defN 23-Apr-21 18:27 faceshine/tasks/base/ai_preprocces.py
@@ -24,14 +24,14 @@
 -rw-rw-r--  2.0 unx     2017 b- defN 23-Apr-07 15:54 faceshine/tasks/lowlight/model/model.py
 -rw-rw-r--  2.0 unx       53 b- defN 23-Jun-02 03:13 faceshine/tasks/segmentation/__init__.py
 -rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-05 19:27 faceshine/tasks/segmentation/task_zero_background.py
 -rw-rw-r--  2.0 unx       43 b- defN 23-Jun-06 22:04 faceshine/tasks/superface/__init__.py
 -rw-rw-r--  2.0 unx     3112 b- defN 23-Jun-07 22:35 faceshine/tasks/superface/task_super_face.py
 -rw-rw-r--  2.0 unx       54 b- defN 23-Jun-06 03:50 faceshine/tasks/zeroscratches/__init__.py
 -rw-rw-r--  2.0 unx      687 b- defN 23-Jun-06 04:07 faceshine/tasks/zeroscratches/task_erase_scratches.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-07 23:50 faceshine-1.0.3.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2205 b- defN 23-Jun-07 23:50 faceshine-1.0.3.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 23:50 faceshine-1.0.3.dist-info/WHEEL
--rw-rw-r--  2.0 unx       54 b- defN 23-Jun-07 23:50 faceshine-1.0.3.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-07 23:50 faceshine-1.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     3218 b- defN 23-Jun-07 23:50 faceshine-1.0.3.dist-info/RECORD
-35 files, 52483 bytes uncompressed, 17967 bytes compressed:  65.8%
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-08 00:05 faceshine-1.0.4.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2192 b- defN 23-Jun-08 00:05 faceshine-1.0.4.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-08 00:05 faceshine-1.0.4.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jun-08 00:05 faceshine-1.0.4.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-08 00:05 faceshine-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3218 b- defN 23-Jun-08 00:05 faceshine-1.0.4.dist-info/RECORD
+35 files, 52470 bytes uncompressed, 17963 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -81,26 +81,26 @@
 
 Filename: faceshine/tasks/zeroscratches/__init__.py
 Comment: 
 
 Filename: faceshine/tasks/zeroscratches/task_erase_scratches.py
 Comment: 
 
-Filename: faceshine-1.0.3.dist-info/LICENSE
+Filename: faceshine-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: faceshine-1.0.3.dist-info/METADATA
+Filename: faceshine-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: faceshine-1.0.3.dist-info/WHEEL
+Filename: faceshine-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: faceshine-1.0.3.dist-info/entry_points.txt
+Filename: faceshine-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: faceshine-1.0.3.dist-info/top_level.txt
+Filename: faceshine-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: faceshine-1.0.3.dist-info/RECORD
+Filename: faceshine-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## faceshine/__init__.py

```diff
@@ -1,9 +1,9 @@
 __appname__ = "Face Shine"
-__version__ = "1.0.3"
+__version__ = "1.0.4"
 
 from .utils import tensor_to_ndarray
 from .utils import image_to_tensor
 from .utils import array2image
 from .utils import data2image
 from .utils import config
 from .app import appFaceShine
```

## Comparing `faceshine-1.0.3.dist-info/LICENSE` & `faceshine-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `faceshine-1.0.3.dist-info/METADATA` & `faceshine-1.0.4.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faceshine
-Version: 1.0.3
+Version: 1.0.4
 Summary: Photo image enhancer
 Home-page: https://github.com/leonelhs/faceshine
 Author: leonel hernandez
 Author-email: leonelhs@gmail.com
 License: Apache
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy (>=1.24.3)
 Requires-Dist: torch (>=2.0.0)
-Requires-Dist: opencv-python (>=4.7.0.72)
+Requires-Dist: opencv-python
 Requires-Dist: flask (>=2.3.2)
 Requires-Dist: flask-restful (>=0.3.10)
 Requires-Dist: pillow (>=9.5.0)
 Requires-Dist: torchvision
 Requires-Dist: colorama
 Requires-Dist: matplotlib
 Requires-Dist: fastprogress
```

## Comparing `faceshine-1.0.3.dist-info/RECORD` & `faceshine-1.0.4.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-faceshine/__init__.py,sha256=h-sm5hTGY8q9jXzhFXY3UJ1qVsHe45Zd16wh1ULpVcQ,239
+faceshine/__init__.py,sha256=syE0xJoEg4ShAQ7XSKpzysRLNUxWKxuw6lKrssbTWlE,239
 faceshine/__main__.py,sha256=drYa5bFqxPKUbEMJjQFzenmZbXPL0KDyNxeR6g6Sv-g,602
 faceshine/app.py,sha256=ePnQ83oYlxuWEp6tbRdYIACULy5EffrVOkO6748ERHw,2857
 faceshine/utils.py,sha256=dl3fBQiPA5ok0PUPNED-7-jnamOlg3uQAq1N0jdGiWo,992
 faceshine/tasks/__init__.py,sha256=iobkjDhxlaocumv0xdSNhpHLZMx7PlyniQGapTDgO2o,276
 faceshine/tasks/base/__init__.py,sha256=NPVMYUE7dRdkPkw3zko3s8Bc22JJl0kNtgIexWffeV8,131
 faceshine/tasks/base/ai_enhancer.py,sha256=-pIp9WpuH8qUL_fYGSN3UHDeCbHc4nnHXD3A1ldVC8w,380
 faceshine/tasks/base/ai_preprocces.py,sha256=lWbXncdNYv8GcKnDqVSInFqYNEmYhnSw_7wIev14boY,367
@@ -23,13 +23,13 @@
 faceshine/tasks/lowlight/model/model.py,sha256=u1ZmarmRVzOMkpHxKWYIMvs-PylOHPp7qoFz8mGUPcM,2017
 faceshine/tasks/segmentation/__init__.py,sha256=kzyIh3PBhevj_NnkI7U9UeCGh1rePBFRgFhykzrO1Qc,53
 faceshine/tasks/segmentation/task_zero_background.py,sha256=4ZUSvLJfU6OBZRvSVMsFZ0BGxnalBfN2p_6q8STfa8c,1440
 faceshine/tasks/superface/__init__.py,sha256=yHspjcjirTIedd6KYj5WGujwNWbRDk8WHXIfScICpgI,43
 faceshine/tasks/superface/task_super_face.py,sha256=Yj79zslIf1ucH7NbJwfTY85WdjtjSC_za85fbo5mOws,3112
 faceshine/tasks/zeroscratches/__init__.py,sha256=ZFLNOrYxPJzcCNFbgJxKJ-ubye4IZAUNv292JRpncGo,54
 faceshine/tasks/zeroscratches/task_erase_scratches.py,sha256=fpifEM9HJ6kA5py3fEnh0803CC19IGnSxgDOlBqFtmo,687
-faceshine-1.0.3.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-faceshine-1.0.3.dist-info/METADATA,sha256=50bvjZlde9UT1tntC13z_8yUJCgqs_RtVGmxhRBfQ4A,2205
-faceshine-1.0.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
-faceshine-1.0.3.dist-info/entry_points.txt,sha256=KRkbAzQEX2XD27tLpnPpofiRGLfQbRdfehtMnNhh9XI,54
-faceshine-1.0.3.dist-info/top_level.txt,sha256=e46vEsYRs7nWGitm7lwdDG_KrKG_Wfle_rLSqNMQXJ8,10
-faceshine-1.0.3.dist-info/RECORD,,
+faceshine-1.0.4.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+faceshine-1.0.4.dist-info/METADATA,sha256=gRfBxbM-T8UFEgT-Ahw-bvmPi2tMeS3kQb4ZHNw_f_A,2192
+faceshine-1.0.4.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+faceshine-1.0.4.dist-info/entry_points.txt,sha256=KRkbAzQEX2XD27tLpnPpofiRGLfQbRdfehtMnNhh9XI,54
+faceshine-1.0.4.dist-info/top_level.txt,sha256=e46vEsYRs7nWGitm7lwdDG_KrKG_Wfle_rLSqNMQXJ8,10
+faceshine-1.0.4.dist-info/RECORD,,
```

