# Comparing `tmp/pyRealEstate-0.0.7.tar.gz` & `tmp/pyRealEstate-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyRealEstate-0.0.7.tar", last modified: Mon Jun  5 17:41:31 2023, max compression
+gzip compressed data, was "pyRealEstate-0.0.8.tar", last modified: Wed Jun  7 20:10:19 2023, max compression
```

## Comparing `pyRealEstate-0.0.7.tar` & `pyRealEstate-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/pyRealEstate/
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/Pre_Processing.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/RealEstateMetrics.py
--rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/Time_Trending.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyRealEstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/pyRealEstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-05 17:41:31.000000 pyRealEstate-0.0.7/pyRealEstate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pypi_description.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 17:41:21.000000 pyRealEstate-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-05 17:41:31.285199 pyRealEstate-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:10:19.856790 pyRealEstate-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-07 20:10:19.856790 pyRealEstate-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:10:19.856790 pyRealEstate-0.0.8/pyRealEstate/
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/pyRealEstate/Pre_Processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2839 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/pyRealEstate/RealEstateMetrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/pyRealEstate/Time_Trending.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/pyRealEstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:10:19.856790 pyRealEstate-0.0.8/pyRealEstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-06-07 20:10:19.000000 pyRealEstate-0.0.8/pyRealEstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-07 20:10:19.000000 pyRealEstate-0.0.8/pyRealEstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:10:19.000000 pyRealEstate-0.0.8/pyRealEstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 20:10:19.000000 pyRealEstate-0.0.8/pyRealEstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 20:10:19.000000 pyRealEstate-0.0.8/pyRealEstate.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/pypi_description.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 20:10:08.000000 pyRealEstate-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-06-07 20:10:19.856790 pyRealEstate-0.0.8/setup.cfg
```

### Comparing `pyRealEstate-0.0.7/LICENSE` & `pyRealEstate-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.7/PKG-INFO` & `pyRealEstate-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.7
+Version: 0.0.8
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.0.7/README.md` & `pyRealEstate-0.0.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -5,9 +5,9 @@
 ## Installation
 
 the pyRealEstate package is available on [PyPi](https://pypi.org/project/pyRealEstate). Simply run: 
 ```
 pip install pyRealEstate
 ```
 ## AVM Evalutation Metrics
-pyRealEstate can provide metrics on the evaluation of your AVM( AAutomated Valuation Model) such as the weighted mean sale ratio, COD (Coefficient Of Disspersion), and PRD ( Price Related Differential) please visit the wiki for detailed documentation [pyRealEstate Evaluation](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/AVM-Evaluation-Metrics)
+pyRealEstate can provide metrics on the evaluation of your AVM (Automated Valuation Model) such as the weighted mean sale ratio, COD (Coefficient Of Disspersion), and PRD ( Price Related Differential) please visit the wiki for detailed documentation [pyRealEstate Evaluation](https://github.com/Joshua-Data-Wizard/PyRealEstate/wiki/AVM-Evaluation-Metrics)
```

### Comparing `pyRealEstate-0.0.7/pyRealEstate/Pre_Processing.py` & `pyRealEstate-0.0.8/pyRealEstate/Pre_Processing.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.7/pyRealEstate/Time_Trending.py` & `pyRealEstate-0.0.8/pyRealEstate/Time_Trending.py`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.7/pyRealEstate.egg-info/PKG-INFO` & `pyRealEstate-0.0.8/pyRealEstate.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyRealEstate
-Version: 0.0.7
+Version: 0.0.8
 Summary: package to assist with data analytics in real estate
 Home-page: https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 Author: Joshua Jorgensen
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.4
```

### Comparing `pyRealEstate-0.0.7/pypi_description.md` & `pyRealEstate-0.0.8/pypi_description.md`

 * *Files identical despite different names*

### Comparing `pyRealEstate-0.0.7/setup.cfg` & `pyRealEstate-0.0.8/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyRealEstate
-version = 0.0.7
+version = 0.0.8
 author = Joshua Jorgensen
 description = package to assist with data analytics in real estate
 long_description = file: pypi_description.md
 long_description_content_type = text/markdown
 url = https://github.com/Joshua-Data-Wizard/PyRealEstate/tree/main
 classifiers = 
 	Programming Language :: Python :: 3
```

