# Comparing `tmp/ssb_sgis-0.2.4.tar.gz` & `tmp/ssb_sgis-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ssb_sgis-0.2.4.tar", max compression
+gzip compressed data, was "ssb_sgis-0.2.5.tar", max compression
```

## Comparing `ssb_sgis-0.2.4.tar` & `ssb_sgis-0.2.5.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1074 2023-05-30 08:15:22.953857 ssb_sgis-0.2.4/LICENSE
--rw-r--r--   0        0        0     7543 2023-05-30 08:15:22.953857 ssb_sgis-0.2.4/README.md
--rw-r--r--   0        0        0     2539 2023-05-30 08:15:38.417915 ssb_sgis-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     2309 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/__init__.py
--rw-r--r--   0        0        0     3243 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/dapla.py
--rw-r--r--   0        0        0      576 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/__init__.py
--rw-r--r--   0        0        0     8028 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/buffer_dissolve_explode.py
--rw-r--r--   0        0        0    23937 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/general.py
--rw-r--r--   0        0        0     5480 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/geometry_types.py
--rw-r--r--   0        0        0    14520 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/neighbors.py
--rw-r--r--   0        0        0    11815 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/overlay.py
--rw-r--r--   0        0        0     6888 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/point_operations.py
--rw-r--r--   0        0        0    18717 2023-05-30 08:15:38.417915 ssb_sgis-0.2.4/src/sgis/geopandas_tools/polygon_operations.py
--rw-r--r--   0        0        0     9722 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/geopandas_tools/to_geodataframe.py
--rw-r--r--   0        0        0     2674 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/helpers.py
--rw-r--r--   0        0        0        0 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/__init__.py
--rw-r--r--   0        0        0    20484 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/explore.py
--rw-r--r--   0        0        0     1938 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/httpserver.py
--rw-r--r--   0        0        0    20499 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/legend.py
--rw-r--r--   0        0        0    17448 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/map.py
--rw-r--r--   0        0        0    16009 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/maps.py
--rw-r--r--   0        0        0    14132 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/maps/thematicmap.py
--rw-r--r--   0        0        0        0 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/__init__.py
--rw-r--r--   0        0        0     6218 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/_get_route.py
--rw-r--r--   0        0        0     2017 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/_od_cost_matrix.py
--rw-r--r--   0        0        0     4206 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/_points.py
--rw-r--r--   0        0        0     4487 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/_service_area.py
--rw-r--r--   0        0        0    12433 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/closing_network_holes.py
--rw-r--r--   0        0        0    11984 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/cutting_lines.py
--rw-r--r--   0        0        0     9375 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/directednetwork.py
--rw-r--r--   0        0        0     3359 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/finding_isolated_networks.py
--rw-r--r--   0        0        0     7686 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/network.py
--rw-r--r--   0        0        0    66761 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/networkanalysis.py
--rw-r--r--   0        0        0    12643 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/networkanalysisrules.py
--rw-r--r--   0        0        0     6740 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/networkanalysis/nodes.py
--rw-r--r--   0        0        0        0 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/py.typed
--rw-r--r--   0        0        0     3774 2023-05-30 08:15:22.989857 ssb_sgis-0.2.4/src/sgis/read_parquet.py
--rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-06-08 11:05:20.483431 ssb_sgis-0.2.5/LICENSE
+-rw-r--r--   0        0        0     7543 2023-06-08 11:05:20.483431 ssb_sgis-0.2.5/README.md
+-rw-r--r--   0        0        0     2539 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2334 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/__init__.py
+-rw-r--r--   0        0        0     3442 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/dapla.py
+-rw-r--r--   0        0        0      576 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/__init__.py
+-rw-r--r--   0        0        0     8080 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py
+-rw-r--r--   0        0        0    17659 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/general.py
+-rw-r--r--   0        0        0     5870 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/geometry_types.py
+-rw-r--r--   0        0        0    14520 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/neighbors.py
+-rw-r--r--   0        0        0    11862 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/overlay.py
+-rw-r--r--   0        0        0     6888 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/point_operations.py
+-rw-r--r--   0        0        0    20336 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/geopandas_tools/polygon_operations.py
+-rw-r--r--   0        0        0     9722 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/geopandas_tools/to_geodataframe.py
+-rw-r--r--   0        0        0     2674 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/helpers.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/maps/__init__.py
+-rw-r--r--   0        0        0    21872 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/explore.py
+-rw-r--r--   0        0        0     1923 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/httpserver.py
+-rw-r--r--   0        0        0    20499 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/maps/legend.py
+-rw-r--r--   0        0        0    18490 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/map.py
+-rw-r--r--   0        0        0    15961 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/maps/maps.py
+-rw-r--r--   0        0        0    14132 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/maps/thematicmap.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/__init__.py
+-rw-r--r--   0        0        0     6218 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_get_route.py
+-rw-r--r--   0        0        0     2017 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_od_cost_matrix.py
+-rw-r--r--   0        0        0     4206 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_points.py
+-rw-r--r--   0        0        0     4487 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/_service_area.py
+-rw-r--r--   0        0        0    12433 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/closing_network_holes.py
+-rw-r--r--   0        0        0    12369 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/networkanalysis/cutting_lines.py
+-rw-r--r--   0        0        0     9375 2023-06-08 11:05:20.519431 ssb_sgis-0.2.5/src/sgis/networkanalysis/directednetwork.py
+-rw-r--r--   0        0        0     3359 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/finding_isolated_networks.py
+-rw-r--r--   0        0        0     7686 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/network.py
+-rw-r--r--   0        0        0    66761 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysis.py
+-rw-r--r--   0        0        0    12643 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysisrules.py
+-rw-r--r--   0        0        0     6767 2023-06-08 11:05:50.623519 ssb_sgis-0.2.5/src/sgis/networkanalysis/nodes.py
+-rw-r--r--   0        0        0        0 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/py.typed
+-rw-r--r--   0        0        0     3774 2023-06-08 11:05:20.523431 ssb_sgis-0.2.5/src/sgis/read_parquet.py
+-rw-r--r--   0        0        0     8831 1970-01-01 00:00:00.000000 ssb_sgis-0.2.5/PKG-INFO
```

### Comparing `ssb_sgis-0.2.4/LICENSE` & `ssb_sgis-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/README.md` & `ssb_sgis-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/pyproject.toml` & `ssb_sgis-0.2.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ssb-sgis"
-version = "0.2.4"
+version = "0.2.5"
 description = "GIS functions used at Statistics Norway."
 authors = ["Statistics Norway <ort@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "sgis", from = "src"}]
 homepage = "https://github.com/statisticsnorway/ssb-sgis"
 repository = "https://github.com/statisticsnorway/ssb-sgis"
@@ -16,15 +16,15 @@
 [tool.poetry.urls]
 Changelog = "https://github.com/statisticsnorway/ssb-sgis/releases"
 
 [tool.poetry.dependencies]
 python = ">=3.10,<3.12"
 branca = ">=0.6.0"
 folium = ">=0.14.0"
-geopandas = ">=0.12.2"
+geopandas = ">=0.13.0"
 igraph = ">=0.10.4"
 mapclassify = ">=2.5.0"
 matplotlib = ">=3.7.0"
 networkx = ">=3.0"
 numpy = ">=1.24.2"
 pandas = ">=1.5.3"
 pyarrow = ">=11.0.0"
```

### Comparing `ssb_sgis-0.2.4/src/sgis/__init__.py` & `ssb_sgis-0.2.5/src/sgis/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,18 +13,16 @@
     coordinate_array,
     drop_inactive_geometry_columns,
     make_grid,
     make_grid_from_bbox,
     make_ssb_grid,
     points_in_bounds,
     random_points,
-    random_points_in_polygons,
     rename_geometry_if,
     to_lines,
-    to_multipoint,
 )
 from .geopandas_tools.geometry_types import (
     get_geom_type,
     is_single_geom_type,
     to_single_geom_type,
 )
 from .geopandas_tools.neighbors import (
@@ -43,15 +41,17 @@
     eliminate_by_smallest,
     get_overlapping_polygon_indices,
     get_overlapping_polygon_product,
     get_overlapping_polygons,
     get_polygon_clusters,
 )
 from .geopandas_tools.to_geodataframe import to_gdf
+from .helpers import get_name
 from .maps.explore import Explore
+from .maps.httpserver import run_html_server
 from .maps.legend import Legend
 from .maps.maps import clipmap, explore, qtm, samplemap
 from .maps.thematicmap import ThematicMap
 from .networkanalysis.closing_network_holes import (
     close_network_holes,
     close_network_holes_to_deadends,
 )
