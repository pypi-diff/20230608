# Comparing `tmp/gameauto-1.0.4.tar.gz` & `tmp/gameauto-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gameauto-1.0.4.tar", last modified: Fri Jun  2 05:09:03 2023, max compression
+gzip compressed data, was "gameauto-1.0.5.tar", last modified: Thu Jun  8 05:27:36 2023, max compression
```

## Comparing `gameauto-1.0.4.tar` & `gameauto-1.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 05:09:03.984724 gameauto-1.0.4/
--rw-rw-rw-   0        0        0     3355 2023-06-02 05:09:03.983540 gameauto-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3048 2023-06-02 05:08:07.000000 gameauto-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 05:09:03.955578 gameauto-1.0.4/gameauto/
--rw-rw-rw-   0        0        0       62 2023-06-02 04:50:23.000000 gameauto-1.0.4/gameauto/__init__.py
--rw-rw-rw-   0        0        0     6005 2023-06-02 04:56:16.000000 gameauto-1.0.4/gameauto/core.py
--rw-rw-rw-   0        0        0     9475 2023-06-02 04:51:29.000000 gameauto-1.0.4/gameauto/images.py
-drwxrwxrwx   0        0        0        0 2023-06-02 05:09:03.982542 gameauto-1.0.4/gameauto.egg-info/
--rw-rw-rw-   0        0        0     3355 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      234 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       37 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-02 05:09:03.000000 gameauto-1.0.4/gameauto.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 05:09:03.985760 gameauto-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0      688 2023-06-02 05:00:54.000000 gameauto-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:27:36.157038 gameauto-1.0.5/
+-rw-rw-rw-   0        0        0     3598 2023-06-08 05:27:36.155530 gameauto-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     3314 2023-06-08 05:24:44.000000 gameauto-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 05:27:36.136368 gameauto-1.0.5/gameauto/
+-rw-rw-rw-   0        0        0       62 2023-06-02 04:50:23.000000 gameauto-1.0.5/gameauto/__init__.py
+-rw-rw-rw-   0        0        0     6124 2023-06-08 05:21:07.000000 gameauto-1.0.5/gameauto/core.py
+-rw-rw-rw-   0        0        0    11139 2023-06-08 04:48:19.000000 gameauto-1.0.5/gameauto/images.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:27:36.153575 gameauto-1.0.5/gameauto.egg-info/
+-rw-rw-rw-   0        0        0     3598 2023-06-08 05:27:36.000000 gameauto-1.0.5/gameauto.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2023-06-08 05:27:36.000000 gameauto-1.0.5/gameauto.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 05:27:36.000000 gameauto-1.0.5/gameauto.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       37 2023-06-08 05:27:36.000000 gameauto-1.0.5/gameauto.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 05:27:36.000000 gameauto-1.0.5/gameauto.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 05:27:36.157038 gameauto-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0      688 2023-06-08 05:27:03.000000 gameauto-1.0.5/setup.py
```

### Comparing `gameauto-1.0.4/PKG-INFO` & `gameauto-1.0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: gameauto
-Version: 1.0.4
+Version: 1.0.5
 Summary: Android Game Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # gameauto
 ## Core
 ### miniFindimage
-    找图函数示例，建议重写
+        """找图函数示例
         Args:
             - template_path (Str/Mat): 图像地址或者opencv格式的图像 小图
             - target_path (Str/Mat): 图像地址或者opencv格式的图像 大图
             - region (list, optional): 模板匹配的区域左上角和右下角两点坐标[Xmin,Ymin,Xmax,Ymax]. Defaults to None.
             - threshold (float, optional): 图像相似度. Defaults to 0.8.
             - is_color (bool, optional): 是否匹配图像颜色. Defaults to False.
             - color_threshold (int, optional): 颜色相似度. Defaults to 30.
+            - use_sift (bool, optional): 是否使用sift算法匹配. Defaults to False.
             - is_click (bool, optional): 是否点击图像. Defaults to False.
-
+           
         Returns:
             list/None: 图像所在区域[Xmin,Ymin,Xmax,Ymax]
+        """
+
+```python
+#推荐使用方法
+args={
+    "template_path":"./1.png",
+    "target_path":"./2.png",
+}
+miniFindImage(**args,is_click=True)
+```
+
 ### miniRandomClick
 ```
 随机点击 建议重写
         Args:
             - region (array): [x_min, y_min, x_max, y_max]
             - point (tuple, optional): 坐标点. Defaults to None.
             - method (int, optional): Defaults to 1.
@@ -90,7 +101,9 @@
     )
     #输入mat格式图像进行计算
     objects = net(m)
     #过滤结果
     yolo_filter("exp",net.class_names,objects,0.8)
 ```
 
