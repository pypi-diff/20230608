# Comparing `tmp/getmodelspec-1.0.332.tar.gz` & `tmp/getmodelspec-1.0.333.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\getmodelspec-1.0.332.tar", last modified: Thu Jun  8 15:41:19 2023, max compression
+gzip compressed data, was "dist\getmodelspec-1.0.333.tar", last modified: Thu Jun  8 15:54:05 2023, max compression
```

## Comparing `getmodelspec-1.0.332.tar` & `getmodelspec-1.0.333.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/
--rw-rw-rw-   0        0        0      351 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/PKG-INFO
--rw-rw-rw-   0        0        0     1572 2023-06-07 21:30:31.000000 getmodelspec-1.0.332/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/getmodelspec/
--rw-rw-rw-   0        0        0      257 2023-06-08 13:56:50.000000 getmodelspec-1.0.332/getmodelspec/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/getmodelspec/src/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.332/getmodelspec/src/__init__.py
--rw-rw-rw-   0        0        0     1257 2023-06-08 15:34:23.000000 getmodelspec-1.0.332/getmodelspec/src/get_score.py
--rw-rw-rw-   0        0        0     3171 2023-06-08 15:33:04.000000 getmodelspec-1.0.332/getmodelspec/src/get_spepcifications.py
--rw-rw-rw-   0        0        0     8364 2023-06-08 15:40:16.000000 getmodelspec-1.0.332/getmodelspec/src/sony.py
--rw-rw-rw-   0        0        0    12888 2023-06-08 15:40:16.000000 getmodelspec-1.0.332/getmodelspec/src/sony_b.py
--rw-rw-rw-   0        0        0      507 2023-06-08 14:05:25.000000 getmodelspec-1.0.332/getmodelspec/test.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/getmodelspec/tools/
--rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.332/getmodelspec/tools/__init__.py
--rw-rw-rw-   0        0        0     1519 2023-06-08 14:24:01.000000 getmodelspec-1.0.332/getmodelspec/tools/functions.py
--rw-rw-rw-   0        0        0     5183 2023-06-08 10:31:24.000000 getmodelspec-1.0.332/getmodelspec/tools/webdriver.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/getmodelspec.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-08 15:41:18.000000 getmodelspec-1.0.332/getmodelspec.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      528 2023-06-08 15:41:18.000000 getmodelspec-1.0.332/getmodelspec.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 15:41:18.000000 getmodelspec-1.0.332/getmodelspec.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-08 15:41:18.000000 getmodelspec-1.0.332/getmodelspec.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       13 2023-06-08 15:41:18.000000 getmodelspec-1.0.332/getmodelspec.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-06-08 15:41:18.000000 getmodelspec-1.0.332/getmodelspec.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 15:41:19.000000 getmodelspec-1.0.332/setup.cfg
--rw-rw-rw-   0        0        0      775 2023-06-08 15:41:17.000000 getmodelspec-1.0.332/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/
+-rw-rw-rw-   0        0        0      351 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/PKG-INFO
+-rw-rw-rw-   0        0        0     1572 2023-06-07 21:30:31.000000 getmodelspec-1.0.333/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/getmodelspec/
+-rw-rw-rw-   0        0        0      255 2023-06-08 15:46:55.000000 getmodelspec-1.0.333/getmodelspec/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/getmodelspec/src/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:11.000000 getmodelspec-1.0.333/getmodelspec/src/__init__.py
+-rw-rw-rw-   0        0        0     8512 2023-06-08 15:53:39.000000 getmodelspec-1.0.333/getmodelspec/src/sony.py
+-rw-rw-rw-   0        0        0    12888 2023-06-08 15:40:16.000000 getmodelspec-1.0.333/getmodelspec/src/sony_b.py
+-rw-rw-rw-   0        0        0     1264 2023-06-08 15:46:55.000000 getmodelspec-1.0.333/getmodelspec/src/tv_score.py
+-rw-rw-rw-   0        0        0     3168 2023-06-08 15:46:55.000000 getmodelspec-1.0.333/getmodelspec/src/tv_spepcifications.py
+-rw-rw-rw-   0        0        0      506 2023-06-08 15:46:55.000000 getmodelspec-1.0.333/getmodelspec/test.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/getmodelspec/tools/
+-rw-rw-rw-   0        0        0        0 2023-06-05 07:20:04.000000 getmodelspec-1.0.333/getmodelspec/tools/__init__.py
+-rw-rw-rw-   0        0        0     1519 2023-06-08 14:24:01.000000 getmodelspec-1.0.333/getmodelspec/tools/functions.py
+-rw-rw-rw-   0        0        0     5183 2023-06-08 10:31:24.000000 getmodelspec-1.0.333/getmodelspec/tools/webdriver.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/getmodelspec.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-08 15:54:04.000000 getmodelspec-1.0.333/getmodelspec.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-06-08 15:54:04.000000 getmodelspec-1.0.333/getmodelspec.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:54:04.000000 getmodelspec-1.0.333/getmodelspec.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-08 15:54:04.000000 getmodelspec-1.0.333/getmodelspec.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 15:54:04.000000 getmodelspec-1.0.333/getmodelspec.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 15:54:04.000000 getmodelspec-1.0.333/getmodelspec.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 15:54:05.000000 getmodelspec-1.0.333/setup.cfg
+-rw-rw-rw-   0        0        0      775 2023-06-08 15:54:00.000000 getmodelspec-1.0.333/setup.py
```

### Comparing `getmodelspec-1.0.332/README.md` & `getmodelspec-1.0.333/README.md`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.332/getmodelspec/src/get_spepcifications.py` & `getmodelspec-1.0.333/getmodelspec/src/tv_spepcifications.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 import requests
 from bs4 import BeautifulSoup
 import time
 from ..tools.functions import *
 
 
-class GetSepcifications:
+class Sepcifications:
     def __init__(self, escapeNum:int=200):
         self.escapeNum = escapeNum
         self.dictUrlModel = {"sony":"https://www.displayspecifications.com/en/brand/47e6f",
                              "lge":"",
                              "panasonic":"",
                              "hisense":"",
                              "tpv":"",
```

