# Comparing `tmp/hvplot-0.8.4a1.tar.gz` & `tmp/hvplot-0.8.5a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hvplot-0.8.4a1.tar", last modified: Mon Jun  5 17:06:56 2023, max compression
+gzip compressed data, was "dist/hvplot-0.8.5a1.tar", last modified: Thu Jun  8 11:12:34 2023, max compression
```

## Comparing `hvplot-0.8.4a1.tar` & `hvplot-0.8.5a1.tar`

### file list

```diff
@@ -1,203 +1,203 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/assets/streamz_demo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/datasets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/pandas/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/reference/xarray/vectorfield.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/examples/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/examples/user_guide/images/simple.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/.version
--rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/backend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    98207 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/cudf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/dask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/assets/
--rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/console.png
--rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/console_server.gif
--rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/diagram.svg
--rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/hvplot-wm.png
--rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/assets/streamz_demo.gif
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/data/crime.csv
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/datasets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/hvplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/getting_started/interactive.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/geopandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/geopandas/points.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/geopandas/polygons.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/andrewscurves.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/area.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/bar.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/barh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/bivariate.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/box.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/errorbars.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/heatmap.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/hexbin.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/hist.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/kde.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/labels.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/lagplot.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/line.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/ohlc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/parallelcoordinates.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/scatter.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/scattermatrix.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/step.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/table.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/pandas/violin.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/contour.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/contourf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/image.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/quadmesh.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/rgb.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/reference/xarray/vectorfield.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Customization.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Explorer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Geographic_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Gridded_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Interactive.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Introduction.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/NetworkX.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Pandas_API.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_Extensions.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Statistical_Plots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Streaming.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Subplots.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Timeseries_Data.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Viewing.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/Widgets.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/images/
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/examples/user_guide/images/simple.svg
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/ibis.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/intake.py
--rw-r--r--   0 runner    (1001) docker     (123)    36819 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/interactive.py
--rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/networkx.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/andrews_curves.py
--rw-r--r--   0 runner    (1001) docker     (123)    77101 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/core.py
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/lag_plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/parallel_coordinates.py
--rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/plotting/scatter_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/streamz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot/tests/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/plotting/testcore.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/plotting/testscattermatrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/test_links.py
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testbackend_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testcharts.py
--rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testgeo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testgridplots.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testhelp.py
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testibis.py
--rw-r--r--   0 runner    (1001) docker     (123)    41686 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testinteractive.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testnetworkx.py
--rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testoperations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testoptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testoverrides.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testpanel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testpatch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testplotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/teststreaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testtransforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testui.py
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/tests/testutil.py
--rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/ui.py
--rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/hvplot/xarray.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/hvplot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-05 17:06:56.000000 hvplot-0.8.4a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-05 17:01:14.000000 hvplot-0.8.4a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/assets/console.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/assets/console_server.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/assets/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/assets/diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/assets/hvplot-wm.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/assets/streamz_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/data/crime.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/datasets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/getting_started/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/getting_started/hvplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/getting_started/interactive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/reference/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/geopandas/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/geopandas/polygons.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/reference/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/andrewscurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/area.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/barh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/bivariate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/box.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/errorbars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/hexbin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/lagplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/ohlc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/parallelcoordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/scattermatrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/step.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/pandas/violin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/reference/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/xarray/contour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/xarray/contourf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/xarray/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/xarray/quadmesh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/xarray/rgb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/reference/xarray/vectorfield.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Customization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Geographic_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Gridded_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/NetworkX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Pandas_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Plotting_Extensions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Plotting_with_Matplotlib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Plotting_with_Plotly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Statistical_Plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Streaming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Timeseries_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/Widgets.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/examples/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/examples/user_guide/images/simple.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 11:12:33.000000 hvplot-0.8.5a1/hvplot/.version
+-rw-r--r--   0 runner    (1001) docker     (123)     9441 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10844 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/backend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    98200 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/cudf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/dask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)   359182 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/assets/console.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1080507 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/assets/console_server.gif
+-rw-r--r--   0 runner    (1001) docker     (123)   160622 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/assets/diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)   633920 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/assets/diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    16120 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/assets/hvplot-wm.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1007817 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/assets/streamz_demo.gif
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/data/crime.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/datasets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/getting_started/
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/getting_started/explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    10052 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/getting_started/hvplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6320 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/getting_started/interactive.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/reference/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/reference/geopandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/geopandas/points.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1620 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/geopandas/polygons.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/andrewscurves.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/area.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/bar.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/barh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/bivariate.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/box.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1703 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/errorbars.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2433 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/heatmap.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/hexbin.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/hist.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/kde.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/labels.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/lagplot.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/line.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2629 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/ohlc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/parallelcoordinates.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/scatter.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/scattermatrix.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/step.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/table.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/pandas/violin.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/contour.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/contourf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/image.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1472 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/quadmesh.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/rgb.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/reference/xarray/vectorfield.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Customization.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6582 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Explorer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    11740 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Geographic_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8635 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Gridded_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Interactive.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6819 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Introduction.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    25828 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/NetworkX.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    31612 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Pandas_API.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    22061 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7326 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting_Extensions.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23435 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23004 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4862 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Statistical_Plots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     9187 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Streaming.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Subplots.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Timeseries_Data.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5327 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Viewing.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5868 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/Widgets.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/images/
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/examples/user_guide/images/simple.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/ibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/intake.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36819 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/interactive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21358 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/networkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/pandas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/plotting/andrews_curves.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77101 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/plotting/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      961 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/plotting/lag_plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/plotting/parallel_coordinates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8739 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/plotting/scatter_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/streamz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot/tests/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/plotting/testcore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/plotting/testscattermatrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/test_links.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testbackend_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17267 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testcharts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11812 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11575 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testgridplots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testhelp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testibis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41686 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testinteractive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testnetworkx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10934 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testoperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22822 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testoptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testoverrides.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testpanel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testpatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2165 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testplotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/teststreaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testtransforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/tests/testutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23363 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17806 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1994 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/hvplot/xarray.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-08 11:12:33.000000 hvplot-0.8.5a1/hvplot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6340 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/hvplot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:12:33.000000 hvplot-0.8.5a1/hvplot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-08 11:12:33.000000 hvplot-0.8.5a1/hvplot.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-06-08 11:12:33.000000 hvplot-0.8.5a1/hvplot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 11:12:33.000000 hvplot-0.8.5a1/hvplot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-08 11:12:34.000000 hvplot-0.8.5a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5137 2023-06-08 11:05:30.000000 hvplot-0.8.5a1/setup.py
```

### Comparing `hvplot-0.8.4a1/LICENSE` & `hvplot-0.8.5a1/LICENSE`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/PKG-INFO` & `hvplot-0.8.5a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvplot
-Version: 0.8.4a1
+Version: 0.8.5a1
 Summary: A high-level plotting API for the PyData ecosystem built on HoloViews.
 Home-page: https://hvplot.pyviz.org
 Author: Philipp Rudiger
 Author-email: developers@pyviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD
```

