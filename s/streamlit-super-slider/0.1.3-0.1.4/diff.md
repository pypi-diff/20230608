# Comparing `tmp/streamlit-super-slider-0.1.3.tar.gz` & `tmp/streamlit-super-slider-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-super-slider-0.1.3.tar", last modified: Thu Jun  8 11:52:37 2023, max compression
+gzip compressed data, was "streamlit-super-slider-0.1.4.tar", last modified: Thu Jun  8 11:59:56 2023, max compression
```

## Comparing `streamlit-super-slider-0.1.3.tar` & `streamlit-super-slider-0.1.4.tar`

### file list

```diff
@@ -1,32 +1,15 @@
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.662963 streamlit-super-slider-0.1.3/
--rw-r--r--   0 dviri     (1976) develop12  (1000)       57 2023-06-08 11:49:56.000000 streamlit-super-slider-0.1.3/MANIFEST.in
--rw-r--r--   0 dviri     (1976) develop12  (1000)     2713 2023-06-08 11:52:37.660861 streamlit-super-slider-0.1.3/PKG-INFO
--rw-r--r--   0 dviri     (1976) develop12  (1000)     2301 2023-06-08 11:40:47.000000 streamlit-super-slider-0.1.3/README.md
--rw-r--r--   0 dviri     (1976) develop12  (1000)       38 2023-06-08 11:52:37.663878 streamlit-super-slider-0.1.3/setup.cfg
--rw-r--r--   0 dviri     (1976) develop12  (1000)      891 2023-06-08 11:52:23.000000 streamlit-super-slider-0.1.3/setup.py
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.534389 streamlit-super-slider-0.1.3/streamlit_super_slider/
--rw-r--r--   0 dviri     (1976) develop12  (1000)      781 2023-05-16 11:29:53.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/__init__.py
--rw-r--r--   0 dviri     (1976) develop12  (1000)      148 2023-05-16 11:01:24.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/app.py
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.501778 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.585138 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/
--rw-r--r--   0 dviri     (1976) develop12  (1000)      890 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/asset-manifest.json
--rw-r--r--   0 dviri     (1976) develop12  (1000)   197459 2023-05-16 11:27:49.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/bootstrap.min.css
--rw-r--r--   0 dviri     (1976) develop12  (1000)     2165 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/index.html
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.508729 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.599676 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/css/
--rw-r--r--   0 dviri     (1976) develop12  (1000)     5533 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/css/2.4e8595b7.chunk.css
--rw-r--r--   0 dviri     (1976) develop12  (1000)     8187 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/css/2.4e8595b7.chunk.css.map
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.657771 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/
--rw-r--r--   0 dviri     (1976) develop12  (1000)   616197 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/2.cf48578d.chunk.js
--rw-r--r--   0 dviri     (1976) develop12  (1000)     2593 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/2.cf48578d.chunk.js.LICENSE.txt
--rw-r--r--   0 dviri     (1976) develop12  (1000)  2526902 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/2.cf48578d.chunk.js.map
--rw-r--r--   0 dviri     (1976) develop12  (1000)     3377 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/main.f737ba85.chunk.js
--rw-r--r--   0 dviri     (1976) develop12  (1000)    14782 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/main.f737ba85.chunk.js.map
--rw-r--r--   0 dviri     (1976) develop12  (1000)     1598 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/runtime-main.f2af49fe.js
--rw-r--r--   0 dviri     (1976) develop12  (1000)     8383 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.3/streamlit_super_slider/frontend/build/static/js/runtime-main.f2af49fe.js.map
-drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:52:37.566768 streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/
--rw-r--r--   0 dviri     (1976) develop12  (1000)     2713 2023-06-08 11:52:36.000000 streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/PKG-INFO
--rw-r--r--   0 dviri     (1976) develop12  (1000)     1147 2023-06-08 11:52:37.000000 streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/SOURCES.txt
--rw-r--r--   0 dviri     (1976) develop12  (1000)        1 2023-06-08 11:52:36.000000 streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/dependency_links.txt
--rw-r--r--   0 dviri     (1976) develop12  (1000)       16 2023-06-08 11:52:36.000000 streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/requires.txt
--rw-r--r--   0 dviri     (1976) develop12  (1000)       23 2023-06-08 11:52:36.000000 streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:59:56.572767 streamlit-super-slider-0.1.4/streamlit_super_slider/
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/streamlit_super_slider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-08 11:59:45.000000 streamlit-super-slider-0.1.4/streamlit_super_slider/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:59:56.576767 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      324 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 11:59:56.000000 streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/top_level.txt
```

### Comparing `streamlit-super-slider-0.1.3/PKG-INFO` & `streamlit-super-slider-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-super-slider
-Version: 0.1.3
+Version: 0.1.4
 Summary: A slider with a lot more features in it than the built in one.
 Home-page: https://github.com/fgdvir/streamlit-super-slider
 Author: Dvir Itzkovits
 Author-email: dvir.itzko@gmail.com
 Keywords: Python,Streamlit,React,JavaScript
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

### Comparing `streamlit-super-slider-0.1.3/README.md` & `streamlit-super-slider-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `streamlit-super-slider-0.1.3/setup.py` & `streamlit-super-slider-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='streamlit-super-slider',
-    version='0.1.3',
+    version='0.1.4',
     author='Dvir Itzkovits',
     author_email='dvir.itzko@gmail.com',
     description='A slider with a lot more features in it than the built in one.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/fgdvir/streamlit-super-slider',
     # packages=['streamlit-super-slider'],
```

### Comparing `streamlit-super-slider-0.1.3/streamlit_super_slider/__init__.py` & `streamlit-super-slider-0.1.4/streamlit_super_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-super-slider-0.1.3/streamlit_super_slider.egg-info/PKG-INFO` & `streamlit-super-slider-0.1.4/streamlit_super_slider.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-super-slider
-Version: 0.1.3
+Version: 0.1.4
 Summary: A slider with a lot more features in it than the built in one.
 Home-page: https://github.com/fgdvir/streamlit-super-slider
 Author: Dvir Itzkovits
 Author-email: dvir.itzko@gmail.com
 Keywords: Python,Streamlit,React,JavaScript
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
```