+
+
```

### Comparing `gameauto-1.0.4/README.md` & `gameauto-1.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 # gameauto
 ## Core
 ### miniFindimage
-    找图函数示例，建议重写
+        """找图函数示例
         Args:
             - template_path (Str/Mat): 图像地址或者opencv格式的图像 小图
             - target_path (Str/Mat): 图像地址或者opencv格式的图像 大图
             - region (list, optional): 模板匹配的区域左上角和右下角两点坐标[Xmin,Ymin,Xmax,Ymax]. Defaults to None.
             - threshold (float, optional): 图像相似度. Defaults to 0.8.
             - is_color (bool, optional): 是否匹配图像颜色. Defaults to False.
             - color_threshold (int, optional): 颜色相似度. Defaults to 30.
+            - use_sift (bool, optional): 是否使用sift算法匹配. Defaults to False.
             - is_click (bool, optional): 是否点击图像. Defaults to False.
-
+           
         Returns:
             list/None: 图像所在区域[Xmin,Ymin,Xmax,Ymax]
+        """
+
+```python
+#推荐使用方法
+args={
+    "template_path":"./1.png",
+    "target_path":"./2.png",
+}
+miniFindImage(**args,is_click=True)
+```
+
 ### miniRandomClick
 ```
 随机点击 建议重写
         Args:
             - region (array): [x_min, y_min, x_max, y_max]
             - point (tuple, optional): 坐标点. Defaults to None.
             - method (int, optional): Defaults to 1.
@@ -75,8 +87,11 @@
         num_threads=4,
         use_gpu=True,
     )
     #输入mat格式图像进行计算
     objects = net(m)
     #过滤结果
     yolo_filter("exp",net.class_names,objects,0.8)
-```
+```
+
+
+
```

### Comparing `gameauto-1.0.4/gameauto/core.py` & `gameauto-1.0.5/gameauto/core.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 import random
 import numpy as np
 
 from minidevice import MiniDevice
-from .images import find_image_color,find_image
+from .images import find_image
 
 def random_number(bbox):
     """
     Generates a random coordinate within a given rectangular boundary.
 
     Args:
         bbox: A tuple containing four values (x_min, y_min, x_max, y_max),
@@ -66,41 +66,47 @@
         self,
         template_path,
         target_path,
         region=None,
         threshold=0.8,
         is_color=False,
         color_threshold=30,
-        is_click=False,
+        use_sift=False,
+        is_click=False
+        
     ):
         """找图函数示例，建议重写
 
         Args:
             - template_path (Str/Mat): 图像地址或者opencv格式的图像 小图
             - target_path (Str/Mat): 图像地址或者opencv格式的图像 大图
             - region (list, optional): 模板匹配的区域左上角和右下角两点坐标[Xmin,Ymin,Xmax,Ymax]. Defaults to None.
             - threshold (float, optional): 图像相似度. Defaults to 0.8.
             - is_color (bool, optional): 是否匹配图像颜色. Defaults to False.
             - color_threshold (int, optional): 颜色相似度. Defaults to 30.
+            - use_sift (bool, optional): 是否使用sift算法匹配. Defaults to False.
             - is_click (bool, optional): 是否点击图像. Defaults to False.
-
+           
         Returns:
             list/None: 图像所在区域[Xmin,Ymin,Xmax,Ymax]
         """
-        if is_color:
-            res = find_image_color(
-                template_path, target_path, region, threshold, True, color_threshold
-            )
-        else:
-            res = find_image(template_path, target_path, region, threshold)
+ 
+        result = find_image(
+            template_path,
+            target_path,
+            region, 
+            threshold,
+            is_color=is_color,
+            color_threshold=color_threshold,
+            use_sift=use_sift)
 
-        if res:
+        if result:
             if is_click:
-                self.miniRandomClick(xywh2xyxy(res))
-            return xywh2xyxy(res)
+                self.miniRandomClick(xywh2xyxy(result))
+            return xywh2xyxy(result)
         else:
             return None
         
     def miniRandomClick(self, region, point=None, method=1):
         """随机点击 同样建议重写
 
         Args:
```

### Comparing `gameauto-1.0.4/gameauto/images.py` & `gameauto-1.0.5/gameauto/images.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import cv2
 import ncnn
 from ncnn.utils.objects import Detect_Object
