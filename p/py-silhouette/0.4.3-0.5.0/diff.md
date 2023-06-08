# Comparing `tmp/py_silhouette-0.4.3.tar.gz` & `tmp/py_silhouette-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_silhouette-0.4.3.tar", last modified: Wed Apr 12 06:33:24 2023, max compression
+gzip compressed data, was "py_silhouette-0.5.0.tar", last modified: Thu Jun  8 05:41:04 2023, max compression
```

## Comparing `py_silhouette-0.4.3.tar` & `py_silhouette-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.752268 py_silhouette-0.4.3/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2670 2019-01-20 19:51:33.000000 py_silhouette-0.4.3/README.md
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/py_silhouette/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      202 2019-01-20 19:37:22.000000 py_silhouette-0.4.3/py_silhouette/__init__.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)    24444 2023-04-12 06:27:29.000000 py_silhouette-0.4.3/py_silhouette/device.py
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       23 2023-04-12 06:31:20.000000 py_silhouette-0.4.3/py_silhouette/version.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/py_silhouette.egg-info/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/PKG-INFO
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)      296 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/SOURCES.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/dependency_links.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/requires.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       14 2023-04-12 06:33:24.000000 py_silhouette-0.4.3/py_silhouette.egg-info/top_level.txt
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2023-04-12 06:33:24.752268 py_silhouette-0.4.3/setup.cfg
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1086 2022-08-26 13:23:43.000000 py_silhouette-0.4.3/setup.py
-drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-04-12 06:33:24.748935 py_silhouette-0.4.3/test/
--rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4367 2020-09-01 13:44:40.000000 py_silhouette-0.4.3/test/test_sheet.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     2670 2019-01-20 19:51:33.000000 py_silhouette-0.5.0/README.md
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.413735 py_silhouette-0.5.0/py_silhouette/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      202 2019-01-20 19:37:22.000000 py_silhouette-0.5.0/py_silhouette/__init__.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)    25201 2023-06-08 05:36:01.000000 py_silhouette-0.5.0/py_silhouette/device.py
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       23 2023-06-08 05:39:41.000000 py_silhouette-0.5.0/py_silhouette/version.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.413735 py_silhouette-0.5.0/py_silhouette.egg-info/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      790 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/PKG-INFO
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)      296 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/SOURCES.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)        1 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/dependency_links.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       27 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/requires.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       14 2023-06-08 05:41:04.000000 py_silhouette-0.5.0/py_silhouette.egg-info/top_level.txt
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)       38 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/setup.cfg
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     1086 2022-08-26 13:23:43.000000 py_silhouette-0.5.0/setup.py
+drwxr-xr-x   0 jonathan  (1000) jonathan  (1000)        0 2023-06-08 05:41:04.417069 py_silhouette-0.5.0/test/
+-rw-r--r--   0 jonathan  (1000) jonathan  (1000)     4367 2020-09-01 13:44:40.000000 py_silhouette-0.5.0/test/test_sheet.py
```

### Comparing `py_silhouette-0.4.3/PKG-INFO` & `py_silhouette-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py_silhouette
-Version: 0.4.3
+Version: 0.5.0
 Summary: A USB driver and Python API to control the Silhouette Portrait plotter.
 Home-page: https://github.com/mossblaser/py_silhouette
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: plotter cutter driver usb silhouette
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `py_silhouette-0.4.3/README.md` & `py_silhouette-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `py_silhouette-0.4.3/py_silhouette/device.py` & `py_silhouette-0.5.0/py_silhouette/device.py`

 * *Files 4% similar despite different names*

```diff
@@ -174,50 +174,67 @@
         area_width_min=inch2mm(3.0),
         area_width_max=inch2mm(8.5),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=None,
         tool_depth_max=None,
     ),
-    # Warning: values for entries below taken from
-    # https://github.com/fablabnbg/inkscape-silhouette and have not been
-    # tested or validated in any way!
+    # Warning: Taken from https://github.com/fablabnbg/inkscape-silhouette and
+    # have not been tested or validated in any way!
     DeviceParameters(
         "Silhouette Portrait2",
         usb_vendor_id=0x0B4D,
         usb_product_id=0x1132,
         area_width_min=inch2mm(3.0),
         area_width_max=inch2mm(8.0),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=0,
         tool_depth_max=10,
     ),
+    # Contributed by GitHub user @gtebbutt (in mossblaser/plottie#9)
+    DeviceParameters(
+        "Silhouette Portrait3",
+        usb_vendor_id=0x0B4D,
+        usb_product_id=0x113A,
+        area_width_min=inch2mm(3.0),
+        area_width_max=inch2mm(8.0),
+        area_height_min=inch2mm(3.0),
+        area_height_max=inch2mm(40.0),
+        tool_depth_min=0,
+        tool_depth_max=10,
+    ),
+    # Warning: Taken from https://github.com/fablabnbg/inkscape-silhouette and
+    # have not been tested or validated in any way!
     DeviceParameters(
         "Silhouette Cameo",
         usb_vendor_id=0x0B4D,
         usb_product_id=0x1121,
         area_width_min=inch2mm(3.0),
         area_width_max=inch2mm(12.0),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=None,
         tool_depth_max=None,
     ),
+    # Warning: Taken from https://github.com/fablabnbg/inkscape-silhouette and
+    # have not been tested or validated in any way!
     DeviceParameters(
         "Silhouette Cameo2",
         usb_vendor_id=0x0B4D,
         usb_product_id=0x112B,
         area_width_min=inch2mm(3.0),
         area_width_max=inch2mm(12.0),
         area_height_min=inch2mm(3.0),
         area_height_max=inch2mm(40.0),
         tool_depth_min=None,
         tool_depth_max=None,
     ),
+    # Warning: Taken from https://github.com/fablabnbg/inkscape-silhouette and
+    # have not been tested or validated in any way!
     DeviceParameters(
         "Silhouette Cameo3",
         usb_vendor_id=0x0B4D,
         usb_product_id=0x112F,
         area_width_min=inch2mm(3.0),
         area_width_max=inch2mm(12.0),
         area_height_min=inch2mm(3.0),
```

### Comparing `py_silhouette-0.4.3/py_silhouette.egg-info/PKG-INFO` & `py_silhouette-0.5.0/py_silhouette.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-silhouette
-Version: 0.4.3
+Version: 0.5.0
 Summary: A USB driver and Python API to control the Silhouette Portrait plotter.
 Home-page: https://github.com/mossblaser/py_silhouette
 Author: Jonathan Heathcote
 License: LGPLv3
 Keywords: plotter cutter driver usb silhouette
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `py_silhouette-0.4.3/setup.py` & `py_silhouette-0.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `py_silhouette-0.4.3/test/test_sheet.py` & `py_silhouette-0.5.0/test/test_sheet.py`

 * *Files identical despite different names*

