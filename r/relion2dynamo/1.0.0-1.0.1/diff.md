# Comparing `tmp/relion2dynamo-1.0.0.tar.gz` & `tmp/relion2dynamo-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "relion2dynamo-1.0.0.tar", last modified: Wed Dec 14 11:19:25 2022, max compression
+gzip compressed data, was "relion2dynamo-1.0.1.tar", last modified: Thu Jun  8 12:46:56 2023, max compression
```

## Comparing `relion2dynamo-1.0.0.tar` & `relion2dynamo-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2022-12-14 11:19:25.687851 relion2dynamo-1.0.0/
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)       75 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/.gitignore
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1520 2022-11-03 13:55:36.000000 relion2dynamo-1.0.0/LICENSE.txt
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1447 2022-12-14 11:19:25.680851 relion2dynamo-1.0.0/PKG-INFO
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)      610 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/README.md
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1595 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/pyproject.toml
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)       38 2022-12-14 11:19:25.690851 relion2dynamo-1.0.0/setup.cfg
-drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2022-12-14 11:19:25.287843 relion2dynamo-1.0.0/src/
-drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2022-12-14 11:19:25.380845 relion2dynamo-1.0.0/src/relion2dynamo/
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)      290 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/src/relion2dynamo/__init__.py
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)      631 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/src/relion2dynamo/_io_converter.py
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)      176 2022-12-14 11:19:24.000000 relion2dynamo-1.0.0/src/relion2dynamo/_version.py
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)     2621 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/src/relion2dynamo/relion2dynamo.py
-drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2022-12-14 11:19:25.493847 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1447 2022-12-14 11:19:25.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/PKG-INFO
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)      528 2022-12-14 11:19:25.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/SOURCES.txt
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)        1 2022-12-14 11:19:25.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/dependency_links.txt
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)       66 2022-12-14 11:19:25.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/entry_points.txt
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)        1 2022-12-14 11:07:58.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/not-zip-safe
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)       76 2022-12-14 11:19:25.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/requires.txt
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)       14 2022-12-14 11:19:25.000000 relion2dynamo-1.0.0/src/relion2dynamo.egg-info/top_level.txt
-drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2022-12-14 11:19:25.664851 relion2dynamo-1.0.0/test_data/
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)  1184116 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/test_data/4_1.star
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)  6871027 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/test_data/import.star
--rw-r--r--   0 pe002     (4133) ubcg97    (1090)   110538 2022-12-14 11:16:05.000000 relion2dynamo-1.0.0/test_data/refine.star
+drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2023-06-08 12:46:56.374780 relion2dynamo-1.0.1/
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)       75 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/.gitignore
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1520 2022-11-03 13:55:36.000000 relion2dynamo-1.0.1/LICENSE.txt
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1447 2023-06-08 12:46:56.372779 relion2dynamo-1.0.1/PKG-INFO
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)      610 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/README.md
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1595 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/pyproject.toml
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)       38 2023-06-08 12:46:56.374780 relion2dynamo-1.0.1/setup.cfg
+drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2023-06-08 12:46:56.236776 relion2dynamo-1.0.1/src/
+drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2023-06-08 12:46:56.256776 relion2dynamo-1.0.1/src/relion2dynamo/
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)      290 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/src/relion2dynamo/__init__.py
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)      631 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/src/relion2dynamo/_io_converter.py
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)      160 2023-06-08 12:46:55.000000 relion2dynamo-1.0.1/src/relion2dynamo/_version.py
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)     3020 2023-06-08 11:41:33.000000 relion2dynamo-1.0.1/src/relion2dynamo/relion2dynamo.py
+drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2023-06-08 12:46:56.278777 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)     1447 2023-06-08 12:46:56.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/PKG-INFO
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)      528 2023-06-08 12:46:56.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/SOURCES.txt
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)        1 2023-06-08 12:46:56.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/dependency_links.txt
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)       66 2023-06-08 12:46:56.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/entry_points.txt
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)        1 2022-12-14 11:07:58.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/not-zip-safe
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)       76 2023-06-08 12:46:56.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/requires.txt
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)       14 2023-06-08 12:46:56.000000 relion2dynamo-1.0.1/src/relion2dynamo.egg-info/top_level.txt
+drwxr-xr-x   0 pe002     (4133) ubcg97    (1090)        0 2023-06-08 12:46:56.368779 relion2dynamo-1.0.1/test_data/
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)  1184116 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/test_data/4_1.star
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)  6871027 2022-12-14 11:16:05.000000 relion2dynamo-1.0.1/test_data/import.star
+-rw-r--r--   0 pe002     (4133) ubcg97    (1090)   110538 2023-06-08 12:41:58.000000 relion2dynamo-1.0.1/test_data/refine.star
```

### Comparing `relion2dynamo-1.0.0/LICENSE.txt` & `relion2dynamo-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/PKG-INFO` & `relion2dynamo-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relion2dynamo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Converts RELION particle star files to Dynamo tables
 Author: Euan Pyle
 Author-email: euanpyle@gmail.com
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/EuanPyle/relion2dynamo
 Project-URL: repository, https://github.com/EuanPyle/relion2dynamo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `relion2dynamo-1.0.0/README.md` & `relion2dynamo-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/pyproject.toml` & `relion2dynamo-1.0.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/src/relion2dynamo/_io_converter.py` & `relion2dynamo-1.0.1/src/relion2dynamo/_io_converter.py`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/src/relion2dynamo/relion2dynamo.py` & `relion2dynamo-1.0.1/src/relion2dynamo/relion2dynamo.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,47 +30,52 @@
 
     # Read STAR file
     relion_star = starfile.read(relion_star_file)
     
     # If exists, remove optics table 
     if isinstance(relion_star,OrderedDict):
         try: 
