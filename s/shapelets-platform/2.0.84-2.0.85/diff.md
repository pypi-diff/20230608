# Comparing `tmp/shapelets-platform-2.0.84.tar.gz` & `tmp/shapelets-platform-2.0.85.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shapelets-platform-2.0.84.tar", last modified: Fri May 19 10:51:28 2023, max compression
+gzip compressed data, was "shapelets-platform-2.0.85.tar", last modified: Thu Jun  8 11:01:24 2023, max compression
```

## Comparing `shapelets-platform-2.0.84.tar` & `shapelets-platform-2.0.85.tar`

### file list

```diff
@@ -1,291 +1,295 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/
--rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/COPYING.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/LICENSE.md
--rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/noxfile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (123)     3007 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.102965 shapelets-platform-2.0.84/src/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.110965 shapelets-platform-2.0.84/src/shapelets/
--rw-r--r--   0 vsts      (1001) docker     (123)      608 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/__main__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6366 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_api.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_cli.py
--rw-r--r--   0 vsts      (1001) docker     (123)    51826 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_relations.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_uom.py
--rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets/_version.py
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/_version.pyi
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.110965 shapelets-platform-2.0.84/src/shapelets/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    62329 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/data_app.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/data_app_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.114965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/
--rw-r--r--   0 vsts      (1001) docker     (123)      713 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2910 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/attribute_names.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.118965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/
--rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/altair_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/bar_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/folium_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/heatmap.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/histogram.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18963 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/line_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/pie_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/plotly_chart.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/polar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/radar_area.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/scatter_plot.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.118965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/
--rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/filtering_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_field.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_filter.py
--rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/temporal_context.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.126965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/
--rw-r--r--   0 vsts      (1001) docker     (123)     1177 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1483 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/button.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4400 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/checkbox.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/collection_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7465 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8049 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/number_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7362 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/progress.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9851 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/radio_group.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.126965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/resources/
--rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
--rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_list.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_selector.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14796 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/slider.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4389 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/table.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text_input.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/timer.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/datetime_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.130965 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/
--rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/grid_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6028 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/horizontal_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/panel.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4987 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/tabs_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5654 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/vertical_layout.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1631 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/util.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24282 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/apps/widgets/widget.py
--rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/iris.csv
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.134965 shapelets-platform-2.0.84/src/shapelets/model/
--rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/altair.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/capsule.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/collection.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/dataframe.py
--rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/function_description.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/function_parameter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/group.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/image.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/metadata_item.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/model.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/ndarray.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/permissions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/replicated_param.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/sequence.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/sequence_axis.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/user.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/model/view_match.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/py.typed
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.138965 shapelets-platform-2.0.84/src/shapelets/svr/
--rw-r--r--   0 vsts      (1001) docker     (123)    10259 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/app.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.138965 shapelets-platform-2.0.84/src/shapelets/svr/authn/
--rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8713 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/authhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8411 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/authrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9640 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/authservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/gc_client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2147 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8961 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.138965 shapelets-platform-2.0.84/src/shapelets/svr/data/
--rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.146965 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/
--rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/access_token_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen2.py
--rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/driver.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/dynamic_credentials.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/ftp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/local.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/protocols.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/smb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/vfs_sample_config.toml
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.146965 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/
--rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataapps_ws.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6025 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9130 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2226 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1515 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1260 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.154965 shapelets-platform-2.0.84/src/shapelets/svr/db/
--rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.154965 shapelets-platform-2.0.84/src/shapelets/svr/db/native/
--rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/native/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/native/database.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/native/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_builder.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3858 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v1.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v3.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/db/setup.py
--rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/docs.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.158965 shapelets-platform-2.0.84/src/shapelets/svr/execution/
--rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1296 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/executionhttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/executionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1033 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/executionservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/iexecutionrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      385 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/execution/iexecutionservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.162965 shapelets-platform-2.0.84/src/shapelets/svr/groups/
--rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/groupservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3770 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/groupshttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4753 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/groupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2094 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2626 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.162965 shapelets-platform-2.0.84/src/shapelets/svr/model/
--rw-r--r--   0 vsts      (1001) docker     (123)      350 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      631 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/dataapps.py
--rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/function.py
--rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/groups.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/principals.py
--rw-r--r--   0 vsts      (1001) docker     (123)      993 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/model/users.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.166965 shapelets-platform-2.0.84/src/shapelets/svr/mustang/
--rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/asttranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/conversions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/core.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/decompiling.py
--rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/hashdict.py
--rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/identifier.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/ormtypes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.170965 shapelets-platform-2.0.84/src/shapelets/svr/mustang/prototypes/
--rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/prototypes/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/python_versions.py
--rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/serialization.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqlbuilding.py
--rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqltranslation.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/server.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.174965 shapelets-platform-2.0.84/src/shapelets/svr/settings/
--rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/client.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/defaults.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/functions.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/http.py
--rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/reload.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/server.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.toml
--rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/ssl.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/telemetry.py
--rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/settings/websocket.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.174965 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/
--rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/itelemetryservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/sysinfo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/telemetry/telemetryservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.178965 shapelets-platform-2.0.84/src/shapelets/svr/users/
--rw-r--r--   0 vsts      (1001) docker     (123)      732 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/http_docs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2248 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/iusersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1827 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/iusersservice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3802 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/usershttp.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9016 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/usersrepo.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3233 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/users/usersservice.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.178965 shapelets-platform-2.0.84/src/shapelets/svr/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/utils/crypto.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/svr/utils/flexbytes.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.178965 shapelets-platform-2.0.84/src/shapelets/svr/www/
--rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/altair.json
--rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/asset-manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/dataapp.json
--rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/favicon.ico
--rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/index.html
--rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/manifest.json
--rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/robots.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.102965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.182965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/
--rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
--rw-r--r--   0 vsts      (1001) docker     (123)    79553 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/main.8349d999.chunk.css
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.190965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/
--rw-r--r--   0 vsts      (1001) docker     (123)  6284390 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   173518 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/4.77242983.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/4.77242983.chunk.js.LICENSE.txt
--rw-r--r--   0 vsts      (1001) docker     (123)   813635 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js
--rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/
--rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/audit.cb539a06.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/bin.7e762965.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/clear.27b15301.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/download-image.87310709.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/filter.cec803b8.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
--rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
--rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logout.57c593a5.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/share.bc9a8370.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
--rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
--rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
--rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
--rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-05-19 10:51:22.000000 shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
--rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-05-19 10:33:32.000000 shapelets-platform-2.0.84/src/shapelets/systemd_template.txt
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-19 10:51:28.194965 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)    11228 2023-05-19 10:51:28.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (123)     1250 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-05-19 10:51:24.000000 shapelets-platform-2.0.84/src/shapelets_platform.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/
+-rw-r--r--   0 vsts      (1001) docker     (123)      134 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/COPYING.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1140 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/LICENSE.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      144 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     4546 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)     1562 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/noxfile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1219 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)     3068 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4030 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.020513 shapelets-platform-2.0.85/src/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.028513 shapelets-platform-2.0.85/src/shapelets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      891 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)       60 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/__main__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8472 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_api.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19249 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_cli.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    51403 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_relations.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4154 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_uom.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      162 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets/_version.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/_version.pyi
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.028513 shapelets-platform-2.0.85/src/shapelets/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      242 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    68076 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/data_app.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4112 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/data_app_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.032513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/
+-rw-r--r--   0 vsts      (1001) docker     (123)      752 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3123 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/attribute_names.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.036513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      744 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3273 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/altair_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/bar_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2602 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/folium_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2500 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/heatmap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/histogram.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19053 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/line_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2028 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/pie_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1159 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/plotly_chart.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2039 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/polar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2937 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/radar_area.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4186 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/scatter_plot.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.036513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      496 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1167 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/filtering_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1106 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_field.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1437 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_filter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      721 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/temporal_context.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.044513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1357 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1996 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/button.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4503 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/checkbox.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2151 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/collection_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7465 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_range_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8050 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4164 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/gauge.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8263 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1315 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5978 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/metric.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2022 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11087 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/number_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7391 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/progress.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9880 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/radio_group.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.044513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/resources/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18534 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg
+-rw-r--r--   0 vsts      (1001) docker     (123)     4678 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/ring.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    10639 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1818 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_list.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1843 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_selector.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14796 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/slider.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8253 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/table.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5969 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9070 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text_input.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5622 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/timer.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4460 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/datetime_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.048513 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/
+-rw-r--r--   0 vsts      (1001) docker     (123)      359 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1975 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/grid_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6057 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/horizontal_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1464 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/panel.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5016 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/tabs_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5683 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/vertical_layout.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2756 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/util.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24284 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/apps/widgets/widget.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      736 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4551 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/iris.csv
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.052513 shapelets-platform-2.0.85/src/shapelets/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1463 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1084 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/altair.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1523 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/capsule.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4487 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/collection.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4297 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/dataframe.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      260 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3472 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/function_description.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2625 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/function_parameter.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1252 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/group.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2214 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/image.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4992 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/metadata_item.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2749 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/model.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2666 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/ndarray.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2360 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/permissions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/replicated_param.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5553 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/sequence.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2292 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/sequence_axis.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1869 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/user.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4446 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/model/view_match.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/py.typed
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.052513 shapelets-platform-2.0.85/src/shapelets/svr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10262 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2459 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/app.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.056513 shapelets-platform-2.0.85/src/shapelets/svr/authn/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2484 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8820 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/authhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9843 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/authrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9665 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/authservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5550 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/gc_client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2162 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8976 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.056513 shapelets-platform-2.0.85/src/shapelets/svr/data/
+-rw-r--r--   0 vsts      (1001) docker     (123)    19485 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.060513 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/
+-rw-r--r--   0 vsts      (1001) docker     (123)     7227 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      841 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/access_token_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3381 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5728 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      799 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/driver.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1311 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/dynamic_credentials.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1756 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4266 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2429 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3806 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_file.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2814 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/ftp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1837 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/local.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2029 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/protocols.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3512 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/smb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3562 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/vfs_sample_config.toml
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.064513 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/
+-rw-r--r--   0 vsts      (1001) docker     (123)      792 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3116 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataapps_ws.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9309 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    25604 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2439 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1781 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1507 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.068513 shapelets-platform-2.0.85/src/shapelets/svr/db/
+-rw-r--r--   0 vsts      (1001) docker     (123)      233 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.068513 shapelets-platform-2.0.85/src/shapelets/svr/db/native/
+-rw-r--r--   0 vsts      (1001) docker     (123)      235 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/native/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9162 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/native/database.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2242 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/native/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      811 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_builder.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3449 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v1.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3517 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3956 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v3.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5579 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v4.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2021 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/db/setup.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      509 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/docs.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.068513 shapelets-platform-2.0.85/src/shapelets/svr/execution/
+-rw-r--r--   0 vsts      (1001) docker     (123)      812 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1710 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/executionhttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      319 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/executionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1854 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/executionservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      265 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/iexecutionrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      337 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/execution/iexecutionservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.072513 shapelets-platform-2.0.85/src/shapelets/svr/groups/
+-rw-r--r--   0 vsts      (1001) docker     (123)      788 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1596 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/groupservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4374 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/groupshttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4754 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/groupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      458 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1968 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2626 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.072513 shapelets-platform-2.0.85/src/shapelets/svr/model/
+-rw-r--r--   0 vsts      (1001) docker     (123)      369 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      826 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/dataapps.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      179 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/function.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      415 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/groups.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2354 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/principals.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      867 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/model/users.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.080513 shapelets-platform-2.0.85/src/shapelets/svr/mustang/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2474 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18919 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/asttranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/conversions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12907 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/core.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    35472 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/decompiling.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      874 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/exceptions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1293 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/hashdict.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      121 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/identifier.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5662 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/ormtypes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.080513 shapelets-platform-2.0.85/src/shapelets/svr/mustang/prototypes/
+-rw-r--r--   0 vsts      (1001) docker     (123)    18157 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/prototypes/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      267 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/python_versions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      591 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/serialization.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11997 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqlbuilding.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    66067 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqltranslation.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4102 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/server.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.084513 shapelets-platform-2.0.85/src/shapelets/svr/settings/
+-rw-r--r--   0 vsts      (1001) docker     (123)      650 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5189 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/client.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2155 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/defaults.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2158 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/functions.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1024 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/http.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      707 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/reload.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6905 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/server.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6374 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5534 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.toml
+-rw-r--r--   0 vsts      (1001) docker     (123)      815 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/ssl.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1107 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/telemetry.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      758 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/settings/websocket.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.084513 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/
+-rw-r--r--   0 vsts      (1001) docker     (123)      329 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      140 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/itelemetryservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2613 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/sysinfo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1778 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/telemetry/telemetryservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.088513 shapelets-platform-2.0.85/src/shapelets/svr/users/
+-rw-r--r--   0 vsts      (1001) docker     (123)      685 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      705 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/http_docs.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2358 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/iusersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2653 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/iusersservice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5587 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/usershttp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    13629 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/usersrepo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3582 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/users/usersservice.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.092513 shapelets-platform-2.0.85/src/shapelets/svr/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)       88 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6279 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/utils/crypto.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1677 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/svr/utils/flexbytes.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.092513 shapelets-platform-2.0.85/src/shapelets/svr/www/
+-rw-r--r--   0 vsts      (1001) docker     (123)   136375 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/altair.json
+-rw-r--r--   0 vsts      (1001) docker     (123)     4655 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/asset-manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)   109691 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/dataapp.json
+-rw-r--r--   0 vsts      (1001) docker     (123)    17042 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/favicon.ico
+-rw-r--r--   0 vsts      (1001) docker     (123)     4111 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/index.html
+-rw-r--r--   0 vsts      (1001) docker     (123)      292 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/manifest.json
+-rw-r--r--   0 vsts      (1001) docker     (123)       67 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/robots.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.020513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.096513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/
+-rw-r--r--   0 vsts      (1001) docker     (123)    90519 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css
+-rw-r--r--   0 vsts      (1001) docker     (123)    79553 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/main.8349d999.chunk.css
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.104513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/
+-rw-r--r--   0 vsts      (1001) docker     (123)  6284390 2023-06-08 11:01:19.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)    15949 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   173518 2023-06-08 11:01:19.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      808 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)    21772 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/4.77242983.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)      188 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/4.77242983.chunk.js.LICENSE.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)   813635 2023-06-08 11:01:19.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js
+-rw-r--r--   0 vsts      (1001) docker     (123)     2357 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.112513 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/
+-rw-r--r--   0 vsts      (1001) docker     (123)      771 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1155 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/audit.cb539a06.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1129 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/bin.7e762965.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1274 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      918 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/clear.27b15301.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2092 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/collections.06fdf54a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1432 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3206 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3225 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2684 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1493 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-time.a1e86419.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1047 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/download-image.87310709.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      828 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/filter.cec803b8.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1609 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1531 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1476 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      852 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    21416 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    15532 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    15668 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png
+-rw-r--r--   0 vsts      (1001) docker     (123)     1265 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logout.57c593a5.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1091 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      958 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1035 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2616 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2628 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf.5d189efa.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      536 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3530 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     2319 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      429 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-vertical-line.2ebc031a.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      935 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/share.bc9a8370.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      868 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1004 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/single-plot.864a583b.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)     3704 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)      521 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg
+-rw-r--r--   0 vsts      (1001) docker     (123)    19199 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png
+-rw-r--r--   0 vsts      (1001) docker     (123)    18616 2023-06-08 11:01:18.000000 shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-top.6d51781b.png
+-rw-r--r--   0 vsts      (1001) docker     (123)      376 2023-06-08 10:43:50.000000 shapelets-platform-2.0.85/src/shapelets/systemd_template.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-08 11:01:24.116513 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6303 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)    11406 2023-06-08 11:01:23.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       44 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)     1305 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)       10 2023-06-08 11:01:20.000000 shapelets-platform-2.0.85/src/shapelets_platform.egg-info/top_level.txt
```

### Comparing `shapelets-platform-2.0.84/LICENSE.md` & `shapelets-platform-2.0.85/LICENSE.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/PKG-INFO` & `shapelets-platform-2.0.85/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.84
+Version: 2.0.85
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.84/README.md` & `shapelets-platform-2.0.85/README.md`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/noxfile.py` & `shapelets-platform-2.0.85/noxfile.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/pyproject.toml` & `shapelets-platform-2.0.85/pyproject.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/setup.cfg` & `shapelets-platform-2.0.85/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -49,27 +49,29 @@
 	jinja2 == 3.0.2
 	jmespath ~= 0.9.3
 	matplotlib >= 3.5.3
 	mypy ~= 0.990
 	numpy >=1.21.6
 	pandas >=1.3.5
 	psutil >= 5.9.2
-	pyarrow >=9.0.0
+	pyarrow >=12.0.0
 	py-cpuinfo>=9.0.0
 	pydantic >= 1.10.2
 	pygeohash >= 1.2.0
 	PyNaCl >= 1.5.0
 	requests >= 2.28.1
-	shapelets_native == 2.0.84
+	setuptools-scm >= 7.1.0
+	shapelets_native == 2.0.85
 	tabulate>=0.8.10
 	tomlkit >= 0.11.4
 	tqdm >= 4.64.1
+	typing_extensions >= 4.6.2
 	uvicorn >= 0.18.3
 	vega-datasets >= 0.9
-	websocket >= 0.2.1
+	websocket-client >= 1.5.2
 	websockets >= 10.3
 	lockfile >= 0.12.2; platform_system!="Windows"
 	python_daemon >= 2.3.2; platform_system!="Windows"
 	uvloop >= 0.17.0; platform_system!="Windows"
 python_requires = >=3.7
 include_package_data = True
 package_dir =
```

