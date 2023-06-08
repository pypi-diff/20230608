# Comparing `tmp/extremitypathfinder-2.6.0.tar.gz` & `tmp/extremitypathfinder-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "extremitypathfinder-2.6.0.tar", max compression
+gzip compressed data, was "extremitypathfinder-2.7.0.tar", max compression
```

## Comparing `extremitypathfinder-2.6.0.tar` & `extremitypathfinder-2.7.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
--rw-r--r--   0        0        0      200 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/.editorconfig
--rw-r--r--   0        0        0     2043 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0     4627 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/CHANGELOG.rst
--rw-r--r--   0        0        0     3091 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1056 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/LICENSE
--rw-r--r--   0        0        0      759 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/Makefile
--rw-r--r--   0        0        0     2447 2023-06-04 21:05:39.698239 extremitypathfinder-2.6.0/README.rst
--rw-r--r--   0        0        0      574 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/example.json
--rw-r--r--   0        0        0      132 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/__init__.py
--rw-r--r--   0        0        0     2234 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/command_line.py
--rw-r--r--   0        0        0      151 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/configs.py
--rw-r--r--   0        0        0    14688 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/extremitypathfinder.py
--rw-r--r--   0        0        0     6902 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/plotting.py
--rw-r--r--   0        0        0      379 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/types.py
--rw-r--r--   0        0        0    51145 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/extremitypathfinder/utils.py
--rw-r--r--   0        0        0     1906 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/__init__.py
--rw-r--r--   0        0        0      580 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/cli_test.py
--rwxr-xr-x   0        0        0     6914 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/helper_fcts_test.py
--rwxr-xr-x   0        0        0      839 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/helpers.py
--rwxr-xr-x   0        0        0     7351 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/main_test.py
--rw-r--r--   0        0        0    10817 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/test_cases.py
--rw-r--r--   0        0        0    12701 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tests/test_find_visible.py
--rwxr-xr-x   0        0        0      318 2023-06-04 21:05:39.710240 extremitypathfinder-2.6.0/tox.ini
--rw-r--r--   0        0        0     3971 1970-01-01 00:00:00.000000 extremitypathfinder-2.6.0/PKG-INFO
+-rw-r--r--   0        0        0      200 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/.editorconfig
+-rw-r--r--   0        0        0     2043 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0     4782 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     3091 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1056 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/LICENSE
+-rw-r--r--   0        0        0      772 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/Makefile
+-rw-r--r--   0        0        0     2532 2023-06-08 10:11:45.720013 extremitypathfinder-2.7.0/README.rst
+-rw-r--r--   0        0        0      574 2023-06-08 10:11:45.728013 extremitypathfinder-2.7.0/example.json
+-rw-r--r--   0        0        0      132 2023-06-08 10:11:45.728013 extremitypathfinder-2.7.0/extremitypathfinder/__init__.py
+-rw-r--r--   0        0        0     2234 2023-06-08 10:11:45.728013 extremitypathfinder-2.7.0/extremitypathfinder/command_line.py
+-rw-r--r--   0        0        0      198 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/configs.py
+-rw-r--r--   0        0        0    14841 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/extremitypathfinder.py
+-rw-r--r--   0        0        0      833 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/numba_replacements.py
+-rw-r--r--   0        0        0     6902 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/plotting.py
+-rw-r--r--   0        0        0      379 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/types.py
+-rw-r--r--   0        0        0    44457 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/utils.py
+-rw-r--r--   0        0        0     7133 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/extremitypathfinder/utils_numba.py
+-rw-r--r--   0        0        0     1970 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      580 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/cli_test.py
+-rwxr-xr-x   0        0        0     7211 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/helper_fcts_test.py
+-rwxr-xr-x   0        0        0      839 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/helpers.py
+-rwxr-xr-x   0        0        0     7351 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/main_test.py
+-rw-r--r--   0        0        0    10817 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/test_cases.py
+-rw-r--r--   0        0        0    12624 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tests/test_find_visible.py
+-rwxr-xr-x   0        0        0      499 2023-06-08 10:11:45.732013 extremitypathfinder-2.7.0/tox.ini
+-rw-r--r--   0        0        0     4137 1970-01-01 00:00:00.000000 extremitypathfinder-2.7.0/PKG-INFO
```

### Comparing `extremitypathfinder-2.6.0/.pre-commit-config.yaml` & `extremitypathfinder-2.7.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/CHANGELOG.rst` & `extremitypathfinder-2.7.0/CHANGELOG.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,18 @@
 Changelog
 =========
 
+
+2.7.0 (2023-06-08)
+-------------------
+
+- optional Numba JIT compilation offering significant speedup
+- extra: `pip install extremitypathfinder[numba]`
+
+
 2.6.0 (2023-06-04)
 -------------------
 
 internal:
 
 * implemented an optimised visibility graph algorithm: sort edges and candidates after their representation to always only check the relevant fraction of candidates for each edge. Runtime complexity O(n^2 log_2 n).
 * added visibility computation tests