```

### Comparing `ssb_sgis-0.2.4/src/sgis/dapla.py` & `ssb_sgis-0.2.5/src/sgis/dapla.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from geopandas.io.arrow import _geopandas_to_arrow
 from pyarrow import parquet
 
 
 def exists(path: str) -> bool:
     """Returns True if the path exists, and False if it doesn't.
 
-    Works in dapla and outside of dapla.
+    Works in Dapla and outside of Dapla.
 
     Args:
         path (str): The path to the file or directory.
 
     Returns:
         True if the path exists, False if not.
     """
@@ -54,35 +54,41 @@
         else:
             with fs.open(path, mode="rb") as file:
                 return gpd.read_file(file, **kwargs)
     except FileNotFoundError as e:
         parent = str(Path(path).parent)
         if exists(parent):
             print(
-                f"Didn't find the file {path}"
-                "\nHere are the files in the given parent directory:"
+                f"Didn't find the file {path}."
+                "\nHere are the files in the parent directory:"
             )
             print(dp.FileClient().ls(parent))
         raise e
 
 
-def write_geopandas(df: gpd.GeoDataFrame, gcs_path: str, **kwargs) -> None:
+def write_geopandas(
+    df: gpd.GeoDataFrame, gcs_path: str, overwrite: bool = True, **kwargs
+) -> None:
     """Writes a GeoDataFrame to the speficied format.
 
     Note:
         Does not currently write to shapelfile or filegeodatabase.
 
     Args:
         df: The GeoDataFrame to write.
         gcs_path: The path to the file you want to write to.
+        overwrite: Whether to overwrite the file if it exists. Defaults to True.
         **kwargs: Additional keyword arguments passed to parquet.write_table
             (for parquet) or geopandas' to_file method (if not parquet).
     """
     pd.io.parquet.BaseImpl.validate_dataframe(df)
 
+    if not overwrite and exists(gcs_path):
+        raise ValueError("File already exists.")
+
     if not len(df):
         try:
             dp.write_pandas(df, gcs_path, **kwargs)
         except Exception:
             dp.write_pandas(
                 df.drop(df._geometry_column_name, axis=1), gcs_path, **kwargs
             )
```

### Comparing `ssb_sgis-0.2.4/src/sgis/exceptions.py` & `ssb_sgis-0.2.5/src/sgis/exceptions.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/buffer_dissolve_explode.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/buffer_dissolve_explode.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 - index_parts is set to False, which will be the default in a future version of geopandas.
 
 - The buff function returns a GeoDataFrame, the geopandas method returns a GeoSeries.
 """
 
 from geopandas import GeoDataFrame, GeoSeries
 
+from .geometry_types import make_all_singlepart
+
 
 def _decide_ignore_index(kwargs: dict) -> tuple[dict, bool]:
     if "ignore_index" in kwargs:
         return kwargs, kwargs.pop("ignore_index")
 
     if not kwargs.get("by", None):
         return kwargs, True
@@ -54,27 +56,28 @@
         index_parts: If False (default), the index after dissolve is respected. If
             True, an integer index level is added during explode.
         copy: Whether to copy the GeoDataFrame before buffering.
         **dissolve_kwargs: additional keyword arguments passed to geopandas' dissolve.
 
     Returns:
         A buffered GeoDataFrame where overlapping geometries are dissolved.
-
     """
     dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
     dissolved = buffdiss(
         gdf,
         distance,
         resolution=resolution,
         copy=copy,
         **dissolve_kwargs,
     )
 
