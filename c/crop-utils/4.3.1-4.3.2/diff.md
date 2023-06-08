# Comparing `tmp/crop_utils-4.3.1.tar.gz` & `tmp/crop_utils-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crop_utils-4.3.1.tar", last modified: Sat May 20 07:33:59 2023, max compression
+gzip compressed data, was "crop_utils-4.3.2.tar", last modified: Thu Jun  8 10:13:31 2023, max compression
```

## Comparing `crop_utils-4.3.1.tar` & `crop_utils-4.3.2.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.907796 crop_utils-4.3.1/
--rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.1/LICENSE
--rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1998 2023-05-20 07:33:59.907796 crop_utils-4.3.1/PKG-INFO
--rw-rw-rw-   0        0        0      910 2023-03-03 09:28:43.000000 crop_utils-4.3.1/README.md
--rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-20 07:33:59.907796 crop_utils-4.3.1/setup.cfg
--rw-rw-rw-   0        0        0      895 2023-05-20 07:33:48.000000 crop_utils-4.3.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.884804 crop_utils-4.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.899805 crop_utils-4.3.1/src/crop_utils/
--rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.1/src/crop_utils/__init__.py
--rw-rw-rw-   0        0        0     2140 2022-04-29 03:15:39.000000 crop_utils-4.3.1/src/crop_utils/html_slot_config.py
--rw-rw-rw-   0        0        0    56899 2022-10-09 03:26:55.000000 crop_utils-4.3.1/src/crop_utils/image.py
--rw-rw-rw-   0        0        0    42170 2023-05-20 07:33:32.000000 crop_utils-4.3.1/src/crop_utils/img_crop.py
--rw-rw-rw-   0        0        0    41524 2021-11-19 07:30:47.000000 crop_utils-4.3.1/src/crop_utils/olg_crop.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:33:59.905796 crop_utils-4.3.1/src/crop_utils.egg-info/
--rw-rw-rw-   0        0        0     1998 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      345 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-05-20 07:33:59.000000 crop_utils-4.3.1/src/crop_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.691264 crop_utils-4.3.2/
+-rw-rw-rw-   0        0        0     1091 2021-10-21 02:22:48.000000 crop_utils-4.3.2/LICENSE
+-rw-rw-rw-   0        0        0       52 2021-10-21 06:40:49.000000 crop_utils-4.3.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1997 2023-06-08 10:13:31.690267 crop_utils-4.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0      910 2023-05-20 07:34:16.000000 crop_utils-4.3.2/README.md
+-rw-rw-rw-   0        0        0      108 2021-10-20 10:50:24.000000 crop_utils-4.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:13:31.691264 crop_utils-4.3.2/setup.cfg
+-rw-rw-rw-   0        0        0      894 2023-06-08 10:13:24.000000 crop_utils-4.3.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.664261 crop_utils-4.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.681261 crop_utils-4.3.2/src/crop_utils/
+-rw-rw-rw-   0        0        0        4 2021-10-21 03:45:02.000000 crop_utils-4.3.2/src/crop_utils/__init__.py
+-rw-rw-rw-   0        0        0     2157 2023-06-06 03:35:58.000000 crop_utils-4.3.2/src/crop_utils/html_slot_config.py
+-rw-rw-rw-   0        0        0    63534 2023-06-07 06:16:06.000000 crop_utils-4.3.2/src/crop_utils/image.py
+-rw-rw-rw-   0        0        0    43293 2023-06-08 09:08:58.000000 crop_utils-4.3.2/src/crop_utils/img_crop.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:13:31.688262 crop_utils-4.3.2/src/crop_utils.egg-info/
+-rw-rw-rw-   0        0        0     1997 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      318 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 10:13:31.000000 crop_utils-4.3.2/src/crop_utils.egg-info/top_level.txt
```

### Comparing `crop_utils-4.3.1/LICENSE` & `crop_utils-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `crop_utils-4.3.1/PKG-INFO` & `crop_utils-4.3.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop_utils
-Version: 4.3.1
-Summary: 详情页扩边
+Version: 4.3.2
+Summary: 鞋类ai识别
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.0 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.1 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `crop_utils-4.3.1/README.md` & `crop_utils-4.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -65,8 +65,8 @@
 
 
 
 # 安装
 
 
 