+import numpy as np
 
 def compare_color(image, point, color, tolerance=0):
     """
     比较某一图像中某点的颜色值是否和传入颜色参数值相等。
 
     参数：
     - image: 图像 Mat格式
@@ -69,108 +70,124 @@
                 and abs(pixel_color[1] - g) <= tolerance
                 and abs(pixel_color[0] - b) <= tolerance
             ):
                 return x, y
     return None
 
 
-def find_image(template_path, target_path, region=None, threshold=0.8,flag=cv2.IMREAD_COLOR):
-    """灰度找图
+def find_image(template_path, target_path, region=None, threshold=0.8,is_color=False,color_threshold=30,use_sift=False,flag=cv2.IMREAD_GRAYSCALE):
+    """找图
 
     Args:
-        params: 一个字典，包含以下参数：
+        - template_path: 模板图像的路径/cv2格式
 
-            - template_path: 模板图像的路径/cv2格式
+        - target_path: 目标图像的路径/cv2格式
 
-                - target_path: 目标图像的路径/cv2格式
+        - region: 指定在目标图像中查找的区域,格式为(x_min, y_min, x_max, y_max),默认为None表示查找整张图片
 
-                - region: 指定在目标图像中查找的区域,格式为(x_min, y_min, x_max, y_max),默认为None表示查找整张图片
+        - threshold: 相似度的阈值,取值为0~1之间,默认为0
 
-                - threshold: 相似度的阈值,取值为0~1之间,默认为0
-
-                - flag:图像读取方式
+        - is_color (bool, optional): _description_. Defaults to False.
 
+        - color_threshold (int, optional): _description_. Defaults to 30.
+         
+        - flag (int, optional):图像读取方式 Defaults to cv2.IMREAD_GRAYSCALE
+            
+        - use_sift (bool, optional): 是否使用sift算法匹配. Defaults to False.
         Returns:
-            一个包含4个元素的元组(x, y,w,h),表示查找到的最相似部分在目标图像中的左上角坐标,如果未找到则返回None
+            一个包含4个元素的list[x,y,w,h,]表示查找到的最相似部分在目标图像中的左上角坐标,如果未找到则返回None
     """
+
+    if is_color:
+        flag = cv2.IMREAD_COLOR
+
     # 读取模板图像和目标图像
     template = (
         cv2.imread(template_path, flag)
         if isinstance(template_path, str)
         else template_path
     )
 
     target = (
-        cv2.imread(target_path, flag) if isinstance(target_path, str) else target_path
+        cv2.imread(target_path, flag)
+        if isinstance(target_path, str)
+        else target_path
     )
+
+    template, target = flag2same(template, target)
+
+    if use_sift:
+        # 创建SIFT对象
+        sift = cv2.SIFT_create()
+        # 计算关键点和描述符
+        kp_template, des_template = sift.detectAndCompute(template, None)
+        kp_target, des_target = sift.detectAndCompute(target, None)
+
+        # 创建BFMatcher对象
+        bf = cv2.BFMatcher()
+        matches = bf.knnMatch(des_template, des_target, k=2)
+
+        # 应用Lowe的比例测试
+        good_matches = []
+        for m, n in matches:
+            if m.distance < 0.75 * n.distance:
+                good_matches.append(m)
+
+        # 如果找到足够的好匹配，则计算单应性矩阵
+        if len(good_matches) > 10:
+            src_pts = np.float32([kp_template[m.queryIdx].pt for m in good_matches]).reshape(-1, 1, 2)
+            dst_pts = np.float32([kp_target[m.trainIdx].pt for m in good_matches]).reshape(-1, 1, 2)
+
+            # 计算单应性矩阵
+            M, mask = cv2.findHomography(src_pts, dst_pts, cv2.RANSAC, 5.0)
+
+            # 将模板图像的角点映射到目标图像中的相应位置
+            if len(template.shape)==2:
+                h, w = template.shape
+            elif len(template.shape)==3:
+                h,w,c = template.shape
+            else :
+                return None
+            pts = np.float32([[0, 0], [0, h - 1], [w - 1, h - 1], [w - 1, 0]]).reshape(-1, 1, 2)
+            dst = cv2.perspectiveTransform(pts, M)
+            region = dst.reshape(-1, 2).tolist()
+            
+            return [int(region[0][0]),int(region[0][1]),int(region[2][0])-int(region[0][0]),int(region[2][1])-int(region[0][1])]
+
+        else:
+            print("Not enough matches are found - %d/%d" % (len(good_matches), 10))
+            return None
+
     # 设置查找区域
     if region is not None:
         x_min, y_min, x_max, y_max = region
         target = target[y_min:y_max, x_min:x_max]
     # 匹配模板图像
     res = cv2.matchTemplate(target, template, cv2.TM_CCOEFF_NORMED)
     # 选择相似度最高的一个结果
     min_val, max_val, min_loc, max_loc = cv2.minMaxLoc(res)
     if max_val < threshold:
         return None
     # 转换坐标系
     if region is not None:
         max_loc = (max_loc[0] + x_min, max_loc[1] + y_min)
