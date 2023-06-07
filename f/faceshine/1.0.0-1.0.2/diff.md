# Comparing `tmp/faceshine-1.0.0-py3-none-any.whl.zip` & `tmp/faceshine-1.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,37 @@
-Zip file size: 9234 bytes, number of entries: 14
--rw-rw-r--  2.0 unx      203 b- defN 23-Jun-02 05:50 faceshine/__init__.py
+Zip file size: 23094 bytes, number of entries: 35
+-rw-rw-r--  2.0 unx      239 b- defN 23-Jun-07 23:27 faceshine/__init__.py
 -rw-rw-r--  2.0 unx      602 b- defN 23-Jun-02 05:58 faceshine/__main__.py
--rw-rw-r--  2.0 unx      994 b- defN 23-Jun-02 06:00 faceshine/app.py
--rw-rw-r--  2.0 unx      636 b- defN 23-Jun-02 03:21 faceshine/utils.py
--rw-rw-r--  2.0 unx       53 b- defN 23-Jun-02 03:13 faceshine/segmentation/__init__.py
--rw-rw-r--  2.0 unx     1435 b- defN 23-Jun-02 04:36 faceshine/segmentation/task_zero_background.py
--rw-rw-r--  2.0 unx      373 b- defN 23-Apr-14 23:28 faceshine/segmentation/base/Task.py
--rw-rw-r--  2.0 unx        0 b- defN 23-Jun-02 02:44 faceshine/segmentation/base/__init__.py
--rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-02 06:35 faceshine-1.0.0.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1115 b- defN 23-Jun-02 06:35 faceshine-1.0.0.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-Jun-02 06:35 faceshine-1.0.0.dist-info/WHEEL
--rw-rw-r--  2.0 unx       54 b- defN 23-Jun-02 06:35 faceshine-1.0.0.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx       10 b- defN 23-Jun-02 06:35 faceshine-1.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1170 b- defN 23-Jun-02 06:35 faceshine-1.0.0.dist-info/RECORD
-14 files, 18094 bytes uncompressed, 7266 bytes compressed:  59.8%
+-rw-rw-r--  2.0 unx     2857 b- defN 23-Jun-07 07:04 faceshine/app.py
+-rw-rw-r--  2.0 unx      992 b- defN 23-Jun-05 22:49 faceshine/utils.py
+-rw-rw-r--  2.0 unx      276 b- defN 23-Jun-06 23:44 faceshine/tasks/__init__.py
+-rw-rw-r--  2.0 unx      131 b- defN 23-Jun-05 22:42 faceshine/tasks/base/__init__.py
+-rw-rw-r--  2.0 unx      380 b- defN 23-Apr-20 16:29 faceshine/tasks/base/ai_enhancer.py
+-rw-rw-r--  2.0 unx      367 b- defN 23-Apr-21 18:27 faceshine/tasks/base/ai_preprocces.py
+-rw-rw-r--  2.0 unx      381 b- defN 23-Apr-20 16:29 faceshine/tasks/base/ai_upsampler.py
+-rw-rw-r--  2.0 unx      373 b- defN 23-Apr-14 23:28 faceshine/tasks/base/task.py
+-rw-rw-r--  2.0 unx       53 b- defN 23-Jun-05 19:58 faceshine/tasks/colorizer/__init__.py
+-rw-rw-r--  2.0 unx     1277 b- defN 23-Jun-07 05:53 faceshine/tasks/colorizer/model_image_colorizer.py
+-rw-rw-r--  2.0 unx     1284 b- defN 23-Jun-07 23:14 faceshine/tasks/colorizer/task_image_colorizer.py
+-rw-rw-r--  2.0 unx       91 b- defN 23-Jun-06 23:44 faceshine/tasks/faceparser/__init__.py
+-rw-rw-r--  2.0 unx     1860 b- defN 23-Jun-07 23:25 faceshine/tasks/faceparser/task_face_segmentation.py
+-rw-rw-r--  2.0 unx        0 b- defN 23-Apr-06 16:36 faceshine/tasks/faceparser/bisnet/__init__.py
+-rw-rw-r--  2.0 unx    10575 b- defN 23-Apr-06 16:36 faceshine/tasks/faceparser/bisnet/model.py
+-rw-rw-r--  2.0 unx     3648 b- defN 23-Apr-06 21:42 faceshine/tasks/faceparser/bisnet/resnet.py
+-rw-rw-r--  2.0 unx       79 b- defN 23-Jun-05 21:35 faceshine/tasks/lowlight/__init__.py
+-rw-rw-r--  2.0 unx     1521 b- defN 23-Jun-07 23:17 faceshine/tasks/lowlight/task_low_light.py
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jun-05 21:35 faceshine/tasks/lowlight/model/__init__.py
+-rw-rw-r--  2.0 unx     1101 b- defN 23-Apr-07 15:54 faceshine/tasks/lowlight/model/dataloader.py
+-rw-rw-r--  2.0 unx     2017 b- defN 23-Apr-07 15:54 faceshine/tasks/lowlight/model/model.py
+-rw-rw-r--  2.0 unx       53 b- defN 23-Jun-02 03:13 faceshine/tasks/segmentation/__init__.py
+-rw-rw-r--  2.0 unx     1440 b- defN 23-Jun-05 19:27 faceshine/tasks/segmentation/task_zero_background.py
+-rw-rw-r--  2.0 unx       43 b- defN 23-Jun-06 22:04 faceshine/tasks/superface/__init__.py
+-rw-rw-r--  2.0 unx     3112 b- defN 23-Jun-07 22:35 faceshine/tasks/superface/task_super_face.py
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jun-06 03:50 faceshine/tasks/zeroscratches/__init__.py
+-rw-rw-r--  2.0 unx      687 b- defN 23-Jun-06 04:07 faceshine/tasks/zeroscratches/task_erase_scratches.py
+-rw-rw-r--  2.0 unx    11357 b- defN 23-Jun-07 23:38 faceshine-1.0.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1818 b- defN 23-Jun-07 23:38 faceshine-1.0.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-Jun-07 23:38 faceshine-1.0.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx       54 b- defN 23-Jun-07 23:38 faceshine-1.0.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx       10 b- defN 23-Jun-07 23:38 faceshine-1.0.2.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     3218 b- defN 23-Jun-07 23:38 faceshine-1.0.2.dist-info/RECORD
+35 files, 52096 bytes uncompressed, 17796 bytes compressed:  65.8%
```

## zipnote {}

```diff
@@ -6,38 +6,101 @@
 
 Filename: faceshine/app.py
 Comment: 
 
 Filename: faceshine/utils.py
 Comment: 
 