```

### Comparing `extremitypathfinder-2.6.0/CONTRIBUTING.rst` & `extremitypathfinder-2.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/LICENSE` & `extremitypathfinder-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/Makefile` & `extremitypathfinder-2.7.0/Makefile`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 install:
 	@echo "installing the development dependencies..."
-	@poetry install
+	@poetry install --all-extras
 	@#poetry install --no-dev
 
 
 update:
 	@echo "updating the dependencies pinned in 'pyproject.toml':"
 	@poetry update -vvv
 	#poetry export -f requirements.txt --output docs/requirements.txt --without-hashes
```

### Comparing `extremitypathfinder-2.6.0/README.rst` & `extremitypathfinder-2.7.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -35,17 +35,19 @@
 
 
 .. image:: ./docs/_static/title_demo_plot.png
 
 
 Quick Guide:
 
+Install the package with the optional Numba extra for a significant speedup:
+
 .. code-block:: console
 
-    pip install extremitypathfinder
+    pip install extremitypathfinder[numba]
 
 
 .. code-block:: python
 
     from extremitypathfinder import PolygonEnvironment
 
     environment = PolygonEnvironment()
```

### Comparing `extremitypathfinder-2.6.0/example.json` & `extremitypathfinder-2.7.0/example.json`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/extremitypathfinder/command_line.py` & `extremitypathfinder-2.7.0/extremitypathfinder/command_line.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/extremitypathfinder/extremitypathfinder.py` & `extremitypathfinder-2.7.0/extremitypathfinder/extremitypathfinder.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import pickle
 import warnings
 from typing import Dict, Iterable, List, Optional, Set, Tuple
 
 import networkx as nx
 import numpy as np
 
+from extremitypathfinder import configs
 from extremitypathfinder import types as t
 from extremitypathfinder import utils
 from extremitypathfinder.configs import DEFAULT_PICKLE_NAME
 from extremitypathfinder.types import InputCoord, InputCoordList, Length, ObstacleIterator, Path
 
 
 class PolygonEnvironment:
@@ -23,15 +24,15 @@
 
     TODO document parameters
     """
 
     nr_edges: int
     prepared: bool = False
     holes: List[np.ndarray]
-    extremity_indices: List[int]
+    extremity_indices: np.ndarray
     reprs_n_distances: Dict[int, np.ndarray]
     graph: t.Graph
     # TODO
     temp_graph: Optional[t.Graph] = None  # for storing and plotting the graph during a query
     boundary_polygon: np.ndarray
     coords: np.ndarray
     edge_vertex_idxs: np.ndarray
@@ -73,34 +74,37 @@
         :param list_of_hole_coordinates: array of coordinates with clockwise edge numbering
         :param validate: whether the requirements of the data should be tested
 
         :raises AssertionError: when validate=True and the input is invalid.
         """
         self.prepared = False
         # loading the map
-        boundary_coordinates = np.array(boundary_coordinates, dtype=float)
-        list_of_hole_coordinates = [np.array(hole_coords, dtype=float) for hole_coords in list_of_hole_coordinates]
+        boundary_coordinates = np.array(boundary_coordinates, dtype=configs.DTYPE_FLOAT)
+        list_of_hole_coordinates = [
+            np.array(hole_coords, dtype=configs.DTYPE_FLOAT) for hole_coords in list_of_hole_coordinates
+        ]
         if validate:
             utils.check_data_requirements(boundary_coordinates, list_of_hole_coordinates)
 
         # Note: independent copy!
         self.holes = list_of_hole_coordinates
         self.boundary_polygon = boundary_coordinates
 
+        # TODO redundant data. refactor all functions to only use one format
         (
             self.coords,
             self.extremity_indices,
             self.extremity_mask,
             self.vertex_edge_idxs,
             self.edge_vertex_idxs,
-        ) = utils.compile_boundary_data_fr_polys(boundary_coordinates, list_of_hole_coordinates)
+        ) = utils.compile_polygon_datastructs(boundary_coordinates, list_of_hole_coordinates)
 
         nr_total_pts = self.edge_vertex_idxs.shape[0]
         self.nr_vertices = nr_total_pts
-        self.reprs_n_distances = {i: utils.cmp_reps_n_distances(i, self.coords) for i in self.extremity_indices}
+        self.reprs_n_distances = utils.cmp_reps_n_distance_dict(self.coords, self.extremity_indices)
 
         # start and goal points will be stored after all polygon coordinates
         self.idx_start = nr_total_pts
         self.idx_goal = nr_total_pts + 1
 
         self.prepare()
```

### Comparing `extremitypathfinder-2.6.0/extremitypathfinder/plotting.py` & `extremitypathfinder-2.7.0/extremitypathfinder/plotting.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/extremitypathfinder/utils.py` & `extremitypathfinder-2.7.0/extremitypathfinder/utils.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,164 +1,54 @@
 import itertools
 import json