### Comparing `shapelets-platform-2.0.84/setup.py` & `shapelets-platform-2.0.85/setup.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/_api.py` & `shapelets-platform-2.0.85/src/shapelets/_api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import os
 
-from typing import Optional
+from typing import List, Optional, Union
 from typing_extensions import Literal
 from requests import Session
 
 from .svr import (
     gc_flow, get_service, get_service_optional, defaults,
     crypto,
-    UserAttributes, IAuthService, Settings, IAuthService,
-    PrefixedSession)
+    UserAttributes, Settings, IAuthService, IGroupsService, GroupProfile,
+    IUsersService,
+    PrefixedSession, UserProfile)
 
 EnterpriseLoginType = Literal['azure', 'linkedin', 'google', 'github']
 
 
 def forget_me():
     """
     Forgets credentials stored in configuration files 
@@ -106,15 +107,16 @@
         defaults(signed_token=signed_token)
 
     session: PrefixedSession = get_service_optional(Session)
     if session is not None:
         session.set_authorization(signed_token)
 
 
-def register(user_name: str, password: str, user_details: Optional[UserAttributes] = None, also_login: bool = True, remember_me: bool = True, force: bool = False):
+def register(user_name: str, password: str, user_details: Optional[UserAttributes] = None, also_login: bool = True,
+             remember_me: bool = True, force: bool = False):
     """
     Registers a new user in Shapelets
 
     Parameters
     ----------
     user_name: str, required
         New user name.  This name should be unique in the system
@@ -148,23 +150,99 @@
     pk = crypto.derive_verify_key(salt, password.encode('ascii'))
     if not auth_svc.register(user_name, salt, pk, user_details):
         raise RuntimeError("Unable to register a new user")
 
     if also_login:
         login(user_name=user_name, password=password, remember_me=remember_me)
 
-def unregister(user_name: str):
+
+def unregister(user_name: str, transfer: str = None):
     """
     Unregisters an existing user in Shapelets
 
     Parameters
     ----------
     user_name: str, required
         Existing user name.
+
+    transfer: str, optional
+        Provide a username to give ownership of all dataApps belonging to the user to be deleted that this user shared with any group.
+        Note: all dataApps not shared with any group will be deleted, as the only belong to the user local space.
+
     """
-    auth_svc = get_service(IAuthService)
-    if auth_svc.user_name_exists(user_name):
-        result = auth_svc.remove_user(user_name)
-        if not result:
-            raise ValueError("Error happens while removing user name")
-    else:
-        raise ValueError("User does not exist. Unable to unregister user name")
+    try:
+        auth_svc = get_service(IAuthService)
+        if auth_svc.user_name_exists(user_name):
+            result = auth_svc.remove_user(user_name, transfer)
+            if not result:
+                raise ValueError("Error happens while removing user name")
+        else:
+            raise ValueError("User does not exist. Unable to unregister user name")
+    except Exception as e:
+        print(e)
+
+
+def list_current_groups() -> List[GroupProfile]:
+    """
+    List current groups available
+    """
+    groups_svc = get_service(IGroupsService)
+    return groups_svc.get_all()
+
+
+def list_current_users() -> List[UserProfile]:
+    """
+    List current users registered in Shapelets
+    """
+    user_svr = get_service(IUsersService)
+    return user_svr.get_all()
+
+
+def create_group(group_name: str, description: str = None) -> GroupProfile:
+    """
+    Create a new group for Shapelets
+
+    Parameters
+    ----------
+    group_name: str, required
+        Group name.
+
+    description: str, optional
+        Group description.
+    """
+    groups_svc = get_service(IGroupsService)
+    return groups_svc.create(group_name, description)
+
+
+def add_user_to_group(user_name: str, groups: Union[List[str], str], write: bool = False):
+    """
+    Add a Shapelets user to an existed group
+
+    Parameters
+    ----------
+    user_name: str, required
+        User name.
+
+    groups: str, optional
+        List of group names where the user will be added.
+
+    write: bool, optional
+        Give user permission to modify dataApps from the group.
+    """
+    user_svr = get_service(IUsersService)
+    user_svr.add_to_group(user_name, groups, write)
+
+
+def remove_user_from_group(user_name: str, groups: Union[List[str], str]):
+    """
+    Remove a Shapelets user from the giving group/s
+
+    Parameters
+    ----------
+    user_name: str, required
+        User name.
+
+    groups: str, optional
+        List of group names where the user will be removed.
+    """
+    user_svr = get_service(IUsersService)
+    user_svr.remove_from_group(user_name, groups)
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/_cli.py` & `shapelets-platform-2.0.85/src/shapelets/_cli.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/_relations.py` & `shapelets-platform-2.0.85/src/shapelets/_relations.py`

 * *Files 4% similar despite different names*

```diff
@@ -878,64 +878,58 @@
                    6.3            2.5             5              1.9  Iris-virginica
                    6.5            3               5.2            2    Iris-virginica
                    6.2            3.4             5.4            2.3  Iris-virginica
                    5.9            3               5.1            1.8  Iris-virginica
 
         [150 rows x 5 columns]
         """
-        rows, cols = self.shape()
-        if len(self) > 10:
-            # If more than 10 rows, print head and tail
-            head = self.head()
-            tail = self.tail()
-            if cols > 10:
-                # Reduce amount of columns showed
-                column_names = head.select_columns(
-                    [0, 1, 2, 3, 4, cols - 5, cols - 4, cols - 3, cols - 2, cols - 1]).columns
-                col_types = list(head.select_columns(column_names).describe()["column_type"])
-                head_list = head.select_columns(column_names).__rel.execute().fetch_all()
-                tail_list = tail.select_columns(column_names).__rel.execute().fetch_all()
-                self._add_reduced_col(head_list)
-                self._add_reduced_col(tail_list)
+        cols = len(self.columns)
+        if cols > 10:
+            filter_data = self.select_columns(
+                [0, 1, 2, 3, 4, cols - 5, cols - 4, cols - 3, cols - 2, cols - 1])
+            column_names = filter_data.columns
+            col_types = [self.schema[x][1] for x in column_names]
+            data = filter_data.__rel.execute().fetch_all()
+            rows = len(data)
+            if rows > 10:
+                head = data[:5]
+                tail = data[-5:]
+                self._add_reduced_col(head)
+                self._add_reduced_col(tail)
                 column_names.insert(5, "...")
                 col_types.insert(5, "...")
+                head.insert(0, [tabulate.SEPARATING_LINE])
+                head.insert(0, col_types)
+                dt_with_space = head + [tabulate.SEPARATING_LINE] + tail
+                str_dataset = f"{tabulate.tabulate(dt_with_space, tablefmt='simple', headers=column_names, missingval='None')}\n\n[{rows} rows x {cols} columns]"
+                return str_dataset
             else:
-                column_names = self.columns
-                col_types = list(head.describe()["column_type"])
-                head_list = head.__rel.execute().fetch_all()
-                tail_list = tail.__rel.execute().fetch_all()
-
-            # Add separation between head and tail elements and column types
-            head_list.insert(0, [tabulate.SEPARATING_LINE])
-            head_list.insert(0, col_types)
-            dt_with_space = head_list + [tabulate.SEPARATING_LINE] + tail_list
-
-            str_dataset = f"{tabulate.tabulate(dt_with_space, tablefmt='simple', headers=column_names, missingval='None')}\n\n[{rows} rows x {cols} columns]"
-            return str_dataset
+                self._add_reduced_col(data)
+                data.insert(0, [tabulate.SEPARATING_LINE])
+                data.insert(0, col_types)
+                str_dataset = f"{tabulate.tabulate(data, headers=column_names, tablefmt='simple', missingval='None')}\n\n[{rows} rows x {cols} columns]"
+                return str_dataset
         else:
-            if cols > 10:
-                # Reduce amount of columns showed
-                column_names = self.select_columns(
-                    [0, 1, 2, 3, 4, cols - 5, cols - 4, cols - 3, cols - 2, cols - 1]).columns
-                col_types = list(self.select_columns(column_names).describe()["column_type"])
-                selected_cols = self.select_columns(column_names).__rel.execute().fetch_all()
-                column_names.insert(5, "...")
-                col_types.insert(5, "...")
-                self._add_reduced_col(selected_cols)
-
+            data = self.__rel.execute().fetch_all()
+            column_names = self.columns
+            col_types = [self.schema[x][1] for x in column_names]
+            rows = len(data)
+            if rows > 10:
+                head = data[:5]
+                tail = data[-5:]
+                head.insert(0, [tabulate.SEPARATING_LINE])
+                head.insert(0, col_types)
+                dt_with_space = head + [tabulate.SEPARATING_LINE] + tail
+                str_dataset = f"{tabulate.tabulate(dt_with_space, tablefmt='simple', headers=column_names, missingval='None')}\n\n[{rows} rows x {cols} columns]"
+                return str_dataset
             else:
-                # If less than 10 rows and 10 cols, print all Dataset
-                column_names = self.columns
-                col_types = list(self.describe()["column_type"])
-                selected_cols = self.__rel.execute().fetch_all()
-            # Add separation between head and tail elements and column types
-            selected_cols.insert(0, [tabulate.SEPARATING_LINE])
-            selected_cols.insert(0, col_types)
-            str_dataset = f"{tabulate.tabulate(selected_cols, headers=column_names, tablefmt='simple', missingval='None')}\n\n[{rows} rows x {cols} columns]"
-            return str_dataset
+                data.insert(0, [tabulate.SEPARATING_LINE])
+                data.insert(0, col_types)
+                str_dataset = f"{tabulate.tabulate(data, headers=column_names, tablefmt='simple', missingval='None')}\n\n[{rows} rows x {cols} columns]"
+                return str_dataset
 
     def _repr_pretty_(self, p, cycle) -> None:
         p.text(self.__tab("plain"))
 
     def _repr_html_(self) -> str:
         return self.__tab("html")
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/_uom.py` & `shapelets-platform-2.0.85/src/shapelets/_uom.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/data_app.py` & `shapelets-platform-2.0.85/src/shapelets/apps/data_app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 import datetime
 import json
-import numpy as np
+# import numpy as np
 import pandas as pd
 import subprocess
 import sys
 import time
 
 from enum import Enum
 from json import JSONEncoder
 from matplotlib.figure import Figure
 from pathlib import Path
-from typing import List, Literal, Optional, Union, NamedTuple
+from typing import List, Optional, Union, NamedTuple
 from typing_extensions import Literal
 
 from .widgets.charts.altair_chart import AltairChartWidget
 from .widgets.charts.folium_chart import FoliumChartWidget
 from .widgets.charts.line_chart import LineChartWidget, LineChartValueType
 # from .widgets.charts.plotly_chart import PlotlyChartWidget
 from .widgets.contexts.filtering_context import FilteringContext
 from .widgets.contexts.metadata_field import MetadataField
 from .widgets.contexts.temporal_context import TemporalContext
 from .widgets.controllers.button import Button
 from .widgets.controllers.checkbox import CheckboxWidget
 from .widgets.controllers.datetime_range_selector import DatetimeRangeSelectorWidget
 from .widgets.controllers.datetime_selector import DateSelectorWidget
+from .widgets.controllers import GaugeWidget, MetricWidget, RingWidget
 from .widgets.controllers.image import ImageWidget
-from .widgets.controllers.list import ListWidget
+# from .widgets.controllers.list import ListWidget
 from .widgets.controllers.number_input import NumberInputWidget
 from .widgets.controllers.progress import ProgressWidget
 from .widgets.controllers.radio_group import RadioGroupWidget
 from .widgets.controllers.selector import SelectorWidget
 from .widgets.controllers.slider import SliderWidget
-from .widgets.controllers.table import TableWidget
+from .widgets.controllers.table import Condition, TableWidget
 from .widgets.controllers.text import TextWidget
 from .widgets.controllers.text_input import TextInputWidget
 from .widgets.controllers.timer import TimerWidget
 from .widgets.layouts.horizontal_layout import HorizontalLayoutWidget
 from .widgets.layouts.panel import PanelWidget
 from .widgets.layouts.tabs_layout import TabsLayoutWidget
 from .widgets.layouts.vertical_layout import VerticalLayoutWidget
@@ -95,22 +96,31 @@
         self.version = version
         self.tags = tags
         self.main_panel = main_panel if main_panel else VerticalLayoutWidget(panel_id=name)
         self.title = name
         self.temporal_contexts = []
         self.filtering_contexts = []
         self.functions = {}
+        self.groups = None
+        self._data = []
 
-    def register(self):
+    def register(self, groups: Optional[Union[List[str], str]] = None):
         """
         Registers the DataApp.
 