### Comparing `hvplot-0.8.4a1/README.md` & `hvplot-0.8.5a1/README.md`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/assets/console.png` & `hvplot-0.8.5a1/examples/assets/console.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/assets/console_server.gif` & `hvplot-0.8.5a1/examples/assets/console_server.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/assets/diagram.png` & `hvplot-0.8.5a1/examples/assets/diagram.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/assets/diagram.svg` & `hvplot-0.8.5a1/examples/assets/diagram.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/assets/hvplot-wm.png` & `hvplot-0.8.5a1/examples/assets/hvplot-wm.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/assets/streamz_demo.gif` & `hvplot-0.8.5a1/examples/assets/streamz_demo.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/data/crime.csv` & `hvplot-0.8.5a1/examples/data/crime.csv`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/datasets.yaml` & `hvplot-0.8.5a1/examples/datasets.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/getting_started/explorer.ipynb` & `hvplot-0.8.5a1/examples/getting_started/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/getting_started/hvplot.ipynb` & `hvplot-0.8.5a1/examples/getting_started/hvplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/getting_started/interactive.ipynb` & `hvplot-0.8.5a1/examples/getting_started/interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/geopandas/points.ipynb` & `hvplot-0.8.5a1/examples/reference/geopandas/points.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/geopandas/polygons.ipynb` & `hvplot-0.8.5a1/examples/reference/geopandas/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/andrewscurves.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/andrewscurves.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/area.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/area.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/bar.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/bar.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/barh.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/barh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/bivariate.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/bivariate.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/box.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/box.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/errorbars.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/errorbars.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/heatmap.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/hexbin.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/hexbin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/hist.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/hist.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/kde.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/kde.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/labels.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/labels.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/lagplot.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/lagplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/line.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/line.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/ohlc.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/ohlc.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/parallelcoordinates.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/parallelcoordinates.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/scatter.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/scatter.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/scattermatrix.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/scattermatrix.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/step.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/step.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/table.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/table.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/pandas/violin.ipynb` & `hvplot-0.8.5a1/examples/reference/pandas/violin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/xarray/contour.ipynb` & `hvplot-0.8.5a1/examples/reference/xarray/contour.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/xarray/contourf.ipynb` & `hvplot-0.8.5a1/examples/reference/xarray/contourf.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/xarray/image.ipynb` & `hvplot-0.8.5a1/examples/reference/xarray/image.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/xarray/quadmesh.ipynb` & `hvplot-0.8.5a1/examples/reference/xarray/quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/xarray/rgb.ipynb` & `hvplot-0.8.5a1/examples/reference/xarray/rgb.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/reference/xarray/vectorfield.ipynb` & `hvplot-0.8.5a1/examples/reference/xarray/vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Customization.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Customization.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Explorer.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Geographic_Data.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Geographic_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Gridded_Data.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Gridded_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Interactive.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Introduction.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/NetworkX.ipynb` & `hvplot-0.8.5a1/examples/user_guide/NetworkX.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Pandas_API.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Pandas_API.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Plotting.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Plotting_Extensions.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Plotting_Extensions.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Plotting_with_Matplotlib.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Plotting_with_Matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Plotting_with_Plotly.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Plotting_with_Plotly.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Statistical_Plots.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Statistical_Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Streaming.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Streaming.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Subplots.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Subplots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Timeseries_Data.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Timeseries_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Viewing.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Viewing.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/Widgets.ipynb` & `hvplot-0.8.5a1/examples/user_guide/Widgets.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/examples/user_guide/images/simple.svg` & `hvplot-0.8.5a1/examples/user_guide/images/simple.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/__init__.py` & `hvplot-0.8.5a1/hvplot/__init__.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/backend_transforms.py` & `hvplot-0.8.5a1/hvplot/backend_transforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/converter.py` & `hvplot-0.8.5a1/hvplot/converter.py`

 * *Files 0% similar despite different names*