-    return dissolved.explode(index_parts=index_parts, ignore_index=ignore_index)
+    return make_all_singlepart(
+        dissolved, ignore_index=ignore_index, index_parts=index_parts
+    )
 
 
 def buffdiss(
     gdf: GeoDataFrame,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
@@ -143,21 +146,19 @@
 
     >>> sg.buffdiss(points, 100, by="group", as_index=False)
       group                                           geometry    number
     0     a  MULTIPOLYGON (((258866.258 6648220.031, 258865...  0.323948
     1     b  MULTIPOLYGON (((258404.858 6647830.931, 258404...  0.687635
     2     d  MULTIPOLYGON (((258180.258 6647935.731, 258179...  0.580157
     """
-    geom_col = gdf._geometry_column_name
-
     buffered = buff(gdf, distance, resolution=resolution, copy=copy)
 
     dissolved = buffered.dissolve(**dissolve_kwargs)
 
-    dissolved[geom_col] = dissolved.make_valid()
+    dissolved[gdf._geometry_column_name] = dissolved.make_valid()
 
     return dissolved
 
 
 def dissexp(
     gdf: GeoDataFrame,
     index_parts: bool = False,
@@ -180,15 +181,17 @@
 
     dissolve_kwargs, ignore_index = _decide_ignore_index(dissolve_kwargs)
 
     dissolved = gdf.dissolve(**dissolve_kwargs)
 
     dissolved[geom_col] = dissolved.make_valid()
 
-    return dissolved.explode(index_parts=index_parts, ignore_index=ignore_index)
+    return make_all_singlepart(
+        dissolved, ignore_index=ignore_index, index_parts=index_parts
+    )
 
 
 def buff(
     gdf: GeoDataFrame | GeoSeries,
     distance: int | float,
     resolution: int = 50,
     copy: bool = True,
@@ -208,17 +211,15 @@
     Returns:
         A buffered GeoDataFrame.
     """
 
     if isinstance(gdf, GeoSeries):
         return gdf.buffer(distance, resolution=resolution, **buffer_kwargs).make_valid()
 
-    geom_col = gdf._geometry_column_name
-
     if copy:
         gdf = gdf.copy()
 
-    gdf[geom_col] = gdf.buffer(
+    gdf[gdf._geometry_column_name] = gdf.buffer(
         distance, resolution=resolution, **buffer_kwargs
     ).make_valid()
 
     return gdf
```

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/general.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/general.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 import warnings
 
 import geopandas as gpd
 import numpy as np
-import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from geopandas.array import GeometryDtype
 from shapely import (
     Geometry,
     box,
-    force_2d,
+    extract_unique_points,
     get_exterior_ring,
     get_interior_ring,
     get_num_interior_rings,
     get_parts,
-    wkt,
 )
 from shapely.geometry import LineString, Point, Polygon
 from shapely.ops import unary_union
 
-from .geometry_types import to_single_geom_type
+from .geometry_types import make_all_singlepart, to_single_geom_type
 from .to_geodataframe import to_gdf
 
 
 def coordinate_array(
     gdf: GeoDataFrame | GeoSeries,
 ) -> np.ndarray[np.ndarray[float], np.ndarray[float]]:
     """Creates a 2d ndarray of coordinates from point geometries.
@@ -179,15 +177,15 @@
 
     Returns:
         GeoDataFrame with grid geometries and a column 'SSBID'.
 
     Raises:
         ValueError: If the GeoDataFrame does not have 25833 as crs.
     """
-    if gdf.crs != 25833:
+    if not gdf.crs.equals(25833):
         raise ValueError(
             "Geodataframe must have crs = 25833. Use df.set_crs(25833) to set "
             "projection or df.to_crs(25833) for transforming."
         )
 
     minx, miny, maxx, maxy = gdf.total_bounds
 
@@ -280,15 +278,17 @@
 
     Args:
         gdf: The GeoDataFrame.
 
     Returns:
         GeoDataFrame of multipoints with same length and index as 'gdf'.
     """
-    return bounds_to_polygon(gdf).pipe(to_multipoint)
+    gdf = bounds_to_polygon(gdf)
+    gdf["geometry"] = extract_unique_points(gdf)
+    return gdf
 
 
 def clean_geoms(
     gdf: GeoDataFrame | GeoSeries, ignore_index: bool = False
 ) -> GeoDataFrame | GeoSeries:
     """Fixes geometries and removes invalid, empty, NaN and None geometries.
 
@@ -411,131 +411,14 @@
     y = np.random.rand(n) * float(loc) * 2
 
     return GeoDataFrame(
         (Point(x, y) for x, y in zip(x, y, strict=True)), columns=["geometry"]
     )
 
 
-def random_points_in_polygons(
-    gdf: GeoDataFrame | GeoSeries, n: int, ignore_index=False
-) -> GeoDataFrame:
-    """Creates n random points inside each polygon of a GeoDataFrame.
-
-    Args:
-        gdf: GeoDataFrame to use as mask for the points.
-        n: Number of points to create per polygon in 'gdf'.
-        ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
-            Defaults to False, meaning the points will have the index of the polygon
-            it is within.
-
-    Returns:
-        A GeoDataFrame of points with 'n' rows per row in 'gdf'. It uses the index
-        values of 'gdf'.
-
-    Examples
-    --------
-    First create and buffer 100 random points.
-
-    >>> import sgis as sg
-    >>> gdf = sg.random_points(100)
-    >>> polygons = sg.buff(gdf, 1)
-    >>> polygons
-                                                 geometry
-    0   POLYGON ((1.49436 0.36088, 1.49387 0.32947, 1....
-    1   POLYGON ((1.38427 0.21069, 1.38378 0.17928, 1....
-    2   POLYGON ((1.78894 0.94134, 1.78845 0.90992, 1....
-    3   POLYGON ((1.47174 0.81259, 1.47125 0.78118, 1....
-    4   POLYGON ((1.13941 0.20821, 1.13892 0.17680, 1....
-    ..                                                ...
-    95  POLYGON ((1.13462 0.18908, 1.13412 0.15767, 1....
-    96  POLYGON ((1.96391 0.43191, 1.96342 0.40050, 1....
-    97  POLYGON ((1.30569 0.46956, 1.30520 0.43815, 1....
-    98  POLYGON ((1.18172 0.10944, 1.18122 0.07803, 1....
-    99  POLYGON ((1.06156 0.99893, 1.06107 0.96752, 1....
-    [100 rows x 1 columns]
-
-    >>> points = sg.random_points_in_polygons(polygons, 3)
-    >>> points
-                        geometry
-    0   POINT (0.74944 -0.41658)
-    0    POINT (1.27490 0.54076)
-    0    POINT (0.22523 0.49323)
-    1   POINT (0.25302 -0.34825)
-    1    POINT (0.21124 0.89223)
-    ..                       ...
-    98  POINT (-0.39865 0.87135)
-    98   POINT (0.03573 0.50788)
-    99  POINT (-0.79089 0.57835)
-    99   POINT (0.39838 1.50881)
-    99   POINT (0.98383 0.77298)
-    [300 rows x 1 columns]
-    """
-    if not isinstance(gdf, GeoDataFrame):
-        gdf = to_gdf(gdf)
-
-    if not all(gdf.geom_type.isin(["Polygon", "MultiPolygon"])):
-        raise ValueError("Geometry types must be polygon.")
-
-    if gdf.index.is_unique:
-        gdf["temp_idx____"] = gdf.index
-    else:
-        gdf["temp_idx____"] = range(len(gdf))
-
-    all_points = pd.DataFrame()
-
-    for _ in range(n):
-        bounds = gdf.bounds
-        temp_idx____ = gdf["temp_idx____"].values
-        overlapping = pd.DataFrame()
-        overlapping_indices = ()
-
-        while len(bounds):
-            xs = np.random.uniform(bounds.minx, bounds.maxx)
-            ys = np.random.uniform(bounds.miny, bounds.maxy)
-
-            points_df = pd.DataFrame({"x": xs, "y": ys}, index=temp_idx____)
-
-            points = to_gdf(points_df, geometry=["x", "y"], crs=gdf.crs).drop(
-                ["x", "y"], axis=1
-            )
-
-            overlapping = points.sjoin(gdf[["temp_idx____", "geometry"]], how="inner")
-
-            overlapping = overlapping.loc[overlapping.index == overlapping.temp_idx____]
-
-            all_points = pd.concat([all_points, overlapping], ignore_index=ignore_index)
-
-            overlapping_indices = overlapping_indices + tuple(overlapping.index.values)
-
-            gdf__ = gdf.loc[~gdf["temp_idx____"].isin(overlapping_indices)]
-            temp_idx____ = gdf__["temp_idx____"].values
-            bounds = gdf__.bounds
-
-    all_points = all_points.sort_index()
-
-    all_points = all_points.loc[
-        :, ~all_points.columns.str.contains("temp_idx____|index_right")
-    ]
-
-    if gdf.index.is_unique:
-        gdf = gdf.drop("temp_idx____", axis=1)
-        return all_points
-
-    original_index = {
-        temp_idx: idx for temp_idx, idx in zip(gdf.temp_idx____, gdf.index)
-    }
-
-    all_points.index = all_points.index.map(original_index)
-    all_points.index.name = None
-
-    gdf = gdf.drop("temp_idx____", axis=1)
-
-    return all_points
-
-
 def points_in_bounds(gdf: GeoDataFrame | GeoSeries, n2: int):
     minx, miny, maxx, maxy = gdf.total_bounds
     xs = np.linspace(minx, maxx, num=n2)
     ys = np.linspace(miny, maxy, num=n2)
     x_coords, y_coords = np.meshgrid(xs, ys, indexing="ij")
     coords = np.concatenate((x_coords.reshape(-1, 1), y_coords.reshape(-1, 1)), axis=1)
     return to_gdf(coords, crs=gdf.crs)
@@ -638,90 +521,15 @@
 
     unioned = lines[0].overlay(lines[1], how="union", keep_geom_type=True)
 
     if len(lines) > 2:
         for line_gdf in lines[2:]:
             unioned = unioned.overlay(line_gdf, how="union", keep_geom_type=True)
 
-    return unioned.explode(ignore_index=True)
-
-
-def to_multipoint(
-    gdf: GeoDataFrame | GeoSeries, copy: bool = True
-) -> GeoDataFrame | GeoSeries:
-    """Creates multipoint geometries from GeoDataFrame or GeoSeries.
-
-    Takes a GeoDataFrame or GeoSeries and turns it into a MultiPoint.
-
-    Args:
-        gdf: The geometry to be converted to MultiPoint.
-        copy: If True, the geometry will be copied. Defaults to True.
-
-    Returns:
-        A GeoDataFrame or GeoSeries with MultiPoint geometries. If the input type
-        if GeoDataFrame, the other columns will be preserved.
-
-    Examples
-    --------
-    Let's create a GeoDataFrame with a point, a line and a polygon.
-
-    >>> from sgis import to_multipoint, to_gdf
-    >>> from shapely.geometry import LineString, Polygon
-    >>> gdf = to_gdf([
-    ...     (0, 0),
-    ...     LineString([(1, 1), (2, 2)]),
-    ...     Polygon([(3, 3), (4, 4), (3, 4), (3, 3)])
-    ...     ])
-    >>> gdf
-                                                geometry
-    0                            POINT (0.00000 0.00000)
-    1      LINESTRING (1.00000 1.00000, 2.00000 2.00000)
-    2  POLYGON ((3.00000 3.00000, 4.00000 4.00000, 3....
-
-    >>> to_multipoint(gdf)
-                                                geometry
-    0                            POINT (0.00000 0.00000)
-    1      MULTIPOINT (1.00000 1.00000, 2.00000 2.00000)
-    2  MULTIPOINT (3.00000 3.00000, 3.00000 4.00000, ...
-    """
-    if copy:
-        gdf = gdf.copy()
-
-    if gdf.is_empty.any():
-        raise ValueError("Cannot create multipoints from empty geometry.")
-
-    def _to_multipoint(gdf):
-        koordinater = "".join(
-            [x for x in gdf.wkt if x.isdigit() or x.isspace() or x == "." or x == ","]
-        ).strip()
-
-        alle_punkter = [
-            wkt.loads(f"POINT ({punkt.strip()})") for punkt in koordinater.split(",")
-        ]
-
-        return unary_union(alle_punkter)
-
-    if isinstance(gdf, GeoDataFrame):
-        gdf[gdf._geometry_column_name] = (
-            gdf[gdf._geometry_column_name]
-            .pipe(force_2d)
-            .apply(lambda x: _to_multipoint(x))
-        )
-
-    elif isinstance(gdf, gpd.GeoSeries):
-        gdf = force_2d(gdf)
-        gdf = gdf.apply(lambda x: _to_multipoint(x))
-
-    else:
-        gdf = to_gdf(gdf)
-        gdf["geometry"] = (
-            gdf["geometry"].pipe(force_2d).apply(lambda x: _to_multipoint(x))
-        )
-
-    return gdf
+    return make_all_singlepart(unioned, ignore_index=True)
 
 
 def clean_clip(
     gdf: GeoDataFrame | GeoSeries,
     mask: GeoDataFrame | GeoSeries | Geometry,
     **kwargs,
 ) -> GeoDataFrame | GeoSeries:
```

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/geometry_types.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/geometry_types.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,25 @@
 """Check and set geometry type."""
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 
 
+def make_all_singlepart(
+    gdf: GeoDataFrame, index_parts: bool = False, ignore_index: bool = False
+) -> GeoDataFrame:
+    gdf = gdf.explode(index_parts=index_parts, ignore_index=ignore_index)
+
+    while not gdf.geom_type.isin(
+        ["Polygon", "Point", "LineString", "LinearRing"]
+    ).all():
+        gdf = gdf.explode(index_parts=index_parts, ignore_index=ignore_index)
+
+    return gdf
+
+
 def to_single_geom_type(
     gdf: GeoDataFrame | GeoSeries,
     geom_type: str,
     ignore_index: bool = False,
 ) -> GeoDataFrame | GeoSeries:
     """Returns only the specified geometry type in a GeoDataFrame or GeoSeries.
 
@@ -65,15 +78,15 @@
     """
     if not isinstance(gdf, (GeoDataFrame, GeoSeries)):
         raise TypeError(f"'gdf' should be GeoDataFrame or GeoSeries, got {type(gdf)}")
 
     # explode collections to single-typed geometries
     collections = gdf.loc[gdf.geom_type == "GeometryCollection"]
     if len(collections):
-        collections = collections.explode(ignore_index=ignore_index, index_parts=False)
+        collections = make_all_singlepart(collections, ignore_index=ignore_index)
 
         gdf = pd.concat([gdf, collections], ignore_index=ignore_index)
 
     if "poly" in geom_type:
         gdf = gdf.loc[gdf.geom_type.isin(["Polygon", "MultiPolygon"])]
     elif "line" in geom_type:
         gdf = gdf.loc[
```

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/neighbors.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/neighbors.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/overlay.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/overlay.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
 from pyproj import CRS
 from shapely import STRtree, difference, intersection, union_all
 
 from .general import _push_geom_col, clean_geoms
-from .geometry_types import get_geom_type, to_single_geom_type
+from .geometry_types import get_geom_type, make_all_singlepart, to_single_geom_type
 
 
 def overlay_update(
     df1: GeoDataFrame,
     df2: GeoDataFrame,
     keep_geom_type: bool = True,
     geom_type: str | tuple[str, str] | None = None,
@@ -124,16 +124,16 @@
     df2 = clean_geoms(df2)
 
     if geom_type_left:
         df1 = to_single_geom_type(df1, geom_type_left)
     if geom_type_right:
         df2 = to_single_geom_type(df2, geom_type_right)
 
-    df1 = df1.explode(ignore_index=True)
-    df2 = df2.explode(ignore_index=True)
+    df1 = make_all_singlepart(df1, ignore_index=True)
+    df2 = make_all_singlepart(df2, ignore_index=True)
 
     overlayed = (
         _shapely_overlay(df1, df2, how=how, crs=crs)
         .pipe(clean_geoms)
         .pipe(_push_geom_col)
     )
```

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/point_operations.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/point_operations.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/polygon_operations.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/polygon_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Functions for polygon geometries."""
+import warnings
 
 import geopandas as gpd
 import networkx as nx
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame, GeoSeries
 from shapely import (
@@ -20,39 +21,43 @@
 from .overlay import clean_overlay
 
 
 def eliminate_by_longest(
     gdf: GeoDataFrame,
     to_eliminate: GeoDataFrame,
     *,
+    remove_isolated: bool = False,
     ignore_index: bool = False,
     aggfunc: str | dict | list = "first",
     **kwargs,
 ) -> GeoDataFrame:
     """Dissolves selected polygons with the longest bordering neighbor polygon.
 
     Eliminates selected geometries by dissolving them with the neighboring
     polygon with the longest shared border. The index and column values of the
     large polygons will be kept, unless else is specified.
 
     Args:
         gdf: GeoDataFrame with polygon geometries.
         to_eliminate: The geometries to be eliminated by 'gdf'.
+        remove_isolated: If False (default), polygons in 'to_eliminate' that share
+            no border with any polygon in 'gdf' will be kept. If True, the isolated
+            polygons will be removed.
         ignore_index: If False (default), the resulting GeoDataFrame will keep the
             index of the large polygons. If True, the resulting axis will be labeled
             0, 1, …, n - 1.
         aggfunc: Aggregation function(s) to use when dissolving. Defaults to 'first',
             meaning the column values of the large polygons are kept.
         kwargs: Keyword arguments passed to the dissolve method.
 
     Returns:
         The GeoDataFrame with the small polygons dissolved into the large polygons.
     """
 
-    # remove polygons in gdf that are present in to_eliminated
+    # remove polygons in gdf that are present in to_eliminate
     gdf = gdf.loc[~gdf.geometry.astype(str).isin(to_eliminate.geometry.astype(str))]
 
     if not ignore_index:
         idx_mapper = {i: idx for i, idx in enumerate(gdf.index)}
         idx_name = gdf.index.name
 
     # resetting in case not unique index
@@ -70,111 +75,122 @@
 
     longest_border = lines.sort_values("length__", ascending=False).drop_duplicates(
         "eliminate_idx"
     )
 
     to_poly_idx = longest_border.set_index("eliminate_idx")["poly_idx"]
     to_eliminate["dissolve_idx"] = to_eliminate["eliminate_idx"].map(to_poly_idx)
+
     gdf["dissolve_idx"] = gdf["poly_idx"]
 
     kwargs.pop("as_index", None)
-    eliminated = (
-        pd.concat([gdf, to_eliminate])
-        .dissolve("dissolve_idx", aggfunc=aggfunc, **kwargs)
-        .drop(
-            ["length__", "eliminate_idx", "poly_idx"],
-            axis=1,
-            errors="ignore",
-        )
+    eliminated = pd.concat([gdf, to_eliminate]).dissolve(
+        "dissolve_idx", aggfunc=aggfunc, **kwargs
     )
 
     if ignore_index:
         return eliminated.reset_index(drop=True)
-
-    eliminated.index = eliminated.index.map(idx_mapper)
-    eliminated.index.name = idx_name
-
-    return eliminated
+    else:
+        eliminated.index = eliminated.index.map(idx_mapper)
+        eliminated.index.name = idx_name
+
+    if not remove_isolated:
+        isolated = to_eliminate.loc[to_eliminate["dissolve_idx"].isna()]
+        eliminated = pd.concat([eliminated, isolated])
+
+    return eliminated.drop(
+        ["dissolve_idx", "length__", "eliminate_idx", "poly_idx"],
+        axis=1,
+        errors="ignore",
+    )
 
 
 def eliminate_by_largest(
     gdf: GeoDataFrame,
     to_eliminate: GeoDataFrame,
+    remove_isolated: bool = False,
     ignore_index: bool = False,
     aggfunc: str | dict | list = "first",
     **kwargs,
 ) -> GeoDataFrame:
     """Dissolves selected polygons with the largest neighbor polygon.
 
     Eliminates selected geometries by dissolving them with the neighboring
     polygon with the largest area. The index and column values of the
     large polygons will be kept, unless else is specified.
 
     Args:
         gdf: GeoDataFrame with polygon geometries.
         to_eliminate: The geometries to be eliminated by 'gdf'.
+        remove_isolated: If False (default), polygons in 'to_eliminate' that share
+            no border with any polygon in 'gdf' will be kept. If True, the isolated
+            polygons will be removed.
         ignore_index: If False (default), the resulting GeoDataFrame will keep the
             index of the large polygons. If True, the resulting axis will be labeled
             0, 1, …, n - 1.
         aggfunc: Aggregation function(s) to use when dissolving. Defaults to 'first',
             meaning the column values of the large polygons are kept.
         kwargs: Keyword arguments passed to the dissolve method.
 
     Returns:
         The GeoDataFrame with the selected polygons dissolved into the polygons of
         'gdf'.
     """
     return _eliminate_by_area(
         gdf,
         to_eliminate=to_eliminate,
+        remove_isolated=remove_isolated,
         ignore_index=ignore_index,
         sort_ascending=False,
         aggfunc=aggfunc,
         **kwargs,
     )
 
 
 def eliminate_by_smallest(
     gdf: GeoDataFrame,
     to_eliminate: GeoDataFrame,
+    remove_isolated: bool = False,
     ignore_index: bool = False,
     aggfunc: str | dict | list = "first",
     **kwargs,
 ) -> GeoDataFrame:
     return _eliminate_by_area(
         gdf,
         to_eliminate=to_eliminate,
+        remove_isolated=remove_isolated,
         ignore_index=ignore_index,
         sort_ascending=True,
         aggfunc=aggfunc,
         **kwargs,
     )
 
 
 def _eliminate_by_area(
     gdf: GeoDataFrame,
     to_eliminate: GeoDataFrame,
+    remove_isolated: bool,
     sort_ascending: bool,
     ignore_index: bool = False,
     aggfunc="first",
     **kwargs,
 ) -> GeoDataFrame:
-    # remove polygons in gdf that are present in to_eliminated
+    # remove polygons in gdf that are present in to_eliminate
     gdf = gdf.loc[~gdf.geometry.astype(str).isin(to_eliminate.geometry.astype(str))]
 
     if not ignore_index:
         idx_mapper = {i: idx for i, idx in enumerate(gdf.index)}
         idx_name = gdf.index.name
 
     gdf = gdf.reset_index(drop=True)
 
     gdf["area__"] = gdf.area
 
     joined = to_eliminate.sjoin(
-        gdf[["area__", "geometry"]], predicate="touches"
+        gdf[["area__", "geometry"]], predicate="touches", how="left"
     ).sort_values("area__", ascending=sort_ascending)
 
     largest = joined[~joined.index.duplicated()]
 
     gdf = gdf.assign(index_right=lambda x: x.index)
 
     kwargs.pop("as_index", None)
@@ -186,14 +202,18 @@
 
     if ignore_index:
         return eliminated.reset_index(drop=True)
 
     eliminated.index = eliminated.index.map(idx_mapper)
     eliminated.index.name = idx_name
 
+    if not remove_isolated:
+        isolated = joined.loc[joined["index_right"].isna()]
+        eliminated = pd.concat([eliminated, isolated])
+
     return eliminated
 
 
 def get_polygon_clusters(
     *gdfs: GeoDataFrame | GeoSeries,
     cluster_col: str = "cluster",
     allow_multipart: bool = False,
@@ -345,54 +365,71 @@
         gdf: GeoDataFrame of polygons.
         ignore_index: If True, the resulting axis will be labeled 0, 1, …, n - 1.
             Defaults to False.
 
     Returns:
         A GeoDataFrame of the overlapping polygons.
     """
-    if not gdf.index.is_unique:
-        raise ValueError(
-            "Index must be unique in order to correctly find "
-            "overlapping polygon indices."
-        )
+    if not any(gdf.geom_type.isin(["Polygon", "MultiPolygon"])):
+        raise ValueError("'gdf' has no polygons.")
+
+    elif not all(gdf.geom_type.isin(["Polygon", "MultiPolygon"])):
+        warnings.warn("'gdf' has mixed geometries. Non-polygons will be removed.")
+
+    if not ignore_index:
+        idx_mapper = {i: idx for i, idx in enumerate(gdf.index)}
+        idx_name = gdf.index.name
 
-    gdf = gdf.assign(overlap=gdf.index)
+    gdf = gdf.reset_index(drop=True).assign(overlap=gdf.index)
 
-    intersected = clean_overlay(gdf, gdf[["geometry"]], how="intersection")
+    intersected = clean_overlay(
+        gdf, gdf[["geometry"]], how="intersection", geom_type="polygon"
+    )
 
     points_joined = intersected.representative_point().to_frame().sjoin(intersected)
 
     duplicated_points = points_joined.loc[points_joined.index.duplicated()]
 
     duplicated_geoms = intersected.loc[intersected.index.isin(duplicated_points.index)]
     duplicated_geoms.index = duplicated_geoms["overlap"].values
 
     if ignore_index:
         duplicated_geoms = duplicated_geoms.reset_index(drop=True)
+    else:
+        duplicated_geoms.index = duplicated_geoms.index.map(idx_mapper)
+        duplicated_geoms.index.name = idx_name
 
     return duplicated_geoms.drop("overlap", axis=1)
 
 
 def get_overlapping_polygon_indices(gdf: GeoDataFrame | GeoSeries) -> pd.Index:
     if not gdf.index.is_unique:
         raise ValueError(
             "Index must be unique in order to correctly find "
             "overlapping polygon indices."
         )
 
-    gdf = gdf.assign(overlap=gdf.index)
+    idx_mapper = {i: idx for i, idx in enumerate(gdf.index)}
+    idx_name = gdf.index.name
 
-    intersected = clean_overlay(gdf, gdf[["geometry"]], how="intersection")
+    gdf = gdf.reset_index(drop=True).assign(overlap=gdf.index)
+
+    intersected = clean_overlay(
+        gdf, gdf[["geometry"]], how="intersection", geom_type="polygon"
+    )
 
     intersected = intersected.set_index("overlap")
 
     points_joined = intersected.representative_point().to_frame().sjoin(intersected)
 
     duplicated_points = points_joined.loc[points_joined.index.duplicated()]
 
+    duplicated_points.index = duplicated_points.index.map(idx_mapper)
+    duplicated_points.index.name = idx_name
+
     return duplicated_points.index.unique()
 
 
 def get_overlapping_polygon_product(gdf: GeoDataFrame | GeoSeries) -> pd.Index:
     if not gdf.index.is_unique:
         raise ValueError("Index must be unique to find overlapping polygon indices.")
```

### Comparing `ssb_sgis-0.2.4/src/sgis/geopandas_tools/to_geodataframe.py` & `ssb_sgis-0.2.5/src/sgis/geopandas_tools/to_geodataframe.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/helpers.py` & `ssb_sgis-0.2.5/src/sgis/helpers.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/maps/explore.py` & `ssb_sgis-0.2.5/src/sgis/maps/explore.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,20 +8,21 @@
 
 import branca as bc
 import folium
 import matplotlib
 import numpy as np
 import pandas as pd
 from geopandas import GeoDataFrame
-from IPython.core.display import display
+from IPython.display import display
 from shapely.geometry import LineString
 
-from ..geopandas_tools.general import clean_geoms, random_points_in_polygons
+from ..geopandas_tools.general import clean_geoms, make_all_singlepart
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..geopandas_tools.to_geodataframe import to_gdf
+from ..helpers import unit_is_degrees
 from .httpserver import run_html_server
 from .map import Map
 
 
 # the geopandas._explore raises a deprication warning. Ignoring for now.
 warnings.filterwarnings(
     action="ignore", category=matplotlib.MatplotlibDeprecationWarning
@@ -63,41 +64,48 @@
 class Explore(Map):
     def __init__(
         self,
         *gdfs,
         column: str | None = None,
         popup: bool = True,
         max_zoom: int = 30,
-        smooth_factor: 2.5,
+        smooth_factor: float = 1.5,
         browser: bool = False,
+        prefer_canvas: bool = True,
+        save=None,
         **kwargs,
     ):
         self.browser = browser
         if not self.browser and "show_in_browser" in kwargs:
             self.browser = kwargs.pop("show_in_browser")
         if not self.browser and "in_browser" in kwargs:
             self.browser = kwargs.pop("in_browser")
 
         super().__init__(*gdfs, column=column, **kwargs)
 
         self.popup = popup
         self.max_zoom = max_zoom
         self.smooth_factor = smooth_factor
+        self.prefer_canvas = prefer_canvas
+        self.save = save
 
         self._to_single_geom_type()
 
         if self._is_categorical:
             if len(self.gdfs) == 1:
                 self._split_categories()
         else:
             if not self._cmap:
                 self._cmap = "viridis"
             self.cmap_start = kwargs.pop("cmap_start", 0)
             self.cmap_stop = kwargs.pop("cmap_stop", 256)
 
+        if self._gdf.crs is None:
+            self.kwargs["crs"] = "Simple"
+
     def explore(
         self, column: str | None = None, center=None, size=None, **kwargs
     ) -> None:
         if column:
             self._column = column
             self._update_column()
             kwargs.pop("column", None)
@@ -146,15 +154,15 @@
             sample = self._gdf.sample(1)
 
         # convert lines to polygons
         if get_geom_type(sample) == "line":
             sample["geometry"] = sample.buffer(1)
 
         if get_geom_type(sample) == "polygon":
-            random_point = random_points_in_polygons(sample, 1)
+            random_point = sample.sample_points(size=1)
 
         # if point or mixed geometries
         else:
             random_point = sample.centroid
 
         self.center = (random_point.geometry.iloc[0].x, random_point.geometry.iloc[0].y)
         print(f"center={self.center}, size={size}")
@@ -180,30 +188,36 @@
             kwargs.pop("column", None)
 
         gdfs: tuple[GeoDataFrame] = ()
         for gdf in self._gdfs:
             gdf = gdf.clip(mask)
             collections = gdf.loc[gdf.geom_type == "GeometryCollection"]
             if len(collections):
-                collections = collections.explode(index_parts=False)
+                collections = make_all_singlepart(collections)
                 gdf = pd.concat([gdf, collections], ignore_index=False)
             gdfs = gdfs + (gdf,)
         self._gdfs = gdfs
         self._gdf = pd.concat(gdfs, ignore_index=True)
         self._explore(**kwargs)
 
     def _explore(self, **kwargs):
         self.kwargs = self.kwargs | kwargs
 
         if self._is_categorical:
             self._create_categorical_map()
         else:
             self._create_continous_map()
 
-        if self.browser:
+        if self.save:
+            import os
+
+            with open(os.getcwd() + "/" + self.save.strip(".html") + ".html", "w") as f:
+                f.write(self.map._repr_html_())
+            return
+        elif self.browser:
             run_html_server(self.map._repr_html_())
         else:
             display(self.map)
 
     def _split_categories(self):
         new_gdfs, new_labels = [], []
         for cat in self._unique_values:
@@ -218,58 +232,62 @@
         """Buffer gdf if mixed geometry types. Expode to singlepart.
 
         Because Folium does not handle mixed geometries well.
         """
 
         new_gdfs = []
         for gdf in self._gdfs:
-            if get_geom_type(gdf) == "mixed":
-                gdf[gdf._geometry_column_name] = gdf.buffer(0.1)
-            gdf = gdf.explode(index_parts=False)
+            if get_geom_type(gdf) == "mixed" and not unit_is_degrees(gdf):
+                gdf[gdf._geometry_column_name] = gdf.buffer(0.01)
+            gdf = make_all_singlepart(gdf)
             new_gdfs.append(gdf)
         self._gdfs = new_gdfs
         self._gdf = pd.concat(new_gdfs, ignore_index=True)
         self._nan_idx = self._gdf[self._column].isna()
 
     def _update_column(self):
         self._is_categorical = self._check_if_categorical()
         self._fillna_if_col_is_missing()
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
     def _create_categorical_map(self):
         self._get_categorical_colors()
 
-        self.map = self._explore_return(
-            self._gdf,
-            return_="empty_map",
+        gdf = self._prepare_gdf_for_map(self._gdf)
+        self.map = self._make_folium_map(
+            gdf,
             max_zoom=self.max_zoom,
             popup=self.popup,
+            prefer_canvas=self.prefer_canvas,
             **self.kwargs,
         )
 
         for gdf, label in zip(self._gdfs, self.labels, strict=True):
             if not len(gdf):
                 continue
 
             f = folium.FeatureGroup(name=label)
 
-            gjs = self._explore_return(
+            gdf = self._prepare_gdf_for_map(gdf)
+            gjs = self._make_geojson(
                 gdf,
                 color=gdf["color"],
-                return_="geojson",
                 tooltip=self._tooltip_cols(gdf),
                 popup=self.popup,
                 **{
                     key: value
                     for key, value in self.kwargs.items()
                     if key not in ["title"]
                 },
             )
-            f.add_child(gjs)
-            self.map.add_child(f)
+
+            gjs.layer_name = label
+
+            gjs.add_to(f)
+            gjs.add_to(self.map)
 
         _categorical_legend(
             self.map,
             self._column,
             self._categories_colors_dict.keys(),
             self._categories_colors_dict.values(),
         )
@@ -281,19 +299,20 @@
         self._prepare_continous_map()
         if self.scheme:
             classified = self._classify_from_bins(self._gdf, bins=self.bins)
             classified_sequential = self._push_classification(classified)
             n_colors = len(np.unique(classified_sequential)) - any(self._nan_idx)
             unique_colors = self._get_continous_colors(n=n_colors)
 
-        self.map = self._explore_return(
-            self._gdf,
-            return_="empty_map",
+        gdf = self._prepare_gdf_for_map(self._gdf)
+        self.map = self._make_folium_map(
+            gdf,
             max_zoom=self.max_zoom,
             popup=self.popup,
+            prefer_canvas=self.prefer_canvas,
             **self.kwargs,
         )
 
         colorbar = bc.colormap.StepColormap(
             unique_colors,
             vmin=self._gdf[self._column].min(),
             vmax=self._gdf[self._column].max(),
@@ -305,75 +324,73 @@
             if not len(gdf):
                 continue
             f = folium.FeatureGroup(name=label)
 
             classified = self._classify_from_bins(gdf, bins=self.bins)
             colorarray = unique_colors[classified]
 
-            gjs = self._explore_return(
+            gdf = self._prepare_gdf_for_map(gdf)
+            gjs = self._make_geojson(
                 gdf,
-                tooltip=self._tooltip_cols(gdf),
                 color=colorarray,
-                return_="geojson",
+                tooltip=self._tooltip_cols(gdf),
                 popup=self.popup,
-                **{key: value for key, value in self.kwargs.items() if key != "title"},
+                prefer_canvas=self.prefer_canvas,
+                **{
+                    key: value
+                    for key, value in self.kwargs.items()
+                    if key not in ["title"]
+                },
             )
+
             f.add_child(gjs)
             self.map.add_child(f)
 
         self.map.add_child(colorbar)
         folium.TileLayer("stamentoner").add_to(self.map)
         folium.TileLayer("cartodbdark_matter").add_to(self.map)
         self.map.add_child(folium.LayerControl())
 
     def _tooltip_cols(self, gdf: GeoDataFrame) -> list:
         if "tooltip" in self.kwargs:
             tooltip = self.kwargs.pop("tooltip")
             return tooltip
         return [col for col in gdf.columns if col not in COLS_TO_DROP]
 
-    def _explore_return(
+    @staticmethod
+    def _prepare_gdf_for_map(gdf):
+        # convert LinearRing to LineString
+        rings_mask = gdf.geom_type == "LinearRing"
+        if rings_mask.any():
+            gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
+                lambda g: LineString(g)
+            )
+
+        if gdf.crs is not None and not gdf.crs.equals(4326):
+            gdf = gdf.to_crs(4326)
+
+        return gdf
+
+    def _make_folium_map(
         self,
         df,
-        return_: str,
-        color=None,
         attr=None,
         tiles="OpenStreetMap",
-        tooltip=True,
-        popup=False,
-        highlight=True,
         width="100%",
         height="100%",
         control_scale=True,
-        marker_type=None,
-        marker_kwds={},
-        style_kwds={},
-        highlight_kwds={},
-        tooltip_kwds={},
-        popup_kwds={},
         map_kwds={},
         **kwargs,
     ):
-        """Contains the nessecary parts of the geopandas _explore function.
-
-        Also has a return_ parameter that controls what is returned. This should be
-        replaced by separate functions, and irrelevant parameters should be removed.
-        """
-        # xyservices is an optional dependency
-        try:
-            import xyzservices
-
-            has_xyzservices = True
-        except ImportError:
-            has_xyzservices = False
+        import xyzservices
 
         gdf = df.copy()
 
         # convert LinearRing to LineString
-        rings_mask = df.geom_type == "LinearRing"
+        rings_mask = gdf.geom_type == "LinearRing"
         if rings_mask.any():
             gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
                 lambda g: LineString(g)
             )
 
         if gdf.crs is None:
             kwargs["crs"] = "Simple"
@@ -404,43 +421,84 @@
                     f"Use the '{i}={map_kwds[i]}' argument instead."
                 )
         map_kwds = {
             **map_kwds,
             **{i: kwargs[i] for i in kwargs.keys() if i in _MAP_KWARGS},
         }
 
-        if has_xyzservices:
-            # match provider name string to xyzservices.TileProvider
-            if isinstance(tiles, str):
-                try:
-                    tiles = xyzservices.providers.query_name(tiles)
-                except ValueError:
-                    pass
-
-            if isinstance(tiles, xyzservices.TileProvider):
-                attr = attr if attr else tiles.html_attribution
-                map_kwds["min_zoom"] = tiles.get("min_zoom", 0)
-                map_kwds["max_zoom"] = tiles.get("max_zoom", 30)
-                tiles = tiles.build_url(scale_factor="{r}")
-
-            map_kwds["zoom_start"] = self.kwargs.get("zoom_start", 15)
-
-            m = folium.Map(
-                location=location,
-                control_scale=control_scale,
-                tiles=tiles,
-                attr=attr,
-                width=width,
-                height=height,
-                **map_kwds,
+        # match provider name string to xyzservices.TileProvider
+        if isinstance(tiles, str):
+            try:
+                tiles = xyzservices.providers.query_name(tiles)
+            except ValueError:
+                pass
+
+        if isinstance(tiles, xyzservices.TileProvider):
+            attr = attr if attr else tiles.html_attribution
+            map_kwds["min_zoom"] = tiles.get("min_zoom", 0)
+            map_kwds["max_zoom"] = tiles.get("max_zoom", 30)
+            tiles = tiles.build_url(scale_factor="{r}")
+
+        m = folium.Map(
+            location=location,
+            control_scale=control_scale,
+            tiles=tiles,
+            attr=attr,
+            width=width,
+            height=height,
+            **map_kwds,
+        )
+
+        # fit bounds to get a proper zoom level
+        if fit and "zoom_start" not in kwargs:
+            m.fit_bounds([[bounds[1], bounds[0]], [bounds[3], bounds[2]]])
+
+        return m
+
+    def _make_geojson(
+        self,
+        df,
+        color=None,
+        tooltip=True,
+        popup=False,
+        highlight=True,
+        marker_type=None,
+        marker_kwds={},
+        style_kwds={},
+        highlight_kwds={},
+        tooltip_kwds={},
+        popup_kwds={},
+        map_kwds={},
+        **kwargs,
+    ):
+        gdf = df.copy()
+
+        # convert LinearRing to LineString
+        rings_mask = gdf.geom_type == "LinearRing"
+        if rings_mask.any():
+            gdf.geometry[rings_mask] = gdf.geometry[rings_mask].apply(
+                lambda g: LineString(g)
             )
 
-            # fit bounds to get a proper zoom level
-            if fit:
-                m.fit_bounds([[bounds[1], bounds[0]], [bounds[3], bounds[2]]])
+        if gdf.crs is None:
+            kwargs["crs"] = "Simple"
+        elif not gdf.crs.equals(4326):
+            gdf = gdf.to_crs(4326)
+
+        # get a subset of kwargs to be passed to folium.Map
+        for i in _MAP_KWARGS:
+            if i in map_kwds:
+                raise ValueError(
+                    f"'{i}' cannot be specified in 'map_kwds'. "
+                    f"Use the '{i}={map_kwds[i]}' argument instead."
+                )
+        map_kwds = {
+            **map_kwds,
+            **{i: kwargs[i] for i in kwargs.keys() if i in _MAP_KWARGS},
+        }
 
         for map_kwd in _MAP_KWARGS:
             kwargs.pop(map_kwd, None)
 
         # set default style
         if "fillOpacity" not in style_kwds:
             style_kwds["fillOpacity"] = 0.5
@@ -517,29 +575,24 @@
             # specify fields to show in the tooltip
             tooltip = _tooltip_popup("tooltip", tooltip, gdf, **tooltip_kwds)
             popup = _tooltip_popup("popup", popup, gdf, **popup_kwds)
         else:
             tooltip = None
             popup = None
 
-        if "geojson" in return_:
-            # add dataframe to map
-            gjs = folium.GeoJson(
-                gdf.__geo_interface__,
-                tooltip=tooltip,
-                popup=popup,
-                marker=marker,
-                style_function=style_function,
-                highlight_function=highlight_function,
-                smooth_factor=self.smooth_factor,
-                **kwargs,
-            )
-            return gjs
-
-        return m
+        return folium.GeoJson(
+            gdf.__geo_interface__,
+            tooltip=tooltip,
+            popup=popup,
+            marker=marker,
+            style_function=style_function,
+            highlight_function=highlight_function,
+            smooth_factor=self.smooth_factor,
+            **kwargs,
+        )
 
 
 def _tooltip_popup(type, fields, gdf, **kwds):
     """get tooltip or popup"""
     import folium
 
     # specify fields to show in the tooltip
```

### Comparing `ssb_sgis-0.2.4/src/sgis/maps/httpserver.py` & `ssb_sgis-0.2.5/src/sgis/maps/httpserver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,16 @@
 import os
 import webbrowser
 from http.server import BaseHTTPRequestHandler, HTTPServer
 
-from IPython.core.display import HTML, display
+from IPython.display import HTML, display
 
 
 def run_html_server(contents: str | None = None, port: int = 3000):
-    """
-    Run a simple, temporary http web server for serving static HTML content.
-    """
+    """Run a simple, temporary http web server for serving static HTML content."""
     if "JUPYTERHUB_SERVICE_PREFIX" in os.environ:
         # Create a link using the https://github.com/jupyterhub/jupyter-server-proxy
         display_address = os.environ["JUPYTERHUB_SERVICE_PREFIX"] + "proxy/{}/".format(
             port
         )
         display_content = HTML(
             f"""
```

### Comparing `ssb_sgis-0.2.4/src/sgis/maps/legend.py` & `ssb_sgis-0.2.5/src/sgis/maps/legend.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/maps/map.py` & `ssb_sgis-0.2.5/src/sgis/maps/map.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,25 +55,27 @@
         *gdfs: GeoDataFrame,
         column: str | None = None,
         labels: tuple[str] | None = None,
         k: int = 5,
         bins: tuple[float] | None = None,
         nan_label: str = "Missing",
         nan_color="#c2c2c2",
+        scheme="fisherjenks",
         **kwargs,
     ):
         if not all(isinstance(gdf, GeoDataFrame) for gdf in gdfs):
             gdfs, column = self._separate_args(gdfs, column)
 
         self._column = column
         self.bins = bins
         self._k = k
         self.nan_label = nan_label
         self.nan_color = nan_color
         self._cmap = kwargs.pop("cmap", None)
+        self.scheme = scheme
 
         if not all(isinstance(gdf, GeoDataFrame) for gdf in gdfs):
             raise ValueError("gdfs must be GeoDataFrames.")
 
         if not any(len(gdf) for gdf in gdfs):
             raise ValueError("None of the GeoDataFrames have rows.")
 
@@ -90,49 +92,47 @@
 
         self._gdfs: list[GeoDataFrame] = [gdf.reset_index(drop=True) for gdf in gdfs]
         self.kwargs = kwargs
 
         if not self.labels:
             self._set_labels()
 
-        if not self._column:
-            for gdf, label in zip(self._gdfs, self.labels, strict=True):
-                gdf["label"] = label
-            self._column = "label"
-
         self._gdfs = self._to_common_crs_and_one_geom_col(self._gdfs)
         self._is_categorical = self._check_if_categorical()
 
-        self._fillna_if_col_is_missing()
+        if self._column:
+            self._fillna_if_col_is_missing()
+        else:
+            for gdf, label in zip(self._gdfs, self.labels, strict=True):
+                gdf["label"] = label
+            self._column = "label"
 
         self._gdf = pd.concat(self._gdfs, ignore_index=True)
 
         self._nan_idx = self._gdf[self._column].isna()
-
         self._get_unique_values()
 
     def _get_unique_values(self):
         if not self._is_categorical:
             self._unique_values = self._get_unique_floats()
-            if self._k > len(self._unique_values):
-                self._k = len(self._unique_values)
         else:
             self._unique_values = sorted(
                 list(self._gdf.loc[~self._nan_idx, self._column].unique())
             )
+        if self._k > len(self._unique_values):
+            self._k = len(self._unique_values)
 
     def _get_unique_floats(self) -> np.array:
         """Get unique floats by multiplying, then converting to integer.
 
         Find a multiplier that makes the max value greater than +- 1_000_000.
         Because floats don't always equal each other. This will make very
         similar values count as the same value in the color classification.
         """
         array = self._gdf.loc[~self._nan_idx, self._column]
-
         self._min = np.min(array)
         self._max = np.max(array)
         self._get_multiplier(array)
 
         unique = array.reset_index(drop=True).drop_duplicates()
         as_int = self._array_to_large_int(unique)
         no_duplicates = as_int.drop_duplicates()
@@ -186,19 +186,27 @@
             bins = [min(self._gdf.loc[~self._nan_idx, self._column])] + bins
 
         if min(bins) < 0 and min(self._gdf.loc[~self._nan_idx, self._column]) < min(
             bins
         ):
             bins = [min(self._gdf.loc[~self._nan_idx, self._column])] + bins
 
-        if max(bins) > 0 and max(self._gdf[self._column]) > max(bins):
-            bins = bins + [max(self._gdf[self._column])]
-
-        if max(bins) < 0 and max(self._gdf[self._column]) < max(bins):
-            bins = bins + [max(self._gdf[self._column])]
+        if max(bins) > 0 and max(
+            self._gdf.loc[self._gdf[self._column].notna(), self._column]
+        ) > max(bins):
+            bins = bins + [
+                max(self._gdf.loc[self._gdf[self._column].notna(), self._column])
+            ]
+
+        if max(bins) < 0 and max(
+            self._gdf.loc[self._gdf[self._column].notna(), self._column]
+        ) < max(bins):
+            bins = bins + [
+                max(self._gdf.loc[self._gdf[self._column].notna(), self._column])
+            ]
 
         return bins
 
     @staticmethod
     def _separate_args(
         args: tuple,
         column: str | None,
@@ -218,30 +226,28 @@
                 gdfs = gdfs + (arg,)
 
         return gdfs, column
 
     def _prepare_continous_map(self):
         """Create bins if not already done and adjust k if needed."""
 
-        default_scheme = "fisherjenks"
-
-        if not hasattr(self, "scheme"):
-            self.scheme = self.kwargs.pop("scheme", default_scheme)
-
         if self.scheme is None:
             return
 
         if not self.bins:
             self.bins = self._create_bins(self._gdf, self._column)
             if len(self.bins) <= self._k and len(self.bins) != len(self._unique_values):
                 self._k = len(self.bins)
-        else:
+        elif not all(self._gdf[self._column].isna()):
             self.bins = self._add_minmax_to_bins(self.bins)
             if len(self._unique_values) <= len(self.bins):
                 self._k = len(self.bins)  # - 1
+        else:
+            self._unique_values = self.nan_label
+            self._k = 1
 
     def _get_labels(self, gdfs: tuple[GeoDataFrame]) -> None:
         """Putting the labels/names in a list before copying the gdfs."""
         self.labels: list[str] = []
         for i, gdf in enumerate(gdfs):
             if hasattr(gdf, "name"):
                 name = gdf.name
@@ -270,18 +276,33 @@
                     gdf = gdf.to_crs(self.crs)
                 except ValueError:
                     gdf = gdf.set_crs(self.crs)
             new_gdfs.append(gdf)
         return new_gdfs
 
     def _fillna_if_col_is_missing(self) -> None:
+        n = 0
         for gdf in self._gdfs:
             if self._column in gdf.columns:
-                continue
-            gdf[self._column] = pd.NA
+                gdf[self._column] = gdf[self._column].fillna(pd.NA)
+                n += 1
+            else:
+                gdf[self._column] = pd.NA
+
+        maybe_area = 1 if "area" in self._column else 0
+        maybe_length = (
+            1 if any(x in self._column for x in ["meter", "metre", "leng"]) else 0
+        )
+        n = n + maybe_area + maybe_length
+
+        if n == 0:
+            raise ValueError(
+                f"The column {self._column!r} is not present in any "
+                "of the passed GeoDataFrames."
+            )
 
     def _check_if_categorical(self) -> bool:
         """Quite messy this..."""
         if not self._column:
             return True
 
         maybe_area = 1 if "area" in self._column else 0
@@ -366,14 +387,19 @@
 
         n_classes = (
             self._k if len(self._unique_values) > self._k else len(self._unique_values)
         )
 
         if self._k == len(self._unique_values) - 1:
             n_classes = self._k - 1
+            self._k = self._k - 1
+
+        if self._k > len(self._unique_values):
+            self._k = len(self._unique_values)
+            n_classes = len(self._unique_values)
 
         if self.scheme == "jenks":
             bins = jenks_breaks(gdf.loc[~self._nan_idx, column], n_classes=n_classes)
         else:
             binning = classify(
                 np.asarray(gdf.loc[~self._nan_idx, column]),
                 scheme=self.scheme,
@@ -387,14 +413,17 @@
 
         if self._k == len(self._unique_values) - 1:
             return np.array(unique_bins)
 
         if len(unique_bins) == len(self._unique_values):
             return np.array(unique_bins)
 
+        if len(unique_bins) == len(bins) - 1:
+            self._k -= 1
+
         return np.array(bins)
 
     def change_cmap(self, cmap: str, start: int = 0, stop: int = 256):
         """Change the color palette of the plot.
 
         Args:
             cmap: The colormap.
```

### Comparing `ssb_sgis-0.2.4/src/sgis/maps/maps.py` & `ssb_sgis-0.2.5/src/sgis/maps/maps.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 The 'qtm' function shows a simple static map of one or more GeoDataFrames.
 """
 from numbers import Number
 
 from geopandas import GeoDataFrame, GeoSeries
 from shapely import Geometry
 
-from ..geopandas_tools.general import clean_clip, random_points_in_polygons, to_gdf
+from ..geopandas_tools.general import clean_clip, to_gdf
 from ..geopandas_tools.geometry_types import get_geom_type
 from ..helpers import make_namedict
 from .explore import Explore
 from .map import Map
 from .thematicmap import ThematicMap
 
 
@@ -220,15 +220,15 @@
 
     Sample area with a radius of 5 kilometers.
 
     >>> samplemap(roads, points, size=5_000, column="meters")
 
     """
 
-    if not size and isinstance(gdfs[-1], (float, int)):
+    if isinstance(gdfs[-1], (float, int)):
         *gdfs, size = gdfs
 
     mask, kwargs = _get_mask(kwargs | {"size": size}, crs=gdfs[0].crs)
     kwargs.pop("size")
 
     if mask is not None:
         gdfs, column = Explore._separate_args(gdfs, column)
@@ -265,15 +265,15 @@
             sample = m._gdf.sample(1)
 
         # convert lines to polygons
         if get_geom_type(sample) == "line":
             sample["geometry"] = sample.buffer(1)
 
         if get_geom_type(sample) == "polygon":
-            random_point = random_points_in_polygons(sample, 1)
+            random_point = sample.sample_points(size=1)
 
         # if point or mixed geometries
         else:
             random_point = sample.centroid
 
         center = (random_point.geometry.iloc[0].x, random_point.geometry.iloc[0].y)
         print(f"center={center}, size={size}")
```

### Comparing `ssb_sgis-0.2.4/src/sgis/maps/thematicmap.py` & `ssb_sgis-0.2.5/src/sgis/maps/thematicmap.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/_get_route.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/_get_route.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/_od_cost_matrix.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/_od_cost_matrix.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/_points.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/_points.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/_service_area.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/_service_area.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/closing_network_holes.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/closing_network_holes.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/cutting_lines.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/cutting_lines.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import pandas as pd
 from geopandas import GeoDataFrame
 from pandas import DataFrame, Series
 from shapely import force_2d
 from shapely.geometry import LineString, Point
 
 from ..geopandas_tools.buffer_dissolve_explode import buff
+from ..geopandas_tools.geometry_types import get_geom_type
 from ..geopandas_tools.neighbors import get_k_nearest_neighbors
 from ..geopandas_tools.point_operations import snap_all, snap_within_distance
 from ..geopandas_tools.to_geodataframe import to_gdf
 from .nodes import make_edge_coords_cols
 
 
 def split_lines_by_nearest_point(
@@ -67,14 +68,20 @@
     of a line.
     """
     BUFFDIST = 0.000001
 
     if points.crs != gdf.crs:
         raise ValueError("crs mismatch:", points.crs, "and", gdf.crs)
 
+    if get_geom_type(gdf) != "line":
+        raise ValueError("'gdf' should only have line geometries.")
+
+    if get_geom_type(points) != "point":
+        raise ValueError("'points' should only have point geometries.")
+
     gdf["temp_idx_"] = gdf.index
 
     # move the points to the nearest exact point of the line
     if max_distance:
         snapped = snap_within_distance(points, gdf, max_distance=max_distance)
     else:
         snapped = snap_all(points, gdf)
@@ -188,14 +195,17 @@
     min           0.0
     25%           5.7
     50%          22.5
     75%          44.7
     max         100.0
     dtype: float64
     """
+    if get_geom_type(gdf) != "line":
+        raise ValueError("'gdf' should only have line geometries.")
+
     gdf["geometry"] = force_2d(gdf.geometry)
 
     gdf = gdf.explode(ignore_index=ignore_index, index_parts=False)
 
     long_lines = gdf.loc[gdf.length > max_length]
 
     if not len(long_lines):
```

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/directednetwork.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/directednetwork.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/finding_isolated_networks.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/finding_isolated_networks.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/network.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/network.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/networkanalysis.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysis.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/networkanalysisrules.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/networkanalysisrules.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/src/sgis/networkanalysis/nodes.py` & `ssb_sgis-0.2.5/src/sgis/networkanalysis/nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Returns:
         A tuple of two GeoDataFrames, one with the lines and one with the nodes.
 
     Note:
         The lines must be singlepart linestrings.
     """
 
-    gdf = gdf.explode(index_parts=False)
+    gdf = gdf.explode(index_parts=False).explode(index_parts=False)
 
     if wkt:
         gdf = make_edge_wkt_cols(gdf)
         geomcol1, geomcol2, geomcol_final = "source_wkt", "target_wkt", "wkt"
     else:
         gdf = make_edge_coords_cols(gdf)
         geomcol1, geomcol2, geomcol_final = "source_coords", "target_coords", "coords"
```

### Comparing `ssb_sgis-0.2.4/src/sgis/read_parquet.py` & `ssb_sgis-0.2.5/src/sgis/read_parquet.py`

 * *Files identical despite different names*

### Comparing `ssb_sgis-0.2.4/PKG-INFO` & `ssb_sgis-0.2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ssb-sgis
-Version: 0.2.4
+Version: 0.2.5
 Summary: GIS functions used at Statistics Norway.
 Home-page: https://github.com/statisticsnorway/ssb-sgis
 License: MIT
 Author: Statistics Norway
 Author-email: ort@ssb.no
 Requires-Python: >=3.10,<3.12
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: GIS
 Requires-Dist: branca (>=0.6.0)
 Requires-Dist: folium (>=0.14.0)
-Requires-Dist: geopandas (>=0.12.2)
+Requires-Dist: geopandas (>=0.13.0)
 Requires-Dist: igraph (>=0.10.4)
 Requires-Dist: ipython (>=8.13.2)
 Requires-Dist: jenkspy (>=0.3.2)
 Requires-Dist: mapclassify (>=2.5.0)
 Requires-Dist: matplotlib (>=3.7.0)
 Requires-Dist: networkx (>=3.0)
 Requires-Dist: numpy (>=1.24.2)
```