+        Parameters
+        ----------
+        groups : List[str], str, optional
+            Group/s where the dataApp will be registered.
+
         It checks DataApp's code to avoid possible errors during Runtime (using mypy library).
         If some error is found, it will print a message to the user but the DataApp will be registered anyway
         """
+        if groups is not None:
+            self.groups = groups
         dataApp_svc = get_service(IDataAppsService)
         response = dataApp_svc.create(self)
 
         try:
             self._check_dataApp()
 
         except FileNotFoundError as exc:
@@ -734,22 +744,22 @@
         -------
         Button
 
         Examples
         --------
         >>> button = app.button("Press me") 
 
-
         You can bind this widget with this:
 
         .. hlist::
             :columns: 1
 
             * :func:`~shapelets.apps.DataApp.button`
 
+        Note: bind function will change button text.
 
         """
         return Button(text, parent_data_app=self, **additional)
 
     def timer(self,
               title: str = None,
               every: Union[int, float] = None,
@@ -945,15 +955,16 @@
         You can bind this widget as: 
 
         .. hlist::
             :columns: 1
 
             * :func:`~shapelets.apps.DataApp.vertical_layout`         
         """
-        return VerticalLayoutWidget(panel_title=title, panel_id=panel_id, vertical_align=vertical_align, span=span, offset=offset,
+        return VerticalLayoutWidget(panel_title=title, panel_id=panel_id, vertical_align=vertical_align, span=span,
+                                    offset=offset,
                                     parent_data_app=self, **additional)
 
     def horizontal_layout(self,
                           title: str = None,
                           panel_id: str = None,
                           horizontal_align: Optional[Literal["start", "center", "end"]] = "start",
                           vertical_align: Optional[Literal["start", "center", "end"]] = "start",
@@ -1687,14 +1698,15 @@
                               stroke_color=stroke_color, stroke_width=stroke_width, show_info=show_info,
                               parent_data_app=self, **additional)
 
     def table(self,
               data: Union[pd.DataFrame, DataSet] = None,
               rows_per_page: Optional[int] = None,
               tools_visible: Optional[bool] = None,
+              conditional_formats: Optional[List[Union[Condition, dict]]] = None,
               **additional):
         """
         Displays rows of data.
 
         Parameters
         ----------
         data : Dataset or pd.Dataframe, optional
@@ -1702,14 +1714,39 @@
 
         rows_per_page : int, optional
             number of rows per page to show
 
         tools_visible : int, optional
             show/hide header, header bold and rowcolumn controls
 
+        conditional_formats: List[Dict, Conditional], optional
+            Add format to a value applying any condition. There are two types of conditional format:
+                * Range: Allow to modify the color and background color of a numeric value
+                * Case: Allow to modify the color and brackgorund color of a string value
+            For example:
+            {
+              "column": "T1",
+              "type": "range",
+              "conditions": [
+                { "min": 0, "max": 20, "backcolor": "#ff0000", "color": "#ffffff" },
+                { "min": 20,"max": 40, "backcolor": "#ff860a" },
+                { "min": 40,"max": 42, "color": "#ff860a" },
+                { "min": 44,"max": 100, "backcolor": "#00aa00" }
+              ]
+            },
+            {
+              "column": "Estado",
+              "type": "case",
+              "conditions": [
+                { "value": "Peligro", "backcolor": "#ff0000", "color": "#ffffff" },
+                { "value": "Precaución", "backcolor": "#000077", "color": "#ffffff" },
+                { "value": "OK", "backcolor": "#00aa00", "color": "#ffffff" }
+              ]
+            }
+
 
         Returns
         -------
         Table
 
         Examples
         --------
@@ -1738,16 +1775,184 @@
             * Shapelets Dataset
             * Pandas DataFrame
             * list
             * :func:`~shapelets.apps.DataApp.table`
 
         """
         return TableWidget(data=data, rows_per_page=rows_per_page, tools_visible=tools_visible,
+                           conditional_formats=conditional_formats, parent_data_app=self, **additional)
+
+    def gauge(self,
+              title: Optional[str] = None,
+              value: Optional[Union[int, float]] = None,
+              **additional) -> GaugeWidget:
+        """
+        Creates a Gauge.
+
+        Parameters
+        ----------
+        title : str, optional
+            Text associated to the Gauge.
+
+        value : int, float, optional
+            Param to indicate the value of the widget
+
+        Returns
+        -------
+        Gauge.
+
+        Examples
+        --------
+        >>> gauge = app.gauge(title='Title', value=25)
+
+        .. rubric:: Bind compatibility
+
+        You can bind this widget with this:
+
+        .. hlist::
+            :columns: 1
+
+            * int
+            * float
+            * :func:`~shapelets.apps.DataApp.gauge`
+
+        .. rubric:: Bindable as
+
+        You can bind this widget as:
+
+        .. hlist::
+            :columns: 1
+
+            * int
+            * float
+            * string
+            * :func:`~shapelets.apps.DataApp.gauge`
+
+        """
+        return GaugeWidget(title=title, value=value,
                            parent_data_app=self, **additional)
 
+    def metric(self,
+               title: Optional[str] = None,
+               value: Optional[str] = None,
+               unit: Optional[str] = None,
+               delta: Optional[str] = None,
+               align: Optional[Literal["right", "left"]] = None,
+               **additional) -> MetricWidget:
+        """
+        Creates a Metric.
+
+        Parameters
+        ----------
+        title : str, optional
+            Text associated to the metric widget.
+
+        value : str, optional
+            Param to indicate the value of the widget
+
+        unit : str, optional
+            Unit of the widget
+
+        delta : str, optional
+            Delta of the metric
+
+        align : str, optional
+            Select how the metric is aligned vertically: right or left.
+
+        Returns
+        -------
+        Metric.
+
+        Examples
+        --------
+        >>> metric = app.metric(title='Title', value="2023,46", unit="$", delta="+20,25", align="right")
+
+        .. rubric:: Bind compatibility
+
+        You can bind this widget with this:
+
+        .. hlist::
+            :columns: 1
+
+            * str
+            * int
+            * float
+            * :func:`~shapelets.apps.DataApp.metric`
+
+        .. rubric:: Bindable as
+
+        You can bind this widget as:
+
+        .. hlist::
+            :columns: 1
+
+            * str
+            * int
+            * float
+            * :func:`~shapelets.apps.DataApp.metric`
+
+            """
+        return MetricWidget(title=title, value=value, unit=unit, delta=delta, align=align,
+                            parent_data_app=self, **additional)
+
+    def ring(self,
+             title: Optional[str] = None,
+             value: Optional[Union[int, float]] = None,
+             color: Optional[str] = None,
+             **additional) -> RingWidget:
+        """
+        Creates a Ring.
+
+        Parameters
+        ----------
+        title : str, optional
+            Text associated to the Ring.
+
+        value : int, float, optional
+            Param to indicate the value of the widget as a percentage
+
+        color : str, optional
+            Color to display the widget
+
+        Returns
+        -------
+        Ring.
+
+        Examples
+        --------
+        >>> ring = app.ring(title='Title', value=25, color="Red")
+
+        .. rubric:: Bind compatibility
+
+        You can bind this widget with this:
+
+        .. hlist::
+            :columns: 1
+
+            * int
+            * float
+            * :func:`~shapelets.apps.DataApp.ring`
+
+        .. rubric:: Bindable as
+
+        You can bind this widget as:
+
+        .. hlist::
+            :columns: 1
+
+            * int
+            * float
+            * string
+            * :func:`~shapelets.apps.DataApp.ring`
+
+            """
+
+        return RingWidget(title=title, value=value, color=color,
+                          parent_data_app=self, **additional)
+
     def place(self, widget: Widget, *args, **kwargs):
         """
         Places a widget into the dataApp.
 
         Parameters
         ----------
         widget : Widget
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/data_app_utils.py` & `shapelets-platform-2.0.85/src/shapelets/apps/data_app_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,28 @@
-
 from .charts import *
 from . import charts
 
 from .contexts import *
 from . import contexts
 
 from .controllers import *
 from . import controllers
 
 from .layouts import *
 from . import layouts
 
 from .attribute_names import AttributeNames
 from .datetime_utils import _transform_date_time_value, _date_to_string
-from .util import unique_id_str, unique_id_int, _to_utf64_arrow_buffer
+from .util import _read_from_arrow_file, _to_utf64_arrow_buffer, _write_arrow_table_file
 from .widget import Widget, StateControl
 
 __all__ = [
     'Widget', 'StateControl',
     'AttributeNames', '_date_to_string',
-    'unique_id_str', 'unique_id_int', '_to_utf64_arrow_buffer', '_transform_date_time_value'
+    '_read_from_arrow_file', '_to_utf64_arrow_buffer',
+    '_transform_date_time_value', '_write_arrow_table_file'
 ]
 
 __all__ += charts.__all__
 __all__ += contexts.__all__
 __all__ += controllers.__all__
 __all__ += layouts.__all__
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/attribute_names.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/attribute_names.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 from enum import Enum
 
 
 class AttributeNames(Enum):
+    ALIGN = "align"
     ALIGN_ITEMS = "alignItems"
     ALLOW_MULTI_SELECTION = "allowMultiSelection"
     ARROW_DATA = "arrowData"
     BEGIN = "begin"
     BIND = "bind"
     BINS = "bins"
     CAPTION = "caption"
     CATEGORIES = "categories"
     CHECKED = "checked"
     COLLECTION_ID = "collectionId"
     COLLECTION_LABEL = "collectionLabel"
+    COLUMN = "column"
     COLS = "cols"
     COL_OFFSET = "colOffset"
     COL_SPAN = "colSpan"
     COLOR = "color"
+    CONDITION = "condition"
+    CONDITIONAL_FORMATS = "conditionalFormats"
     CUMULATIVE = "cumulative"
     DATA = "data"
     DATE = "date"
     DATE_TIME = "date_time"
     DEFAULT = "default"
+    DELTA = "delta"
     DISABLED = "disabled"
     DRAGGABLE = "draggable"
     END = "end"
     END_DATE = "endDate"
     EVENTS = "events"
     EVERY = "every"
     GROUPS = "groups"
     FORMAT = "format"
     HEADER_SHOW = "header_show"
     HEADER_BOLD = "header_bold"
     HIDDEN = "hidden"
-    HORIZONTAL_ALIGN ="horizontalAlign"
+    HORIZONTAL_ALIGN = "horizontalAlign"
     ID = "id"
     INDEX_BY = "indexBy"
     INPUT_FILTERS = "inputFilters"
     IN_RANGE = "inRange"
     LABEL = "label"
     LABEL_BY = "labelBy"
     LANE_INDEX = "laneIndex"
@@ -67,19 +72,21 @@
     POSITION = "position"
     PROPERTIES = "properties"
     RANGE = "range"
     REF = "$ref"
     RESIZABLE = "resizable"
     ROW = "row"
     ROW_NUMBER_SHOW = "row_number_show"
-    ROWS_PER_PAGE = "rows_per_page"
+    ROWS_PER_PAGE = "rowsPerPage"
     ROW_SPAN = "rowSpan"
     TIME_FORMAT = "timeFormat"
     TOGGLE = "toggle"
     TOOLBAR = "toolbar"
+    TOTAL_PAGES = "totalPages"
+    TOTAL_ROWS = "totalRows"
     SEQUENCE = "sequence"
     SEQUENCE_ID = "sequenceId"
     SEQUENCE_LABEL = "sequenceLabel"
     SIZE = "size"
     SHOW_INFO = "showInfo"
     START = "start"
     START_DELAY = "startDelay"
@@ -90,18 +97,19 @@
     STROKE_COLOR = "strokeColor"
     STROKE_WIDTH = "strokeWidth"
     TABS = "tabs"
     TEXT = "text"
     TEXT_STYLE = "textStyle"
     TIMES = "times"
     TITLE = "title"
-    TOOLS_VISIBLE = "tools_visible"
+    TOOLS_VISIBLE = "toolsVisible"
     TREND_LINE = "trendLine"
     TYPE = "type"
     TYPE_NOT_SUPPORTED = "only supports int/float types"
+    UNIT = "unit"
     UNITS = "units"
     VALUE = "value"
     VALUE_BY = "valueBy"
     VALUES = "values"
     VERTICAL_ALIGN = "verticalAlign"
     VIEWS = "views"
     WIDGET = "widget"
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/altair_chart.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/altair_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/bar_chart.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/bar_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/folium_chart.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/folium_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/heatmap.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/heatmap.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/histogram.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/histogram.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/line_chart.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/line_chart.py`

 * *Files 1% similar despite different names*

```diff
@@ -148,14 +148,16 @@
     filtering_context: Optional[FilteringContext] = None
     multi_line_chart: Optional[bool] = True
     multi_lane: Optional[bool] = True
     _plots: List = field(default_factory=lambda: [])
     _is_type = None
 
     def __post_init__(self):
+        if not hasattr(self, "widget_id"):
+            self.widget_id = str(uuid.uuid1())
         # A subtype to differentiate between sequences or y_axis/x_axis. Requested by UI.
         self.linechart_sub_type = None
         self.sequence = None
         self.y_axis = None
         self.x_axis = None
         if isinstance(self.data, Sequence):
             self.linechart_sub_type = f"{AttributeNames.SEQUENCE.value.capitalize()}"
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/pie_chart.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/pie_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/plotly_chart.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/plotly_chart.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/polar_area.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/polar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/radar_area.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/radar_area.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/charts/scatter_plot.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/charts/scatter_plot.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/filtering_context.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/filtering_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_field.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_field.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/metadata_filter.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/metadata_filter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/contexts/temporal_context.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/contexts/temporal_context.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 from .button import Button
 # from .collection_selector import CollectionSelector
 from .datetime_selector import DateSelector, DateSelectorWidget
 from .datetime_range_selector import DateRangeSelector, DatetimeRangeSelectorWidget
 from .image import Image, ImageWidget
 from .list import ListControl, ListWidget
 from .checkbox import Checkbox, CheckboxWidget
+from .gauge import Gauge, GaugeWidget
 # from .multi_sequence_selector import MultiSequenceSelector
+from .metric import Metric, MetricWidget
 from .number_input import NumberInput, NumberInputWidget
 from .progress import Progress, ProgressWidget
 from .radio_group import RadioGroup, RadioGroupWidget
+from .ring import Ring, RingWidget
 from .selector import Selector, SelectorWidget
 # from .sequence_list import SequenceList
 # from .sequence_selector import SequenceSelector
 from .slider import Slider, SliderWidget
-from .table import Table, TableWidget
+from .table import Condition, Table, TableWidget
 from .text import Text, TextWidget
 from .text_input import TextInput, TextInputWidget
 from .timer import Timer, TimerWidget
 
-
 __all__ = [
     'Button',
     'Checkbox',
+    'Condition',
     'DateSelector',
     'DateRangeSelector',
+    'Gauge',
     'Image',
     'ListControl',
+    'Metric',
     'NumberInput',
     'Progress',
     'RadioGroup',
+    'Ring',
     'Selector',
     'Slider',
     'Table',
     'Text',
     'TextInput',
     'Timer'
 ]
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/button.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/grid_layout.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,53 +1,50 @@
-from ..widget import AttributeNames, Widget
+# Copyright (c) 2021 Grumpy Cat Software S.L.
+#
+# This Source Code is licensed under the MIT 2.0 license.
+# the terms can be found in LICENSE.md at the root of
+# this project, or at http://mozilla.org/MPL/2.0/.
+from ...widgets import Widget, AttributeNames
+from .panel import Panel
 
-
-class Button(Widget):
+class GridPanel(Panel):
     """
-    Creates a button.
-
-    Parameters
-    ----------
-    text : str, optional
-        String placed inside the button.
-
-    Returns
-    -------
-    Button
-
-    Examples
-    --------
-    >>> button = app.button("Press me") 
-
-
+    TO BE FILLED
     """
 
     def __init__(self,
-                 text_button: str = None,
-                 **additional):
-        Widget.__init__(self, self.__class__.__name__,
-                        compatibility=tuple([Button.__name__,]),
-                        **additional)
-        self.text = text_button
-
-    def to_dict_widget(self):
-        button_dict = super().to_dict_widget()
-        _widget_providers = []
-        if self.text is not None:
-            if isinstance(self.text, str):
-                button_dict[AttributeNames.PROPERTIES.value].update({
-                    AttributeNames.TEXT.value: self.text,
-                })
-            elif isinstance(self.text, Widget):
-                target = {"id": self.text.widget_id, "target": AttributeNames.TEXT.value}
-                _widget_providers.append(target)
-            else:
-                raise ValueError(f"Error Widget {self.widget_type}: Text value should be a string or another widget")
-
-        if _widget_providers:
-            self.add_widget_providers(button_dict, _widget_providers)
-
-        return button_dict
+                 num_rows: int,
+                 num_cols: int,
+                 panel_title: str = None,
+                 panel_id: str = None,
+                 **additional
+                 ):
+        super().__init__(panel_title=panel_title, panel_id=panel_id, **additional)
+        self.num_rows = num_rows
+        self.num_cols = num_cols
+        self.placements = dict()
+
+    def place(self, widget: Widget, row: int, col: int, row_span: int = 1, col_span: int = 1):
+        GridPanel.__check_bounds("row", row + row_span - 1, self.num_rows)
+        GridPanel.__check_bounds("col", col + col_span - 1, self.num_cols)
+        super()._place(widget)
+        self.placements[widget.widget_id] = (row, col, row_span, col_span)
 
     @staticmethod