-    # 返回匹配结果
-    return [max_loc[0], max_loc[1], template.shape[1], template.shape[0]]
-
-
-def find_image_color(
-    template_path,
-    target_path,
-    region=None,
-    threshold=0.8,
-    is_color=False,
-    color_threshold=30,
-):
-    """找图进阶含找色
-
-    Args:
-        template_path (_type_): _description_
-        target_path (_type_): _description_
-        region (_type_): _description_
-        threshold (float, optional): _description_. Defaults to 0.8.
-        is_color (bool, optional): _description_. Defaults to False.
-        color_threshold (int, optional): _description_. Defaults to 30.
-
-    Returns:
-        _type_: _description_
-    """
-    flag = cv2.IMREAD_COLOR
-    # 读取模板图像和目标图像
-    template = (
-        cv2.imread(template_path, flag)
-        if isinstance(template_path, str)
-        else template_path
-    )
-
-    target = (
-        cv2.imread(target_path, flag) if isinstance(target_path, str) else target_path
-    )
-
-    res = find_image(template, target, region, threshold)
-
+        
     if res:
         if is_color:
             if (
                 find_color(
                     target,
                     get_color(template, [0, 0]),
                     [res[0], res[1], res[0] + 10, res[0] + 10],
                     color_threshold,
                 )
                 is None
             ):
                 return None
-        return res
+        return [max_loc[0], max_loc[1], template.shape[1], template.shape[0]]
     else:
         return None
 
 
 def readImgArr(imgPathArr):
     """读取图像并返回cv2图像字典
 
@@ -182,14 +199,33 @@
     """
     imgArr = {}
     for imgPath in imgPathArr:
         imgArr[imgPath.split("/")[-1].split(".")[0]] = cv2.imread(imgPath)
     return imgArr
 
 
+    
+def flag2same(template, target):
+    """统一图像格式
+
+    Args:
+        template (_type_): _description_
+        target (_type_): _description_
+
+    Returns:
+        _type_: _description_
+    """
+    if len(target.shape)==2 or len(template.shape)==2:
+        if len(target.shape)==3:
+            target=cv2.cvtColor(target,cv2.COLOR_BGR2GRAY)
+        if len(template.shape)==3:
+            template=cv2.cvtColor(template,cv2.COLOR_BGR2GRAY)
+    return template,target
+
+
 class YoloV3:
     def __init__(
         self,
         param_path:str,
         bin_path:str,
         class_names:list,
         tiny=False,
```

### Comparing `gameauto-1.0.4/gameauto.egg-info/PKG-INFO` & `gameauto-1.0.5/gameauto.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,46 @@
 Metadata-Version: 2.1
 Name: gameauto
-Version: 1.0.4
+Version: 1.0.5
 Summary: Android Game Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
-Platform: UNKNOWN
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 
 # gameauto
 ## Core
 ### miniFindimage
-    找图函数示例，建议重写
+        """找图函数示例
         Args:
             - template_path (Str/Mat): 图像地址或者opencv格式的图像 小图
             - target_path (Str/Mat): 图像地址或者opencv格式的图像 大图
             - region (list, optional): 模板匹配的区域左上角和右下角两点坐标[Xmin,Ymin,Xmax,Ymax]. Defaults to None.
             - threshold (float, optional): 图像相似度. Defaults to 0.8.
             - is_color (bool, optional): 是否匹配图像颜色. Defaults to False.
             - color_threshold (int, optional): 颜色相似度. Defaults to 30.
+            - use_sift (bool, optional): 是否使用sift算法匹配. Defaults to False.
             - is_click (bool, optional): 是否点击图像. Defaults to False.
-
+           
         Returns:
             list/None: 图像所在区域[Xmin,Ymin,Xmax,Ymax]
+        """
+
+```python
+#推荐使用方法
+args={
+    "template_path":"./1.png",
+    "target_path":"./2.png",
+}
+miniFindImage(**args,is_click=True)
+```
+
 ### miniRandomClick
 ```
 随机点击 建议重写
         Args:
             - region (array): [x_min, y_min, x_max, y_max]
             - point (tuple, optional): 坐标点. Defaults to None.
             - method (int, optional): Defaults to 1.
@@ -90,7 +101,9 @@
     )
     #输入mat格式图像进行计算
     objects = net(m)
     #过滤结果
     yolo_filter("exp",net.class_names,objects,0.8)
 ```
 
+
+
```

### Comparing `gameauto-1.0.4/setup.py` & `gameauto-1.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='gameauto',
-      version='1.0.4',
+      version='1.0.5',
       description='Android Game Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
       keywords='game',
       project_urls={},
       packages=find_packages(),
       include_package_data=True,
-      install_requires=['minidevice>=1.0.4','ncnn>=1.0.20230517'],
+      install_requires=['minidevice>=1.0.8','ncnn>=1.0.20230517'],
       python_requires='>=3'
       )
```