-import math
 import pickle
 from itertools import combinations
-from typing import Dict, Iterable, List, Optional, Set, Tuple
+from typing import Dict, Iterable, List, Set, Tuple
 
 import networkx as nx
 import numpy as np
 import numpy.linalg
 
+from extremitypathfinder import configs
 from extremitypathfinder import types as t
 from extremitypathfinder.configs import BOUNDARY_JSON_KEY, DEFAULT_PICKLE_NAME, HOLES_JSON_KEY
-
-
-def _compute_repr_n_dist(np_vector: np.ndarray) -> Tuple[float, float]:
-    """computing representation for the angle from the origin to a given vector
-
-    value in [0.0 : 4.0[
-    every quadrant contains angle measures from 0.0 to 1.0
-    there are 4 quadrants (counterclockwise numbering)
-    0 / 360 degree -> 0.0
-    90 degree -> 1.0
-    180 degree -> 2.0
-    270 degree -> 3.0
-    ...
-    Useful for comparing angles without actually computing expensive trigonometrical functions
-    This representation does not grow directly proportional to its represented angle,
-    but it its bijective and monotonous:
-    rep(p1) > rep(p2) <=> angle(p1) > angle(p2)
-    rep(p1) = rep(p2) <=> angle(p1) = angle(p2)
-    angle(p): counterclockwise angle between the two line segments (0,0)'--(1,0)' and (0,0)'--p
-    with (0,0)' being the vector representing the origin
-
-    :param np_vector:
-    :return:
-    """
-    dx, dy = np_vector
-    distance = math.sqrt(dx**2 + dy**2)  # l-2 norm
-    if distance == 0.0:
-        angle_measure = np.nan
-    else:
-        # 2D vector: (dx, dy) = np_vector
-        dx_positive = dx >= 0
-        dy_positive = dy >= 0
-
-        if dx_positive and dy_positive:
-            quadrant = 0.0
-            angle_measure = dy
-
-        elif not dx_positive and dy_positive:
-            quadrant = 1.0
-            angle_measure = -dx
-
-        elif not dx_positive and not dy_positive:
-            quadrant = 2.0
-            angle_measure = -dy
-
-        else:
-            quadrant = 3.0
-            angle_measure = dx
-
-        # normalise angle measure to [0; 1]
-        angle_measure /= distance
-        angle_measure += quadrant
-
-    return angle_measure, distance
+from extremitypathfinder.utils_numba import (
+    _angle_rep_inverse,
+    _compute_repr_n_dist,
+    _fill_edge_vertex_idxs,
+    _fill_extremity_mask,
+    _has_clockwise_numbering,
+    _inside_polygon,
+    _no_identical_consequent_vertices,
+)
 
 
 def cmp_reps_n_distances(orig_idx: int, coords: np.ndarray) -> np.ndarray:
     coords_orig = coords[orig_idx]
     coords_translated = coords - coords_orig
     repr_n_dists = np.apply_along_axis(_compute_repr_n_dist, axis=1, arr=coords_translated)
     return repr_n_dists.T
 
 
-def _inside_polygon(p: np.ndarray, coords: np.ndarray, border_value: bool) -> bool:
-    # should return the border value for point equal to any polygon vertex
-    # TODO overflow possible with large values when comparing slopes, change procedure
-    # and if the point p lies on any polygon edge
-    p1 = coords[-1, :]
-    for p2 in coords[:]:
-        if np.array_equal(p2, p):
-            return border_value
-        rep_p1_p, _ = _compute_repr_n_dist(p1 - p)
-        rep_p2_p, _ = _compute_repr_n_dist(p2 - p)
-        if abs(rep_p1_p - rep_p2_p) == 2.0:
-            return border_value
-        p1 = p2
-
-    # regular point in polygon algorithm: ray casting
-    x, y = p
-    x_coords = coords[:, 0]
-    y_coords = coords[:, 1]
-    nr_coords = len(x_coords)
-    inside = False
-
-    # the edge from the last to the first point is checked first
-    y1 = y_coords[-1]
-    y_gt_y1 = y > y1
-    for i in range(nr_coords):
-        y2 = y_coords[i]
-        y_gt_y2 = y > y2
-        if y_gt_y1 ^ y_gt_y2:  # XOR
-            # [p1-p2] crosses horizontal line in p
-            x1 = x_coords[i - 1]
-            x2 = x_coords[i]
-            # only count crossings "right" of the point ( >= x)
-            x_le_x1 = x <= x1
-            x_le_x2 = x <= x2
-            if x_le_x1 or x_le_x2:
-                if x_le_x1 and x_le_x2:
-                    # p1 and p2 are both to the right -> valid crossing
-                    inside = not inside
-                else:
-                    # compare the slope of the line [p1-p2] and [p-p2]
-                    # depending on the position of p2 this determines whether
-                    # the polygon edge is right or left of the point
-                    # to avoid expensive division the divisors (of the slope dy/dx) are brought to the other side
-                    # ( dy/dx > a  ==  dy > a * dx )
-                    # only one of the points is to the right
-                    slope1 = (y2 - y) * (x2 - x1)
-                    slope2 = (y2 - y1) * (x2 - x)
-                    # NOTE: accept slope equality to also detect if p lies directly on an edge
-                    if y_gt_y1:
-                        if slope1 <= slope2:
-                            inside = not inside
-                    elif slope1 >= slope2:  # NOT y_gt_y1
-                        inside = not inside
-
-        # next point
-        y1 = y2
-        y_gt_y1 = y_gt_y2
-
-    return inside
+def cmp_reps_n_distance_dict(coords: np.ndarray, extremity_indices: np.ndarray) -> Dict[int, np.ndarray]:
+    # Note: distance and angle representation relation are symmetric,
+    # but exploiting this has been found to be slower than using the numpy functionality with slight overhead
+    reps_n_distance_dict = {i: cmp_reps_n_distances(i, coords) for i in extremity_indices}
+    return reps_n_distance_dict
 
 
 def is_within_map(p: np.ndarray, boundary: np.ndarray, holes: Iterable[np.ndarray]) -> bool:
     if not _inside_polygon(p, boundary, border_value=True):
         return False
     for hole in holes:
         if _inside_polygon(p, hole, border_value=False):
             return False
     return True
 
 
