# Comparing `tmp/veros-extra-setups-1.4.5.tar.gz` & `tmp/veros-extra-setups-1.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "veros-extra-setups-1.4.5.tar", last modified: Mon Aug 22 07:45:57 2022, max compression
+gzip compressed data, was "veros-extra-setups-1.4.6.tar", last modified: Thu Jun  8 12:25:05 2023, max compression
```

## Comparing `veros-extra-setups-1.4.5.tar` & `veros-extra-setups-1.4.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/
--rw-r--r--   0 runner    (1001) docker     (121)     1066 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       79 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      152 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      345 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1965 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      497 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups/setups/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups/setups/acc_sector/
--rw-r--r--   0 runner    (1001) docker     (121)       89 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/acc_sector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9297 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/acc_sector/acc_sector.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups/setups/fjord/
--rw-r--r--   0 runner    (1001) docker     (121)       75 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/fjord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9690 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/fjord/fjord.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      337 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/assets.json
--rw-r--r--   0 runner    (1001) docker     (121)    19282 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/na_mask.png
--rw-r--r--   0 runner    (1001) docker     (121)    36904 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/topography_idealized.png
--rw-r--r--   0 runner    (1001) docker     (121)    19980 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/wave_propagation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-22 07:45:57.515697 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1270 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      938 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-22 07:45:57.000000 veros-extra-setups-1.4.5/veros_extra_setups.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)    78254 2022-08-22 07:45:45.000000 veros-extra-setups-1.4.5/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups/
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups/setups/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups/setups/acc_sector/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/acc_sector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/acc_sector/acc_sector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups/setups/fjord/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/fjord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9690 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/fjord/fjord.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/assets.json
+-rw-r--r--   0 runner    (1001) docker     (123)    19282 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/na_mask.png
+-rw-r--r--   0 runner    (1001) docker     (123)    36904 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/topography_idealized.png
+-rw-r--r--   0 runner    (1001) docker     (123)    19980 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/wave_propagation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:25:05.514324 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 12:25:05.000000 veros-extra-setups-1.4.6/veros_extra_setups.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-06-08 12:24:56.000000 veros-extra-setups-1.4.6/versioneer.py
```

### Comparing `veros-extra-setups-1.4.5/LICENSE` & `veros-extra-setups-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/PKG-INFO` & `veros-extra-setups-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veros-extra-setups
-Version: 1.4.5
+Version: 1.4.6
 Summary: Extra setups for Veros, the versatile ocean simulator.
 Home-page: https://veros-extra-setups.readthedocs.io
 Author: Dion Häfner (NBI Copenhagen)
 Author-email: dion.haefner@nbi.ku.dk
 License: MIT
 Keywords: oceanography python parallel numpy multi-core geophysics ocean-model mpi4py jax
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `veros-extra-setups-1.4.5/setup.py` & `veros-extra-setups-1.4.6/setup.py`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups/__init__.py` & `veros-extra-setups-1.4.6/veros_extra_setups/__init__.py`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups/setups/acc_sector/acc_sector.py` & `veros-extra-setups-1.4.6/veros_extra_setups/setups/acc_sector/acc_sector.py`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups/setups/fjord/fjord.py` & `veros-extra-setups-1.4.6/veros_extra_setups/setups/fjord/fjord.py`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/na_mask.png` & `veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/na_mask.png`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/topography_idealized.png` & `veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/topography_idealized.png`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups/setups/wave_propagation/wave_propagation.py` & `veros-extra-setups-1.4.6/veros_extra_setups/setups/wave_propagation/wave_propagation.py`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups.egg-info/PKG-INFO` & `veros-extra-setups-1.4.6/veros_extra_setups.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: veros-extra-setups
-Version: 1.4.5
+Version: 1.4.6
 Summary: Extra setups for Veros, the versatile ocean simulator.
 Home-page: https://veros-extra-setups.readthedocs.io
 Author: Dion Häfner (NBI Copenhagen)
 Author-email: dion.haefner@nbi.ku.dk
 License: MIT
 Keywords: oceanography python parallel numpy multi-core geophysics ocean-model mpi4py jax
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `veros-extra-setups-1.4.5/veros_extra_setups.egg-info/SOURCES.txt` & `veros-extra-setups-1.4.6/veros_extra_setups.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `veros-extra-setups-1.4.5/versioneer.py` & `veros-extra-setups-1.4.6/versioneer.py`

 * *Files identical despite different names*

