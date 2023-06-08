# Comparing `tmp/hazelbean-1.4.4.tar.gz` & `tmp/hazelbean-1.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hazelbean-1.4.4.tar", last modified: Wed Jun  7 15:47:03 2023, max compression
+gzip compressed data, was "hazelbean-1.4.5.tar", last modified: Thu Jun  8 15:02:20 2023, max compression
```

## Comparing `hazelbean-1.4.4.tar` & `hazelbean-1.4.5.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 15:47:03.927000 hazelbean-1.4.4/
--rw-rw-rw-   0        0        0    14763 2023-06-07 15:46:58.000000 hazelbean-1.4.4/LICENSE
--rw-rw-rw-   0        0        0      145 2023-06-07 15:46:58.000000 hazelbean-1.4.4/MANIFEST.in
--rw-rw-rw-   0        0        0      443 2023-06-07 15:47:03.878000 hazelbean-1.4.4/PKG-INFO
--rw-rw-rw-   0        0        0     4863 2023-06-07 15:46:58.000000 hazelbean-1.4.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 15:47:02.028000 hazelbean-1.4.4/hazelbean/
--rw-rw-rw-   0        0        0     8196 2022-09-28 15:14:40.000000 hazelbean-1.4.4/hazelbean/__init__.py
--rw-rw-rw-   0        0        0    15645 2022-09-28 14:32:01.000000 hazelbean-1.4.4/hazelbean/arrayframe.py
--rw-rw-rw-   0        0        0     6865 2022-05-09 18:31:33.000000 hazelbean-1.4.4/hazelbean/arrayframe_functions.py
--rw-rw-rw-   0        0        0     5787 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/arrayframe_numpy_functions.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:47:03.054000 hazelbean-1.4.4/hazelbean/calculation_core/
--rw-rw-rw-   0        0        0     2523 2022-09-27 18:48:13.000000 hazelbean-1.4.4/hazelbean/calculation_core/__init__.py
--rw-rw-rw-   0        0        0   364367 2023-01-30 15:25:17.000000 hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.c
--rw-rw-rw-   0        0        0    59392 2023-01-30 15:25:21.000000 hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0   370413 2023-06-06 15:16:35.000000 hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.cpp
--rw-rw-rw-   0        0        0     5843 2023-01-30 15:25:06.000000 hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.pyx
--rw-rw-rw-   0        0        0      746 2023-06-01 20:11:21.000000 hazelbean-1.4.4/hazelbean/calculation_core/compile_cython_functions.py
--rw-rw-rw-   0        0        0  3445406 2023-06-01 20:11:20.000000 hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.c
--rw-rw-rw-   0        0        0   567808 2023-06-02 01:58:12.000000 hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  3452047 2023-06-06 15:16:35.000000 hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.cpp
--rw-rw-rw-   0        0        0   150011 2023-06-01 20:11:20.000000 hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.pyx
--rw-rw-rw-   0        0        0     4830 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/cat_ears.py
--rw-rw-rw-   0        0        0     7177 2023-06-01 20:54:47.000000 hazelbean-1.4.4/hazelbean/cloud_utils.py
--rw-rw-rw-   0        0        0    19206 2022-09-23 17:47:57.000000 hazelbean-1.4.4/hazelbean/config.py
--rw-rw-rw-   0        0        0     3471 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/conventions.py
--rw-rw-rw-   0        0        0     8594 2023-06-05 19:37:33.000000 hazelbean-1.4.4/hazelbean/core.py
--rw-rw-rw-   0        0        0    21132 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/data_structures.py
--rw-rw-rw-   0        0        0    30780 2023-02-16 18:33:50.000000 hazelbean-1.4.4/hazelbean/file_io.py
--rw-rw-rw-   0        0        0   115964 2022-09-23 21:13:00.000000 hazelbean-1.4.4/hazelbean/geoprocessing.py
--rw-rw-rw-   0        0        0    74113 2023-03-08 17:18:14.000000 hazelbean-1.4.4/hazelbean/geoprocessing_extension.py
--rw-rw-rw-   0        0        0    44554 2022-09-22 15:56:20.000000 hazelbean-1.4.4/hazelbean/globals.py
--rw-rw-rw-   0        0        0    43887 2023-06-01 20:11:20.000000 hazelbean-1.4.4/hazelbean/netcdf.py
--rw-rw-rw-   0        0        0    75326 2023-06-01 20:11:20.000000 hazelbean-1.4.4/hazelbean/os_utils.py
--rw-rw-rw-   0        0        0    20647 2023-01-28 21:04:04.000000 hazelbean-1.4.4/hazelbean/parallel.py
--rw-rw-rw-   0        0        0    52148 2023-05-08 17:19:48.000000 hazelbean-1.4.4/hazelbean/project_flow.py
--rw-rw-rw-   0        0        0   100770 2023-05-09 13:27:50.000000 hazelbean-1.4.4/hazelbean/pyramids.py
--rw-rw-rw-   0        0        0    52342 2022-06-15 17:44:31.000000 hazelbean-1.4.4/hazelbean/raster_vector_interface.py
--rw-rw-rw-   0        0        0      290 2022-09-22 18:26:12.000000 hazelbean-1.4.4/hazelbean/slow_config.py
--rw-rw-rw-   0        0        0    38359 2022-09-28 14:32:01.000000 hazelbean-1.4.4/hazelbean/spatial_projection.py
--rw-rw-rw-   0        0        0   237426 2023-06-01 20:11:20.000000 hazelbean-1.4.4/hazelbean/spatial_utils.py
--rw-rw-rw-   0        0        0    90574 2023-01-12 21:05:30.000000 hazelbean-1.4.4/hazelbean/stats.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:47:03.855000 hazelbean-1.4.4/hazelbean/ui/
--rw-rw-rw-   0        0        0        0 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/__init__.py
--rw-rw-rw-   0        0        0     5376 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/auto_ui.py
--rw-rw-rw-   0        0        0     6353 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/auto_ui_tg.py
--rw-rw-rw-   0        0        0    23376 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/cli.py
--rw-rw-rw-   0        0        0    24868 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/datastack.py
--rw-rw-rw-   0        0        0     2621 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/execution.py
--rw-rw-rw-   0        0        0   102272 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/inputs.py
--rw-rw-rw-   0        0        0     2565 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/launcher.py
--rw-rw-rw-   0        0        0   112823 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/model.py
--rw-rw-rw-   0        0        0    10862 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/usage.py
--rw-rw-rw-   0        0        0     3750 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/usage_logger.py
--rw-rw-rw-   0        0        0    18766 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/utils.py
--rw-rw-rw-   0        0        0     5941 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/ui/validation.py
--rw-rw-rw-   0        0        0    31806 2023-06-07 14:28:37.000000 hazelbean-1.4.4/hazelbean/utils.py
--rw-rw-rw-   0        0        0    82552 2023-03-03 14:42:11.000000 hazelbean-1.4.4/hazelbean/visualization.py
--rw-rw-rw-   0        0        0     8838 2022-03-21 14:48:42.000000 hazelbean-1.4.4/hazelbean/watershed_processing.py
-drwxrwxrwx   0        0        0        0 2023-06-07 15:47:02.252000 hazelbean-1.4.4/hazelbean.egg-info/
--rw-rw-rw-   0        0        0      443 2023-06-07 15:46:59.000000 hazelbean-1.4.4/hazelbean.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1857 2023-06-07 15:47:00.000000 hazelbean-1.4.4/hazelbean.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 15:46:59.000000 hazelbean-1.4.4/hazelbean.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-07 15:46:59.000000 hazelbean-1.4.4/hazelbean.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-07 15:47:03.923000 hazelbean-1.4.4/setup.cfg
--rw-rw-rw-   0        0        0     1708 2023-06-07 15:46:58.000000 hazelbean-1.4.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:02:20.126000 hazelbean-1.4.5/
+-rw-rw-rw-   0        0        0    14763 2023-06-08 15:02:14.000000 hazelbean-1.4.5/LICENSE
+-rw-rw-rw-   0        0        0      145 2023-06-08 15:02:14.000000 hazelbean-1.4.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      443 2023-06-08 15:02:20.063000 hazelbean-1.4.5/PKG-INFO
+-rw-rw-rw-   0        0        0     4863 2023-06-08 15:02:14.000000 hazelbean-1.4.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 15:02:18.028000 hazelbean-1.4.5/hazelbean/
+-rw-rw-rw-   0        0        0     8196 2022-09-28 15:14:40.000000 hazelbean-1.4.5/hazelbean/__init__.py
+-rw-rw-rw-   0        0        0    15645 2022-09-28 14:32:01.000000 hazelbean-1.4.5/hazelbean/arrayframe.py
+-rw-rw-rw-   0        0        0     6865 2022-05-09 18:31:33.000000 hazelbean-1.4.5/hazelbean/arrayframe_functions.py
+-rw-rw-rw-   0        0        0     5787 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/arrayframe_numpy_functions.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:02:19.119000 hazelbean-1.4.5/hazelbean/calculation_core/
+-rw-rw-rw-   0        0        0     2523 2022-09-27 18:48:13.000000 hazelbean-1.4.5/hazelbean/calculation_core/__init__.py
+-rw-rw-rw-   0        0        0   364367 2023-01-30 15:25:17.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.c
+-rw-rw-rw-   0        0        0    59392 2023-01-30 15:25:21.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0   370413 2023-06-06 15:16:35.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.cpp
+-rw-rw-rw-   0        0        0     5843 2023-01-30 15:25:06.000000 hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.pyx
+-rw-rw-rw-   0        0        0      746 2023-06-01 20:11:21.000000 hazelbean-1.4.5/hazelbean/calculation_core/compile_cython_functions.py
+-rw-rw-rw-   0        0        0  3445406 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.c
+-rw-rw-rw-   0        0        0   567808 2023-06-02 01:58:12.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  3452047 2023-06-06 15:16:35.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.cpp
+-rw-rw-rw-   0        0        0   150011 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.pyx
+-rw-rw-rw-   0        0        0     4830 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/cat_ears.py
+-rw-rw-rw-   0        0        0     7177 2023-06-01 20:54:47.000000 hazelbean-1.4.5/hazelbean/cloud_utils.py
+-rw-rw-rw-   0        0        0    19206 2022-09-23 17:47:57.000000 hazelbean-1.4.5/hazelbean/config.py
+-rw-rw-rw-   0        0        0     3471 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/conventions.py
+-rw-rw-rw-   0        0        0     8594 2023-06-05 19:37:33.000000 hazelbean-1.4.5/hazelbean/core.py
+-rw-rw-rw-   0        0        0    21132 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/data_structures.py
+-rw-rw-rw-   0        0        0    30780 2023-02-16 18:33:50.000000 hazelbean-1.4.5/hazelbean/file_io.py
+-rw-rw-rw-   0        0        0   115964 2022-09-23 21:13:00.000000 hazelbean-1.4.5/hazelbean/geoprocessing.py
+-rw-rw-rw-   0        0        0    74113 2023-03-08 17:18:14.000000 hazelbean-1.4.5/hazelbean/geoprocessing_extension.py
+-rw-rw-rw-   0        0        0    44554 2022-09-22 15:56:20.000000 hazelbean-1.4.5/hazelbean/globals.py
+-rw-rw-rw-   0        0        0    43887 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/netcdf.py
+-rw-rw-rw-   0        0        0    75326 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/os_utils.py
+-rw-rw-rw-   0        0        0    20647 2023-01-28 21:04:04.000000 hazelbean-1.4.5/hazelbean/parallel.py
+-rw-rw-rw-   0        0        0    52148 2023-05-08 17:19:48.000000 hazelbean-1.4.5/hazelbean/project_flow.py
+-rw-rw-rw-   0        0        0   100770 2023-05-09 13:27:50.000000 hazelbean-1.4.5/hazelbean/pyramids.py
+-rw-rw-rw-   0        0        0    52342 2022-06-15 17:44:31.000000 hazelbean-1.4.5/hazelbean/raster_vector_interface.py
+-rw-rw-rw-   0        0        0      290 2022-09-22 18:26:12.000000 hazelbean-1.4.5/hazelbean/slow_config.py
+-rw-rw-rw-   0        0        0    38359 2022-09-28 14:32:01.000000 hazelbean-1.4.5/hazelbean/spatial_projection.py
+-rw-rw-rw-   0        0        0   237426 2023-06-01 20:11:20.000000 hazelbean-1.4.5/hazelbean/spatial_utils.py
+-rw-rw-rw-   0        0        0    90574 2023-01-12 21:05:30.000000 hazelbean-1.4.5/hazelbean/stats.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:02:20.040000 hazelbean-1.4.5/hazelbean/ui/
+-rw-rw-rw-   0        0        0        0 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/__init__.py
+-rw-rw-rw-   0        0        0     5376 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/auto_ui.py
+-rw-rw-rw-   0        0        0     6353 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/auto_ui_tg.py
+-rw-rw-rw-   0        0        0    23376 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/cli.py
+-rw-rw-rw-   0        0        0    24868 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/datastack.py
+-rw-rw-rw-   0        0        0     2621 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/execution.py
+-rw-rw-rw-   0        0        0   102272 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/inputs.py
+-rw-rw-rw-   0        0        0     2565 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/launcher.py
+-rw-rw-rw-   0        0        0   112823 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/model.py
+-rw-rw-rw-   0        0        0    10862 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/usage.py
+-rw-rw-rw-   0        0        0     3750 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/usage_logger.py
+-rw-rw-rw-   0        0        0    18766 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/utils.py
+-rw-rw-rw-   0        0        0     5941 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/ui/validation.py
+-rw-rw-rw-   0        0        0    31953 2023-06-07 19:23:27.000000 hazelbean-1.4.5/hazelbean/utils.py
+-rw-rw-rw-   0        0        0    82552 2023-03-03 14:42:11.000000 hazelbean-1.4.5/hazelbean/visualization.py
+-rw-rw-rw-   0        0        0     8838 2022-03-21 14:48:42.000000 hazelbean-1.4.5/hazelbean/watershed_processing.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:02:18.299000 hazelbean-1.4.5/hazelbean.egg-info/
+-rw-rw-rw-   0        0        0      443 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1857 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-08 15:02:15.000000 hazelbean-1.4.5/hazelbean.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-08 15:02:20.120000 hazelbean-1.4.5/setup.cfg
+-rw-rw-rw-   0        0        0     1708 2023-06-08 15:02:14.000000 hazelbean-1.4.5/setup.py
```

### Comparing `hazelbean-1.4.4/LICENSE` & `hazelbean-1.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/README.md` & `hazelbean-1.4.5/README.md`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/__init__.py` & `hazelbean-1.4.5/hazelbean/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/arrayframe.py` & `hazelbean-1.4.5/hazelbean/arrayframe.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/arrayframe_functions.py` & `hazelbean-1.4.5/hazelbean/arrayframe_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/arrayframe_numpy_functions.py` & `hazelbean-1.4.5/hazelbean/arrayframe_numpy_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/__init__.py` & `hazelbean-1.4.5/hazelbean/calculation_core/__init__.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.c` & `hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.c`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.cpp` & `hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.cpp`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/aspect_ratio_array_functions.pyx` & `hazelbean-1.4.5/hazelbean/calculation_core/aspect_ratio_array_functions.pyx`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/compile_cython_functions.py` & `hazelbean-1.4.5/hazelbean/calculation_core/compile_cython_functions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.c` & `hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.c`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.cpp` & `hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.cpp`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/calculation_core/cython_functions.pyx` & `hazelbean-1.4.5/hazelbean/calculation_core/cython_functions.pyx`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/cat_ears.py` & `hazelbean-1.4.5/hazelbean/cat_ears.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/cloud_utils.py` & `hazelbean-1.4.5/hazelbean/cloud_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/config.py` & `hazelbean-1.4.5/hazelbean/config.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/conventions.py` & `hazelbean-1.4.5/hazelbean/conventions.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/core.py` & `hazelbean-1.4.5/hazelbean/core.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/data_structures.py` & `hazelbean-1.4.5/hazelbean/data_structures.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/file_io.py` & `hazelbean-1.4.5/hazelbean/file_io.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/geoprocessing.py` & `hazelbean-1.4.5/hazelbean/geoprocessing.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/geoprocessing_extension.py` & `hazelbean-1.4.5/hazelbean/geoprocessing_extension.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/globals.py` & `hazelbean-1.4.5/hazelbean/globals.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/netcdf.py` & `hazelbean-1.4.5/hazelbean/netcdf.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/os_utils.py` & `hazelbean-1.4.5/hazelbean/os_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/parallel.py` & `hazelbean-1.4.5/hazelbean/parallel.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/project_flow.py` & `hazelbean-1.4.5/hazelbean/project_flow.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/pyramids.py` & `hazelbean-1.4.5/hazelbean/pyramids.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/raster_vector_interface.py` & `hazelbean-1.4.5/hazelbean/raster_vector_interface.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/spatial_projection.py` & `hazelbean-1.4.5/hazelbean/spatial_projection.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/spatial_utils.py` & `hazelbean-1.4.5/hazelbean/spatial_utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/stats.py` & `hazelbean-1.4.5/hazelbean/stats.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/auto_ui.py` & `hazelbean-1.4.5/hazelbean/ui/auto_ui.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/auto_ui_tg.py` & `hazelbean-1.4.5/hazelbean/ui/auto_ui_tg.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/cli.py` & `hazelbean-1.4.5/hazelbean/ui/cli.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/datastack.py` & `hazelbean-1.4.5/hazelbean/ui/datastack.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/execution.py` & `hazelbean-1.4.5/hazelbean/ui/execution.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/inputs.py` & `hazelbean-1.4.5/hazelbean/ui/inputs.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/launcher.py` & `hazelbean-1.4.5/hazelbean/ui/launcher.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/model.py` & `hazelbean-1.4.5/hazelbean/ui/model.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/usage.py` & `hazelbean-1.4.5/hazelbean/ui/usage.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/usage_logger.py` & `hazelbean-1.4.5/hazelbean/ui/usage_logger.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/utils.py` & `hazelbean-1.4.5/hazelbean/ui/utils.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/ui/validation.py` & `hazelbean-1.4.5/hazelbean/ui/validation.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/utils.py` & `hazelbean-1.4.5/hazelbean/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -768,18 +768,20 @@
     path = os.path.join(possible_dirs[0], relative_path)
 
     # START HERE: Got confused on logic because of double-nesting the filename
     return path
 
 
 
-def path_to_url(input_path, left_path, url_start=''):
-    splitted_path = hb.split_assume_two(input_path, left_path) 
-
-    url = os.path.join(url_start, left_path, splitted_path[1])
+def path_to_url(input_path, local_path_to_strip, url_start=''):
+    splitted_path = hb.split_assume_two(input_path.replace('\\', '/'), local_path_to_strip.replace('\\', '/')) 
+    right_path = splitted_path[1]
+    if right_path.startswith('/'):
+        right_path = right_path[1:]
+    url = os.path.join(url_start, right_path)
     url = url.replace('\\', '/')
 
     return url
 
 def url_to_path(input_url, left_path, path_start):
     splitted_path = hb.split_assume_two(input_url, left_path)
```

### Comparing `hazelbean-1.4.4/hazelbean/visualization.py` & `hazelbean-1.4.5/hazelbean/visualization.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean/watershed_processing.py` & `hazelbean-1.4.5/hazelbean/watershed_processing.py`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/hazelbean.egg-info/SOURCES.txt` & `hazelbean-1.4.5/hazelbean.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hazelbean-1.4.4/setup.py` & `hazelbean-1.4.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 packages=find_packages()
 include_package_data=True
 
 setup(
   name = 'hazelbean',
   packages = packages,
-  version = '1.4.4',
+  version = '1.4.5',
   description = 'Geospatial research tools',
   long_description = 'Geospatial research tools for economics and sustainability science.',
   author = 'Justin Andrew Johnson',
   url = 'https://github.com/jandrewjohnson/hazelbean',
   download_url = 'https://github.com/jandrewjohnson/hazelbean',
   keywords = ['geospatial', 'raster', 'shapefile', 'sustainability science'],
   classifiers = ["Programming Language :: Python :: 3"],
```

