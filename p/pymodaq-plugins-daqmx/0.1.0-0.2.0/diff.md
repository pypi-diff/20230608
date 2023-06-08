# Comparing `tmp/pymodaq_plugins_daqmx-0.1.0.tar.gz` & `tmp/pymodaq_plugins_daqmx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymodaq_plugins_daqmx-0.1.0.tar", last modified: Wed Nov 10 20:46:11 2021, max compression
+gzip compressed data, was "pymodaq_plugins_daqmx-0.2.0.tar", last modified: Thu Jun  8 08:40:12 2023, max compression
```

## Comparing `pymodaq_plugins_daqmx-0.1.0.tar` & `pymodaq_plugins_daqmx-0.2.0.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1108 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       44 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1226 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1676 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.128651 pymodaq_plugins_daqmx-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.128651 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/
--rw-r--r--   0 runner    (1001) docker     (121)        5 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/VERSION
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_move_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)      485 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_move_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_move_plugins/daq_move_DAQmx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/
--rw-r--r--   0 runner    (1001) docker     (121)        3 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      625 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx.py
--rw-r--r--   0 runner    (1001) docker     (121)     6628 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmxAI.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      742 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/daq_1Dviewer_DAQmx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_2D/
--rw-r--r--   0 runner    (1001) docker     (121)      488 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_2D/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_ND/
--rw-r--r--   0 runner    (1001) docker     (121)      487 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_ND/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    38679 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daq_NIDAQmx.py
--rw-r--r--   0 runner    (1001) docker     (121)    27875 2021-11-10 20:45:58.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daqmx.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-10 20:46:11.132652 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2122 2021-11-10 20:46:10.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1339 2021-11-10 20:46:11.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-10 20:46:10.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-11-10 20:46:10.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-11-10 20:46:10.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-11-10 20:46:10.000000 pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.470096 pymodaq_plugins_daqmx-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.470096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_move_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_move_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_move_plugins/daq_move_DAQmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmxAI.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5602 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx_PLcounter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/daq_1Dviewer_DAQmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_2D/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_ND/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_ND/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38672 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daq_NIDAQmx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30700 2023-06-08 08:40:00.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daqmx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:40:12.474096 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-06-08 08:40:12.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-08 08:40:12.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:40:12.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 08:40:12.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 08:40:12.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 08:40:12.000000 pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/top_level.txt
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/LICENSE` & `pymodaq_plugins_daqmx-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_daqmx-0.1.0/PKG-INFO` & `pymodaq_plugins_daqmx-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodaq_plugins_daqmx
-Version: 0.1.0
+Version: 0.2.0
 Summary: Hardware plugins for PyMoDAQ using the NiDAQmx framework (pydaqmx wrapper)
-Home-page: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
@@ -26,16 +25,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_daqmx/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx
 
 Plugin devoted to the National Instrument signal acquisition and generation using the NiDAQmx library. Includes an
 actuator plugin for signal generation, a 1D viewer plugin for data acquisition as a function of time and a 0D viewer
 plugin for quick time averaging acquisition
 
 Authors
 =======
@@ -63,9 +62,7 @@
 
 Viewer1D
 ++++++++
 
 * **DAQmx**: Analog acquisition
 
 
-
-
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/README.rst` & `pymodaq_plugins_daqmx-0.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_daqmx/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx
 
 Plugin devoted to the National Instrument signal acquisition and generation using the NiDAQmx library. Includes an
 actuator plugin for signal generation, a 1D viewer plugin for data acquisition as a function of time and a 0D viewer
 plugin for quick time averaging acquisition
 
 Authors
 =======
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/setup.py` & `pymodaq_plugins_daqmx-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_move_plugins/daq_move_DAQmx.py` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_move_plugins/daq_move_DAQmx.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx.py` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from ...hardware.national_instruments.daq_NIDAQmx import DAQ_NIDAQmx_Viewer
+from pymodaq_plugins_daqmx.hardware.national_instruments.daq_NIDAQmx import DAQ_NIDAQmx_Viewer
+from pymodaq.daq_viewer.utility_classes import main
 
 
 class DAQ_0DViewer_DAQmx(DAQ_NIDAQmx_Viewer):
     """
         ==================== ========================
         **Attributes**         **Type**
         *data_grabed_signal*   instance of Signal
@@ -15,7 +16,10 @@
         refresh_hardware
     """
     control_type = "0D"  # could be "0D", "1D"
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, control_type=self.control_type, **kwargs)
 