-            relion_star = pd.DataFrame.from_dict(relion_star['particles'])
+            relion_particles = pd.DataFrame.from_dict(relion_star['particles'])
+            relion_optics = pd.DataFrame.from_dict(relion_star['optics'])
         except KeyError:
-            raise RuntimeError("Cannot find data_particles in star file")    
+            raise RuntimeError("Cannot find data_particles or data_optics in star file")    
     
     # Initialise empty dict for dynamo
     dynamo_data = {}
 
     # Get XYZ positions and put into data
+    unbinned_pixel_size = relion_optics['rlnTomoTiltSeriesPixelSize']
+    
     for axis in ('x', 'y', 'z'):
-        relion_heading = 'rlnCoordinate' + axis.upper()
-        dynamo_data[axis] = relion_star[relion_heading]
+        relion_coordinate_heading = 'rlnCoordinate' + axis.upper()
+        relion_shift_heading = 'rlnOrigin' + axis.upper() + 'Angst'
+        relion_shift = relion_particles[relion_shift_heading] / unbinned_pixel_size
+        dynamo_data[axis] = relion_particles[relion_coordinate_heading] - relion_shift 
 
     # Get euler angles and convert to dynamo convention (only if eulers present in STAR file)
-    if 'rlnAngleRot' in relion_star.columns:
-        eulers_relion = relion_star[['rlnAngleRot', 'rlnAngleTilt', 'rlnAnglePsi']].to_numpy()			       
+    if 'rlnAngleRot' in relion_particles.columns:
+        eulers_relion = relion_particles[['rlnAngleRot', 'rlnAngleTilt', 'rlnAnglePsi']].to_numpy()			       
         eulers_dynamo = convert_eulers(eulers_relion,
                                        source_meta='relion',
                                        target_meta='dynamo')				       
 	
         dynamo_data['tdrot'] = eulers_dynamo[:, 0]
         dynamo_data['tilt'] = eulers_dynamo[:, 1]
         dynamo_data['narot'] = eulers_dynamo[:, 2]
     
     # Add tomo to Dynamo table    
-    dynamo_data['tomo'] = relion_star['rlnTomoName'].str.split('_').str[1]
+    dynamo_data['tomo'] = relion_particles['rlnTomoName'].str.split('_').str[1]
         
     # Add object number to Dynamo table
-    if 'rlnObjectNumber' in relion_star.columns:
-        dynamo_data['reg'] = relion_star['rlnObjectNumber']
+    if 'rlnObjectNumber' in relion_particles.columns:
+        dynamo_data['reg'] = relion_particles['rlnObjectNumber']
 
     # Add class number to Dynamo table
-    if 'rlnClassNumber' in relion_star.columns:
-        dynamo_data['class'] = relion_star['rlnClassNumber']
+    if 'rlnClassNumber' in relion_particles.columns:
+        dynamo_data['class'] = relion_particles['rlnClassNumber']
 
     # Convert to DataFrame
     df = pd.DataFrame.from_dict(dynamo_data)
 
     # Write table file
     io_names = IOConverter(
         input_star = relion_star_file,
```

### Comparing `relion2dynamo-1.0.0/src/relion2dynamo.egg-info/PKG-INFO` & `relion2dynamo-1.0.1/src/relion2dynamo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: relion2dynamo
-Version: 1.0.0
+Version: 1.0.1
 Summary: Converts RELION particle star files to Dynamo tables
 Author: Euan Pyle
 Author-email: euanpyle@gmail.com
 License: BSD 3-Clause License
 Project-URL: homepage, https://github.com/EuanPyle/relion2dynamo
 Project-URL: repository, https://github.com/EuanPyle/relion2dynamo
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `relion2dynamo-1.0.0/src/relion2dynamo.egg-info/SOURCES.txt` & `relion2dynamo-1.0.1/src/relion2dynamo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/test_data/4_1.star` & `relion2dynamo-1.0.1/test_data/4_1.star`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/test_data/import.star` & `relion2dynamo-1.0.1/test_data/import.star`

 * *Files identical despite different names*

### Comparing `relion2dynamo-1.0.0/test_data/refine.star` & `relion2dynamo-1.0.1/test_data/refine.star`

 * *Files identical despite different names*