-    def bind():
-        raise AttributeError("Button widget does not allow bind")
+    def __check_bounds(name, index, max_index):
+        if not (0 <= index < max_index):
+            raise IndexError(f"{name} index out of bounds {index} not in [0, {max_index})")
+
+    def to_dict_widget(self):
+        panel_dict = super().to_dict_widget()
+        panel_dict[AttributeNames.PROPERTIES.value].update({
+            AttributeNames.NUM_ROWS.value: self.num_rows,
+            AttributeNames.NUM_COLS.value: self.num_cols,
+            AttributeNames.PLACEMENTS.value: [{
+                AttributeNames.WIDGET_REF.value: key,
+                AttributeNames.ROW.value: row,
+                AttributeNames.COL.value: col,
+                AttributeNames.ROW_SPAN.value: row_span,
+                AttributeNames.COL_SPAN.value: col_span
+            } for key, (row, col, row_span, col_span) in self.placements.items()]
+        })
+        return panel_dict
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/checkbox.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/checkbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -119,14 +119,17 @@
             if isinstance(self.toggle, bool):
                 checkbox_dict[AttributeNames.PROPERTIES.value].update({
                     AttributeNames.TOGGLE.value: self.toggle
                 })
             else:
                 raise ValueError(f"Unexpected type {type(self.toggle)} in toggle")
 
