# Comparing `tmp/netbox-plugin-device-map-0.1.2.tar.gz` & `tmp/netbox-plugin-device-map-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-plugin-device-map-0.1.2.tar", last modified: Fri Aug 26 15:02:17 2022, max compression
+gzip compressed data, was "netbox-plugin-device-map-0.1.3.tar", last modified: Thu Jun  8 10:03:09 2023, max compression
```

## Comparing `netbox-plugin-device-map-0.1.2.tar` & `netbox-plugin-device-map-0.1.3.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.747520 netbox-plugin-device-map-0.1.2/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1086 2022-08-18 08:43:06.000000 netbox-plugin-device-map-0.1.2/LICENSE
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      110 2022-04-19 08:32:25.000000 netbox-plugin-device-map-0.1.2/MANIFEST.in
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6364 2022-08-26 15:02:17.747520 netbox-plugin-device-map-0.1.2/PKG-INFO
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     5676 2022-08-26 14:09:40.000000 netbox-plugin-device-map-0.1.2/README.md
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.656520 netbox-plugin-device-map-0.1.2/netbox_device_map/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      791 2022-08-26 15:01:14.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/__init__.py
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1183 2022-04-27 10:19:18.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/forms.py
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1603 2022-04-28 13:33:44.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/geographical_map.py
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1895 2022-08-26 10:52:22.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/helpers.py
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      166 2022-04-18 10:02:29.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/navigation.py
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      302 2022-04-26 13:27:09.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/settings.py
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.649520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.656520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.657520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/js/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     4615 2022-05-25 08:49:03.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/js/map.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    11317 2022-04-26 06:24:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/js/svg-icon.js
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.689520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.700520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1259 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/layers-2x.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      696 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/layers.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     2464 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon-2x.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1466 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      618 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/marker-shadow.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   412215 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   841092 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js.map
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   437177 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   841184 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js.map
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    14661 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet.css
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   143908 2022-04-18 07:43:56.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   196318 2022-04-18 07:43:56.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js.map
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.739520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.745520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1259 2016-07-01 15:58:38.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers-2x.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      696 2016-08-05 09:33:58.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     2464 2018-04-06 20:24:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon-2x.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1466 2016-07-01 15:58:38.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6466 2022-04-21 07:12:43.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-shadow.png
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   406479 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   772884 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js.map
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   431131 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   824089 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js.map
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    14272 2022-03-11 17:51:12.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.css
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   141941 2022-03-11 18:01:26.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   194829 2022-03-11 18:00:30.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js.map
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.692520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet-sidebar/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     2938 2022-04-27 13:04:27.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.css
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6044 2022-04-27 13:04:39.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.js
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.694520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      992 2022-04-20 10:20:15.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.css
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     9510 2022-04-20 10:20:44.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      945 2022-04-20 10:24:47.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/icon-fullscreen.svg
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.698520 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1287 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.Default.css
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      872 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.css
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    81160 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   164874 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js.map
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    34136 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    41953 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js.map
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      356 2022-04-28 08:43:53.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/style.css
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.650520 netbox-plugin-device-map-0.1.2/netbox_device_map/templates/
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.745520 netbox-plugin-device-map-0.1.2/netbox_device_map/templates/netbox_device_map/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     4618 2022-05-25 08:49:44.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/templates/netbox_device_map/main.html
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      214 2022-04-27 13:45:46.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/urls.py
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     3428 2022-04-28 12:47:21.000000 netbox-plugin-device-map-0.1.2/netbox_device_map/views.py
-drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2022-08-26 15:02:17.746520 netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6364 2022-08-26 15:02:17.000000 netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/PKG-INFO
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     3460 2022-08-26 15:02:17.000000 netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/SOURCES.txt
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)        1 2022-08-26 15:02:17.000000 netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/dependency_links.txt
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)        1 2022-04-19 08:13:31.000000 netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/not-zip-safe
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)       18 2022-08-26 15:02:17.000000 netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/top_level.txt
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)       38 2022-08-26 15:02:17.747520 netbox-plugin-device-map-0.1.2/setup.cfg
--rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1010 2022-08-26 15:00:54.000000 netbox-plugin-device-map-0.1.2/setup.py
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.332836 netbox-plugin-device-map-0.1.3/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1086 2022-08-18 08:43:06.000000 netbox-plugin-device-map-0.1.3/LICENSE
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      110 2022-04-19 08:32:25.000000 netbox-plugin-device-map-0.1.3/MANIFEST.in
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6514 2023-06-08 10:03:09.332836 netbox-plugin-device-map-0.1.3/PKG-INFO
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     5826 2023-06-08 09:58:56.000000 netbox-plugin-device-map-0.1.3/README.md
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.293836 netbox-plugin-device-map-0.1.3/netbox_device_map/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      791 2023-06-08 10:01:50.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/__init__.py
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1217 2023-06-08 09:53:19.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/forms.py
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1603 2022-04-28 13:33:44.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/geographical_map.py
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1895 2023-06-08 09:14:28.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/helpers.py
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      166 2022-04-18 10:02:29.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/navigation.py
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      302 2022-04-26 13:27:09.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/settings.py
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.290836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.294836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.295836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/js/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     4615 2022-05-25 08:49:03.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/js/map.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    11317 2022-04-26 06:24:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/js/svg-icon.js
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.307836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.316836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1259 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/layers-2x.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      696 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/layers.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     2464 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon-2x.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1466 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      618 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/marker-shadow.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   412215 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   841092 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js.map
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   437177 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   841184 2022-04-18 07:43:54.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js.map
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    14661 2022-04-18 07:42:32.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet.css
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   143908 2022-04-18 07:43:56.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   196318 2022-04-18 07:43:56.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js.map
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.327836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.329836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1259 2016-07-01 15:58:38.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers-2x.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      696 2016-08-05 09:33:58.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     2464 2018-04-06 20:24:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon-2x.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1466 2016-07-01 15:58:38.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6466 2022-04-21 07:12:43.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-shadow.png
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   406479 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   772884 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js.map
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   431131 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   824089 2022-03-11 18:00:26.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js.map
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    14272 2022-03-11 17:51:12.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.css
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   141941 2022-03-11 18:01:26.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   194829 2022-03-11 18:00:30.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js.map
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.309836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet-sidebar/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     2938 2022-04-27 13:04:27.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.css
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6044 2022-04-27 13:04:39.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.js
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.310836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      992 2022-04-20 10:20:15.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.css
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     9510 2022-04-20 10:20:44.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      945 2022-04-20 10:24:47.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/icon-fullscreen.svg
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.314836 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1287 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.Default.css
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      872 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.css
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    81160 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)   164874 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js.map
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    34136 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)    41953 1985-10-26 08:15:00.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js.map
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      356 2022-04-28 08:43:53.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/style.css
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.291836 netbox-plugin-device-map-0.1.3/netbox_device_map/templates/
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.330836 netbox-plugin-device-map-0.1.3/netbox_device_map/templates/netbox_device_map/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     4618 2022-05-25 08:49:44.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/templates/netbox_device_map/main.html
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)      214 2022-04-27 13:45:46.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/urls.py
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     3428 2022-04-28 12:47:21.000000 netbox-plugin-device-map-0.1.3/netbox_device_map/views.py
+drwxr-xr-x   0 golovanenko.v (14788) пользователи домена (10513)        0 2023-06-08 10:03:09.331836 netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     6514 2023-06-08 10:03:09.000000 netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/PKG-INFO
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     3460 2023-06-08 10:03:09.000000 netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/SOURCES.txt
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)        1 2023-06-08 10:03:09.000000 netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/dependency_links.txt
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)        1 2022-04-19 08:13:31.000000 netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/not-zip-safe
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)       18 2023-06-08 10:03:09.000000 netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/top_level.txt
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)       38 2023-06-08 10:03:09.332836 netbox-plugin-device-map-0.1.3/setup.cfg
+-rw-r--r--   0 golovanenko.v (14788) пользователи домена (10513)     1010 2023-06-08 10:01:34.000000 netbox-plugin-device-map-0.1.3/setup.py
```

### Comparing `netbox-plugin-device-map-0.1.2/LICENSE` & `netbox-plugin-device-map-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/PKG-INFO` & `netbox-plugin-device-map-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-device-map
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple device map with filter criteria
 Home-page: https://github.com/drygdryg/netbox-plugin-device-map
