# Comparing `tmp/streamlit-super-slider-0.1.1.tar.gz` & `tmp/streamlit-super-slider-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit-super-slider-0.1.1.tar", last modified: Wed May 17 02:50:55 2023, max compression
+gzip compressed data, was "streamlit-super-slider-0.1.2.tar", last modified: Thu Jun  8 11:44:49 2023, max compression
```

## Comparing `streamlit-super-slider-0.1.1.tar` & `streamlit-super-slider-0.1.2.tar`

### file list

```diff
@@ -1,15 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:50:55.818742 streamlit-super-slider-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-17 02:50:39.000000 streamlit-super-slider-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-17 02:50:55.814742 streamlit-super-slider-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-05-17 02:50:39.000000 streamlit-super-slider-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 02:50:55.818742 streamlit-super-slider-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      891 2023-05-17 02:50:39.000000 streamlit-super-slider-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:50:55.814742 streamlit-super-slider-0.1.1/streamlit_super_slider/
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-17 02:50:39.000000 streamlit-super-slider-0.1.1/streamlit_super_slider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 02:50:39.000000 streamlit-super-slider-0.1.1/streamlit_super_slider/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 02:50:55.814742 streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2424 2023-05-17 02:50:55.000000 streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      324 2023-05-17 02:50:55.000000 streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 02:50:55.000000 streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-17 02:50:55.000000 streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 02:50:55.000000 streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/top_level.txt
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:49.218721 streamlit-super-slider-0.1.2/
+-rw-r--r--   0 dviri     (1976) develop12  (1000)       57 2023-05-16 11:46:24.000000 streamlit-super-slider-0.1.2/MANIFEST.in
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     2713 2023-06-08 11:44:49.205738 streamlit-super-slider-0.1.2/PKG-INFO
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     2301 2023-06-08 11:40:47.000000 streamlit-super-slider-0.1.2/README.md
+-rw-r--r--   0 dviri     (1976) develop12  (1000)       38 2023-06-08 11:44:49.221671 streamlit-super-slider-0.1.2/setup.cfg
+-rw-r--r--   0 dviri     (1976) develop12  (1000)      891 2023-06-08 11:44:32.000000 streamlit-super-slider-0.1.2/setup.py
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:48.855676 streamlit-super-slider-0.1.2/streamlit_super_slider/
+-rw-r--r--   0 dviri     (1976) develop12  (1000)      781 2023-05-16 11:29:53.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/__init__.py
+-rw-r--r--   0 dviri     (1976) develop12  (1000)      148 2023-05-16 11:01:24.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/app.py
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:48.767537 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:48.977196 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/
+-rw-r--r--   0 dviri     (1976) develop12  (1000)      890 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/asset-manifest.json
+-rw-r--r--   0 dviri     (1976) develop12  (1000)   197459 2023-05-16 11:27:49.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/bootstrap.min.css
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     2165 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/index.html
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:48.780736 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:49.012765 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/css/
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     5533 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/css/2.4e8595b7.chunk.css
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     8187 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/css/2.4e8595b7.chunk.css.map
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:49.195255 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/
+-rw-r--r--   0 dviri     (1976) develop12  (1000)   616197 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/2.cf48578d.chunk.js
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     2593 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/2.cf48578d.chunk.js.LICENSE.txt
+-rw-r--r--   0 dviri     (1976) develop12  (1000)  2526902 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/2.cf48578d.chunk.js.map
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     3377 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/main.f737ba85.chunk.js
+-rw-r--r--   0 dviri     (1976) develop12  (1000)    14782 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/main.f737ba85.chunk.js.map
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     1598 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/runtime-main.f2af49fe.js
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     8383 2023-05-16 11:28:25.000000 streamlit-super-slider-0.1.2/streamlit_super_slider/frontend/build/static/js/runtime-main.f2af49fe.js.map
+drwxr-sr-x   0 dviri     (1976) develop12  (1000)        0 2023-06-08 11:44:48.937210 streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     2713 2023-06-08 11:44:47.000000 streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/PKG-INFO
+-rw-r--r--   0 dviri     (1976) develop12  (1000)     1147 2023-06-08 11:44:48.000000 streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/SOURCES.txt
+-rw-r--r--   0 dviri     (1976) develop12  (1000)        1 2023-06-08 11:44:47.000000 streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/dependency_links.txt
+-rw-r--r--   0 dviri     (1976) develop12  (1000)       16 2023-06-08 11:44:47.000000 streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/requires.txt
+-rw-r--r--   0 dviri     (1976) develop12  (1000)       23 2023-06-08 11:44:47.000000 streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/top_level.txt
```

### Comparing `streamlit-super-slider-0.1.1/PKG-INFO` & `streamlit-super-slider-0.1.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-super-slider
-Version: 0.1.1
+Version: 0.1.2
 Summary: A slider with a lot more features in it than the built in one.
 Home-page: https://github.com/fgdvir/streamlit-super-slider
 Author: Dvir Itzkovits
 Author-email: dvir.itzko@gmail.com
 Keywords: Python,Streamlit,React,JavaScript
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -60,12 +60,21 @@
 
 # Use the Streamlit Super Slider component
 slider_value = st_slider(min_value, max_value, default_value)
 
 st.write(f"Selected value: {slider_value}")
 ```
 
+## Demo
+In the following demo you can see usage of the slider to show images, and all the different ways to chose where to go:
+* keybaord shortcut
+* Pressing the arrows buttons
+* Changing the value in the input text box
+* Dragging the slider
+
+![Demo](./assets/ezgif.com-video-to-gif.gif)
+
 ## Contributing
 
 We welcome contributions to the Streamlit Super Slider project. If you'd like to report bugs, request features, or contribute to the code, please [open an issue](https://github.com/fgdvir/streamlit-super-slider/issues) or [submit a pull request](https://github.com/fgdvir/streamlit-super-slider/pulls) on the GitHub repository.
```

