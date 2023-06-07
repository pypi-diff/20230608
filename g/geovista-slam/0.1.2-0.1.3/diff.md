# Comparing `tmp/geovista-slam-0.1.2.tar.gz` & `tmp/geovista-slam-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovista-slam-0.1.2.tar", last modified: Fri Apr 21 16:25:34 2023, max compression
+gzip compressed data, was "geovista-slam-0.1.3.tar", last modified: Wed Jun  7 22:30:57 2023, max compression
```

## Comparing `geovista-slam-0.1.2.tar` & `geovista-slam-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.560565 geovista-slam-0.1.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/issue.md
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      525 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/workflows/ci-citation.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/workflows/ci-locks.yml
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/workflows/ci-manifest.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4066 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/.github/workflows/ci-wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7475 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.560565 geovista-slam-0.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/src/geovista_slam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8519 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/geovista_slam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/geovista_slam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/geovista_slam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/geovista_slam.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/geovista_slam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/geovista_slam.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:25:34.564565 geovista-slam-0.1.2/src/slam/
--rw-r--r--   0 runner    (1001) docker     (123)    21728 2023-04-21 16:25:24.000000 geovista-slam-0.1.2/src/slam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 16:25:34.000000 geovista-slam-0.1.2/src/slam/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/issue.md
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      525 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/workflows/ci-citation.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4019 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/workflows/ci-locks.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/workflows/ci-manifest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/.github/workflows/ci-wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     5488 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9597 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2559 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.837831 geovista-slam-0.1.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/src/geovista_slam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/geovista_slam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/geovista_slam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/geovista_slam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/geovista_slam.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/geovista_slam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/geovista_slam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:30:57.841831 geovista-slam-0.1.3/src/slam/
+-rw-r--r--   0 runner    (1001) docker     (123)    21744 2023-06-07 22:30:48.000000 geovista-slam-0.1.3/src/slam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-07 22:30:57.000000 geovista-slam-0.1.3/src/slam/_version.py
```

### Comparing `geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/bug-report.md` & `geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.2/.github/ISSUE_TEMPLATE/feature-request.md` & `geovista-slam-0.1.3/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.2/.github/workflows/ci-citation.yml` & `geovista-slam-0.1.3/.github/workflows/ci-citation.yml`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.2/.github/workflows/ci-locks.yml` & `geovista-slam-0.1.3/.github/workflows/ci-locks.yml`

 * *Files 1% similar despite different names*

```diff
@@ -92,15 +92,15 @@
       id: generate-token
       with:
         app_id: ${{ secrets.AUTH_APP_ID }}
         private_key: ${{ secrets.AUTH_APP_PRIVATE_KEY }}
 
     - name: "generate pull-request"
       id: cpr
-      uses: peter-evans/create-pull-request@5b4a9f6a9e2af26e5f02351490b90d01eb8ec1e5
+      uses: peter-evans/create-pull-request@284f54f989303d2699d373481a0cfa13ad5a6666
       with:
         token: ${{ steps.generate-token.outputs.token }}
         add-paths: ${{ github.workspace }}/requirements/locks/*.txt
         commit-message: "updated conda lock files"
         branch: conda-lock-auto-update
         delete-branch: true
         title: "[geovista.ci] conda lock auto-update"
```

### Comparing `geovista-slam-0.1.2/.github/workflows/ci-manifest.yml` & `geovista-slam-0.1.3/.github/workflows/ci-manifest.yml`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 # Reference:
 #   - https://github.com/actions/checkout
 
 name: ci-manifest
 
 on:
   pull_request:
-    branches:
-      - "*"
 
   push:
-    branches-ignore:
-      - "conda-lock-auto-update"
-      - "pre-commit-ci-update-config"
-      - "dependabot/*"
+    branches:
+      - "main"
+      - "v*x"
+      - "!conda-lock-auto-update"
+      - "!pre-commit-ci-update-config"
+      - "!dependabot/*"
+    tags:
+      - "v*"
 
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
```

### Comparing `geovista-slam-0.1.2/.github/workflows/ci-wheels.yml` & `geovista-slam-0.1.3/.github/workflows/ci-wheels.yml`

 * *Files 3% similar despite different names*

```diff
@@ -8,24 +8,24 @@
 #   - https://github.com/pypa/gh-action-pypi-publish
 #   - https://test.pypi.org/help/#apitoken
 
 name: ci-wheels
 
 on:
   pull_request:
-    branches:
-      - "*"
 
   push:
+    branches:
+      - "main"
+      - "v*x"
+      - "!conda-lock-auto-update"
+      - "!pre-commit-ci-update-config"
+      - "!dependabot/*"
     tags:
       - "v*"
-    branches-ignore:
-      - "conda-lock-auto-update"
-      - "pre-commit-ci-update-config"
-      - "dependabot/*"
 
   workflow_dispatch:
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
```

### Comparing `geovista-slam-0.1.2/CODE_OF_CONDUCT.md` & `geovista-slam-0.1.3/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.2/LICENSE` & `geovista-slam-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.2/pyproject.toml` & `geovista-slam-0.1.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -20,20 +20,19 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering :: Atmospheric Science",
 ]
-description = "Structured Local Area Model"
 dependencies = [
-    "appdirs",
-    "geovista",
-    "scitools-iris",
+    "geovista>=0.2",
+    "scitools-iris>=3.2",
 ]
+description = "Structured Local Area Model"
 dynamic = [
     "readme",
     "version",
 ]
 keywords = [
     "curvilinear",
     "earth-science",
```

### Comparing `geovista-slam-0.1.2/src/geovista_slam.egg-info/SOURCES.txt` & `geovista-slam-0.1.3/src/geovista_slam.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `geovista-slam-0.1.2/src/slam/__init__.py` & `geovista-slam-0.1.3/src/slam/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from copy import deepcopy
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import Any, Union
 import warnings
 
 import geovista as gv
-from geovista.common import to_xy0, wrap
+from geovista.common import from_cartesian, wrap
 from geovista.crs import WGS84
 from iris.coord_systems import CoordSystem
 from iris.coords import AuxCoord, DimCoord
 from iris.cube import Cube
 import numpy as np
 from pyvista import PolyData, UnstructuredGrid
 
@@ -409,15 +409,15 @@
         else:
             src_crs = src_crs.as_cartopy_crs()
 
         coords = ucube.mesh.face_coords
 
         if coords is None:
             face_centers = mesh.cell_centers()
-            xy0 = to_xy0(face_centers, stacked=False)
+            xy0 = from_cartesian(face_centers, stacked=False)
             face_x, face_y = xy0[0], xy0[1]
         else:
             face_x, face_y = coords.face_x.points, coords.face_y.points
 
         if crs is not None:
             transformed = crs.as_cartopy_crs().transform_points(src_crs, face_x, face_y)
             if decimals is not None:
```