-Download-URL: https://github.com/drygdryg/netbox-plugin-device-map/archive/v0.1.2.zip
+Download-URL: https://github.com/drygdryg/netbox-plugin-device-map/archive/v0.1.3.zip
 Author: Victor Golovanenko
 Author-email: drygdryg2014@yandex.com
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,19 @@
 # NetBox device map
 A simple device map plugin with filtering criteria for NetBox
 
 ![Map screenshot](docs/images/screenshot_map.png)
 ![Map filters screenshot](docs/images/screenshot_map_filters.png)
 
 ## Installation
+### Requirements
+The plugin has been tested and confirmed works on NetBox versions from 3.2 to 3.5 and Python versions from 3.10 to 3.11.
+
+### Steps
+
 1. If your NetBox installation uses virtualenv, activate it like this:
 ```
 source /opt/netbox/venv/bin/activate
 ```
 
 2. Install the plugin.
 
@@ -99,15 +104,15 @@
 | tiles       | …                                                                      | Tiles layer settings                                  |
 
 Custom tiles layer settings:
 
 | Setting      | Example value                                                   | Description                                                                                                                                                                                                                                                                                                                            |
 |--------------|-----------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | url_template | `https://{s}.somedomain.com/blabla/{z}/{x}/{y}{r}.png`          | `{s}` means one of the available subdomains (used sequentially to help with browser parallel requests per domain limitation; subdomain values are specified in options; a, b or c by default, can be omitted), `{z}` — zoom level, `{x}` and `{y}` — tile coordinates. `{r}` can be used to add "@2x" to the URL to load retina tiles. |