-Filename: faceshine/segmentation/__init__.py
+Filename: faceshine/tasks/__init__.py
 Comment: 
 
-Filename: faceshine/segmentation/task_zero_background.py
+Filename: faceshine/tasks/base/__init__.py
 Comment: 
 
-Filename: faceshine/segmentation/base/Task.py
+Filename: faceshine/tasks/base/ai_enhancer.py
 Comment: 
 
-Filename: faceshine/segmentation/base/__init__.py
+Filename: faceshine/tasks/base/ai_preprocces.py
 Comment: 
 
-Filename: faceshine-1.0.0.dist-info/LICENSE
+Filename: faceshine/tasks/base/ai_upsampler.py
 Comment: 
 
-Filename: faceshine-1.0.0.dist-info/METADATA
+Filename: faceshine/tasks/base/task.py
 Comment: 
 
-Filename: faceshine-1.0.0.dist-info/WHEEL
+Filename: faceshine/tasks/colorizer/__init__.py
 Comment: 
 
-Filename: faceshine-1.0.0.dist-info/entry_points.txt
+Filename: faceshine/tasks/colorizer/model_image_colorizer.py
 Comment: 
 
-Filename: faceshine-1.0.0.dist-info/top_level.txt
+Filename: faceshine/tasks/colorizer/task_image_colorizer.py
 Comment: 
 
-Filename: faceshine-1.0.0.dist-info/RECORD
+Filename: faceshine/tasks/faceparser/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/faceparser/task_face_segmentation.py
+Comment: 
+
+Filename: faceshine/tasks/faceparser/bisnet/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/faceparser/bisnet/model.py
+Comment: 
+
+Filename: faceshine/tasks/faceparser/bisnet/resnet.py
+Comment: 
+
+Filename: faceshine/tasks/lowlight/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/lowlight/task_low_light.py
+Comment: 
+
+Filename: faceshine/tasks/lowlight/model/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/lowlight/model/dataloader.py
+Comment: 
+
+Filename: faceshine/tasks/lowlight/model/model.py
+Comment: 
+
+Filename: faceshine/tasks/segmentation/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/segmentation/task_zero_background.py
+Comment: 
+
+Filename: faceshine/tasks/superface/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/superface/task_super_face.py
+Comment: 
+
+Filename: faceshine/tasks/zeroscratches/__init__.py
+Comment: 
+
+Filename: faceshine/tasks/zeroscratches/task_erase_scratches.py
+Comment: 
+
+Filename: faceshine-1.0.2.dist-info/LICENSE
+Comment: 
+
+Filename: faceshine-1.0.2.dist-info/METADATA
+Comment: 
+
+Filename: faceshine-1.0.2.dist-info/WHEEL
+Comment: 
+
+Filename: faceshine-1.0.2.dist-info/entry_points.txt
+Comment: 
+
+Filename: faceshine-1.0.2.dist-info/top_level.txt
+Comment: 
+
+Filename: faceshine-1.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## faceshine/__init__.py

```diff
@@ -1,9 +1,9 @@
 __appname__ = "Face Shine"
-__version__ = "1.0.0"
+__version__ = "1.0.2"
 
+from .utils import tensor_to_ndarray
 from .utils import image_to_tensor
 from .utils import array2image
 from .utils import data2image
 from .utils import config
 from .app import appFaceShine
-
```

## faceshine/app.py