+        if _widget_providers:
+            self.add_widget_providers(checkbox_dict, _widget_providers)
+
         return checkbox_dict
 
 
 class CheckboxWidget(Widget, Checkbox):
 
     def __init__(self,
                  title: Optional[str] = None,
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/collection_selector.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/collection_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_range_selector.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_range_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/datetime_selector.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/datetime_selector.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
                 target = {"id": self.title.widget_id, "target": AttributeNames.TITLE.value}
                 _widget_providers.append(target)
             else:
                 raise ValueError(f"Unexpected type {type(self.title)} in title")
 
         if self.date_time is not None:
             date_dict[AttributeNames.PROPERTIES.value].update({
-                AttributeNames.DATE.value: self._date_time_str,
+                AttributeNames.VALUE.value: self._date_time_str,
             })
 
             if self._format is not None:
                 date_dict[AttributeNames.PROPERTIES.value].update({
                     AttributeNames.FORMAT.value: self._format
                 })
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/image.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/list.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/multi_sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/number_input.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/number_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/progress.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/progress.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import uuid
 
 from dataclasses import dataclass
-from typing import List, Literal, Optional, Union
+from typing import List, Optional, Union
+from typing_extensions import Literal
 
 from ..widget import AttributeNames, Widget, StateControl
 
 
 @dataclass
 class Progress(StateControl):
     value: Optional[Union[str, int, float]] = None
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/radio_group.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/radio_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import uuid
 
 from dataclasses import dataclass
-from typing import List, Literal, Optional, Union
+from typing import List, Optional, Union
+from typing_extensions import Literal
 
 from ..widget import AttributeNames, StateControl, Widget
 
 
 @dataclass
 class RadioGroup(StateControl):
     """
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/resources/placeholder.jpg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/selector.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_list.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_list.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/sequence_selector.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/sequence_selector.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/slider.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/slider.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/text_input.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/text_input.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/controllers/timer.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/controllers/timer.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/datetime_utils.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/grid_layout.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/panel.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,42 @@
-# Copyright (c) 2021 Grumpy Cat Software S.L.
-#
-# This Source Code is licensed under the MIT 2.0 license.
-# the terms can be found in LICENSE.md at the root of
-# this project, or at http://mozilla.org/MPL/2.0/.
-from ...widgets import Widget, AttributeNames
-from .panel import Panel
+from dataclasses import dataclass, field
+from typing import List, Optional, Tuple
 
-class GridPanel(Panel):
+from ..widget import Widget, AttributeNames, StateControl
+
+
+@dataclass
+class Panel(StateControl):
+    panel_title: Optional[str] = None
+    panel_id: Optional[str] = None
+    widgets: Optional[List[Widget]] = field(default_factory=lambda: [])
+
+
+class PanelWidget(Widget, Panel):
     """
-    TO BE FILLED
+    Container + Layout: a Panel is a plain layout where widgets can be placed.
     """
 
     def __init__(self,
-                 num_rows: int,
-                 num_cols: int,
-                 panel_title: str = None,
-                 panel_id: str = None,
+                 panel_title: Optional[str] = None,
+                 panel_id: Optional[str] = None,
+                 compatibility: tuple = None,
                  **additional
                  ):
-        super().__init__(panel_title=panel_title, panel_id=panel_id, **additional)
-        self.num_rows = num_rows
-        self.num_cols = num_cols
-        self.placements = dict()
-
-    def place(self, widget: Widget, row: int, col: int, row_span: int = 1, col_span: int = 1):
-        GridPanel.__check_bounds("row", row + row_span - 1, self.num_rows)
-        GridPanel.__check_bounds("col", col + col_span - 1, self.num_cols)
-        super()._place(widget)
-        self.placements[widget.widget_id] = (row, col, row_span, col_span)
-
-    @staticmethod
-    def __check_bounds(name, index, max_index):
-        if not (0 <= index < max_index):
-            raise IndexError(f"{name} index out of bounds {index} not in [0, {max_index})")
+        Widget.__init__(self, widget_type=self._parent_class, widget_id=panel_id, compatibility=compatibility, **additional)
+        Panel.__init__(self, panel_title=panel_title)
+
+    def _place(self, *widget: Tuple[Widget, ...]):
+        self.widgets.extend(widget)
 
     def to_dict_widget(self):
         panel_dict = super().to_dict_widget()
-        panel_dict[AttributeNames.PROPERTIES.value].update({
-            AttributeNames.NUM_ROWS.value: self.num_rows,
-            AttributeNames.NUM_COLS.value: self.num_cols,
-            AttributeNames.PLACEMENTS.value: [{
-                AttributeNames.WIDGET_REF.value: key,
-                AttributeNames.ROW.value: row,
-                AttributeNames.COL.value: col,
-                AttributeNames.ROW_SPAN.value: row_span,
-                AttributeNames.COL_SPAN.value: col_span
-            } for key, (row, col, row_span, col_span) in self.placements.items()]
-        })
+        if self.widgets is not None:
+            widgets = [widget.to_dict_widget() for widget in self.widgets]
+            panel_dict[AttributeNames.PROPERTIES.value].update({
+                AttributeNames.WIDGETS.value: widgets
+            })
+        if self.panel_title:
+            panel_dict[AttributeNames.PROPERTIES.value].update({
+                AttributeNames.TITLE.value: self.panel_title
+            })
         return panel_dict
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/horizontal_layout.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/horizontal_layout.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 
 from dataclasses import dataclass, field
-from typing import Optional, Literal
+from typing import Optional
+from typing_extensions import Literal
 
 from ..widget import Widget, AttributeNames
 from .panel import PanelWidget, Panel
 
 
 @dataclass
 class HorizontalLayout(Panel):
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/tabs_layout.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/tabs_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 
 import uuid
 
 from dataclasses import dataclass, field
-from typing import Literal, Optional, Tuple, Union
+from typing import Optional, Tuple, Union
+from typing_extensions import Literal
 
 from ..widget import Widget, AttributeNames, StateControl
 from .panel import PanelWidget, Panel
 
 
 @dataclass
 class TabsLayout(Panel):
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/layouts/vertical_layout.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/layouts/vertical_layout.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import uuid
 
 from dataclasses import dataclass, field
-from typing import List, Literal, Optional
+from typing import List, Optional
+from typing_extensions import Literal
 
 from ..widget import Widget, AttributeNames
 from .panel import PanelWidget, Panel
 
 
 @dataclass
 class VerticalLayout(Panel):
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/util.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 import base64
 import numpy as np
 import pandas as pd
 import pyarrow as pa
-import uuid
+import os
 
 from typing import Union
 
 from ... import DataSet
 
-
-def unique_id_str() -> str:
-    return str(uuid.uuid1())
-
-
-def unique_id_int() -> int:
-    return uuid.uuid1().int
+SH_DIR = os.path.expanduser('~/.shapelets')
+DATA_DIR = os.path.join(SH_DIR, 'data')
 
 
 def _to_utf64_arrow_buffer(data: Union[pd.DataFrame, DataSet], preserve_index: bool = True) -> str:
     """
     Transform pandas dataframe or Shapelets dataset to an arrow buffer
     """
     if isinstance(data, pd.DataFrame):
@@ -48,7 +43,40 @@
     parray = pa.Array.from_pandas(series)
     batch = pa.record_batch([parray], names=["values"])
     sink = pa.BufferOutputStream()
     with pa.ipc.RecordBatchFileWriter(sink, batch.schema) as writer:
         writer.write(batch)
     buffer = sink.getvalue()
     return base64.b64encode(buffer).decode("utf-8")
+
+
+def _write_arrow_table_file(data: Union[pd.DataFrame, DataSet], table_id: str, preserve_index: bool = False):
+    if isinstance(data, pd.DataFrame):
+        table = pa.Table.from_pandas(data, preserve_index=preserve_index)
+    elif isinstance(data, DataSet):
+        table = data.to_arrow_table(1024)
+
+    os.makedirs(DATA_DIR, exist_ok=True)
+    path = os.path.join(DATA_DIR, table_id)
+
+    sink = pa.BufferOutputStream()
+    with pa.ipc.RecordBatchFileWriter(sink, table.schema) as writer:
+        writer.write(table)
+    buffer = sink.getvalue()
+    with open(path, 'wb') as sink:
+        sink.write(buffer)
+
+
+def _read_from_arrow_file(file_name: str, from_row: int = 0, n: int = 10) -> str:
+    path = os.path.join(DATA_DIR, file_name)
+    with open(path, "rb") as file:
+        reader = pa.ipc.open_file(file)
+        table = reader.read_all()
+    return _serialize_table(table.slice(from_row, n))
+
+
+def _serialize_table(table: pa.Table):
+    sink = pa.BufferOutputStream()
+    with pa.ipc.RecordBatchFileWriter(sink, table.schema) as writer:
+        writer.write(table)
+    buffer = sink.getvalue()
+    return base64.b64encode(buffer).decode("utf-8")
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/apps/widgets/widget.py` & `shapelets-platform-2.0.85/src/shapelets/apps/widgets/widget.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from __future__ import annotations
 
 import base64
 import dill
 import inspect
+import uuid
+import zlib
 
 from dataclasses import dataclass
 from typing import Callable, overload, Union, List, Dict, Tuple
 from typing_extensions import get_args
 
-from .util import unique_id_str
 from .attribute_names import AttributeNames
 
 import __main__
 import sys
 
 
 class Widget:
@@ -29,15 +30,15 @@
                  placeholder: str = None,
                  disabled: bool = None,
                  compatibility: tuple = None,
                  parent_data_app: object = None) -> object:
         # parent_data_app is a reference to the DataApp used as a factory
         # for this widget
         self.parent_data_app = parent_data_app
-        self.widget_id = widget_id if widget_id else unique_id_str()
+        self.widget_id = widget_id if widget_id else str(uuid.uuid1())
         self.widget_type = widget_type
         self.placeholder = placeholder
         self.disabled = disabled
         self.draggable = draggable
         self.resizable = resizable
         self._bind = []
         self._mainlist = []
@@ -263,15 +264,15 @@
             # Adjust entry arguments
             fn = self._adjust_arguments(fn, entry_arguments)
 
             body = fn
             if return_type != self._parent_class:
                 body = self._adjust_return(fn, return_type)
             result = {
-                "body": str(base64.b64encode(dill.dumps(body, recurse=True)), encoding='utf-8'),
+                "body": base64.b64encode(zlib.compress(dill.dumps(body, recurse=True))).decode('utf-8'),
                 "parameters": entry_arguments,
                 "result": self._parent_class
             }
 
             # Add to DataApp Structure
             self.parent_data_app.functions[fn_original_name] = result
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/functions.py` & `shapelets-platform-2.0.85/src/shapelets/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/iris.csv` & `shapelets-platform-2.0.85/src/shapelets/iris.csv`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/model/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/altair.py` & `shapelets-platform-2.0.85/src/shapelets/model/altair.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/capsule.py` & `shapelets-platform-2.0.85/src/shapelets/model/capsule.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/collection.py` & `shapelets-platform-2.0.85/src/shapelets/model/collection.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/dataframe.py` & `shapelets-platform-2.0.85/src/shapelets/model/dataframe.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/function_description.py` & `shapelets-platform-2.0.85/src/shapelets/model/function_description.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/function_parameter.py` & `shapelets-platform-2.0.85/src/shapelets/model/function_parameter.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/group.py` & `shapelets-platform-2.0.85/src/shapelets/model/group.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/image.py` & `shapelets-platform-2.0.85/src/shapelets/model/image.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/metadata_item.py` & `shapelets-platform-2.0.85/src/shapelets/model/metadata_item.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/model.py` & `shapelets-platform-2.0.85/src/shapelets/model/model.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/ndarray.py` & `shapelets-platform-2.0.85/src/shapelets/model/ndarray.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/permissions.py` & `shapelets-platform-2.0.85/src/shapelets/model/permissions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/replicated_param.py` & `shapelets-platform-2.0.85/src/shapelets/model/replicated_param.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/sequence.py` & `shapelets-platform-2.0.85/src/shapelets/model/sequence.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/sequence_axis.py` & `shapelets-platform-2.0.85/src/shapelets/model/sequence_axis.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/user.py` & `shapelets-platform-2.0.85/src/shapelets/model/user.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/model/view_match.py` & `shapelets-platform-2.0.85/src/shapelets/model/view_match.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
 # Public APIs
 from .authn import (
     IAuthService, UserAlreadyExists, InvalidLength,
     VerificationError, UnknownUser, InvalidUserName,
     Challenge, Addresses, gc_flow)
 from .model import (
-    DataAppProfile, FunctionProfile, GCPrincipalId,
+    DataAppAttributes, FunctionProfile, GCPrincipalId,
     GroupAttributes, GroupField, GroupProfile,
     PrincipalId, ResolvedPrincipalId, SignedPrincipalId,
     UserAllFields, UserAttributes, UserField,
     UserId, UserProfile)
 
 from .dataapps import IDataAppsService
 from .execution import IExecutionService
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/app.py` & `shapelets-platform-2.0.85/src/shapelets/svr/app.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/authhttp.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/authhttp.py`

 * *Files 3% similar despite different names*

```diff
@@ -73,17 +73,18 @@
             return self.json(self._svr.user_name_exists(username))
         except InvalidUserName as e:
             return self.bad_request(str(e))
         except Exception as e:
             return self.status_code(500, str(e))
 
     @get('/unp/remove')
-    async def remove_user(self, userName: str) -> bool:
+    async def remove_user(self, userName: str, transfer: str = None) -> bool:
         try:
-            return self.json(self._svr.remove_user(userName))
+            resutl = self.json(self._svr.remove_user(userName, transfer))
+            return resutl
         except InvalidUserName as e:
             return self.bad_request(str(e))
         except Exception as e:
             return self.status_code(500, str(e))
 
     @get('/unp/challenge')
     async def generate_challenge(self, userName: str) -> Challenge:
@@ -145,19 +146,18 @@
         response = self.session.get('/api/login/unp/check', params=[("username", userName)])
 
         if response.status_code == 400:
             raise InvalidUserName(userName)
 
         return response.ok and bool(response.json() == True)
 
-    def remove_user(self, userName: str) -> bool:
-        response = self.session.get('/api/login/unp/remove', params=[("userName", userName)])
-
-        if response.status_code == 400:
-            raise InvalidUserName(userName)
+    def remove_user(self, userName: str, transfer: str = None) -> bool:
+        response = self.session.get('/api/login/unp/remove', params=[("userName", userName), ("transfer", transfer)])
+        if response.status_code != 200:
+            raise Exception(response.content)
 
         return response.ok and bool(response.json() == True)
 
     def generate_challenge(self, userName: str) -> Challenge:
         response = self.session.get('/api/login/unp/challenge', params=[("userName", userName)])
         if response.status_code == 400:
             raise InvalidUserName(userName)
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/authrepo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/authrepo.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,13 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from typing import Optional, Tuple
 
 from .iauthrepo import IAuthRepo
+from ..dataapps.dataappsrepo import _user_group_dataapp_list, _user_local_dataapp_list, _delete_dataapp
 from ..db import Connection, connect, transaction
-from ..model import UserAttributes
+from ..model import UserAttributes, DataAppAllFields
 
 
 def _nextId(conn: Connection) -> int:
     conn.execute("SELECT nextval('shapelets.id_gen')")
     return int(conn.fetch_one()[0])
 
 
@@ -112,14 +108,43 @@
 
 def _principals_find_userName(uid: int, conn: Connection) -> Optional[str]:
     conn.execute("SELECT id FROM principals where uid = ? and scope = ?", [uid, 'unp'])
     record = conn.fetch_one()
     return None if record is None else str(record[0])
 
 
+def _transfer_data_apps(old_user_id: int, new_user_id: int, conn: Connection):
+    conn.execute("""
+    SELECT name 
+    FROM groups 
+    LEFT JOIN users_groups on users_groups.groupId = groups.uid where users_groups.userId = ?
+    """, [new_user_id])
+    new_user_groups = conn.fetch_all()
+    if new_user_groups:
+        group_names = [group[0] for group in new_user_groups]
+    else:
+        raise ValueError("Transfer user does not belong to any group")
+    # Try transferring dataApps with group
+    dataapp_with_group = _user_group_dataapp_list(old_user_id, conn)
+    for app in dataapp_with_group:
+        if any(x in app.groups for x in group_names):
+            conn.execute(""" 
+                UPDATE dataapps 
+                SET userId = ?
+                WHERE uid = ?;
+            """, [new_user_id, app.uid])
+        else:
+            raise Exception("Transfer user does not have access to the group where this dataApp belong")
+    # delete old user private dataApps
+    private_apps = _user_local_dataapp_list(old_user_id, conn)
+    if private_apps:
+        for app in private_apps:
+            _delete_dataapp(app.uid, old_user_id, conn)
+
+
 class AuthRepo(IAuthRepo):
 
     def find_userId(self, scope: str, id: str) -> Optional[int]:
         with connect() as conn:
             return _principals_find_userId(scope, id, conn)
 
     def create_new_user_unp(self, userName: str, salt: bytes, verify_key: bytes, user_details: UserAttributes) -> int:
@@ -141,21 +166,27 @@
         with connect() as conn:
             return _unp_challenges_last_nonce(userName, conn)
 
     def user_name_exists(self, userName: str) -> bool:
         with connect() as conn:
             return _unp_users_has_userName(userName, conn)
 
-    def remove_user(self, userName: str) -> bool:
+    def remove_user(self, userName: str, transfer: str) -> bool:
         with transaction() as conn:
             scope = 'unp'
             uid = _principals_find_userId(scope, userName, conn)
             if uid is None:
                 return False
 
+            if transfer is not None:
+                transfer_user_id = _principals_find_userId(scope, transfer, conn)
+                if transfer_user_id is None:
+                    return False
+                _transfer_data_apps(uid, transfer_user_id, conn)
+
             _principals_delete_by_userId(uid, scope, conn)
             _unp_users_delete(userName, conn)
             _users_delete(uid, conn)
             return True
 
     def get_salt(self, userName: str) -> Optional[bytes]:
         with connect() as conn:
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/authservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/authservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,16 +131,16 @@
     ##########################
     # User Name and Password #
     ##########################
 
     def user_name_exists(self, userName: str) -> bool:
         return self._auth_repo.user_name_exists(userName)
 
-    def remove_user(self, userName: str) -> bool:
-        return self._auth_repo.remove_user(userName)
+    def remove_user(self, userName: str, transfer: str) -> bool:
+        return self._auth_repo.remove_user(userName, transfer)
 
     def register(self, userName: str, salt: bytes, verify_key: bytes, user_details: UserAttributes) -> bool:
 
         if userName is None or len(userName) == 0:
             raise InvalidUserName(userName)
 
         if len(salt) != crypto.salt_bytes():
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/gc_client.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/gc_client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthrepo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthrepo.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         pass
 
     @abstractmethod
     def user_name_exists(self, userName: str) -> bool:
         pass
 
     @abstractmethod
-    def remove_user(self, userName: str) -> bool:
+    def remove_user(self, userName: str, transfer: str) -> bool:
         pass
 
     @abstractmethod
     def get_salt(self, userName: str) -> Optional[bytes]:
         pass
 
     @abstractmethod
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/authn/iauthservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/authn/iauthservice.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
     def user_name_exists(self, userName: str) -> bool:
         """
         Checks for the uniqueness of a user name (for username and password)
         """
         pass
 
     @abstractmethod
-    def remove_user(self, userName: str) -> bool:
+    def remove_user(self, userName: str, transfer: str) -> bool:
         """
         Remove the user indicated by user name
         """
         pass
 
     @abstractmethod
     def register(self, userName: str, salt: bytes, verify_key: bytes, user_details: UserAttributes) -> bool:
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/access_token_credentials.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/access_token_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen1.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen1.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/azure_gen2.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/azure_gen2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/driver.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/driver.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/dynamic_credentials.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/dynamic_credentials.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_config.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_config.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_factory.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/fsspec_vfs_file.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/fsspec_vfs_file.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/ftp.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/ftp.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/local.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/local.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/protocols.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/protocols.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/smb.py` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/smb.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/data/vfs/vfs_sample_config.toml` & `shapelets-platform-2.0.85/src/shapelets/svr/data/vfs/vfs_sample_config.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataapps_ws.py` & `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataapps_ws.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/dataappsservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/dataappsservice.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,63 @@
-# Copyright (c) 2022 Shapelets.io
-# 
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
-
 from typing import List, Optional, Set, Tuple
 
 from .idataappsrepo import IDataAppsRepo
 from .idataappsservice import IDataAppsService
 from ..db import transaction
 from ..model import (
-    DataAppField,
     DataAppAllFields,
+    DataAppAttributes,
+    DataAppField,
     DataAppProfile
 )
 
 
 class DataAppsService(IDataAppsService):
     __slots__ = ('_dataapps_repo',)
 
     def __init__(self, dataapp_repo: IDataAppsRepo) -> None:
         self._dataapp_repo = dataapp_repo
 
     def get_all(self,
+                user_id: int,
                 attributes: Optional[Set[DataAppField]] = DataAppAllFields,
                 sort_by: Optional[List[Tuple[DataAppField, bool]]] = None,
                 skip: Optional[int] = None,
                 limit: Optional[int] = None) -> List[DataAppProfile]:
-        return self._dataapp_repo.load_all(attributes, sort_by, skip, limit)
+        return self._dataapp_repo.load_all(user_id, attributes, sort_by, skip, limit)
+
+    def user_local_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
+        return self._dataapp_repo.user_local_dataapp_list(user_id)
+
+    def user_group_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
+        return self._dataapp_repo.user_group_dataapp_list(user_id)
 
-    def create(self, attributes: DataAppProfile) -> DataAppProfile:
-        # TODO: some checks
-        # if attributes.version is None:
-        #     raise ValueError("Invalid version")
+    def create(self, attributes: DataAppAttributes, data: List[str] = None) -> DataAppProfile:
         with transaction():
-            return self._dataapp_repo.create(attributes)
+            return self._dataapp_repo.create(attributes, data)
 
     def get_dataapp(self, dataapp_name: str):
         return self._dataapp_repo.load_by_name(dataapp_name)
 
-    def delete_dataapp(self, dataapp_name: str, major: int, minor: int) -> DataAppProfile:
-        return self._dataapp_repo.delete_by_name(dataapp_name, major, minor)
+    def get_dataapp_by_id(self, uid: int) -> DataAppProfile:
+        return self._dataapp_repo.load_by_id(uid)
+
+    def delete_dataapp(self, uid: int, user_id: int) -> bool:
+        return self._dataapp_repo.delete_dataapp(uid, user_id)
 
     def delete_all(self) -> bool:
         self._dataapp_repo.delete_all()
 
-    def get_dataapp_privileges(self, dataapp_name: str) -> List[DataAppProfile]:
-        pass
-
     def get_dataapp_versions(self, dataapp_name: str) -> List[float]:
         return self._dataapp_repo.get_dataapp_versions(dataapp_name)
 
-    def get_dataapp_by_version(self, dataapp_name: str, major: int, minor: int) -> DataAppProfile:
+    def get_dataapp_by_version(self, dataapp_name: str, major: int, minor: int) -> DataAppAttributes:
         return self._dataapp_repo.get_dataapp_by_version(dataapp_name, major, minor)
 
     def get_dataapp_last_version(self, dataapp_name: str) -> float:
         self._dataapp_repo.get_dataapp_last_version(dataapp_name)
 
     def get_dataapp_tags(self, dataapp_name: str) -> List[str]:
         self._dataapp_repo.get_dataapp_tags(dataapp_name)
+
+    def get_dataapp_privileges(self, dataapp_name: str) -> List[DataAppAttributes]:
+        pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/http_docs.py` & `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsrepo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsrepo.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,63 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from abc import ABC, abstractmethod
 from typing import List, Optional, Set, Tuple
 
-from ..model import DataAppField, DataAppProfile, PrincipalId
+from ..model import DataAppField, DataAppAttributes, DataAppProfile, PrincipalId
 
 
 class IDataAppsRepo(ABC):
     @abstractmethod
-    def create(self, details: DataAppProfile) -> Optional[DataAppProfile]:
+    def load_all(self,
+                 user_id: int,
+                 attributes: Set[DataAppField],
+                 skip: Optional[int],
+                 sort_by: Optional[List[Tuple[DataAppField, bool]]],
+                 limit: Optional[int]) -> List[DataAppProfile]:
         pass
 
     @abstractmethod
-    def load_by_name(self, dataapp_name: str) -> Optional[DataAppProfile]:
+    def user_local_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
         pass
 
     @abstractmethod
-    def load_by_principal(self, principal: PrincipalId) -> Optional[DataAppProfile]:
+    def user_group_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
         pass
 
     @abstractmethod
-    def delete_all(self):
+    def create(self, details: DataAppAttributes, data: List[str] = None) -> Optional[DataAppProfile]:
         pass
 
     @abstractmethod
-    def delete_by_name(self, dataapp_name: str, major: int, minor: int):
+    def load_by_name(self, dataapp_name: str) -> Optional[DataAppProfile]:
         pass
 
     @abstractmethod
-    def load_all(self,
-                 attributes: Set[DataAppField],
-                 skip: Optional[int],
-                 sort_by: Optional[List[Tuple[DataAppField, bool]]],
-                 limit: Optional[int]) -> List[DataAppProfile]:
+    def load_by_id(self, uid: str) -> Optional[DataAppProfile]:
+        pass
+
+    @abstractmethod
+    def delete_dataapp(self, uid: int, user_id: int) -> bool:
+        pass
+
+    @abstractmethod
+    def delete_all(self):
         pass
 
     @abstractmethod
     def get_dataapp_versions(self, dataapp_name: str) -> List[float]:
         pass
 
     @abstractmethod
-    def get_dataapp_by_version(self, dataapp_name: str, major: int, minor: int) -> DataAppProfile:
+    def get_dataapp_by_version(self, dataapp_name: str, major: int, minor: int) -> DataAppAttributes:
         pass
 
     @abstractmethod
     def get_dataapp_last_version(self, dataapp_name: str) -> float:
         pass
 
     @abstractmethod
     def get_dataapp_tags(self, dataapp_name: str) -> List[str]:
         pass
+
+    @abstractmethod
+    def load_by_principal(self, principal: PrincipalId) -> Optional[DataAppAttributes]:
+        pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/dataapps/idataappsservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/dataapps/idataappsservice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,59 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from abc import ABC, abstractmethod
 from typing import List
 
-from ..model import DataAppProfile
+from ..model import DataAppAttributes, DataAppProfile
 
 
 class IDataAppsService(ABC):
+
     @abstractmethod
-    def get_all(self) -> List[DataAppProfile]:
+    def get_all(self, user_id: int) -> List[DataAppProfile]:
         pass
 
     @abstractmethod
-    def create(self, attributes: DataAppProfile) -> DataAppProfile:
+    def user_local_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
+        pass
+
+    @abstractmethod
+    def user_group_dataapp_list(self, user_id: int) -> List[DataAppProfile]:
+        pass
+
+    @abstractmethod
+    def create(self, attributes: DataAppAttributes, data: List[str] = None) -> DataAppProfile:
         pass
 
     @abstractmethod
     def get_dataapp(self, dataapp_name: str) -> DataAppProfile:
         pass
 
     @abstractmethod
-    def delete_dataapp(self, dataapp_name: str, major: int, minor: int):
+    def get_dataapp_by_id(self, uid: int) -> DataAppProfile:
         pass
 
     @abstractmethod
-    def delete_all(self) -> bool:
+    def delete_dataapp(self, uid: int, user_id: int) -> bool:
         pass
 
     @abstractmethod
-    def get_dataapp_privileges(self, dataapp_name: str) -> List[DataAppProfile]:
+    def delete_all(self) -> bool:
         pass
 
     @abstractmethod
     def get_dataapp_versions(self, dataapp_name: str) -> List[float]:
         pass
 
     @abstractmethod
-    def get_dataapp_by_version(self, dataapp_name: str, major: int, minor: int) -> DataAppProfile:
+    def get_dataapp_by_version(self, dataapp_name: str, major: int, minor: int) -> DataAppAttributes:
         pass
 
     @abstractmethod
     def get_dataapp_last_version(self, dataapp_name: str) -> float:
         pass
 
     @abstractmethod
     def get_dataapp_tags(self, dataapp_name: str) -> List[str]:
         pass
+
+    @abstractmethod
+    def get_dataapp_privileges(self, dataapp_name: str) -> List[DataAppAttributes]:
+        pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/native/database.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/native/database.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/native/settings.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/native/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_builder.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_builder.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v1.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v1.py`

 * *Files 14% similar despite different names*

```diff
@@ -74,21 +74,14 @@
             CREATE TABLE groups (
                 uid INTEGER PRIMARY KEY,
                 name VARCHAR UNIQUE NOT NULL, 
                 description VARCHAR NULL
                 );
         """)
 