```diff
@@ -393,15 +393,15 @@
         self._process_data(
             kind, data, x, y, by, groupby, row, col, use_dask,
             persist, backlog, label, group_label, value_label,
             hover_cols, attr_labels, transforms, stream, kwds
         )
 
         self.dynamic = dynamic
-        self.geo = any([geo, crs, global_extent, projection, project, coastline, features, tiles])
+        self.geo = any([geo, crs, global_extent, projection, project, coastline, features])
         self.crs = self._process_crs(data, crs) if self.geo else None
         self.project = project
         self.coastline = coastline
         self.features = features
         self.tiles = tiles
         self.sort_date = sort_date
```

### Comparing `hvplot-0.8.4a1/hvplot/cudf.py` & `hvplot-0.8.5a1/hvplot/cudf.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/dask.py` & `hvplot-0.8.5a1/hvplot/dask.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/assets/console.png` & `hvplot-0.8.5a1/hvplot/examples/assets/console.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/assets/console_server.gif` & `hvplot-0.8.5a1/hvplot/examples/assets/console_server.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/assets/diagram.png` & `hvplot-0.8.5a1/hvplot/examples/assets/diagram.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/assets/diagram.svg` & `hvplot-0.8.5a1/hvplot/examples/assets/diagram.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/assets/hvplot-wm.png` & `hvplot-0.8.5a1/hvplot/examples/assets/hvplot-wm.png`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/assets/streamz_demo.gif` & `hvplot-0.8.5a1/hvplot/examples/assets/streamz_demo.gif`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/data/crime.csv` & `hvplot-0.8.5a1/hvplot/examples/data/crime.csv`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/datasets.yaml` & `hvplot-0.8.5a1/hvplot/examples/datasets.yaml`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/getting_started/explorer.ipynb` & `hvplot-0.8.5a1/hvplot/examples/getting_started/explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/getting_started/hvplot.ipynb` & `hvplot-0.8.5a1/hvplot/examples/getting_started/hvplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/getting_started/interactive.ipynb` & `hvplot-0.8.5a1/hvplot/examples/getting_started/interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/geopandas/points.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/geopandas/points.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/geopandas/polygons.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/geopandas/polygons.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/andrewscurves.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/andrewscurves.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/area.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/area.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/bar.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/bar.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/barh.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/barh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/bivariate.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/bivariate.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/box.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/box.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/errorbars.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/errorbars.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/heatmap.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/heatmap.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/hexbin.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/hexbin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/hist.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/hist.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/kde.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/kde.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/labels.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/labels.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/lagplot.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/lagplot.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/line.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/line.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/ohlc.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/ohlc.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/parallelcoordinates.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/parallelcoordinates.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/scatter.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/scatter.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/scattermatrix.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/scattermatrix.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/step.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/step.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/table.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/table.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/pandas/violin.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/pandas/violin.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/xarray/contour.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/xarray/contour.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/xarray/contourf.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/xarray/contourf.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/xarray/image.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/xarray/image.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/xarray/quadmesh.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/xarray/quadmesh.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/xarray/rgb.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/xarray/rgb.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/reference/xarray/vectorfield.ipynb` & `hvplot-0.8.5a1/hvplot/examples/reference/xarray/vectorfield.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Customization.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Customization.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Explorer.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Explorer.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Geographic_Data.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Geographic_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Gridded_Data.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Gridded_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Interactive.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Interactive.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Introduction.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Introduction.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/NetworkX.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/NetworkX.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Pandas_API.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Pandas_API.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_Extensions.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting_Extensions.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting_with_Matplotlib.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Plotting_with_Plotly.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Statistical_Plots.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Statistical_Plots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Streaming.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Streaming.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Subplots.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Subplots.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Timeseries_Data.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Timeseries_Data.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Viewing.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Viewing.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/Widgets.ipynb` & `hvplot-0.8.5a1/hvplot/examples/user_guide/Widgets.ipynb`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/examples/user_guide/images/simple.svg` & `hvplot-0.8.5a1/hvplot/examples/user_guide/images/simple.svg`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/intake.py` & `hvplot-0.8.5a1/hvplot/intake.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/interactive.py` & `hvplot-0.8.5a1/hvplot/interactive.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/networkx.py` & `hvplot-0.8.5a1/hvplot/networkx.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/pandas.py` & `hvplot-0.8.5a1/hvplot/pandas.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/plotting/__init__.py` & `hvplot-0.8.5a1/hvplot/plotting/__init__.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/plotting/andrews_curves.py` & `hvplot-0.8.5a1/hvplot/plotting/andrews_curves.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/plotting/core.py` & `hvplot-0.8.5a1/hvplot/plotting/core.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/plotting/lag_plot.py` & `hvplot-0.8.5a1/hvplot/plotting/lag_plot.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/plotting/parallel_coordinates.py` & `hvplot-0.8.5a1/hvplot/plotting/parallel_coordinates.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/plotting/scatter_matrix.py` & `hvplot-0.8.5a1/hvplot/plotting/scatter_matrix.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/sample_data.py` & `hvplot-0.8.5a1/hvplot/sample_data.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/streamz.py` & `hvplot-0.8.5a1/hvplot/streamz.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/plotting/testcore.py` & `hvplot-0.8.5a1/hvplot/tests/plotting/testcore.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/plotting/testscattermatrix.py` & `hvplot-0.8.5a1/hvplot/tests/plotting/testscattermatrix.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/test_links.py` & `hvplot-0.8.5a1/hvplot/tests/test_links.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testbackend_transforms.py` & `hvplot-0.8.5a1/hvplot/tests/testbackend_transforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testcharts.py` & `hvplot-0.8.5a1/hvplot/tests/testcharts.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testgeo.py` & `hvplot-0.8.5a1/hvplot/tests/testgeo.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testgridplots.py` & `hvplot-0.8.5a1/hvplot/tests/testgridplots.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testhelp.py` & `hvplot-0.8.5a1/hvplot/tests/testhelp.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testinteractive.py` & `hvplot-0.8.5a1/hvplot/tests/testinteractive.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testnetworkx.py` & `hvplot-0.8.5a1/hvplot/tests/testnetworkx.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testoperations.py` & `hvplot-0.8.5a1/hvplot/tests/testoperations.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testoptions.py` & `hvplot-0.8.5a1/hvplot/tests/testoptions.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testoverrides.py` & `hvplot-0.8.5a1/hvplot/tests/testoverrides.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testpanel.py` & `hvplot-0.8.5a1/hvplot/tests/testpanel.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testpatch.py` & `hvplot-0.8.5a1/hvplot/tests/testpatch.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testplotting.py` & `hvplot-0.8.5a1/hvplot/tests/testplotting.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/teststreaming.py` & `hvplot-0.8.5a1/hvplot/tests/teststreaming.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testtransforms.py` & `hvplot-0.8.5a1/hvplot/tests/testtransforms.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testui.py` & `hvplot-0.8.5a1/hvplot/tests/testui.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/tests/testutil.py` & `hvplot-0.8.5a1/hvplot/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/ui.py` & `hvplot-0.8.5a1/hvplot/ui.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/util.py` & `hvplot-0.8.5a1/hvplot/util.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/utilities.py` & `hvplot-0.8.5a1/hvplot/utilities.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot/xarray.py` & `hvplot-0.8.5a1/hvplot/xarray.py`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot.egg-info/PKG-INFO` & `hvplot-0.8.5a1/hvplot.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hvplot
-Version: 0.8.4a1
+Version: 0.8.5a1
 Summary: A high-level plotting API for the PyData ecosystem built on HoloViews.
 Home-page: https://hvplot.pyviz.org
 Author: Philipp Rudiger
 Author-email: developers@pyviz.org
 Maintainer: HoloViz developers
 Maintainer-email: developers@pyviz.org
 License: BSD
```

### Comparing `hvplot-0.8.4a1/hvplot.egg-info/SOURCES.txt` & `hvplot-0.8.5a1/hvplot.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/hvplot.egg-info/requires.txt` & `hvplot-0.8.5a1/hvplot.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `hvplot-0.8.4a1/setup.py` & `hvplot-0.8.5a1/setup.py`

 * *Files identical despite different names*

