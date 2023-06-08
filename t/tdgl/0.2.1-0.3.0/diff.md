# Comparing `tmp/tdgl-0.2.1.tar.gz` & `tmp/tdgl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tdgl-0.2.1.tar", last modified: Tue Feb  7 22:48:12 2023, max compression
+gzip compressed data, was "tdgl-0.3.0.tar", last modified: Thu Jun  8 18:23:28 2023, max compression
```

## Comparing `tdgl-0.2.1.tar` & `tdgl-0.3.0.tar`

### file list

```diff
@@ -1,65 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.210352 tdgl-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-02-07 22:47:53.000000 tdgl-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-02-07 22:48:12.210352 tdgl-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-02-07 22:47:53.000000 tdgl-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-07 22:48:12.210352 tdgl-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-02-07 22:47:53.000000 tdgl-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.202351 tdgl-0.2.1/tdgl/
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/about.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.206352 tdgl-0.2.1/tdgl/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33275 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/device/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/device/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/device/meshing.py
--rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/device/polygon.py
--rw-r--r--   0 runner    (1001) docker     (123)    14177 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/em.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.206352 tdgl-0.2.1/tdgl/finite_volume/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/finite_volume/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4235 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/finite_volume/edge_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/finite_volume/mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    10850 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/finite_volume/operators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13607 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/finite_volume/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/fluxoid.py
--rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/geometry.py
--rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/parameter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.206352 tdgl-0.2.1/tdgl/solution/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solution/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solution/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solution/plot_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    42196 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solution/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.206352 tdgl-0.2.1/tdgl/solver/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    12570 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solver/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    19225 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/solver/solve.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.206352 tdgl-0.2.1/tdgl/sources/
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/sources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/sources/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/sources/loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.210352 tdgl-0.2.1/tdgl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_about.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_em.py
--rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_solution.py
--rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_solve.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/test/test_visualize.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.210352 tdgl-0.2.1/tdgl/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/visualization/animate.py
--rw-r--r--   0 runner    (1001) docker     (123)     5576 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/visualization/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/visualization/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/visualization/io.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3884 2023-02-07 22:47:53.000000 tdgl-0.2.1/tdgl/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-07 22:48:12.206352 tdgl-0.2.1/tdgl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3516 2023-02-07 22:48:12.000000 tdgl-0.2.1/tdgl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-07 22:48:12.000000 tdgl-0.2.1/tdgl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-07 22:48:12.000000 tdgl-0.2.1/tdgl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-02-07 22:48:12.000000 tdgl-0.2.1/tdgl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-02-07 22:48:12.000000 tdgl-0.2.1/tdgl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.258404 tdgl-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-08 18:23:10.000000 tdgl-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-08 18:23:28.258404 tdgl-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4076 2023-06-08 18:23:10.000000 tdgl-0.3.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:23:28.258404 tdgl-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-06-08 18:23:10.000000 tdgl-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2957 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/about.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33522 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4988 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/meshing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21251 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/device/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14231 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/em.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/finite_volume/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4259 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/edge_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15712 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/operators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13761 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/finite_volume/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/fluxoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11888 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/parameter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/solution/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15806 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24575 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/plot_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42236 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solution/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4405 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12567 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21147 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/solver/solve.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl/sources/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/sources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/sources/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/sources/loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.258404 tdgl-0.3.0/tdgl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_em.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4192 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4006 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_solve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/test/test_visualize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.258404 tdgl-0.3.0/tdgl/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8195 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/animate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8597 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3969 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualization/io.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4332 2023-06-08 18:23:10.000000 tdgl-0.3.0/tdgl/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:28.254404 tdgl-0.3.0/tdgl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3567 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 18:23:28.000000 tdgl-0.3.0/tdgl.egg-info/top_level.txt
```

### Comparing `tdgl-0.2.1/LICENSE` & `tdgl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/PKG-INFO` & `tdgl-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdgl
-Version: 0.2.1
+Version: 0.3.0
 Summary: pyTDGL: Time-dependent Ginzburg-Landau in Python.
 Home-page: https://github.com/loganbvh/py-tdgl
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor vortex Ginzburg-Landau
 Platform: Linux
@@ -18,18 +18,19 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: jax
 License-File: LICENSE
```

### Comparing `tdgl-0.2.1/README.md` & `tdgl-0.3.0/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -53,17 +53,46 @@
 Editable installation:
 
 ```bash
 git clone https://github.com/loganbvh/py-tdgl.git
 cd py-tdgl
 pip install -e ".[dev,docs]"
 ```
+## About `pyTDGL`
 
-## Acknowledgments
+### Authors
 
-Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following:
+- Primary author and maintainer: [@loganbvh](https://github.com/loganbvh/).
+
+### Citing `pyTDGL`
+
+`pyTDGL` is described in the following paper:
+
+>*pyTDGL: Time-dependent Ginzburg-Landau in Python*, Computer Physics Communications **291**, 108799 (2023), DOI: [10.1016/j.cpc.2023.108799](https://doi.org/10.1016/j.cpc.2023.108799).
+
+If you use `pyTDGL` in your research, please cite the paper linked above.
+
+    % BibTeX citation
+    @article{
+        Bishop-Van_Horn2023-wr,
+        title    = "{pyTDGL}: Time-dependent {Ginzburg-Landau} in Python",
+        author   = "Bishop-Van Horn, Logan",
+        journal  = "Comput. Phys. Commun.",
+        volume   =  291,
+        pages    = "108799",
+        month    =  may,
+        year     =  2023,
+        url      = "http://dx.doi.org/10.1016/j.cpc.2023.108799",
+        issn     = "0010-4655",
+        doi      = "10.1016/j.cpc.2023.108799"
+    }
+
+
+### Acknowledgments
+
+Parts of this package have been adapted from [`SuperDetectorPy`](https://github.com/afsa/super-detector-py), a GitHub repo authored by [Mattias Jönsson](https://github.com/afsa). Both `SuperDetectorPy` and `py-tdgl` are released under the open-source MIT License. If you use either package in an academic publication or similar, please consider citing the following in addition to the `pyTDGL` paper:
 
 - Mattias Jönsson, Theory for superconducting few-photon detectors (Doctoral dissertation), KTH Royal Institute of Technology (2022) ([Link](http://urn.kb.se/resolve?urn=urn:nbn:se:kth:diva-312132))
 - Mattias Jönsson, Robert Vedin, Samuel Gyger, James A. Sutton, Stephan Steinhauer, Val Zwiller, Mats Wallin, Jack Lidmar, Current crowding in nanoscale superconductors within the Ginzburg-Landau model, Phys. Rev. Applied 17, 064046 (2022) ([Link](https://journals.aps.org/prapplied/abstract/10.1103/PhysRevApplied.17.064046))
 
 The user interface is adapted from [`SuperScreen`](https://github.com/loganbvh/superscreen).
```

### Comparing `tdgl-0.2.1/setup.py` & `tdgl-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,23 +40,24 @@
 LONG_DESCRIPTION = __doc__
 
 NAME = "tdgl"
 AUTHOR = "Logan Bishop-Van Horn"
 AUTHOR_EMAIL = "logan.bvh@gmail.com"
 URL = "https://github.com/loganbvh/py-tdgl"
 LICENSE = "MIT"
-PYTHON_VERSION = ">=3.8, <3.11"
+PYTHON_VERSION = ">=3.8, <3.12"
 
 INSTALL_REQUIRES = [
     "cloudpickle",
     "h5py",
     "joblib",
     "jupyter",
     "matplotlib",
     "meshpy",
+    "numba",
     "numpy",
     "pint",
     "pytest",
     "pytest-cov",
     "scipy",
     "shapely",
     "tqdm",
@@ -94,14 +95,15 @@
     "Operating System :: POSIX",
     "Operating System :: Unix",
     "Operating System :: Microsoft :: Windows",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Intended Audience :: Science/Research",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Physics",
 ]
 
 PLATFORMS = ["Linux", "Mac OSX", "Unix", "Windows"]
 KEYWORDS = "superconductor vortex Ginzburg-Landau"
```

### Comparing `tdgl-0.2.1/tdgl/__init__.py` & `tdgl-0.3.0/tdgl/__init__.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/about.py` & `tdgl-0.3.0/tdgl/about.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import sys
 import time
 from typing import Dict, Optional
 
 import IPython
 import joblib
 import matplotlib
+import numba
 import numpy
 import scipy
 from IPython.display import HTML
 
 try:
     import jax
 
@@ -55,14 +56,15 @@
     cpu_count = [joblib.cpu_count(only_physical_cores=b) for b in (True, False)]
     return {
         "tdgl": tdgl.__version__,
         "Numpy": numpy.__version__,
         "SciPy": scipy.__version__,
         "matplotlib": matplotlib.__version__,
         "jax": str(jax_version),
+        "numba": numba.__version__,
         "IPython": IPython.__version__,
         "Python": sys.version,
         "OS": f"{os.name} [{sys.platform}]",
         "Number of CPUs": f"Physical: {cpu_count[0]}, Logical: {cpu_count[1]}",
         "BLAS Info": _blas_info(),
     }
```

### Comparing `tdgl-0.2.1/tdgl/device/device.py` & `tdgl-0.3.0/tdgl/device/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import logging
 import os
+import time
 from contextlib import contextmanager, nullcontext
 from operator import attrgetter, itemgetter
 from typing import Any, Dict, List, NamedTuple, Sequence, Tuple, Union
 
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
@@ -100,15 +101,14 @@
         self.probe_points = probe_points
 
         # Make units a "read-only" attribute.
         # It should never be changed after instantiation.
         self._length_units = length_units
 
         self.mesh = None
-        self.mesh_info = None
 
     @property
     def length_units(self) -> str:
         """Length units used for the device geometry."""
         return self._length_units
 
     @property
@@ -137,15 +137,15 @@
         if self.layer.conductivity is None:
             return None
         return self.layer.conductivity * ureg(f"siemens / {self.length_units}")
 
     @property
     def kappa(self) -> float:
         """The Ginzburg-Landau parameter, :math:`\\kappa=\\lambda/\\xi`."""
-        return (self.london_lambda / self.coherence_length).magnitude
+        return (self.london_lambda / self.coherence_length).to_base_units().magnitude
 
     @property
     def Bc2(self) -> pint.Quantity:
         """Upper critical field, :math:`B_{c2}=\\Phi_0/(2\\pi\\xi^2)`."""
         return (
             ureg("Phi_0") / (2 * np.pi * self.coherence_length**2)
         ).to_base_units()
@@ -518,35 +518,40 @@
                 Passing a value <= 0 means that the number of mesh points will be
                 determined solely by the density of points in the Device's film and holes.
                 Defaults to 1.0 * self.coherence_length.
             smooth: Number of Laplacian smoothing iterations to perform.
             **meshpy_kwargs: Passed to meshpy.triangle.build().
         """
         logger.info("Generating mesh...")
+        t0 = time.perf_counter()
         if max_edge_length is None:
             max_edge_length = 1.0 * self.coherence_length.magnitude
         points, triangles = generate_mesh(
             self.film.points,
             hole_coords=[hole.points for hole in self.holes],
             min_points=min_points,
             max_edge_length=max_edge_length,
             boundary=self.film.points,
             **meshpy_kwargs,
         )
         if smooth:
+            logger.info("Smoothing mesh.")
             mesh = Mesh.from_triangulation(
                 points, triangles, create_submesh=False
             ).smooth(smooth, create_submesh=False)
             points = mesh.sites
             triangles = mesh.elements
+        logger.info("Creating Mesh object from triangulation.")
+        self._create_dimensionless_mesh(points, triangles)
+        t1 = time.perf_counter()
         logger.info(
             f"Finished generating mesh with {len(points)} points and "
             f"{len(triangles)} triangles."
         )
-        self._create_dimensionless_mesh(points, triangles)
+        logger.info(f"Total mesh generation time: {(t1 - t0):.3f} seconds")
 
     def _create_dimensionless_mesh(
         self, points: np.ndarray, triangles: np.ndarray
     ) -> Mesh:
         """Creates the dimensionless mesh.
 
         Args:
```

### Comparing `tdgl-0.2.1/tdgl/device/layer.py` & `tdgl-0.3.0/tdgl/device/layer.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/device/meshing.py` & `tdgl-0.3.0/tdgl/device/meshing.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import List, Tuple, Union
 
 import numpy as np
 from meshpy import triangle
 from scipy import spatial
 from shapely.geometry.polygon import Polygon
 
-from ..finite_volume.util import get_edge_lengths
+from ..finite_volume.util import get_max_edge_length
 from ..geometry import ensure_unique
 
 logger = logging.getLogger(__name__)
 
 
 def generate_mesh(
     poly_coords: np.ndarray,
@@ -86,40 +86,38 @@
         # that lies in each hole. Here we use the centroid of the hole.
         holes = [
             np.array(Polygon(hole).centroid.coords[0]) - r0.squeeze()
             for hole in hole_coords
         ]
         mesh_info.set_holes(holes)
 
-    if "min_angle" not in kwargs:
-        kwargs["min_angle"] = min_angle
+    kwargs = kwargs.copy()
+    kwargs["min_angle"] = min_angle
 
     mesh = triangle.build(mesh_info=mesh_info, **kwargs)
     points = np.array(mesh.points) + r0
     triangles = np.array(mesh.elements)
     if min_points is None and (max_edge_length is None or max_edge_length <= 0):
         return points, triangles
 
-    kwargs = kwargs.copy()
     kwargs["max_volume"] = dx * dy / 100
     i = 1
     if min_points is None:
         min_points = 0
     if max_edge_length is None or max_edge_length <= 0:
         max_edge_length = np.inf
-    max_length = get_edge_lengths(points, triangles).max()
+    max_length = get_max_edge_length(points, triangles)
     while (len(points) < min_points) or (max_length > max_edge_length):
         mesh = triangle.build(mesh_info=mesh_info, **kwargs)
         points = np.array(mesh.points) + r0
         triangles = np.array(mesh.elements)
-        max_length = get_edge_lengths(points, triangles).max()
-        logger.debug(
-            f"Iteration {i}: Made mesh with {len(points)} points and "
-            f"{len(triangles)} triangles with maximum edge length: "
-            f"{max_length:.2e}. Target maximum edge length: {max_edge_length:.2e}."
+        max_length = get_max_edge_length(points, triangles)
+        logger.info(
+            f"Iteration {i}: {len(points)} points, {len(triangles)} triangles,"
+            f" max_edge_length: {max_length:.1e} (target: {max_edge_length:.1e})."
         )
         if np.isfinite(max_edge_length):
             kwargs["max_volume"] *= min(0.98, np.sqrt(max_edge_length / max_length))
         else:
             kwargs["max_volume"] *= 0.98
         i += 1
     return points, triangles
```

### Comparing `tdgl-0.2.1/tdgl/device/polygon.py` & `tdgl-0.3.0/tdgl/device/polygon.py`

 * *Files 0% similar despite different names*

```diff
@@ -594,15 +594,15 @@
         return Polygon(
             name=name,
             points=np.array(h5_group["points"]),
             mesh=h5_group.attrs["mesh"],
         )
 
     def __repr__(self) -> str:
-        name = f'"{self.name}"' if self.name is not None else None
+        name = f"{self.name!r}" if self.name is not None else None
         return (
             f"{self.__class__.__name__}(name={name}, "
             f"points=<ndarray: shape={self.points.shape}>, mesh={self.mesh})"
         )
 
     def __eq__(self, other) -> bool:
         if other is self:
```

### Comparing `tdgl-0.2.1/tdgl/em.py` & `tdgl-0.3.0/tdgl/em.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from typing import Optional, Sequence, Union
 
 import numpy as np
 import pint
 from scipy import spatial, special
 from scipy.constants import mu_0
 
+from .distance import pairwise_difference
 from .finite_volume.mesh import Mesh
 
 ureg = pint.UnitRegistry()
 
 
 def convert_field(
     value: Union[np.ndarray, float, str, pint.Quantity],
@@ -98,17 +99,17 @@
     current_vectors = np.atleast_2d(current_vectors)
     currents = np.atleast_2d(currents)
     assert eval_positions.shape[-1] == 3
     assert current_positions.shape[-1] == 3
     assert current_vectors.shape[-1] == 3
     assert currents.shape[-1] == 1
 
-    dx = np.subtract.outer(eval_positions[:, 0], current_positions[:, 0])
-    dy = np.subtract.outer(eval_positions[:, 1], current_positions[:, 1])
-    dz = np.subtract.outer(eval_positions[:, 2], current_positions[:, 2])
+    dx = pairwise_difference(eval_positions[:, 0], current_positions[:, 0])
+    dy = pairwise_difference(eval_positions[:, 1], current_positions[:, 1])
+    dz = pairwise_difference(eval_positions[:, 2], current_positions[:, 2])
     rprime = np.stack([dx, dy, dz], axis=-1)
     denom = (np.linalg.norm(rprime, axis=-1) ** 3)[:, :, np.newaxis]
     integrand = np.cross(current_vectors, rprime) / denom
     integral = np.einsum("jk,ijk -> ik", currents, integrand)
     return mu_0 / (4 * np.pi) * integral * ureg("tesla")
 
 
@@ -185,17 +186,17 @@
     positions = positions * to_meter
     z0 = z0 * to_meter
     current_densities = current_densities * to_amp_per_meter
     # Calculate the pairwise distance between the current sheet and evaluation
     # points for each axis.
     x0, y0 = positions[:, 0], positions[:, 1]
     Jx, Jy = current_densities[:, 0], current_densities[:, 1]
-    dx = np.subtract.outer(x, x0)
-    dy = np.subtract.outer(y, y0)
-    dz = np.subtract.outer(z, z0 * np.ones_like(x0))
+    dx = pairwise_difference(x, x0)
+    dy = pairwise_difference(y, y0)
+    dz = pairwise_difference(z, z0 * np.ones_like(x0))
     if areas is None:
         # Triangulate the current sheet to assign an effective area to each vertex.
         triangles = spatial.Delaunay(positions).simplices
         mesh = Mesh.from_triangulation(positions[:, 0], positions[:, 1], triangles)
         areas = mesh.areas
     else:
         areas = areas * to_meter**2
```

### Comparing `tdgl-0.2.1/tdgl/finite_volume/edge_mesh.py` & `tdgl-0.3.0/tdgl/finite_volume/edge_mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,15 @@
         directions = np.diff(edge_coords, axis=1).squeeze()
         edge_lengths = np.linalg.norm(directions, axis=1)
         dual_edge_lengths = get_dual_edge_lengths(
             edge_centers,
             elements,
             dual_sites,
             edges,
+            len(sites),
         )
         return EdgeMesh(
             edge_centers,
             edges,
             boundary_edge_indices,
             directions,
             edge_lengths,
```

### Comparing `tdgl-0.2.1/tdgl/finite_volume/mesh.py` & `tdgl-0.3.0/tdgl/finite_volume/mesh.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/finite_volume/operators.py` & `tdgl-0.3.0/tdgl/finite_volume/operators.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import numpy as np
 import scipy.sparse as sp
 
 from .mesh import Mesh
 
 
-def build_divergence(mesh: Mesh) -> sp.csr_matrix:
+def build_divergence(mesh: Mesh) -> sp.csr_array:
     """Build the divergence matrix that takes the divergence of a function living
     on the edges onto the sites.
 
     Args:
         mesh: The mesh.
 
     Returns:
@@ -26,24 +26,24 @@
     edges0 = edge_mesh.edges[:, 0]
     edges1 = edge_mesh.edges[:, 1]
     rows = np.concatenate([edges0, edges1])
     cols = np.concatenate([edge_indices, edge_indices])
     values = np.concatenate(
         [weights / mesh.areas[edges0], -weights / mesh.areas[edges1]]
     )
-    return sp.csr_matrix(
+    return sp.csr_array(
         (values, (rows, cols)), shape=(len(mesh.sites), len(edge_mesh.edges))
     )
 
 
 def build_gradient(
     mesh: Mesh,
     link_exponents: Union[np.ndarray, None] = None,
     weights: Union[np.ndarray, None] = None,
-) -> sp.csr_matrix:
+) -> sp.csr_array:
     """Build the gradient for a function living on the sites onto the edges.
 
     Args:
         mesh: The mesh.
         link_exponents: The value is integrated, exponentiated and used as
             a link variable.
 
@@ -59,27 +59,27 @@
     else:
         link_variable_weights = np.exp(
             -1j * np.einsum("ij, ij -> i", link_exponents, edge_mesh.directions)
         )
     rows = np.concatenate([edge_indices, edge_indices])
     cols = np.concatenate([edge_mesh.edges[:, 1], edge_mesh.edges[:, 0]])
     values = np.concatenate([link_variable_weights * weights, -weights])
-    return sp.csr_matrix(
+    return sp.csr_array(
         (values, (rows, cols)), shape=(len(edge_mesh.edges), len(mesh.sites))
     )
 
 
 def build_laplacian(
     mesh: Mesh,
     link_exponents: Union[np.ndarray, None] = None,
     fixed_sites: Union[np.ndarray, None] = None,
     free_rows: Union[np.ndarray, None] = None,
     fixed_sites_eigenvalues: float = 1,
     weights: Union[np.ndarray, None] = None,
-) -> Tuple[sp.csc_matrix, np.ndarray]:
+) -> Tuple[sp.csc_array, np.ndarray]:
     """Build a Laplacian matrix on a given mesh.
 
     The default boundary condition is homogenous Neumann conditions. To get
     Dirichlet conditions, add fixed sites. To get non-homogenous Neumann condition,
     the flux needs to be specified using a Neumann boundary Laplacian matrix.
 
     Args:
@@ -126,23 +126,23 @@
     cols = cols[free_rows]
     values = values[free_rows]
     rows = np.concatenate([rows, fixed_sites])
     cols = np.concatenate([cols, fixed_sites])
     values = np.concatenate(
         [values, fixed_sites_eigenvalues * np.ones(len(fixed_sites))]
     )
-    laplacian = sp.csc_matrix(
+    laplacian = sp.csc_array(
         (values, (rows, cols)), shape=(len(mesh.sites), len(mesh.sites))
     )
     return laplacian, free_rows
 
 
 def build_neumann_boundary_laplacian(
     mesh: Mesh, fixed_sites: Union[np.ndarray, None] = None
-) -> sp.csr_matrix:
+) -> sp.csr_array:
     """Build extra matrix for the Laplacian to set non-homogenous Neumann
     boundary conditions.
 
     Args:
         mesh: The mesh.
         fixed_sites: The fixed sites.
 
@@ -163,42 +163,48 @@
     values = np.concatenate(
         [
             boundary_edges_length / (2 * mesh.areas[boundary_edges[:, 0]]),
             boundary_edges_length / (2 * mesh.areas[boundary_edges[:, 1]]),
         ]
     )
     # Build the matrix
-    neumann_laplacian = sp.csr_matrix(
+    neumann_laplacian = sp.csr_array(
         (values, (rows, cols)), shape=(len(mesh.sites), len(boundary_index))
     )
     # Change the rows corresponding to fixed sites to identity
     if fixed_sites is not None:
         # Convert laplacian to list of lists
         # This makes it quick to do slices
         neumann_laplacian = neumann_laplacian.tolil()
         # Change the rows corresponding to the fixed sites
         neumann_laplacian[fixed_sites, :] = 0
 
-    return neumann_laplacian.tocsr()
+    return neumann_laplacian.tocsr(copy=False)
 
 
 class MeshOperators:
     """A container for the finite volume operators for a given mesh.
 
     Args:
         mesh: The :class:`tdgl.finite_volume.Mesh` instance for which to construct
             operators.
         fixed_sites: The indices of any sites for which the value of :math:`\\psi`
             and :math:`\\mu` are fixed as boundary conditions.
     """
 
-    def __init__(self, mesh: Mesh, fixed_sites: Union[np.ndarray, None] = None):
+    def __init__(
+        self,
+        mesh: Mesh,
+        fixed_sites: Union[np.ndarray, None] = None,
+        fix_psi: bool = True,
+    ):
         self.mesh = mesh
         edge_mesh = mesh.edge_mesh
         self.fixed_sites = fixed_sites
+        self.fix_psi = fix_psi
         self.laplacian_free_rows: Union[np.ndarray, None] = None
         self.divergence: Union[sp.spmatrix, None] = None
         self.mu_laplacian: Union[sp.spmatrix, None] = None
         self.mu_boundary_laplacian: Union[sp.spmatrix, None] = None
         self.mu_laplacian_lu: Union[sp.linalg.SuperLU, None] = None
         self.psi_gradient: Union[sp.spmatrix, None] = None
         self.psi_laplacian: Union[sp.spmatrix, None] = None
@@ -239,19 +245,24 @@
         if self.psi_gradient is None:
             # Build the matrices from scratch
             self.psi_gradient = build_gradient(
                 mesh,
                 link_exponents=link_exponents,
                 weights=self.gradient_weights,
             )
+            if self.fix_psi:
+                fixed_sites = self.fixed_sites
+                free_rows = self.laplacian_free_rows
+            else:
+                fixed_sites = free_rows = None
             self.psi_laplacian, self.laplacian_free_rows = build_laplacian(
                 mesh,
                 link_exponents=link_exponents,
-                fixed_sites=self.fixed_sites,
-                free_rows=self.laplacian_free_rows,
+                fixed_sites=fixed_sites,
+                free_rows=free_rows,
                 weights=self.laplacian_weights,
             )
             return
         # Just update the link variables
         directions = mesh.edge_mesh.directions
         if self.link_exponents is None:
             link_variables = np.ones(len(directions))
@@ -267,17 +278,24 @@
             values = self.gradient_weights * link_variables
             rows, cols = self.gradient_link_rows, self.gradient_link_cols
             self.psi_gradient[rows, cols] = values
             # Update Laplacian for psi
             areas0 = mesh.areas[mesh.edge_mesh.edges[:, 0]]
             areas1 = mesh.areas[mesh.edge_mesh.edges[:, 1]]
             # Only update rows that are not fixed by boundary conditions
-            free_rows = self.laplacian_free_rows[: len(self.laplacian_link_rows)]
-            rows = self.laplacian_link_rows[free_rows]
-            cols = self.laplacian_link_cols[free_rows]
+            if self.fix_psi:
+                free_rows = self.laplacian_free_rows[: len(self.laplacian_link_rows)]
+                rows = self.laplacian_link_rows[free_rows]
+                cols = self.laplacian_link_cols[free_rows]
+            else:
+                rows = self.laplacian_link_rows
+                cols = self.laplacian_link_cols
             values = np.concatenate(
                 [
                     self.laplacian_weights * link_variables / areas0,
                     self.laplacian_weights * link_variables.conjugate() / areas1,
                 ]
-            )[free_rows]
+            )
+            if self.fix_psi:
+                values = values[free_rows]
+
             self.psi_laplacian[rows, cols] = values
```

### Comparing `tdgl-0.2.1/tdgl/finite_volume/util.py` & `tdgl-0.3.0/tdgl/finite_volume/util.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 import logging
-import multiprocessing as mp
-from functools import partial
+from collections import defaultdict
 from typing import List, Tuple
 
-import joblib
 import numpy as np
 import scipy.sparse as sp
 from scipy.spatial import ConvexHull, Delaunay, QhullError
 from shapely.geometry import MultiLineString
 from shapely.ops import orient, polygonize
+from tqdm import tqdm
 
 logger = logging.getLogger("tdgl.finite_volume")
 
 
 def get_edges(elements: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
     """Finds the edges from a list of triangle indices.
 
     Args:
-        elements: The triangle indices, shape ``(n, 3)``.
+        elements: The triangle indices, shape ``(n, 3)``
 
     Returns:
         A tuple containing an integer array of edges and a boolean array
         indicating whether each edge on in the boundary.
     """
     edges = np.concatenate([elements[:, e] for e in [(0, 1), (1, 2), (2, 0)]])
     edges = np.sort(edges, axis=1)
@@ -29,61 +28,73 @@
     return edges, counts == 1
 
 
 def get_edge_lengths(points: np.ndarray, elements: np.ndarray) -> np.ndarray:
     """Returns the lengths of all edges in a triangulation.
 
     Args:
-        points: Vertex coordinates.
-        elements: Triangle indices.
+        points: Vertex coordinates
+        elements: Triangle indices
 
     Returns:
-        An array of edge lengths.
+        An array of edge lengths
     """
     edges, _ = get_edges(elements)
     return np.linalg.norm(np.diff(points[edges], axis=1), axis=2).squeeze()
 
 
+def get_max_edge_length(points: np.ndarray, elements: np.ndarray) -> float:
+    """Returns the maximum edge length in a triangulation.
+
+    Args:
+        points: Vertex coordinates
+        elements: Triangle indices
+
+    Returns:
+        The maximum edge length
+    """
+    edges = np.concatenate([elements[:, e] for e in [(0, 1), (1, 2), (2, 0)]])
+    return np.linalg.norm(np.diff(points[edges], axis=1), axis=2).max()
+
+
 def get_dual_edge_lengths(
     edge_centers: np.ndarray,
     elements: np.ndarray,
     dual_sites: np.ndarray,
     edges: np.ndarray,
+    num_sites: float,
 ) -> np.ndarray:
     """
     Compute the lengths of the dual edges.
 
     Args:
         edge_centers: The (x, y) coordinates of the edge centers.
         elements: The triangular elements in the tesselation.
         dual_sites: The (x, y) coordinates for the dual mesh (Voronoi sites).
         edges: The edges connecting the sites.
+        num_sites: The number of sites in the mesh.
 
     Returns:
         An array of dual edge lengths.
     """
     # Create a dict with keys corresponding to the edges and values
-    # corresponding to the triangles
-    edge_to_element = {}
-    # Iterate over all elements to create the edge_to_element dict
-    edge_element_indices = [[0, 1], [1, 2], [2, 0]]
-    for i, element in enumerate(elements):
-        for idx in edge_element_indices:
-            # Make the array hashable by converting it to a tuple
-            edge = tuple(np.sort(element[idx]))
-            if edge in edge_to_element:
-                edge_to_element[edge].append(i)
-            else:
-                edge_to_element[edge] = [i]
+    # corresponding to the triangle indices
+    adj = make_adj_directed_tri_indices(elements, num_sites)
+    edge_to_element = defaultdict(list)
+    for i, j, v in zip(*sp.find(adj)):
+        # The triangle index is the entry in the adjacency matrix minus 1
+        edge_to_element[frozenset((i, j))].append(v - 1)
+    edge_to_element = dict(edge_to_element)
+
     dual_lengths = np.zeros(len(edge_centers), dtype=float)
     for i, edge in enumerate(edges):
-        indices = edge_to_element[tuple(edge)]
-        if len(indices) == 1:  # Boundary edges
+        indices = edge_to_element[frozenset(edge)]
+        if len(indices) == 1:  # Boundary edge
             dual_lengths[i] = np.linalg.norm(dual_sites[indices[0]] - edge_centers[i])
-        else:  # Inner edges
+        else:  # Inner edge
             dual_lengths[i] = np.linalg.norm(
                 dual_sites[indices[0]] - dual_sites[indices[1]]
             )
     return dual_lengths
 
 
 def generate_voronoi_vertices(
@@ -109,56 +120,54 @@
     D = 2 * B[:, 0] * C[:, 1] - 2 * B[:, 1] * C[:, 0]
     Ux = (C[:, 1] * (B**2).sum(axis=1) - B[:, 1] * (C**2).sum(axis=1)) / D
     Uy = (B[:, 0] * (C**2).sum(axis=1) - C[:, 0] * (B**2).sum(axis=1)) / D
     # Convert back to the initial coordinate system
     return np.array([Ux, Uy]).T + A
 
 
-def _get_polygon_indices(
-    elements: np.ndarray, site_index: int
-) -> Tuple[int, np.ndarray]:
-    """Helper function for get_voronoi_polygon_indices()."""
-    return np.where((elements == site_index).any(axis=1))[0]
+def make_adj_directed_tri_indices(elements: np.ndarray, num_sites: int) -> sp.csc_array:
+    """Construct the directed adjacency matrix.
+
+    Each element (i, j) represents an edge in the mesh, and the value at (i, j)
+    is 1 + the index of a triangle containing that edge.
+
+    Args:
+        elements: The triangle indices, shape ``(m, 3)``
+        num_sites: The number of sites in the mesh
+
+    Returns:
+        A directed adjacency matrix containing triangle indices + 1
+    """
+    t0 = elements[:, 0]
+    t1 = elements[:, 1]
+    t2 = elements[:, 2]
+    i = np.column_stack([t0, t1, t2]).ravel()
+    j = np.column_stack([t1, t2, t0]).ravel()
+    # store triangle index + 1 (zero means no edge connecting i and j)
+    data = np.repeat(np.arange(1, elements.shape[0] + 1), 3)
+    return sp.csc_array((data, (i, j)), shape=(num_sites, num_sites))
 
 
 def get_voronoi_polygon_indices(
-    elements: np.ndarray,
-    num_sites: int,
-    parallel: bool = True,
-    min_sites_for_multiprocessing: int = 10_000,
+    elements: np.ndarray, num_sites: int
 ) -> List[np.ndarray]:
     """Find the polygons surrounding each site.
 
+    The indices of the Voronoi vertices surrounding each site are the
+    same as the indices of the triangles adjacent to each site.
+
     Args:
         elements: The triangular elements in the tesselation.
         num_sites: The number of sites
-        parallel: If True and the number of sites is greater than
-            ``min_sites_for_multiprocessing``, then use multiprocessing.
-        min_sites_for_multiprocessing: If ``parallel`` is True and ``num_sites``
-            is greater than this value, then use multiprocessing.
 
     Returns:
         A list of arrays of Voronoi polygon indices.
     """
-    # Iterate over all sites and find the triangles that the site belongs to
-    # The indices for the triangles are the same as the indices for the
-    # Voronoi lattice
-    # This is by far the costliest step in Mesh.from_triangulation(),
-    # so by default we will use multiprocessing if there are many sites.
-    if (
-        parallel
-        and (ncpus := joblib.cpu_count(only_physical_cores=True)) > 1
-        and num_sites > min_sites_for_multiprocessing
-    ):
-        with mp.Pool(processes=ncpus) as pool:
-            results = pool.map(
-                partial(_get_polygon_indices, elements), range(num_sites)
-            )
-        return results
-    return [np.where((elements == i).any(axis=1))[0] for i in range(num_sites)]
+    adj = make_adj_directed_tri_indices(elements, num_sites).tolil()
+    return [np.array(tri) - 1 for tri in adj.data]
 
 
 def compute_voronoi_polygon_areas(
     sites: np.ndarray,
     dual_sites: np.ndarray,
     boundary: np.ndarray,
     edges: np.ndarray,
@@ -183,21 +192,23 @@
         counterclockwise-oriented Voronoi polygon vertices.
     """
 
     boundary_set = set(boundary)
     boundary_edges = edges[boundary_edge_indices]
     areas = np.zeros(len(polygons), dtype=float)
     voronoi_sites = []
-    for site, polygon in enumerate(polygons):
+    for site, polygon in enumerate(
+        tqdm(polygons, desc="Constructing Voronoi polygons")
+    ):
         # Get the polygon points
         poly = dual_sites[polygon]
-        # Polygon vertices may end up very close (e.g. delta = 2e-17) due to floating
-        # point errors, so we need to remove near-duplicate vertices.
-        _, unique = np.unique(poly.round(decimals=13), axis=0, return_index=True)
-        poly = poly[unique]
+        # # Polygon vertices may end up very close (e.g. delta = 2e-17) due to floating
+        # # point errors, so we need to remove near-duplicate vertices.
+        # _, unique = np.unique(poly.round(decimals=13), axis=0, return_index=True)
+        # poly = poly[unique]
         if site not in boundary_set:
             areas[site], is_convex = get_convex_polygon_area(poly)
             assert is_convex  # All interior Voronoi cells are convex.
             voronoi_sites.append(orient_convex_polygon(poly))
             continue
         # For points on the boundary, add vertices at the mesh site and the midpoints
         # of the two edges adjacent to the mesh site to complete the Voronoi polygon.
@@ -339,15 +350,15 @@
         polygon = orient(p)
         indices = np.array([points_list.index(xy) for xy in polygon.exterior.coords])
         polygon_indices.append(indices[:-1])
     return polygon_indices
 
 
 def get_supercurrent(
-    psi: np.ndarray, gradient: sp.csr_matrix, edges: np.ndarray
+    psi: np.ndarray, gradient: sp.csr_array, edges: np.ndarray
 ) -> np.ndarray:
     """Compute the supercurrent on the edges.
 
     Args:
         psi: The value of the complex order parameter.
         gradient: The covariant derivative matrix.
         edges: The indices for the edges.
```

### Comparing `tdgl-0.2.1/tdgl/fluxoid.py` & `tdgl-0.3.0/tdgl/fluxoid.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/geometry.py` & `tdgl-0.3.0/tdgl/geometry.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/parameter.py` & `tdgl-0.3.0/tdgl/parameter.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/solution/data.py` & `tdgl-0.3.0/tdgl/solution/data.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/solution/plot_solution.py` & `tdgl-0.3.0/tdgl/solution/plot_solution.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/solution/solution.py` & `tdgl-0.3.0/tdgl/solution/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,16 @@
 
 import cloudpickle
 import h5py
 import matplotlib.pyplot as plt
 import numpy as np
 import pint
 from scipy import interpolate
-from scipy.spatial import distance
 
+from .. import distance
 from ..about import version_dict
 from ..device.device import Device
 from ..device.polygon import Polygon
 from ..em import biot_savart_2d, convert_field
 from ..finite_volume.operators import build_gradient
 from ..fluxoid import Fluxoid
 from ..geometry import path_vectors
@@ -864,15 +864,17 @@
 
         with save_context as f:
             if "mesh" in f:
                 del f["mesh"]
             data_grp = f.require_group("data")
             if save_tdgl_data:
                 self.tdgl_data.to_hdf5(data_grp)
-                self.dynamics.to_hdf5(data_grp.require_group(str(self.tdgl_data.step)))
+                self.dynamics.to_hdf5(
+                    data_grp.require_group(f"{self.tdgl_data.step}/running_state")
+                )
             if "solution" in f:
                 del f["solution"]
             group = f.create_group("solution")
             options_grp = group.create_group("options")
             for k, v in dataclasses.asdict(self.options).items():
                 if v is not None:
                     options_grp.attrs[k] = v
@@ -912,15 +914,15 @@
             else:
                 shutil.copy(self.path, h5path)
                 self._save_to_hdf5_file(h5path, save_mesh=save_mesh)
             return
 
         if h5path is None:
             raise ValueError(
-                "The solution HDF5 file does not exist, "
+                "The solution HDF5 file does not exist "
                 "and a new HDF5 file was not given."
             )
         self._save_to_hdf5_file(h5path, save_tdgl_data=True, save_mesh=save_mesh)
 
     @staticmethod
     def from_hdf5(path: os.PathLike, solve_step: int = -1) -> "Solution":
         """Loads a :class:`tdgl.Solution` from file.
```

### Comparing `tdgl-0.2.1/tdgl/solver/options.py` & `tdgl-0.3.0/tdgl/solver/options.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,15 @@
             is equivalent to setting ``adaptive = False``.
         adaptive_window: Number of most recent solve steps to consider when
             computing the time step adaptively.
         max_solve_retries: The maximum number of times to reduce the time step in a
             given solve iteration before giving up.
         adaptive_time_step_multiplier: The factor by which to multiple the time
             step ``dt`` for each adaptive solve retry.
+        terminal_psi: Fixed value for the order parameter in current terminals.
         field_units: The units for magnetic fields.
         current_units: The units for currents.
         output_file: Path to an HDF5 file in which to save the data.
             If the file name already exists, a unique name will be generated.
             If ``output_file`` is ``None``, the solver results will not be saved
             to disk.
         save_every: Save interval in units of solve steps.
@@ -36,38 +37,48 @@
         max_iterations_per_step: The maximum number of screening iterations per solve
             step.
         screening_tolerance: Relative tolerance for the induced vector potential, used
             to evaluate convergence of the screening calculation within a single time
             step.
         screening_step_size: Step size :math:`\\alpha` for Polyak's method.
         screening_step_drag: Drag parameter :math:`\\beta` for Polyak's method.
+        screening_use_numba: Use numba for the screening calculation.
+        screening_use_jax: Use jax for the screenig calculation.
     """
 
     solve_time: float
     skip_time: float = 0.0
     dt_init: float = 1e-6
     dt_max: float = 1e-1
     adaptive: bool = True
     adaptive_window: int = 10
     max_solve_retries: int = 10
     adaptive_time_step_multiplier: float = 0.25
+    terminal_psi: Union[float, complex, None] = 0.0
     save_every: int = 100
     progress_interval: int = 0
     field_units: str = "mT"
     current_units: str = "uA"
     output_file: Union[os.PathLike, None] = None
     include_screening: bool = False
     max_iterations_per_step: int = 1000
     screening_tolerance: float = 1e-3
     screening_step_size: float = 1.0
     screening_step_drag: float = 0.5
+    screening_use_numba: bool = True
+    screening_use_jax: bool = False
 
     def validate(self) -> None:
         if self.dt_init > self.dt_max:
             raise SolverOptionsError("dt_init must be less than or equal to dt_max.")
+        if self.terminal_psi is not None and not (0 <= abs(self.terminal_psi) <= 1):
+            raise SolverOptionsError(
+                "terminal_psi must be None or have absolute value in [0, 1]"
+                f" (got {self.terminal_psi})."
+            )
         if not (0 < self.adaptive_time_step_multiplier < 1):
             raise SolverOptionsError(
                 "adaptive_time_step_multiplier must be in (0, 1)"
                 f" (got {self.adaptive_time_step_multiplier})."
             )
         if not (0 < self.screening_step_drag <= 1):
             raise SolverOptionsError(
@@ -80,7 +91,11 @@
                 f" (got {self.screening_step_size})."
             )
         if self.screening_tolerance <= 0:
             raise SolverOptionsError(
                 "screening_tolerance must be in > 0"
                 f" (got {self.screening_tolerance})."
             )
+        if self.screening_use_jax and self.screening_use_numba:
+            raise SolverOptionsError(
+                "screening_use_jax and screening_use_numba cannot both be true."
+            )
```

### Comparing `tdgl-0.2.1/tdgl/solver/runner.py` & `tdgl-0.3.0/tdgl/solver/runner.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,34 +237,34 @@
         self.state["time"] = self.time
         self.state["dt"] = self.dt
         self.data_handler.save_fixed_values(
             dict(zip(self.fixed_names, self.fixed_values))
         )
         # Thermalize if enabled
         if self.options.skip_time:
-            self._run_stage_(
+            self._run_stage(
                 "Thermalizing",
                 start_time=self.time,
                 end_time=self.options.skip_time,
                 save=False,
             )
             self.running_state.clear()
         self.time = 0
         self.state["step"] = 0
         self.state["time"] = self.time
         self.state["dt"] = self.options.dt_init
         # Run the simulation
-        self._run_stage_(
+        self._run_stage(
             "Simulating",
             start_time=self.time,
             end_time=self.options.solve_time,
             save=True,
         )
 
-    def _run_stage_(
+    def _run_stage(
         self,
         name: str,
         start_time: float,
         end_time: float,
         save: bool = True,
     ) -> None:
         """Run a stage of the simulation.
```

### Comparing `tdgl-0.2.1/tdgl/solver/solve.py` & `tdgl-0.3.0/tdgl/solver/solve.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,38 +1,70 @@
 import itertools
 import logging
 from datetime import datetime
 from typing import Callable, Dict, Sequence, Tuple, Union
 
+import numba
 import numpy as np
 import scipy.sparse as sp
-from scipy import spatial
 
 try:
     import jax
     import jax.numpy as jnp
 except (ModuleNotFoundError, ImportError):
     jax = None
 
+from .. import distance
 from ..device.device import Device, TerminalInfo
 from ..em import ureg
 from ..finite_volume.operators import MeshOperators
 from ..finite_volume.util import get_supercurrent
 from ..solution.solution import Solution
 from ..sources.constant import ConstantField
 from .options import SolverOptions
 from .runner import DataHandler, Runner
 
 logger = logging.getLogger(__name__)
 
 
-if jax is None:
-    einsum = np.einsum
-else:
-    einsum = jnp.einsum
+@numba.njit(fastmath=True, parallel=True)
+def get_A_induced_numba(
+    J_site: np.ndarray,
+    areas: np.ndarray,
+    sites: np.ndarray,
+    edge_centers: np.ndarray,
+) -> np.ndarray:
+    """Calculates the induced vector potential on the mesh edges.
+
+    Args:
+        J_site: The current density on the sites, shape ``(n, )``
+        areas: The mesh site areas, shape ``(n, )``
+        sites: The mesh site coordinates, shape ``(n, 2)``
+        edge_centers: The coordinates of the edge centers, shape ``(m, 2)``
+
+    Returns:
+        The induced vector potential on the mesh edges.
+    """
+    assert J_site.ndim == 2
+    assert J_site.shape[1] == 2
+    assert sites.shape == J_site.shape
+    assert edge_centers.ndim == 2
+    assert edge_centers.shape[1] == 2
+    out = np.empty((edge_centers.shape[0], sites.shape[1]), dtype=J_site.dtype)
+    for i in numba.prange(edge_centers.shape[0]):
+        for k in range(J_site.shape[1]):
+            tmp = 0.0
+            for j in range(J_site.shape[0]):
+                dr = np.sqrt(
+                    (edge_centers[i, 0] - sites[j, 0]) ** 2
+                    + (edge_centers[i, 1] - sites[j, 1]) ** 2
+                )
+                tmp += J_site[j, k] * areas[j] / dr
+            out[i, k] = tmp
+    return out
 
 
 def validate_terminal_currents(
     terminal_currents: Union[Callable, Dict[str, float]],
     terminal_info: Sequence[TerminalInfo],
     solver_options: SolverOptions,
     num_evals: int = 100,
@@ -243,14 +275,20 @@
     assert "dimensionless" in str(vector_potential.units)
     vector_potential = vector_potential.magnitude
 
     dt_max = options.dt_max if options.adaptive else options.dt_init
 
     # Find the current terminal sites.
     terminal_info = device.terminal_info()
+    for term_info in terminal_info:
+        if term_info.length == 0:
+            raise ValueError(
+                f"Terminal {term_info.name!r} does not contain any points"
+                " on the boundary of the mesh."
+            )
     if terminal_info:
         normal_boundary_index = np.concatenate(
             [t.site_indices for t in terminal_info], dtype=np.int64
         )
     else:
         normal_boundary_index = np.array([], dtype=np.int64)
     # Define the source-drain current.
@@ -270,48 +308,58 @@
 
         def current_func(t):
             return terminal_currents
 
     validate_terminal_currents(current_func, terminal_info, options)
 
     # Construct finite-volume operators
-    operators = MeshOperators(mesh, fixed_sites=normal_boundary_index)
+    terminal_psi = options.terminal_psi
+    operators = MeshOperators(
+        mesh,
+        fixed_sites=normal_boundary_index,
+        fix_psi=(terminal_psi is not None),
+    )
     operators.build_operators()
     operators.set_link_exponents(vector_potential)
     divergence = operators.divergence
     mu_boundary_laplacian = operators.mu_boundary_laplacian
     mu_laplacian_lu = operators.mu_laplacian_lu
     mu_gradient = operators.mu_gradient
     # Initialize the order parameter and electric potential
     psi_init = np.ones(len(mesh.sites), dtype=np.complex128)
-    psi_init[normal_boundary_index] = 0
+    if terminal_psi is not None:
+        psi_init[normal_boundary_index] = terminal_psi
     mu_init = np.zeros(len(mesh.sites))
     mu_boundary = np.zeros_like(mesh.edge_mesh.boundary_edge_indices, dtype=float)
     # Create the epsilon parameter, which sets the local critical temperature.
     if callable(disorder_epsilon):
         epsilon = np.array([float(disorder_epsilon(r)) for r in sites])
     else:
         epsilon = disorder_epsilon * np.ones(len(sites), dtype=float)
     if np.any(epsilon < -1) or np.any(epsilon > 1):
         raise ValueError("The disorder parameter epsilon must be in range [-1, 1].")
 
     if options.include_screening:
-        # Pre-compute the kernel for the screening integral.
-        directions = mesh.edge_mesh.directions
-        directions = directions / np.linalg.norm(directions, axis=1)[:, np.newaxis]
-        inv_rho = 1 / spatial.distance.cdist(mesh.edge_mesh.centers, mesh.sites)
-        # (edges, sites, spatial dimensions)
-        inv_rho = inv_rho[:, :, np.newaxis] * mesh.areas[np.newaxis, :, np.newaxis]
         A_scale = (ureg("mu_0") / (4 * np.pi) * K0 / Bc2).to_base_units().magnitude
-        inv_rho *= A_scale
+        areas = A_scale * mesh.areas
+        edge_centers = mesh.edge_mesh.centers
+        if not options.screening_use_numba:
+            # Pre-compute the kernel for the screening integral.
+            inv_rho = A_scale / distance.cdist(
+                edge_centers.astype(np.float32), sites.astype(np.float32)
+            )
+            areas = areas[:, np.newaxis].astype(np.float32)
 
-        if jax is not None:
-            # Even without a GPU, jax.numpy.einsum seems to be much faster
-            # than numpy.einsum. This may just be because jax uses float32 by default.
-            inv_rho = jax.device_put(inv_rho)
+            if options.screening_use_jax:
+                if jax is None:
+                    logger.warning(
+                        "Ignoring options.screening_use_jax because jax is not available."
+                    )
+                else:
+                    inv_rho = jax.device_put(inv_rho)
 
     # Running list of the max abs change in |psi|^2 between subsequent solve steps.
     # This list is used to calculate the adaptive time step.
     d_psi_sq_vals = []
     tentative_dt = options.dt_init
     # Parameters for the self-consistent screening calculation.
     step_size = options.screening_step_size
@@ -341,31 +389,31 @@
             )
             mu_boundary[term.boundary_edge_indices] = J_scale * current_density
 
         screening_error = np.inf
         A_induced_vals = []
         v = [0]  # Velocity for Polyak's method
         # This loop runs only once if options.include_screening is False
-        for screening_iterations in itertools.count():
+        for screening_iteration in itertools.count():
             if screening_error < options.screening_tolerance:
                 break  # Screening calculation converged.
-            if screening_iterations > options.max_iterations_per_step:
+            if screening_iteration > options.max_iterations_per_step:
                 raise RuntimeError(
                     f"Screening calculation failed to converge at step {step} after"
                     f" {options.max_iterations_per_step} iterations. Relative error in"
                     f" induced vector potential: {screening_error:.2e}"
                     f" (tolerance: {options.screening_tolerance:.2e})."
                 )
             if options.include_screening:
-                # If screening is included, update the link variables in the covariant
-                # Laplacian and gradient for psi based on the induced vector potential
-                # from the previous iteration.
+                # Update the link variables in the covariant Laplacian and gradient
+                # for psi based on the induced vector potential from the previous iteration.
                 operators.set_link_exponents(vector_potential + A_induced)
+
             # Adjust the time step and calculate the new the order parameter
-            if screening_iterations == 0:
+            if screening_iteration == 0:
                 # Find a new time step only for the first screening iteration.
                 dt = tentative_dt
             psi, abs_sq_psi, dt = adaptive_euler_step(
                 step,
                 psi,
                 old_sq_psi,
                 mu,
@@ -381,18 +429,24 @@
             lhs = (divergence @ supercurrent) - (mu_boundary_laplacian @ mu_boundary)
             mu = mu_laplacian_lu.solve(lhs)
             normal_current = -(mu_gradient @ mu)
 
             if not options.include_screening:
                 break
 
-            # Evaluate the induced vector potential
+            # Evaluate the induced vector potential.
+            # This matrix multiplication takes the vast majority of the time
+            # during a solve with screening.
             J_site = mesh.get_quantity_on_site(supercurrent + normal_current)
-            # i: edges, j: sites, k: spatial dimensions
-            new_A_induced = np.asarray(einsum("jk, ijk -> ik", J_site, inv_rho))
+            if options.screening_use_numba:
+                new_A_induced = get_A_induced_numba(J_site, areas, sites, edge_centers)
+            elif options.screening_use_jax and jax is not None:
+                new_A_induced = np.asarray(jnp.matmul(inv_rho, J_site * areas))
+            else:
+                new_A_induced = np.matmul(inv_rho, J_site * areas)
             # Update induced vector potential using Polyak's method
             dA = new_A_induced - A_induced
             v.append((1 - drag) * v[-1] + step_size * dA)
             A_induced = A_induced + v[-1]
             A_induced_vals.append(A_induced)
             if len(A_induced_vals) > 1:
                 screening_error = np.max(
@@ -403,15 +457,15 @@
 
         running_state.append("dt", dt)
         if probe_points is not None:
             # Update the voltage and phase difference
             running_state.append("mu", mu[probe_points])
             running_state.append("theta", np.angle(psi[probe_points]))
         if options.include_screening:
-            running_state.append("screening_iterations", screening_iterations)
+            running_state.append("screening_iterations", screening_iteration)
 
         if options.adaptive:
             # Compute the max abs change in |psi|^2, averaged over the adaptive window,
             # and use it to select a new time step.
             d_psi_sq_vals.append(np.abs(abs_sq_psi - old_sq_psi).max())
             window = options.adaptive_window
             if step > window:
```

### Comparing `tdgl-0.2.1/tdgl/sources/constant.py` & `tdgl-0.3.0/tdgl/sources/constant.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/sources/loop.py` & `tdgl-0.3.0/tdgl/sources/loop.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/test/conftest.py` & `tdgl-0.3.0/tdgl/test/conftest.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,19 +71,19 @@
         terminal_currents=dict(source=10, drain=-10),
     )
     return solution
 
 
 @pytest.fixture(scope="package")
 def box_device():
-    london_lambda = 1.5
+    london_lambda = 1.0
     xi = 1.5
     d = 0.1
     layer = tdgl.Layer(coherence_length=xi, london_lambda=london_lambda, thickness=d)
-    film = tdgl.Polygon("film", points=box(10))
+    film = tdgl.Polygon("film", points=box(10)).resample(501)
     device = tdgl.Device("film", layer=layer, film=film)
     device.make_mesh(min_points=2000, smooth=40, max_edge_length=xi / 2)
     return device
 
 
 @pytest.fixture(scope="package")
 def box_device_solution_no_screening(box_device):
```

### Comparing `tdgl-0.2.1/tdgl/test/test_device.py` & `tdgl-0.3.0/tdgl/test/test_device.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/test/test_em.py` & `tdgl-0.3.0/tdgl/test/test_em.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/test/test_parameter.py` & `tdgl-0.3.0/tdgl/test/test_parameter.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/test/test_solution.py` & `tdgl-0.3.0/tdgl/test/test_solution.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/test/test_solve.py` & `tdgl-0.3.0/tdgl/test/test_solve.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 import numpy as np
 import pytest
 
 import tdgl
 from tdgl.solver.options import SolverOptionsError
 
 
-@pytest.mark.parametrize("current", [5.0, 10.0, lambda t: 10])
+@pytest.mark.parametrize("current", [5.0, lambda t: 10])
 @pytest.mark.parametrize("field", [0, 1])
-def test_source_drain_current(transport_device, current, field):
+@pytest.mark.parametrize("terminal_psi", [0, 1])
+def test_source_drain_current(transport_device, current, field, terminal_psi):
     device = transport_device
     total_time = 100
 
     options = tdgl.SolverOptions(
         solve_time=total_time,
         field_units="uT",
         current_units="uA",
         save_every=100,
+        terminal_psi=terminal_psi,
     )
     if callable(current):
 
         def terminal_currents(t):
             return dict(source=current(0), drain=-current(0))
 
     else:
         terminal_currents = dict(source=current, drain=-current)
+
+    with pytest.raises(ValueError):
+        solution = tdgl.solve(
+            device,
+            options,
+            disorder_epsilon=2,
+            applied_vector_potential=field,
+            terminal_currents=terminal_currents,
+        )
     solution = tdgl.solve(
         device,
         options,
+        disorder_epsilon=lambda r: 1,
         applied_vector_potential=field,
         terminal_currents=terminal_currents,
     )
 
     if callable(current):
         current = current(0)
 
@@ -41,53 +53,72 @@
         measured_currents.append(
             solution.current_through_path(coords, with_units=False)
         )
     measured_currents = np.array(measured_currents)
     assert np.allclose(measured_currents, current, rtol=0.1)
 
 
-def test_screening(box_device):
+@pytest.mark.skip
+@pytest.mark.parametrize(
+    "use_numba, use_jax", [(False, True), (True, False), (False, False)]
+)
+def test_screening(box_device, use_numba, use_jax):
     device = box_device
-    total_time = 50
+    total_time = 5
 
     with pytest.raises(SolverOptionsError):
+        tdgl.SolverOptions(solve_time=total_time, dt_init=1e-3, dt_max=1e-4).validate()
+    with pytest.raises(SolverOptionsError):
+        tdgl.SolverOptions(solve_time=total_time, terminal_psi=2).validate()
+    with pytest.raises(SolverOptionsError):
         tdgl.SolverOptions(solve_time=total_time, screening_step_size=-1).validate()
     with pytest.raises(SolverOptionsError):
         tdgl.SolverOptions(solve_time=total_time, screening_tolerance=-1).validate()
     with pytest.raises(SolverOptionsError):
         tdgl.SolverOptions(solve_time=total_time, screening_step_drag=2).validate()
     with pytest.raises(SolverOptionsError):
         tdgl.SolverOptions(
             solve_time=total_time, adaptive_time_step_multiplier=2
         ).validate()
+    with pytest.raises(SolverOptionsError):
+        tdgl.SolverOptions(
+            solve_time=total_time, screening_use_jax=True, screening_use_numba=True
+        ).validate()
 
     options = tdgl.SolverOptions(
         solve_time=total_time,
         field_units="uT",
         current_units="uA",
+        screening_use_jax=use_jax,
+        screening_use_numba=use_numba,
     )
     field = tdgl.sources.ConstantField(50)
 
     options.include_screening = False
     solution = tdgl.solve(
         device,
         options,
         applied_vector_potential=field,
     )
 
     circle = tdgl.geometry.circle(2, points=401)
     centers = [(0, 0), (-1.5, -2.5), (2.5, 2), (0, 1)]
 
+    fluxoids_without_screening = []
     for r0 in centers:
         fluxoid = solution.polygon_fluxoid(circle + np.atleast_2d(r0), with_units=False)
-        assert abs(sum(fluxoid) / fluxoid.flux_part) >= 2e-2
+        # Without screening the fluxoid will not be quantized.
+        fluxoids_without_screening.append(abs(sum(fluxoid)))
 
     options.include_screening = True
     solution = tdgl.solve(
         device,
         options,
         applied_vector_potential=field,
     )
 
+    fluxoids_with_screening = []
     for r0 in centers:
         fluxoid = solution.polygon_fluxoid(circle + np.atleast_2d(r0), with_units=False)
-        assert abs(sum(fluxoid) / fluxoid.flux_part) < 2e-2
+        fluxoids_with_screening.append(abs(sum(fluxoid)))
+
+    assert np.all(fluxoids_with_screening < fluxoids_without_screening)
```

### Comparing `tdgl-0.2.1/tdgl/test/test_visualization.py` & `tdgl-0.3.0/tdgl/test/test_visualization.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/test/test_visualize.py` & `tdgl-0.3.0/tdgl/test/test_visualize.py`

 * *Files 6% similar despite different names*

```diff
@@ -107,15 +107,16 @@
     "quantities",
     [
         "all",
         # None,
         # "order_parameter phase vorticity supercurrent",
     ],
 )
-def test_animate_cli(solution, quantities):
+@pytest.mark.parametrize("autoscale", [True, False])
+def test_animate_cli(solution, quantities, autoscale):
     parser = visualize.make_parser()
     cmd = [
         "--input",
         solution.path,
         "animate",
         "--output",
         solution.path.replace(".h5", "-cli.gif"),
@@ -124,13 +125,15 @@
         "--max-frame",
         "-1",
         "--fps",
         "30",
         "--dpi",
         "200",
     ]
+    if autoscale:
+        cmd.append("--autoscale")
     if quantities is not None:
         cmd.extend(["--quantities"] + quantities.split(" "))
     args = parser.parse_args(cmd)
     with tdgl.non_gui_backend():
         tdgl.visualize.main(args)
         plt.close("all")
```

### Comparing `tdgl-0.2.1/tdgl/visualization/animate.py` & `tdgl-0.3.0/tdgl/visualization/animate.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     output_file: Union[str, None] = None,
     quantities: Union[str, Sequence[str]],
     fps: int = 30,
     dpi: float = 100,
     max_cols: int = 4,
     min_frame: int = 0,
     max_frame: int = -1,
+    autoscale: bool = False,
     quiver: bool = False,
     axes_off: bool = False,
     title_off: bool = False,
     full_title: bool = True,
     logger: Union[Logger, None] = None,
     silent: bool = False,
     figure_kwargs: Union[Dict[str, Any], None] = None,
@@ -47,14 +48,15 @@
             e.g., as a gif or mp4 video.
         quantities: The names of the quantities to animate.
         fps: Frame rate in frames per second.
         dpi: Resolution in dots per inch.
         max_cols: The maxiumum number of columns in the subplot grid.
         min_frame: The first frame of the animation.
         max_frame: The last frame of the animation.
+        autoscale: Autoscale colorbar limits at each frame.
         quiver: Add quiver arrows to the plots.
         axes_off: Turn off the axes for each subplot.
         title_off: Turn off the figure suptitle.
         full_title: Include the full "state" for each frame in the figure suptitle.
         figure_kwargs: Keyword arguments passed to ``plt.subplots()`` when creating
             the figure.
         writer: A :class:`matplotlib.animation.MovieWriter` instance to use when
@@ -74,15 +76,15 @@
     quantities = [Quantity.from_key(name.upper()) for name in quantities]
     num_plots = len(quantities)
     logger = logger or logging.getLogger()
     figure_kwargs = figure_kwargs or dict()
     figure_kwargs.setdefault("constrained_layout", True)
     default_figsize = (
         3.25 * min(max_cols, num_plots),
-        3 * max(1, num_plots // max_cols),
+        2.5 * max(1, num_plots // max_cols),
     )
     figure_kwargs.setdefault("figsize", default_figsize)
 
     logger.info(f"Creating animation for {[obs.name for obs in quantities]!r}.")
 
     mpl_context = nullcontext() if output_file is None else plt.ioff()
     if isinstance(input_file, str):
@@ -120,14 +122,16 @@
                 collection = ax.tripcolor(
                     x,
                     y,
                     temp_value,
                     triangles=mesh.elements,
                     shading="gouraud",
                     cmap=opts.cmap,
+                    vmin=opts.vmin,
+                    vmax=opts.vmax,
                 )
                 if quiver:
                     quiver = ax.quiver(
                         x,
                         y,
                         temp_value,
                         temp_value,
@@ -146,28 +150,45 @@
 
             vmins = [+np.inf for _ in quantities]
             vmaxs = [-np.inf for _ in quantities]
 
             def update(frame):
                 if not h5file:
                     return
+                frame += min_frame
                 state = get_state_string(h5file, frame, max_frame)
                 if not full_title:
                     state = state.split(",")[0]
                 if not title_off:
                     fig.suptitle(state)
                 for i, (quantity, collection) in enumerate(
                     zip(quantities, collections)
                 ):
-                    value, direction, limits = get_plot_data(
-                        h5file, mesh, quantity, frame
-                    )
-                    vmins[i] = min(vmins[i], limits[0])
-                    vmaxs[i] = max(vmaxs[i], limits[1])
-                    collection.set_array(value)
+                    opts = PLOT_DEFAULTS[quantity]
+                    values, direction, _ = get_plot_data(h5file, mesh, quantity, frame)
+                    mask = np.abs(values - np.mean(values)) <= 6 * np.std(values)
+                    if opts.vmin is None:
+                        if autoscale:
+                            vmins[i] = np.min(values[mask])
+                        else:
+                            vmins[i] = min(vmins[i], np.min(values[mask]))
+                    else:
+                        vmins[i] = opts.vmin
+                    if opts.vmax is None:
+                        if autoscale:
+                            vmaxs[i] = np.max(values[mask])
+                        else:
+                            vmaxs[i] = max(vmaxs[i], np.max(values[mask]))
+                    else:
+                        vmaxs[i] = opts.vmax
+                    if opts.symmetric:
+                        vmax = max(abs(vmins[i]), abs(vmaxs[i]))
+                        vmaxs[i] = vmax
+                        vmins[i] = -vmax
+                    collection.set_array(values)
                     collection.set_clim(vmins[i], vmaxs[i])
                 if quiver:
                     quiver.set_UVC(direction[:, 0], direction[:, 1])
                 fig.canvas.draw()
 
             anim = animation.FuncAnimation(
                 fig,
```

### Comparing `tdgl-0.2.1/tdgl/visualization/common.py` & `tdgl-0.3.0/tdgl/visualization/common.py`

 * *Files 5% similar despite different names*

```diff
@@ -44,34 +44,42 @@
 
 @dataclass
 class PlotDefault:
     cmap: str
     clabel: str
     xlabel: str = "$x/\\xi$"
     ylabel: str = "$y/\\xi$"
+    vmin: Union[float, None] = None
+    vmax: Union[float, None] = None
+    symmetric: bool = False
 
 
 PLOT_DEFAULTS = {
-    Quantity.ORDER_PARAMETER: PlotDefault(cmap="viridis", clabel="$|\\psi|$"),
+    Quantity.ORDER_PARAMETER: PlotDefault(
+        cmap="viridis", clabel="$|\\psi|$", vmin=0, vmax=1
+    ),
     Quantity.PHASE: PlotDefault(
-        cmap="twilight_shifted",
-        clabel="$\\arg(\\psi)/\\pi$",
+        cmap="twilight_shifted", clabel="$\\arg(\\psi)/\\pi$", vmin=-1, vmax=1
     ),
     Quantity.SUPERCURRENT: PlotDefault(cmap="inferno", clabel="$|\\vec{{J}}_s|/J_0$"),
     Quantity.NORMAL_CURRENT: PlotDefault(cmap="inferno", clabel="$|\\vec{{J}}_n|/J_0$"),
     Quantity.SCALAR_POTENTIAL: PlotDefault(cmap="magma", clabel="$\\mu/v_0$"),
     Quantity.APPLIED_VECTOR_POTENTIAL: PlotDefault(
         cmap="cividis", clabel="$a_\\mathrm{{applied}}/(\\xi B_{{c2}})$"
     ),
     Quantity.INDUCED_VECTOR_POTENTIAL: PlotDefault(
         cmap="cividis", clabel="$a_\\mathrm{{induced}}/(\\xi B_{{c2}})$"
     ),
-    Quantity.EPSILON: PlotDefault(cmap="viridis", clabel="$\\epsilon$"),
+    Quantity.EPSILON: PlotDefault(
+        cmap="viridis", clabel="$\\epsilon$", vmin=-1, vmax=1
+    ),
     Quantity.VORTICITY: PlotDefault(
-        cmap="coolwarm", clabel="$(\\vec{{\\nabla}}\\times\\vec{{J}})\\cdot\\hat{{z}}$"
+        cmap="coolwarm",
+        clabel="$(\\vec{{\\nabla}}\\times\\vec{{J}})\\cdot\\hat{{z}}$",
+        symmetric=True,
     ),
 }
 
 DEFAULT_QUANTITIES = (
     "order_parameter",
     "phase",
     "supercurrent",
```

### Comparing `tdgl-0.2.1/tdgl/visualization/interactive.py` & `tdgl-0.3.0/tdgl/visualization/interactive.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/visualization/io.py` & `tdgl-0.3.0/tdgl/visualization/io.py`

 * *Files identical despite different names*

### Comparing `tdgl-0.2.1/tdgl/visualize.py` & `tdgl-0.3.0/tdgl/visualize.py`

 * *Files 9% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     interactive_parser.add_argument(
         "-q",
         "--quantities",
         type=lambda s: str(s).upper(),
         choices=Quantity.get_keys() + ["ALL"],
         nargs="*",
         help=(
-            "Name(s) of the quantities to show. Because ``quantities`` takes a "
+            "Name(s) of the quantities to show. Because 'quantities' takes a "
             "variable number of arguments, it must be the last argument provided."
         ),
     )
 
     interactive_parser.set_defaults(func=visualize_tdgl)
 
     animate_parser = subparsers.add_parser(
@@ -57,26 +57,38 @@
     animate_parser.add_argument(
         "-f", "--fps", type=int, default=30, help="Frame rate of the animation."
     )
     animate_parser.add_argument(
         "-d", "--dpi", type=float, default=200, help="Resolution in dots per inch."
     )
     animate_parser.add_argument(
+        "--figsize",
+        type=float,
+        nargs=2,
+        default=None,
+        help="Figure size (width, height) in inches.",
+    )
+    animate_parser.add_argument(
         "--min-frame",
         type=int,
         default=0,
         help="The first frame to render.",
     )
     animate_parser.add_argument(
         "--max-frame",
         type=int,
         default=-1,
         help="The last frame to render (-1 indicates the last step in the simulation).",
     )
     animate_parser.add_argument(
+        "--autoscale",
+        action="store_true",
+        help="Autoscale colorbar limits at each frame.",
+    )
+    animate_parser.add_argument(
         "--axes-off",
         action="store_true",
         help="Turn the axes off.",
     )
     animate_parser.add_argument(
         "--title-off",
         action="store_true",
@@ -105,17 +117,20 @@
         output_file=args.output,
         logger=logger,
         silent=args.silent,
         dpi=args.dpi,
         fps=args.fps,
         min_frame=args.min_frame,
         max_frame=args.max_frame,
+        autoscale=args.autoscale,
         axes_off=args.axes_off,
         title_off=args.title_off,
     )
+    if args.figsize is not None:
+        kwargs["figure_kwargs"] = dict(figsize=args.figsize)
     if args.quantities is None or "ALL" in args.quantities:
         kwargs["quantities"] = DEFAULT_QUANTITIES
     else:
         kwargs["quantities"] = args.quantities
     create_animation(**kwargs)
```

### Comparing `tdgl-0.2.1/tdgl.egg-info/PKG-INFO` & `tdgl-0.3.0/tdgl.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tdgl
-Version: 0.2.1
+Version: 0.3.0
 Summary: pyTDGL: Time-dependent Ginzburg-Landau in Python.
 Home-page: https://github.com/loganbvh/py-tdgl
 Author: Logan Bishop-Van Horn
 Author-email: logan.bvh@gmail.com
 License: MIT
 Keywords: superconductor vortex Ginzburg-Landau
 Platform: Linux
@@ -18,18 +18,19 @@
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: jax
 License-File: LICENSE
```

### Comparing `tdgl-0.2.1/tdgl.egg-info/SOURCES.txt` & `tdgl-0.3.0/tdgl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE
 README.md
 setup.py
 tdgl/__init__.py
 tdgl/about.py
+tdgl/distance.py
 tdgl/em.py
 tdgl/fluxoid.py
 tdgl/geometry.py
 tdgl/parameter.py
 tdgl/testing.py
 tdgl/version.py
 tdgl/visualize.py
@@ -36,14 +37,15 @@
 tdgl/sources/__init__.py
 tdgl/sources/constant.py
 tdgl/sources/loop.py
 tdgl/test/__init__.py
 tdgl/test/conftest.py
 tdgl/test/test_about.py
 tdgl/test/test_device.py
+tdgl/test/test_distance.py
 tdgl/test/test_em.py
 tdgl/test/test_parameter.py
 tdgl/test/test_solution.py
 tdgl/test/test_solve.py
 tdgl/test/test_visualization.py
 tdgl/test/test_visualize.py
 tdgl/visualization/__init__.py
```