### Comparing `getmodelspec-1.0.332/getmodelspec/src/sony.py` & `getmodelspec-1.0.333/getmodelspec/src/sony.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,47 +8,48 @@
 from selenium.webdriver.support.ui import WebDriverWait
 from selenium.webdriver.support import expected_conditions as EC
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.common.exceptions import TimeoutException
 
 from ..tools.functions import *
 from ..tools.webdriver import WebDriver
-from ..src.get_spepcifications import GetSepcifications
+from ..src.tv_spepcifications import Sepcifications
+from ..src.tv_score import Score
 
 ## 가격 정보만 찾기
 
 
 class GetSONY:
     def __init__(self, envr:str=None):
         self.weakCon = 'weak'
         self.waitTime = 5
 
         self.envr = envr
-        self.dir_1st = "sony/log/MainSeries"
-        self.dir_2nd = "sony/log/SubSeries"
+        self.dir_1st = "sony/log/Stream"
+        self.dir_2nd = "sony/log/Series"
         self.dir_3rd = "sony/log/models"
         makeDir(self.dir_1st)
         makeDir(self.dir_2nd)
         makeDir(self.dir_3rd)
         pass
 
     # #
     def getModels(self, toExcel:bool = True) -> pd.DataFrame:
 
         # 메인 페이지에서 시리즈를 추출
-        seriesUrls = self.__getPage1st__(url= 'https://electronics.sony.com/tv-video/televisions/c/all-tvs')
+        seriesUrls = self.__getStream__(url= 'https://electronics.sony.com/tv-video/televisions/c/all-tvs')
 
         # ==========================================================================
         backUp(seriesUrls, "seriesUrls")
         # ==========================================================================
 
         ## 서브 시리즈 페이지에서 모델을 추출
         dictAllSeries = {}
         for url in seriesUrls:
-            dictSeries = self.__getPage2nd__(url=url)
+            dictSeries = self.__getSeries__(url=url)
             print(dictSeries)
             dictAllSeries.update(dictSeries)
         print("Number of all Series:", len(dictAllSeries))
 
         # ==========================================================================
         backUp(dictAllSeries, "dictAllSeries")
         # with open(f"dictAllSeries.pickle", "rb") as file:
@@ -56,19 +57,20 @@
         # ==========================================================================
 
         # 모든 모델 리스트를 추출
         dictModels = {}
         for cnt, model in enumerate(dictAllSeries.keys()):
             print(f"{cnt+1}/{len(dictAllSeries)} | {model}")
             try:
-                dictModels.update(self.__getPage3rd__(model))
+                dictModels.update({model:self.__getSpec__(model)})
+
             except:
                 print(f"fail to get info from {model}")
 
-                dictModels.update({getNamefromURL(model): dict()})
+                dictModels.update({model:self.__getSpec__(model)})
                 pass
 
         dfModels = pd.DataFrame.from_dict(dictModels, orient="index")
         dfModels = dfModels.rename_axis('model').reset_index()
 
         if toExcel == True:
             fileName = f"sony_TV_series_{date.today().strftime('%Y-%m-%d')}.xlsx"
