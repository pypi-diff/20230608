# Comparing `tmp/neuroshape-0.0.4.1.tar.gz` & `tmp/neuroshape-0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neuroshape-0.0.4.1.tar", last modified: Thu Jun  8 07:37:40 2023, max compression
+gzip compressed data, was "neuroshape-0.0.4.2.tar", last modified: Thu Jun  8 10:46:14 2023, max compression
```

## Comparing `neuroshape-0.0.4.1.tar` & `neuroshape-0.0.4.2.tar`

### file list

```diff
@@ -1,47 +1,61 @@
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.326776 neuroshape-0.0.4.1/
--rw-r--r--   0 nik        (502) admin       (80)     1501 2023-06-07 02:08:37.000000 neuroshape-0.0.4.1/LICENSE
--rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-08 07:37:40.326508 neuroshape-0.0.4.1/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     4445 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/README.rst
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.311140 neuroshape-0.0.4.1/neuroshape/
--rw-r--r--   0 nik        (502) admin       (80)        0 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)    21494 2023-06-07 06:22:41.000000 neuroshape-0.0.4.1/neuroshape/connectopic_laplacian.py
--rw-r--r--   0 nik        (502) admin       (80)     5054 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/eigenmaps.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.316638 neuroshape-0.0.4.1/neuroshape/nulls/
--rw-r--r--   0 nik        (502) admin       (80)       44 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/neuroshape/nulls/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     5351 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/burt.py
--rw-r--r--   0 nik        (502) admin       (80)    14902 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/eigenshuff.py
--rw-r--r--   0 nik        (502) admin       (80)    11914 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/neuroshape/nulls/eigensphere.py
--rw-r--r--   0 nik        (502) admin       (80)    25239 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/nulls.py
--rw-r--r--   0 nik        (502) admin       (80)    27669 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/spins.py
--rw-r--r--   0 nik        (502) admin       (80)    12845 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/nulls/waveshuff.py
--rw-r--r--   0 nik        (502) admin       (80)     4078 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/permutation.py
--rw-r--r--   0 nik        (502) admin       (80)     5145 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/poly_eigenmaps.py
--rw-r--r--   0 nik        (502) admin       (80)     5400 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/stats.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.325254 neuroshape-0.0.4.1/neuroshape/utils/
--rw-r--r--   0 nik        (502) admin       (80)       25 2023-06-07 00:31:38.000000 neuroshape-0.0.4.1/neuroshape/utils/__init__.py
--rw-r--r--   0 nik        (502) admin       (80)     1345 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/check_fs_subjid.py
--rw-r--r--   0 nik        (502) admin       (80)      616 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/check_map.py
--rw-r--r--   0 nik        (502) admin       (80)     6553 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/checks.py
--rw-r--r--   0 nik        (502) admin       (80)      917 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/compare_parallel.py
--rw-r--r--   0 nik        (502) admin       (80)     3501 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/compute_geodesic_distance.py
--rw-r--r--   0 nik        (502) admin       (80)     6248 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/concavehull.py
--rw-r--r--   0 nik        (502) admin       (80)    10192 2023-06-08 03:48:59.000000 neuroshape-0.0.4.1/neuroshape/utils/eigen.py
--rw-r--r--   0 nik        (502) admin       (80)    25397 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/fs_shapeDNA.py
--rw-r--r--   0 nik        (502) admin       (80)     9310 2023-06-07 04:41:54.000000 neuroshape-0.0.4.1/neuroshape/utils/geometry.py
--rw-r--r--   0 nik        (502) admin       (80)      348 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/load_mesh_vertices.py
--rw-r--r--   0 nik        (502) admin       (80)     2639 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/meshtransforms.py
--rw-r--r--   0 nik        (502) admin       (80)      201 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/swap_single_row.py
--rw-r--r--   0 nik        (502) admin       (80)      540 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/tmpname.py
--rw-r--r--   0 nik        (502) admin       (80)      193 2023-06-04 23:43:38.000000 neuroshape-0.0.4.1/neuroshape/utils/zscore_avg_method.py
--rw-r--r--   0 nik        (502) admin       (80)    15295 2023-06-07 02:28:43.000000 neuroshape-0.0.4.1/neuroshape/volume_eigenmodes.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.312037 neuroshape-0.0.4.1/neuroshape.egg-info/
--rw-r--r--   0 nik        (502) admin       (80)      468 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/PKG-INFO
--rw-r--r--   0 nik        (502) admin       (80)     1105 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/SOURCES.txt
--rw-r--r--   0 nik        (502) admin       (80)        1 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/dependency_links.txt
--rw-r--r--   0 nik        (502) admin       (80)       11 2023-06-08 07:37:40.000000 neuroshape-0.0.4.1/neuroshape.egg-info/top_level.txt
--rw-r--r--   0 nik        (502) admin       (80)       38 2023-06-08 07:37:40.326853 neuroshape-0.0.4.1/setup.cfg
--rw-r--r--   0 nik        (502) admin       (80)     1063 2023-06-08 07:37:35.000000 neuroshape-0.0.4.1/setup.py
-drwxr-xr-x   0 nik        (502) admin       (80)        0 2023-06-08 07:37:40.326123 neuroshape-0.0.4.1/src/
--rw-r--r--   0 nik        (502) admin       (80)     5389 2023-06-07 07:20:28.000000 neuroshape-0.0.4.1/src/eta_squared.c
--rw-r--r--   0 nik        (502) admin       (80)     2545 2023-06-06 05:49:54.000000 neuroshape-0.0.4.1/src/euler_threshold.c
--rw-r--r--   0 nik        (502) admin       (80)     5946 2023-06-06 05:46:53.000000 neuroshape-0.0.4.1/src/glmfit.c
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.966253 neuroshape-0.0.4.2/
+-rw-r--r--   0 c3336955   (503) staff       (20)     1501 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/LICENSE
+-rw-r--r--   0 c3336955   (503) staff       (20)     2350 2023-06-08 10:46:14.961895 neuroshape-0.0.4.2/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     4445 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/README.rst
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.929746 neuroshape-0.0.4.2/neuroshape/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    21494 2023-06-08 07:46:54.000000 neuroshape-0.0.4.2/neuroshape/connectopic_laplacian.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5054 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/eigenmaps.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.938101 neuroshape-0.0.4.2/neuroshape/nipype/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/__init__.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.938444 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/__init__.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.939482 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/
+-rw-r--r--   0 c3336955   (503) staff       (20)      269 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    13219 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nipype/interfaces/workbench/metric.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.944555 neuroshape-0.0.4.2/neuroshape/nulls/
+-rw-r--r--   0 c3336955   (503) staff       (20)       44 2023-06-08 02:12:42.000000 neuroshape-0.0.4.2/neuroshape/nulls/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5351 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    14902 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/eigenshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    11914 2023-06-08 02:09:49.000000 neuroshape-0.0.4.2/neuroshape/nulls/eigensphere.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25239 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    27669 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/spins.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.947480 neuroshape-0.0.4.2/neuroshape/nulls/tests/
+-rw-r--r--   0 c3336955   (503) staff       (20)        0 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      530 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_burt.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      804 2023-06-08 09:00:37.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_eigenresamp.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      695 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_nulls.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      814 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/tests/test_spins.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    12845 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/nulls/waveshuff.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     4078 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/permutation.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5145 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/poly_eigenmaps.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     5400 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/stats.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.958478 neuroshape-0.0.4.2/neuroshape/utils/
+-rw-r--r--   0 c3336955   (503) staff       (20)       25 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/neuroshape/utils/__init__.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     1345 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/check_fs_subjid.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      616 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/check_map.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6553 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/checks.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      917 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/compare_parallel.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     3501 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/compute_geodesic_distance.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     6248 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/concavehull.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    10192 2023-06-08 01:18:54.000000 neuroshape-0.0.4.2/neuroshape/utils/eigen.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    25397 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/fs_shapeDNA.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     9310 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/neuroshape/utils/geometry.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      348 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/load_mesh_vertices.py
+-rw-r--r--   0 c3336955   (503) staff       (20)     2639 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/meshtransforms.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      201 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/swap_single_row.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      540 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/tmpname.py
+-rw-r--r--   0 c3336955   (503) staff       (20)      193 2023-06-03 12:09:04.000000 neuroshape-0.0.4.2/neuroshape/utils/zscore_avg_method.py
+-rw-r--r--   0 c3336955   (503) staff       (20)    15295 2023-06-07 11:17:25.000000 neuroshape-0.0.4.2/neuroshape/volume_eigenmodes.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.937490 neuroshape-0.0.4.2/neuroshape.egg-info/
+-rw-r--r--   0 c3336955   (503) staff       (20)     2350 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/PKG-INFO
+-rw-r--r--   0 c3336955   (503) staff       (20)     1479 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/SOURCES.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)        1 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/dependency_links.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)       11 2023-06-08 10:46:14.000000 neuroshape-0.0.4.2/neuroshape.egg-info/top_level.txt
+-rw-r--r--   0 c3336955   (503) staff       (20)      617 2023-06-08 10:46:08.000000 neuroshape-0.0.4.2/pyproject.toml
+-rw-r--r--   0 c3336955   (503) staff       (20)       38 2023-06-08 10:46:14.966414 neuroshape-0.0.4.2/setup.cfg
+-rw-r--r--   0 c3336955   (503) staff       (20)     1039 2023-06-08 10:46:05.000000 neuroshape-0.0.4.2/setup.py
+drwxr-xr-x   0 c3336955   (503) staff       (20)        0 2023-06-08 10:46:14.961075 neuroshape-0.0.4.2/src/
+-rw-r--r--   0 c3336955   (503) staff       (20)     4664 2023-06-06 11:30:08.000000 neuroshape-0.0.4.2/src/eta_squared.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     2545 2023-06-06 10:51:35.000000 neuroshape-0.0.4.2/src/euler_threshold.c
+-rw-r--r--   0 c3336955   (503) staff       (20)     5946 2023-06-06 00:28:41.000000 neuroshape-0.0.4.2/src/glmfit.c
```

### Comparing `neuroshape-0.0.4.1/LICENSE` & `neuroshape-0.0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/README.rst` & `neuroshape-0.0.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/connectopic_laplacian.py` & `neuroshape-0.0.4.2/neuroshape/connectopic_laplacian.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/eigenmaps.py` & `neuroshape-0.0.4.2/neuroshape/eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/nulls/burt.py` & `neuroshape-0.0.4.2/neuroshape/nulls/burt.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/nulls/eigenshuff.py` & `neuroshape-0.0.4.2/neuroshape/nulls/eigenshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/nulls/eigensphere.py` & `neuroshape-0.0.4.2/neuroshape/nulls/eigensphere.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/nulls/nulls.py` & `neuroshape-0.0.4.2/neuroshape/nulls/nulls.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/nulls/spins.py` & `neuroshape-0.0.4.2/neuroshape/nulls/spins.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/nulls/waveshuff.py` & `neuroshape-0.0.4.2/neuroshape/nulls/waveshuff.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/permutation.py` & `neuroshape-0.0.4.2/neuroshape/permutation.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/poly_eigenmaps.py` & `neuroshape-0.0.4.2/neuroshape/poly_eigenmaps.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/stats.py` & `neuroshape-0.0.4.2/neuroshape/stats.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/check_fs_subjid.py` & `neuroshape-0.0.4.2/neuroshape/utils/check_fs_subjid.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/check_map.py` & `neuroshape-0.0.4.2/neuroshape/utils/check_map.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/checks.py` & `neuroshape-0.0.4.2/neuroshape/utils/checks.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/compare_parallel.py` & `neuroshape-0.0.4.2/neuroshape/utils/compare_parallel.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/compute_geodesic_distance.py` & `neuroshape-0.0.4.2/neuroshape/utils/compute_geodesic_distance.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/concavehull.py` & `neuroshape-0.0.4.2/neuroshape/utils/concavehull.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/eigen.py` & `neuroshape-0.0.4.2/neuroshape/utils/eigen.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/fs_shapeDNA.py` & `neuroshape-0.0.4.2/neuroshape/utils/fs_shapeDNA.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/geometry.py` & `neuroshape-0.0.4.2/neuroshape/utils/geometry.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/meshtransforms.py` & `neuroshape-0.0.4.2/neuroshape/utils/meshtransforms.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/utils/tmpname.py` & `neuroshape-0.0.4.2/neuroshape/utils/tmpname.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape/volume_eigenmodes.py` & `neuroshape-0.0.4.2/neuroshape/volume_eigenmodes.py`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/neuroshape.egg-info/SOURCES.txt` & `neuroshape-0.0.4.2/neuroshape.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 LICENSE
 README.rst
+pyproject.toml
 setup.py
 neuroshape/__init__.py
 neuroshape/connectopic_laplacian.py
 neuroshape/eigenmaps.py
 neuroshape/permutation.py
 neuroshape/poly_eigenmaps.py
 neuroshape/stats.py
 neuroshape/volume_eigenmodes.py
 neuroshape.egg-info/PKG-INFO
 neuroshape.egg-info/SOURCES.txt
 neuroshape.egg-info/dependency_links.txt
 neuroshape.egg-info/top_level.txt
+neuroshape/nipype/__init__.py
+neuroshape/nipype/interfaces/__init__.py
+neuroshape/nipype/interfaces/workbench/__init__.py
+neuroshape/nipype/interfaces/workbench/metric.py
 neuroshape/nulls/__init__.py
 neuroshape/nulls/burt.py
 neuroshape/nulls/eigenshuff.py
 neuroshape/nulls/eigensphere.py
 neuroshape/nulls/nulls.py
 neuroshape/nulls/spins.py
 neuroshape/nulls/waveshuff.py
+neuroshape/nulls/tests/__init__.py
+neuroshape/nulls/tests/test_burt.py
+neuroshape/nulls/tests/test_eigenresamp.py
+neuroshape/nulls/tests/test_nulls.py
+neuroshape/nulls/tests/test_spins.py
 neuroshape/utils/__init__.py
 neuroshape/utils/check_fs_subjid.py
 neuroshape/utils/check_map.py
 neuroshape/utils/checks.py
 neuroshape/utils/compare_parallel.py
 neuroshape/utils/compute_geodesic_distance.py
 neuroshape/utils/concavehull.py
```