### Comparing `streamlit-super-slider-0.1.1/README.md` & `streamlit-super-slider-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -48,12 +48,21 @@
 
 # Use the Streamlit Super Slider component
 slider_value = st_slider(min_value, max_value, default_value)
 
 st.write(f"Selected value: {slider_value}")
 ```
 
+## Demo
+In the following demo you can see usage of the slider to show images, and all the different ways to chose where to go:
+* keybaord shortcut
+* Pressing the arrows buttons
+* Changing the value in the input text box
+* Dragging the slider
+
+![Demo](./assets/ezgif.com-video-to-gif.gif)
+
 ## Contributing
 
 We welcome contributions to the Streamlit Super Slider project. If you'd like to report bugs, request features, or contribute to the code, please [open an issue](https://github.com/fgdvir/streamlit-super-slider/issues) or [submit a pull request](https://github.com/fgdvir/streamlit-super-slider/pulls) on the GitHub repository.
```

### Comparing `streamlit-super-slider-0.1.1/setup.py` & `streamlit-super-slider-0.1.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='streamlit-super-slider',
-    version='0.1.1',
+    version='0.1.2',
     author='Dvir Itzkovits',
     author_email='dvir.itzko@gmail.com',
     description='A slider with a lot more features in it than the built in one.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/fgdvir/streamlit-super-slider',
     # packages=['streamlit-super-slider'],
```

### Comparing `streamlit-super-slider-0.1.1/streamlit_super_slider/__init__.py` & `streamlit-super-slider-0.1.2/streamlit_super_slider/__init__.py`

 * *Files identical despite different names*

### Comparing `streamlit-super-slider-0.1.1/streamlit_super_slider.egg-info/PKG-INFO` & `streamlit-super-slider-0.1.2/streamlit_super_slider.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-super-slider
-Version: 0.1.1
+Version: 0.1.2
 Summary: A slider with a lot more features in it than the built in one.
 Home-page: https://github.com/fgdvir/streamlit-super-slider
 Author: Dvir Itzkovits
 Author-email: dvir.itzko@gmail.com
 Keywords: Python,Streamlit,React,JavaScript
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
@@ -60,12 +60,21 @@
 
 # Use the Streamlit Super Slider component
 slider_value = st_slider(min_value, max_value, default_value)
 
 st.write(f"Selected value: {slider_value}")
 ```
 
+## Demo
+In the following demo you can see usage of the slider to show images, and all the different ways to chose where to go:
+* keybaord shortcut
+* Pressing the arrows buttons
+* Changing the value in the input text box
+* Dragging the slider
+
+![Demo](./assets/ezgif.com-video-to-gif.gif)
+
 ## Contributing
 
 We welcome contributions to the Streamlit Super Slider project. If you'd like to report bugs, request features, or contribute to the code, please [open an issue](https://github.com/fgdvir/streamlit-super-slider/issues) or [submit a pull request](https://github.com/fgdvir/streamlit-super-slider/pulls) on the GitHub repository.
```