-pip install crop-utils==4.3.0 -i  https://pypi.python.org/simple/
+pip install crop-utils==4.3.1 -i  https://pypi.python.org/simple/
```

### Comparing `crop_utils-4.3.1/setup.py` & `crop_utils-4.3.2/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="crop_utils",  # 包名称
-    version="4.3.1",  # 版本号
+    version="4.3.2",  # 版本号
     author="libo",
     author_email="6878595@qq.com",
-    description="详情页扩边",
+    description="鞋类ai识别",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="http://git.chaomy.com/libo/ecpro-utils.git",
     project_urls={
         "Bug Tracker": "https://github.com/pypa/sampleproject/issues",
     },
     classifiers=[
```

### Comparing `crop_utils-4.3.1/src/crop_utils/html_slot_config.py` & `crop_utils-4.3.2/src/crop_utils/html_slot_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,14 +43,15 @@
 RETAIN_X_OR_Y = "r_x_o_y"  # # 保留上下 y 保留左右居中 x  最大限度满足兴趣区域上下裁剪 interest_x
 MAIN_PRODUCT_CROP = "m_p_c"  # 0不裁剪主商品  1 裁剪主商品
 MODEL_TOP = 'm_t'
 MODEL_BUST = 'm_bu'
 MODEL_BOTTOM = 'm_bo'
 MODEL_FULL = 'm_f'
 TILE = 't'
+SHOES = 'shoes'
 BRAND = 'b'
 CROP_DETAIL = 'c_d'
 GIF = 'g'
 
 TOP_SITE = 'ts'
 BOTTOM_SITE = 'bs'
 TOP = 't'
```

### Comparing `crop_utils-4.3.1/src/crop_utils/image.py` & `crop_utils-4.3.2/src/crop_utils/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,25 +2,32 @@
 
 IMG_CLASSIFY = [['模特图', '模特上身图', '模特上身正面'], ['模特图', '模特上身图', '模特上身侧面'], ['模特图', '模特上身图', '模特上身背面'],
                 ['模特图', '模特胸像图', '模特胸像正面'], ['模特图', '模特胸像图', '模特胸像侧面'], ['模特图', '模特胸像图', '模特胸像背面'],
                 ['模特图', '模特下身图', '模特下身正面'], ['模特图', '模特下身图', '模特下身侧面'], ['模特图', '模特下身图', '模特下身背面'],
                 ['模特图', '模特全身图', '模特全身正面'], ['模特图', '模特全身图', '模特全身侧面'], ['模特图', '模特全身图', '模特全身背面'],
                 ['细节图', '面料'], ['细节图', '领部'], ['细节图', '肩部'], ['细节图', '腰部'], ['细节图', '衣袖'], ['细节图', '下摆'],
                 ['细节图', '口袋'], ['细节图', '门襟'], ['细节图', '内衬'], ['细节图', '图案'], ['细节图', '裤脚'],
+                ['细节图-鞋子', '鞋头'], ['细节图-鞋子', '鞋跟/鞋帮'], ['细节图-鞋子', '鞋口'], ['细节图-鞋子', '鞋底'], ['细节图-鞋子', '鞋标'],
                 ['平铺图', '平铺图背面'], ['平铺图', '平铺图正面'], ['平铺图', '平铺图侧面'],
+                ['静物图-鞋子', '前面'], ['静物图-鞋子', '后面'], ['静物图-鞋子', '鞋顶面'], ['静物图-鞋子', '鞋底面'],
+                ['静物图-鞋子', '侧面45度'], ['静物图-鞋子', '侧面90度'], ['静物图-鞋子', '侧面135度'], ['静物图-鞋子', '侧面225度'],
+                ['静物图-鞋子', '侧面270度'], ['静物图-鞋子', '侧面315度'],
                 ['资质图', '吊牌图'], ['资质图', '洗水唛'],
                 ['动图']
                 ]
 
 CROP_TYPE = {
     'm_t': ['模特上身正面', '模特上身侧面', '模特上身背面'],
     'm_bu': ['模特胸像正面', '模特胸像侧面', '模特胸像背面'],
     'm_bo': ['模特下身正面', '模特下身侧面', '模特下身背面'],
     'm_f': ['模特全身正面', '模特全身侧面', '模特全身背面'],
     't': ['平铺图背面', '平铺图正面', '平铺图侧面'],
+    'shoes': ['前面', '后面', '鞋顶面', '鞋靴底面',
+              '左侧45度', '左侧135度', '右侧45度',
+              '右侧135度'],
     'b': ['资质图', '吊牌图', '洗水唛'],
     'g': ['动图'],
 }
 
 
 class Image:
     def __init__(self, data):
@@ -79,14 +86,16 @@
             if self.image_classification in img_class_list:
                 self.img_crop_type = t
 
         image_analysis['storage_key'] = self.storage_key
         self.humans = Human(image_analysis)
         self.cloths = Cloths(image_analysis)
 
+        self.shoes = Shoes(image_analysis)
+
         self.image_analysis = image_analysis
         # 获取主商品
         self.crop_point = self.deal_crop_key_point()
         # 获取图片背景图
         self.image_background = self.deal_image_background()
 
         self.image_detail = ImageDetail()
@@ -287,45 +296,63 @@
                                 'default': True,
                             },
                         ],
                         'value':
                             'other-category',
                     },
                 ]'''
-        cat_mapping = {'model': '模特', 'top': '上身', 'up': "胸像", "down": "下身", "all": "全身",
-                       'tile': "平铺图",
-                       "detail": "细节图", "fabric": "面料", "other": "其他",
-                       "intelligence": "", 'drop': "吊牌图", 'tag': "洗水唛",
-                       "positive": "正面", "side": "侧面", "back": "背面",
-                       "sweep": "下摆", "lining": "内衬", "pocket": "口袋",
-                       "pattern": "图案", "shoulder": "肩部", "waist": "腰部",
-                       "sleeve": "衣袖", "leg": "裤脚", "stay": "门襟",
-                       "collar": "领部",
-                       "gif": "动图"
-                       }
+        # cat_mapping = {'model': '模特', 'top': '上身', 'up': "胸像", "down": "下身", "all": "全身",
+        #                'tile': "平铺图",
+        #                "detail": "细节图", "fabric": "面料", "other": "其他",
+        #                "intelligence": "", 'drop': "吊牌图", 'tag': "洗水唛",
+        #                "positive": "正面", "side": "侧面", "back": "背面",
+        #                "sweep": "下摆", "lining": "内衬", "pocket": "口袋",
+        #                "pattern": "图案", "shoulder": "肩部", "waist": "腰部",
+        #                "sleeve": "衣袖", "leg": "裤脚", "stay": "门襟",
+        #                "collar": "领部",
+        #                "gif": "动图",
+        #                }
+        storage_to_slot = {'model-top_positive': '模特上身正面', 'model-top_side': '模特上身侧面', 'model-top_back': '模特上身背面',
+                           'model-up_positive': '模特胸像正面', 'model-up_side': '模特胸像侧面', 'model-up_back': '模特胸像背面',
+                           'model-down_positive': '模特下身正面', 'model-down_side': '模特下身侧面', 'model-down_back': '模特下身背面',
+                           'model-all_positive': '模特全身正面', 'model-all_side': '模特全身侧面', 'model-all_back': '模特全身背面',
+                           'tile_positive': '平铺图正面', 'tile_back': '平铺图背面', 'tile_side': '平铺图侧面',
+                           'tile-shoes_front': '前面', 'tile-shoes_back': '后面', 'tile-shoes_side45': '侧面45度',
+                           'tile-shoes_side90': '侧面90度', 'tile-shoes_side135': '侧面135度', 'tile-shoes_side225': '侧面225度',
+                           'tile-shoes_side270': '侧面270度', 'tile-shoes_side315': '侧面315度',
+                           'tile-shoes_bottom': '鞋底面', 'tile-shoes_top': '鞋顶面',
+                           'detail_sweep': '下摆', 'detail_lining': '内衬', 'detail_pocket': '口袋',
+                           'detail_pattern': '图案', 'detail_shoulder': '肩部', 'detail_waist': '腰部', 'detail_sleeve': '衣袖',
+                           'detail_leg': '裤脚', 'detail_stay': '门襟', 'detail_fabric': '面料', 'detail_collar': '领部',
+                           'detail_other': '其他',
+                           'detail-shoes_toe': '鞋头', 'detail-shoes_heel': '鞋跟/鞋帮',
+                           'detail-shoes_soles': '鞋底', 'detail-shoes_mouth': '鞋口', 'detail-shoes_label': '鞋标',
+                           'intelligence_drop': '吊牌图', 'intelligence_tag': '洗水唛', 'gif': '动图',
+                           'other': '其他'}
         try:
             # 素材中心，分类不存在 或 不存在识别分类，则按照ai识别结果的分类处理
             if not image_classification or ('no-watch' in image_classification):
                 return '未识别'
-            # 其他分类
-            if '_' not in image_classification:
-                return cat_mapping[image_classification]
-            cat, sub_category = image_classification.split('_')
-            if '-' not in cat:
-                if sub_category != "other":
-                    if cat == 'tile':
-                        return cat_mapping[cat] + cat_mapping[sub_category]
-                    return cat_mapping[sub_category]
-                if cat == 'detail':
-                    # 来个默认细节图
-                    return "细节图"
-                # 保持原有识别
-                return self.ai_image_classification
-            model, body = cat.split('-')
-            return cat_mapping[model] + cat_mapping[body] + cat_mapping[sub_category]
+            return storage_to_slot.get(image_classification, '未识别')
+            # # 其他分类
+            # if '_' not in image_classification:
+            #     return cat_mapping[image_classification]
+            # cat, sub_category = image_classification.split('_')
+            # if '-' not in cat:
+            #     if sub_category != "other":
+            #         if cat == 'tile':
+            #             return cat_mapping[cat] + cat_mapping[sub_category]
+            #         return cat_mapping[sub_category]
+            #     if cat == 'detail':
+            #         # 来个默认细节图
+            #         return "细节图"
+            #     # 保持原有识别
+            #     return self.ai_image_classification
+            # model, body = cat.split('-')
+            # return cat_mapping[model] + cat_mapping[body] + cat_mapping[sub_category]
         except Exception as e:
             # logging.error(f"图片{self.filename}, 分类解析失败: {e}", exc_info=True)
             return '未识别'
 
     def deal_image_background(self):
         """
         background : 0 不限 1 透明 2 白底 3 其他背景
@@ -384,14 +411,15 @@
             'top_site': [0, 0],
             'bottom_site': [1, 1]
         }
         crop_point_dict = self.humans.deal_human_crop_point(crop_point_dict)
 
         self.cloths.cloth_classify = cloth_classify  # 期望的衣服
         crop_point_dict = self.cloths.deal_cloth_crop_point(crop_point_dict)
+        crop_point_dict = self.shoes.deal_shoes_crop_point(crop_point_dict)
         self.crop_point = crop_point_dict
         return crop_point_dict
 
     def deal_crop_detail_img(self, ai_result):
         """传入 ai 识别结果，获取到 各个裁剪细节"""
 
         crop_name = '裁剪'
@@ -459,15 +487,14 @@
             image_analysis['human_pose'] = self.add_new_crop_point(image_analysis.get("recognition"),
                                                                    image_analysis.get("human_pose"))
         self.image_width = None
         self.image_height = None
         self.human_body_width = None
         self.human_bodies_list = self.ai_human_pose(image_analysis.get('human_pose'))
 
-
     def calculate_mouth(self, ai_crop_point_dict):
         """
         1.根据 眼镜 鼻子 计算嘴巴的位置
         2.根据眼睛鼻子判断 头顶是否要删除
         3.根据脚踝判断 脚底是否要删除
         """
         # y: 鼻子的y + (鼻子的y - 眼睛最低的y)
@@ -643,15 +670,16 @@
 
         # 人的数量保持一致
         if len(human_bodies_list) != len(human_pose_result):
             return human_pose
 
         for i, human in enumerate(human_bodies_list):
             # ['右踝', '右膝', '右臀', '左臀', '左膝', '左踝', '腰', '脊柱', '颈', '头', '右腕', '右肘', '右肩', '左肩', '左肘', '左腕']
-            r_ank, r_kne, r_hip, l_hip, l_kne, l_ank, pel, spi, nec, hea, r_wri, r_elb, r_sho, l_sho, l_elb, l_wri = human['keypoints']
+            r_ank, r_kne, r_hip, l_hip, l_kne, l_ank, pel, spi, nec, hea, r_wri, r_elb, r_sho, l_sho, l_elb, l_wri = \
+            human['keypoints']
 
             if hea[2] > 0:
                 self.head = True
             if len(human_pose_result[i]['keypoints']) == 17:
                 # 倒着insert 不会改变前面点的index
                 # 在recognition keypoints 内 index 为6 的是腰部
                 human_pose_result[i]['keypoints'].insert(self.HUMAN_BODY_KEY_POINTS.index('left_hip'),
@@ -1006,14 +1034,101 @@
         # 取最大
         crop_point_dict['brand_top']['bottom_site'] = max(brand_bottom_site[0], brand_box[2]), max(
             brand_bottom_site[1], brand_box[3])
         crop_point_dict['brand_bottom'] = crop_point_dict['brand_top']
         return crop_point_dict
 
 
+class Shoes:
+    # 鞋类识别
+    def __init__(self, image_analysis):
+        self.image_analysis = image_analysis
+        self.threshold = 0.6  # 小于0.6不可信
+        self.shoes_list = self.ai_shoes_info(image_analysis.get("recognition"))
+
+    def ai_shoes_info(self, shoes_json):
+        '''计算各个鞋的分类 及box '''
+
+        if not shoes_json:
+            return []
+
+        shoes_list = []
+        try:
+            shoes_info = json.loads(shoes_json)
+            # 获取cloth
+            if not shoes_info.get('clothes'):
+                return []
+            self.image_width, self.image_height = shoes_info['image']['width'], shoes_info['image']['height']
+            for one_shoes in shoes_info['clothes']:
+                if one_shoes['confidence'] < self.threshold:  # 置信度过低
+                    continue
+                if one_shoes['category_id'] != 8:  # 类型不是鞋子
+                    continue
+                shoes = self.deal_shoes(one_shoes)
+                shoes_list.append(shoes)
+        except Exception:
+            raise Exception(f"ai识别结果-资质图box-解析失败: {json.dumps(self.image_analysis)}")
+            # logging.error(f"ai识别结果-资质图box-解析失败: {json.dumps(self.image_analysis)} ", exc_info=True)
+        return shoes_list
+
+    def deal_shoes(self, one_shoes):
+        '''处理下 每个资质图的 box cat_id cat_name confidence'''
+
+        shoes = dict()
+
+        #  服装的区域
+        shoes['box'] = [
+            one_shoes['bbox'][0] / self.image_width,
+            one_shoes['bbox'][1] / self.image_height,
+            one_shoes['bbox'][2] / self.image_width,
+            one_shoes['bbox'][3] / self.image_height
+        ]
+
+        shoes['cat_id'] = one_shoes['category_id']  # 服装分类id
+        shoes['cat_name'] = one_shoes['category']  # 资质图分类name
+        return shoes
+
+    def deal_shoes_crop_point(self, crop_point_dict):
+        if not self.shoes_list:
+            crop_point_dict['shoes_top'] = {
+                'top_site': [0, 0], 'bottom_site': [1, 1]
+            }
+            crop_point_dict['shoes_bottom'] = {
+                'top_site': [0, 0], 'bottom_site': [1, 1]
+            }
+            return crop_point_dict
+
+        for shoes in self.shoes_list:
+            crop_point_dict = self.shoes_crop_point(shoes, crop_point_dict)
+        return crop_point_dict
+
+    def shoes_crop_point(self, shoes, crop_point_dict):
+        # 鞋上边: shoes_top
+        # 鞋下边: shoes_bottom
+
+        shoes_box = shoes['box']
+        if not crop_point_dict.get('shoes_top'):
+            point = dict()
+            point['top_site'] = shoes_box[0], shoes_box[1]
+            point['bottom_site'] = shoes_box[2], shoes_box[3]
+            crop_point_dict['shoes_top'] = crop_point_dict['shoes_bottom'] = point
+            return crop_point_dict
+
+        shoes_top_site = crop_point_dict['shoes_top']['top_site']
+        shoes_bottom_site = crop_point_dict['shoes_bottom']['bottom_site']
+        # 取最小
+        crop_point_dict['shoes_top']['top_site'] = min(shoes_top_site[0], shoes_box[0]), min(shoes_top_site[1],
+                                                                                             shoes_box[1])
+        # 取最大
+        crop_point_dict['shoes_top']['bottom_site'] = max(shoes_bottom_site[0], shoes_box[2]), max(
+            shoes_bottom_site[1], shoes_box[3])
+        crop_point_dict['shoes_bottom'] = crop_point_dict['shoes_top']
+        return crop_point_dict
+
+
 class ImageDetail:
     """
     TB链接：https://thoughts.teambition.com/workspaces/5e37b6adf0f331001a9c172d/docs/607e874e4cc5830001d956c7
 
     从图片中，根据ai识别结果，标识出出细节图的位置
     帽子 hat
     袖口
```

### Comparing `crop_utils-4.3.1/src/crop_utils/img_crop.py` & `crop_utils-4.3.2/src/crop_utils/img_crop.py`

 * *Files 2% similar despite different names*

```diff
@@ -136,17 +136,18 @@
 
 class ImageCrop:
 
     def __init__(self):
         self.si = ShouldIndex()
         # 裁剪点 向上向下兼容顺序顺序
         self.crop_sequence = ['pic_top', 'human_top', 'eye', 'nose', 'ear', 'mouth', 'mandible', 'shoulder',
-                              'elbow',
-                              'wrist', "waist", 'hip', 'knee', 'ankle', 'human_bottom', 'pic_bottom']
-        self.garment_crop_sequence = ['pic_top', 'human_top', 'garment_top', 'garment_bottom', 'human_bottom',
+                              'elbow', 'wrist', "waist", 'hip', 'knee', 'ankle',
+                              'shoes_top', 'shoes_bottom', 'human_bottom', 'pic_bottom']
+        self.garment_crop_sequence = ['pic_top', 'human_top', 'garment_top', 'garment_bottom',
+                                      'shoes_top', 'shoes_bottom', 'human_bottom',
                                       'pic_bottom']
 
         # 记录图片每一步的裁剪流程
         # 具体图片裁剪信息，在裁剪过程中不断计算，更新
         self.set_top_name = None
         self.set_bottom_name = None
         self.set_crop_parameter = None
@@ -678,20 +679,32 @@
                                                   {'top_site': [0, 0], 'bottom_site': [1, 1]})['bottom_site']
 
             crop_top = crop_top_site[1]
             crop_bottom = crop_bottom_site[1]
             crop_left = crop_top_site[0]
             crop_right = crop_bottom_site[0]
             self.si.get_crop_site(['garment_top', 'garment_bottom'], ['garment_top', 'garment_bottom'])
+
+        elif img.img_crop_type == SHOES:  # 鞋类静物图
+            crop_top_site = img.crop_point.get('shoes_top',
+                                               {'top_site': [0, 0], 'bottom_site': [1, 1]})['top_site']
+            crop_bottom_site = img.crop_point.get('shoes_bottom',
+                                                  {'top_site': [0, 0], 'bottom_site': [1, 1]})['bottom_site']
+
+            crop_top = crop_top_site[1]
+            crop_bottom = crop_bottom_site[1]
+            crop_left = crop_top_site[0]
+            crop_right = crop_bottom_site[0]
+            self.si.get_crop_site(['shoes_top', 'shoes_bottom'], ['shoes_top', 'shoes_bottom'])
+
         else:  # 模特图
             top_site = crop_parameter.get(TOP_SITE)
             bottom_site = crop_parameter.get(BOTTOM_SITE)
-            # 取裁剪点/兼容的裁剪点
+            # 取裁剪点 取不到则 图片边缘
             #  Todo 裁剪点 顺序
-
             crop_top_site, crop_top_name = self._from_img_get_top_site(img.crop_point, top_site)
             crop_bottom_site, crop_bottom_name = self._from_img_get_bottom_site(img.crop_point, bottom_site)
 
             self.si.get_crop_site([top_site, bottom_site], [crop_top_name, crop_bottom_name])
 
             crop_top = crop_top_site[1]
             crop_bottom = crop_bottom_site[1]
@@ -756,56 +769,62 @@
             crop_right = max(cloth_box_top[0], cloth_box_bottom[0])
         else:
             crop_left = crop_right = 0.5
 
         return crop_left, crop_right
 
     def _from_img_get_top_site(self, crop_point, top_site):
-        if top_site not in self.crop_sequence:
-            flag_index = self.garment_crop_sequence.index(top_site)
-            crop_top, crop_top_name = None, None
-            while flag_index >= 0:
-                crop_top, crop_top_name = crop_point.get(self.garment_crop_sequence[flag_index]), \
-                                          self.garment_crop_sequence[flag_index]
-                if crop_top:
-                    break
-                flag_index -= 1
-            return crop_top['top_site'], crop_top_name
-
-        flag_index = self.crop_sequence.index(top_site)
-        crop_top, crop_top_name = None, None
-        while flag_index >= 0:
-            crop_top, crop_top_name = crop_point.get(self.crop_sequence[flag_index]), self.crop_sequence[flag_index]
-            if crop_top:
-                break
-            flag_index -= 1
-        return crop_top['top_site'], crop_top_name
+        # if top_site not in self.crop_sequence:
+        #     flag_index = self.garment_crop_sequence.index(top_site)
+        #     crop_top, crop_top_name = None, None
+        #     while flag_index >= 0:
+        #         crop_top, crop_top_name = crop_point.get(self.garment_crop_sequence[flag_index]), \
+        #                                   self.garment_crop_sequence[flag_index]
+        #         if crop_top:
+        #             break
+        #         flag_index -= 1
+        #     return crop_top['top_site'], crop_top_name
+        #
+        # flag_index = self.crop_sequence.index(top_site)
+        # crop_top, crop_top_name = None, None
+        # while flag_index >= 0:
+        #     crop_top, crop_top_name = crop_point.get(self.crop_sequence[flag_index]), self.crop_sequence[flag_index]
+        #     if crop_top:
+        #         break
+        #     flag_index -= 1
+
+        if top_site in crop_point.keys():
+            return crop_point[top_site]['top_site'], top_site
+
+        return crop_point['pic_top']['top_site'], 'pic_top'
 
     def _from_img_get_bottom_site(self, crop_point, bottom_site):
-        if bottom_site not in self.crop_sequence:
-            flag_index = self.garment_crop_sequence.index(bottom_site)
-            crop_bottom, crop_bottom_name = None, None
-            while flag_index < len(self.crop_sequence):
-                crop_bottom, crop_bottom_name = crop_point.get(self.garment_crop_sequence[flag_index]), \
-                                                self.garment_crop_sequence[
-                                                    flag_index]
-                if crop_bottom:
-                    break
-                flag_index += 1
-            return crop_bottom['bottom_site'], crop_bottom_name
-
-        flag_index = self.crop_sequence.index(bottom_site)
-        crop_bottom, crop_bottom_name = None, None
-        while flag_index < len(self.crop_sequence):
-            crop_bottom, crop_bottom_name = crop_point.get(self.crop_sequence[flag_index]), self.crop_sequence[
-                flag_index]
-            if crop_bottom:
-                break
-            flag_index += 1
-        return crop_bottom['bottom_site'], crop_bottom_name
+        # if bottom_site not in self.crop_sequence:
+        #     flag_index = self.garment_crop_sequence.index(bottom_site)
+        #     crop_bottom, crop_bottom_name = None, None
+        #     while flag_index < len(self.crop_sequence):
+        #         crop_bottom, crop_bottom_name = crop_point.get(self.garment_crop_sequence[flag_index]), \
+        #                                         self.garment_crop_sequence[
+        #                                             flag_index]
+        #         if crop_bottom:
+        #             break
+        #         flag_index += 1
+        #     return crop_bottom['bottom_site'], crop_bottom_name
+        #
+        # flag_index = self.crop_sequence.index(bottom_site)
+        # crop_bottom, crop_bottom_name = None, None
+        # while flag_index < len(self.crop_sequence):
+        #     crop_bottom, crop_bottom_name = crop_point.get(self.crop_sequence[flag_index]), self.crop_sequence[
+        #         flag_index]
+        #     if crop_bottom:
+        #         break
+        #     flag_index += 1
+        if bottom_site in crop_point.keys():
+            return crop_point[bottom_site]['bottom_site'], bottom_site
+        return crop_bottom['pic_bottom']['bottom_site'], 'pic_bottom'
 
     def _alternative_interest_center(self, center, slot_height_or_width, transform_height_or_width,
                                      interest_left_or_top,
                                      interest_slot_height_or_width):
         center_ = center * transform_height_or_width
         # 在图片的范围内
         tag_1 = (center_ - interest_slot_height_or_width / 2 - interest_left_or_top) >= 0
```

### Comparing `crop_utils-4.3.1/src/crop_utils.egg-info/PKG-INFO` & `crop_utils-4.3.2/src/crop_utils.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: crop-utils
-Version: 4.3.1
-Summary: 详情页扩边
+Version: 4.3.2
+Summary: 鞋类ai识别
 Home-page: http://git.chaomy.com/libo/ecpro-utils.git
 Author: libo
 Author-email: 6878595@qq.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Description: 为了区分3.0与4.0版本，同时资源图与详情页也共用的一套裁剪逻辑代码。
         
@@ -74,14 +74,14 @@
         
         
         
         # 安装
         
         
         
-        pip install crop-utils==4.3.0 -i  https://pypi.python.org/simple/
+        pip install crop-utils==4.3.1 -i  https://pypi.python.org/simple/
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