```diff
@@ -1,17 +1,23 @@
 from flask import Flask, jsonify
 from flask_restful import Resource, Api, reqparse
+from werkzeug.datastructures import FileStorage
 
 from faceshine import data2image
-from .segmentation import TaskZeroBackground
-from werkzeug.datastructures import FileStorage
+from faceshine.tasks import TaskZeroBackground, \
+    TaskImageColorizer, TaskLowLight, TaskEraseScratches, TaskSuperFace, TaskFaceSegmentation
 
 appFaceShine = Flask(__name__)
 api = Api(appFaceShine)
 
+taskFaceSegmentation = TaskFaceSegmentation()
+taskSuperFace = TaskSuperFace()
+taskLowLight = TaskLowLight()
+taskEraseScratches = TaskEraseScratches()
+taskImageColorizer = TaskImageColorizer()
 taskZeroBackground = TaskZeroBackground()
 
 parser = reqparse.RequestParser()
 
 parser.add_argument('image',
                     type=FileStorage,
                     location='files',
@@ -20,18 +26,68 @@
 
 
 class Index(Resource):
     def get(self):
         return {'It works!': 'AI Remote Procedure Machine'}
 
 
+class FaceSegmentation(Resource):
+    def post(self):
+        args = parser.parse_args()
+        stream = args['image'].read()
+        image = data2image(stream)
+        prediction = taskFaceSegmentation.executeTask(image)
+        return jsonify(prediction.tolist())
+
+
+class SuperFace(Resource):
+    def post(self):
+        args = parser.parse_args()
+        stream_a = args['image'].read()
+        image = data2image(stream_a)
+        prediction = taskSuperFace.executeTask(image)
+        return jsonify(prediction.tolist())
+
+
+class ImageLowLight(Resource):
+    def post(self):
+        args = parser.parse_args()
+        stream_a = args['image'].read()
+        image = data2image(stream_a)
+        prediction = taskLowLight.executeTask(image)
+        return jsonify(prediction.tolist())
+
+
+class EraseScratches(Resource):
+    def post(self):
+        args = parser.parse_args()
+        stream_a = args['image'].read()
+        image = data2image(stream_a)
+        prediction = taskEraseScratches.executeTask(image)
+        return jsonify(prediction.tolist())
+
+
+class ImageColorizer(Resource):
+    def post(self):
+        args = parser.parse_args()
+        stream_a = args['image'].read()
+        image = data2image(stream_a)
+        prediction = taskImageColorizer.executeTask(image)
+        return jsonify(prediction.tolist())
+
+
 class ZeroBackground(Resource):
     def post(self):
         args = parser.parse_args()
         stream_a = args['image'].read()
         image = data2image(stream_a)
         prediction = taskZeroBackground.executeTask(image)
         return jsonify(prediction.tolist())
 
 
+api.add_resource(FaceSegmentation, '/segment_face')
+api.add_resource(SuperFace, '/super_face')
+api.add_resource(EraseScratches, '/erase_scratches')
+api.add_resource(ImageLowLight, '/enhance_light')
+api.add_resource(ImageColorizer, '/colorize')
 api.add_resource(ZeroBackground, '/zero_background')
 api.add_resource(Index, '/')
```

## faceshine/utils.py

```diff
@@ -1,14 +1,15 @@
-import json
-
 import PIL
 import cv2
+import json
+import torch
 import numpy as np
 from PIL.Image import Image
 import torchvision.transforms as transforms
+from torchvision.utils import make_grid
 
 
 def config():
     data = open('faceshine/conf.json')
     return json.load(data)
 
 
@@ -24,7 +25,19 @@
 def image_to_tensor(image):
     to_tensor = transforms.Compose([
         transforms.ToTensor(),
         transforms.Normalize((0.485, 0.456, 0.406), (0.229, 0.224, 0.225)),
     ])
 
     return to_tensor(image)
+
+
+# Method are common to:
+# TaskMaskScratches
+# TaskEraseScratches
+# TaskLowLight
+
+def tensor_to_ndarray(tensor, nrow=1, padding=0, normalize=True):
+    grid = make_grid(tensor, nrow, padding, normalize)
+    return grid.mul(255).add_(0.5).clamp_(0, 255).permute(1, 2, 0).to("cpu", torch.uint8).numpy()
+
+
```

## Comparing `faceshine/segmentation/task_zero_background.py` & `faceshine/tasks/segmentation/task_zero_background.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #   Reimplemented by: Leonel Hernández
 #
 ##############################################################################
 import numpy as np
 import torch
 
 from faceshine import array2image, image_to_tensor
-from .base.Task import Task
+from faceshine.tasks import Task
 
 
 class TaskZeroBackground(Task):
     def __init__(self):
         super().__init__()
         self.model = torch.hub.load('pytorch/vision:v0.6.0', 'deeplabv3_resnet101', weights='DEFAULT')
         self.model.eval()
```

## Comparing `faceshine-1.0.0.dist-info/LICENSE` & `faceshine-1.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