### Comparing `neuroshape-0.0.4.1/setup.py` & `neuroshape-0.0.4.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 '''
     setup.py file for neuroshape module
 '''
 
-from setuptools import setup, Extension
+from setuptools import setup, Extension, find_packages
 import numpy
 
 # define the extension module
 eta = Extension('neuroshape.eta', sources=['src/eta_squared.c'],
                           include_dirs=[numpy.get_include()])
 
 glmfit = Extension('neuroshape._stats', sources=['src/glmfit.c'],
                    include_dirs=[numpy.get_include()])
 
 euler = Extension('neuroshape.euler', sources=['src/euler_threshold.c'],
                   include_dirs=[numpy.get_include()])
 
 # run the setup
 setup(name='neuroshape',
-      version='0.0.4.1',
+      version='0.0.4.2',
       description="For computing connectopic and geometric Laplacian eigenmodes and performing null hypothesis testing. As implementation is ongoing, this description is subject to rapid change.",
       author='Nikitas C. Koussis, Systems Neuroscience Group Newcastle',
       author_email='nikitas.koussis@gmail.com',
       url='https://github.com/nikitas-k/neuroshape-dev',
-      packages=['neuroshape', 'neuroshape.nulls', 'neuroshape.utils'],
+      packages=find_packages(),
       ext_modules=[eta, glmfit, euler])
```

### Comparing `neuroshape-0.0.4.1/src/eta_squared.c` & `neuroshape-0.0.4.2/src/eta_squared.c`

 * *Files 16% similar despite different names*

```diff
@@ -24,135 +24,119 @@
  *
  * For this program to work, numpy.vectorize must be called in
  * in python to generate a numpy-friendly function. See 
  * neuroshape/examples/compute_eta_squared.py for an example
  * 
  */
 
+/* declare main function */
+static PyObject* eta_squared(PyObject* self, PyObject* args);
+
+/*
+ * This tells Python what methods this module has
+ *
+ */
+static PyMethodDef EtaMethods[] = {
+    {"eta_squared",
+        eta_squared,
+        METH_VARARGS, "Compute eta-squared coefficient row-wise of a 2-dimensional array."},
+    {NULL, NULL, 0, NULL}
+};
+
 /*
  * This actually defines the eta squared function for
  * input args from Python.
  */
 
 
 static PyObject* eta_squared(PyObject* self, PyObject* args)
 {
     PyArrayObject* arr;
     if (!PyArg_ParseTuple(args, "O!", &PyArray_Type, &arr))
         return NULL;
     
-    int N = arr->dimensions[0];
-    int p = arr->dimensions[1];
-    
+    int num_rows = arr->dimensions[0];
+    int num_cols = arr->dimensions[1];
     /* check number of dims and whether data is in correct format */
-    if ( N < p ) {
+    if ( num_rows < num_cols ) {
         printf('ERROR: Number of observations must exceed number of features (is your data transposed?)');
         return NULL;    
     }
     npy_intp nd = PyArray_NDIM(arr);
     if ( nd != 2 ) {
         printf('ERROR: Input must be a 2-dimensional matrix');
         return NULL;    
     }
     
-    npy_intp dims[2] = {N, N};
+    npy_intp dims[2] = {num_rows, num_rows};
 
     PyArrayObject* oarr = (PyArrayObject*)PyArray_SimpleNew(nd, dims, NPY_DOUBLE);
     if (oarr == NULL)
         return NULL;
 
-    double* z = PyArray_DATA(arr);
-    double* eta = PyArray_DATA(oarr);
+    double* data_ptr = PyArray_DATA(arr);
+    double* out_ptr = PyArray_DATA(oarr);
 
-    double* mu = (double*)malloc(N * p * sizeof(double));
-    double* mu_bar = (double*)malloc(N * sizeof(double));
+    double mu_bar = 0.0;
+    double mu_1 = 0.0;
+    int count = 0;
     
     npy_intp row_stride = PyArray_STRIDE(arr, 0) / sizeof(double);
     npy_intp col_stride = PyArray_STRIDE(arr, 1) / sizeof(double);
-    npy_intp outrow_stride = PyArray_STRIDE(oarr, 0) / sizeof(double);
-    npy_intp outcol_stride = PyArray_STRIDE(oarr, 1) / sizeof(double);
     
-    for (int i = 0; i < N; i++) {
-        // Calculate mu
-        for (int k = 0; k < p; k++) {
-            double sum = 0.0;
-            for (int j = 0; j < N; j++) {
-                if (j != i)
-                    sum += z[j * row_stride + k * col_stride];
-            }
-            mu[k] = (z[i * row_stride + k * col_stride] + sum) / N;
-        }
-
+    npy_intp i,j,k;
 
-        // Calculate mu_bar
-        for (int k = 0; k < p; k++) {
-            double sum = 0.0;
-            for (int j = 0; j < N; j++) {
-                sum += z[j * p + k];
+    // Calculate mu_bar
+    for (i = 0; i < num_rows; i++) {
+        for (k = 0; k < num_rows; k++) {
+            for (j = 0; j < num_cols; j++) {
+                double vali = data_ptr[i * row_stride + j * col_stride];
+                double valk = data_ptr[k * row_stride + j * col_stride];
+                double mu = (vali + valk) / 2.0;
+                mu_1 += mu;
+                count++;
             }
-            mu_bar[k] = sum / N;
         }
+    }
+    mu_bar = mu_1 / count;
 
-        // Calculate eta_squared
-        for (int j = 0; j < N; j++) {
+    // Calculate eta-squared coefficients
+    for (i = 0; i < num_rows; i++) {
+        for (k = 0; k < num_rows; k++) {
             double num = 0.0;
             double denom = 0.0;
-            for (int k = 0; k < p; k++) {
-                double diff = z[i * row_stride + k * col_stride] - mu[k];
-                num += diff * diff;
-                double diff_bar = z[j * row_stride + k * col_stride] - mu_bar[k];
-                denom += diff_bar * diff_bar;
+            for (j = 0; j < num_cols; j++) {
+                double vali = data_ptr[i * row_stride + j * col_stride];
+                double valk = data_ptr[k * row_stride + j * col_stride];
+                double mu = (vali + valk) / 2.0;
+                double diff_a = vali - mu;
+                double diff_b = valk - mu;
+                double powera = diff_a * diff_a;
+                double powerb = diff_b * diff_b;
+                double diff_bar_a = vali - mu_bar;
+                double diff_bar_b = valk - mu_bar;
+                double powerax = diff_bar_a * diff_bar_a;
+                double powerbx = diff_bar_b * diff_bar_b;
+                num += powera + powerb;
+                denom += powerax + powerbx;
+            }
+            if ( denom == 0.0 ){
+                double eta = 0.0;
+                out_ptr[i*num_rows + k] = eta;
+            } else {
+                double eta = 1.0 - (num / denom);
+                out_ptr[i*num_rows + k] = eta;
             }
-            eta[j * outrow_stride + i * outcol_stride] = 1.0 - (num / denom);
+            
         }
     }
 
-    free(mu);
-    free(mu_bar);
-
+    Py_DECREF(out_ptr);
     return PyArray_Return(oarr);
 }
-//     // Calculate eta-squared coefficients
-//     for (i = 0; i < num_rows; i++) {
-//         for (k = 0; k < num_rows; k++) {
-//             double num = 0.0;
-//             double denom = 0.0;
-//             for (j = 0; j < num_cols; j++) {
-//                 double vali = data_ptr[i * row_stride + j * col_stride];
-//                 double valk = data_ptr[k * row_stride + j * col_stride];
-//                 double mu = (vali + valk) / 2.0;
-//                 double diff_a = vali - mu;
-//                 double diff_b = valk - mu;
-//                 double powera = diff_a * diff_a;
-//                 double powerb = diff_b * diff_b;
-//                 double diff_bar_a = vali - mu_bar;
-//                 double diff_bar_b = valk - mu_bar;
-//                 double powerax = diff_bar_a * diff_bar_a;
-//                 double powerbx = diff_bar_b * diff_bar_b;
-//                 num += powera + powerb;
-//                 denom += powerax + powerbx;
-//             }
-//             if ( denom == 0.0 ){
-//                 double eta = 0.0;
-//                 out_ptr[i*num_rows + k] = eta;
-//             } else {
-//                 double eta = 1.0 - (num / denom);
-//                 out_ptr[i*num_rows + k] = eta;
-//             }
-//             
-//         }
-//     }
-
-
-static PyMethodDef EtaMethods[] = {
-    {"eta_squared",
-        eta_squared,
-        METH_VARARGS, "Compute eta-squared coefficient row-wise of a 2-dimensional array."},
-    {NULL, NULL, 0, NULL}
-};
 
 static struct PyModuleDef cModPyDem = {
     PyModuleDef_HEAD_INIT,
     "neuroshape.eta",
     "Eta-squared 2-dimensional array calculation implementation in C",
     -1,
     EtaMethods
```

### Comparing `neuroshape-0.0.4.1/src/euler_threshold.c` & `neuroshape-0.0.4.2/src/euler_threshold.c`

 * *Files identical despite different names*

### Comparing `neuroshape-0.0.4.1/src/glmfit.c` & `neuroshape-0.0.4.2/src/glmfit.c`

 * *Files identical despite different names*