-def _no_identical_consequent_vertices(coords):
-    p1 = coords[-1]
-    for p2 in coords:
-        # TODO adjust allowed difference: rtol, atol
-        if np.array_equal(p1, p2):
-            return False
-        p1 = p2
-
-    return True
-
-
 def _get_intersection_status(p1, p2, q1, q2):
     # return:
     #   0: no intersection
     #   1: intersection in ]p1;p2[
     # TODO support 2 remaining possibilities
     #   2: intersection directly in p1 or p2
     #   3: intersection directly in q1 or q2
@@ -238,32 +128,14 @@
         # print(p1, p2, q1, q2)
 
     # TODO check for intersections across 2 edges! use computed intersection
 
     return True
 
 
-def _has_clockwise_numbering(coords: np.ndarray) -> bool:
-    """tests if a polygon has clockwise vertex numbering
-    approach: Sum over the edges, (x2 − x1)(y2 + y1). If the result is positive the curve is clockwise.
-    from:
-    https://stackoverflow.com/questions/1165647/how-to-determine-if-a-list-of-polygon-points-are-in-clockwise-order
-    :param coords: the list of (x,y) coordinates representing the polygon to be tested
-    :return: true if the polygon has been given in clockwise numbering
-    """
-    total_sum = 0.0
-    p1 = coords[-1]
-    for p2 in coords:
-        x1, y1 = p1
-        x2, y2 = p2
-        total_sum += (x2 - x1) * (y2 + y1)
-        p1 = p2
-    return total_sum > 0
-
-
 def _check_polygon(polygon):
     """ensures that all the following conditions on the polygons are fulfilled:
     - must at least contain 3 vertices
     - no consequent vertices with identical coordinates in the polygons! In general might have the same coordinates
     - a polygon must not have self intersections (intersections with other polygons are allowed)
     """
     if not polygon.shape[0] >= 3:
@@ -279,18 +151,14 @@
 def check_data_requirements(boundary_coords: np.ndarray, list_hole_coords: List[np.ndarray]):
     """ensures that all the following conditions on the polygons are fulfilled:
         - basic polygon requirements (s. above)
         - edge numbering has to follow this convention (for easier computations):
             * outer boundary polygon: counter clockwise
             * holes: clockwise
 
-    TODO test
-    todo - polygons must not intersect each other
-    TODO data rectification
-
     :param boundary_coords:
     :param list_hole_coords:
     :return:
     """
     _check_polygon(boundary_coords)
     if _has_clockwise_numbering(boundary_coords):
         raise ValueError("Vertex numbering of the boundary polygon must be counter clockwise.")
@@ -361,65 +229,14 @@
             res = not res
         return res
 
     idxs_within = {i for i in candidate_idxs if within_filter_func(representations[i])}
     return idxs_within
 
 