+
+if __name__ == '__main__':
+    main(__file__, False)
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmxAI.py` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmxAI.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import numpy as np
 from easydict import EasyDict as edict
 from pymodaq.daq_utils.daq_utils import ThreadCommand, getLineInfo, DataFromPlugins, Axis, set_logger, get_module_name
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base, comon_parameters, main
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base, comon_parameters, main
 
 from pymodaq_plugins_daqmx.hardware.national_instruments.daqmx import DAQmx, DAQ_analog_types, DAQ_thermocouples,\
     DAQ_termination, Edge, DAQ_NIDAQ_source, \
     ClockSettings, AIChannel, Counter, AIThermoChannel, AOChannel, TriggerSettings, DOChannel, DIChannel
 
 logger = set_logger(get_module_name(__file__))
 
 class DAQ_0DViewer_DAQmxAI(DAQ_Viewer_base):
     """
     """
     params = comon_parameters+[
-        {'title': 'Display type:', 'name': 'display', 'type': 'list', 'values': ['0D', '1D']},
+        {'title': 'Display type:', 'name': 'display', 'type': 'list', 'limits': ['0D', '1D']},
         {'title': 'Frequency Acq.:', 'name': 'frequency', 'type': 'int', 'value': 1000, 'min': 1},
         {'title': 'Nsamples:', 'name': 'Nsamples', 'type': 'int', 'value': 100, 'default': 100, 'min': 1},
         {'title': 'AI:', 'name': 'ai_channel', 'type': 'list',
-         'values': DAQmx.get_NIDAQ_channels(source_type='Analog_Input'),
+         'limits': DAQmx.get_NIDAQ_channels(source_type='Analog_Input'),
          'value': DAQmx.get_NIDAQ_channels(source_type='Analog_Input')[0]},
         ]
     hardware_averaging = True
     live_mode_available = True
 
     def __init__(self, parent=None, params_state=None):
         super().__init__(parent, params_state)
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/daq_1Dviewer_DAQmx.py` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/daq_1Dviewer_DAQmx.py`

 * *Files identical despite different names*

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daq_NIDAQmx.py` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daq_NIDAQmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,63 @@
 from qtpy import QtWidgets, QtCore
 from qtpy.QtCore import Signal, QThread
 from pymodaq.daq_utils.daq_utils import ThreadCommand, DataFromPlugins, Axis, getLineInfo
 import numpy as np
-from pymodaq.daq_viewer.utility_classes import DAQ_Viewer_base
-from pymodaq.daq_move.utility_classes import DAQ_Move_base
+from pymodaq.control_modules.viewer_utility_classes import DAQ_Viewer_base
+from pymodaq.control_modules.move_utility_classes import DAQ_Move_base
 from easydict import EasyDict as edict
 from abc import ABC, abstractmethod
 
-from pymodaq.daq_viewer.utility_classes import comon_parameters as viewer_params
+from pymodaq.control_modules.viewer_utility_classes import comon_parameters as viewer_params
 from pymodaq.daq_move.utility_classes import comon_parameters as actuator_params
 
 from pyqtgraph.parametertree import Parameter, ParameterTree, registerParameterType
 import pyqtgraph.parametertree.parameterTypes as pTypes
 import pymodaq.daq_utils.parameter.pymodaq_ptypes as pymodaq_ptypes
 
 from .daqmx import DAQmx, DAQ_analog_types, DAQ_thermocouples, DAQ_termination, Edge, DAQ_NIDAQ_source, \
     ClockSettings, AIChannel, Counter, AIThermoChannel, AOChannel, TriggerSettings, DOChannel, DIChannel
 
 
-class ScalableGroupAI(pymodaq_ptypes.GroupParameterCustom):
+class ScalableGroupAI(pTypes.GroupParameter):
     """
         |
 
         ================ =============
         **Attributes**    **Type**
         *opts*            dictionnary
         ================ =============
 
         See Also
         --------
         hardware.DAQ_Move_Stage_type
     """
 
