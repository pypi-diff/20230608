# Comparing `tmp/oceanum-0.7.6.tar.gz` & `tmp/oceanum-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oceanum-0.7.6.tar", last modified: Sun May 14 21:38:12 2023, max compression
+gzip compressed data, was "oceanum-0.7.7.tar", last modified: Thu Jun  8 20:58:07 2023, max compression
```

## Comparing `oceanum-0.7.6.tar` & `oceanum-0.7.7.tar`

### file list

```diff
@@ -1,70 +1,70 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.480132 oceanum-0.7.6/
--rw-rw-r--   0 dave      (1000) dave      (1000)      151 2022-03-11 03:30:04.000000 oceanum-0.7.6/AUTHORS.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2022-02-24 22:26:12.000000 oceanum-0.7.6/CONTRIBUTING.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       89 2022-05-20 01:30:23.000000 oceanum-0.7.6/HISTORY.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2022-02-24 22:26:12.000000 oceanum-0.7.6/LICENSE
--rw-rw-r--   0 dave      (1000) dave      (1000)      262 2022-02-24 22:26:12.000000 oceanum-0.7.6/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-05-14 21:38:12.480132 oceanum-0.7.6/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)      788 2022-05-20 01:30:52.000000 oceanum-0.7.6/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.456133 oceanum-0.7.6/docs/
--rw-rw-r--   0 dave      (1000) dave      (1000)      639 2022-03-11 19:57:18.000000 oceanum-0.7.6/docs/Makefile
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.448133 oceanum-0.7.6/docs/_build/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.448133 oceanum-0.7.6/docs/_build/html/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.456133 oceanum-0.7.6/docs/_build/html/_static/
--rw-rw-r--   0 dave      (1000) dave      (1000)      286 2022-12-01 21:44:17.000000 oceanum-0.7.6/docs/_build/html/_static/file.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.7.6/docs/_build/html/_static/minus.png
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2022-12-01 21:44:17.000000 oceanum-0.7.6/docs/_build/html/_static/plus.png
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.448133 oceanum-0.7.6/docs/_templates/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.456133 oceanum-0.7.6/docs/_templates/autosummary/
--rw-rw-r--   0 dave      (1000) dave      (1000)      481 2022-03-11 19:44:27.000000 oceanum-0.7.6/docs/_templates/autosummary/class.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       73 2022-04-07 02:34:44.000000 oceanum-0.7.6/docs/about.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      593 2022-09-21 00:26:04.000000 oceanum-0.7.6/docs/api.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.448133 oceanum-0.7.6/docs/classes/
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.456133 oceanum-0.7.6/docs/classes/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      406 2022-04-08 05:43:00.000000 oceanum-0.7.6/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      713 2022-09-21 00:26:04.000000 oceanum-0.7.6/docs/classes/datamesh/oceanum.datamesh.Connector.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      131 2022-09-21 00:26:04.000000 oceanum-0.7.6/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      116 2022-04-08 05:43:00.000000 oceanum-0.7.6/docs/classes/datamesh/oceanum.datamesh.Query.rst
--rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2022-09-21 00:26:04.000000 oceanum-0.7.6/docs/conf.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      160 2022-10-12 22:11:24.000000 oceanum-0.7.6/docs/index.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2022-03-11 04:02:04.000000 oceanum-0.7.6/docs/installation.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      801 2022-03-11 19:49:35.000000 oceanum-0.7.6/docs/make.bat
--rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-01-10 19:39:49.000000 oceanum-0.7.6/docs/modules.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-01-10 19:32:56.000000 oceanum-0.7.6/docs/oceanum.datamesh.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-01-10 19:39:49.000000 oceanum-0.7.6/docs/oceanum.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2022-10-12 19:27:10.000000 oceanum-0.7.6/docs/usage.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.460132 oceanum-0.7.6/oceanum/
--rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-05-14 20:57:25.000000 oceanum-0.7.6/oceanum/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      313 2022-03-11 20:11:41.000000 oceanum-0.7.6/oceanum/cli.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.464132 oceanum-0.7.6/oceanum/datamesh/
--rw-rw-r--   0 dave      (1000) dave      (1000)      122 2022-03-11 20:13:21.000000 oceanum-0.7.6/oceanum/datamesh/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2022-11-15 20:33:48.000000 oceanum-0.7.6/oceanum/datamesh/catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    20478 2023-05-02 20:29:57.000000 oceanum-0.7.6/oceanum/datamesh/connection.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-03-21 00:40:55.000000 oceanum-0.7.6/oceanum/datamesh/datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-01-16 20:20:49.000000 oceanum-0.7.6/oceanum/datamesh/exceptions.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     7536 2023-05-14 20:54:51.000000 oceanum-0.7.6/oceanum/datamesh/query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     4683 2023-03-20 03:18:19.000000 oceanum-0.7.6/oceanum/datamesh/zarr.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.464132 oceanum-0.7.6/oceanum.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/entry_points.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/not-zip-safe
--rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/requires.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-05-14 21:38:12.000000 oceanum-0.7.6/oceanum.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-05-14 21:38:12.480132 oceanum-0.7.6/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2022-12-12 20:30:18.000000 oceanum-0.7.6/setup.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.468133 oceanum-0.7.6/tests/
--rw-rw-r--   0 dave      (1000) dave      (1000)        0 2022-02-24 22:26:12.000000 oceanum-0.7.6/tests/__init__.py
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-05-14 21:38:12.480132 oceanum-0.7.6/tests/data/
--rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2022-09-21 00:26:04.000000 oceanum-0.7.6/tests/data/grid_data_1.nc
--rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2022-12-12 20:29:37.000000 oceanum-0.7.6/tests/data/ocean_test_1.mp4
--rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2022-09-21 00:26:04.000000 oceanum-0.7.6/tests/data/point_data_1.csv
--rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2022-11-15 08:03:53.000000 oceanum-0.7.6/tests/test_catalog.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2022-11-15 03:23:40.000000 oceanum-0.7.6/tests/test_datamesh_connect.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2022-09-28 03:24:15.000000 oceanum-0.7.6/tests/test_datamesh_load.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2022-10-09 05:38:00.000000 oceanum-0.7.6/tests/test_datamesh_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-01-16 20:20:49.000000 oceanum-0.7.6/tests/test_datamesh_write.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2022-10-26 22:51:30.000000 oceanum-0.7.6/tests/test_datasource.py
--rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-03-06 19:00:50.000000 oceanum-0.7.6/tests/test_query.py
--rw-rw-r--   0 dave      (1000) dave      (1000)      805 2022-12-12 20:29:37.000000 oceanum-0.7.6/tests/test_video_compat.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.151425 oceanum-0.7.7/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      151 2023-05-14 22:31:40.000000 oceanum-0.7.7/AUTHORS.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3501 2023-05-14 22:31:40.000000 oceanum-0.7.7/CONTRIBUTING.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       89 2023-05-14 22:31:40.000000 oceanum-0.7.7/HISTORY.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1077 2023-05-14 22:31:40.000000 oceanum-0.7.7/LICENSE
+-rw-rw-r--   0 dave      (1000) dave      (1000)      262 2023-05-14 22:31:40.000000 oceanum-0.7.7/MANIFEST.in
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-08 20:58:07.151425 oceanum-0.7.7/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      788 2023-05-14 22:31:40.000000 oceanum-0.7.7/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.107426 oceanum-0.7.7/docs/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      639 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/Makefile
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/_build/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/_build/html/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.107426 oceanum-0.7.7/docs/_build/html/_static/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      286 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_build/html/_static/file.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_build/html/_static/minus.png
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_build/html/_static/plus.png
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/_templates/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.111425 oceanum-0.7.7/docs/_templates/autosummary/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      481 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/_templates/autosummary/class.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)       73 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/about.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      593 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/api.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.103426 oceanum-0.7.7/docs/classes/
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.111425 oceanum-0.7.7/docs/classes/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      406 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Catalog.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      713 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Connector.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      131 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Datasource.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      116 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Query.rst
+-rwxrwxr-x   0 dave      (1000) dave      (1000)     5220 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/conf.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      160 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/index.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1133 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/installation.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      801 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/make.bat
+-rw-rw-r--   0 dave      (1000) dave      (1000)       58 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/modules.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      967 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/oceanum.datamesh.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)      365 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/oceanum.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1437 2023-05-14 22:31:40.000000 oceanum-0.7.7/docs/usage.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.111425 oceanum-0.7.7/oceanum/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      474 2023-06-08 20:52:48.000000 oceanum-0.7.7/oceanum/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      313 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/cli.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.123425 oceanum-0.7.7/oceanum/datamesh/
+-rw-rw-r--   0 dave      (1000) dave      (1000)      122 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3425 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    20720 2023-06-08 20:52:11.000000 oceanum-0.7.7/oceanum/datamesh/connection.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10443 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      144 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/exceptions.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     7537 2023-05-14 22:35:23.000000 oceanum-0.7.7/oceanum/datamesh/query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     4683 2023-05-14 22:31:40.000000 oceanum-0.7.7/oceanum/datamesh/zarr.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.119425 oceanum-0.7.7/oceanum.egg-info/
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1180 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1384 2023-06-08 20:58:07.000000 oceanum-0.7.7/oceanum.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       45 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/entry_points.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/not-zip-safe
+-rw-rw-r--   0 dave      (1000) dave      (1000)      128 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/requires.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2023-06-08 20:58:06.000000 oceanum-0.7.7/oceanum.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)      419 2023-06-08 20:58:07.151425 oceanum-0.7.7/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1373 2023-05-14 22:31:40.000000 oceanum-0.7.7/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.127425 oceanum-0.7.7/tests/
+-rw-rw-r--   0 dave      (1000) dave      (1000)        0 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/__init__.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2023-06-08 20:58:07.151425 oceanum-0.7.7/tests/data/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    21010 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/data/grid_data_1.nc
+-rw-rw-r--   0 dave      (1000) dave      (1000)  2029589 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/data/ocean_test_1.mp4
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1727 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/data/point_data_1.csv
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1222 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_catalog.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1072 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_connect.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1643 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_load.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2578 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     3255 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datamesh_write.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2936 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_datasource.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1482 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_query.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)      805 2023-05-14 22:31:40.000000 oceanum-0.7.7/tests/test_video_compat.py
```

### Comparing `oceanum-0.7.6/CONTRIBUTING.rst` & `oceanum-0.7.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/LICENSE` & `oceanum-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/PKG-INFO` & `oceanum-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.6
+Version: 0.7.7
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.7.6/README.rst` & `oceanum-0.7.7/README.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/Makefile` & `oceanum-0.7.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/api.rst` & `oceanum-0.7.7/docs/api.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/classes/datamesh/oceanum.datamesh.Connector.rst` & `oceanum-0.7.7/docs/classes/datamesh/oceanum.datamesh.Connector.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/conf.py` & `oceanum-0.7.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/installation.rst` & `oceanum-0.7.7/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/make.bat` & `oceanum-0.7.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/oceanum.datamesh.rst` & `oceanum-0.7.7/docs/oceanum.datamesh.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/docs/usage.rst` & `oceanum-0.7.7/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/oceanum/datamesh/catalog.py` & `oceanum-0.7.7/oceanum/datamesh/catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/oceanum/datamesh/connection.py` & `oceanum-0.7.7/oceanum/datamesh/connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,16 @@
             params=params,
         )
         if resp.status_code == 404:
             raise DatameshConnectError(f"Datasource {datasource_id} not found")
         elif resp.status_code == 401:
             raise DatameshConnectError(f"Datasource {datasource_id} not Authorized")
         elif resp.status_code != 200:
