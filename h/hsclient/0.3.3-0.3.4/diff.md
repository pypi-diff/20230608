# Comparing `tmp/hsclient-0.3.3.tar.gz` & `tmp/hsclient-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hsclient-0.3.3.tar", last modified: Wed Apr 19 20:50:47 2023, max compression
+gzip compressed data, was "hsclient-0.3.4.tar", last modified: Thu Jun  8 16:12:11 2023, max compression
```

## Comparing `hsclient-0.3.3.tar` & `hsclient-0.3.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:50:47.155613 hsclient-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-04-19 20:50:37.000000 hsclient-0.3.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-19 20:50:47.155613 hsclient-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-04-19 20:50:37.000000 hsclient-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:50:47.155613 hsclient-0.3.3/hsclient/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42466 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/hydroshare.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/json_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/oauth2_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-19 20:50:37.000000 hsclient-0.3.3/hsclient/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 20:50:47.155613 hsclient-0.3.3/hsclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4084 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-19 20:50:47.000000 hsclient-0.3.3/hsclient.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-19 20:50:47.155613 hsclient-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-04-19 20:50:37.000000 hsclient-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:12:11.827695 hsclient-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 16:11:58.000000 hsclient-0.3.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-08 16:12:11.827695 hsclient-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-08 16:11:58.000000 hsclient-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:12:11.823695 hsclient-0.3.4/hsclient/
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 16:11:58.000000 hsclient-0.3.4/hsclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63541 2023-06-08 16:11:58.000000 hsclient-0.3.4/hsclient/hydroshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-08 16:11:58.000000 hsclient-0.3.4/hsclient/json_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 16:11:58.000000 hsclient-0.3.4/hsclient/oauth2_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-08 16:11:58.000000 hsclient-0.3.4/hsclient/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:12:11.827695 hsclient-0.3.4/hsclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-08 16:12:11.000000 hsclient-0.3.4/hsclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-06-08 16:12:11.000000 hsclient-0.3.4/hsclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:12:11.000000 hsclient-0.3.4/hsclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-06-08 16:12:11.000000 hsclient-0.3.4/hsclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 16:12:11.000000 hsclient-0.3.4/hsclient.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-08 16:12:11.827695 hsclient-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-06-08 16:11:58.000000 hsclient-0.3.4/setup.py
```

### Comparing `hsclient-0.3.3/LICENSE.txt` & `hsclient-0.3.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.3/PKG-INFO` & `hsclient-0.3.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: hsclient
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python client for managing HydroShare resources
 Home-page: https://github.com/hydroshare/hsclient
 Author: Scott Black
 Author-email: scott.black@usu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: pandas
+Provides-Extra: xarray
+Provides-Extra: rasterio
+Provides-Extra: fiona
+Provides-Extra: all
 License-File: LICENSE.txt
 
 # hsclient
 A python client for interacting with HydroShare in an object oriented way.
 
 ## Jupyter Notebooks
 HydroShare has a resource with example notebooks.  Click [here](https://www.hydroshare.org/resource/7561aa12fd824ebb8edbee05af19b910/) then click the blue `Open with...` dropdown and select `Cuahsi Jupyterhub` to launch the notebooks into a Jupyter Environment to start using this project.
```

### Comparing `hsclient-0.3.3/README.md` & `hsclient-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.3/hsclient/json_models.py` & `hsclient-0.3.4/hsclient/json_models.py`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.3/hsclient/utils.py` & `hsclient-0.3.4/hsclient/utils.py`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.3/hsclient.egg-info/PKG-INFO` & `hsclient-0.3.4/hsclient.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,27 @@
 Metadata-Version: 2.1
 Name: hsclient
-Version: 0.3.3
+Version: 0.3.4
 Summary: A python client for managing HydroShare resources
 Home-page: https://github.com/hydroshare/hsclient
 Author: Scott Black
 Author-email: scott.black@usu.edu
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.6
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+Provides-Extra: pandas
+Provides-Extra: xarray
+Provides-Extra: rasterio
+Provides-Extra: fiona
+Provides-Extra: all
 License-File: LICENSE.txt
 
 # hsclient
 A python client for interacting with HydroShare in an object oriented way.
 
 ## Jupyter Notebooks
 HydroShare has a resource with example notebooks.  Click [here](https://www.hydroshare.org/resource/7561aa12fd824ebb8edbee05af19b910/) then click the blue `Open with...` dropdown and select `Cuahsi Jupyterhub` to launch the notebooks into a Jupyter Environment to start using this project.
```

### Comparing `hsclient-0.3.3/setup.cfg` & `hsclient-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `hsclient-0.3.3/setup.py` & `hsclient-0.3.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import pathlib
 from setuptools import setup, find_packages
 
 README = (pathlib.Path(__file__).parent / "README.md").read_text()
 
 setup(
     name='hsclient',
-    version='0.3.3',
+    version='0.3.4',
     packages=find_packages(include=['hsclient', 'hsclient.*'],
                            exclude=("tests",)),
     install_requires=[
         'hsmodels>=0.5.5',
         'requests',
         'requests_oauthlib',
-        'pandas'
     ],
+    extras_require={
+        "pandas": ["pandas"],
+        "xarray": ["netCDF4", "xarray"],
+        "rasterio": ["rasterio"],
+        "fiona": ["fiona"],
+        "all": ["pandas", "netCDF4", "xarray", "rasterio", "fiona"],
+    },
     url='https://github.com/hydroshare/hsclient',
     license='MIT',
     author='Scott Black',
     author_email='scott.black@usu.edu',
     description='A python client for managing HydroShare resources',
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     long_description=README,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
```