-    params = [{'title': 'AI type:', 'name': 'ai_type', 'type': 'list', 'values': DAQ_analog_types.names()},
+    params = [{'title': 'AI type:', 'name': 'ai_type', 'type': 'list', 'limits': DAQ_analog_types.names()},
               {'title': 'Voltages:', 'name': 'voltage_settings', 'type': 'group', 'children': [
                   {'title': 'Voltage Min:', 'name': 'volt_min', 'type': 'list', 'value': -10.},
                   {'title': 'Voltage Max:', 'name': 'volt_max', 'type': 'list', 'value': 10.},
               ]},
               {'title': 'Current:', 'name': 'current_settings', 'type': 'group', 'visible': False, 'children': [
                   {'title': 'Current Min:', 'name': 'curr_min', 'type': 'float', 'value': -1, 'suffix': 'A'},
                   {'title': 'Current Max:', 'name': 'curr_max', 'type': 'float', 'value': 1, 'suffix': 'A'},
               ]},
               {'title': 'Thermocouple:', 'name': 'thermoc_settings', 'type': 'group', 'visible': False, 'children': [
-                  {'title': 'Thc. type:', 'name': 'thermoc_type', 'type': 'list', 'values': DAQ_thermocouples.names(),
+                  {'title': 'Thc. type:', 'name': 'thermoc_type', 'type': 'list', 'limits': DAQ_thermocouples.names(),
                    'value': 'K'},
                   {'title': 'Temp. Min (°C):', 'name': 'T_min', 'type': 'float', 'value': 0, 'suffix': '°C'},
                   {'title': 'Temp. Max (°C):', 'name': 'T_max', 'type': 'float', 'value': 50, 'suffix': '°C'},
               ]},
-              {'title': 'Termination:', 'name': 'termination', 'type': 'list', 'values': DAQ_termination.names()},
+              {'title': 'Termination:', 'name': 'termination', 'type': 'list', 'limits': DAQ_termination.names()},
               ]
 
     def __init__(self, **opts):
         opts['type'] = 'groupai'
         opts['addText'] = "Add"
-        opts['addList'] = opts['values']
+        opts['addList'] = opts['limits']
         pTypes.GroupParameter.__init__(self, **opts)
 
     def addNew(self, typ):
         """
             Add a child.
 
             =============== ===========
@@ -74,43 +74,43 @@
         child = {'title': typ, 'name': 'ai{:02.0f}'.format(newindex), 'type': 'group', 'children': self.params,
                  'removable': True, 'renamable': False}
 
         self.addChild(child)
 registerParameterType('groupai', ScalableGroupAI, override=True)
 
 
-class ScalableGroupAO(pymodaq_ptypes.GroupParameterCustom):
+class ScalableGroupAO(pTypes.GroupParameter):
     """
         |
 
         ================ =============
         **Attributes**    **Type**
         *opts*            dictionnary
         ================ =============
 
         See Also
         --------
         hardware.DAQ_Move_Stage_type
     """
 
-    params = [{'title': 'AO type:', 'name': 'ao_type', 'type': 'list', 'values': DAQ_analog_types.names()[0:2]},
+    params = [{'title': 'AO type:', 'name': 'ao_type', 'type': 'list', 'limits': DAQ_analog_types.names()[0:2]},
               {'title': 'Voltages:', 'name': 'voltage_settings', 'type': 'group', 'children': [
                   {'title': 'Voltage Min:', 'name': 'volt_min', 'type': 'list', 'value': -10., },
                   {'title': 'Voltage Max:', 'name': 'volt_max', 'type': 'list', 'value': 10., },
               ]},
               {'title': 'Current:', 'name': 'current_settings', 'type': 'group', 'visible': False, 'children': [
                   {'title': 'Current Min:', 'name': 'curr_min', 'type': 'float', 'value': -1, 'suffix': 'A'},
                   {'title': 'Current Max:', 'name': 'curr_max', 'type': 'float', 'value': 1, 'suffix': 'A'},
               ]},
               ]
 
     def __init__(self, **opts):
         opts['type'] = 'groupao'
         opts['addText'] = "Add"
-        opts['addList'] = opts['values']
+        opts['addList'] = opts['limits']
         pTypes.GroupParameter.__init__(self, **opts)
 
     def addNew(self, typ):
         """
             Add a child.
 
             =============== ===========
@@ -127,34 +127,34 @@
         child = {'title': typ, 'name': 'ao{:02.0f}'.format(newindex), 'type': 'group', 'children': self.params,
                  'removable': True, 'renamable': False}
 
         self.addChild(child)
 registerParameterType('groupao', ScalableGroupAO, override=True)
 
 
-class ScalableGroupCounter(pymodaq_ptypes.GroupParameterCustom):
+class ScalableGroupCounter(pTypes.GroupParameter):
     """
         |
 
         ================ =============
         **Attributes**    **Type**
         *opts*            dictionnary
         ================ =============
 
         See Also
         --------
         hardware.DAQ_Move_Stage_type
     """
 
-    params = [{'title': 'Edge type:', 'name': 'edge', 'type': 'list', 'values': Edge.names()}, ]
+    params = [{'title': 'Edge type:', 'name': 'edge', 'type': 'list', 'limits': Edge.names()}, ]
 
     def __init__(self, **opts):
         opts['type'] = 'groupcounter'
         opts['addText'] = "Add"
-        opts['addList'] = opts['values']
+        opts['addList'] = opts['limits']
         pTypes.GroupParameter.__init__(self, **opts)
 
     def addNew(self, typ):
         """
             Add a child.
 
             =============== ===========
@@ -171,24 +171,24 @@
         child = {'title': typ, 'name': 'counter{:02.0f}'.format(newindex), 'type': 'group', 'children': self.params,
                  'removable': True, 'renamable': False}
 
         self.addChild(child)
 registerParameterType('groupcounter', ScalableGroupCounter, override=True)
 
 
-class ScalableGroupDI(pymodaq_ptypes.GroupParameterCustom):
+class ScalableGroupDI(pTypes.GroupParameter):
     """
     """
 
     params = []
 
     def __init__(self, **opts):
         opts['type'] = 'groupdi'
         opts['addText'] = "Add"
-        opts['addList'] = opts['values']
+        opts['addList'] = opts['limits']
         pTypes.GroupParameter.__init__(self, **opts)
 
     def addNew(self, typ):
         """
             Add a child.
 
             =============== ===========
@@ -203,24 +203,25 @@
             newindex = len(childnames)
 
         child = {'title': typ, 'name': 'di{:02.0f}'.format(newindex), 'type': 'group', 'children': self.params,
                  'removable': True, 'renamable': False}
         self.addChild(child)
 registerParameterType('groupdi', ScalableGroupDI, override=True)
 
-class ScalableGroupDO(pymodaq_ptypes.GroupParameterCustom):
+
+class ScalableGroupDO(pTypes.GroupParameter):
     """
     """
 
     params = []
 
     def __init__(self, **opts):
         opts['type'] = 'groupdo'
         opts['addText'] = "Add"
-        opts['addList'] = opts['values']
+        opts['addList'] = opts['limits']
         pTypes.GroupParameter.__init__(self, **opts)
 
     def addNew(self, typ):
         """
             Add a child.
 
             =============== ===========
@@ -240,63 +241,64 @@
 registerParameterType('groupdo', ScalableGroupDO, override=True)
 
 
 class DAQ_NIDAQmx_base(DAQmx):
     data_grabed_signal = Signal(list)
 
     params =[{'title': 'Refresh hardware:', 'name': 'refresh_hardware', 'type': 'bool', 'value': False},
-            {'title': 'Signal type:', 'name': 'NIDAQ_type', 'type': 'list', 'values': DAQ_NIDAQ_source.names()},
+            {'title': 'Signal type:', 'name': 'NIDAQ_type', 'type': 'list', 'limits': DAQ_NIDAQ_source.names()},
              {'title': 'AO Settings:', 'name': 'ao_settings', 'type': 'group', 'children': [
-                 {'title': 'Waveform:', 'name': 'waveform', 'type': 'list', 'value': 'DC', 'values': ['DC', 'Sinus', 'Ramp']},
+                 {'title': 'Waveform:', 'name': 'waveform', 'type': 'list', 'value': 'DC', 'limits': ['DC', 'Sinus', 'Ramp']},
 
                  {'title': 'Controlled param:', 'name': 'cont_param', 'type': 'list', 'value': 'offset',
-                  'values': ['offset', 'amplitude', 'frequency']},
+                  'limits': ['offset', 'amplitude', 'frequency']},
                  {'title': 'Waveform Settings:', 'name': 'waveform_settings', 'type': 'group', 'visible': False, 'children': [
                      {'title': 'Offset:', 'name': 'offset', 'type': 'float', 'value': 0., },
                      {'title': 'Amplitude:', 'name': 'amplitude', 'type': 'float', 'value': 1., },
                      {'title': 'Frequency:', 'name': 'frequency', 'type': 'float', 'value': 10., },
                     ]},
              ]},
             {'title': 'Clock Settings:', 'name': 'clock_settings', 'type': 'group', 'children': [
                 {'title': 'Nsamples:', 'name': 'Nsamples', 'type': 'int', 'value': 1000, 'default': 1000, 'min': 1},
                 {'title': 'Frequency:', 'name': 'frequency', 'type': 'float', 'value': 1000., 'default': 1000.,
                  'min': 0., 'suffix': 'Hz'},
                 {'title': 'Repetition?:', 'name': 'repetition', 'type': 'bool', 'value': False, },
             ]
             },
             {'title': 'AI Channels:', 'name': 'ai_channels', 'type': 'groupai',
-                  'values': DAQmx.get_NIDAQ_channels(source_type='Analog_Input')},
+                  'limits': DAQmx.get_NIDAQ_channels(source_type='Analog_Input')},
             {'title': 'AO Channels:', 'name': 'ao_channels', 'type': 'groupao',
-                 'values': DAQmx.get_NIDAQ_channels(source_type='Analog_Output')},
+                 'limits': DAQmx.get_NIDAQ_channels(source_type='Analog_Output')},
             {'title': 'DO Channels:', 'name': 'do_channels', 'type': 'groupdo',
-                'values': DAQmx.get_NIDAQ_channels(source_type='Digital_Output')},
+                'limits': DAQmx.get_NIDAQ_channels(source_type='Digital_Output')},
              {'title': 'DI Channels:', 'name': 'di_channels', 'type': 'groupdi',
-              'values': DAQmx.get_NIDAQ_channels(source_type='Digital_Input')},
+              'limits': DAQmx.get_NIDAQ_channels(source_type='Digital_Input')},
             {'title': 'Counter Settings:', 'name': 'counter_settings', 'type': 'group', 'visible': True, 'children': [
                 {'title': 'Counting time (ms):', 'name': 'counting_time', 'type': 'float', 'value': 100.,
                 'default': 100., 'min': 0.},
                 {'title': 'Counting Channels:', 'name': 'counter_channels', 'type': 'groupcounter',
-                'values': DAQmx.get_NIDAQ_channels(source_type='Counter')},
+                'limits': DAQmx.get_NIDAQ_channels(source_type='Counter')},
             ]},
             {'title': 'Trigger Settings:', 'name': 'trigger_settings', 'type': 'group', 'visible': True, 'children': [
                 {'title': 'Enable?:', 'name': 'enable', 'type': 'bool', 'value': False, },
                 {'title': 'Trigger Source:', 'name': 'trigger_channel', 'type': 'list',
-                 'values': DAQmx.getTriggeringSources()},
-                {'title': 'Edge type:', 'name': 'edge', 'type': 'list', 'values': Edge.names(), 'visible': False},
+                 'limits': DAQmx.getTriggeringSources()},
+                {'title': 'Edge type:', 'name': 'edge', 'type': 'list', 'limits': Edge.names(), 'visible': False},
                 {'title': 'Level:', 'name': 'level', 'type': 'float', 'value': 1., 'visible': False}
                 ]}
             ]
 
     def __init__(self):
         super().__init__()
 
         self.timer = None
         self.channels = None
         self.clock_settings = None
         self.trigger_settings = None
+        self.live = False
         self.refresh_hardware()
 
 
     def commit_settings(self, param):
         """
             Activate the parameters changes in the hardware.
 
@@ -641,16 +643,16 @@
               # elements to be added here as dicts in order to control your custom stage
               ############
               {'title': 'MultiAxes:', 'name': 'multiaxes', 'type': 'group', 'visible': is_multiaxes,
                'children': [
                    {'title': 'is Multiaxes:', 'name': 'ismultiaxes', 'type': 'bool', 'value': is_multiaxes,
                     'default': False},
                    {'title': 'Status:', 'name': 'multi_status', 'type': 'list', 'value': 'Master',
-                    'values': ['Master', 'Slave']},
-                   {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'values': stage_names},
+                    'limits': ['Master', 'Slave']},
+                   {'title': 'Axis:', 'name': 'axis', 'type': 'list', 'limits': stage_names},
 
                ]}] + actuator_params
 
     def __init__(self, parent=None, params_state=None, control_type="Actuator"):
         DAQ_Move_base.__init__(self, parent, params_state)  # defines settings attribute and various other methods
         DAQ_NIDAQmx_base.__init__(self)
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daqmx.py` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx/hardware/national_instruments/daqmx.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import ctypes
 from enum import IntEnum
 import numpy as np
 from pymodaq.daq_utils.daq_utils import set_logger, get_module_name
 
 logger = set_logger(get_module_name(__file__))
 
+
 class DAQ_NIDAQ_source(IntEnum):
     """
         Enum class of NIDAQ_source
 
         =============== ==========
         **Attributes**   **Type**
         *Analog_Input*   int
@@ -131,14 +132,15 @@
 class ChangeDetectionSettings(ClockSettingsBase):
     def __init__(self, Nsamples=1000, rising_channel='', falling_channel='',
                  repetition=False):
         super().__init__(Nsamples, repetition)
         self.rising_channel = rising_channel
         self.falling_channel = falling_channel
 
+
 class TriggerSettings:
     def __init__(self, trig_source='', enable=False, edge=Edge.names()[0], level=0.1):
         assert edge in Edge.names()
         self.trig_source = trig_source
         self.enable = enable
         self.edge = edge
         self.level = level
@@ -165,14 +167,15 @@
         max: (float) maximum value for the configured input channel
         """
         super().__init__(**kwargs)
         self.value_min = value_min
         self.value_max = value_max
         self.analog_type = analog_type
 
+
 class AIChannel(AChannel):
     def __init__(self, termination=DAQ_termination.names()[0], **kwargs):
         super().__init__(**kwargs)
         assert termination in DAQ_termination.names()
         self.termination = termination
 
 
@@ -186,31 +189,49 @@
 class AOChannel(AChannel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
 class Counter(Channel):
     def __init__(self, edge=Edge.names()[0], **kwargs):
-        assert edge in Edge.names()
+        assert edge in Edge.names()    
         super().__init__(**kwargs)
         self.edge = edge
+        self.counter_type = "Edge Counter"
+
+        
+class ClockCounter(Counter):
+    def __init__(self, clock_frequency, **kwargs):
+        super().__init__(**kwargs)
+        self.clock_frequency = clock_frequency
+        self.counter_type = "Clock Output"
+
+        
+class SemiPeriodCounter(Counter):
+    def __init__(self, value_max, **kwargs):
+        super().__init__(**kwargs)
+        self.value_max = value_max
+        self.counter_type = "SemiPeriod Input"
 
+        
 class DigitalChannel(Channel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
 
 class DOChannel(DigitalChannel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
+
 class DIChannel(DigitalChannel):
     def __init__(self, **kwargs):
         super().__init__(**kwargs)
 
+
 def try_string_buffer(fun, *args):
     """
     generic function to read string from a PyDAQmx function making sure the chosen buffer is large enough
     Parameters
     ----------
     fun: (PyDAQmx function pointer) e.g. PyDAQmx.DAQmxGetSysDevNames
     kwargs
@@ -235,14 +256,15 @@
                     buff_size = 2 * buff_size
                 else:
                     raise e
             else:
                 raise e
     return buff.value.decode()
 
+
 class DAQmx:
 
     def __init__(self):
         super().__init__()
         self.devices = []
         self.channels = []
         self._device = None
@@ -398,15 +420,15 @@
             self._task = PyDAQmx.Task()
 
 
             ## create all channels one task for one type of channels
             for channel in channels:
                 if channel.source == 'Analog_Input': #analog input
                     if channel.analog_type == "Voltage":
-                        err_code = self._task.CreateAIVoltageChan(channel.name, "",
+                        err_code = self._task.CreateAIVoltageChan(channel.name, "analog voltage task",
                                      DAQ_termination[channel.termination].value,
                                      channel.value_min,
                                      channel.value_max,
                                      PyDAQmx.DAQmx_Val_Volts, None)
 
                     elif channel.analog_type == "Current":
                         err_code = self._task.CreateAICurrentChan(channel.name, "",
@@ -421,17 +443,39 @@
                                                                   channel.value_min,
                                                                   channel.value_max,
                                                                   PyDAQmx.DAQmx_Val_DegC,
                                                                   DAQ_termination[channel.thermo_type].value,
                                                                   PyDAQmx.DAQmx_Val_BuiltIn, 0., "")
 
                 elif channel.source == 'Counter': #counter
-                    err_code = self._task.CreateCICountEdgesChan(channel.name, "",
-                                                               Edge[channel.edge].value, 0,
-                                                               PyDAQmx.DAQmx_Val_CountUp)
+                    if channel.counter_type == "Edge Counter":
+                        err_code = self._task.CreateCICountEdgesChan(channel.name, "",
+                                                                     Edge[channel.edge].value, 0,
+                                                                     PyDAQmx.DAQmx_Val_CountUp)
+                    elif channel.counter_type == "Clock Output":
+                        err_code = self._task.CreateCOPulseChanFreq(channel.name, "clock task",
+                                                                    # units, Hertz in our case
+                                                                    PyDAQmx.DAQmx_Val_Hz,
+                                                                    # idle state
+                                                                    PyDAQmx.DAQmx_Val_Low,
+                                                                    # initial delay
+                                                                    0,
+                                                                    # pulse frequency
+                                                                    channel.clock_frequency,
+                                                                    # duty cycle of pulses, 0.5 such that
+                                                                    # high and low duration are both
+                                                                    # equal to count_interval
+                                                                    0.5)
+                    elif channel.counter_type == "SemiPeriod Input":
+                        err_code = self._task.CreateCISemiPeriodChan(channel.name, "counter task",
+                                                                     0, # expected min
+                                                                     channel.value_max, # expected max
+                                                                     PyDAQmx.DAQmx_Val_Ticks, "")
+                        
+                    
                     if not not err_code:
                         status = self.DAQmxGetErrorString(err_code)
                         raise IOError(status)
 
                 elif channel.source == 'Analog_Output':  # Analog_Output
                     if channel.analog_type == "Voltage":
                         err_code = self._task.CreateAOVoltageChan(channel.name, "",
@@ -522,22 +566,26 @@
             #         if not not err_code:
             #             status = self.DAQmxGetErrorString(err_code)
             #             raise IOError(status)
             #
             # else:
             #     pass
 
-            ##configure the triggering
+            ##configure the triggering, except for counters
             if not trigger_settings.enable:
-                err = self._task.DisableStartTrig()
-                if err != 0:
-                    raise IOError(self.DAQmxGetErrorString(err))
+                if channel.source == 'Counter':
+                    pass
+                else:
+                    err = self._task.DisableStartTrig()
+                    if err != 0:
+                        raise IOError(self.DAQmxGetErrorString(err))
             else:
                 if 'PF' in trigger_settings.trig_source:
-                    self._task.CfgDigEdgeStartTrig(trigger_settings.trig_source, Edge[trigger_settings.edge].value)
+                    self._task.CfgDigEdgeStartTrig(trigger_settings.trig_source,
+                                                   Edge[trigger_settings.edge].value)
                 elif 'ai' in trigger_settings.trig_source:
                     self._task.CfgAnlgEdgeStartTrig(trigger_settings.trig_source,
                                                     Edge[trigger_settings.edge].value,
                                                     PyDAQmx.c_double(trigger_settings.level))
                 else:
                     raise IOError('Unsupported Trigger source')
 
@@ -623,21 +671,27 @@
         self._task.ReadAnalogF64(N, timeout, PyDAQmx.DAQmx_Val_GroupByChannel, data, len(data),
                                  PyDAQmx.byref(read), None)
         if read.value == N:
             return data
         else:
             raise IOError(f'Insufficient number of samples have been read:{read.value}/{N}')
 
-    def readCounter(self, Nchannels, counting_time=10.):
+    def readCounter(self, Nchannels, counting_time=10., read_function="Ex"):
 
         data_counter = np.zeros(Nchannels, dtype='uint32')
         read = PyDAQmx.int32()
-        self._task.ReadCounterU32Ex(PyDAQmx.DAQmx_Val_Auto, 2*counting_time, PyDAQmx.DAQmx_Val_GroupByChannel,
-                                    data_counter,
-                                    Nchannels, PyDAQmx.byref(read), None)
+        if read_function == "Ex":
+            self._task.ReadCounterU32Ex(PyDAQmx.DAQmx_Val_Auto, 2*counting_time,
+                                        PyDAQmx.DAQmx_Val_GroupByChannel,
+                                        data_counter,
+                                        Nchannels, PyDAQmx.byref(read), None)
+        else:
+            self._task.ReadCounterU32(PyDAQmx.DAQmx_Val_Auto, 2*counting_time,
+                                        data_counter, Nchannels, PyDAQmx.byref(read), None)
+            
         self._task.StopTask()
 
         if read.value == Nchannels:
             return data_counter
         else:
             raise IOError(f'Insufficient number of samples have been read:{read}/{Nchannels}')
 
@@ -659,24 +713,26 @@
         values.astype(np.uint8)
         written = PyDAQmx.int32()
         self._task.WriteDigitalLines(Nchannels, autostart, 0, PyDAQmx.DAQmx_Val_GroupByChannel,
                                       values, PyDAQmx.byref(written), None)
         if written.value != Nchannels:
             raise IOError(f'Insufficient number of samples have been written:{written}/{Nchannels}')
 
-    def getAIVoltageRange(self, device='Dev1'):
+    @classmethod
+    def getAIVoltageRange(cls, device='Dev1'):
         buff_size = 100
         ranges = ctypes.pointer((buff_size*ctypes.c_double)())
         ret = PyDAQmx.DAQmxGetDevAIVoltageRngs(device, ranges[0], buff_size)
         if ret == 0:
             return [tuple(ranges.contents[2*ind:2*(ind+1)]) for ind in range(int(buff_size/2-2))
                     if np.abs(ranges.contents[2*ind]) > 1e-12]
         return [(-10., 10.)]
 
-    def getAOVoltageRange(self, device='Dev1'):
+    @classmethod
+    def getAOVoltageRange(cls, device='Dev1'):
         buff_size = 100
         ranges = ctypes.pointer((buff_size*ctypes.c_double)())
         ret = PyDAQmx.DAQmxGetDevAOVoltageRngs(device, ranges[0], buff_size)
         if ret == 0:
             return [tuple(ranges.contents[2*ind:2*(ind+1)]) for ind in range(int(buff_size/2-2))
                     if np.abs(ranges.contents[2*ind]) > 1e-12]
         return [(-10., 10.)]
@@ -726,8 +782,8 @@
             update_NIDAQ_devices, update_NIDAQ_channels
         """
         devices = self.update_NIDAQ_devices()
         self.update_NIDAQ_channels(devices)
 
 if __name__ == '__main__':
     print(DAQmx.get_NIDAQ_channels())
-    pass
+    pass
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/PKG-INFO` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: pymodaq-plugins-daqmx
-Version: 0.1.0
+Version: 0.2.0
 Summary: Hardware plugins for PyMoDAQ using the NiDAQmx framework (pydaqmx wrapper)