-            raise DatameshConnectError(resp.text)
+            msg = resp.json()["detail"]
+            raise DatameshConnectError(msg)
         return resp
 
     def _metadata_write(self, datasource):
         if datasource._exists:
             resp = requests.patch(
                 f"{self._proto}://{self._host}/datasource/{datasource.id}/",
                 data=datasource.json(by_alias=True),
@@ -122,24 +123,26 @@
         else:
             resp = requests.post(
                 f"{self._proto}://{self._host}/datasource/",
                 data=datasource.json(by_alias=True),
                 headers={**self._auth_headers, "Content-Type": "application/json"},
             )
         if resp.status_code >= 300:
-            raise DatameshConnectError(resp.text)
+            msg = resp.json()["detail"]
+            raise DatameshConnectError(msg)
         return resp
 
     def _delete(self, datasource_id):
         resp = requests.delete(
             f"{self._gateway}/data/{datasource_id}",
             headers=self._auth_headers,
         )
         if resp.status_code >= 300:
-            raise DatameshConnectError(resp.text)
+            msg = resp.json()["detail"]
+            raise DatameshConnectError(msg)
         return True
 
     def _zarr_proxy(self, datasource_id, parameters={}):
         try:
             mapper = fsspec.get_mapper(
                 f"{self._gateway}/zarr/{datasource_id}",
                 headers={
@@ -154,15 +157,16 @@
     def _data_request(self, datasource_id, data_format="application/json", cache=False):
         tmpfile = os.path.join(self._cachedir.name, datasource_id)
         resp = requests.get(
             f"{self._gateway}/data/{datasource_id}",
             headers={"Accept": data_format, **self._auth_headers},
         )
         if not resp.status_code == 200:
-            raise DatameshConnectError(resp.text)
+            msg = resp.json()["detail"]
+            raise DatameshConnectError(msg)
         else:
             with open(tmpfile, "wb") as f:
                 f.write(resp.content)
             return tmpfile
 
     def _data_write(
         self,
@@ -184,27 +188,29 @@
                 headers["X-Append"] = str(append)
             resp = requests.patch(
                 f"{self._gateway}/data/{datasource_id}",
                 data=data,
                 headers=headers,
             )
         if not resp.status_code == 200:
-            raise DatameshConnectError(resp.text)
+            msg = resp.json()["detail"]
+            raise DatameshConnectError(msg)
         return Datasource(**resp.json())
 
     def _stage_request(self, query, cache=False):
         qhash = hashlib.sha224(query.json().encode()).hexdigest()
 
         resp = requests.post(
             f"{self._gateway}/oceanql/stage/",
             headers=self._auth_headers,
             data=query.json(),
         )
         if resp.status_code >= 400:
-            raise DatameshQueryError(resp.text)
+            msg = resp.json()["detail"]
+            raise DatameshQueryError(msg)
         elif resp.status_code == 204:
             return None
         else:
             return Stage(**resp.json())
 
     def _query(self, query, use_dask=True):
         if not isinstance(query, Query):
@@ -225,15 +231,16 @@
                 else "application/parquet"
             )
             headers = {"Accept": transfer_format, **self._auth_headers}
             resp = requests.post(
                 f"{self._gateway}/oceanql/", headers=headers, data=query.json()
             )
             if resp.status_code >= 400:
-                raise DatameshQueryError(resp.text)
+                msg = resp.json()["detail"]
+                raise DatameshQueryError(msg)
             else:
                 with tempfile.NamedTemporaryFile("wb", delete=False) as f:
                     f.write(resp.content)
                     f.seek(0)
                     if stage.container == Container.Dataset:
                         ds = xarray.load_dataset(f.name)
                     elif stage.container == Container.GeoDataFrame:
```

### Comparing `oceanum-0.7.6/oceanum/datamesh/datasource.py` & `oceanum-0.7.7/oceanum/datamesh/datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/oceanum/datamesh/query.py` & `oceanum-0.7.7/oceanum/datamesh/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     )
 
     @validator("geom", pre=True)
     def validate_geom(cls, v):
         if isinstance(v, list):
             if len(v) != 4:
                 raise ValueError(
-                    "bbox must be a list of length 4 [x_min,y_min,x_max,y_max]"
+                    "bbox must be a list of length 4: [x_min,y_min,x_max,y_max]"
                 )
         elif isinstance(v, dict):
             if "properties" not in v:
                 v["properties"] = {}
             v = Feature(**v)
         return v
```

### Comparing `oceanum-0.7.6/oceanum/datamesh/zarr.py` & `oceanum-0.7.7/oceanum/datamesh/zarr.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/oceanum.egg-info/PKG-INFO` & `oceanum-0.7.7/oceanum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oceanum
-Version: 0.7.6
+Version: 0.7.7
 Summary: Library for oceanum.io services
 Home-page: https://github.com/oceanum/oceanum-python
 Author: Oceanum Developers
 Author-email: developers@oceanum.science
 License: MIT license
 Keywords: oceanum
 License-File: LICENSE
```

### Comparing `oceanum-0.7.6/oceanum.egg-info/SOURCES.txt` & `oceanum-0.7.7/oceanum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/setup.py` & `oceanum-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/data/grid_data_1.nc` & `oceanum-0.7.7/tests/data/grid_data_1.nc`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/data/ocean_test_1.mp4` & `oceanum-0.7.7/tests/data/ocean_test_1.mp4`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/data/point_data_1.csv` & `oceanum-0.7.7/tests/data/point_data_1.csv`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_catalog.py` & `oceanum-0.7.7/tests/test_catalog.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_datamesh_connect.py` & `oceanum-0.7.7/tests/test_datamesh_connect.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_datamesh_load.py` & `oceanum-0.7.7/tests/test_datamesh_load.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_datamesh_query.py` & `oceanum-0.7.7/tests/test_datamesh_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_datamesh_write.py` & `oceanum-0.7.7/tests/test_datamesh_write.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_datasource.py` & `oceanum-0.7.7/tests/test_datasource.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_query.py` & `oceanum-0.7.7/tests/test_query.py`

 * *Files identical despite different names*

### Comparing `oceanum-0.7.6/tests/test_video_compat.py` & `oceanum-0.7.7/tests/test_video_compat.py`

 * *Files identical despite different names*