-def lies_within_range(
-    repr1: float,
-    repr2: float,
-    repr: float,
-    angle_range_less_180: bool,
-    equal_repr_allowed: bool,
-) -> bool:
-    """
-    filters out all vertices whose representation lies within the range between
-      the two given angle representations
-    which range ('clockwise' or 'counter-clockwise') should be checked is determined by:
-      - query angle (range) is < 180deg or not (>= 180deg)
-    :param repr1:
-    :param repr2:
-    :param candidate_idxs:
-    :param angle_range_less_180: whether the angle between repr1 and repr2 is < 180 deg
-    :param equal_repr_allowed: whether vertices with the same representation should also be returned
-    :param representations:
-    :return:
-    """
-    eq_repr = (repr == repr1) or (repr == repr2)
-    if eq_repr:
-        return equal_repr_allowed
-
-    min_repr = min(repr1, repr2)
-    max_repr = max(repr1, repr2)  # = min_angle + angle_diff
-
-    # Note: vertices with the same representation will NOT be returned!
-    res = min_repr < repr < max_repr
-
-    # depending on the angle, the included range is clockwise or anti-clockwise
-    # (from min_repr to max_val or the other way around)
-    # when the range contains the 0.0 value (transition from 3.99... -> 0.0)
-    # it is easier to check if a representation does NOT lie within this range
-    # -> invert filter condition
-    # special case: angle == 180deg <-> lies on the line
-    repr_diff = max_repr - min_repr
-    on_line_inv = repr_diff == 2.0 and repr1 >= repr2
-    # which range to filter is determined by the order of the points
-    # since the polygons follow a numbering convention,
-    # the 'left' side of p1-p2 always lies inside the map
-    # -> filter out everything on the right side (='outside')
-    # ^: XOR
-    inversion_condition = on_line_inv or ((repr_diff < 2.0) ^ angle_range_less_180)
-
-    if inversion_condition:
-        res = not res
-
-    return res
-
-
 def get_neighbour_idxs(i: int, vertex_edge_idxs: np.ndarray, edge_vertex_idxs: np.ndarray) -> Tuple[int, int]:
     edge_idx1, edge_idx2 = vertex_edge_idxs[i]
     neigh_idx1 = edge_vertex_idxs[edge_idx1, 0]
     neigh_idx2 = edge_vertex_idxs[edge_idx2, 1]
     return neigh_idx1, neigh_idx2
 
 
@@ -464,15 +281,14 @@
     if nr_candidates_total == 0:
         return candidates
     # TODO immutable
     # eliminate candidates with equal representations: only keep the closest (min dist)
     candidates_sorted = _eliminate_eq_candidates(candidates, distances, representations)
     print(candidates_sorted)
 
