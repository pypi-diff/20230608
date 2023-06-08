# Comparing `tmp/symforce-sym-0.8.0.tar.gz` & `tmp/symforce-sym-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "symforce-sym-0.8.0.tar", last modified: Fri Feb  3 20:54:01 2023, max compression
+gzip compressed data, was "symforce-sym-0.9.0.tar", last modified: Wed Jun  7 20:23:16 2023, max compression
```

## Comparing `symforce-sym-0.8.0.tar` & `symforce-sym-0.9.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.050713 symforce-sym-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-03 20:54:01.050713 symforce-sym-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-03 20:54:01.050713 symforce-sym-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.042713 symforce-sym-0.8.0/sym/
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8533 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/atan_camera_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/double_sphere_camera_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8538 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/equirectangular_camera_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/linear_camera_cal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.042713 symforce-sym-0.8.0/sym/ops/
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.042713 symforce-sym-0.8.0/sym/ops/atan_camera_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/atan_camera_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13251 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/atan_camera_cal/camera_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/atan_camera_cal/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3579 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/atan_camera_cal/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.042713 symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20132 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/camera_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3864 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.042713 symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10179 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/camera_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6372 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3561 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.046713 symforce-sym-0.8.0/sym/ops/linear_camera_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/linear_camera_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8205 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/linear_camera_cal/camera_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6138 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/linear_camera_cal/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3435 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/linear_camera_cal/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.046713 symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/camera_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.046713 symforce-sym-0.8.0/sym/ops/pose2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/pose2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/pose2/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3929 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/pose2/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.046713 symforce-sym-0.8.0/sym/ops/pose3/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/pose3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26440 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/pose3/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     6400 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/pose3/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.046713 symforce-sym-0.8.0/sym/ops/rot2/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/rot2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/rot2/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/rot2/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.046713 symforce-sym-0.8.0/sym/ops/rot3/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/rot3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13339 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/rot3/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5870 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/rot3/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.050713 symforce-sym-0.8.0/sym/ops/spherical_camera_cal/
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/spherical_camera_cal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7433 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/spherical_camera_cal/camera_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)    16001 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/spherical_camera_cal/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     4337 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/spherical_camera_cal/lie_group_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.050713 symforce-sym-0.8.0/sym/ops/unit3/
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/unit3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10086 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/unit3/group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5344 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/ops/unit3/lie_group_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/polynomial_camera_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)    10923 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/pose2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13103 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/pose3.py
--rw-r--r--   0 runner    (1001) docker     (123)     7802 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/rot2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11981 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/rot3.py
--rw-r--r--   0 runner    (1001) docker     (123)     9363 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/spherical_camera_cal.py
--rw-r--r--   0 runner    (1001) docker     (123)     8968 2023-02-03 20:53:39.000000 symforce-sym-0.8.0/sym/unit3.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-03 20:54:01.050713 symforce-sym-0.8.0/symforce_sym.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-02-03 20:54:01.000000 symforce-sym-0.8.0/symforce_sym.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-02-03 20:54:01.000000 symforce-sym-0.8.0/symforce_sym.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 20:54:01.000000 symforce-sym-0.8.0/symforce_sym.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-03 20:54:00.000000 symforce-sym-0.8.0/symforce_sym.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-02-03 20:54:01.000000 symforce-sym-0.8.0/symforce_sym.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-03 20:54:01.000000 symforce-sym-0.8.0/symforce_sym.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.811790 symforce-sym-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 20:23:16.811790 symforce-sym-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:23:16.811790 symforce-sym-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8464 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/atan_camera_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9137 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/double_sphere_camera_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8469 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/equirectangular_camera_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/linear_camera_cal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/atan_camera_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/atan_camera_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13181 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/atan_camera_cal/camera_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7505 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/atan_camera_cal/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/atan_camera_cal/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20062 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/camera_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3866 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10109 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/camera_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6374 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/linear_camera_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/linear_camera_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8135 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/linear_camera_cal/camera_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6140 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/linear_camera_cal/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3437 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/linear_camera_cal/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7209 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/camera_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13532 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4181 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/pose2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/pose2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6319 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/pose2/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/pose2/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/pose3/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/pose3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26442 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/pose3/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6402 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/pose3/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/rot2/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/rot2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3880 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/rot2/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/rot2/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.807789 symforce-sym-0.9.0/sym/ops/rot3/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/rot3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13341 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/rot3/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5872 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/rot3/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.811790 symforce-sym-0.9.0/sym/ops/spherical_camera_cal/
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/spherical_camera_cal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7437 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/spherical_camera_cal/camera_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16003 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/spherical_camera_cal/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4339 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/spherical_camera_cal/lie_group_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.811790 symforce-sym-0.9.0/sym/ops/unit3/
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/unit3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10088 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/unit3/group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5346 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/ops/unit3/lie_group_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8543 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/polynomial_camera_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/pose2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13306 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/pose3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7814 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/rot2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/rot3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/spherical_camera_cal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9074 2023-06-07 20:22:57.000000 symforce-sym-0.9.0/sym/unit3.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:23:16.811790 symforce-sym-0.9.0/symforce_sym.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-07 20:23:16.000000 symforce-sym-0.9.0/symforce_sym.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 2023-06-07 20:23:16.000000 symforce-sym-0.9.0/symforce_sym.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:23:16.000000 symforce-sym-0.9.0/symforce_sym.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:23:16.000000 symforce-sym-0.9.0/symforce_sym.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-07 20:23:16.000000 symforce-sym-0.9.0/symforce_sym.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-07 20:23:16.000000 symforce-sym-0.9.0/symforce_sym.egg-info/top_level.txt
```

### Comparing `symforce-sym-0.8.0/setup.py` & `symforce-sym-0.9.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # -----------------------------------------------------------------------------
 
 from setuptools import find_packages
 from setuptools import setup
 
 setup(
     name="symforce-sym",
-    version="0.8.0",
+    version="0.9.0",
     description="generated numerical python package (installed by SymForce)",
     license_file="LICENSE",
     long_description="generated numerical python package (installed by SymForce)",
     author="Skydio, Inc",
     author_email="hayk@skydio.com",
     install_requires=["numpy"],
     license="Apache 2.0",
```

### Comparing `symforce-sym-0.8.0/sym/__init__.py` & `symforce-sym-0.9.0/sym/__init__.py`

 * *Files identical despite different names*

### Comparing `symforce-sym-0.8.0/sym/atan_camera_cal.py` & `symforce-sym-0.9.0/sym/atan_camera_cal.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import numpy
 
 from .ops import atan_camera_cal as ops
 
 
 class ATANCameraCal(object):
     """
-    Autogenerated Python implementation of <class 'symforce.cam.atan_camera_cal.ATANCameraCal'>.
+    Autogenerated Python implementation of :py:class:`symforce.cam.atan_camera_cal.ATANCameraCal`.
 
     ATAN camera with 5 parameters [fx, fy, cx, cy, omega].
+
     (fx, fy) representing focal length, (cx, cy) representing principal point,
     and omega representing the distortion parameter.
 
     See here for more details:
     https://hal.inria.fr/inria-00267247/file/distcalib.pdf
     """
 
@@ -93,55 +94,53 @@
         return ops.CameraOps.principal_point(self)
 
     def pixel_from_camera_point(self, point, epsilon):
         # type: (ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.pixel_from_camera_point(self, point, epsilon)
 
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         return ops.CameraOps.pixel_from_camera_point_with_jacobians(self, point, epsilon)
 
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.camera_ray_from_pixel(self, pixel, epsilon)
 
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         return ops.CameraOps.camera_ray_from_pixel_with_jacobians(self, pixel, epsilon)
```

### Comparing `symforce-sym-0.8.0/sym/double_sphere_camera_cal.py` & `symforce-sym-0.9.0/sym/double_sphere_camera_cal.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,26 +9,27 @@
 import numpy
 
 from .ops import double_sphere_camera_cal as ops
 
 
 class DoubleSphereCameraCal(object):
     """
-    Autogenerated Python implementation of <class 'symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal'>.
+    Autogenerated Python implementation of :py:class:`symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal`.
 
     Camera model where a point is consecutively projected onto two unit spheres
-    with centers shifted by `xi`, then projected into the image plane using the
-    pinhole model shifted by `alpha / (1 - alpha)`.
+    with centers shifted by ``xi``, then projected into the image plane using the
+    pinhole model shifted by ``alpha / (1 - alpha)``.
 
     There are important differences here from the derivation in the paper and in other open-source
     packages with double sphere models; see notebooks/double_sphere_derivation.ipynb for more
     information.
 
     The storage for this class is:
-    [ fx fy cx cy xi alpha ]
+
+        [ fx fy cx cy xi alpha ]
 
     TODO(aaron): Create double_sphere_derivation.ipynb
 
     TODO(aaron): Probably want to check that values and derivatives are correct (or at least sane)
     on the valid side of the is_valid boundary
 
     Reference:
@@ -106,55 +107,53 @@
         return ops.CameraOps.principal_point(self)
 
     def pixel_from_camera_point(self, point, epsilon):
         # type: (DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.pixel_from_camera_point(self, point, epsilon)
 
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         return ops.CameraOps.pixel_from_camera_point_with_jacobians(self, point, epsilon)
 
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.camera_ray_from_pixel(self, pixel, epsilon)
 
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         return ops.CameraOps.camera_ray_from_pixel_with_jacobians(self, pixel, epsilon)
```

### Comparing `symforce-sym-0.8.0/sym/equirectangular_camera_cal.py` & `symforce-sym-0.9.0/sym/equirectangular_camera_cal.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import numpy
 
 from .ops import equirectangular_camera_cal as ops
 
 
 class EquirectangularCameraCal(object):
     """
-    Autogenerated Python implementation of <class 'symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal'>.
+    Autogenerated Python implementation of :py:class:`symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal`.
 
     Equirectangular camera model with parameters [fx, fy, cx, cy].
+
     (fx, fy) representing focal length; (cx, cy) representing principal point.
     """
 
     __slots__ = ["data"]
 
     # This is because of an issue where mypy doesn't recognize attributes defined in __slots__
     # See https://github.com/python/mypy/issues/5941
@@ -88,55 +89,53 @@
         return ops.CameraOps.principal_point(self)
 
     def pixel_from_camera_point(self, point, epsilon):
         # type: (EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.pixel_from_camera_point(self, point, epsilon)
 
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         return ops.CameraOps.pixel_from_camera_point_with_jacobians(self, point, epsilon)
 
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.camera_ray_from_pixel(self, pixel, epsilon)
 
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         return ops.CameraOps.camera_ray_from_pixel_with_jacobians(self, pixel, epsilon)
```

### Comparing `symforce-sym-0.8.0/sym/linear_camera_cal.py` & `symforce-sym-0.9.0/sym/linear_camera_cal.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,17 +9,18 @@
 import numpy
 
 from .ops import linear_camera_cal as ops
 
 
 class LinearCameraCal(object):
     """
-    Autogenerated Python implementation of <class 'symforce.cam.linear_camera_cal.LinearCameraCal'>.
+    Autogenerated Python implementation of :py:class:`symforce.cam.linear_camera_cal.LinearCameraCal`.
 
     Standard pinhole camera w/ four parameters [fx, fy, cx, cy].
+
     (fx, fy) representing focal length; (cx, cy) representing principal point.
     """
 
     __slots__ = ["data"]
 
     # This is because of an issue where mypy doesn't recognize attributes defined in __slots__
     # See https://github.com/python/mypy/issues/5941
@@ -88,55 +89,53 @@
         return ops.CameraOps.principal_point(self)
 
     def pixel_from_camera_point(self, point, epsilon):
         # type: (LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.pixel_from_camera_point(self, point, epsilon)
 
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         return ops.CameraOps.pixel_from_camera_point_with_jacobians(self, point, epsilon)
 
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.camera_ray_from_pixel(self, pixel, epsilon)
 
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         return ops.CameraOps.camera_ray_from_pixel_with_jacobians(self, pixel, epsilon)
```

### Comparing `symforce-sym-0.8.0/sym/ops/atan_camera_cal/camera_ops.py` & `symforce-sym-0.9.0/sym/ops/atan_camera_cal/camera_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class CameraOps(object):
     """
-    Python CameraOps implementation for <class 'symforce.cam.atan_camera_cal.ATANCameraCal'>.
+    Python CameraOps implementation for :py:class:`symforce.cam.atan_camera_cal.ATANCameraCal`.
     """
 
     @staticmethod
     def focal_length(self):
         # type: (sym.ATANCameraCal) -> numpy.ndarray
         """
         Return the focal length.
@@ -59,15 +59,15 @@
 
     @staticmethod
     def pixel_from_camera_point(self, point, epsilon):
         # type: (sym.ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 25
 
         # Input arrays
@@ -96,15 +96,15 @@
 
     @staticmethod
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (sym.ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         # Total ops: 113
@@ -197,17 +197,15 @@
 
     @staticmethod
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (sym.ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 27
 
         # Input arrays
@@ -245,15 +243,15 @@
 
     @staticmethod
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (sym.ATANCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         # Total ops: 133
```

### Comparing `symforce-sym-0.8.0/sym/ops/atan_camera_cal/group_ops.py` & `symforce-sym-0.9.0/sym/ops/atan_camera_cal/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.cam.atan_camera_cal.ATANCameraCal'>.
+    Python GroupOps implementation for :py:class:`symforce.cam.atan_camera_cal.ATANCameraCal`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.ATANCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/atan_camera_cal/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/atan_camera_cal/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.cam.atan_camera_cal.ATANCameraCal'>.
+    Python LieGroupOps implementation for :py:class:`symforce.cam.atan_camera_cal.ATANCameraCal`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.ATANCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/camera_ops.py` & `symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/camera_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class CameraOps(object):
     """
-    Python CameraOps implementation for <class 'symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal'>.
+    Python CameraOps implementation for :py:class:`symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal`.
     """
 
     @staticmethod
     def focal_length(self):
         # type: (sym.DoubleSphereCameraCal) -> numpy.ndarray
         """
         Return the focal length.
@@ -59,15 +59,15 @@
 
     @staticmethod
     def pixel_from_camera_point(self, point, epsilon):
         # type: (sym.DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 73
 
         # Input arrays
@@ -149,15 +149,15 @@
 
     @staticmethod
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (sym.DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         # Total ops: 136
@@ -284,17 +284,15 @@
 
     @staticmethod
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (sym.DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 62
 
         # Input arrays
@@ -337,15 +335,15 @@
 
     @staticmethod
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (sym.DoubleSphereCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         # Total ops: 297
```

### Comparing `symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/group_ops.py` & `symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal'>.
+    Python GroupOps implementation for :py:class:`symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.DoubleSphereCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/double_sphere_camera_cal/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/double_sphere_camera_cal/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal'>.
+    Python LieGroupOps implementation for :py:class:`symforce.cam.double_sphere_camera_cal.DoubleSphereCameraCal`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.DoubleSphereCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/camera_ops.py` & `symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/camera_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class CameraOps(object):
     """
-    Python CameraOps implementation for <class 'symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal'>.
+    Python CameraOps implementation for :py:class:`symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal`.
     """
 
     @staticmethod
     def focal_length(self):
         # type: (sym.EquirectangularCameraCal) -> numpy.ndarray
         """
         Return the focal length.
@@ -59,15 +59,15 @@
 
     @staticmethod
     def pixel_from_camera_point(self, point, epsilon):
         # type: (sym.EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 19
 
         # Input arrays
@@ -104,15 +104,15 @@
 
     @staticmethod
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (sym.EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         # Total ops: 34
@@ -168,17 +168,15 @@
 
     @staticmethod
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (sym.EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 19
 
         # Input arrays
@@ -217,15 +215,15 @@
 
     @staticmethod
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (sym.EquirectangularCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         # Total ops: 44
```

### Comparing `symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/group_ops.py` & `symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal'>.
+    Python GroupOps implementation for :py:class:`symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.EquirectangularCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/equirectangular_camera_cal/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/equirectangular_camera_cal/lie_group_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal'>.
+    Python LieGroupOps implementation for :py:class:`symforce.cam.equirectangular_camera_cal.EquirectangularCameraCal`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.EquirectangularCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/linear_camera_cal/camera_ops.py` & `symforce-sym-0.9.0/sym/ops/linear_camera_cal/camera_ops.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class CameraOps(object):
     """
-    Python CameraOps implementation for <class 'symforce.cam.linear_camera_cal.LinearCameraCal'>.
+    Python CameraOps implementation for :py:class:`symforce.cam.linear_camera_cal.LinearCameraCal`.
     """
 
     @staticmethod
     def focal_length(self):
         # type: (sym.LinearCameraCal) -> numpy.ndarray
         """
         Return the focal length.
@@ -59,15 +59,15 @@
 
     @staticmethod
     def pixel_from_camera_point(self, point, epsilon):
         # type: (sym.LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 10
 
         # Input arrays
@@ -93,15 +93,15 @@
 
     @staticmethod
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (sym.LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         # Total ops: 24
@@ -156,17 +156,15 @@
 
     @staticmethod
     def camera_ray_from_pixel(self, pixel, epsilon):
         # type: (sym.LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        TODO(hayk): Add a normalize boolean argument? Like in `cam.Camera`
-
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 4
 
         # Input arrays
@@ -192,15 +190,15 @@
 
     @staticmethod
     def camera_ray_from_pixel_with_jacobians(self, pixel, epsilon):
         # type: (sym.LinearCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Backproject a 2D pixel coordinate into a 3D ray in the camera frame.
 
-        Return:
+        Returns:
             camera_ray: The ray in the camera frame (NOT normalized)
             is_valid: 1 if the operation is within bounds else 0
             point_D_cal: Derivative of point with respect to intrinsic calibration parameters
             point_D_pixel: Derivation of point with respect to pixel
         """
 
         # Total ops: 14
```

### Comparing `symforce-sym-0.8.0/sym/ops/linear_camera_cal/group_ops.py` & `symforce-sym-0.9.0/sym/ops/linear_camera_cal/group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.cam.linear_camera_cal.LinearCameraCal'>.
+    Python GroupOps implementation for :py:class:`symforce.cam.linear_camera_cal.LinearCameraCal`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.LinearCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/linear_camera_cal/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/linear_camera_cal/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.cam.linear_camera_cal.LinearCameraCal'>.
+    Python LieGroupOps implementation for :py:class:`symforce.cam.linear_camera_cal.LinearCameraCal`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.LinearCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/camera_ops.py` & `symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/camera_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class CameraOps(object):
     """
-    Python CameraOps implementation for <class 'symforce.cam.polynomial_camera_cal.PolynomialCameraCal'>.
+    Python CameraOps implementation for :py:class:`symforce.cam.polynomial_camera_cal.PolynomialCameraCal`.
     """
 
     @staticmethod
     def focal_length(self):
         # type: (sym.PolynomialCameraCal) -> numpy.ndarray
         """
         Return the focal length.
@@ -59,15 +59,15 @@
 
     @staticmethod
     def pixel_from_camera_point(self, point, epsilon):
         # type: (sym.PolynomialCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 32
 
         # Input arrays
@@ -108,15 +108,15 @@
 
     @staticmethod
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (sym.PolynomialCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         # Total ops: 103
```

### Comparing `symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/group_ops.py` & `symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.cam.polynomial_camera_cal.PolynomialCameraCal'>.
+    Python GroupOps implementation for :py:class:`symforce.cam.polynomial_camera_cal.PolynomialCameraCal`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.PolynomialCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/polynomial_camera_cal/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/polynomial_camera_cal/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.cam.polynomial_camera_cal.PolynomialCameraCal'>.
+    Python LieGroupOps implementation for :py:class:`symforce.cam.polynomial_camera_cal.PolynomialCameraCal`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.PolynomialCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/pose2/group_ops.py` & `symforce-sym-0.9.0/sym/ops/pose2/group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.geo.pose2.Pose2'>.
+    Python GroupOps implementation for :py:class:`symforce.geo.pose2.Pose2`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.Pose2
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/pose2/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/pose2/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.geo.pose2.Pose2'>.
+    Python LieGroupOps implementation for :py:class:`symforce.geo.pose2.Pose2`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.Pose2
 
         # Total ops: 2
```

### Comparing `symforce-sym-0.8.0/sym/ops/pose3/group_ops.py` & `symforce-sym-0.9.0/sym/ops/pose3/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.geo.pose3.Pose3'>.
+    Python GroupOps implementation for :py:class:`symforce.geo.pose3.Pose3`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.Pose3
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/pose3/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/pose3/lie_group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.geo.pose3.Pose3'>.
+    Python LieGroupOps implementation for :py:class:`symforce.geo.pose3.Pose3`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.Pose3
 
         # Total ops: 15
```

### Comparing `symforce-sym-0.8.0/sym/ops/rot2/group_ops.py` & `symforce-sym-0.9.0/sym/ops/rot2/group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.geo.rot2.Rot2'>.
+    Python GroupOps implementation for :py:class:`symforce.geo.rot2.Rot2`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.Rot2
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/rot2/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/rot2/lie_group_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.geo.rot2.Rot2'>.
+    Python LieGroupOps implementation for :py:class:`symforce.geo.rot2.Rot2`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.Rot2
 
         # Total ops: 2
```

### Comparing `symforce-sym-0.8.0/sym/ops/rot3/group_ops.py` & `symforce-sym-0.9.0/sym/ops/rot3/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.geo.rot3.Rot3'>.
+    Python GroupOps implementation for :py:class:`symforce.geo.rot3.Rot3`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.Rot3
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/rot3/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/rot3/lie_group_ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.geo.rot3.Rot3'>.
+    Python LieGroupOps implementation for :py:class:`symforce.geo.rot3.Rot3`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.Rot3
 
         # Total ops: 15
```

### Comparing `symforce-sym-0.8.0/sym/ops/spherical_camera_cal/camera_ops.py` & `symforce-sym-0.9.0/sym/ops/spherical_camera_cal/camera_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class CameraOps(object):
     """
-    Python CameraOps implementation for <class 'symforce.cam.spherical_camera_cal.SphericalCameraCal'>.
+    Python CameraOps implementation for :py:class:`symforce.cam.spherical_camera_cal.SphericalCameraCal`.
     """
 
     @staticmethod
     def focal_length(self):
         # type: (sym.SphericalCameraCal) -> numpy.ndarray
         """
         Return the focal length.
@@ -59,15 +59,15 @@
 
     @staticmethod
     def pixel_from_camera_point(self, point, epsilon):
         # type: (sym.SphericalCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         # Total ops: 30
 
         # Input arrays
@@ -102,15 +102,15 @@
 
     @staticmethod
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (sym.SphericalCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         # Total ops: 129
```

### Comparing `symforce-sym-0.8.0/sym/ops/spherical_camera_cal/group_ops.py` & `symforce-sym-0.9.0/sym/ops/spherical_camera_cal/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.cam.spherical_camera_cal.SphericalCameraCal'>.
+    Python GroupOps implementation for :py:class:`symforce.cam.spherical_camera_cal.SphericalCameraCal`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.SphericalCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/spherical_camera_cal/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/spherical_camera_cal/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.cam.spherical_camera_cal.SphericalCameraCal'>.
+    Python LieGroupOps implementation for :py:class:`symforce.cam.spherical_camera_cal.SphericalCameraCal`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.SphericalCameraCal
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/unit3/group_ops.py` & `symforce-sym-0.9.0/sym/ops/unit3/group_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class GroupOps(object):
     """
-    Python GroupOps implementation for <class 'symforce.geo.unit3.Unit3'>.
+    Python GroupOps implementation for :py:class:`symforce.geo.unit3.Unit3`.
     """
 
     @staticmethod
     def identity():
         # type: () -> sym.Unit3
 
         # Total ops: 0
```

### Comparing `symforce-sym-0.8.0/sym/ops/unit3/lie_group_ops.py` & `symforce-sym-0.9.0/sym/ops/unit3/lie_group_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import numpy
 
 import sym  # pylint: disable=unused-import
 
 
 class LieGroupOps(object):
     """
-    Python LieGroupOps implementation for <class 'symforce.geo.unit3.Unit3'>.
+    Python LieGroupOps implementation for :py:class:`symforce.geo.unit3.Unit3`.
     """
 
     @staticmethod
     def from_tangent(vec, epsilon):
         # type: (numpy.ndarray, float) -> sym.Unit3
 
         # Total ops: 13
```

### Comparing `symforce-sym-0.8.0/sym/polynomial_camera_cal.py` & `symforce-sym-0.9.0/sym/polynomial_camera_cal.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 import numpy
 
 from .ops import polynomial_camera_cal as ops
 
 
 class PolynomialCameraCal(object):
     """
-    Autogenerated Python implementation of <class 'symforce.cam.polynomial_camera_cal.PolynomialCameraCal'>.
+    Autogenerated Python implementation of :py:class:`symforce.cam.polynomial_camera_cal.PolynomialCameraCal`.
 
-    Polynomial camera model in the style of OpenCV.
-    Distortion is a multiplicitive factor applied to the image plane coordinates in the camera
+    Polynomial camera model in the style of OpenCV
+
+    Distortion is a multiplicative factor applied to the image plane coordinates in the camera
     frame. Mapping between distorted image plane coordinates and image coordinates is done using
     a standard linear model.
 
     The distortion function is a 6th order even polynomial that is a function of the radius of the
-    image plane coordinates.
-    r = (p_img[0] ** 2 + p_img[1]**2) ** 0.5
-    distorted_weight = 1 + c0 * r^2 + c1 * r^4 + c2 * r^6
-    uv = p_img * distorted_weight
+    image plane coordinates::
+
+        r = (p_img[0] ** 2 + p_img[1] ** 2) ** 0.5
+        distorted_weight = 1 + c0 * r^2 + c1 * r^4 + c2 * r^6
+        uv = p_img * distorted_weight
     """
 
     __slots__ = ["data"]
 
     # This is because of an issue where mypy doesn't recognize attributes defined in __slots__
     # See https://github.com/python/mypy/issues/5941
     if T.TYPE_CHECKING:
@@ -115,27 +117,27 @@
         return ops.CameraOps.principal_point(self)
 
     def pixel_from_camera_point(self, point, epsilon):
         # type: (PolynomialCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.pixel_from_camera_point(self, point, epsilon)
 
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (PolynomialCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         return ops.CameraOps.pixel_from_camera_point_with_jacobians(self, point, epsilon)
```

### Comparing `symforce-sym-0.8.0/sym/pose2.py` & `symforce-sym-0.9.0/sym/pose2.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,37 +13,38 @@
 
 # isort: split
 from .ops import pose2 as ops
 
 
 class Pose2(object):
     """
-    Autogenerated Python implementation of <class 'symforce.geo.pose2.Pose2'>.
+    Autogenerated Python implementation of :py:class:`symforce.geo.pose2.Pose2`.
 
     Group of two-dimensional rigid body transformations - R2 x SO(2).
 
     The storage space is a complex (real, imag) for rotation followed by a position (x, y).
 
     The tangent space is one angle for rotation followed by two elements for translation in the
     non-rotated frame.
 
     For Lie group enthusiasts: This class is on the PRODUCT manifold.  On this class, the group
     operations (e.g. compose and between) operate as you'd expect for a Pose or SE(2), but the
     manifold operations (e.g. retract and local_coordinates) operate on the product manifold
     SO(2) x R2.  This means that:
 
-      - retract(a, vec) != compose(a, from_tangent(vec))
+    - retract(a, vec) != compose(a, from_tangent(vec))
 
-      - local_coordinates(a, b) != to_tangent(between(a, b))
+    - local_coordinates(a, b) != to_tangent(between(a, b))
 
-      - There is no hat operator, because from_tangent/to_tangent is not the matrix exp/log
+    - There is no hat operator, because from_tangent/to_tangent is not the matrix exp/log
 
-    If you need a type that has these properties in symbolic expressions, you should use Pose2_SE2.
-    There is no runtime equivalent of Pose2_SE2, see the docstring on that class for more
-    information.
+    If you need a type that has these properties in symbolic expressions, you should use
+    :class:`symforce.geo.unsupported.pose2_se2.Pose2_SE2`. There is no runtime equivalent of
+    :class:`Pose2_SE2 <symforce.geo.unsupported.pose2_se2.Pose2_SE2>`, see the docstring on that
+    class for more information.
     """
 
     __slots__ = ["data"]
 
     def __repr__(self):
         # type: () -> str
         return "<{} {}>".format(self.__class__.__name__, self.data)
@@ -131,20 +132,14 @@
         _res[1] = _self[3]
         return _res
 
     def compose_with_point(self, right):
         # type: (Pose2, numpy.ndarray) -> numpy.ndarray
         """
         Left-multiply with a compatible quantity.
-
-        Args:
-            right: (Pose2 | R2)
-
-        Returns:
-            (Pose2 | R2)
         """
 
         # Total ops: 8
 
         # Input arrays
         _self = self.data
         if right.shape == (2,):
@@ -163,23 +158,18 @@
         _res[0] = _self[0] * right[0, 0] - _self[1] * right[1, 0] + _self[2]
         _res[1] = _self[0] * right[1, 0] + _self[1] * right[0, 0] + _self[3]
         return _res
 
     def inverse_compose(self, point):
         # type: (Pose2, numpy.ndarray) -> numpy.ndarray
         """
-        This function was autogenerated from a symbolic function. Do not modify by hand.
-
-        Symbolic function: pose2_inverse_compose
-
-        Args:
-            point: Matrix21
+        Returns ``self.inverse() * point``
 
-        Outputs:
-            res: Matrix21
+        This is more efficient than calling the generated inverse and compose methods separately, if
+        doing this for one point.
         """
 
         # Total ops: 14
 
         # Input arrays
         _self = self.data
         if point.shape == (2,):
```

### Comparing `symforce-sym-0.8.0/sym/pose3.py` & `symforce-sym-0.9.0/sym/pose3.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,33 +13,38 @@
 
 # isort: split
 from .ops import pose3 as ops
 
 
 class Pose3(object):
     """
-    Autogenerated Python implementation of <class 'symforce.geo.pose3.Pose3'>.
+    Autogenerated Python implementation of :py:class:`symforce.geo.pose3.Pose3`.
 
     Group of three-dimensional rigid body transformations - SO(3) x R3.
 
     The storage is a quaternion (x, y, z, w) for rotation followed by position (x, y, z).
 
     The tangent space is 3 elements for rotation followed by 3 elements for translation in the
     non-rotated frame.
 
-    For Lie group enthusiasts: This class is on the PRODUCT manifold, if you really really want
-    SE(3) you should use Pose3_SE3.  On this class, the group operations (e.g. compose and between)
-    operate as you'd expect for a Pose or SE(3), but the manifold operations (e.g. retract and
-    local_coordinates) operate on the product manifold SO(3) x R3.  This means that:
+    For Lie group enthusiasts: This class is on the PRODUCT manifold.  On this class, the group
+    operations (e.g. compose and between) operate as you'd expect for a Pose or SE(3), but the
+    manifold operations (e.g. retract and local_coordinates) operate on the product manifold
+    SO(3) x R3.  This means that:
 
-      - retract(a, vec) != compose(a, from_tangent(vec))
+    - retract(a, vec) != compose(a, from_tangent(vec))
 
-      - local_coordinates(a, b) != to_tangent(between(a, b))
+    - local_coordinates(a, b) != to_tangent(between(a, b))
 
-      - There is no hat operator, because from_tangent/to_tangent is not the matrix exp/log
+    - There is no hat operator, because from_tangent/to_tangent is not the matrix exp/log
+
+    If you need a type that has these properties in symbolic expressions, you should use
+    :class:`symforce.geo.unsupported.pose3_se3.Pose3_SE3`. There is no runtime equivalent of
+    :class:`Pose3_SE3 <symforce.geo.unsupported.pose3_se3.Pose3_SE3>`, see the docstring on that
+    class for more information.
     """
 
     __slots__ = ["data"]
 
     def __repr__(self):
         # type: () -> str
         return "<{} {}>".format(self.__class__.__name__, self.data)
@@ -183,23 +188,18 @@
             + right[2, 0] * (_tmp3 + _tmp8 + 1)
         )
         return _res
 
     def inverse_compose(self, point):
         # type: (Pose3, numpy.ndarray) -> numpy.ndarray
         """
-        This function was autogenerated from a symbolic function. Do not modify by hand.
-
-        Symbolic function: pose3_inverse_compose
-
-        Args:
-            point: Matrix31
+        Returns ``self.inverse() * point``
 
-        Outputs:
-            res: Matrix31
+        This is more efficient than calling the generated inverse and compose methods separately, if
+        doing this for one point.
         """
 
         # Total ops: 61
 
         # Input arrays
         _self = self.data
         if point.shape == (3,):
```

### Comparing `symforce-sym-0.8.0/sym/rot2.py` & `symforce-sym-0.9.0/sym/rot2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 # isort: split
 from .ops import rot2 as ops
 
 
 class Rot2(object):
     """
-    Autogenerated Python implementation of <class 'symforce.geo.rot2.Rot2'>.
+    Autogenerated Python implementation of :py:class:`symforce.geo.rot2.Rot2`.
 
-    Group of two-dimensional orthogonal matrices with determinant +1, representing rotations
+    Group of two-dimensional orthogonal matrices with determinant ``+1``, representing rotations
     in 2D space. Backed by a complex number.
     """
 
     __slots__ = ["data"]
 
     def __repr__(self):
         # type: () -> str
@@ -82,17 +82,17 @@
         _res[1] = _self[0] * right[1, 0] + _self[1] * right[0, 0]
         return _res
 
     @staticmethod
     def from_angle(theta):
         # type: (float) -> Rot2
         """
-        Create a Rot2 from an angle `theta` in radians
+        Create a Rot2 from an angle ``theta`` in radians
 
-        This is equivalent to from_tangent([theta])
+        This is equivalent to ``from_tangent([theta])``
         """
 
         # Total ops: 2
 
         # Input arrays
 
         # Intermediate terms (0)
```

### Comparing `symforce-sym-0.8.0/sym/rot3.py` & `symforce-sym-0.9.0/sym/rot3.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,17 +11,17 @@
 
 # isort: split
 from .ops import rot3 as ops
 
 
 class Rot3(object):
     """
-    Autogenerated Python implementation of <class 'symforce.geo.rot3.Rot3'>.
+    Autogenerated Python implementation of :py:class:`symforce.geo.rot3.Rot3`.
 
-    Group of three-dimensional orthogonal matrices with determinant +1, representing
+    Group of three-dimensional orthogonal matrices with determinant ``+1``, representing
     rotations in 3D space. Backed by a quaternion with (x, y, z, w) storage.
     """
 
     __slots__ = ["data"]
 
     def __repr__(self):
         # type: () -> str
@@ -254,14 +254,96 @@
         _res = [0.0] * 4
         _res[0] = -_tmp1 * _tmp6 + _tmp10 * _tmp7
         _res[1] = _tmp1 * _tmp12 + _tmp11 * _tmp7
         _res[2] = -_tmp1 * _tmp10 + _tmp6 * _tmp7
         _res[3] = _tmp1 * _tmp11 + _tmp12 * _tmp7
         return Rot3.from_storage(_res)
 
+    @staticmethod
+    def from_angle_axis(angle, axis):
+        # type: (float, numpy.ndarray) -> Rot3
+        """
+        Construct from an angle in radians and a (normalized) axis as a 3-vector.
+        """
+
+        # Total ops: 6
+
+        # Input arrays
+        if axis.shape == (3,):
+            axis = axis.reshape((3, 1))
+        elif axis.shape != (3, 1):
+            raise IndexError(
+                "axis is expected to have shape (3, 1) or (3,); instead had shape {}".format(
+                    axis.shape
+                )
+            )
+
+        # Intermediate terms (2)
+        _tmp0 = (1.0 / 2.0) * angle
+        _tmp1 = math.sin(_tmp0)
+
+        # Output terms
+        _res = [0.0] * 4
+        _res[0] = _tmp1 * axis[0, 0]
+        _res[1] = _tmp1 * axis[1, 0]
+        _res[2] = _tmp1 * axis[2, 0]
+        _res[3] = math.cos(_tmp0)
+        return Rot3.from_storage(_res)
+
+    @staticmethod
+    def from_two_unit_vectors(a, b, epsilon):
+        # type: (numpy.ndarray, numpy.ndarray, float) -> Rot3
+        """
+        Return a rotation that transforms a to b. Both inputs are three-vectors that
+        are expected to be normalized.
+
+        Reference:
+            http://lolengine.net/blog/2013/09/18/beautiful-maths-quaternion-from-vectors
+        """
+
+        # Total ops: 44
+
+        # Input arrays
+        if a.shape == (3,):
+            a = a.reshape((3, 1))
+        elif a.shape != (3, 1):
+            raise IndexError(
+                "a is expected to have shape (3, 1) or (3,); instead had shape {}".format(a.shape)
+            )
+
+        if b.shape == (3,):
+            b = b.reshape((3, 1))
+        elif b.shape != (3, 1):
+            raise IndexError(
+                "b is expected to have shape (3, 1) or (3,); instead had shape {}".format(b.shape)
+            )
+
+        # Intermediate terms (7)
+        _tmp0 = 1.0 / 2.0 - 1.0 / 2.0 * (
+            0.0
+            if a[1, 0] ** 2 + a[2, 0] ** 2 - epsilon ** 2 == 0
+            else math.copysign(1, a[1, 0] ** 2 + a[2, 0] ** 2 - epsilon ** 2)
+        )
+        _tmp1 = a[0, 0] * b[0, 0] + a[1, 0] * b[1, 0] + a[2, 0] * b[2, 0]
+        _tmp2 = (
+            0.0 if -epsilon + abs(_tmp1 + 1) == 0 else math.copysign(1, -epsilon + abs(_tmp1 + 1))
+        ) + 1
+        _tmp3 = (1.0 / 2.0) * _tmp2
+        _tmp4 = 1 - _tmp3
+        _tmp5 = math.sqrt(2 * _tmp1 + epsilon + 2)
+        _tmp6 = _tmp3 / _tmp5
+
+        # Output terms
+        _res = [0.0] * 4
+        _res[0] = _tmp4 * (1 - _tmp0) + _tmp6 * (a[1, 0] * b[2, 0] - a[2, 0] * b[1, 0])
+        _res[1] = _tmp0 * _tmp4 + _tmp6 * (-a[0, 0] * b[2, 0] + a[2, 0] * b[0, 0])
+        _res[2] = _tmp6 * (a[0, 0] * b[1, 0] - a[1, 0] * b[0, 0])
+        _res[3] = (1.0 / 4.0) * _tmp2 * _tmp5
+        return Rot3.from_storage(_res)
+
     # --------------------------------------------------------------------------
     # StorageOps concept
     # --------------------------------------------------------------------------
 
     @staticmethod
     def storage_dim():
         # type: () -> int
```

### Comparing `symforce-sym-0.8.0/sym/spherical_camera_cal.py` & `symforce-sym-0.9.0/sym/spherical_camera_cal.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,43 +9,45 @@
 import numpy
 
 from .ops import spherical_camera_cal as ops
 
 
 class SphericalCameraCal(object):
     """
-    Autogenerated Python implementation of <class 'symforce.cam.spherical_camera_cal.SphericalCameraCal'>.
+    Autogenerated Python implementation of :py:class:`symforce.cam.spherical_camera_cal.SphericalCameraCal`.
 
     Kannala-Brandt camera model, where radial distortion is modeled relative to the 3D angle theta
     off the optical axis as opposed to radius within the image plane (i.e. ATANCamera)
 
     I.e. the radius in the image plane as a function of the angle theta from the camera z-axis is
-    assumed to be given by:
+    assumed to be given by::
 
         r(theta) = theta + d[0] * theta^3 + d[1] * theta^5 + d[2] * theta^7 + d[3] * theta^9
 
     With no tangential coefficients, this model is over-parameterized in that we may scale all the
     distortion coefficients by a constant, and the focal length by the inverse of that constant. To
     fix this issue, we peg the first coefficient at 1. So while the distortion dimension is '4',
     the actual total number of coeffs is 5.
 
     Additionally, the storage for this class includes the critical theta, the maximum angle from the
     optical axis where projection is invertible; although the critical theta is a function of the
     other parameters, this function requires polynomial root finding, so it should be computed
     externally at runtime and set to the computed value.
 
-    Paper:
-    A generic camera model and calibration method for conventional, wide-angle, and fish-eye lenses
-    Kannala, Juho; Brandt, Sami S.
-    PAMI 2006
+    Paper::
+
+        A generic camera model and calibration method for conventional, wide-angle, and fish-eye lenses
+        Kannala, Juho; Brandt, Sami S.
+        PAMI 2006
 
     This is the simpler "P9" model without any non-radially-symmetric distortion params.
 
     The storage for this class is:
-    [ fx fy cx cy critical_theta d0 d1 d2 d3 ]
+
+        [ fx fy cx cy critical_theta d0 d1 d2 d3 ]
     """
 
     __slots__ = ["data"]
 
     # This is because of an issue where mypy doesn't recognize attributes defined in __slots__
     # See https://github.com/python/mypy/issues/5941
     if T.TYPE_CHECKING:
@@ -130,27 +132,27 @@
         return ops.CameraOps.principal_point(self)
 
     def pixel_from_camera_point(self, point, epsilon):
         # type: (SphericalCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
         """
 
         return ops.CameraOps.pixel_from_camera_point(self, point, epsilon)
 
     def pixel_from_camera_point_with_jacobians(self, point, epsilon):
         # type: (SphericalCameraCal, numpy.ndarray, float) -> T.Tuple[numpy.ndarray, float, numpy.ndarray, numpy.ndarray]
         """
         Project a 3D point in the camera frame into 2D pixel coordinates.
 
-        Return:
+        Returns:
             pixel: (x, y) coordinate in pixels if valid
             is_valid: 1 if the operation is within bounds else 0
             pixel_D_cal: Derivative of pixel with respect to intrinsic calibration parameters
             pixel_D_point: Derivative of pixel with respect to point
         """
 
         return ops.CameraOps.pixel_from_camera_point_with_jacobians(self, point, epsilon)
```

### Comparing `symforce-sym-0.8.0/sym/unit3.py` & `symforce-sym-0.9.0/sym/unit3.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,29 +13,31 @@
 
 # isort: split
 from .ops import unit3 as ops
 
 
 class Unit3(object):
     """
-    Autogenerated Python implementation of <class 'symforce.geo.unit3.Unit3'>.
+    Autogenerated Python implementation of :py:class:`symforce.geo.unit3.Unit3`.
+
+    Direction in R^3, represented as a :class:`Rot3 <symforce.geo.rot3.Rot3>` that transforms
+    [0, 0, 1] to the desired direction.
 
-    Direction in R^3, represented as a Rot3 that transforms [0, 0, 1] to the desired direction.
     The storage is therefore a quaternion and the tangent space is 2 dimensional.
-    Most operations are implemented using operations from Rot3.
+    Most operations are implemented using operations from :class:`Rot3 <symforce.geo.rot3.Rot3>`.
 
     Note: an alternative implementation could directly store a unit vector and define its boxplus
     manifold as described in Appendix B.2 of [Hertzberg 2013]. This can be done by finding the
     Householder reflector of x and use it to transform the exponential map of delta, which is a
-    small perturbation in the tangent space (R^2). Namely,
+    small perturbation in the tangent space (R^2). Namely::
 
-    x.retract(delta) = x [+] delta = Rx * Exp(delta), where
-    Exp(delta) = [sinc(||delta||) * delta, cos(||delta||)], and
-    Rx = (I - 2 vv^T / (v^Tv))X, v = x - e_z != 0, X is a matrix negating 2nd vector component
-       = I                     , x = e_z
+        x.retract(delta) = x [+] delta = Rx * Exp(delta), where
+        Exp(delta) = [sinc(||delta||) * delta, cos(||delta||)], and
+        Rx = (I - 2 vv^T / (v^Tv))X, v = x - e_z != 0, X is a matrix negating 2nd vector component
+        = I                     , x = e_z
 
     [Hertzberg 2013] Integrating Generic Sensor Fusion Algorithms with Sound State Representations
     through Encapsulation of Manifolds
     """
 
     __slots__ = ["data"]
 
@@ -58,16 +60,17 @@
     # Custom generated methods
     # --------------------------------------------------------------------------
 
     @staticmethod
     def from_vector(a, epsilon):
         # type: (numpy.ndarray, float) -> Unit3
         """
-        Return a Unit3 that points along the direction of vector a. a does not have to be a unit
-        vector.
+        Return a :class:`Unit3` that points along the direction of vector ``a``
+
+        ``a`` does not have to be a unit vector.
         """
 
         # Total ops: 35
 
         # Input arrays
         if a.shape == (3,):
             a = a.reshape((3, 1))
```

### Comparing `symforce-sym-0.8.0/symforce_sym.egg-info/SOURCES.txt` & `symforce-sym-0.9.0/symforce_sym.egg-info/SOURCES.txt`

 * *Files identical despite different names*