@@ -78,15 +80,15 @@
 
         dfModels = self.__getData4th__(dfModels)
 
 
         return dfModels
 
     ###=====================get info main page====================================##
-    def __getPage1st__(self, url:str) -> set:
+    def __getStream__(self, url:str) -> set:
         set_mainSeries = set()
         scrolling_cnt: int = 10
 
         wd =  WebDriver.get_crome()
         wd.get(url=url)
         wait = WebDriverWait(wd, 30)
 
@@ -112,15 +114,15 @@
 
             wd.save_screenshot(f"./{self.dir_1st}/Main_Series_{cnt}_{get_today()}.png")  # 스크린 샷
         wd.quit()
         print("Number of SONY Main Series:", len(set_mainSeries))
         return set_mainSeries
 
     ###=====================get info Sub page====================================##
-    def __getPage2nd__(self, url: str) -> dict:
+    def __getSeries__(self, url: str) -> dict:
         cntTryTotal = 5
         for cntTry in range(cntTryTotal):
             try:
                 dictSeries = {}
                 wd = WebDriver.get_crome()
                 wd.get(url=url)
                 print("connect to", url)
@@ -153,36 +155,36 @@
                 return dictSeries
             except Exception as e:
                 wd.quit()
                 waitingPage(self.waitTime)
                 print(f"stage 2nd try: {cntTry}/{cntTryTotal}")
 
     ###======================final stage===============================##
-    def __getPage3rd__(self, model) -> dict:
-        specs = GetSepcifications()
-
-
+    def __getSpec__(self, model) -> dict:
+        specs = Sepcifications()
+        score = Score()
         dictSpec = specs.getSpec(maker="sony", )
+        series = model.split("-")[1][2:-1]
+        dictSpec.update(score.getRthinsScore(series))
         return dictSpec
-
         pass
 
     def __getData4th__(self, dfModels):
         new_columns = dfModels['model'].apply(self.__extractInfo__)
         df_combined = pd.concat([new_columns, dfModels], axis=1).set_index('model')
         return df_combined
 
 
 # ===============================
 
-    def __extractInfo__(self, row):
-        grade = row.split("-")[0]
-        size = row.split("-")[1][:2]
-        series = row.split("-")[1][2:-1]
-        year = row.split("-")[1][-1]
+    def __extractInfo__(self, model):
+        grade = model.split("-")[0]
+        size = model.split("-")[1][:2]
+        series = model.split("-")[1][2:-1]
+        year = model.split("-")[1][-1]
 
         year_mapping = {
             "N": 2025,
             "M": 2024,
             'L': 2023,
             'K': 2022,
             'J': 2021,
```

### Comparing `getmodelspec-1.0.332/getmodelspec/src/sony_b.py` & `getmodelspec-1.0.333/getmodelspec/src/sony_b.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.332/getmodelspec/tools/functions.py` & `getmodelspec-1.0.333/getmodelspec/tools/functions.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.332/getmodelspec/tools/webdriver.py` & `getmodelspec-1.0.333/getmodelspec/tools/webdriver.py`

 * *Files identical despite different names*

### Comparing `getmodelspec-1.0.332/getmodelspec.egg-info/SOURCES.txt` & `getmodelspec-1.0.333/getmodelspec.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,14 @@
 getmodelspec.egg-info/PKG-INFO
 getmodelspec.egg-info/SOURCES.txt
 getmodelspec.egg-info/dependency_links.txt
 getmodelspec.egg-info/entry_points.txt
 getmodelspec.egg-info/requires.txt
 getmodelspec.egg-info/top_level.txt
 getmodelspec/src/__init__.py
-getmodelspec/src/get_score.py
-getmodelspec/src/get_spepcifications.py
 getmodelspec/src/sony.py
 getmodelspec/src/sony_b.py
+getmodelspec/src/tv_score.py
+getmodelspec/src/tv_spepcifications.py
 getmodelspec/tools/__init__.py
 getmodelspec/tools/functions.py
 getmodelspec/tools/webdriver.py
```

### Comparing `getmodelspec-1.0.332/setup.py` & `getmodelspec-1.0.333/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='getmodelspec',
-    version='1.0.332',
+    version='1.0.333',
     author='xikest',
     description='get model spec,',
     packages=find_packages(),
     python_requires='>=3.7',
     install_requires=[
         'numpy',
         'pandas',
```