-    # TODO test
     (
         crossing_edges,
         edges_is_crossing,
         edges_max_dist,
         edges_max_rep,
         edges_min_rep,
         non_crossing_edges,
@@ -1200,23 +1016,15 @@
             pass
 
         hole_list.append(hole)
 
     return boundary_edges, hole_list
 
 
-def _angle_rep_inverse(repr: Optional[float]) -> Optional[float]:
-    if repr is None:
-        repr_inv = None
-    else:
-        repr_inv = (repr + 2.0) % 4.0
-    return repr_inv
-
-
-def _compute_extremity_idxs(coordinates: np.ndarray) -> List[int]:
+def _cmp_extremity_mask(coordinates: np.ndarray) -> np.ndarray:
     """identify all protruding points = vertices with an inside angle of > 180 degree ('extremities')
     expected edge numbering:
         outer boundary polygon: counterclockwise
         holes: clockwise
 
     basic idea:
       - translate the coordinate system to have p2 as origin
@@ -1226,78 +1034,60 @@
     %4 because the quadrant has to be in [0,1,2,3] (representation in [0:4[)
     if the representation lies within quadrant 0 or 1 (<2.0), the inside angle
       (for boundary polygon inside, for holes outside) between p1p2p3 is > 180 degree
     then p2 = extremity
     :param coordinates:
     :return:
     """
-    nr_coordinates = len(coordinates)
-    extr_idxs = []
-    p1 = coordinates[-2]
-    p2 = coordinates[-1]
-    for i, p3 in enumerate(coordinates):
-        # since consequent vertices are not permitted to be equal,
-        #   the angle representation of the difference is well-defined
-        diff_p3_p2 = p3 - p2
-        diff_p1_p2 = p1 - p2
-        repr_p3_p2, _ = _compute_repr_n_dist(diff_p3_p2)
-        repr_p1_p2, _ = _compute_repr_n_dist(diff_p1_p2)
-        rep_diff = repr_p3_p2 - repr_p1_p2
-        if rep_diff % 4.0 < 2.0:  # inside angle > 180 degree
-            # p2 is an extremity
-            idx_p2 = (i - 1) % nr_coordinates
-            extr_idxs.append(idx_p2)
-
-        # move to the next point
-        p1 = p2
-        p2 = p3
-    return extr_idxs
-
+    extremity_mask = np.full(len(coordinates), False, dtype=bool)
+    _fill_extremity_mask(coordinates, extremity_mask)
+    return extremity_mask
+
+
+def _cmp_extremities(list_of_polygons, coords, boundary_coordinates, list_of_hole_coordinates):
+    extremity_masks = [_cmp_extremity_mask(coords_poly) for coords_poly in list_of_polygons]
+    extremity_mask = np.concatenate(extremity_masks, axis=0, dtype=bool)
+    # Attention: since polygons are allowed to overlap, only consider extremities that are actually within the map
+    for extremity_idx in np.where(extremity_mask)[0]:
+        extrimity_coords = coords[extremity_idx]
+        if not is_within_map(extrimity_coords, boundary_coordinates, list_of_hole_coordinates):
+            extremity_mask[extremity_idx] = False
+    extremity_indices = np.where(extremity_mask)[0]
+    return extremity_indices, extremity_mask
+
+
+def _cmp_edge_vertex_idxs(coordinates: np.ndarray) -> Tuple[np.ndarray, np.ndarray]:
+    nr_coords = len(coordinates)
+    edge_vertex_idxs = np.empty((nr_coords, 2), dtype=int)
+    vertex_edge_idxs = np.empty((nr_coords, 2), dtype=int)
+    _fill_edge_vertex_idxs(edge_vertex_idxs, vertex_edge_idxs)
+    return edge_vertex_idxs, vertex_edge_idxs
 
-def load_pickle(path=DEFAULT_PICKLE_NAME):
-    print("loading map from:", path)
-    with open(path, "rb") as f:
-        return pickle.load(f)
 
+def _cmp_edge_and_vertex_idxs(list_of_polygons):
+    # compute edge and vertex indices from polygon data structure
+    edge_and_vertex_indices = [_cmp_edge_vertex_idxs(coords_poly) for coords_poly in list_of_polygons]
+    offset = 0
+    for edge_vertex_idxs, vertex_edge_idxs in edge_and_vertex_indices:
+        edge_vertex_idxs += offset
+        vertex_edge_idxs += offset
+        offset += len(edge_vertex_idxs)
+    edge_vertex_idxs, vertex_edge_idxs = zip(*edge_and_vertex_indices)
+    edge_vertex_idxs = np.concatenate(edge_vertex_idxs, axis=0)
+    vertex_edge_idxs = np.concatenate(vertex_edge_idxs, axis=0)
+    return edge_vertex_idxs, vertex_edge_idxs
 
-def compile_boundary_data_fr_polys(boundary_coordinates, list_of_hole_coordinates):
-    def within_map(coord):
-        return is_within_map(coord, boundary_coordinates, list_of_hole_coordinates)
 
+def compile_polygon_datastructs(boundary_coordinates: np.ndarray, list_of_hole_coordinates: List[np.ndarray]):
     list_of_polygons = [boundary_coordinates] + list_of_hole_coordinates
-    nr_total_pts = sum(map(len, list_of_polygons))
-
-    # compute edge and vertex indices from polygon data structure
-    vertex_edge_idxs = np.empty((nr_total_pts, 2), dtype=int)
-    # TODO required? inverse of the other. get_neighbours function
-    edge_vertex_idxs = np.empty((nr_total_pts, 2), dtype=int)
-    edge_idx = 0
-    offset = 0
-    extremity_indices = set()
-    for poly in list_of_polygons:
-        poly_extr_idxs = _compute_extremity_idxs(poly)
-        poly_extr_idxs = {i + offset for i in poly_extr_idxs}
-        extremity_indices |= poly_extr_idxs
-
-        nr_coords = len(poly)
-        v1 = -1 % nr_coords
-        # TODO col 1 is just np.arange?!
-        for v2 in range(nr_coords):
-            v1_idx = v1 + offset
-            v2_idx = v2 + offset
-            edge_vertex_idxs[edge_idx, 0] = v1_idx
-            edge_vertex_idxs[edge_idx, 1] = v2_idx
-            vertex_edge_idxs[v1_idx, 1] = edge_idx
-            vertex_edge_idxs[v2_idx, 0] = edge_idx
-            # move to the next vertex/edge
-            v1 = v2
-            edge_idx += 1
-
-        offset = edge_idx
-
-    coords = np.concatenate(list_of_polygons, axis=0)
-    # Attention: only consider extremities that are actually within the map (polygons are allowed to overlap)
-    extremity_indices = [i for i in extremity_indices if within_map(coords[i])]
-    extremity_mask = np.full(nr_total_pts, False, dtype=bool)
-    for i in extremity_indices:
-        extremity_mask[i] = True
+    coords = np.concatenate(list_of_polygons, axis=0, dtype=configs.DTYPE_FLOAT)
+    edge_vertex_idxs, vertex_edge_idxs = _cmp_edge_and_vertex_idxs(list_of_polygons)
+    extremity_indices, extremity_mask = _cmp_extremities(
+        list_of_polygons, coords, boundary_coordinates, list_of_hole_coordinates
+    )
     return coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs
+
+
+def load_pickle(path=DEFAULT_PICKLE_NAME):
+    print("loading map from:", path)
+    with open(path, "rb") as f:
+        return pickle.load(f)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `extremitypathfinder-2.6.0/pyproject.toml` & `extremitypathfinder-2.7.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "extremitypathfinder"
-version = "2.6.0"
+version = "2.7.0"
 license = "MIT"
 readme = "README.rst"
 repository = "https://github.com/jannikmi/extremitypathfinder"
 homepage = "https://extremitypathfinder.readthedocs.io/en/latest/"
 documentation = "https://extremitypathfinder.readthedocs.io/en/latest/"
 keywords = ["path-planning", "path-finding", "shortest-path", "visibility", "graph", "polygon", "grid", "map", "robotics", "navigation", "offline"]
 classifiers = [
@@ -38,14 +38,15 @@
 [tool.poetry.scripts]
 extremitypathfinder = "extremitypathfinder.command_line:main"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 numpy = "^1.22"
 networkx = "^3"
+numba = {version = "^0.56.0", optional = true}
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "*"
 
 [tool.poetry.group.plot.dependencies]
 matplotlib = "*"
 
@@ -53,16 +54,16 @@
 pytest = "*"
 tox = "*"
 
 [tool.poetry.group.docs.dependencies]
 Sphinx = "*"
 sphinx-rtd-theme = "*"
 
-
 [tool.poetry.extras]
+numba = ["numba"]
 plot = ["matplotlib"]
 test = ["pytest", "tox"]
 docs = ["Sphinx", "sphinx-rtd-theme"]
 
 [build-system]
 requires = ["poetry-core>=1.5", "poetry>=1.4"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `extremitypathfinder-2.6.0/tests/cli_test.py` & `extremitypathfinder-2.7.0/tests/cli_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/tests/helper_fcts_test.py` & `extremitypathfinder-2.7.0/tests/helper_fcts_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,32 +5,33 @@
 """
 from os.path import abspath, join, pardir
 from typing import Dict, Set
 
 import numpy as np
 import pytest
 
-from extremitypathfinder import PolygonEnvironment
+from extremitypathfinder import PolygonEnvironment, configs
 from extremitypathfinder.utils import (
-    _compute_extremity_idxs,
+    _cmp_extremity_mask,
     _compute_repr_n_dist,
     _has_clockwise_numbering,
     _inside_polygon,
     read_json,
 )
 from tests.helpers import proto_test_case
 from tests.test_find_visible import _clean_visibles
 
 
 def test_inside_polygon():
+    polygon_test_case = np.array([(-1.0, -1.0), (1.0, -1.0), (1.0, 1.0), (-1.0, 1.0)], dtype=configs.DTYPE_FLOAT)
+
     for border_value in [True, False]:
 
         def test_fct(input):
-            polygon_test_case = np.array([(-1.0, -1.0), (1.0, -1.0), (1.0, 1.0), (-1.0, 1.0)])
-            p = np.array(input, dtype=float)
+            p = np.array(input, dtype=configs.DTYPE_FLOAT)
             return _inside_polygon(p, polygon_test_case, border_value)
 
         p_test_cases = [
             # (x,y),
             # inside
             (0.0, 0.0),
             # # outside
@@ -145,16 +146,17 @@
                 (0, -1),
             ],
             {6, 1},
         ),
     ],
 )
 def test_compute_extremity_idxs(coords, expected):
-    coords = np.array(coords)
-    res = _compute_extremity_idxs(coords)
+    coords = np.array(coords, dtype=configs.DTYPE_FLOAT)
+    extremity_mask = _cmp_extremity_mask(coords)
+    res = list(np.where(extremity_mask)[0])
     assert set(res) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
     [
         # clockwise numbering!
@@ -166,15 +168,16 @@
         ([(0.0, 0.0), (10.0, 0.0), (10.0, 10.0), (0.0, 10.0)], False),
         ([(0.0, 0.0), (10.0, 0.0), (10.0, 5.0), (10.0, 10.0), (0.0, 10.0)], False),
         ([(0.0, 0.0), (10.0, 0.0), (9.0, 5.0), (10.0, 10.0), (0.0, 10.0)], False),
     ],
 )
 def test_clockwise_numering(input, expected):
     def clockwise_test_fct(input):
-        return _has_clockwise_numbering(np.array(input))
+        inp = np.array(input, dtype=configs.DTYPE_FLOAT)
+        return _has_clockwise_numbering(inp)
 
     assert clockwise_test_fct(input) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
     [
@@ -185,15 +188,16 @@
         ([0.0, 1.0], (1.0, 1.0)),
         ([-6.0, -5.0], (2.64018439966448, 7.810249675906654)),
         ([-5.0, -6.0], (2.768221279597376, 7.810249675906654)),
     ],
 )
 def test_compute_repr_n_dist(input, expected):
     def test_fct(input):
-        return _compute_repr_n_dist(np.array(input))
+        inp = np.array(input, dtype=configs.DTYPE_FLOAT)
+        return _compute_repr_n_dist(inp)
 
     assert test_fct(input) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
     [
@@ -205,15 +209,16 @@
         ([0.0, 2.0], 1.0),
         ([-2.0, 0.0], 2.0),
         ([0.0, -2.0], 3.0),
     ],
 )
 def test_angle_representation(input, expected):
     def func(input):
-        repr, dist = _compute_repr_n_dist(np.array(input))
+        inp = np.array(input, dtype=configs.DTYPE_FLOAT)
+        repr, dist = _compute_repr_n_dist(inp)
         return repr
 
     assert func(input) == expected
 
 
 @pytest.mark.parametrize(
     "input, expected",
@@ -238,13 +243,14 @@
         ([-0.00001, 1.0], 1.0),
         ([-1.0, -0.00001], 2.0),
         ([-0.00001, -1.0], 2.0),
     ],
 )
 def test_angle_repr_quadrant(input, expected):
     def func(input):
-        repr, dist = _compute_repr_n_dist(np.array(input))
+        inp = np.array(input, dtype=configs.DTYPE_FLOAT)
+        repr, dist = _compute_repr_n_dist(inp)
         return repr
 
     res = func(input)
     assert res >= expected
     assert res < expected + 1
```

### Comparing `extremitypathfinder-2.6.0/tests/helpers.py` & `extremitypathfinder-2.7.0/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/tests/main_test.py` & `extremitypathfinder-2.7.0/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/tests/test_cases.py` & `extremitypathfinder-2.7.0/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `extremitypathfinder-2.6.0/tests/test_find_visible.py` & `extremitypathfinder-2.7.0/tests/test_find_visible.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import itertools
 from typing import Set, Tuple
 
 import numpy as np
 import pytest
 
-from extremitypathfinder import PolygonEnvironment, utils
+from extremitypathfinder import PolygonEnvironment, configs, utils
 from extremitypathfinder.utils import _find_within_range, _lies_behind, get_neighbour_idxs
 from tests.test_cases import GRID_ENV_PARAMS, POLYGON_ENVS
 
 
 def find_candidates_behind(
     origin: int, v1: int, v2: int, candidates: Set[int], distances: np.ndarray, coords: np.ndarray
 ) -> Set[int]:
@@ -218,18 +218,18 @@
     # all remaining vertices were not concealed behind any edge and hence are visible
     visibles.update(candidates)
     return _clean_visibles(visibles, representations, distances)
 
 
 def compile_boundary_data(env):
     boundary, holes = env
-    boundary = np.array(boundary)
-    holes = [np.array(hole) for hole in holes]
+    boundary = np.array(boundary, dtype=configs.DTYPE_FLOAT)
+    holes = [np.array(hole, dtype=configs.DTYPE_FLOAT) for hole in holes]
     # (coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs)
-    return utils.compile_boundary_data_fr_polys(boundary, holes)
+    return utils.compile_polygon_datastructs(boundary, holes)
 
 
 def _yield_input_args(boundary_data):
     coords, extremity_indices, extremity_mask, vertex_edge_idxs, edge_vertex_idxs = boundary_data
     candidates = set(np.where(extremity_mask)[0])
     nr_edges = len(edge_vertex_idxs)
     edges_to_check = set(range(nr_edges))
@@ -251,16 +251,14 @@
             edge_vertex_idxs,
             vertex_edge_idxs,
             extremity_mask,
         )
 
 
 def _yield_reference(boundary_data):
-    # TODO move old implementation to tests test_cases.FIND_VISIBLE_TEST_CASES
-    # TODO compile test cases with output from ref. impl.
     for (
         origin,
         candidates,
         edges_to_check,
         coords,
         representations,
         distances,
```

### Comparing `extremitypathfinder-2.6.0/PKG-INFO` & `extremitypathfinder-2.7.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extremitypathfinder
-Version: 2.6.0
+Version: 2.7.0
 Summary: python package for fast shortest path computation on 2D polygon or grid maps
 Home-page: https://extremitypathfinder.readthedocs.io/en/latest/
 License: MIT
 Keywords: path-planning,path-finding,shortest-path,visibility,graph,polygon,grid,map,robotics,navigation,offline
 Author: jannikmi
 Author-email: github@michelfe.it
 Requires-Python: >=3.8,<4.0
@@ -21,17 +21,19 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
 Classifier: Topic :: Games/Entertainment
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Provides-Extra: docs
+Provides-Extra: numba
 Provides-Extra: plot
 Provides-Extra: test
 Requires-Dist: networkx (>=3,<4)
+Requires-Dist: numba (>=0.56.0,<0.57.0) ; extra == "numba"
 Requires-Dist: numpy (>=1.22,<2.0)
 Project-URL: Documentation, https://extremitypathfinder.readthedocs.io/en/latest/
 Project-URL: Repository, https://github.com/jannikmi/extremitypathfinder
 Description-Content-Type: text/x-rst
 
 ===================
 extremitypathfinder
@@ -70,17 +72,19 @@
 
 
 .. image:: ./docs/_static/title_demo_plot.png
 
 
 Quick Guide:
 
+Install the package with the optional Numba extra for a significant speedup:
+
 .. code-block:: console
 
-    pip install extremitypathfinder
+    pip install extremitypathfinder[numba]
 
 
 .. code-block:: python
 
     from extremitypathfinder import PolygonEnvironment
 
     environment = PolygonEnvironment()
```