-Home-page: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx
+Home-page: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx
 Author: Sébastien Weber
 Author-email: sebastien.weber@cemes.fr
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Human Machine Interfaces
 Classifier: Topic :: Scientific/Engineering :: Visualization
 Classifier: License :: OSI Approved :: MIT License
@@ -26,16 +25,16 @@
    :target: https://pypi.org/project/pymodaq_plugins_daqmx/
    :alt: Latest Version
 
 .. image:: https://readthedocs.org/projects/pymodaq/badge/?version=latest
    :target: https://pymodaq.readthedocs.io/en/stable/?badge=latest
    :alt: Documentation Status
 
-.. image:: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx/workflows/Upload%20Python%20Package/badge.svg
-    :target: https://github.com/CEMES-CNRS/pymodaq_plugins_daqmx
+.. image:: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx/workflows/Upload%20Python%20Package/badge.svg
+    :target: https://github.com/PyMoDAQ/pymodaq_plugins_daqmx
 
 Plugin devoted to the National Instrument signal acquisition and generation using the NiDAQmx library. Includes an
 actuator plugin for signal generation, a 1D viewer plugin for data acquisition as a function of time and a 0D viewer
 plugin for quick time averaging acquisition
 
 Authors
 =======
@@ -63,9 +62,7 @@
 
 Viewer1D
 ++++++++
 
 * **DAQmx**: Analog acquisition
 
 
-
-
```

### Comparing `pymodaq_plugins_daqmx-0.1.0/src/pymodaq_plugins_daqmx.egg-info/SOURCES.txt` & `pymodaq_plugins_daqmx-0.2.0/src/pymodaq_plugins_daqmx.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 src/pymodaq_plugins_daqmx.egg-info/top_level.txt
 src/pymodaq_plugins_daqmx/daq_move_plugins/__init__.py
 src/pymodaq_plugins_daqmx/daq_move_plugins/daq_move_DAQmx.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/__init__.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/__init__.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmxAI.py
+src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_0D/daq_0Dviewer_DAQmx_PLcounter.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/__init__.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_1D/daq_1Dviewer_DAQmx.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_2D/__init__.py
 src/pymodaq_plugins_daqmx/daq_viewer_plugins/plugins_ND/__init__.py
 src/pymodaq_plugins_daqmx/hardware/__init__.py
 src/pymodaq_plugins_daqmx/hardware/national_instruments/__init__.py
 src/pymodaq_plugins_daqmx/hardware/national_instruments/daq_NIDAQmx.py
```