-    def _insert_default_group(self,
-                              conn: Connection,
-                              group_id: int = 1,
-                              name: str = "default_group",
-                              description: str = "Unique group for Shapelets"):
-        conn.execute("INSERT INTO groups VALUES(?, ?, ?);", [group_id, name, description])
-
     def _create_dataapps_table(self, conn: Connection):
         conn.execute("""
             CREATE TABLE dataapps (
                 name VARCHAR NOT NULL, 
                 version DECIMAL NOT NULL, 
                 description VARCHAR NULL,
                 creationDate BIGINT NOT NULL,
@@ -107,13 +100,12 @@
             self._create_sequence(conn)
             self._create_user_table(conn)
             self._create_principals_table(conn)
             self._create_unp_challenges(conn)
             self._create_unp_users(conn)
             self._create_relations(conn)
             self._create_groups_table(conn)
-            self._insert_default_group(conn)
             self._create_dataapps_table(conn)
 
     def patch(self, conn: Connection):
         # Since this is the first version, no patching
         pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v2.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v2.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/schema_v3.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/schema_v3.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/db/setup.py` & `shapelets-platform-2.0.85/src/shapelets/svr/db/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import Optional
 
 from .native import Connection, DatabaseSettings, initialize_db, transaction
 from .schema_v1 import BuilderV1
 from .schema_v2 import BuilderV2
 from .schema_v3 import BuilderV3
+from .schema_v4 import BuilderV4
 
 
 def create_version_table(conn: Connection) -> str:
     conn.execute(""" 
         CREATE TABLE IF NOT EXISTS schema_version (
             version INTEGER NOT NULL
         );
@@ -30,15 +31,15 @@
 
 def setup_database(dbSettings: DatabaseSettings):
     # initialize db
     initialize_db(dbSettings)
 
     # Get a list of builders and sort them 
     # using the version property
-    builders = [BuilderV1(), BuilderV2(), BuilderV3()]
+    builders = [BuilderV1(), BuilderV2(), BuilderV3(), BuilderV4()]
     builders.sort(key=lambda x: x.version)
 
     # ensure the schema and the version table is there 
     with transaction() as conn:
         create_version_table(conn)
         version = get_schema_version(conn)
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/execution/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/execution/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/execution/executionhttp.py` & `shapelets-platform-2.0.85/src/shapelets/svr/execution/executionhttp.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 from blacksheep.server.controllers import ApiController, get, post, delete, ws
 from requests import Session
 from typing import Any, List, Optional
 
 from .iexecutionservice import IExecutionService
 from ..docs import docs
 from ..model.function import FunctionProfile
+
+
 # from ...apps.widgets import Widget
 
 
 class ExecutionHttpServer(ApiController):
     def __init__(self, svr: IExecutionService) -> None:
         self._svr = svr
         super().__init__()
@@ -26,14 +28,22 @@
     async def run_execution(self, fn: FromJSON[FunctionProfile]) -> Any:
         function = FunctionProfile(body=fn.value.body,
                                    parameters=fn.value.parameters,
                                    result=fn.value.result)
         result = self._svr.execute_function(function)
         return result.to_dict_widget()
 
+    @get("/tableData")
+    async def table_data(self, table: str, fromRow: int, n: int) -> Any:
+        return self._svr.table_data(table, fromRow, n)
+
 
 class ExecutionHttpProxy(IExecutionService):
     def __init__(self, session: Session) -> None:
         self.session = session
 
-    def execute_function(self):
-        return self.session.post('/api/executions/runFn/')
+    def execute_function(self, fn: FunctionProfile):
+        return self.session.post('/api/executions/runFn/', params=[("fn", fn)])
+
+    def table_data(self, table_id: str, from_row: int, n: int):
+        params = [("table_id", table_id), ("from_row", from_row), ("n", n)]
+        return self.session.get('/api/executions/tableData/', params=params)
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/execution/http_docs.py` & `shapelets-platform-2.0.85/src/shapelets/svr/execution/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/groups/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/groups/groupservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/groups/groupservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/groups/groupshttp.py` & `shapelets-platform-2.0.85/src/shapelets/svr/groups/groupshttp.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from requests import Session
 from typing import List, Optional
 
 from . import http_docs
 from .igroupsservice import IGroupsService, InvalidGroupName
 
 from ..docs import docs
-from ..model import GroupProfile
+from ..model import GroupProfile, GroupAttributes
 
 
 class GroupsHttpServer(ApiController):
     def __init__(self, svr: IGroupsService) -> None:
         self._svr = svr
         super().__init__()
 
@@ -27,16 +27,19 @@
     async def get_groups(self) -> List[GroupProfile]:
         try:
             return self.json(self._svr.get_all())
         except Exception as e:
             return self.status_code(500, str(e))
 
     @post("/")
-    async def create(self):
-        pass
+    async def create(self, groupName: str, groupDescription: str) -> Optional[GroupProfile]:
+        try:
+            return self.json(self._svr.create(GroupAttributes(name=groupName, description=groupDescription)))
+        except Exception as e:
+            return self.status_code(500, str(e))
 
     @get("/unp/all")
     async def get_all(self) -> List[GroupProfile]:
         try:
             return self.json(self._svr.get_all())
         except Exception as e:
             return self.status_code(500, str(e))
@@ -73,16 +76,19 @@
             return self.status_code(500, str(e))
 
 
 class GroupsHttpProxy(IGroupsService):
     def __init__(self, session: Session) -> None:
         self.session = session
 
-    def create(self):
-        pass
+    def create(self, group_name: str, group_description: str) -> Optional[GroupProfile]:
+        response = self.session.post('/api/groups/', params=[("groupName", group_name), ("groupDescription", group_description)])
+        if response.status_code == 400 or response.status_code == 500:
+            raise Exception(response.content)
+        return response.json()
 
     def get_all(self) -> List[GroupProfile]:
         response = self.session.get('/api/groups/unp/all')
         return response.json()
 
     def get_details(self, group_name: str) -> Optional[GroupProfile]:
         response = self.session.get('/api/groups/unp/details', params=[("groupName", group_name)])
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/groups/groupsrepo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/groups/groupsrepo.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     if isinstance(group_like, GroupProfile):
         return group_like.uid
     return int(group_like)
 
 
 def _next_id(conn: Connection) -> int:
     conn.execute("SELECT nextval('shapelets.id_gen')")
-    return int(conn.fetchone()[0])
+    return int(conn.fetch_one()[0])
 
 
 def _insert_group(uid: int, details: GroupAttributes, conn: Connection):
     conn.execute("""
             INSERT INTO groups 
             (uid,
             name,
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsrepo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsrepo.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,7 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from __future__ import annotations
 from abc import ABC, abstractmethod
 from typing import List, Optional, Tuple
 
 from ..model import GroupAttributes, GroupField, GroupProfile, UserProfile
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/groups/igroupsservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/groups/igroupsservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/model/dataapps.py` & `shapelets-platform-2.0.85/src/shapelets/svr/model/dataapps.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 from pydantic import BaseModel
-from typing import Optional, Set
+from typing import List, Optional, Set, Union
 from typing_extensions import Literal
 
-DataAppField = Literal['name', 'major', 'minor', 'description', 'creationDate', 'updateDate', 'specId', 'tags']
+DataAppField = Literal[
+    'uid', 'name', 'major', 'minor', 'description', 'creationDate', 'updateDate', 'specId', 'tags', 'userId']
 DataAppAllFields: Set[DataAppField] = set(
-    ['name', 'major', 'minor', 'description', 'creationDate', 'updateDate', 'specId', 'tags'])
+    ['uid', 'name', 'major', 'minor', 'description', 'creationDate', 'updateDate', 'specId', 'tags', 'userId'])
 
 
-class DataAppProfile(BaseModel):
+class DataAppAttributes(BaseModel):
     name: str
     major: Optional[int]
     minor: Optional[int]
     description: Optional[str] = None
     creationDate: Optional[int] = None
     updateDate: Optional[int] = None
     specId: Optional[str] = None
     tags: Optional[list] = None
+    userId: Optional[int] = None
+    groups: Optional[Union[List[str], str]] = None
+
+
+class DataAppProfile(DataAppAttributes):
+    uid: int
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/model/principals.py` & `shapelets-platform-2.0.85/src/shapelets/svr/model/principals.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/model/users.py` & `shapelets-platform-2.0.85/src/shapelets/svr/model/users.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,9 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from pydantic import AnyUrl, BaseModel, EmailStr
-from typing import Optional, Set, Union
+from typing import List, Optional, Set, Union
 from typing_extensions import Literal
 
 UserField = Literal[
     'uid', 'nickName', 'email', 'firstName', 'familyName', 'locale', 'picture', 'bio', 'location', 'url']
 UserAllFields: Set[UserField] = set(
     ['uid', 'nickName', 'email', 'firstName', 'familyName', 'locale', 'picture', 'bio', 'location', 'url'])
 UserId = Union[int, str]
@@ -20,12 +15,12 @@
     firstName: Optional[str] = None
     familyName: Optional[str] = None
     locale: Optional[str] = None
     picture: Optional[str] = None
     bio: Optional[str] = None
     location: Optional[str] = None
     url: Optional[AnyUrl] = None
-    groupName: Optional[str] = "default_group"
+    groupIds: Optional[List[int]] = None
 
 
 class UserProfile(UserAttributes):
     uid: int
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/asttranslation.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/asttranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/conversions.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/conversions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/core.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/core.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/decompiling.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/decompiling.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/exceptions.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/exceptions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/hashdict.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/hashdict.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/ormtypes.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/ormtypes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/prototypes/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/serialization.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/serialization.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqlbuilding.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqlbuilding.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/mustang/sqltranslation.py` & `shapelets-platform-2.0.85/src/shapelets/svr/mustang/sqltranslation.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/server.py` & `shapelets-platform-2.0.85/src/shapelets/svr/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/client.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/client.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/defaults.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/defaults.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/functions.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/functions.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/http.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/http.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/reload.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/reload.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/server.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/server.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/settings.toml` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/settings.toml`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/ssl.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/ssl.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/telemetry.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/telemetry.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/settings/websocket.py` & `shapelets-platform-2.0.85/src/shapelets/svr/settings/websocket.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/telemetry/sysinfo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/telemetry/sysinfo.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/telemetry/telemetryservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/telemetry/telemetryservice.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/users/__init__.py` & `shapelets-platform-2.0.85/src/shapelets/svr/users/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,11 @@
-# Copyright (c) 2022 Shapelets.io
-# 
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from rodi import Container
 
 from .iusersrepo import IUsersRepo
-from .iusersservice import IUsersService
+from .iusersservice import IUsersService, UserDoesNotBelong, WritePermission
 from .usershttp import UsersHttpProxy, UsersHttpServer
 from .usersrepo import UsersRepo
 from .usersservice import UsersService
 
 
 def setup_remote_client(container: Container):
     container.add_singleton(IUsersService, UsersHttpProxy)
@@ -19,9 +14,10 @@
 def setup_services(container: Container):
     container.add_singleton(IUsersRepo, UsersRepo)
     container.add_singleton(IUsersService, UsersService)
 
 
 __all__ = [
     'setup_remote_client', 'setup_services',
-    'IUsersRepo', 'IUsersService', 'UsersHttpServer'
+    'IUsersRepo', 'IUsersService', 'UsersHttpServer',
+    'UserDoesNotBelong', 'WritePermission'
 ]
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/users/http_docs.py` & `shapelets-platform-2.0.85/src/shapelets/svr/users/http_docs.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/users/iusersrepo.py` & `shapelets-platform-2.0.85/src/shapelets/svr/users/iusersrepo.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,28 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from abc import ABC, abstractmethod
 from typing import List, Optional, Set, Tuple
 
 from ..model import PrincipalId, ResolvedPrincipalId, UserAttributes, UserField, UserId, UserProfile
 
 
 class IUsersRepo(ABC):
 
     @abstractmethod
     def create(self, details: UserAttributes) -> Optional[UserProfile]:
         pass
 
     @abstractmethod
+    def add_to_group(self, user_name: str, groups: List[str], write: bool = False) -> bool:
+        pass
+
+    @abstractmethod
+    def remove_from_group(self, user_name: str, groups: List[str]) -> bool:
+        pass
+
+    @abstractmethod
     def load_by_id(self, uid: UserId) -> Optional[UserProfile]:
         pass
 
     @abstractmethod
     def load_by_name(self, name: str) -> Optional[UserProfile]:
         pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/users/iusersservice.py` & `shapelets-platform-2.0.85/src/shapelets/svr/users/iusersservice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,63 @@
-# Copyright (c) 2022 Shapelets.io
-#
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
 from abc import ABC, abstractmethod
 from typing import List, Optional, Set, Tuple, Union
 
 from ..model import (
     PrincipalId,
     ResolvedPrincipalId,
     UserAttributes,
     UserAllFields,
     UserId,
     UserField,
     UserProfile
 )
 
 
+class UserDoesNotBelong(Exception):
+    def __init__(self, user_name: str, group_name:str, *args: object) -> None:
+        self._user_name = user_name
+        self._group_name = group_name
+        super().__init__(*args)
+
+    def __str__(self) -> str:
+        return f"User {self._user_name} does not belong to the group {self._group_name}."
+
+
+class WritePermission(Exception):
+    def __init__(self, user_name: str, group_name: str, *args: object) -> None:
+        self._user_name = user_name
+        self._group_name = group_name
+        super().__init__(*args)
+
+    def __str__(self) -> str:
+        return f"User {self._user_name} has no write permission for {self._group_name} group."
+
+
 class IUsersService(ABC):
     @abstractmethod
     def get_all(self,
                 attributes: Optional[Set[UserField]] = UserAllFields,
                 sort_by: Optional[List[Tuple[UserField, bool]]] = None,
                 skip: Optional[int] = None,
                 limit: Optional[int] = None) -> List[UserProfile]:
         pass
 
     @abstractmethod
     def create(self, attributes: UserAttributes, principal: Optional[PrincipalId]) -> UserProfile:
         pass
 
     @abstractmethod
+    def add_to_group(self, user_name: str, groups: Union[List[str], str], write: bool = False) -> bool:
+        pass
+
+    @abstractmethod
+    def remove_from_group(self, user_name: str, groups: Union[List[str], str]) -> bool:
+        pass
+
+    @abstractmethod
     def delete_user(self, uid: UserId):
         pass
 
     @abstractmethod
     def delete_all(self):
         pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/users/usershttp.py` & `shapelets-platform-2.0.85/src/shapelets/svr/users/usersservice.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,114 +1,91 @@
-# Copyright (c) 2022 Shapelets.io
-# 
-# This software is released under the MIT License.
-# https://opensource.org/licenses/MIT
-
-from blacksheep.server.controllers import ApiController, delete, get, post, put
-from guardpost.asynchronous.authentication import Identity
-from requests import Session
-from typing import List, Optional
-
-from . import http_docs, IUsersService
-from ..docs import docs
-from ..model import PrincipalId, ResolvedPrincipalId, UserAttributes, UserId, UserProfile
-
-
-class UsersHttpServer(ApiController):
-    def __init__(self, svr: IUsersService) -> None:
-        self._svr = svr
-        super().__init__()
-
-    @classmethod
-    def route(cls) -> Optional[str]:
-        return '/api/users'
-
-    @get("/")
-    async def user_list(self) -> List[UserProfile]:
-        return self._svr.get_all()
-
-    @delete("/")
-    async def delete_all_users(self) -> bool:
-        return self._svr.delete_all()
-
-    @post("/checkNickName")  # description="Checks if the proposed username already exists"
-    @docs(http_docs.nickname_doc)
-    async def check_nickname(self, nickName: str) -> bool:
-        return self._svr.nickname_exists(nickName)
-
-    @get("/me")
-    @docs(http_docs.me_doc)
-    async def my_details(self, identity: Optional[Identity]) -> UserProfile:
-        if identity:
-            return self._svr.get_user_details(identity.claims.get("userId"))
-        return False
-
-    @get("/{id}")
-    async def get_user_details(self, id: int) -> Optional[UserProfile]:
-        return self._svr.get_user_details(id)
-
-    @put("/{id}")
-    async def save_user_details(self, id: int, details: UserProfile) -> Optional[UserProfile]:
-        self._svr.save_user_details(id, details)
-
-    @delete("/{id}")
-    async def delete_user(self, id: int):
-        self._svr.delete(id)
-
-    @get("/{id}/groups")
-    async def get_user_groups(self, id: int):
-        pass
-
-    @get("/{id}/principals")
-    async def get_user_principals(self, id: int) -> List[PrincipalId]:
-        return self._svr.get_principals(id)
-
-
-class UsersHttpProxy(IUsersService):
-    def __init__(self, session: Session) -> None:
-        self.session = session
-
-    def get_all(self) -> List[UserProfile]:
-        users = self.session.get('/api/users/')
-        return users
+from typing import List, Optional, Set, Tuple, Union
 
-    def create(self, attributes: UserAttributes, principal: Optional[PrincipalId]) -> UserProfile:
-        pass
-
-    def delete_user(self, id: int):
-        self.session.delete('/api/users/{id}', params=[("id", id)])
-
-    def delete_all(self) -> bool:
-        self.session.delete('/api/users/')
-        return True
-
-    def get_user_details(self, id: int) -> Optional[UserProfile]:
-        return self.session.get('/api/users/{id}', params=[("id", id)])
+from .iusersrepo import IUsersRepo
+from .iusersservice import IUsersService
+from ..db import transaction
+from ..model import (
+    PrincipalId,
+    ResolvedPrincipalId,
+    UserAttributes,
+    UserAllFields,
+    UserId,
+    UserField,
+    UserProfile
+)
+
+
+class UsersService(IUsersService):
+    __slots__ = ('_users_repo',)
+
+    def __init__(self, users_repo: IUsersRepo) -> None:
+        self._users_repo = users_repo
+
+    def get_all(self,
+                attributes: Optional[Set[UserField]] = UserAllFields,
+                sort_by: Optional[List[Tuple[UserField, bool]]] = None,
+                skip: Optional[int] = None,
+                limit: Optional[int] = None) -> List[UserProfile]:
+
+        attributes.add('uid')
+        attributes.add('nickName')
+        return self._users_repo.load_all(attributes, sort_by, skip, limit)
 
-    def save_user_details(self, id: int, details: UserProfile) -> Optional[UserProfile]:
-        self.session.put('/api/users/{id}', params=[("id", id), ("details", details)])
-        pass
-
-    @docs(http_docs.nickname_doc)
-    def nickname_exists(self, nickName: str) -> bool:
-        return self.session.get('/api/users/checkNickName', params=[("nickName", nickName)])
-
-    def get_principals(self, id: int) -> List[PrincipalId]:
-        return self.session.get('/api/users/{id}/principals', params=[("id", id)])
+    def create(self, attributes: UserAttributes, principal: Optional[PrincipalId]) -> UserProfile:
+        if attributes.nickName is None:
+            raise ValueError("Invalid user name")
+        with transaction():
+            profile = self._users_repo.create(attributes)
+            if principal is not None:
+                self._users_repo.associate_principal(profile.uid, principal)
+            return profile
+
+    def add_to_group(self, user_name: str, groups: Union[List[str], str], write: bool = False) -> bool:
+        if not isinstance(groups, list):
+            groups = [groups]
+        return self._users_repo.add_to_group(user_name, groups, write)
+
+    def remove_from_group(self, user_name: str, groups:  Union[List[str], str]) -> bool:
+        if not isinstance(groups, list):
+            groups = [groups]
+        return self._users_repo.remove_from_group(user_name, groups)
+
+    def delete_user(self, uid: UserId):
+        if isinstance(uid, str):
+            return self._users_repo.delete_by_name(uid)
+        return self._users_repo.delete_by_id(str(uid))
+
+    def delete_all(self):
+        self._users_repo.delete_all()
+
+    def get_user_details(self, user_ref: Union[UserId, PrincipalId]) -> Optional[UserProfile]:
+        if isinstance(user_ref, str):
+            return self._users_repo.load_by_name(user_ref)
+        if isinstance(user_ref, PrincipalId):
+            return self._users_repo.load_by_principal(user_ref.scope, user_ref.id)
+        return self._users_repo.load_by_id(int(user_ref))
+
+    def save_user_details(self, id: UserId, details: UserAttributes) -> Optional[UserProfile]:
+        if isinstance(id, str):
+            return self._users_repo.update_by_name(id, details)
+        return self._users_repo.update_by_id(int(id), details)
+
+    def nickname_exists(self, nickname: str) -> bool:
+        return self._users_repo.nickname_exists(nickname)
+
+    def get_principals(self, uid: UserId) -> List[PrincipalId]:
+        if isinstance(uid, str):
+            return self._users_repo.principals_by_name(uid)
+        return self._users_repo.principals_by_id(int(uid))
 
     def dissociate_principal(self, principal: PrincipalId):
-        pass
+        self._users_repo.dissociate_principal(principal)
 
     def verify_principal(self, resolved_principal: ResolvedPrincipalId) -> bool:
-        pass
+        return self._users_repo.association_exists(resolved_principal)
 
     def resolve_principal(self, scope: str, pid: str) -> Optional[ResolvedPrincipalId]:
-        pass
+        uid = self._users_repo.find_userId_by_principal(scope, pid)
+        return None if uid is None else ResolvedPrincipalId(userId=uid, scope=scope, id=pid)
 
-    def get_user_groups(self, id: int):
-        response = self.session.get('/api/users/{id}/groups', params=[("id", id)])
-        pass
-
-    @docs(http_docs.me_doc)
-    def my_details(self) -> UserProfile:
-        response = self.session.get('/api/users/me')
-        return UserProfile(uid=-1, nickName="pepe")
+    # def get_user_groups(self, uid: UserId):
+    #     pass
```

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/utils/crypto.py` & `shapelets-platform-2.0.85/src/shapelets/svr/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/utils/flexbytes.py` & `shapelets-platform-2.0.85/src/shapelets/svr/utils/flexbytes.py`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/altair.json` & `shapelets-platform-2.0.85/src/shapelets/svr/www/altair.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/asset-manifest.json` & `shapelets-platform-2.0.85/src/shapelets/svr/www/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/dataapp.json` & `shapelets-platform-2.0.85/src/shapelets/svr/www/dataapp.json`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/favicon.ico` & `shapelets-platform-2.0.85/src/shapelets/svr/www/favicon.ico`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/index.html` & `shapelets-platform-2.0.85/src/shapelets/svr/www/index.html`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/2.5f981f7f.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/css/main.8349d999.chunk.css` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/css/main.8349d999.chunk.css`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/2.de03ab12.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/3.0b0c8593.chunk.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/4.77242983.chunk.js` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/4.77242983.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/main.83b9aa07.chunk.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/js/runtime-main.fd20aea3.js`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/angle-arrow.fd898372.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/audit.cb539a06.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/audit.cb539a06.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/bin.7e762965.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/bin.7e762965.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/calendar-union.40d29ff3.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/clear.27b15301.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/clear.27b15301.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/collections.06fdf54a.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/collections.06fdf54a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/config-icon.21fc14b5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/dashboards.c7c2e0db.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/data-apps.68f8fed0.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-calendar.b3dcec1a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/date-time.a1e86419.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/date-time.a1e86419.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/download-image.87310709.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/download-image.87310709.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/filter.cec803b8.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/filter.cec803b8.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/flattened-plots.0d4072df.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-info.20e20aa1.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/header-settings.65b1d738.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/login-background.fa1c48cf.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo-shapelets.2f17f918.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logo_horizontal.66e82fe9.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logotipo-white.fd733505.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/logout.57c593a5.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/logout.57c593a5.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active-open.6959652a.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu-active.c5ce6476.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/open-menu.c8db4f67.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf-hover.08c475fc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/pdf.5d189efa.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/pdf.5d189efa.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/plus-sign.b5c476da.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb-negativo.b6c9f89e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-horizontal-color-rgb.483d5b71.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb-negativo.52482bbc.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/shapelets-isotipo-color-rgb.2781d14c.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/share.bc9a8370.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/share.bc9a8370.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/show-eye.e4cdc92e.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/single-plot.864a583b.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/single-plot.864a583b.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/teams.ba2dcf85.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/user-icon.1dfb2795.svg`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-mid.1bc00efa.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets/svr/www/static/media/wave-top.6d51781b.png` & `shapelets-platform-2.0.85/src/shapelets/svr/www/static/media/wave-top.6d51781b.png`

 * *Files identical despite different names*

### Comparing `shapelets-platform-2.0.84/src/shapelets_platform.egg-info/PKG-INFO` & `shapelets-platform-2.0.85/src/shapelets_platform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shapelets-platform
-Version: 2.0.84
+Version: 2.0.85
 Summary: Data Scientist platform
 Home-page: https://shapelets.io
 Author: Shapelets Dev Team
 Author-email: info@shapelets.io
 Maintainer: Shapelets Dev Team
 Maintainer-email: info@shapelets.io
 Project-URL: Homepage, https://shapelets.io/
```

### Comparing `shapelets-platform-2.0.84/src/shapelets_platform.egg-info/SOURCES.txt` & `shapelets-platform-2.0.85/src/shapelets_platform.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -45,20 +45,23 @@
 src/shapelets/apps/widgets/contexts/temporal_context.py
 src/shapelets/apps/widgets/controllers/__init__.py
 src/shapelets/apps/widgets/controllers/button.py
 src/shapelets/apps/widgets/controllers/checkbox.py
 src/shapelets/apps/widgets/controllers/collection_selector.py
 src/shapelets/apps/widgets/controllers/datetime_range_selector.py
 src/shapelets/apps/widgets/controllers/datetime_selector.py
+src/shapelets/apps/widgets/controllers/gauge.py
 src/shapelets/apps/widgets/controllers/image.py
 src/shapelets/apps/widgets/controllers/list.py
+src/shapelets/apps/widgets/controllers/metric.py
 src/shapelets/apps/widgets/controllers/multi_sequence_selector.py
 src/shapelets/apps/widgets/controllers/number_input.py
 src/shapelets/apps/widgets/controllers/progress.py
 src/shapelets/apps/widgets/controllers/radio_group.py
+src/shapelets/apps/widgets/controllers/ring.py
 src/shapelets/apps/widgets/controllers/selector.py
 src/shapelets/apps/widgets/controllers/sequence_list.py
 src/shapelets/apps/widgets/controllers/sequence_selector.py
 src/shapelets/apps/widgets/controllers/slider.py
 src/shapelets/apps/widgets/controllers/table.py
 src/shapelets/apps/widgets/controllers/text.py
 src/shapelets/apps/widgets/controllers/text_input.py
@@ -125,14 +128,15 @@
 src/shapelets/svr/dataapps/idataappsrepo.py
 src/shapelets/svr/dataapps/idataappsservice.py
 src/shapelets/svr/db/__init__.py
 src/shapelets/svr/db/schema_builder.py
 src/shapelets/svr/db/schema_v1.py
 src/shapelets/svr/db/schema_v2.py
 src/shapelets/svr/db/schema_v3.py
+src/shapelets/svr/db/schema_v4.py
 src/shapelets/svr/db/setup.py
 src/shapelets/svr/db/native/__init__.py
 src/shapelets/svr/db/native/database.py
 src/shapelets/svr/db/native/settings.py
 src/shapelets/svr/execution/__init__.py
 src/shapelets/svr/execution/executionhttp.py
 src/shapelets/svr/execution/executionrepo.py
```

### Comparing `shapelets-platform-2.0.84/src/shapelets_platform.egg-info/requires.txt` & `shapelets-platform-2.0.85/src/shapelets_platform.egg-info/requires.txt`

 * *Files 6% similar despite different names*

```diff
@@ -9,27 +9,29 @@
 jinja2==3.0.2
 jmespath~=0.9.3
 matplotlib>=3.5.3
 mypy~=0.990
 numpy>=1.21.6
 pandas>=1.3.5
 psutil>=5.9.2
-pyarrow>=9.0.0
+pyarrow>=12.0.0
 py-cpuinfo>=9.0.0
 pydantic>=1.10.2
 pygeohash>=1.2.0
 PyNaCl>=1.5.0
 requests>=2.28.1
-shapelets_native==2.0.84
+setuptools-scm>=7.1.0
+shapelets_native==2.0.85
 tabulate>=0.8.10
 tomlkit>=0.11.4
 tqdm>=4.64.1
+typing_extensions>=4.6.2
 uvicorn>=0.18.3
 vega-datasets>=0.9
-websocket>=0.2.1
+websocket-client>=1.5.2
 websockets>=10.3
 
 [:platform_system != "Windows"]
 lockfile>=0.12.2
 python_daemon>=2.3.2
 uvloop>=0.17.0
```