-| options      | `{'subdomains' : ['a', 'b', 'c'], 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/SlavaUkraini/reference.html#tilelayer) options                                                                                                                                                                                                                                               |
+| options      | `{'subdomains' : ['a', 'b', 'c'], 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/reference.html#tilelayer) options                                                                                                                                                                                                                                                            |
 
 ## Acknowledgements
 - [Leaflet](https://leafletjs.com/)
 ### Leaflet plugins
 - [leaflet.fullscreen](https://github.com/brunob/leaflet.fullscreen)
 - [Leaflet-SVGIcon](https://github.com/iatkin/leaflet-svgicon)
 - [leaflet-sidebar](https://github.com/Turbo87/leaflet-sidebar)
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: netbox-plugin-device-map Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: netbox-plugin-device-map Version: 0.1.3 Summary: A
 simple device map with filter criteria Home-page: https://github.com/drygdryg/
 netbox-plugin-device-map Download-URL: https://github.com/drygdryg/netbox-
-plugin-device-map/archive/v0.1.2.zip Author: Victor Golovanenko Author-email:
+plugin-device-map/archive/v0.1.3.zip Author: Victor Golovanenko Author-email:
 drygdryg2014@yandex.com License: MIT Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License Classifier: Topic :: System
 :: Networking Classifier: Topic :: System :: Systems Administration Requires-
 Python: >3.9 Description-Content-Type: text/markdown License-File: LICENSE #
 NetBox device map A simple device map plugin with filtering criteria for NetBox
 ![Map screenshot](docs/images/screenshot_map.png) ![Map filters screenshot]
-(docs/images/screenshot_map_filters.png) ## Installation 1. If your NetBox
-installation uses virtualenv, activate it like this: ``` source /opt/netbox/
-venv/bin/activate ``` 2. Install the plugin. To ensure plugin is automatically
-re-installed during future NetBox upgrades, create a file named
+(docs/images/screenshot_map_filters.png) ## Installation ### Requirements The
+plugin has been tested and confirmed works on NetBox versions from 3.2 to 3.5
+and Python versions from 3.10 to 3.11. ### Steps 1. If your NetBox installation
+uses virtualenv, activate it like this: ``` source /opt/netbox/venv/bin/
+activate ``` 2. Install the plugin. To ensure plugin is automatically re-
+installed during future NetBox upgrades, create a file named
 `local_requirements.txt` (if not already existing) in the NetBox root directory
 and list the `nextbox-plugin-device-map` package: - Option A: if you want to
 install it from PyPI: ``` echo netbox-plugin-device-map | sudo tee -a /opt/
 netbox/local_requirements.txt ``` - Option B: if you manually downloaded the
 plugin distribution from releases: ``` echo "/path/to/netbox-plugin-device-
 map.tar.gz" | sudo tee -a /opt/netbox/local_requirements.txt ``` Then run: ```
 sudo pip install -U -r /opt/netbox/local_requirements.txt ``` to install the
@@ -53,12 +55,12 @@
 -----------------| | url_template | `https://{s}.somedomain.com/blabla/{z}/{x}/
 {y}{r}.png` | `{s}` means one of the available subdomains (used sequentially to
 help with browser parallel requests per domain limitation; subdomain values are
 specified in options; a, b or c by default, can be omitted), `{z}` â zoom
 level, `{x}` and `{y}` â tile coordinates. `{r}` can be used to add "@2x" to
 the URL to load retina tiles. | | options | `{'subdomains' : ['a', 'b', 'c'],
 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/
-SlavaUkraini/reference.html#tilelayer) options | ## Acknowledgements -
-[Leaflet](https://leafletjs.com/) ### Leaflet plugins - [leaflet.fullscreen]
-(https://github.com/brunob/leaflet.fullscreen) - [Leaflet-SVGIcon](https://
-github.com/iatkin/leaflet-svgicon) - [leaflet-sidebar](https://github.com/
-Turbo87/leaflet-sidebar)
+reference.html#tilelayer) options | ## Acknowledgements - [Leaflet](https://
+leafletjs.com/) ### Leaflet plugins - [leaflet.fullscreen](https://github.com/
+brunob/leaflet.fullscreen) - [Leaflet-SVGIcon](https://github.com/iatkin/
+leaflet-svgicon) - [leaflet-sidebar](https://github.com/Turbo87/leaflet-
+sidebar)
```

### Comparing `netbox-plugin-device-map-0.1.2/README.md` & `netbox-plugin-device-map-0.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 # NetBox device map
 A simple device map plugin with filtering criteria for NetBox
 
 ![Map screenshot](docs/images/screenshot_map.png)
 ![Map filters screenshot](docs/images/screenshot_map_filters.png)
 
 ## Installation
+### Requirements
+The plugin has been tested and confirmed works on NetBox versions from 3.2 to 3.5 and Python versions from 3.10 to 3.11.
+
+### Steps
+
 1. If your NetBox installation uses virtualenv, activate it like this:
 ```
 source /opt/netbox/venv/bin/activate
 ```
 
 2. Install the plugin.
 
@@ -80,15 +85,15 @@
 | tiles       | …                                                                      | Tiles layer settings                                  |
 
 Custom tiles layer settings:
 
 | Setting      | Example value                                                   | Description                                                                                                                                                                                                                                                                                                                            |
 |--------------|-----------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | url_template | `https://{s}.somedomain.com/blabla/{z}/{x}/{y}{r}.png`          | `{s}` means one of the available subdomains (used sequentially to help with browser parallel requests per domain limitation; subdomain values are specified in options; a, b or c by default, can be omitted), `{z}` — zoom level, `{x}` and `{y}` — tile coordinates. `{r}` can be used to add "@2x" to the URL to load retina tiles. |
-| options      | `{'subdomains' : ['a', 'b', 'c'], 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/SlavaUkraini/reference.html#tilelayer) options                                                                                                                                                                                                                                               |
+| options      | `{'subdomains' : ['a', 'b', 'c'], 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/reference.html#tilelayer) options                                                                                                                                                                                                                                                            |
 
 ## Acknowledgements
 - [Leaflet](https://leafletjs.com/)
 ### Leaflet plugins
 - [leaflet.fullscreen](https://github.com/brunob/leaflet.fullscreen)
 - [Leaflet-SVGIcon](https://github.com/iatkin/leaflet-svgicon)
 - [leaflet-sidebar](https://github.com/Turbo87/leaflet-sidebar)
```

#### html2text {}

```diff
@@ -1,10 +1,12 @@
 # NetBox device map A simple device map plugin with filtering criteria for
 NetBox ![Map screenshot](docs/images/screenshot_map.png) ![Map filters
-screenshot](docs/images/screenshot_map_filters.png) ## Installation 1. If your
+screenshot](docs/images/screenshot_map_filters.png) ## Installation ###
+Requirements The plugin has been tested and confirmed works on NetBox versions
+from 3.2 to 3.5 and Python versions from 3.10 to 3.11. ### Steps 1. If your
 NetBox installation uses virtualenv, activate it like this: ``` source /opt/
 netbox/venv/bin/activate ``` 2. Install the plugin. To ensure plugin is
 automatically re-installed during future NetBox upgrades, create a file named
 `local_requirements.txt` (if not already existing) in the NetBox root directory
 and list the `nextbox-plugin-device-map` package: - Option A: if you want to
 install it from PyPI: ``` echo netbox-plugin-device-map | sudo tee -a /opt/
 netbox/local_requirements.txt ``` - Option B: if you manually downloaded the
@@ -44,12 +46,12 @@
 -----------------| | url_template | `https://{s}.somedomain.com/blabla/{z}/{x}/
 {y}{r}.png` | `{s}` means one of the available subdomains (used sequentially to
 help with browser parallel requests per domain limitation; subdomain values are
 specified in options; a, b or c by default, can be omitted), `{z}` â zoom
 level, `{x}` and `{y}` â tile coordinates. `{r}` can be used to add "@2x" to
 the URL to load retina tiles. | | options | `{'subdomains' : ['a', 'b', 'c'],
 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/
-SlavaUkraini/reference.html#tilelayer) options | ## Acknowledgements -
-[Leaflet](https://leafletjs.com/) ### Leaflet plugins - [leaflet.fullscreen]
-(https://github.com/brunob/leaflet.fullscreen) - [Leaflet-SVGIcon](https://
-github.com/iatkin/leaflet-svgicon) - [leaflet-sidebar](https://github.com/
-Turbo87/leaflet-sidebar)
+reference.html#tilelayer) options | ## Acknowledgements - [Leaflet](https://
+leafletjs.com/) ### Leaflet plugins - [leaflet.fullscreen](https://github.com/
+brunob/leaflet.fullscreen) - [Leaflet-SVGIcon](https://github.com/iatkin/
+leaflet-svgicon) - [leaflet-sidebar](https://github.com/Turbo87/leaflet-
+sidebar)
```

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/__init__.py` & `netbox-plugin-device-map-0.1.3/netbox_device_map/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from extras.plugins import PluginConfig
 
 
 class DeviceMapConfig(PluginConfig):
     name = 'netbox_device_map'
     verbose_name = 'Device map'
-    version = '0.1.2'
+    version = '0.1.3'
     author = 'Victor Golovanenko'
     author_email = 'drygdryg2014@yandex.com'
     base_url = 'device-map'
     default_settings = {
         'device_geolocation_cf': 'geolocation',
         'cpe_device_role': 'CPE',
         'geomap_settings': {
```

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/forms.py` & `netbox-plugin-device-map-0.1.3/netbox_device_map/forms.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from django import forms
 
 from dcim.models import DeviceRole, Device
 from ipam.models import VLANGroup, VLAN
-from utilities.forms import BootstrapMixin, DynamicModelChoiceField, DynamicModelMultipleChoiceField
+from utilities.forms import BootstrapMixin
+from utilities.forms.fields import DynamicModelChoiceField, DynamicModelMultipleChoiceField
 
 
 class DeviceMapFilterForm(BootstrapMixin, forms.Form):
     vlan_group = DynamicModelChoiceField(
         queryset=VLANGroup.objects.all(),
         required=False,
         label="VLAN group",
```

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/geographical_map.py` & `netbox-plugin-device-map-0.1.3/netbox_device_map/geographical_map.py`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/helpers.py` & `netbox-plugin-device-map-0.1.3/netbox_device_map/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/js/map.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/js/map.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/js/svg-icon.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/js/svg-icon.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/layers-2x.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/layers.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/layers.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon-2x.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/images/marker-shadow.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet.css` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet.css`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers-2x.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers-2x.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/layers.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon-2x.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon-2x.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-icon.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-shadow.png` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/images/marker-shadow.png`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.esm.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet-src.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.css` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.css`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet/v1.7.1/leaflet.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.css` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.css`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet-sidebar/L.Control.Sidebar.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.css` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.css`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/Control.FullScreen.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/icon-fullscreen.svg` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.fullscreen/icon-fullscreen.svg`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.Default.css` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.Default.css`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.css` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/MarkerCluster.css`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster-src.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js.map` & `netbox-plugin-device-map-0.1.3/netbox_device_map/static/netbox_device_map/leaflet.markercluster/leaflet.markercluster.js.map`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/templates/netbox_device_map/main.html` & `netbox-plugin-device-map-0.1.3/netbox_device_map/templates/netbox_device_map/main.html`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_device_map/views.py` & `netbox-plugin-device-map-0.1.3/netbox_device_map/views.py`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/PKG-INFO` & `netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: netbox-plugin-device-map
-Version: 0.1.2
+Version: 0.1.3
 Summary: A simple device map with filter criteria
 Home-page: https://github.com/drygdryg/netbox-plugin-device-map
-Download-URL: https://github.com/drygdryg/netbox-plugin-device-map/archive/v0.1.2.zip
+Download-URL: https://github.com/drygdryg/netbox-plugin-device-map/archive/v0.1.3.zip
 Author: Victor Golovanenko
 Author-email: drygdryg2014@yandex.com
 License: MIT
 Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License
@@ -20,14 +20,19 @@
 # NetBox device map
 A simple device map plugin with filtering criteria for NetBox
 
 ![Map screenshot](docs/images/screenshot_map.png)
 ![Map filters screenshot](docs/images/screenshot_map_filters.png)
 
 ## Installation
+### Requirements
+The plugin has been tested and confirmed works on NetBox versions from 3.2 to 3.5 and Python versions from 3.10 to 3.11.
+
+### Steps
+
 1. If your NetBox installation uses virtualenv, activate it like this:
 ```
 source /opt/netbox/venv/bin/activate
 ```
 
 2. Install the plugin.
 
@@ -99,15 +104,15 @@
 | tiles       | …                                                                      | Tiles layer settings                                  |
 
 Custom tiles layer settings:
 
 | Setting      | Example value                                                   | Description                                                                                                                                                                                                                                                                                                                            |
 |--------------|-----------------------------------------------------------------|----------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
 | url_template | `https://{s}.somedomain.com/blabla/{z}/{x}/{y}{r}.png`          | `{s}` means one of the available subdomains (used sequentially to help with browser parallel requests per domain limitation; subdomain values are specified in options; a, b or c by default, can be omitted), `{z}` — zoom level, `{x}` and `{y}` — tile coordinates. `{r}` can be used to add "@2x" to the URL to load retina tiles. |
-| options      | `{'subdomains' : ['a', 'b', 'c'], 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/SlavaUkraini/reference.html#tilelayer) options                                                                                                                                                                                                                                               |
+| options      | `{'subdomains' : ['a', 'b', 'c'], 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/reference.html#tilelayer) options                                                                                                                                                                                                                                                            |
 
 ## Acknowledgements
 - [Leaflet](https://leafletjs.com/)
 ### Leaflet plugins
 - [leaflet.fullscreen](https://github.com/brunob/leaflet.fullscreen)
 - [Leaflet-SVGIcon](https://github.com/iatkin/leaflet-svgicon)
 - [leaflet-sidebar](https://github.com/Turbo87/leaflet-sidebar)
```

#### html2text {}

```diff
@@ -1,22 +1,24 @@
-Metadata-Version: 2.1 Name: netbox-plugin-device-map Version: 0.1.2 Summary: A
+Metadata-Version: 2.1 Name: netbox-plugin-device-map Version: 0.1.3 Summary: A
 simple device map with filter criteria Home-page: https://github.com/drygdryg/
 netbox-plugin-device-map Download-URL: https://github.com/drygdryg/netbox-
-plugin-device-map/archive/v0.1.2.zip Author: Victor Golovanenko Author-email:
+plugin-device-map/archive/v0.1.3.zip Author: Victor Golovanenko Author-email:
 drygdryg2014@yandex.com License: MIT Classifier: Environment :: Plugins
 Classifier: Environment :: Web Environment Classifier: Framework :: Django
 Classifier: License :: OSI Approved :: MIT License Classifier: Topic :: System
 :: Networking Classifier: Topic :: System :: Systems Administration Requires-
 Python: >3.9 Description-Content-Type: text/markdown License-File: LICENSE #
 NetBox device map A simple device map plugin with filtering criteria for NetBox
 ![Map screenshot](docs/images/screenshot_map.png) ![Map filters screenshot]
-(docs/images/screenshot_map_filters.png) ## Installation 1. If your NetBox
-installation uses virtualenv, activate it like this: ``` source /opt/netbox/
-venv/bin/activate ``` 2. Install the plugin. To ensure plugin is automatically
-re-installed during future NetBox upgrades, create a file named
+(docs/images/screenshot_map_filters.png) ## Installation ### Requirements The
+plugin has been tested and confirmed works on NetBox versions from 3.2 to 3.5
+and Python versions from 3.10 to 3.11. ### Steps 1. If your NetBox installation
+uses virtualenv, activate it like this: ``` source /opt/netbox/venv/bin/
+activate ``` 2. Install the plugin. To ensure plugin is automatically re-
+installed during future NetBox upgrades, create a file named
 `local_requirements.txt` (if not already existing) in the NetBox root directory
 and list the `nextbox-plugin-device-map` package: - Option A: if you want to
 install it from PyPI: ``` echo netbox-plugin-device-map | sudo tee -a /opt/
 netbox/local_requirements.txt ``` - Option B: if you manually downloaded the
 plugin distribution from releases: ``` echo "/path/to/netbox-plugin-device-
 map.tar.gz" | sudo tee -a /opt/netbox/local_requirements.txt ``` Then run: ```
 sudo pip install -U -r /opt/netbox/local_requirements.txt ``` to install the
@@ -53,12 +55,12 @@
 -----------------| | url_template | `https://{s}.somedomain.com/blabla/{z}/{x}/
 {y}{r}.png` | `{s}` means one of the available subdomains (used sequentially to
 help with browser parallel requests per domain limitation; subdomain values are
 specified in options; a, b or c by default, can be omitted), `{z}` â zoom
 level, `{x}` and `{y}` â tile coordinates. `{r}` can be used to add "@2x" to
 the URL to load retina tiles. | | options | `{'subdomains' : ['a', 'b', 'c'],
 'minZoom': 0, 'maxZoom': 18}` | [Leaflet TileLayer](https://leafletjs.com/
-SlavaUkraini/reference.html#tilelayer) options | ## Acknowledgements -
-[Leaflet](https://leafletjs.com/) ### Leaflet plugins - [leaflet.fullscreen]
-(https://github.com/brunob/leaflet.fullscreen) - [Leaflet-SVGIcon](https://
-github.com/iatkin/leaflet-svgicon) - [leaflet-sidebar](https://github.com/
-Turbo87/leaflet-sidebar)
+reference.html#tilelayer) options | ## Acknowledgements - [Leaflet](https://
+leafletjs.com/) ### Leaflet plugins - [leaflet.fullscreen](https://github.com/
+brunob/leaflet.fullscreen) - [Leaflet-SVGIcon](https://github.com/iatkin/
+leaflet-svgicon) - [leaflet-sidebar](https://github.com/Turbo87/leaflet-
+sidebar)
```

### Comparing `netbox-plugin-device-map-0.1.2/netbox_plugin_device_map.egg-info/SOURCES.txt` & `netbox-plugin-device-map-0.1.3/netbox_plugin_device_map.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox-plugin-device-map-0.1.2/setup.py` & `netbox-plugin-device-map-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-version = '0.1.2'
+version = '0.1.3'
 
 with open('README.md', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='netbox-plugin-device-map',
     version=version,
```

