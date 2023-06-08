# Comparing `tmp/commonMethods_zhaozl_green-2.2.tar.gz` & `tmp/commonMethods_zhaozl_green-2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commonMethods_zhaozl_green-2.2.tar", last modified: Wed May 31 12:13:20 2023, max compression
+gzip compressed data, was "commonMethods_zhaozl_green-2.3.tar", last modified: Thu Jun  8 03:38:03 2023, max compression
```

## Comparing `commonMethods_zhaozl_green-2.2.tar` & `commonMethods_zhaozl_green-2.3.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.372518 commonMethods_zhaozl_green-2.2/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      994 2023-05-31 12:13:20.372398 commonMethods_zhaozl_green-2.2/PKG-INFO
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      324 2023-05-31 12:11:38.000000 commonMethods_zhaozl_green-2.2/README.md
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.369574 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2378 2023-05-31 12:09:13.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/__init__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/__version__.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8061 2023-05-31 12:11:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/core.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.372108 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8260 2023-05-31 12:08:15.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_processBar.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1902 2023-05-31 12:08:58.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/__init__.py
-drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-05-31 12:13:20.370340 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      994 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/PKG-INFO
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)      841 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/SOURCES.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/dependency_links.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/requires.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-05-31 12:13:20.000000 commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/top_level.txt
--rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-05-31 12:13:20.372563 commonMethods_zhaozl_green-2.2/setup.cfg
--rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-05-31 12:10:23.000000 commonMethods_zhaozl_green-2.2/setup.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.815474 commonMethods_zhaozl_green-2.3/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)     1027 2023-06-08 03:38:03.815325 commonMethods_zhaozl_green-2.3/PKG-INFO
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      359 2023-06-08 03:36:49.000000 commonMethods_zhaozl_green-2.3/README.md
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.810873 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2605 2023-06-08 03:32:18.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/__init__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)      353 2021-03-20 02:19:04.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/__version__.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8061 2023-05-31 12:11:20.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/core.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.814958 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5919 2021-04-21 06:17:46.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    10898 2021-04-16 08:39:53.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     6639 2021-04-20 02:05:23.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     5354 2021-09-12 12:24:17.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     8260 2023-05-31 12:08:15.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_processBar.py
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)     2084 2023-06-08 03:30:17.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_shuffle.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     1821 2023-05-31 01:17:47.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)    15542 2021-04-21 06:44:27.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     2113 2023-06-08 03:31:57.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/__init__.py
+drwxr-xr-x   0 zhaozhenglei   (501) staff       (20)        0 2023-06-08 03:38:03.812195 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)     1027 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/PKG-INFO
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)      894 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/SOURCES.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)        1 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/dependency_links.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       97 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/requires.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       27 2023-06-08 03:38:03.000000 commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/top_level.txt
+-rw-r--r--   0 zhaozhenglei   (501) staff       (20)       38 2023-06-08 03:38:03.815528 commonMethods_zhaozl_green-2.3/setup.cfg
+-rw-rw-rw-   0 zhaozhenglei   (501) staff       (20)     4066 2023-06-08 03:36:29.000000 commonMethods_zhaozl_green-2.3/setup.py
```

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/__init__.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,9 +40,17 @@
             ** compareWithOthersAverage, 同类测点温度值稳定，单一测点温度测量在正常范围内，但明显高于除本测点外的同类平均值
 
             ** circleSimilarity, 全体测点与均值圆的相似度, 使用向量间的相似度进行衡量
 
             ** modulo， 向量的模计算
 
             ** angleCal， 向量间夹角余弦值计算
+
+        * shuffle: 包括三种方法（之一为构造函数）
+
+            ** 将数据集进行随机打乱
+
+            ** 使用打乱秩序对新的数据集进行打乱
+
+            ** 恢复打乱的数据集
 """
 from .core import *
```

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/core.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/core.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_processBar.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_processBar.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_timeTrans.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py`

 * *Files identical despite different names*

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green/toolbox/__init__.py` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green/toolbox/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,10 +31,18 @@
         ** compareWithOthersAverage, 同类测点温度值稳定，单一测点温度测量在正常范围内，但明显高于除本测点外的同类平均值
 
         ** circleSimilarity, 全体测点与均值圆的相似度, 使用向量间的相似度进行衡量
 
         ** modulo， 向量的模计算
 
         ** angleCal， 向量间夹角余弦值计算
+
+    * shuffle: 包括三种方法（之一为构造函数）
+
+        ** 将数据集进行随机打乱
+
+        ** 使用打乱秩序对新的数据集进行打乱
+
+        ** 恢复打乱的数据集
 """
 
 from . import *
```

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/PKG-INFO` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commonMethods-zhaozl-green
-Version: 2.2
+Version: 2.3
 Summary: timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……
 Home-page: 
 Author: zhaozl1123
 Author-email: 545362989@qq.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -23,7 +23,9 @@
 v1.1 从commonMethods_zhaozl==v3.14版本中，删除bpNetWork的内容，相比v1.0增加proportionalGrouping函数
 
 v1.2 修正了冗余代码
 
 v2.0 简化并优化了脚本，适应Python3.8
 
 v2.2 增加了几种进度条
+
+v2.3 toolbox中增加了Shuffle
```

### Comparing `commonMethods_zhaozl_green-2.2/commonMethods_zhaozl_green.egg-info/SOURCES.txt` & `commonMethods_zhaozl_green-2.3/commonMethods_zhaozl_green.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -9,10 +9,11 @@
 commonMethods_zhaozl_green.egg-info/requires.txt
 commonMethods_zhaozl_green.egg-info/top_level.txt
 commonMethods_zhaozl_green/toolbox/Method_bounceAnalyzer.py
 commonMethods_zhaozl_green/toolbox/Method_comtradeParse.py
 commonMethods_zhaozl_green/toolbox/Method_evennessDetermine.py
 commonMethods_zhaozl_green/toolbox/Method_mysqlOperator.py
 commonMethods_zhaozl_green/toolbox/Method_processBar.py
+commonMethods_zhaozl_green/toolbox/Method_shuffle.py
 commonMethods_zhaozl_green/toolbox/Method_timeTrans.py
 commonMethods_zhaozl_green/toolbox/Method_trendAnalyzer.py
 commonMethods_zhaozl_green/toolbox/__init__.py
```

### Comparing `commonMethods_zhaozl_green-2.2/setup.py` & `commonMethods_zhaozl_green-2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'commonMethods_zhaozl_green'
 DESCRIPTION = 'timeTrans code2Name mysqlOperator printWithColor comtradeParse processBar trendAnalyzer bounceAnalyzer evennessDetermine……'
 URL = ''
 EMAIL = '545362989@qq.com'
 AUTHOR = 'zhaozl1123'
 REQUIRES_PYTHON = '>=3.8.0'
-VERSION = '2.2'
+VERSION = '2.3'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     'numpy==1.24.3', 'joblib>=0.16.0', 'pandas==1.5.3', 'matplotlib>=3.3.0', 'scikit-learn>=1.2.2', 'PyMySQL>=0.10.0'
 ]
 
 # What packages are optional?
```

