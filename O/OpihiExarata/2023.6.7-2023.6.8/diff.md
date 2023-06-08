# Comparing `tmp/OpihiExarata-2023.6.7.tar.gz` & `tmp/OpihiExarata-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpihiExarata-2023.6.7.tar", last modified: Wed Jun  7 06:52:34 2023, max compression
+gzip compressed data, was "OpihiExarata-2023.6.8.tar", last modified: Thu Jun  8 02:48:22 2023, max compression
```

## Comparing `OpihiExarata-2023.6.7.tar` & `OpihiExarata-2023.6.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.108388 OpihiExarata-2023.6.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.108388 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-07 06:52:34.000000 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-07 06:52:34.000000 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:52:34.000000 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-07 06:52:34.000000 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-07 06:52:34.000000 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-07 06:52:34.000000 OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.108388 OpihiExarata-2023.6.7/src/opihiexarata/
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.108388 OpihiExarata-2023.6.7/src/opihiexarata/astrometry/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/astrometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/astrometry/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/astrometry/webclient.py
--rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/configuration.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.108388 OpihiExarata-2023.6.7/src/opihiexarata/ephemeris/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/ephemeris/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/ephemeris/jplhorizons.py
--rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/ephemeris/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.112388 OpihiExarata-2023.6.7/src/opihiexarata/gui/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38521 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/functions.py
--rw-r--r--   0 runner    (1001) docker     (123)   128567 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/name.py
--rw-r--r--   0 runner    (1001) docker     (123)    41206 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/old_automatic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.112388 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/automatic.ui
--rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
--rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
--rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
--rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/old_manual.ui
--rw-r--r--   0 runner    (1001) docker     (123)    17002 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/qtui_automatic.py
--rw-r--r--   0 runner    (1001) docker     (123)   110826 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/qtui_manual.py
--rw-r--r--   0 runner    (1001) docker     (123)    14249 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/qtui_selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/selector.ui
--rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/window_icon.png
--rw-r--r--   0 runner    (1001) docker     (123)    50479 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/gui/selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/src/opihiexarata/library/
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    13554 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/fits.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/hint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/http.py
--rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/mpcrecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/phototable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/tcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/library/temporary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/src/opihiexarata/opihi/
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/opihi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/opihi/database.py
--rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/opihi/preprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/opihi/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/src/opihiexarata/orbit/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/orbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/orbit/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/orbit/orbfit.py
--rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/orbit/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/src/opihiexarata/photometry/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/photometry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12117 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/photometry/panstarrs.py
--rw-r--r--   0 runner    (1001) docker     (123)    34061 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/photometry/solution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/src/opihiexarata/propagate/
--rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/propagate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/propagate/polynomial.py
--rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/propagate/solution.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/src/opihiexarata/secrets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:52:34.116388 OpihiExarata-2023.6.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-07 06:52:16.000000 OpihiExarata-2023.6.7/tests/test_global.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.614615 OpihiExarata-2023.6.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 02:48:22.000000 OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8536 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22668 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29919 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/astrometry/webclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15986 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/configuration.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23092 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/jplhorizons.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7861 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.618615 OpihiExarata-2023.6.8/src/opihiexarata/gui/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39220 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6924 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)   129487 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41611 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/old_automatic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.622615 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12887 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/automatic.ui
+-rw-r--r--   0 runner    (1001) docker     (123)   264160 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png
+-rw-r--r--   0 runner    (1001) docker     (123)   276135 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   277313 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   278520 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)   282276 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png
+-rw-r--r--   0 runner    (1001) docker     (123)    81555 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    61288 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/old_manual.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    18337 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_automatic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125614 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_manual.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15431 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10677 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/selector.ui
+-rw-r--r--   0 runner    (1001) docker     (123)    32711 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/window_icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50589 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/gui/selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/library/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7723 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14051 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13735 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/hint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12014 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1043 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/mpcrecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9978 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6049 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/phototable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/tcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/library/temporary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/opihi/
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42391 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22047 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/preprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54721 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/opihi/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/orbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27658 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/orbfit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18894 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/orbit/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.626615 OpihiExarata-2023.6.8/src/opihiexarata/photometry/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/photometry/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12147 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/photometry/panstarrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34086 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/photometry/solution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/src/opihiexarata/propagate/
+-rw-r--r--   0 runner    (1001) docker     (123)      261 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/propagate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19685 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/propagate/polynomial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17859 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/propagate/solution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/src/opihiexarata/secrets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:48:22.630615 OpihiExarata-2023.6.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 02:48:05.000000 OpihiExarata-2023.6.8/tests/test_global.py
```

### Comparing `OpihiExarata-2023.6.7/LICENSE` & `OpihiExarata-2023.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/PKG-INFO` & `OpihiExarata-2023.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.6.7/README.md` & `OpihiExarata-2023.6.8/README.md`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/setup.py` & `OpihiExarata-2023.6.8/setup.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/PKG-INFO` & `OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: OpihiExarata
-Version: 2023.6.7
+Version: 2023.6.8
 Summary: Analysis software for the IRTF Opihi telescope.
 Home-page: https://github.com/psmd-iberutaru/OpihiExarata
 Author: Sparrow
 Author-email: psmd.iberutaru@gmail.com
 Project-URL: Bug Tracker, https://github.com/psmd-iberutaru/OpihiExarata/issues
 Project-URL: Documentation, https://github.com/psmd-iberutaru/OpihiExarata
 Project-URL: Source Code, https://github.com/psmd-iberutaru/OpihiExarata
```

### Comparing `OpihiExarata-2023.6.7/src/OpihiExarata.egg-info/SOURCES.txt` & `OpihiExarata-2023.6.8/src/OpihiExarata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/__init__.py` & `OpihiExarata-2023.6.8/src/opihiexarata/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/__main__.py` & `OpihiExarata-2023.6.8/src/opihiexarata/__main__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/astrometry/solution.py` & `OpihiExarata-2023.6.8/src/opihiexarata/astrometry/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/astrometry/webclient.py` & `OpihiExarata-2023.6.8/src/opihiexarata/astrometry/webclient.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/configuration.yaml` & `OpihiExarata-2023.6.8/src/opihiexarata/configuration.yaml`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/ephemeris/jplhorizons.py` & `OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/jplhorizons.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/ephemeris/solution.py` & `OpihiExarata-2023.6.8/src/opihiexarata/ephemeris/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/__init__.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/automatic.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/automatic.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 import opihiexarata.library.hint as hint
 
 import opihiexarata.astrometry as astrometry
 import opihiexarata.photometry as photometry
 
 import opihiexarata.gui as gui
 
+
 class OpihiAutomaticWindow(QtWidgets.QMainWindow):
     """The GUI that is responsible for the implementation of the automatic mode
     of Opihi, fetching images automatically based on time and solving for both
     the astrometry and photometry.
 
     Only non-GUI attributes are listed here.
 
@@ -96,15 +97,14 @@
         # The configuration file has a default fits fetch directory.
         AF_DIR = library.config.GUI_AUTOMATIC_INITIAL_AUTOMATIC_IMAGE_FETCHING_DIRECTORY
         if os.path.isdir(AF_DIR):
             self.fits_fetch_directory = os.path.abspath(AF_DIR)
         else:
             self.fits_fetch_directory = None
 
-        
         # Preparing the buttons, GUI, and other functionality.
         self.__init_gui_connections()
         self.__init_preprocess_solution()
 
         # Preparing the zero point database if the user desired the database
         # to record observations.
         if library.config.GUI_AUTOMATIC_DATABASE_SAVE_OBSERVATIONS:
@@ -116,15 +116,15 @@
         self.zero_point_database = database
 
         # Update all of the text.
         self.refresh_window()
 
         # All done.
         return None
-    
+
     def __init_gui_connections(self) -> None:
         """Creating the function connections for the GUI interface.
 
         Parameters
         ----------
         None
 
@@ -140,15 +140,14 @@
         # For the start and stop buttons.
         self.ui.push_button_start.clicked.connect(self.__connect_push_button_start)
         self.ui.push_button_stop.clicked.connect(self.__connect_push_button_stop)
         self.ui.push_button_trigger.clicked.connect(self.__connect_push_button_trigger)
 
         # All done.
         return None
-    
 
     def __init_preprocess_solution(self):
         """Initialize the preprocessing solution. The preprocessing files
         should be specified in the configuration file.
 
         Parameters
         ----------
@@ -181,21 +180,27 @@
                 bias_fits_filename=library.config.PREPROCESS_BIAS_FITS_FILENAME,
                 dark_current_fits_filename=library.config.PREPROCESS_DARK_CURRENT_FITS_FILENAME,
                 linearity_fits_filename=library.config.PREPROCESS_LINEARITY_FITS_FILENAME,
             )
         except Exception as err:
             # Something failed with making the preprocess solution, a
             # configuration file issue is likely the reason.
-            error.warn(warn_class=error.UnknownWarning, message="We are not sure why the preprocess solution failed. {e}".format(e=err))
+            error.warn(
+                warn_class=error.UnknownWarning,
+                message=(
+                    "We are not sure why the preprocess solution failed. {e}".format(
+                        e=err
+                    )
+                ),
+            )
         finally:
             self.preprocess_solution = preprocess
         # All done.
         return None
 
-
     def __connect_push_button_change_directory(self) -> None:
         """The connection for the button to change the automatic fetch
         directory.
 
         Parameters
         ----------
         None
@@ -311,100 +316,113 @@
         except ValueError:
             # There is likely no actual matching file in the directory.
             fetched_filename = None
         else:
             # Absolute paths are generally much easier to work with.
             fetched_filename = os.path.abspath(fetched_filename)
         return fetched_filename
-    
-    def verify_new_filename(self, filename:str) -> bool:
-        """This function verifies a filename. Basically, it checks that the 
+
+    def verify_new_filename(self, filename: str) -> bool:
+        """This function verifies a filename. Basically, it checks that the
         file exists and has not already been done before.
-        
+
         Parameters
         ----------
         filename : string
             The filename to verify.
 
         Returns
         -------
         verification : bool
             If the filename is good, it it True.
         """
+        # We assume the filename is good.
+        verification = True
+
         # Initial check.
         if filename is None:
             # There is no filename.
             verification = False
             return verification
         else:
-            filename = str(filename)
-        
-        # Absolute paths are easier to work with.
-        filename = os.path.abspath(filename)
-        # We assume the filename is good.
-        verification = True
+            # Absolute paths are easier to work with.
+            filename = os.path.abspath(str(filename))
 
         # We first need to test if the file even exits.
         if not os.path.isfile(filename):
             # The file does not exist so it fails verification.
             verification = False
 
         # If the file is the same as the results file, it
         # has already been done.
         working_fits_filename = str(copy.deepcopy(self.working_fits_filename))
         results_fits_filename = str(copy.deepcopy(self.results_fits_filename))
-        if os.path.isfile(working_fits_filename) and os.path.samefile(filename, working_fits_filename):
+        if os.path.isfile(working_fits_filename) and os.path.samefile(
+            filename, working_fits_filename
+        ):
             verification = False
-        if os.path.isfile(results_fits_filename) and os.path.samefile(filename, results_fits_filename):
+        if os.path.isfile(results_fits_filename) and os.path.samefile(
+            filename, results_fits_filename
+        ):
             verification = False
 
         # If the file is already a processed file.
         if library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX in filename:
             verification = False
         if library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX in filename:
             verification = False
 
         # If there exists processed versions of the file.
-        file_dir, file_base, file_ext = library.path.split_pathname(
-            pathname=filename
-        )
+        file_dir, file_base, file_ext = library.path.split_pathname(pathname=filename)
         proposed_preprocess_filename = library.path.merge_pathname(
-                    directory=file_dir,
-                    filename=file_base + library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX,
-                    extension=file_ext,
-                )
-        proposed_processed_filename = library.path.merge_pathname(
-                    directory=file_dir,
-                    filename=file_base + library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX,
-                    extension=file_ext,
-                )
+            directory=file_dir,
+            filename=file_base + library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX,
+            extension=file_ext,
+        )
+        proposed_solved_filename = library.path.merge_pathname(
+            directory=file_dir,
+            filename=file_base
+            + library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX,
+            extension=file_ext,
+        )
+        proposed_preprocess_solved_filename = library.path.merge_pathname(
+            directory=file_dir,
+            filename=file_base
+            + library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX
+            + library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX,
+            extension=file_ext,
+        )
         if os.path.isfile(proposed_preprocess_filename):
             verification = False
-        if os.path.isfile(proposed_processed_filename):
+        if os.path.isfile(proposed_solved_filename):
+            verification = False
+        if os.path.isfile(proposed_preprocess_solved_filename):
             verification = False
 
         # We do an early exit check here to save processing time.
         if not verification:
             return verification
-        
+
         # Now we check based on all previously fetched files.
         for filedex in copy.deepcopy(self.fetch_filename_record):
             if filename == filedex:
                 verification = False
 
         # It passed all of the verification tests, only a True verification
         # should be sent.
         if not verification:
-            raise error.DevelopmentError("The automatic mode file pass all of the verification tests, but the verification is still False.")
+            raise error.DevelopmentError(
+                "The automatic mode file pass all of the verification tests, but the"
+                " verification is still False."
+            )
         return bool(verification)
-    
 
     def trigger_opihi_image_solve(self) -> None:
         """This function does a single instance of the automatic solving.
-        
+
         Parameters
         ----------
         None
 
         Returns
         -------
         None
@@ -423,28 +441,29 @@
         # The filename is officially a working filename now.
         working_fits_filename = copy.deepcopy(self.fetch_fits_filename)
         self.working_fits_filename = copy.deepcopy(working_fits_filename)
         self.refresh_window()
         # We add it to the record.
         self.fetch_filename_record.append(working_fits_filename)
 
-        # We have a new file, however, in the unlikely event that this 
+        # We have a new file, however, in the unlikely event that this
         # file is still being written and is locked under permissions because
         # it is mid-write, we wait a little bit.
         library.http.api_request_sleep(seconds=1)
 
         # If we have a preprocessing solution, we can preprocess the data first.
         if isinstance(self.preprocess_solution, opihiexarata.OpihiPreprocessSolution):
-            preprocess_filename = self.preprocess_opihi_image(filename=working_fits_filename)
+            preprocess_filename = self.preprocess_opihi_image(
+                filename=working_fits_filename
+            )
         else:
             # No preprocessing done.
             preprocess_filename = working_fits_filename
-            
 
-        # We need to determine the engines which we will be using to solve 
+        # We need to determine the engines which we will be using to solve
         # this image.
         astrometry_engine_name = self.ui.combo_box_astrometry_engine.currentText()
         astrometry_engine_name = astrometry_engine_name.casefold()
         photometry_engine_name = self.ui.combo_box_photometry_engine.currentText()
         photometry_engine_name = photometry_engine_name.casefold()
         astrometry_engine = opihiexarata.gui.functions.pick_engine_class_from_name(
             engine_name=astrometry_engine_name,
@@ -452,30 +471,38 @@
         )
         photometry_engine = opihiexarata.gui.functions.pick_engine_class_from_name(
             engine_name=photometry_engine_name,
             engine_type=library.engine.PhotometryEngine,
         )
 
         # Now, we try and solve the image.
-        opihi_solution = self.solve_opihi_image(filename=preprocess_filename, astrometry_engine=astrometry_engine, photometry_engine=photometry_engine)
+        opihi_solution = self.solve_opihi_image(
+            filename=preprocess_filename,
+            astrometry_engine=astrometry_engine,
+            photometry_engine=photometry_engine,
+        )
 
         # Refreshing any data.
         self.refresh_window()
 
         # We attempt to write a zero point record to the database, the wrapper
         # writing function checks if writing to the database is a valid
         # operation. We work on a copy of the solution just in case.
         self.write_zero_point_record_to_database(opihi_solution=opihi_solution)
 
         # Finally, we try and save the image.
         # Extracting the entire path from the current name, we are saving it
         # to the same location.
-        directory, basename, extension = library.path.split_pathname(pathname=preprocess_filename)
+        directory, basename, extension = library.path.split_pathname(
+            pathname=preprocess_filename
+        )
         # We are just adding the suffix to the filename.
-        new_basename = basename + library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX
+        new_basename = (
+            basename + library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX
+        )
         # Recombining the path.
         saving_fits_filename = library.path.merge_pathname(
             directory=directory, filename=new_basename, extension=extension
         )
         opihi_solution.save_to_fits_file(filename=saving_fits_filename, overwrite=True)
 
         # The solution is now the most recent results solution.
@@ -484,37 +511,34 @@
 
         # Refreshing any data.
         self.refresh_window()
 
         # All done.
         return None
 
-
     def threaded_trigger_opihi_image_solve(self) -> None:
-        """This function is just a wrapper around the original function to 
+        """This function is just a wrapper around the original function to
         allow for threading.
-        
+
         Parameters
         ----------
         None
 
         Returns
         -------
         None
         """
         # We just call the trigger itself. We still thread it out as to not
         # completely freeze the GUI.
         trigger_solving_thread = threading.Thread(target=self.trigger_opihi_image_solve)
         trigger_solving_thread.start()
 
-
-
     def automatic_opihi_image_solve(self) -> None:
         """This function contains the loop which runs to do automatic solving.
-        
+
         We just model automatic mode as repeatedly clicking the trigger button.
 
         Parameters
         ----------
         None
 
         Returns
@@ -523,26 +547,28 @@
         """
         # Just to check if there is already a reason to stop.
         stop = self.check_automatic_stops()
         self.refresh_window()
         if stop:
             # We should not even try to do the loop, we are stopped.
             return None
-        
+
         # Automatic triggering is an infinite loop as we want to do it
         # until stopped via the stop checks.
         while not stop:
             # See if we are to stop; if so, we stop.
             stop = self.check_automatic_stops()
             if stop:
                 break
 
             # We take a little break to ensure that, in the case of no new
             # file from the trigger, we are not hammering the disk too hard.
-            __ = library.http.api_request_sleep(seconds=library.config.GUI_AUTOMATIC_SOLVE_LOOP_COOLDOWN_DELAY_SECONDS)
+            __ = library.http.api_request_sleep(
+                seconds=library.config.GUI_AUTOMATIC_SOLVE_LOOP_COOLDOWN_DELAY_SECONDS
+            )
 
             # We attempt to do another trigger solve.
             self.threaded_trigger_opihi_image_solve()
 
             # Refreshing the window.
             self.refresh_window()
 
@@ -551,33 +577,33 @@
         # active.
         stop = True
         self.loop_state = "stopped"
         self.refresh_window()
         # All done.
         self.refresh_window()
 
-
     def threaded_automatic_opihi_image_solve(self) -> None:
-        """This function is just a wrapper around the original function to 
+        """This function is just a wrapper around the original function to
         allow for threading.
-        
+
         Parameters
         ----------
         None
 
         Returns
         -------
         None
         """
         # We just call the trigger itself. We still thread it out as to not
         # completely freeze the GUI.
-        automatic_solving_thread = threading.Thread(target=self.automatic_opihi_image_solve)
+        automatic_solving_thread = threading.Thread(
+            target=self.automatic_opihi_image_solve
+        )
         automatic_solving_thread.start()
 
-
     def check_automatic_stops(self) -> bool:
         """This function checks for the stops to stop the automatic triggering
         of the next image.
 
         Parameters
         ----------
         None
@@ -594,113 +620,128 @@
 
             # Check if internally the GUI stop flag was made.
             if self.loop_state == "running":
                 stop = False
             else:
                 stop = True
 
-            # The automatic mode should not be running during the day. We set 
+            # The automatic mode should not be running during the day. We set
             # this time as a "good enough" always-daytime limit. This also serves
             # to stop it.
             current_24hour_time = int(time.strftime("%H"))
             # Hardcoded "daytime hours".
             if 8 <= current_24hour_time <= 17:
                 stop = True
 
             # Check if a stop file was placed in the directory where the automatic
             # files are being retrieved from. As this is a manual file intervention
             # the program is considered halted rather than stopped.
             stop_file_dir = self.fits_fetch_directory
             stop_file_fname = "opihiexarata"
             stop_file_ext = "stop"
             stop_file_pathname = library.path.merge_pathname(
-                directory=stop_file_dir, filename=stop_file_fname, extension=stop_file_ext
+                directory=stop_file_dir,
+                filename=stop_file_fname,
+                extension=stop_file_ext,
             )
             if os.path.exists(stop_file_pathname):
                 self.loop_state = "halted"
                 stop = True
 
         except Exception as err:
-            # For some reason, one of the stop checks could not be done 
+            # For some reason, one of the stop checks could not be done
             # properly, we stop.
             stop = True
 
         # All done.
         return stop
 
-    def preprocess_opihi_image(self, filename:str) -> str:
-        """This function preprocess an Opihi image, where available and 
+    def preprocess_opihi_image(self, filename: str) -> str:
+        """This function preprocess an Opihi image, where available and
         returns the filename of the preprocessed file.
-        
+
         Parameters
         ----------
         filename : string
             The filename of file which will be preprocessed.
-            
+
         Returns
         -------
         preprocess_filename : string
-            The filename of the file which has been preprocessed with the 
+            The filename of the file which has been preprocessed with the
             preprocessed solution of this class instance.
         """
         # We first need to check that we have a preprocess solution.
-        if not isinstance(self.preprocess_solution, opihiexarata.OpihiPreprocessSolution):
-            raise error.InputError("The preprocess solution does not exist, we cannot preprocess any data.")
-        
+        if not isinstance(
+            self.preprocess_solution, opihiexarata.OpihiPreprocessSolution
+        ):
+            raise error.InputError(
+                "The preprocess solution does not exist, we cannot preprocess any data."
+            )
+
         # We check if the file was already preprocessed.
         header, __ = library.fits.read_fits_image_file(filename=filename)
         is_preprocessed = header.get("OXM_REDU", False)
         if is_preprocessed:
             # The file is already preprocessed, nothing to do.
             return filename
-        
+
         # Deriving the preprocessed filename.
-        file_dir, file_base, file_ext = library.path.split_pathname(
-                    pathname=filename
-                )
+        file_dir, file_base, file_ext = library.path.split_pathname(pathname=filename)
         preprocess_filename = library.path.merge_pathname(
-                    directory=file_dir,
-                    filename=file_base + library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX,
-                    extension=file_ext,
-                )
-        
+            directory=file_dir,
+            filename=file_base + library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX,
+            extension=file_ext,
+        )
+
         # Finally, we attempt to preprocess the data.
         try:
             self.preprocess_solution.preprocess_fits_file(
-                    raw_filename=filename,
-                    out_filename=preprocess_filename,
-                    overwrite=True,
-                )
+                raw_filename=filename,
+                out_filename=preprocess_filename,
+                overwrite=True,
+            )
         except Exception as err:
             # Sending out a warning.
-            error.warn(warn_class=error.UnknownWarning, message="The data could not be preprocessed, an error was thrown: {e}".format(e=err))
+            error.warn(
+                warn_class=error.UnknownWarning,
+                message=(
+                    "The data could not be preprocessed, an error was thrown: {e}".format(
+                        e=err
+                    )
+                ),
+            )
             # For some reason, the preprocessing failed. Reverting.
             preprocess_filename = filename
         # All done.
         return preprocess_filename
 
     @staticmethod
-    def solve_opihi_image(filename:str, astrometry_engine:hint.AstrometryEngine, photometry_engine:hint.PhotometryEngine) -> hint.OpihiSolution:
+    def solve_opihi_image(
+        filename: str,
+        astrometry_engine: hint.AstrometryEngine,
+        photometry_engine: hint.PhotometryEngine,
+    ) -> hint.OpihiSolution:
         """This function solves the Opihi image provided by the filename.
-        
+
         We use a static method here to be a little more thread safe.
-        
+
         Parameters
         ----------
         filename : string
             The filename to load and solve.
         astrometry_engine : AstrometryEngine
             The astrometry engine to use.
         photometry_engine : PhotometryEngine
             The photometry engine to use.
-            
+
         Returns
         -------
         opihi_solution : OpihiSolution
-            The solution class of the Opihi image after it has been solved 
+            The solution class of the Opihi image after it has been solved
             (or at least attempted to be).
         """
         # Extracting the header of this fits file to get the observing
         # metadata from it.
         header, __ = library.fits.read_fits_image_file(filename=filename)
         # The filter which image is in, extracted from the fits file,
         # assuming standard form.
@@ -733,24 +774,28 @@
             __, __ = opihi_solution.solve_astrometry(
                 solver_engine=astrometry_engine,
                 overwrite=True,
                 raise_on_error=True,
                 vehicle_args={},
             )
             __, __ = opihi_solution.solve_photometry(
-                    solver_engine=photometry_engine,
-                    overwrite=True,
-                    raise_on_error=True,
-                    vehicle_args={},
-                )
-    
+                solver_engine=photometry_engine,
+                overwrite=True,
+                raise_on_error=True,
+                vehicle_args={},
+            )
+
         except error.ExarataException as err:
             # Something went wrong with the solving. We do nothing more.
-            error.warn(warn_class=error.InputWarning, message="The filename {f} failed to solve with the error {e}".format(f=filename, e=err))
-    
+            error.warn(
+                warn_class=error.InputWarning,
+                message="The filename {f} failed to solve with the error {e}".format(
+                    f=filename, e=err
+                ),
+            )
 
         # All done.
         return opihi_solution
 
     def write_zero_point_record_to_database(
         self, opihi_solution: hint.OpihiSolution
     ) -> None:
@@ -798,16 +843,14 @@
 
         # We additionally create a new figure for the monitoring webpage.
         self.zero_point_database.create_plotly_monitoring_html_plot_via_configuration()
 
         # All done.
         return None
 
-
-
     def refresh_window(self) -> None:
         """Refreshes the GUI window with new information where available.
 
         Parameters
         ----------
         None
 
@@ -975,37 +1018,35 @@
         self.ui.label_dynamic_filter.setText("FF")
         # Operational status.
         self.ui.label_dynamic_operational_status.setText("Default")
 
         # All done.
         return None
 
-    
     def closeEvent(self, event) -> None:
-        """We override the original Qt close event to take into account the 
+        """We override the original Qt close event to take into account the
         automatic loop.
-        
+
         Parameters
         ----------
         event : ?
             The event that occurs.
-        
+
         Returns
         -------
         None
         """
         # We just need to stop the loop, if it is going on.
         self.loop_state = "halted"
         # We can close now.
         event.accept()
         # All done.
         return None
 
 
-
 def start_automatic_window() -> None:
     """This is the function to create the automatic window for usage.
 
     Parameters
     ----------
     None
 
@@ -1022,23 +1063,7 @@
     sys.exit(app.exec())
     # All done.
     return None
 
 
 if __name__ == "__main__":
     start_automatic_window()
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/functions.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/functions.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/manual.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/manual.py`

 * *Files 1% similar despite different names*

```diff
@@ -695,30 +695,44 @@
         -------
         None
         """
         # If there is no astrometric solution, nothing can be done. Exit this
         # early.
         primary_solution = self.opihi_solution_list[self.primary_file_index]
         if not isinstance(primary_solution, opihiexarata.OpihiSolution):
-            error.warn(warn_class=error.SequentialOrderWarning, message="The file does not actually have a solution attached to it.")
+            error.warn(
+                warn_class=error.SequentialOrderWarning,
+                message="The file does not actually have a solution attached to it.",
+            )
             return None
         # In order to send the TCS the target's location, it must have been
         # defined already. Otherwise, there is nothing to do.
         if (
             primary_solution.asteroid_location is None
             or primary_solution.asteroid_location == (None, None)
         ):
-            error.warn(warn_class=error.SequentialOrderWarning, message="The location of the target has not been provided, we cannot calculate a position and so nothing can be sent to the TCS.")
+            error.warn(
+                warn_class=error.SequentialOrderWarning,
+                message=(
+                    "The location of the target has not been provided, we cannot"
+                    " calculate a position and so nothing can be sent to the TCS."
+                ),
+            )
             return None
         # The astrometric solution itself is also required.
         if not (
             isinstance(primary_solution.astrometrics, astrometry.AstrometricSolution)
             and primary_solution.astrometrics_status
         ):
-            error.warn(warn_class="The astrometric solution has not been computed yet. We cannot calculate the position to send to the TCS.")
+            error.warn(
+                warn_class=(
+                    "The astrometric solution has not been computed yet. We cannot"
+                    " calculate the position to send to the TCS."
+                )
+            )
             return None
 
         # Extracting the needed parameters for the TCS command.
         # Name...
         target_name = primary_solution.asteroid_name
         # On-sky location...
         target_x, target_y = primary_solution.asteroid_location
@@ -979,17 +993,26 @@
                         overwrite=True,
                         raise_on_error=True,
                         vehicle_args=vehicle_args,
                     )
                 except error.InputError:
                     # An input error is typically due to improper filters being
                     # provided
-                    error.warn(warn_class=error.InputWarning,message="An InputError was caught from the photometry solution, this is likely because the filter was incorrect.")
+                    error.warn(
+                        warn_class=error.InputWarning,
+                        message=(
+                            "An InputError was caught from the photometry solution,"
+                            " this is likely because the filter was incorrect."
+                        ),
+                    )
                 except Exception as err:
-                    error.warn(warn_class=error.UnknownWarning, message="The following error was thrown: {e}".format(e=err))
+                    error.warn(
+                        warn_class=error.UnknownWarning,
+                        message="The following error was thrown: {e}".format(e=err),
+                    )
                     raise err
                 else:
                     # Photometry is special as the data may also be saved to the
                     # zero point database. We attempt to write a zero point record to
                     # the database, the wrapper writing function checks if writing to
                     # the database is a valid operation. We work on a copy of the
                     # solution just in case.
@@ -1163,15 +1186,21 @@
         """
         # If there is no ephemeris solution, there is nothing to be done.
         primary_solution = self.opihi_solution_list[self.primary_file_index]
         if not (
             isinstance(primary_solution, opihiexarata.OpihiSolution)
             and isinstance(primary_solution.ephemeritics, ephemeris.EphemeriticSolution)
         ):
-            error.warn(warn_class=error.SequentialOrderWarning, message="There is no ephemeris solution and thus no rates to send to update the TCS.")
+            error.warn(
+                warn_class=error.SequentialOrderWarning,
+                message=(
+                    "There is no ephemeris solution and thus no rates to send to update"
+                    " the TCS."
+                ),
+            )
             return None
 
         # We use the ephemeritic solution rates to update the TCS, the
         # function provided already converts the values as needed
         # so we can provide the units as per convention.
         # We do not care about the response for now.
         __ = library.tcs.t3io_tcs_ns_rate(
@@ -1327,15 +1356,21 @@
         """
         # If there is no propagation solution, there is nothing to be done.
         primary_solution = self.opihi_solution_list[self.primary_file_index]
         if not (
             isinstance(primary_solution, opihiexarata.OpihiSolution)
             and isinstance(primary_solution.propagatives, propagate.PropagativeSolution)
         ):
-            error.warn(warn_class=error.SequentialOrderWarning, message="There is no propagation solution and thus no rates to send to update the TCS.")
+            error.warn(
+                warn_class=error.SequentialOrderWarning,
+                message=(
+                    "There is no propagation solution and thus no rates to send to"
+                    " update the TCS."
+                ),
+            )
             return None
 
         # We use the propagative solution rates to update the TCS, the
         # function provided already converts the values as needed
         # so we can provide the units as per convention.
         # We do not care about the response for now.
         __ = library.tcs.t3io_tcs_ns_rate(
@@ -1784,15 +1819,21 @@
             archive_filename = archive_filename
         else:
             archive_filename = self._get_mpcrecord_archive_filename()
 
         # If the file does not exist, there is nothing to load so a blank
         # history is returned.
         if not os.path.isfile(archive_filename):
-            error.warn(warn_class=error.InputWarning, message="We cannot find an an archive filename for historical astroid observations. No history is being provided.")
+            error.warn(
+                warn_class=error.InputWarning,
+                message=(
+                    "We cannot find an an archive filename for historical astroid"
+                    " observations. No history is being provided."
+                ),
+            )
             target_history = []
         else:
             # Read the historical data.
             with open(archive_filename, "r") as mpcfile:
                 raw_lines = mpcfile.readlines()
                 # The files have new line characters on them, they need
                 # to be removed to have the normal 80 characters.
@@ -1822,15 +1863,21 @@
             try:
                 archive_filename = self._get_mpcrecord_archive_filename()
             except Exception:
                 archive_filename = None
         # An archive filename cannot be determined, we cannot save the
         # observational history. There is no point in continuing.
         if not isinstance(archive_filename, str):
-            error.warn(warn_class=error.InputWarning, message="The archive filename cannot be determined, so we cannot save any of the observational data.")
+            error.warn(
+                warn_class=error.InputWarning,
+                message=(
+                    "The archive filename cannot be determined, so we cannot save any"
+                    " of the observational data."
+                ),
+            )
             return None
 
         # Loading the old history.
         archive_history = self.load_target_history_archive(
             archive_filename=archive_filename
         )
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/name.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/name.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/old_automatic.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/old_automatic.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,22 @@
                 bias_fits_filename=library.config.PREPROCESS_BIAS_FITS_FILENAME,
                 dark_current_fits_filename=library.config.PREPROCESS_DARK_CURRENT_FITS_FILENAME,
                 linearity_fits_filename=library.config.PREPROCESS_LINEARITY_FITS_FILENAME,
             )
         except Exception as err:
             # Something failed with making the preprocess solution, a
             # configuration file issue is likely the reason.
-            error.warn(warn_class=error.UnknownWarning, message="We are not sure why the preprocess solution failed. {e}".format(e=err))
+            error.warn(
+                warn_class=error.UnknownWarning,
+                message=(
+                    "We are not sure why the preprocess solution failed. {e}".format(
+                        e=err
+                    )
+                ),
+            )
         finally:
             self.preprocess_solution = preprocess
         # All done.
         return None
 
     def __connect_push_button_change_directory(self) -> None:
         """The connection for the button to change the automatic fetch
@@ -426,18 +433,18 @@
             # There is likely no actual matching file in the directory.
             fetched_filename = None
         else:
             # Absolute paths are generally much easier to work with.
             fetched_filename = os.path.abspath(fetched_filename)
         return fetched_filename
 
-    def verify_new_filename(self, fetched_filename:str) -> bool:
-        """This function verifies if the new filename is actually new, or it 
+    def verify_new_filename(self, fetched_filename: str) -> bool:
+        """This function verifies if the new filename is actually new, or it
         is a file that has already been fetched before.
-        
+
         Parameters
         ----------
         fetched_filename : string
             The filename which was fetched which will be verified.
 
         Returns
         -------
@@ -447,20 +454,21 @@
         """
         # Absolute paths are easier to work with.
         fetched_filename = os.path.abspath(fetched_filename)
         # We first need to test if the file even exits.
         if not os.path.isfile(fetched_filename):
             # The file does not exist so it fails verification.
             return False
+
         # If the file is the same as any of the previously fetched files.
         def _is_same_file(file_1: str, file_2: str) -> bool:
             """A small inner function to see if two files are the same
             for the purposes of fetching files.
-            
-            Note we also check for the root of the filename so we avoid any 
+
+            Note we also check for the root of the filename so we avoid any
             loops with the intermediate files in reduction.
             """
             # Assume false, they are not the same file.
             file_1 = file_1 if isinstance(file_1, str) else ""
             file_2 = file_2 if isinstance(file_2, str) else ""
             # If they are the same...
             if file_1 == file_2:
@@ -469,33 +477,37 @@
             if not os.path.isfile(file_1) and not os.path.isfile(file_2):
                 return True
             # If they are the same file in the OS...
             try:
                 return bool(os.path.samefile(file_1, file_2))
             except FileNotFoundError:
                 pass
-            # If their base names are the same; assuming we remove all of the 
+            # If their base names are the same; assuming we remove all of the
             # reduction tags.
-            base_file_1 = file_1.replace(library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, "").replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
-            base_file_2 = file_2.replace(library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, "").replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
+            base_file_1 = file_1.replace(
+                library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, ""
+            ).replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
+            base_file_2 = file_2.replace(
+                library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, ""
+            ).replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
             if base_file_1 == base_file_2:
                 return True
             # All done; as no check says they are the same file, they are not.
             return False
+
         # We test on the working and results files.
         if _is_same_file(file_1=fetched_filename, file_2=self.working_fits_filename):
             return False
         if _is_same_file(file_1=fetched_filename, file_2=self.results_fits_filename):
             return False
         # Finally, we test on all other files in the record.
         for filedex in copy.deepcopy(self.fetch_filename_record):
             if _is_same_file(file_1=fetched_filename, file_2=filedex):
                 return False
 
-
     def solve_astrometry_photometry_single_image(
         self, filename: str
     ) -> hint.OpihiSolution:
         """This solves for the astrometric and photometric solutions of a
         provided file. The engines are provided based on the dropdown menus.
 
         Note this calculation does not affect the `opihi_solution` instance of
@@ -584,15 +596,23 @@
         # Check that the filter compatibility. If the photometry failed, this
         # may be one of the reasons so it is something to warn about.
         if not photometry_solve_status:
             avaliable_filters = getattr(
                 opihi_solution.photometrics, "available_filters", []
             )
             if filter_name not in avaliable_filters:
-                error.warn(warn_class=error.FilterWarning, message="The filter {f} is not within the list of available filters {af}; hence photometry failed.".format(f=filter_name, af=avaliable_filters))
+                error.warn(
+                    warn_class=error.FilterWarning,
+                    message=(
+                        "The filter {f} is not within the list of available filters"
+                        " {af}; hence photometry failed.".format(
+                            f=filter_name, af=avaliable_filters
+                        )
+                    ),
+                )
 
         # Saving the file.
         # Extracting the entire path from the current name, we are saving it
         # to the same location.
         directory, basename, extension = library.path.split_pathname(pathname=filename)
         # We are just adding the suffix to the filename.
         suffix = str(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX)
@@ -687,16 +707,16 @@
         fetched_filename = self.fetch_new_filename()
 
         # Test to see if we have already processed this file and currently
         # have information about it. This prevents doing too much work.
         def _is_same_file(file_1: str, file_2: str) -> bool:
             """A small inner function to see if two files are the same
             for the purposes of fetching files.
-            
-            Note we also check for the root of the filename so we avoid any 
+
+            Note we also check for the root of the filename so we avoid any
             loops with the intermediate files in reduction.
             """
             # Assume false, they are not the same file.
             file_1 = file_1 if isinstance(file_1, str) else ""
             file_2 = file_2 if isinstance(file_2, str) else ""
             # If they are the same...
             if file_1 == file_2:
@@ -705,18 +725,22 @@
             if not os.path.isfile(file_1) and not os.path.isfile(file_2):
                 return True
             # If they are the same file in the OS...
             try:
                 return bool(os.path.samefile(file_1, file_2))
             except FileNotFoundError:
                 pass
-            # If their base names are the same; assuming we remove all of the 
+            # If their base names are the same; assuming we remove all of the
             # reduction tags.
-            base_file_1 = file_1.replace(library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, "").replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
-            base_file_2 = file_2.replace(library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, "").replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
+            base_file_1 = file_1.replace(
+                library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, ""
+            ).replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
+            base_file_2 = file_2.replace(
+                library.config.PREPROCESS_DEFAULT_SAVING_SUFFIX, ""
+            ).replace(library.config.GUI_AUTOMATIC_DEFAULT_FITS_SAVING_SUFFIX, "")
             if base_file_1 == base_file_2:
                 return True
 
             # All done; as no check says they are the same file, they are not.
             return False
 
         # Checking if the files are the same...
@@ -732,15 +756,15 @@
             return None
         else:
             # This new file becomes our working file.
             self.working_fits_filename = fetched_filename
             # Keeping the GUI up to date while in the loop.
             self.refresh_window()
 
-        # We have a new file, however, in the unlikely event that this 
+        # We have a new file, however, in the unlikely event that this
         # file is still being written and is locked under permissions because
         # it is mid-write, we wait a little bit.
         library.http.api_request_sleep(seconds=1)
 
         # With this new working fits file, we attempt to solve it.
         # First preprocessing the file. We desire to reduce the data if a
         # preprocess solution exists to do so.
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/automatic.ui` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/automatic.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_1of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_2of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_3of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/busy_image_pyukumuku_4of4.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/manual.ui` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/old_manual.ui` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/old_manual.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/qtui_automatic.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_automatic.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,323 +4,465 @@
 ## Form generated from reading UI file 'automatic.ui'
 ##
 ## Created by: Qt User Interface Compiler version 6.4.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
-    QFont, QFontDatabase, QGradient, QIcon,
-    QImage, QKeySequence, QLinearGradient, QPainter,
-    QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QApplication, QComboBox, QFrame, QGridLayout,
-    QHBoxLayout, QLabel, QMainWindow, QPushButton,
-    QSizePolicy, QVBoxLayout, QWidget)
+from PySide6.QtCore import (
+    QCoreApplication,
+    QDate,
+    QDateTime,
+    QLocale,
+    QMetaObject,
+    QObject,
+    QPoint,
+    QRect,
+    QSize,
+    QTime,
+    QUrl,
+    Qt,
+)
+from PySide6.QtGui import (
+    QBrush,
+    QColor,
+    QConicalGradient,
+    QCursor,
+    QFont,
+    QFontDatabase,
+    QGradient,
+    QIcon,
+    QImage,
+    QKeySequence,
+    QLinearGradient,
+    QPainter,
+    QPalette,
+    QPixmap,
+    QRadialGradient,
+    QTransform,
+)
+from PySide6.QtWidgets import (
+    QApplication,
+    QComboBox,
+    QFrame,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QMainWindow,
+    QPushButton,
+    QSizePolicy,
+    QVBoxLayout,
+    QWidget,
+)
+
 
 class Ui_AutomaticWindow(object):
     def setupUi(self, AutomaticWindow):
         if not AutomaticWindow.objectName():
-            AutomaticWindow.setObjectName(u"AutomaticWindow")
+            AutomaticWindow.setObjectName("AutomaticWindow")
         AutomaticWindow.resize(621, 360)
         self.centralwidget = QWidget(AutomaticWindow)
-        self.centralwidget.setObjectName(u"centralwidget")
+        self.centralwidget.setObjectName("centralwidget")
         self.verticalLayoutWidget = QWidget(self.centralwidget)
-        self.verticalLayoutWidget.setObjectName(u"verticalLayoutWidget")
+        self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
         self.verticalLayoutWidget.setGeometry(QRect(9, 9, 601, 341))
         font = QFont()
-        font.setFamilies([u"Cantarell"])
+        font.setFamilies(["Cantarell"])
         font.setPointSize(12)
         self.verticalLayoutWidget.setFont(font)
         self.vertical_layout_automatic = QVBoxLayout(self.verticalLayoutWidget)
-        self.vertical_layout_automatic.setObjectName(u"vertical_layout_automatic")
+        self.vertical_layout_automatic.setObjectName("vertical_layout_automatic")
         self.vertical_layout_automatic.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_directory = QHBoxLayout()
-        self.horizontal_layout_directory.setObjectName(u"horizontal_layout_directory")
+        self.horizontal_layout_directory.setObjectName("horizontal_layout_directory")
         self.label_static_fits_directory = QLabel(self.verticalLayoutWidget)
-        self.label_static_fits_directory.setObjectName(u"label_static_fits_directory")
+        self.label_static_fits_directory.setObjectName("label_static_fits_directory")
         self.label_static_fits_directory.setFont(font)
 
         self.horizontal_layout_directory.addWidget(self.label_static_fits_directory)
 
         self.label_dynamic_fits_directory = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_fits_directory.setObjectName(u"label_dynamic_fits_directory")
+        self.label_dynamic_fits_directory.setObjectName("label_dynamic_fits_directory")
         self.label_dynamic_fits_directory.setFont(font)
 
         self.horizontal_layout_directory.addWidget(self.label_dynamic_fits_directory)
 
         self.line_4 = QFrame(self.verticalLayoutWidget)
-        self.line_4.setObjectName(u"line_4")
+        self.line_4.setObjectName("line_4")
         font1 = QFont()
-        font1.setFamilies([u"Cantarell"])
+        font1.setFamilies(["Cantarell"])
         self.line_4.setFont(font1)
         self.line_4.setFrameShape(QFrame.VLine)
         self.line_4.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_directory.addWidget(self.line_4)
 
         self.push_button_change_directory = QPushButton(self.verticalLayoutWidget)
-        self.push_button_change_directory.setObjectName(u"push_button_change_directory")
+        self.push_button_change_directory.setObjectName("push_button_change_directory")
         self.push_button_change_directory.setFont(font)
 
         self.horizontal_layout_directory.addWidget(self.push_button_change_directory)
 
-
         self.vertical_layout_automatic.addLayout(self.horizontal_layout_directory)
 
         self.line_7 = QFrame(self.verticalLayoutWidget)
-        self.line_7.setObjectName(u"line_7")
+        self.line_7.setObjectName("line_7")
         self.line_7.setFont(font1)
         self.line_7.setFrameShape(QFrame.HLine)
         self.line_7.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_automatic.addWidget(self.line_7)
 
         self.horizontal_layout_engines = QHBoxLayout()
-        self.horizontal_layout_engines.setObjectName(u"horizontal_layout_engines")
+        self.horizontal_layout_engines.setObjectName("horizontal_layout_engines")
         self.label_static_engines = QLabel(self.verticalLayoutWidget)
-        self.label_static_engines.setObjectName(u"label_static_engines")
+        self.label_static_engines.setObjectName("label_static_engines")
         self.label_static_engines.setFont(font1)
 
         self.horizontal_layout_engines.addWidget(self.label_static_engines)
 
         self.combo_box_astrometry_engine = QComboBox(self.verticalLayoutWidget)
         self.combo_box_astrometry_engine.addItem("")
         self.combo_box_astrometry_engine.addItem("")
-        self.combo_box_astrometry_engine.setObjectName(u"combo_box_astrometry_engine")
+        self.combo_box_astrometry_engine.setObjectName("combo_box_astrometry_engine")
         self.combo_box_astrometry_engine.setFont(font1)
 
         self.horizontal_layout_engines.addWidget(self.combo_box_astrometry_engine)
 
         self.combo_box_photometry_engine = QComboBox(self.verticalLayoutWidget)
         self.combo_box_photometry_engine.addItem("")
-        self.combo_box_photometry_engine.setObjectName(u"combo_box_photometry_engine")
+        self.combo_box_photometry_engine.setObjectName("combo_box_photometry_engine")
         self.combo_box_photometry_engine.setFont(font1)
 
         self.horizontal_layout_engines.addWidget(self.combo_box_photometry_engine)
 
-
         self.vertical_layout_automatic.addLayout(self.horizontal_layout_engines)
 
         self.line_2 = QFrame(self.verticalLayoutWidget)
-        self.line_2.setObjectName(u"line_2")
+        self.line_2.setObjectName("line_2")
         self.line_2.setFont(font1)
         self.line_2.setFrameShape(QFrame.HLine)
         self.line_2.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_automatic.addWidget(self.line_2)
 
         self.grid_layout_fits_filenames = QGridLayout()
-        self.grid_layout_fits_filenames.setObjectName(u"grid_layout_fits_filenames")
+        self.grid_layout_fits_filenames.setObjectName("grid_layout_fits_filenames")
         self.label_static_results_filename = QLabel(self.verticalLayoutWidget)
-        self.label_static_results_filename.setObjectName(u"label_static_results_filename")
+        self.label_static_results_filename.setObjectName(
+            "label_static_results_filename"
+        )
         self.label_static_results_filename.setFont(font1)
 
-        self.grid_layout_fits_filenames.addWidget(self.label_static_results_filename, 2, 0, 1, 1)
+        self.grid_layout_fits_filenames.addWidget(
+            self.label_static_results_filename, 2, 0, 1, 1
+        )
 
         self.label_dynamic_results_filename = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_results_filename.setObjectName(u"label_dynamic_results_filename")
+        self.label_dynamic_results_filename.setObjectName(
+            "label_dynamic_results_filename"
+        )
         self.label_dynamic_results_filename.setFont(font1)
 
-        self.grid_layout_fits_filenames.addWidget(self.label_dynamic_results_filename, 2, 1, 1, 1)
+        self.grid_layout_fits_filenames.addWidget(
+            self.label_dynamic_results_filename, 2, 1, 1, 1
+        )
 
         self.label_static_working_filename = QLabel(self.verticalLayoutWidget)
-        self.label_static_working_filename.setObjectName(u"label_static_working_filename")
+        self.label_static_working_filename.setObjectName(
+            "label_static_working_filename"
+        )
         self.label_static_working_filename.setFont(font1)
 
-        self.grid_layout_fits_filenames.addWidget(self.label_static_working_filename, 1, 0, 1, 1)
+        self.grid_layout_fits_filenames.addWidget(
+            self.label_static_working_filename, 1, 0, 1, 1
+        )
 
         self.label_dynamic_working_filename = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_working_filename.setObjectName(u"label_dynamic_working_filename")
+        self.label_dynamic_working_filename.setObjectName(
+            "label_dynamic_working_filename"
+        )
         self.label_dynamic_working_filename.setFont(font1)
 
-        self.grid_layout_fits_filenames.addWidget(self.label_dynamic_working_filename, 1, 1, 1, 1)
+        self.grid_layout_fits_filenames.addWidget(
+            self.label_dynamic_working_filename, 1, 1, 1, 1
+        )
 
         self.label_static_fetch_filename = QLabel(self.verticalLayoutWidget)
-        self.label_static_fetch_filename.setObjectName(u"label_static_fetch_filename")
+        self.label_static_fetch_filename.setObjectName("label_static_fetch_filename")
 
-        self.grid_layout_fits_filenames.addWidget(self.label_static_fetch_filename, 0, 0, 1, 1)
+        self.grid_layout_fits_filenames.addWidget(
+            self.label_static_fetch_filename, 0, 0, 1, 1
+        )
 
         self.label_dynamic_fetch_filename = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_fetch_filename.setObjectName(u"label_dynamic_fetch_filename")
-
-        self.grid_layout_fits_filenames.addWidget(self.label_dynamic_fetch_filename, 0, 1, 1, 1)
+        self.label_dynamic_fetch_filename.setObjectName("label_dynamic_fetch_filename")
 
+        self.grid_layout_fits_filenames.addWidget(
+            self.label_dynamic_fetch_filename, 0, 1, 1, 1
+        )
 
         self.vertical_layout_automatic.addLayout(self.grid_layout_fits_filenames)
 
         self.horizontal_layout_astrometry_results = QHBoxLayout()
-        self.horizontal_layout_astrometry_results.setObjectName(u"horizontal_layout_astrometry_results")
+        self.horizontal_layout_astrometry_results.setObjectName(
+            "horizontal_layout_astrometry_results"
+        )
         self.label_static_ra_dec = QLabel(self.verticalLayoutWidget)
-        self.label_static_ra_dec.setObjectName(u"label_static_ra_dec")
+        self.label_static_ra_dec.setObjectName("label_static_ra_dec")
         self.label_static_ra_dec.setFont(font1)
 
         self.horizontal_layout_astrometry_results.addWidget(self.label_static_ra_dec)
 
         self.label_dynamic_ra = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_ra.setObjectName(u"label_dynamic_ra")
+        self.label_dynamic_ra.setObjectName("label_dynamic_ra")
         self.label_dynamic_ra.setFont(font1)
 
         self.horizontal_layout_astrometry_results.addWidget(self.label_dynamic_ra)
 
         self.label_dynamic_dec = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_dec.setObjectName(u"label_dynamic_dec")
+        self.label_dynamic_dec.setObjectName("label_dynamic_dec")
         self.label_dynamic_dec.setFont(font1)
 
         self.horizontal_layout_astrometry_results.addWidget(self.label_dynamic_dec)
 
         self.line_9 = QFrame(self.verticalLayoutWidget)
-        self.line_9.setObjectName(u"line_9")
+        self.line_9.setObjectName("line_9")
         self.line_9.setFont(font1)
         self.line_9.setFrameShape(QFrame.VLine)
         self.line_9.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_astrometry_results.addWidget(self.line_9)
 
         self.label_dynamic_date = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_date.setObjectName(u"label_dynamic_date")
+        self.label_dynamic_date.setObjectName("label_dynamic_date")
         self.label_dynamic_date.setFont(font1)
         self.label_dynamic_date.setAlignment(Qt.AlignCenter)
 
         self.horizontal_layout_astrometry_results.addWidget(self.label_dynamic_date)
 
         self.label_dynamic_time = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_time.setObjectName(u"label_dynamic_time")
+        self.label_dynamic_time.setObjectName("label_dynamic_time")
         self.label_dynamic_time.setFont(font1)
         self.label_dynamic_time.setAlignment(Qt.AlignCenter)
 
         self.horizontal_layout_astrometry_results.addWidget(self.label_dynamic_time)
 
-
-        self.vertical_layout_automatic.addLayout(self.horizontal_layout_astrometry_results)
+        self.vertical_layout_automatic.addLayout(
+            self.horizontal_layout_astrometry_results
+        )
 
         self.horizontal_layout_photometry_results = QHBoxLayout()
-        self.horizontal_layout_photometry_results.setObjectName(u"horizontal_layout_photometry_results")
+        self.horizontal_layout_photometry_results.setObjectName(
+            "horizontal_layout_photometry_results"
+        )
         self.label_static_zero_point = QLabel(self.verticalLayoutWidget)
-        self.label_static_zero_point.setObjectName(u"label_static_zero_point")
+        self.label_static_zero_point.setObjectName("label_static_zero_point")
         self.label_static_zero_point.setFont(font1)
 
-        self.horizontal_layout_photometry_results.addWidget(self.label_static_zero_point)
+        self.horizontal_layout_photometry_results.addWidget(
+            self.label_static_zero_point
+        )
 
         self.label_dynamic_zero_point = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_zero_point.setObjectName(u"label_dynamic_zero_point")
+        self.label_dynamic_zero_point.setObjectName("label_dynamic_zero_point")
         self.label_dynamic_zero_point.setFont(font1)
 
-        self.horizontal_layout_photometry_results.addWidget(self.label_dynamic_zero_point)
+        self.horizontal_layout_photometry_results.addWidget(
+            self.label_dynamic_zero_point
+        )
 
         self.line_5 = QFrame(self.verticalLayoutWidget)
-        self.line_5.setObjectName(u"line_5")
+        self.line_5.setObjectName("line_5")
         self.line_5.setFont(font1)
         self.line_5.setFrameShape(QFrame.VLine)
         self.line_5.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_photometry_results.addWidget(self.line_5)
 
         self.label_static_filter = QLabel(self.verticalLayoutWidget)
-        self.label_static_filter.setObjectName(u"label_static_filter")
+        self.label_static_filter.setObjectName("label_static_filter")
         self.label_static_filter.setFont(font1)
 
         self.horizontal_layout_photometry_results.addWidget(self.label_static_filter)
 
         self.label_dynamic_filter = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_filter.setObjectName(u"label_dynamic_filter")
+        self.label_dynamic_filter.setObjectName("label_dynamic_filter")
         self.label_dynamic_filter.setFont(font1)
 
         self.horizontal_layout_photometry_results.addWidget(self.label_dynamic_filter)
 
-
-        self.vertical_layout_automatic.addLayout(self.horizontal_layout_photometry_results)
+        self.vertical_layout_automatic.addLayout(
+            self.horizontal_layout_photometry_results
+        )
 
         self.line = QFrame(self.verticalLayoutWidget)
-        self.line.setObjectName(u"line")
+        self.line.setObjectName("line")
         self.line.setFont(font)
         self.line.setFrameShape(QFrame.HLine)
         self.line.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_automatic.addWidget(self.line)
 
         self.horizontal_layout_start_stop = QHBoxLayout()
-        self.horizontal_layout_start_stop.setObjectName(u"horizontal_layout_start_stop")
+        self.horizontal_layout_start_stop.setObjectName("horizontal_layout_start_stop")
         self.label_static_operational_status = QLabel(self.verticalLayoutWidget)
-        self.label_static_operational_status.setObjectName(u"label_static_operational_status")
+        self.label_static_operational_status.setObjectName(
+            "label_static_operational_status"
+        )
         self.label_static_operational_status.setFont(font1)
 
-        self.horizontal_layout_start_stop.addWidget(self.label_static_operational_status)
+        self.horizontal_layout_start_stop.addWidget(
+            self.label_static_operational_status
+        )
 
         self.label_dynamic_operational_status = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_operational_status.setObjectName(u"label_dynamic_operational_status")
+        self.label_dynamic_operational_status.setObjectName(
+            "label_dynamic_operational_status"
+        )
         self.label_dynamic_operational_status.setFont(font1)
         self.label_dynamic_operational_status.setAlignment(Qt.AlignCenter)
 
-        self.horizontal_layout_start_stop.addWidget(self.label_dynamic_operational_status)
+        self.horizontal_layout_start_stop.addWidget(
+            self.label_dynamic_operational_status
+        )
 
         self.push_button_start = QPushButton(self.verticalLayoutWidget)
-        self.push_button_start.setObjectName(u"push_button_start")
+        self.push_button_start.setObjectName("push_button_start")
         self.push_button_start.setFont(font1)
 
         self.horizontal_layout_start_stop.addWidget(self.push_button_start)
 
         self.push_button_stop = QPushButton(self.verticalLayoutWidget)
-        self.push_button_stop.setObjectName(u"push_button_stop")
+        self.push_button_stop.setObjectName("push_button_stop")
         self.push_button_stop.setFont(font1)
 
         self.horizontal_layout_start_stop.addWidget(self.push_button_stop)
 
         self.line_3 = QFrame(self.verticalLayoutWidget)
-        self.line_3.setObjectName(u"line_3")
+        self.line_3.setObjectName("line_3")
         self.line_3.setFont(font1)
         self.line_3.setFrameShape(QFrame.VLine)
         self.line_3.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_start_stop.addWidget(self.line_3)
 
         self.push_button_trigger = QPushButton(self.verticalLayoutWidget)
-        self.push_button_trigger.setObjectName(u"push_button_trigger")
+        self.push_button_trigger.setObjectName("push_button_trigger")
         self.push_button_trigger.setFont(font1)
 
         self.horizontal_layout_start_stop.addWidget(self.push_button_trigger)
 
-
         self.vertical_layout_automatic.addLayout(self.horizontal_layout_start_stop)
 
         AutomaticWindow.setCentralWidget(self.centralwidget)
 
         self.retranslateUi(AutomaticWindow)
 
         QMetaObject.connectSlotsByName(AutomaticWindow)
+
     # setupUi
 
     def retranslateUi(self, AutomaticWindow):
-        AutomaticWindow.setWindowTitle(QCoreApplication.translate("AutomaticWindow", u"OpihiExarata Automatic Mode", None))
-        self.label_static_fits_directory.setText(QCoreApplication.translate("AutomaticWindow", u"Fetch Directory:", None))
-        self.label_dynamic_fits_directory.setText(QCoreApplication.translate("AutomaticWindow", u"/path/to/fits/directory/", None))
-        self.push_button_change_directory.setText(QCoreApplication.translate("AutomaticWindow", u"Change", None))
-        self.label_static_engines.setText(QCoreApplication.translate("AutomaticWindow", u"Engines (A, P)", None))
-        self.combo_box_astrometry_engine.setItemText(0, QCoreApplication.translate("AutomaticWindow", u"Astrometry.net Nova", None))
-        self.combo_box_astrometry_engine.setItemText(1, QCoreApplication.translate("AutomaticWindow", u"Astrometry.net Host", None))
-
-        self.combo_box_photometry_engine.setItemText(0, QCoreApplication.translate("AutomaticWindow", u"Pan-STARRS 3pi DR2 MAST", None))
-
-        self.label_static_results_filename.setText(QCoreApplication.translate("AutomaticWindow", u"Results:", None))
-        self.label_dynamic_results_filename.setText(QCoreApplication.translate("AutomaticWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAA.00001.b.fits", None))
-        self.label_static_working_filename.setText(QCoreApplication.translate("AutomaticWindow", u"Working:", None))
-        self.label_dynamic_working_filename.setText(QCoreApplication.translate("AutomaticWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAA.00001.a.fits", None))
-        self.label_static_fetch_filename.setText(QCoreApplication.translate("AutomaticWindow", u"Fetch:", None))
-        self.label_dynamic_fetch_filename.setText(QCoreApplication.translate("AutomaticWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAA.00001.a.fits", None))
-        self.label_static_ra_dec.setText(QCoreApplication.translate("AutomaticWindow", u"Coordinates", None))
-        self.label_dynamic_ra.setText(QCoreApplication.translate("AutomaticWindow", u"RR:RR:RR.RRR", None))
-        self.label_dynamic_dec.setText(QCoreApplication.translate("AutomaticWindow", u"+DD:DD:DD.DDD", None))
-        self.label_dynamic_date.setText(QCoreApplication.translate("AutomaticWindow", u"YYYY-MM-DD", None))
-        self.label_dynamic_time.setText(QCoreApplication.translate("AutomaticWindow", u"HH:MM:SS.S", None))
-        self.label_static_zero_point.setText(QCoreApplication.translate("AutomaticWindow", u"Zero Point", None))
-        self.label_dynamic_zero_point.setText(QCoreApplication.translate("AutomaticWindow", u"ZZZ.ZZZ + EE.EEE", None))
-        self.label_static_filter.setText(QCoreApplication.translate("AutomaticWindow", u"Filter", None))
-        self.label_dynamic_filter.setText(QCoreApplication.translate("AutomaticWindow", u"FF", None))
-        self.label_static_operational_status.setText(QCoreApplication.translate("AutomaticWindow", u"Loop Status", None))
-        self.label_dynamic_operational_status.setText(QCoreApplication.translate("AutomaticWindow", u"Default", None))
-        self.push_button_start.setText(QCoreApplication.translate("AutomaticWindow", u"Start", None))
-        self.push_button_stop.setText(QCoreApplication.translate("AutomaticWindow", u"Stop", None))
-        self.push_button_trigger.setText(QCoreApplication.translate("AutomaticWindow", u"Trigger", None))
-    # retranslateUi
+        AutomaticWindow.setWindowTitle(
+            QCoreApplication.translate(
+                "AutomaticWindow", "OpihiExarata Automatic Mode", None
+            )
+        )
+        self.label_static_fits_directory.setText(
+            QCoreApplication.translate("AutomaticWindow", "Fetch Directory:", None)
+        )
+        self.label_dynamic_fits_directory.setText(
+            QCoreApplication.translate(
+                "AutomaticWindow", "/path/to/fits/directory/", None
+            )
+        )
+        self.push_button_change_directory.setText(
+            QCoreApplication.translate("AutomaticWindow", "Change", None)
+        )
+        self.label_static_engines.setText(
+            QCoreApplication.translate("AutomaticWindow", "Engines (A, P)", None)
+        )
+        self.combo_box_astrometry_engine.setItemText(
+            0,
+            QCoreApplication.translate("AutomaticWindow", "Astrometry.net Nova", None),
+        )
+        self.combo_box_astrometry_engine.setItemText(
+            1,
+            QCoreApplication.translate("AutomaticWindow", "Astrometry.net Host", None),
+        )
+
+        self.combo_box_photometry_engine.setItemText(
+            0,
+            QCoreApplication.translate(
+                "AutomaticWindow", "Pan-STARRS 3pi DR2 MAST", None
+            ),
+        )
+
+        self.label_static_results_filename.setText(
+            QCoreApplication.translate("AutomaticWindow", "Results:", None)
+        )
+        self.label_dynamic_results_filename.setText(
+            QCoreApplication.translate(
+                "AutomaticWindow", "opi.20XXA999.YYMMDD.AAAAAAAAA.00001.b.fits", None
+            )
+        )
+        self.label_static_working_filename.setText(
+            QCoreApplication.translate("AutomaticWindow", "Working:", None)
+        )
+        self.label_dynamic_working_filename.setText(
+            QCoreApplication.translate(
+                "AutomaticWindow", "opi.20XXA999.YYMMDD.AAAAAAAAA.00001.a.fits", None
+            )
+        )
+        self.label_static_fetch_filename.setText(
+            QCoreApplication.translate("AutomaticWindow", "Fetch:", None)
+        )
+        self.label_dynamic_fetch_filename.setText(
+            QCoreApplication.translate(
+                "AutomaticWindow", "opi.20XXA999.YYMMDD.AAAAAAAAA.00001.a.fits", None
+            )
+        )
+        self.label_static_ra_dec.setText(
+            QCoreApplication.translate("AutomaticWindow", "Coordinates", None)
+        )
+        self.label_dynamic_ra.setText(
+            QCoreApplication.translate("AutomaticWindow", "RR:RR:RR.RRR", None)
+        )
+        self.label_dynamic_dec.setText(
+            QCoreApplication.translate("AutomaticWindow", "+DD:DD:DD.DDD", None)
+        )
+        self.label_dynamic_date.setText(
+            QCoreApplication.translate("AutomaticWindow", "YYYY-MM-DD", None)
+        )
+        self.label_dynamic_time.setText(
+            QCoreApplication.translate("AutomaticWindow", "HH:MM:SS.S", None)
+        )
+        self.label_static_zero_point.setText(
+            QCoreApplication.translate("AutomaticWindow", "Zero Point", None)
+        )
+        self.label_dynamic_zero_point.setText(
+            QCoreApplication.translate("AutomaticWindow", "ZZZ.ZZZ + EE.EEE", None)
+        )
+        self.label_static_filter.setText(
+            QCoreApplication.translate("AutomaticWindow", "Filter", None)
+        )
+        self.label_dynamic_filter.setText(
+            QCoreApplication.translate("AutomaticWindow", "FF", None)
+        )
+        self.label_static_operational_status.setText(
+            QCoreApplication.translate("AutomaticWindow", "Loop Status", None)
+        )
+        self.label_dynamic_operational_status.setText(
+            QCoreApplication.translate("AutomaticWindow", "Default", None)
+        )
+        self.push_button_start.setText(
+            QCoreApplication.translate("AutomaticWindow", "Start", None)
+        )
+        self.push_button_stop.setText(
+            QCoreApplication.translate("AutomaticWindow", "Stop", None)
+        )
+        self.push_button_trigger.setText(
+            QCoreApplication.translate("AutomaticWindow", "Trigger", None)
+        )
 
+    # retranslateUi
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/qtui_manual.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_manual.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,1674 +4,3053 @@
 ## Form generated from reading UI file 'manual.ui'
 ##
 ## Created by: Qt User Interface Compiler version 6.4.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
-    QFont, QFontDatabase, QGradient, QIcon,
-    QImage, QKeySequence, QLinearGradient, QPainter,
-    QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QApplication, QButtonGroup, QComboBox, QDateTimeEdit,
-    QFrame, QGraphicsView, QGridLayout, QHBoxLayout,
-    QLabel, QLayout, QLineEdit, QMainWindow,
-    QPushButton, QRadioButton, QSizePolicy, QTabWidget,
-    QVBoxLayout, QWidget)
+from PySide6.QtCore import (
+    QCoreApplication,
+    QDate,
+    QDateTime,
+    QLocale,
+    QMetaObject,
+    QObject,
+    QPoint,
+    QRect,
+    QSize,
+    QTime,
+    QUrl,
+    Qt,
+)
+from PySide6.QtGui import (
+    QBrush,
+    QColor,
+    QConicalGradient,
+    QCursor,
+    QFont,
+    QFontDatabase,
+    QGradient,
+    QIcon,
+    QImage,
+    QKeySequence,
+    QLinearGradient,
+    QPainter,
+    QPalette,
+    QPixmap,
+    QRadialGradient,
+    QTransform,
+)
+from PySide6.QtWidgets import (
+    QApplication,
+    QButtonGroup,
+    QComboBox,
+    QDateTimeEdit,
+    QFrame,
+    QGraphicsView,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QLayout,
+    QLineEdit,
+    QMainWindow,
+    QPushButton,
+    QRadioButton,
+    QSizePolicy,
+    QTabWidget,
+    QVBoxLayout,
+    QWidget,
+)
+
 
 class Ui_ManualWindow(object):
     def setupUi(self, ManualWindow):
         if not ManualWindow.objectName():
-            ManualWindow.setObjectName(u"ManualWindow")
+            ManualWindow.setObjectName("ManualWindow")
         ManualWindow.resize(930, 821)
         self.central_widget = QWidget(ManualWindow)
-        self.central_widget.setObjectName(u"central_widget")
+        self.central_widget.setObjectName("central_widget")
         self.verticalLayoutWidget = QWidget(self.central_widget)
-        self.verticalLayoutWidget.setObjectName(u"verticalLayoutWidget")
+        self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
         self.verticalLayoutWidget.setGeometry(QRect(10, 10, 911, 801))
         font = QFont()
-        font.setFamilies([u"Cantarell"])
+        font.setFamilies(["Cantarell"])
         font.setPointSize(12)
         self.verticalLayoutWidget.setFont(font)
         self.vertical_layout_window = QVBoxLayout(self.verticalLayoutWidget)
-        self.vertical_layout_window.setObjectName(u"vertical_layout_window")
+        self.vertical_layout_window.setObjectName("vertical_layout_window")
         self.vertical_layout_window.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_image_file = QHBoxLayout()
-        self.horizontal_layout_image_file.setObjectName(u"horizontal_layout_image_file")
+        self.horizontal_layout_image_file.setObjectName("horizontal_layout_image_file")
         self.vertical_layout_image = QVBoxLayout()
-        self.vertical_layout_image.setObjectName(u"vertical_layout_image")
+        self.vertical_layout_image.setObjectName("vertical_layout_image")
         self.graphics_view_dummy_opihi_image = QGraphicsView(self.verticalLayoutWidget)
-        self.graphics_view_dummy_opihi_image.setObjectName(u"graphics_view_dummy_opihi_image")
+        self.graphics_view_dummy_opihi_image.setObjectName(
+            "graphics_view_dummy_opihi_image"
+        )
         sizePolicy = QSizePolicy(QSizePolicy.Maximum, QSizePolicy.Maximum)
         sizePolicy.setHorizontalStretch(0)
         sizePolicy.setVerticalStretch(0)
-        sizePolicy.setHeightForWidth(self.graphics_view_dummy_opihi_image.sizePolicy().hasHeightForWidth())
+        sizePolicy.setHeightForWidth(
+            self.graphics_view_dummy_opihi_image.sizePolicy().hasHeightForWidth()
+        )
         self.graphics_view_dummy_opihi_image.setSizePolicy(sizePolicy)
         self.graphics_view_dummy_opihi_image.setMinimumSize(QSize(400, 400))
         self.graphics_view_dummy_opihi_image.setMaximumSize(QSize(400, 400))
         self.graphics_view_dummy_opihi_image.setFont(font)
 
         self.vertical_layout_image.addWidget(self.graphics_view_dummy_opihi_image)
 
         self.label_static_dummy_opihi_navbar = QLabel(self.verticalLayoutWidget)
-        self.label_static_dummy_opihi_navbar.setObjectName(u"label_static_dummy_opihi_navbar")
+        self.label_static_dummy_opihi_navbar.setObjectName(
+            "label_static_dummy_opihi_navbar"
+        )
         sizePolicy1 = QSizePolicy(QSizePolicy.Minimum, QSizePolicy.Preferred)
         sizePolicy1.setHorizontalStretch(0)
         sizePolicy1.setVerticalStretch(0)
-        sizePolicy1.setHeightForWidth(self.label_static_dummy_opihi_navbar.sizePolicy().hasHeightForWidth())
+        sizePolicy1.setHeightForWidth(
+            self.label_static_dummy_opihi_navbar.sizePolicy().hasHeightForWidth()
+        )
         self.label_static_dummy_opihi_navbar.setSizePolicy(sizePolicy1)
         self.label_static_dummy_opihi_navbar.setMinimumSize(QSize(0, 25))
         self.label_static_dummy_opihi_navbar.setBaseSize(QSize(0, 0))
         self.label_static_dummy_opihi_navbar.setFont(font)
         self.label_static_dummy_opihi_navbar.setAlignment(Qt.AlignCenter)
 
         self.vertical_layout_image.addWidget(self.label_static_dummy_opihi_navbar)
 
-
         self.horizontal_layout_image_file.addLayout(self.vertical_layout_image)
 
         self.line = QFrame(self.verticalLayoutWidget)
-        self.line.setObjectName(u"line")
+        self.line.setObjectName("line")
         self.line.setFont(font)
         self.line.setFrameShape(QFrame.VLine)
         self.line.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_image_file.addWidget(self.line)
 
         self.grid_layout_file_selector = QGridLayout()
-        self.grid_layout_file_selector.setObjectName(u"grid_layout_file_selector")
+        self.grid_layout_file_selector.setObjectName("grid_layout_file_selector")
         self.label_dynamic_target_4_pixel_location = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_target_4_pixel_location.setObjectName(u"label_dynamic_target_4_pixel_location")
+        self.label_dynamic_target_4_pixel_location.setObjectName(
+            "label_dynamic_target_4_pixel_location"
+        )
         self.label_dynamic_target_4_pixel_location.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_target_4_pixel_location, 12, 3, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_target_4_pixel_location, 12, 3, 1, 1
+        )
 
         self.label_static_target_3_location = QLabel(self.verticalLayoutWidget)
-        self.label_static_target_3_location.setObjectName(u"label_static_target_3_location")
-
-        self.grid_layout_file_selector.addWidget(self.label_static_target_3_location, 9, 2, 1, 1)
+        self.label_static_target_3_location.setObjectName(
+            "label_static_target_3_location"
+        )
+
+        self.grid_layout_file_selector.addWidget(
+            self.label_static_target_3_location, 9, 2, 1, 1
+        )
 
         self.label_static_target_4_location = QLabel(self.verticalLayoutWidget)
-        self.label_static_target_4_location.setObjectName(u"label_static_target_4_location")
-
-        self.grid_layout_file_selector.addWidget(self.label_static_target_4_location, 12, 2, 1, 1)
-
-        self.push_button_relocate_target_location_1 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_relocate_target_location_1.setObjectName(u"push_button_relocate_target_location_1")
+        self.label_static_target_4_location.setObjectName(
+            "label_static_target_4_location"
+        )
+
+        self.grid_layout_file_selector.addWidget(
+            self.label_static_target_4_location, 12, 2, 1, 1
+        )
+
+        self.push_button_relocate_target_location_1 = QPushButton(
+            self.verticalLayoutWidget
+        )
+        self.push_button_relocate_target_location_1.setObjectName(
+            "push_button_relocate_target_location_1"
+        )
         self.push_button_relocate_target_location_1.setFont(font)
 
-        self.grid_layout_file_selector.addWidget(self.push_button_relocate_target_location_1, 3, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_relocate_target_location_1, 3, 4, 1, 1
+        )
 
         self.label_dynamic_target_1_pixel_location = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_target_1_pixel_location.setObjectName(u"label_dynamic_target_1_pixel_location")
+        self.label_dynamic_target_1_pixel_location.setObjectName(
+            "label_dynamic_target_1_pixel_location"
+        )
         self.label_dynamic_target_1_pixel_location.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_target_1_pixel_location, 3, 3, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_target_1_pixel_location, 3, 3, 1, 1
+        )
 
         self.push_button_load_filename_3 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_load_filename_3.setObjectName(u"push_button_load_filename_3")
+        self.push_button_load_filename_3.setObjectName("push_button_load_filename_3")
 
-        self.grid_layout_file_selector.addWidget(self.push_button_load_filename_3, 8, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_load_filename_3, 8, 4, 1, 1
+        )
 
         self.label_dynamic_filename_3 = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_filename_3.setObjectName(u"label_dynamic_filename_3")
+        self.label_dynamic_filename_3.setObjectName("label_dynamic_filename_3")
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_filename_3, 8, 0, 1, 4)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_filename_3, 8, 0, 1, 4
+        )
 
         self.label_dynamic_filename_1 = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_filename_1.setObjectName(u"label_dynamic_filename_1")
+        self.label_dynamic_filename_1.setObjectName("label_dynamic_filename_1")
         self.label_dynamic_filename_1.setFont(font)
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_filename_1, 2, 0, 1, 4)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_filename_1, 2, 0, 1, 4
+        )
 
         self.label_dynamic_filename_2 = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_filename_2.setObjectName(u"label_dynamic_filename_2")
+        self.label_dynamic_filename_2.setObjectName("label_dynamic_filename_2")
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_filename_2, 5, 0, 1, 4)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_filename_2, 5, 0, 1, 4
+        )
 
         self.line_35 = QFrame(self.verticalLayoutWidget)
-        self.line_35.setObjectName(u"line_35")
+        self.line_35.setObjectName("line_35")
         self.line_35.setFrameShape(QFrame.VLine)
         self.line_35.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_35, 6, 1, 1, 1)
 
         self.line_37 = QFrame(self.verticalLayoutWidget)
-        self.line_37.setObjectName(u"line_37")
+        self.line_37.setObjectName("line_37")
         self.line_37.setFrameShape(QFrame.VLine)
         self.line_37.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_37, 12, 1, 1, 1)
 
         self.label_dynamic_filename_4 = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_filename_4.setObjectName(u"label_dynamic_filename_4")
+        self.label_dynamic_filename_4.setObjectName("label_dynamic_filename_4")
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_filename_4, 11, 0, 1, 4)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_filename_4, 11, 0, 1, 4
+        )
 
         self.radio_button_primary_file_3 = QRadioButton(self.verticalLayoutWidget)
         self.button_group_primary_working_file = QButtonGroup(ManualWindow)
-        self.button_group_primary_working_file.setObjectName(u"button_group_primary_working_file")
-        self.button_group_primary_working_file.addButton(self.radio_button_primary_file_3)
-        self.radio_button_primary_file_3.setObjectName(u"radio_button_primary_file_3")
+        self.button_group_primary_working_file.setObjectName(
+            "button_group_primary_working_file"
+        )
+        self.button_group_primary_working_file.addButton(
+            self.radio_button_primary_file_3
+        )
+        self.radio_button_primary_file_3.setObjectName("radio_button_primary_file_3")
         self.radio_button_primary_file_3.setEnabled(True)
         sizePolicy2 = QSizePolicy(QSizePolicy.Minimum, QSizePolicy.Fixed)
         sizePolicy2.setHorizontalStretch(0)
         sizePolicy2.setVerticalStretch(0)
-        sizePolicy2.setHeightForWidth(self.radio_button_primary_file_3.sizePolicy().hasHeightForWidth())
+        sizePolicy2.setHeightForWidth(
+            self.radio_button_primary_file_3.sizePolicy().hasHeightForWidth()
+        )
         self.radio_button_primary_file_3.setSizePolicy(sizePolicy2)
         self.radio_button_primary_file_3.setMaximumSize(QSize(30, 16777215))
 
-        self.grid_layout_file_selector.addWidget(self.radio_button_primary_file_3, 9, 0, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.radio_button_primary_file_3, 9, 0, 1, 1
+        )
 
         self.line_36 = QFrame(self.verticalLayoutWidget)
-        self.line_36.setObjectName(u"line_36")
+        self.line_36.setObjectName("line_36")
         self.line_36.setFrameShape(QFrame.VLine)
         self.line_36.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_36, 9, 1, 1, 1)
 
         self.line_34 = QFrame(self.verticalLayoutWidget)
-        self.line_34.setObjectName(u"line_34")
+        self.line_34.setObjectName("line_34")
         self.line_34.setFrameShape(QFrame.VLine)
         self.line_34.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_34, 3, 1, 1, 1)
 
         self.radio_button_primary_file_4 = QRadioButton(self.verticalLayoutWidget)
-        self.button_group_primary_working_file.addButton(self.radio_button_primary_file_4)
-        self.radio_button_primary_file_4.setObjectName(u"radio_button_primary_file_4")
+        self.button_group_primary_working_file.addButton(
+            self.radio_button_primary_file_4
+        )
+        self.radio_button_primary_file_4.setObjectName("radio_button_primary_file_4")
         self.radio_button_primary_file_4.setEnabled(True)
-        sizePolicy2.setHeightForWidth(self.radio_button_primary_file_4.sizePolicy().hasHeightForWidth())
+        sizePolicy2.setHeightForWidth(
+            self.radio_button_primary_file_4.sizePolicy().hasHeightForWidth()
+        )
         self.radio_button_primary_file_4.setSizePolicy(sizePolicy2)
         self.radio_button_primary_file_4.setMaximumSize(QSize(30, 16777215))
 
-        self.grid_layout_file_selector.addWidget(self.radio_button_primary_file_4, 12, 0, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.radio_button_primary_file_4, 12, 0, 1, 1
+        )
 
         self.label_dynamic_target_2_pixel_location = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_target_2_pixel_location.setObjectName(u"label_dynamic_target_2_pixel_location")
+        self.label_dynamic_target_2_pixel_location.setObjectName(
+            "label_dynamic_target_2_pixel_location"
+        )
         self.label_dynamic_target_2_pixel_location.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_target_2_pixel_location, 6, 3, 1, 1)
-
-        self.push_button_relocate_target_location_3 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_relocate_target_location_3.setObjectName(u"push_button_relocate_target_location_3")
-
-        self.grid_layout_file_selector.addWidget(self.push_button_relocate_target_location_3, 9, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_target_2_pixel_location, 6, 3, 1, 1
+        )
+
+        self.push_button_relocate_target_location_3 = QPushButton(
+            self.verticalLayoutWidget
+        )
+        self.push_button_relocate_target_location_3.setObjectName(
+            "push_button_relocate_target_location_3"
+        )
+
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_relocate_target_location_3, 9, 4, 1, 1
+        )
 
         self.radio_button_primary_file_1 = QRadioButton(self.verticalLayoutWidget)
-        self.button_group_primary_working_file.addButton(self.radio_button_primary_file_1)
-        self.radio_button_primary_file_1.setObjectName(u"radio_button_primary_file_1")
-        sizePolicy2.setHeightForWidth(self.radio_button_primary_file_1.sizePolicy().hasHeightForWidth())
+        self.button_group_primary_working_file.addButton(
+            self.radio_button_primary_file_1
+        )
+        self.radio_button_primary_file_1.setObjectName("radio_button_primary_file_1")
+        sizePolicy2.setHeightForWidth(
+            self.radio_button_primary_file_1.sizePolicy().hasHeightForWidth()
+        )
         self.radio_button_primary_file_1.setSizePolicy(sizePolicy2)
         self.radio_button_primary_file_1.setMaximumSize(QSize(30, 16777215))
         self.radio_button_primary_file_1.setChecked(True)
 
-        self.grid_layout_file_selector.addWidget(self.radio_button_primary_file_1, 3, 0, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.radio_button_primary_file_1, 3, 0, 1, 1
+        )
 
         self.label_dynamic_target_3_pixel_location = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_target_3_pixel_location.setObjectName(u"label_dynamic_target_3_pixel_location")
+        self.label_dynamic_target_3_pixel_location.setObjectName(
+            "label_dynamic_target_3_pixel_location"
+        )
         self.label_dynamic_target_3_pixel_location.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_file_selector.addWidget(self.label_dynamic_target_3_pixel_location, 9, 3, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.label_dynamic_target_3_pixel_location, 9, 3, 1, 1
+        )
 
         self.radio_button_primary_file_2 = QRadioButton(self.verticalLayoutWidget)
-        self.button_group_primary_working_file.addButton(self.radio_button_primary_file_2)
-        self.radio_button_primary_file_2.setObjectName(u"radio_button_primary_file_2")
-        sizePolicy2.setHeightForWidth(self.radio_button_primary_file_2.sizePolicy().hasHeightForWidth())
+        self.button_group_primary_working_file.addButton(
+            self.radio_button_primary_file_2
+        )
+        self.radio_button_primary_file_2.setObjectName("radio_button_primary_file_2")
+        sizePolicy2.setHeightForWidth(
+            self.radio_button_primary_file_2.sizePolicy().hasHeightForWidth()
+        )
         self.radio_button_primary_file_2.setSizePolicy(sizePolicy2)
         self.radio_button_primary_file_2.setMaximumSize(QSize(30, 16777215))
 
-        self.grid_layout_file_selector.addWidget(self.radio_button_primary_file_2, 6, 0, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.radio_button_primary_file_2, 6, 0, 1, 1
+        )
 
         self.label_static_target_2_location = QLabel(self.verticalLayoutWidget)
-        self.label_static_target_2_location.setObjectName(u"label_static_target_2_location")
-
-        self.grid_layout_file_selector.addWidget(self.label_static_target_2_location, 6, 2, 1, 1)
-
-        self.push_button_relocate_target_location_2 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_relocate_target_location_2.setObjectName(u"push_button_relocate_target_location_2")
-
-        self.grid_layout_file_selector.addWidget(self.push_button_relocate_target_location_2, 6, 4, 1, 1)
+        self.label_static_target_2_location.setObjectName(
+            "label_static_target_2_location"
+        )
+
+        self.grid_layout_file_selector.addWidget(
+            self.label_static_target_2_location, 6, 2, 1, 1
+        )
+
+        self.push_button_relocate_target_location_2 = QPushButton(
+            self.verticalLayoutWidget
+        )
+        self.push_button_relocate_target_location_2.setObjectName(
+            "push_button_relocate_target_location_2"
+        )
+
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_relocate_target_location_2, 6, 4, 1, 1
+        )
 
         self.push_button_load_filename_1 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_load_filename_1.setObjectName(u"push_button_load_filename_1")
+        self.push_button_load_filename_1.setObjectName("push_button_load_filename_1")
         self.push_button_load_filename_1.setFont(font)
 
-        self.grid_layout_file_selector.addWidget(self.push_button_load_filename_1, 2, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_load_filename_1, 2, 4, 1, 1
+        )
 
         self.push_button_load_filename_2 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_load_filename_2.setObjectName(u"push_button_load_filename_2")
+        self.push_button_load_filename_2.setObjectName("push_button_load_filename_2")
 
-        self.grid_layout_file_selector.addWidget(self.push_button_load_filename_2, 5, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_load_filename_2, 5, 4, 1, 1
+        )
 
         self.label_static_target_1_location = QLabel(self.verticalLayoutWidget)
-        self.label_static_target_1_location.setObjectName(u"label_static_target_1_location")
+        self.label_static_target_1_location.setObjectName(
+            "label_static_target_1_location"
+        )
         self.label_static_target_1_location.setFont(font)
 
-        self.grid_layout_file_selector.addWidget(self.label_static_target_1_location, 3, 2, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.label_static_target_1_location, 3, 2, 1, 1
+        )
 
         self.push_button_load_filename_4 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_load_filename_4.setObjectName(u"push_button_load_filename_4")
-
-        self.grid_layout_file_selector.addWidget(self.push_button_load_filename_4, 11, 4, 1, 1)
+        self.push_button_load_filename_4.setObjectName("push_button_load_filename_4")
 
-        self.push_button_relocate_target_location_4 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_relocate_target_location_4.setObjectName(u"push_button_relocate_target_location_4")
-
-        self.grid_layout_file_selector.addWidget(self.push_button_relocate_target_location_4, 12, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_load_filename_4, 11, 4, 1, 1
+        )
+
+        self.push_button_relocate_target_location_4 = QPushButton(
+            self.verticalLayoutWidget
+        )
+        self.push_button_relocate_target_location_4.setObjectName(
+            "push_button_relocate_target_location_4"
+        )
+
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_relocate_target_location_4, 12, 4, 1, 1
+        )
 
         self.push_button_force_reset = QPushButton(self.verticalLayoutWidget)
-        self.push_button_force_reset.setObjectName(u"push_button_force_reset")
+        self.push_button_force_reset.setObjectName("push_button_force_reset")
 
-        self.grid_layout_file_selector.addWidget(self.push_button_force_reset, 0, 4, 1, 1)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_force_reset, 0, 4, 1, 1
+        )
 
         self.push_button_save_and_reset = QPushButton(self.verticalLayoutWidget)
-        self.push_button_save_and_reset.setObjectName(u"push_button_save_and_reset")
+        self.push_button_save_and_reset.setObjectName("push_button_save_and_reset")
         sizePolicy3 = QSizePolicy(QSizePolicy.MinimumExpanding, QSizePolicy.Fixed)
         sizePolicy3.setHorizontalStretch(0)
         sizePolicy3.setVerticalStretch(0)
-        sizePolicy3.setHeightForWidth(self.push_button_save_and_reset.sizePolicy().hasHeightForWidth())
+        sizePolicy3.setHeightForWidth(
+            self.push_button_save_and_reset.sizePolicy().hasHeightForWidth()
+        )
         self.push_button_save_and_reset.setSizePolicy(sizePolicy3)
 
-        self.grid_layout_file_selector.addWidget(self.push_button_save_and_reset, 0, 0, 1, 4)
+        self.grid_layout_file_selector.addWidget(
+            self.push_button_save_and_reset, 0, 0, 1, 4
+        )
 
         self.line_38 = QFrame(self.verticalLayoutWidget)
-        self.line_38.setObjectName(u"line_38")
+        self.line_38.setObjectName("line_38")
         self.line_38.setFrameShape(QFrame.HLine)
         self.line_38.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_38, 1, 0, 1, 5)
 
         self.line_2 = QFrame(self.verticalLayoutWidget)
-        self.line_2.setObjectName(u"line_2")
+        self.line_2.setObjectName("line_2")
         self.line_2.setFrameShape(QFrame.HLine)
         self.line_2.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_2, 4, 1, 1, 4)
 
         self.line_3 = QFrame(self.verticalLayoutWidget)
-        self.line_3.setObjectName(u"line_3")
+        self.line_3.setObjectName("line_3")
         self.line_3.setFrameShape(QFrame.HLine)
         self.line_3.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_3, 7, 1, 1, 4)
 
         self.line_4 = QFrame(self.verticalLayoutWidget)
-        self.line_4.setObjectName(u"line_4")
+        self.line_4.setObjectName("line_4")
         self.line_4.setFrameShape(QFrame.HLine)
         self.line_4.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_file_selector.addWidget(self.line_4, 10, 1, 1, 4)
 
-
         self.horizontal_layout_image_file.addLayout(self.grid_layout_file_selector)
 
-
         self.vertical_layout_window.addLayout(self.horizontal_layout_image_file)
 
         self.line_5 = QFrame(self.verticalLayoutWidget)
-        self.line_5.setObjectName(u"line_5")
+        self.line_5.setObjectName("line_5")
         self.line_5.setFrameShape(QFrame.HLine)
         self.line_5.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_window.addWidget(self.line_5)
 
         self.tab_widget_solutions = QTabWidget(self.verticalLayoutWidget)
-        self.tab_widget_solutions.setObjectName(u"tab_widget_solutions")
+        self.tab_widget_solutions.setObjectName("tab_widget_solutions")
         self.tab_widget_solutions.setEnabled(True)
         sizePolicy4 = QSizePolicy(QSizePolicy.Minimum, QSizePolicy.Expanding)
         sizePolicy4.setHorizontalStretch(0)
         sizePolicy4.setVerticalStretch(0)
-        sizePolicy4.setHeightForWidth(self.tab_widget_solutions.sizePolicy().hasHeightForWidth())
+        sizePolicy4.setHeightForWidth(
+            self.tab_widget_solutions.sizePolicy().hasHeightForWidth()
+        )
         self.tab_widget_solutions.setSizePolicy(sizePolicy4)
         self.tab_widget_solutions.setFont(font)
         self.tab_summary = QWidget()
-        self.tab_summary.setObjectName(u"tab_summary")
+        self.tab_summary.setObjectName("tab_summary")
         self.verticalLayoutWidget_2 = QWidget(self.tab_summary)
-        self.verticalLayoutWidget_2.setObjectName(u"verticalLayoutWidget_2")
+        self.verticalLayoutWidget_2.setObjectName("verticalLayoutWidget_2")
         self.verticalLayoutWidget_2.setGeometry(QRect(9, 9, 881, 291))
         self.vertical_layout_summary = QVBoxLayout(self.verticalLayoutWidget_2)
-        self.vertical_layout_summary.setObjectName(u"vertical_layout_summary")
+        self.vertical_layout_summary.setObjectName("vertical_layout_summary")
         self.vertical_layout_summary.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_target_name = QHBoxLayout()
-        self.horizontal_layout_target_name.setObjectName(u"horizontal_layout_target_name")
+        self.horizontal_layout_target_name.setObjectName(
+            "horizontal_layout_target_name"
+        )
         self.label_static_detected_target_name = QLabel(self.verticalLayoutWidget_2)
-        self.label_static_detected_target_name.setObjectName(u"label_static_detected_target_name")
-
-        self.horizontal_layout_target_name.addWidget(self.label_static_detected_target_name)
+        self.label_static_detected_target_name.setObjectName(
+            "label_static_detected_target_name"
+        )
+
+        self.horizontal_layout_target_name.addWidget(
+            self.label_static_detected_target_name
+        )
 
         self.line_edit_detected_target_name = QLineEdit(self.verticalLayoutWidget_2)
-        self.line_edit_detected_target_name.setObjectName(u"line_edit_detected_target_name")
-
-        self.horizontal_layout_target_name.addWidget(self.line_edit_detected_target_name)
+        self.line_edit_detected_target_name.setObjectName(
+            "line_edit_detected_target_name"
+        )
+
+        self.horizontal_layout_target_name.addWidget(
+            self.line_edit_detected_target_name
+        )
 
         self.push_button_change_target_name = QPushButton(self.verticalLayoutWidget_2)
-        self.push_button_change_target_name.setObjectName(u"push_button_change_target_name")
-
-        self.horizontal_layout_target_name.addWidget(self.push_button_change_target_name)
+        self.push_button_change_target_name.setObjectName(
+            "push_button_change_target_name"
+        )
+
+        self.horizontal_layout_target_name.addWidget(
+            self.push_button_change_target_name
+        )
 
         self.line_33 = QFrame(self.verticalLayoutWidget_2)
-        self.line_33.setObjectName(u"line_33")
+        self.line_33.setObjectName("line_33")
         self.line_33.setFrameShape(QFrame.VLine)
         self.line_33.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_target_name.addWidget(self.line_33)
 
         self.push_button_send_target_to_tcs = QPushButton(self.verticalLayoutWidget_2)
-        self.push_button_send_target_to_tcs.setObjectName(u"push_button_send_target_to_tcs")
-
-        self.horizontal_layout_target_name.addWidget(self.push_button_send_target_to_tcs)
-
+        self.push_button_send_target_to_tcs.setObjectName(
+            "push_button_send_target_to_tcs"
+        )
+
+        self.horizontal_layout_target_name.addWidget(
+            self.push_button_send_target_to_tcs
+        )
 
         self.vertical_layout_summary.addLayout(self.horizontal_layout_target_name)
 
         self.label = QLabel(self.verticalLayoutWidget_2)
-        self.label.setObjectName(u"label")
+        self.label.setObjectName("label")
 
         self.vertical_layout_summary.addWidget(self.label)
 
         self.tab_widget_solutions.addTab(self.tab_summary, "")
         self.tab_astrometry = QWidget()
-        self.tab_astrometry.setObjectName(u"tab_astrometry")
+        self.tab_astrometry.setObjectName("tab_astrometry")
         self.verticalLayoutWidget_3 = QWidget(self.tab_astrometry)
-        self.verticalLayoutWidget_3.setObjectName(u"verticalLayoutWidget_3")
+        self.verticalLayoutWidget_3.setObjectName("verticalLayoutWidget_3")
         self.verticalLayoutWidget_3.setGeometry(QRect(10, 10, 881, 291))
         self.vertical_layout_astrometry = QVBoxLayout(self.verticalLayoutWidget_3)
-        self.vertical_layout_astrometry.setObjectName(u"vertical_layout_astrometry")
+        self.vertical_layout_astrometry.setObjectName("vertical_layout_astrometry")
         self.vertical_layout_astrometry.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_astrometry_solve = QHBoxLayout()
-        self.horizontal_layout_astrometry_solve.setObjectName(u"horizontal_layout_astrometry_solve")
-        self.horizontal_layout_astrometry_solve.setSizeConstraint(QLayout.SetDefaultConstraint)
+        self.horizontal_layout_astrometry_solve.setObjectName(
+            "horizontal_layout_astrometry_solve"
+        )
+        self.horizontal_layout_astrometry_solve.setSizeConstraint(
+            QLayout.SetDefaultConstraint
+        )
         self.label_static_astrometry_engine = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_engine.setObjectName(u"label_static_astrometry_engine")
-
-        self.horizontal_layout_astrometry_solve.addWidget(self.label_static_astrometry_engine)
+        self.label_static_astrometry_engine.setObjectName(
+            "label_static_astrometry_engine"
+        )
+
+        self.horizontal_layout_astrometry_solve.addWidget(
+            self.label_static_astrometry_engine
+        )
 
         self.combo_box_astrometry_engine = QComboBox(self.verticalLayoutWidget_3)
         self.combo_box_astrometry_engine.addItem("")
         self.combo_box_astrometry_engine.addItem("")
-        self.combo_box_astrometry_engine.setObjectName(u"combo_box_astrometry_engine")
+        self.combo_box_astrometry_engine.setObjectName("combo_box_astrometry_engine")
 
-        self.horizontal_layout_astrometry_solve.addWidget(self.combo_box_astrometry_engine)
+        self.horizontal_layout_astrometry_solve.addWidget(
+            self.combo_box_astrometry_engine
+        )
 
         self.push_button_solve_astrometry = QPushButton(self.verticalLayoutWidget_3)
-        self.push_button_solve_astrometry.setObjectName(u"push_button_solve_astrometry")
-
-        self.horizontal_layout_astrometry_solve.addWidget(self.push_button_solve_astrometry)
+        self.push_button_solve_astrometry.setObjectName("push_button_solve_astrometry")
 
-
-        self.vertical_layout_astrometry.addLayout(self.horizontal_layout_astrometry_solve)
+        self.horizontal_layout_astrometry_solve.addWidget(
+            self.push_button_solve_astrometry
+        )
+
+        self.vertical_layout_astrometry.addLayout(
+            self.horizontal_layout_astrometry_solve
+        )
 
         self.line_6 = QFrame(self.verticalLayoutWidget_3)
-        self.line_6.setObjectName(u"line_6")
+        self.line_6.setObjectName("line_6")
         self.line_6.setFrameShape(QFrame.HLine)
         self.line_6.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_astrometry.addWidget(self.line_6)
 
         self.grid_layout_astrometry_results = QGridLayout()
-        self.grid_layout_astrometry_results.setObjectName(u"grid_layout_astrometry_results")
-        self.label_static_astrometry_results_center_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_center_dec.setObjectName(u"label_static_astrometry_results_center_dec")
+        self.grid_layout_astrometry_results.setObjectName(
+            "grid_layout_astrometry_results"
+        )
+        self.label_static_astrometry_results_center_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_center_dec.setObjectName(
+            "label_static_astrometry_results_center_dec"
+        )
         self.label_static_astrometry_results_center_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_center_dec, 1, 3, 1, 1)
-
-        self.label_dynamic_astrometry_file_3_target_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_3_target_ra.setObjectName(u"label_dynamic_astrometry_file_3_target_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_center_dec, 1, 3, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_3_target_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_3_target_ra.setObjectName(
+            "label_dynamic_astrometry_file_3_target_ra"
+        )
         self.label_dynamic_astrometry_file_3_target_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_3_target_ra, 5, 5, 1, 1)
-
-        self.label_static_astrometry_results_center_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_center_ra.setObjectName(u"label_static_astrometry_results_center_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_3_target_ra, 5, 5, 1, 1
+        )
+
+        self.label_static_astrometry_results_center_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_center_ra.setObjectName(
+            "label_static_astrometry_results_center_ra"
+        )
         self.label_static_astrometry_results_center_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_center_ra, 1, 2, 1, 1)
-
-        self.label_dynamic_astrometry_file_4_center_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_4_center_ra.setObjectName(u"label_dynamic_astrometry_file_4_center_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_center_ra, 1, 2, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_4_center_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_4_center_ra.setObjectName(
+            "label_dynamic_astrometry_file_4_center_ra"
+        )
         self.label_dynamic_astrometry_file_4_center_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_4_center_ra, 6, 2, 1, 1)
-
-        self.label_static_astrometry_results_center = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_center.setObjectName(u"label_static_astrometry_results_center")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_4_center_ra, 6, 2, 1, 1
+        )
+
+        self.label_static_astrometry_results_center = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_center.setObjectName(
+            "label_static_astrometry_results_center"
+        )
         self.label_static_astrometry_results_center.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_center, 0, 2, 1, 2)
-
-        self.label_dynamic_astrometry_file_4_target_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_4_target_ra.setObjectName(u"label_dynamic_astrometry_file_4_target_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_center, 0, 2, 1, 2
+        )
+
+        self.label_dynamic_astrometry_file_4_target_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_4_target_ra.setObjectName(
+            "label_dynamic_astrometry_file_4_target_ra"
+        )
         self.label_dynamic_astrometry_file_4_target_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_4_target_ra, 6, 5, 1, 1)
-
-        self.label_dynamic_astrometry_file_3_target_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_3_target_dec.setObjectName(u"label_dynamic_astrometry_file_3_target_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_4_target_ra, 6, 5, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_3_target_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_3_target_dec.setObjectName(
+            "label_dynamic_astrometry_file_3_target_dec"
+        )
         self.label_dynamic_astrometry_file_3_target_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_3_target_dec, 5, 6, 1, 1)
-
-        self.label_dynamic_astrometry_file_4_target_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_4_target_dec.setObjectName(u"label_dynamic_astrometry_file_4_target_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_3_target_dec, 5, 6, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_4_target_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_4_target_dec.setObjectName(
+            "label_dynamic_astrometry_file_4_target_dec"
+        )
         self.label_dynamic_astrometry_file_4_target_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_4_target_dec, 6, 6, 1, 1)
-
-        self.label_dynamic_astrometry_file_2_target_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_2_target_ra.setObjectName(u"label_dynamic_astrometry_file_2_target_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_4_target_dec, 6, 6, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_2_target_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_2_target_ra.setObjectName(
+            "label_dynamic_astrometry_file_2_target_ra"
+        )
         self.label_dynamic_astrometry_file_2_target_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_2_target_ra, 4, 5, 1, 1)
-
-        self.label_dynamic_astrometry_file_3_center_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_3_center_dec.setObjectName(u"label_dynamic_astrometry_file_3_center_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_2_target_ra, 4, 5, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_3_center_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_3_center_dec.setObjectName(
+            "label_dynamic_astrometry_file_3_center_dec"
+        )
         self.label_dynamic_astrometry_file_3_center_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_3_center_dec, 5, 3, 1, 1)
-
-        self.label_dynamic_astrometry_file_4_center_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_4_center_dec.setObjectName(u"label_dynamic_astrometry_file_4_center_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_3_center_dec, 5, 3, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_4_center_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_4_center_dec.setObjectName(
+            "label_dynamic_astrometry_file_4_center_dec"
+        )
         self.label_dynamic_astrometry_file_4_center_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_4_center_dec, 6, 3, 1, 1)
-
-        self.label_dynamic_astrometry_file_2_center_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_2_center_dec.setObjectName(u"label_dynamic_astrometry_file_2_center_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_4_center_dec, 6, 3, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_2_center_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_2_center_dec.setObjectName(
+            "label_dynamic_astrometry_file_2_center_dec"
+        )
         self.label_dynamic_astrometry_file_2_center_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_2_center_dec, 4, 3, 1, 1)
-
-        self.label_static_astrometry_results_target_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_target_dec.setObjectName(u"label_static_astrometry_results_target_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_2_center_dec, 4, 3, 1, 1
+        )
+
+        self.label_static_astrometry_results_target_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_target_dec.setObjectName(
+            "label_static_astrometry_results_target_dec"
+        )
         self.label_static_astrometry_results_target_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_target_dec, 1, 6, 1, 1)
-
-        self.label_static_astrometry_results_target_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_target_ra.setObjectName(u"label_static_astrometry_results_target_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_target_dec, 1, 6, 1, 1
+        )
+
+        self.label_static_astrometry_results_target_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_target_ra.setObjectName(
+            "label_static_astrometry_results_target_ra"
+        )
         self.label_static_astrometry_results_target_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_target_ra, 1, 5, 1, 1)
-
-        self.label_dynamic_astrometry_file_2_target_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_2_target_dec.setObjectName(u"label_dynamic_astrometry_file_2_target_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_target_ra, 1, 5, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_2_target_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_2_target_dec.setObjectName(
+            "label_dynamic_astrometry_file_2_target_dec"
+        )
         self.label_dynamic_astrometry_file_2_target_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_2_target_dec, 4, 6, 1, 1)
-
-        self.label_dynamic_astrometry_file_3_center_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_3_center_ra.setObjectName(u"label_dynamic_astrometry_file_3_center_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_2_target_dec, 4, 6, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_3_center_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_3_center_ra.setObjectName(
+            "label_dynamic_astrometry_file_3_center_ra"
+        )
         self.label_dynamic_astrometry_file_3_center_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_3_center_ra, 5, 2, 1, 1)
-
-        self.label_dynamic_astrometry_file_2_center_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_2_center_ra.setObjectName(u"label_dynamic_astrometry_file_2_center_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_3_center_ra, 5, 2, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_2_center_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_2_center_ra.setObjectName(
+            "label_dynamic_astrometry_file_2_center_ra"
+        )
         self.label_dynamic_astrometry_file_2_center_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_2_center_ra, 4, 2, 1, 1)
-
-        self.label_static_astrometry_results_target = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_target.setObjectName(u"label_static_astrometry_results_target")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_2_center_ra, 4, 2, 1, 1
+        )
+
+        self.label_static_astrometry_results_target = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_target.setObjectName(
+            "label_static_astrometry_results_target"
+        )
         self.label_static_astrometry_results_target.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_target, 0, 5, 1, 2)
-
-        self.label_dynamic_astrometry_file_1_center_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_1_center_dec.setObjectName(u"label_dynamic_astrometry_file_1_center_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_target, 0, 5, 1, 2
+        )
+
+        self.label_dynamic_astrometry_file_1_center_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_1_center_dec.setObjectName(
+            "label_dynamic_astrometry_file_1_center_dec"
+        )
         self.label_dynamic_astrometry_file_1_center_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_1_center_dec, 3, 3, 1, 1)
-
-        self.label_static_astrometry_results_file_1 = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_file_1.setObjectName(u"label_static_astrometry_results_file_1")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_1_center_dec, 3, 3, 1, 1
+        )
+
+        self.label_static_astrometry_results_file_1 = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_file_1.setObjectName(
+            "label_static_astrometry_results_file_1"
+        )
         self.label_static_astrometry_results_file_1.setMinimumSize(QSize(50, 0))
         self.label_static_astrometry_results_file_1.setMaximumSize(QSize(50, 16777215))
         self.label_static_astrometry_results_file_1.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_file_1, 3, 0, 1, 1)
-
-        self.label_dynamic_astrometry_file_1_target_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_1_target_dec.setObjectName(u"label_dynamic_astrometry_file_1_target_dec")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_file_1, 3, 0, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_1_target_dec = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_1_target_dec.setObjectName(
+            "label_dynamic_astrometry_file_1_target_dec"
+        )
         self.label_dynamic_astrometry_file_1_target_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_1_target_dec, 3, 6, 1, 1)
-
-        self.label_dynamic_astrometry_file_1_target_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_1_target_ra.setObjectName(u"label_dynamic_astrometry_file_1_target_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_1_target_dec, 3, 6, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_1_target_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_1_target_ra.setObjectName(
+            "label_dynamic_astrometry_file_1_target_ra"
+        )
         self.label_dynamic_astrometry_file_1_target_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_1_target_ra, 3, 5, 1, 1)
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_1_target_ra, 3, 5, 1, 1
+        )
 
         self.label_static_astrometry_results_file = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_file.setObjectName(u"label_static_astrometry_results_file")
+        self.label_static_astrometry_results_file.setObjectName(
+            "label_static_astrometry_results_file"
+        )
         self.label_static_astrometry_results_file.setMinimumSize(QSize(50, 0))
         self.label_static_astrometry_results_file.setMaximumSize(QSize(50, 16777215))
         self.label_static_astrometry_results_file.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_file, 0, 0, 1, 1)
-
-        self.label_dynamic_astrometry_file_1_center_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_dynamic_astrometry_file_1_center_ra.setObjectName(u"label_dynamic_astrometry_file_1_center_ra")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_file, 0, 0, 1, 1
+        )
+
+        self.label_dynamic_astrometry_file_1_center_ra = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_dynamic_astrometry_file_1_center_ra.setObjectName(
+            "label_dynamic_astrometry_file_1_center_ra"
+        )
         self.label_dynamic_astrometry_file_1_center_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_dynamic_astrometry_file_1_center_ra, 3, 2, 1, 1)
-
-        self.label_static_astrometry_results_file_3 = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_file_3.setObjectName(u"label_static_astrometry_results_file_3")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_dynamic_astrometry_file_1_center_ra, 3, 2, 1, 1
+        )
+
+        self.label_static_astrometry_results_file_3 = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_file_3.setObjectName(
+            "label_static_astrometry_results_file_3"
+        )
         self.label_static_astrometry_results_file_3.setMinimumSize(QSize(50, 0))
         self.label_static_astrometry_results_file_3.setMaximumSize(QSize(50, 16777215))
         self.label_static_astrometry_results_file_3.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_file_3, 5, 0, 1, 1)
-
-        self.label_static_astrometry_results_file_2 = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_file_2.setObjectName(u"label_static_astrometry_results_file_2")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_file_3, 5, 0, 1, 1
+        )
+
+        self.label_static_astrometry_results_file_2 = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_file_2.setObjectName(
+            "label_static_astrometry_results_file_2"
+        )
         self.label_static_astrometry_results_file_2.setMinimumSize(QSize(50, 0))
         self.label_static_astrometry_results_file_2.setMaximumSize(QSize(50, 16777215))
         self.label_static_astrometry_results_file_2.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_file_2, 4, 0, 1, 1)
-
-        self.label_static_astrometry_results_file_4 = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_results_file_4.setObjectName(u"label_static_astrometry_results_file_4")
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_file_2, 4, 0, 1, 1
+        )
+
+        self.label_static_astrometry_results_file_4 = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_results_file_4.setObjectName(
+            "label_static_astrometry_results_file_4"
+        )
         self.label_static_astrometry_results_file_4.setMinimumSize(QSize(50, 0))
         self.label_static_astrometry_results_file_4.setMaximumSize(QSize(50, 16777215))
         self.label_static_astrometry_results_file_4.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_results.addWidget(self.label_static_astrometry_results_file_4, 6, 0, 1, 1)
+        self.grid_layout_astrometry_results.addWidget(
+            self.label_static_astrometry_results_file_4, 6, 0, 1, 1
+        )
 
         self.line_23 = QFrame(self.verticalLayoutWidget_3)
-        self.line_23.setObjectName(u"line_23")
+        self.line_23.setObjectName("line_23")
         self.line_23.setFrameShape(QFrame.HLine)
         self.line_23.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_astrometry_results.addWidget(self.line_23, 2, 2, 1, 2)
 
         self.line_26 = QFrame(self.verticalLayoutWidget_3)
-        self.line_26.setObjectName(u"line_26")
+        self.line_26.setObjectName("line_26")
         self.line_26.setFrameShape(QFrame.HLine)
         self.line_26.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_astrometry_results.addWidget(self.line_26, 2, 5, 1, 2)
 
         self.line_27 = QFrame(self.verticalLayoutWidget_3)
-        self.line_27.setObjectName(u"line_27")
+        self.line_27.setObjectName("line_27")
         self.line_27.setFrameShape(QFrame.HLine)
         self.line_27.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_astrometry_results.addWidget(self.line_27, 2, 0, 1, 1)
 
         self.line_7 = QFrame(self.verticalLayoutWidget_3)
-        self.line_7.setObjectName(u"line_7")
+        self.line_7.setObjectName("line_7")
         self.line_7.setFrameShape(QFrame.VLine)
         self.line_7.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_astrometry_results.addWidget(self.line_7, 0, 1, 7, 1)
 
         self.line_8 = QFrame(self.verticalLayoutWidget_3)
-        self.line_8.setObjectName(u"line_8")
+        self.line_8.setObjectName("line_8")
         self.line_8.setFrameShape(QFrame.VLine)
         self.line_8.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_astrometry_results.addWidget(self.line_8, 0, 4, 7, 1)
 
-
         self.vertical_layout_astrometry.addLayout(self.grid_layout_astrometry_results)
 
         self.line_9 = QFrame(self.verticalLayoutWidget_3)
-        self.line_9.setObjectName(u"line_9")
+        self.line_9.setObjectName("line_9")
         self.line_9.setFrameShape(QFrame.HLine)
         self.line_9.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_astrometry.addWidget(self.line_9)
 
         self.grid_layout_astrometry_custom = QGridLayout()
-        self.grid_layout_astrometry_custom.setObjectName(u"grid_layout_astrometry_custom")
-        self.line_edit_astrometry_custom_pixel_y = QLineEdit(self.verticalLayoutWidget_3)
-        self.line_edit_astrometry_custom_pixel_y.setObjectName(u"line_edit_astrometry_custom_pixel_y")
-
-        self.grid_layout_astrometry_custom.addWidget(self.line_edit_astrometry_custom_pixel_y, 1, 2, 1, 1)
+        self.grid_layout_astrometry_custom.setObjectName(
+            "grid_layout_astrometry_custom"
+        )
+        self.line_edit_astrometry_custom_pixel_y = QLineEdit(
+            self.verticalLayoutWidget_3
+        )
+        self.line_edit_astrometry_custom_pixel_y.setObjectName(
+            "line_edit_astrometry_custom_pixel_y"
+        )
+
+        self.grid_layout_astrometry_custom.addWidget(
+            self.line_edit_astrometry_custom_pixel_y, 1, 2, 1, 1
+        )
 
         self.line_edit_astrometry_custom_dec = QLineEdit(self.verticalLayoutWidget_3)
-        self.line_edit_astrometry_custom_dec.setObjectName(u"line_edit_astrometry_custom_dec")
-
-        self.grid_layout_astrometry_custom.addWidget(self.line_edit_astrometry_custom_dec, 1, 4, 1, 1)
+        self.line_edit_astrometry_custom_dec.setObjectName(
+            "line_edit_astrometry_custom_dec"
+        )
+
+        self.grid_layout_astrometry_custom.addWidget(
+            self.line_edit_astrometry_custom_dec, 1, 4, 1, 1
+        )
 
         self.line_edit_astrometry_custom_ra = QLineEdit(self.verticalLayoutWidget_3)
-        self.line_edit_astrometry_custom_ra.setObjectName(u"line_edit_astrometry_custom_ra")
-
-        self.grid_layout_astrometry_custom.addWidget(self.line_edit_astrometry_custom_ra, 1, 3, 1, 1)
-
-        self.line_edit_astrometry_custom_pixel_x = QLineEdit(self.verticalLayoutWidget_3)
-        self.line_edit_astrometry_custom_pixel_x.setObjectName(u"line_edit_astrometry_custom_pixel_x")
-
-        self.grid_layout_astrometry_custom.addWidget(self.line_edit_astrometry_custom_pixel_x, 1, 1, 1, 1)
-
-        self.label_static_astrometry_custom_pixel_x = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_custom_pixel_x.setObjectName(u"label_static_astrometry_custom_pixel_x")
+        self.line_edit_astrometry_custom_ra.setObjectName(
+            "line_edit_astrometry_custom_ra"
+        )
+
+        self.grid_layout_astrometry_custom.addWidget(
+            self.line_edit_astrometry_custom_ra, 1, 3, 1, 1
+        )
+
+        self.line_edit_astrometry_custom_pixel_x = QLineEdit(
+            self.verticalLayoutWidget_3
+        )
+        self.line_edit_astrometry_custom_pixel_x.setObjectName(
+            "line_edit_astrometry_custom_pixel_x"
+        )
+
+        self.grid_layout_astrometry_custom.addWidget(
+            self.line_edit_astrometry_custom_pixel_x, 1, 1, 1, 1
+        )
+
+        self.label_static_astrometry_custom_pixel_x = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_custom_pixel_x.setObjectName(
+            "label_static_astrometry_custom_pixel_x"
+        )
         self.label_static_astrometry_custom_pixel_x.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_custom.addWidget(self.label_static_astrometry_custom_pixel_x, 0, 1, 1, 1)
-
-        self.label_static_astrometry_coordinate_solve = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_coordinate_solve.setObjectName(u"label_static_astrometry_coordinate_solve")
-
-        self.grid_layout_astrometry_custom.addWidget(self.label_static_astrometry_coordinate_solve, 0, 0, 1, 1)
-
-        self.label_static_astrometry_custom_pixel_y = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_custom_pixel_y.setObjectName(u"label_static_astrometry_custom_pixel_y")
+        self.grid_layout_astrometry_custom.addWidget(
+            self.label_static_astrometry_custom_pixel_x, 0, 1, 1, 1
+        )
+
+        self.label_static_astrometry_coordinate_solve = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_coordinate_solve.setObjectName(
+            "label_static_astrometry_coordinate_solve"
+        )
+
+        self.grid_layout_astrometry_custom.addWidget(
+            self.label_static_astrometry_coordinate_solve, 0, 0, 1, 1
+        )
+
+        self.label_static_astrometry_custom_pixel_y = QLabel(
+            self.verticalLayoutWidget_3
+        )
+        self.label_static_astrometry_custom_pixel_y.setObjectName(
+            "label_static_astrometry_custom_pixel_y"
+        )
         self.label_static_astrometry_custom_pixel_y.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_custom.addWidget(self.label_static_astrometry_custom_pixel_y, 0, 2, 1, 1)
+        self.grid_layout_astrometry_custom.addWidget(
+            self.label_static_astrometry_custom_pixel_y, 0, 2, 1, 1
+        )
 
         self.label_static_astrometry_custom_ra = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_custom_ra.setObjectName(u"label_static_astrometry_custom_ra")
+        self.label_static_astrometry_custom_ra.setObjectName(
+            "label_static_astrometry_custom_ra"
+        )
         self.label_static_astrometry_custom_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_custom.addWidget(self.label_static_astrometry_custom_ra, 0, 3, 1, 1)
+        self.grid_layout_astrometry_custom.addWidget(
+            self.label_static_astrometry_custom_ra, 0, 3, 1, 1
+        )
 
         self.label_static_astrometry_custom_dec = QLabel(self.verticalLayoutWidget_3)
-        self.label_static_astrometry_custom_dec.setObjectName(u"label_static_astrometry_custom_dec")
+        self.label_static_astrometry_custom_dec.setObjectName(
+            "label_static_astrometry_custom_dec"
+        )
         self.label_static_astrometry_custom_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_astrometry_custom.addWidget(self.label_static_astrometry_custom_dec, 0, 4, 1, 1)
-
-        self.push_button_astrometry_custom_solve = QPushButton(self.verticalLayoutWidget_3)
-        self.push_button_astrometry_custom_solve.setObjectName(u"push_button_astrometry_custom_solve")
-
-        self.grid_layout_astrometry_custom.addWidget(self.push_button_astrometry_custom_solve, 1, 0, 1, 1)
-
+        self.grid_layout_astrometry_custom.addWidget(
+            self.label_static_astrometry_custom_dec, 0, 4, 1, 1
+        )
+
+        self.push_button_astrometry_custom_solve = QPushButton(
+            self.verticalLayoutWidget_3
+        )
+        self.push_button_astrometry_custom_solve.setObjectName(
+            "push_button_astrometry_custom_solve"
+        )
+
+        self.grid_layout_astrometry_custom.addWidget(
+            self.push_button_astrometry_custom_solve, 1, 0, 1, 1
+        )
 
         self.vertical_layout_astrometry.addLayout(self.grid_layout_astrometry_custom)
 
         self.tab_widget_solutions.addTab(self.tab_astrometry, "")
         self.tab_photometry = QWidget()
-        self.tab_photometry.setObjectName(u"tab_photometry")
+        self.tab_photometry.setObjectName("tab_photometry")
         self.verticalLayoutWidget_4 = QWidget(self.tab_photometry)
-        self.verticalLayoutWidget_4.setObjectName(u"verticalLayoutWidget_4")
+        self.verticalLayoutWidget_4.setObjectName("verticalLayoutWidget_4")
         self.verticalLayoutWidget_4.setGeometry(QRect(10, 10, 881, 291))
         self.vertical_layout_photometry = QVBoxLayout(self.verticalLayoutWidget_4)
-        self.vertical_layout_photometry.setObjectName(u"vertical_layout_photometry")
+        self.vertical_layout_photometry.setObjectName("vertical_layout_photometry")
         self.vertical_layout_photometry.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_photometry_solve = QHBoxLayout()
-        self.horizontal_layout_photometry_solve.setObjectName(u"horizontal_layout_photometry_solve")
+        self.horizontal_layout_photometry_solve.setObjectName(
+            "horizontal_layout_photometry_solve"
+        )
         self.label_static_photometry_engine = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_engine.setObjectName(u"label_static_photometry_engine")
-
-        self.horizontal_layout_photometry_solve.addWidget(self.label_static_photometry_engine)
+        self.label_static_photometry_engine.setObjectName(
+            "label_static_photometry_engine"
+        )
+
+        self.horizontal_layout_photometry_solve.addWidget(
+            self.label_static_photometry_engine
+        )
 
         self.combo_box_photometry_engine = QComboBox(self.verticalLayoutWidget_4)
         self.combo_box_photometry_engine.addItem("")
-        self.combo_box_photometry_engine.setObjectName(u"combo_box_photometry_engine")
+        self.combo_box_photometry_engine.setObjectName("combo_box_photometry_engine")
 
-        self.horizontal_layout_photometry_solve.addWidget(self.combo_box_photometry_engine)
+        self.horizontal_layout_photometry_solve.addWidget(
+            self.combo_box_photometry_engine
+        )
 
         self.push_button_solve_photometry = QPushButton(self.verticalLayoutWidget_4)
-        self.push_button_solve_photometry.setObjectName(u"push_button_solve_photometry")
-
-        self.horizontal_layout_photometry_solve.addWidget(self.push_button_solve_photometry)
+        self.push_button_solve_photometry.setObjectName("push_button_solve_photometry")
 
-
-        self.vertical_layout_photometry.addLayout(self.horizontal_layout_photometry_solve)
+        self.horizontal_layout_photometry_solve.addWidget(
+            self.push_button_solve_photometry
+        )
+
+        self.vertical_layout_photometry.addLayout(
+            self.horizontal_layout_photometry_solve
+        )
 
         self.line_10 = QFrame(self.verticalLayoutWidget_4)
-        self.line_10.setObjectName(u"line_10")
+        self.line_10.setObjectName("line_10")
         self.line_10.setFrameShape(QFrame.HLine)
         self.line_10.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_photometry.addWidget(self.line_10)
 
         self.grid_layout_photometry_results = QGridLayout()
-        self.grid_layout_photometry_results.setObjectName(u"grid_layout_photometry_results")
-        self.label_static_photometry_results_file_1 = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_1.setObjectName(u"label_static_photometry_results_file_1")
+        self.grid_layout_photometry_results.setObjectName(
+            "grid_layout_photometry_results"
+        )
+        self.label_static_photometry_results_file_1 = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_1.setObjectName(
+            "label_static_photometry_results_file_1"
+        )
         self.label_static_photometry_results_file_1.setMinimumSize(QSize(50, 0))
         self.label_static_photometry_results_file_1.setMaximumSize(QSize(50, 16777215))
         self.label_static_photometry_results_file_1.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_1, 2, 0, 1, 1)
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_1, 2, 0, 1, 1
+        )
 
         self.label_static_photometry_results_file = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file.setObjectName(u"label_static_photometry_results_file")
+        self.label_static_photometry_results_file.setObjectName(
+            "label_static_photometry_results_file"
+        )
         self.label_static_photometry_results_file.setMinimumSize(QSize(50, 0))
         self.label_static_photometry_results_file.setMaximumSize(QSize(50, 16777215))
         self.label_static_photometry_results_file.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file, 0, 0, 1, 1)
-
-        self.label_static_photometry_results_file_2 = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_2.setObjectName(u"label_static_photometry_results_file_2")
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file, 0, 0, 1, 1
+        )
+
+        self.label_static_photometry_results_file_2 = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_2.setObjectName(
+            "label_static_photometry_results_file_2"
+        )
         self.label_static_photometry_results_file_2.setMinimumSize(QSize(50, 0))
         self.label_static_photometry_results_file_2.setMaximumSize(QSize(50, 16777215))
         self.label_static_photometry_results_file_2.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_2, 3, 0, 1, 1)
-
-        self.label_static_photometry_results_file_4 = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_4.setObjectName(u"label_static_photometry_results_file_4")
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_2, 3, 0, 1, 1
+        )
+
+        self.label_static_photometry_results_file_4 = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_4.setObjectName(
+            "label_static_photometry_results_file_4"
+        )
         self.label_static_photometry_results_file_4.setMinimumSize(QSize(50, 0))
         self.label_static_photometry_results_file_4.setMaximumSize(QSize(50, 16777215))
         self.label_static_photometry_results_file_4.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_4, 5, 0, 1, 1)
-
-        self.label_static_photometry_results_file_3 = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_3.setObjectName(u"label_static_photometry_results_file_3")
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_4, 5, 0, 1, 1
+        )
+
+        self.label_static_photometry_results_file_3 = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_3.setObjectName(
+            "label_static_photometry_results_file_3"
+        )
         self.label_static_photometry_results_file_3.setMinimumSize(QSize(50, 0))
         self.label_static_photometry_results_file_3.setMaximumSize(QSize(50, 16777215))
         self.label_static_photometry_results_file_3.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_3, 4, 0, 1, 1)
-
-        self.label_static_photometry_results_zero_point = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_zero_point.setObjectName(u"label_static_photometry_results_zero_point")
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_3, 4, 0, 1, 1
+        )
+
+        self.label_static_photometry_results_zero_point = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_zero_point.setObjectName(
+            "label_static_photometry_results_zero_point"
+        )
         self.label_static_photometry_results_zero_point.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_zero_point, 0, 3, 1, 1)
-
-        self.label_static_photometry_results_file_2_filter_name = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_2_filter_name.setObjectName(u"label_static_photometry_results_file_2_filter_name")
-        self.label_static_photometry_results_file_2_filter_name.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_2_filter_name, 3, 2, 1, 1)
-
-        self.label_static_photometry_results_aperture_magnitude = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_aperture_magnitude.setObjectName(u"label_static_photometry_results_aperture_magnitude")
-        self.label_static_photometry_results_aperture_magnitude.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_aperture_magnitude, 0, 4, 1, 1)
-
-        self.label_static_photometry_results_filter_name = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_filter_name.setObjectName(u"label_static_photometry_results_filter_name")
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_zero_point, 0, 3, 1, 1
+        )
+
+        self.label_static_photometry_results_file_2_filter_name = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_2_filter_name.setObjectName(
+            "label_static_photometry_results_file_2_filter_name"
+        )
+        self.label_static_photometry_results_file_2_filter_name.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_2_filter_name, 3, 2, 1, 1
+        )
+
+        self.label_static_photometry_results_aperture_magnitude = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_aperture_magnitude.setObjectName(
+            "label_static_photometry_results_aperture_magnitude"
+        )
+        self.label_static_photometry_results_aperture_magnitude.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_aperture_magnitude, 0, 4, 1, 1
+        )
+
+        self.label_static_photometry_results_filter_name = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_filter_name.setObjectName(
+            "label_static_photometry_results_filter_name"
+        )
         self.label_static_photometry_results_filter_name.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_filter_name, 0, 2, 1, 1)
-
-        self.label_static_photometry_results_file_4_filter_name = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_4_filter_name.setObjectName(u"label_static_photometry_results_file_4_filter_name")
-        self.label_static_photometry_results_file_4_filter_name.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_4_filter_name, 5, 2, 1, 1)
-
-        self.label_static_photometry_results_file_1_filter_name = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_1_filter_name.setObjectName(u"label_static_photometry_results_file_1_filter_name")
-        self.label_static_photometry_results_file_1_filter_name.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_1_filter_name, 2, 2, 1, 1)
-
-        self.label_static_photometry_results_file_3_filter_name = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_3_filter_name.setObjectName(u"label_static_photometry_results_file_3_filter_name")
-        self.label_static_photometry_results_file_3_filter_name.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_3_filter_name, 4, 2, 1, 1)
-
-        self.label_static_photometry_results_file_1_zero_point = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_1_zero_point.setObjectName(u"label_static_photometry_results_file_1_zero_point")
-        self.label_static_photometry_results_file_1_zero_point.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_1_zero_point, 2, 3, 1, 1)
-
-        self.label_static_photometry_results_file_4_zero_point = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_4_zero_point.setObjectName(u"label_static_photometry_results_file_4_zero_point")
-        self.label_static_photometry_results_file_4_zero_point.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_4_zero_point, 5, 3, 1, 1)
-
-        self.label_static_photometry_results_file_2_zero_point = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_2_zero_point.setObjectName(u"label_static_photometry_results_file_2_zero_point")
-        self.label_static_photometry_results_file_2_zero_point.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_2_zero_point, 3, 3, 1, 1)
-
-        self.label_static_photometry_results_file_3_zero_point = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_3_zero_point.setObjectName(u"label_static_photometry_results_file_3_zero_point")
-        self.label_static_photometry_results_file_3_zero_point.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_3_zero_point, 4, 3, 1, 1)
-
-        self.label_static_photometry_results_file_1_magnitude = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_1_magnitude.setObjectName(u"label_static_photometry_results_file_1_magnitude")
-        self.label_static_photometry_results_file_1_magnitude.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_1_magnitude, 2, 4, 1, 1)
-
-        self.label_static_photometry_results_file_2_magnitude = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_2_magnitude.setObjectName(u"label_static_photometry_results_file_2_magnitude")
-        self.label_static_photometry_results_file_2_magnitude.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_2_magnitude, 3, 4, 1, 1)
-
-        self.label_static_photometry_results_file_3_magnitude = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_3_magnitude.setObjectName(u"label_static_photometry_results_file_3_magnitude")
-        self.label_static_photometry_results_file_3_magnitude.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_3_magnitude, 4, 4, 1, 1)
-
-        self.label_static_photometry_results_file_4_magnitude = QLabel(self.verticalLayoutWidget_4)
-        self.label_static_photometry_results_file_4_magnitude.setObjectName(u"label_static_photometry_results_file_4_magnitude")
-        self.label_static_photometry_results_file_4_magnitude.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_photometry_results.addWidget(self.label_static_photometry_results_file_4_magnitude, 5, 4, 1, 1)
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_filter_name, 0, 2, 1, 1
+        )
+
+        self.label_static_photometry_results_file_4_filter_name = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_4_filter_name.setObjectName(
+            "label_static_photometry_results_file_4_filter_name"
+        )
+        self.label_static_photometry_results_file_4_filter_name.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_4_filter_name, 5, 2, 1, 1
+        )
+
+        self.label_static_photometry_results_file_1_filter_name = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_1_filter_name.setObjectName(
+            "label_static_photometry_results_file_1_filter_name"
+        )
+        self.label_static_photometry_results_file_1_filter_name.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_1_filter_name, 2, 2, 1, 1
+        )
+
+        self.label_static_photometry_results_file_3_filter_name = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_3_filter_name.setObjectName(
+            "label_static_photometry_results_file_3_filter_name"
+        )
+        self.label_static_photometry_results_file_3_filter_name.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_3_filter_name, 4, 2, 1, 1
+        )
+
+        self.label_static_photometry_results_file_1_zero_point = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_1_zero_point.setObjectName(
+            "label_static_photometry_results_file_1_zero_point"
+        )
+        self.label_static_photometry_results_file_1_zero_point.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_1_zero_point, 2, 3, 1, 1
+        )
+
+        self.label_static_photometry_results_file_4_zero_point = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_4_zero_point.setObjectName(
+            "label_static_photometry_results_file_4_zero_point"
+        )
+        self.label_static_photometry_results_file_4_zero_point.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_4_zero_point, 5, 3, 1, 1
+        )
+
+        self.label_static_photometry_results_file_2_zero_point = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_2_zero_point.setObjectName(
+            "label_static_photometry_results_file_2_zero_point"
+        )
+        self.label_static_photometry_results_file_2_zero_point.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_2_zero_point, 3, 3, 1, 1
+        )
+
+        self.label_static_photometry_results_file_3_zero_point = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_3_zero_point.setObjectName(
+            "label_static_photometry_results_file_3_zero_point"
+        )
+        self.label_static_photometry_results_file_3_zero_point.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_3_zero_point, 4, 3, 1, 1
+        )
+
+        self.label_static_photometry_results_file_1_magnitude = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_1_magnitude.setObjectName(
+            "label_static_photometry_results_file_1_magnitude"
+        )
+        self.label_static_photometry_results_file_1_magnitude.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_1_magnitude, 2, 4, 1, 1
+        )
+
+        self.label_static_photometry_results_file_2_magnitude = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_2_magnitude.setObjectName(
+            "label_static_photometry_results_file_2_magnitude"
+        )
+        self.label_static_photometry_results_file_2_magnitude.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_2_magnitude, 3, 4, 1, 1
+        )
+
+        self.label_static_photometry_results_file_3_magnitude = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_3_magnitude.setObjectName(
+            "label_static_photometry_results_file_3_magnitude"
+        )
+        self.label_static_photometry_results_file_3_magnitude.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_3_magnitude, 4, 4, 1, 1
+        )
+
+        self.label_static_photometry_results_file_4_magnitude = QLabel(
+            self.verticalLayoutWidget_4
+        )
+        self.label_static_photometry_results_file_4_magnitude.setObjectName(
+            "label_static_photometry_results_file_4_magnitude"
+        )
+        self.label_static_photometry_results_file_4_magnitude.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_photometry_results.addWidget(
+            self.label_static_photometry_results_file_4_magnitude, 5, 4, 1, 1
+        )
 
         self.line_11 = QFrame(self.verticalLayoutWidget_4)
-        self.line_11.setObjectName(u"line_11")
+        self.line_11.setObjectName("line_11")
         self.line_11.setFrameShape(QFrame.VLine)
         self.line_11.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_photometry_results.addWidget(self.line_11, 0, 1, 6, 1)
 
         self.line_28 = QFrame(self.verticalLayoutWidget_4)
-        self.line_28.setObjectName(u"line_28")
+        self.line_28.setObjectName("line_28")
         self.line_28.setFrameShape(QFrame.HLine)
         self.line_28.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_photometry_results.addWidget(self.line_28, 1, 2, 1, 3)
 
         self.line_29 = QFrame(self.verticalLayoutWidget_4)
-        self.line_29.setObjectName(u"line_29")
+        self.line_29.setObjectName("line_29")
         self.line_29.setFrameShape(QFrame.HLine)
         self.line_29.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_photometry_results.addWidget(self.line_29, 1, 0, 1, 1)
 
-
         self.vertical_layout_photometry.addLayout(self.grid_layout_photometry_results)
 
         self.tab_widget_solutions.addTab(self.tab_photometry, "")
         self.tab_orbit = QWidget()
-        self.tab_orbit.setObjectName(u"tab_orbit")
+        self.tab_orbit.setObjectName("tab_orbit")
         self.tab_orbit.setEnabled(False)
         self.verticalLayoutWidget_5 = QWidget(self.tab_orbit)
-        self.verticalLayoutWidget_5.setObjectName(u"verticalLayoutWidget_5")
+        self.verticalLayoutWidget_5.setObjectName("verticalLayoutWidget_5")
         self.verticalLayoutWidget_5.setGeometry(QRect(10, 10, 881, 291))
         self.vertical_layout_orbit = QVBoxLayout(self.verticalLayoutWidget_5)
-        self.vertical_layout_orbit.setObjectName(u"vertical_layout_orbit")
+        self.vertical_layout_orbit.setObjectName("vertical_layout_orbit")
         self.vertical_layout_orbit.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_orbit_solve = QHBoxLayout()
-        self.horizontal_layout_orbit_solve.setObjectName(u"horizontal_layout_orbit_solve")
+        self.horizontal_layout_orbit_solve.setObjectName(
+            "horizontal_layout_orbit_solve"
+        )
         self.label_static_orbit_engine = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_engine.setObjectName(u"label_static_orbit_engine")
+        self.label_static_orbit_engine.setObjectName("label_static_orbit_engine")
 
         self.horizontal_layout_orbit_solve.addWidget(self.label_static_orbit_engine)
 
         self.combo_box_orbit_engine = QComboBox(self.verticalLayoutWidget_5)
         self.combo_box_orbit_engine.addItem("")
         self.combo_box_orbit_engine.addItem("")
-        self.combo_box_orbit_engine.setObjectName(u"combo_box_orbit_engine")
+        self.combo_box_orbit_engine.setObjectName("combo_box_orbit_engine")
 
         self.horizontal_layout_orbit_solve.addWidget(self.combo_box_orbit_engine)
 
         self.push_button_solve_orbit = QPushButton(self.verticalLayoutWidget_5)
-        self.push_button_solve_orbit.setObjectName(u"push_button_solve_orbit")
+        self.push_button_solve_orbit.setObjectName("push_button_solve_orbit")
 
         self.horizontal_layout_orbit_solve.addWidget(self.push_button_solve_orbit)
 
-
         self.vertical_layout_orbit.addLayout(self.horizontal_layout_orbit_solve)
 
         self.line_12 = QFrame(self.verticalLayoutWidget_5)
-        self.line_12.setObjectName(u"line_12")
+        self.line_12.setObjectName("line_12")
         self.line_12.setFrameShape(QFrame.HLine)
         self.line_12.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_orbit.addWidget(self.line_12)
 
         self.grid_layout_orbit_results = QGridLayout()
-        self.grid_layout_orbit_results.setObjectName(u"grid_layout_orbit_results")
-        self.line_edit_orbit_results_ascending_node_error = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_ascending_node_error.setObjectName(u"line_edit_orbit_results_ascending_node_error")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_ascending_node_error, 3, 6, 1, 1)
-
-        self.line_edit_orbit_results_ascending_node_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_ascending_node_value.setObjectName(u"line_edit_orbit_results_ascending_node_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_ascending_node_value, 3, 5, 1, 1)
-
-        self.line_edit_orbit_results_mean_anomaly_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_mean_anomaly_value.setObjectName(u"line_edit_orbit_results_mean_anomaly_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_mean_anomaly_value, 4, 5, 1, 1)
-
-        self.line_edit_orbit_results_mean_anomaly_error = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_mean_anomaly_error.setObjectName(u"line_edit_orbit_results_mean_anomaly_error")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_mean_anomaly_error, 4, 6, 1, 1)
-
-        self.line_edit_orbit_results_epoch_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_epoch_value.setObjectName(u"line_edit_orbit_results_epoch_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_epoch_value, 0, 5, 1, 2)
+        self.grid_layout_orbit_results.setObjectName("grid_layout_orbit_results")
+        self.line_edit_orbit_results_ascending_node_error = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_ascending_node_error.setObjectName(
+            "line_edit_orbit_results_ascending_node_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_ascending_node_error, 3, 6, 1, 1
+        )
+
+        self.line_edit_orbit_results_ascending_node_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_ascending_node_value.setObjectName(
+            "line_edit_orbit_results_ascending_node_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_ascending_node_value, 3, 5, 1, 1
+        )
+
+        self.line_edit_orbit_results_mean_anomaly_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_mean_anomaly_value.setObjectName(
+            "line_edit_orbit_results_mean_anomaly_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_mean_anomaly_value, 4, 5, 1, 1
+        )
+
+        self.line_edit_orbit_results_mean_anomaly_error = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_mean_anomaly_error.setObjectName(
+            "line_edit_orbit_results_mean_anomaly_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_mean_anomaly_error, 4, 6, 1, 1
+        )
+
+        self.line_edit_orbit_results_epoch_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_epoch_value.setObjectName(
+            "line_edit_orbit_results_epoch_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_epoch_value, 0, 5, 1, 2
+        )
 
         self.label_static_orbit_results_value = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_value.setObjectName(u"label_static_orbit_results_value")
-        self.label_static_orbit_results_value.setAlignment(Qt.AlignRight|Qt.AlignTrailing|Qt.AlignVCenter)
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_value, 0, 1, 1, 1)
+        self.label_static_orbit_results_value.setObjectName(
+            "label_static_orbit_results_value"
+        )
+        self.label_static_orbit_results_value.setAlignment(
+            Qt.AlignRight | Qt.AlignTrailing | Qt.AlignVCenter
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_value, 0, 1, 1, 1
+        )
 
         self.label_static_orbit_results_error = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_error.setObjectName(u"label_static_orbit_results_error")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_error, 0, 2, 1, 1)
-
-        self.label_static_orbit_results_semimajor_axis = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_semimajor_axis.setObjectName(u"label_static_orbit_results_semimajor_axis")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_semimajor_axis, 2, 0, 1, 1)
-
-        self.label_static_orbit_results_eccentricity = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_eccentricity.setObjectName(u"label_static_orbit_results_eccentricity")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_eccentricity, 2, 4, 1, 1)
-
-        self.label_static_orbit_results_mean_anomaly = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_mean_anomaly.setObjectName(u"label_static_orbit_results_mean_anomaly")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_mean_anomaly, 4, 4, 1, 1)
-
-        self.label_static_orbit_results_inclination = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_inclination.setObjectName(u"label_static_orbit_results_inclination")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_inclination, 3, 0, 1, 1)
+        self.label_static_orbit_results_error.setObjectName(
+            "label_static_orbit_results_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_error, 0, 2, 1, 1
+        )
+
+        self.label_static_orbit_results_semimajor_axis = QLabel(
+            self.verticalLayoutWidget_5
+        )
+        self.label_static_orbit_results_semimajor_axis.setObjectName(
+            "label_static_orbit_results_semimajor_axis"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_semimajor_axis, 2, 0, 1, 1
+        )
+
+        self.label_static_orbit_results_eccentricity = QLabel(
+            self.verticalLayoutWidget_5
+        )
+        self.label_static_orbit_results_eccentricity.setObjectName(
+            "label_static_orbit_results_eccentricity"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_eccentricity, 2, 4, 1, 1
+        )
+
+        self.label_static_orbit_results_mean_anomaly = QLabel(
+            self.verticalLayoutWidget_5
+        )
+        self.label_static_orbit_results_mean_anomaly.setObjectName(
+            "label_static_orbit_results_mean_anomaly"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_mean_anomaly, 4, 4, 1, 1
+        )
+
+        self.label_static_orbit_results_inclination = QLabel(
+            self.verticalLayoutWidget_5
+        )
+        self.label_static_orbit_results_inclination.setObjectName(
+            "label_static_orbit_results_inclination"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_inclination, 3, 0, 1, 1
+        )
 
         self.label_static_orbit_results_perihelion = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_perihelion.setObjectName(u"label_static_orbit_results_perihelion")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_perihelion, 4, 0, 1, 1)
-
-        self.line_edit_orbit_results_semimajor_axis_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_semimajor_axis_value.setObjectName(u"line_edit_orbit_results_semimajor_axis_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_semimajor_axis_value, 2, 1, 1, 1)
-
-        self.line_edit_orbit_results_perihelion_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_perihelion_value.setObjectName(u"line_edit_orbit_results_perihelion_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_perihelion_value, 4, 1, 1, 1)
-
-        self.label_static_orbit_results_ascending_node = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_ascending_node.setObjectName(u"label_static_orbit_results_ascending_node")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_ascending_node, 3, 4, 1, 1)
+        self.label_static_orbit_results_perihelion.setObjectName(
+            "label_static_orbit_results_perihelion"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_perihelion, 4, 0, 1, 1
+        )
+
+        self.line_edit_orbit_results_semimajor_axis_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_semimajor_axis_value.setObjectName(
+            "line_edit_orbit_results_semimajor_axis_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_semimajor_axis_value, 2, 1, 1, 1
+        )
+
+        self.line_edit_orbit_results_perihelion_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_perihelion_value.setObjectName(
+            "line_edit_orbit_results_perihelion_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_perihelion_value, 4, 1, 1, 1
+        )
+
+        self.label_static_orbit_results_ascending_node = QLabel(
+            self.verticalLayoutWidget_5
+        )
+        self.label_static_orbit_results_ascending_node.setObjectName(
+            "label_static_orbit_results_ascending_node"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_ascending_node, 3, 4, 1, 1
+        )
 
         self.label_static_orbit_results_epoch = QLabel(self.verticalLayoutWidget_5)
-        self.label_static_orbit_results_epoch.setObjectName(u"label_static_orbit_results_epoch")
-
-        self.grid_layout_orbit_results.addWidget(self.label_static_orbit_results_epoch, 0, 4, 1, 1)
-
-        self.line_edit_orbit_results_inclination_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_inclination_value.setObjectName(u"line_edit_orbit_results_inclination_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_inclination_value, 3, 1, 1, 1)
-
-        self.line_edit_orbit_results_eccentricity_error = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_eccentricity_error.setObjectName(u"line_edit_orbit_results_eccentricity_error")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_eccentricity_error, 2, 6, 1, 1)
-
-        self.line_edit_orbit_results_inclination_error = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_inclination_error.setObjectName(u"line_edit_orbit_results_inclination_error")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_inclination_error, 3, 2, 1, 1)
-
-        self.line_edit_orbit_results_perihelion_error = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_perihelion_error.setObjectName(u"line_edit_orbit_results_perihelion_error")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_perihelion_error, 4, 2, 1, 1)
-
-        self.line_edit_orbit_results_eccentricity_value = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_eccentricity_value.setObjectName(u"line_edit_orbit_results_eccentricity_value")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_eccentricity_value, 2, 5, 1, 1)
-
-        self.line_edit_orbit_results_semimajor_axis_error = QLineEdit(self.verticalLayoutWidget_5)
-        self.line_edit_orbit_results_semimajor_axis_error.setObjectName(u"line_edit_orbit_results_semimajor_axis_error")
-
-        self.grid_layout_orbit_results.addWidget(self.line_edit_orbit_results_semimajor_axis_error, 2, 2, 1, 1)
+        self.label_static_orbit_results_epoch.setObjectName(
+            "label_static_orbit_results_epoch"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.label_static_orbit_results_epoch, 0, 4, 1, 1
+        )
+
+        self.line_edit_orbit_results_inclination_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_inclination_value.setObjectName(
+            "line_edit_orbit_results_inclination_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_inclination_value, 3, 1, 1, 1
+        )
+
+        self.line_edit_orbit_results_eccentricity_error = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_eccentricity_error.setObjectName(
+            "line_edit_orbit_results_eccentricity_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_eccentricity_error, 2, 6, 1, 1
+        )
+
+        self.line_edit_orbit_results_inclination_error = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_inclination_error.setObjectName(
+            "line_edit_orbit_results_inclination_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_inclination_error, 3, 2, 1, 1
+        )
+
+        self.line_edit_orbit_results_perihelion_error = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_perihelion_error.setObjectName(
+            "line_edit_orbit_results_perihelion_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_perihelion_error, 4, 2, 1, 1
+        )
+
+        self.line_edit_orbit_results_eccentricity_value = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_eccentricity_value.setObjectName(
+            "line_edit_orbit_results_eccentricity_value"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_eccentricity_value, 2, 5, 1, 1
+        )
+
+        self.line_edit_orbit_results_semimajor_axis_error = QLineEdit(
+            self.verticalLayoutWidget_5
+        )
+        self.line_edit_orbit_results_semimajor_axis_error.setObjectName(
+            "line_edit_orbit_results_semimajor_axis_error"
+        )
+
+        self.grid_layout_orbit_results.addWidget(
+            self.line_edit_orbit_results_semimajor_axis_error, 2, 2, 1, 1
+        )
 
         self.line_30 = QFrame(self.verticalLayoutWidget_5)
-        self.line_30.setObjectName(u"line_30")
+        self.line_30.setObjectName("line_30")
         self.line_30.setFrameShape(QFrame.VLine)
         self.line_30.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_orbit_results.addWidget(self.line_30, 2, 3, 3, 1)
 
         self.line_31 = QFrame(self.verticalLayoutWidget_5)
-        self.line_31.setObjectName(u"line_31")
+        self.line_31.setObjectName("line_31")
         self.line_31.setFrameShape(QFrame.HLine)
         self.line_31.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_orbit_results.addWidget(self.line_31, 1, 0, 1, 7)
 
         self.line_32 = QFrame(self.verticalLayoutWidget_5)
-        self.line_32.setObjectName(u"line_32")
+        self.line_32.setObjectName("line_32")
         self.line_32.setFrameShape(QFrame.VLine)
         self.line_32.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_orbit_results.addWidget(self.line_32, 0, 3, 1, 1)
 
-
         self.vertical_layout_orbit.addLayout(self.grid_layout_orbit_results)
 
         self.tab_widget_solutions.addTab(self.tab_orbit, "")
         self.tab_ephemeris = QWidget()
-        self.tab_ephemeris.setObjectName(u"tab_ephemeris")
+        self.tab_ephemeris.setObjectName("tab_ephemeris")
         self.tab_ephemeris.setEnabled(False)
         self.verticalLayoutWidget_6 = QWidget(self.tab_ephemeris)
-        self.verticalLayoutWidget_6.setObjectName(u"verticalLayoutWidget_6")
+        self.verticalLayoutWidget_6.setObjectName("verticalLayoutWidget_6")
         self.verticalLayoutWidget_6.setGeometry(QRect(10, 10, 881, 291))
         self.vertical_layout_ephemeris = QVBoxLayout(self.verticalLayoutWidget_6)
-        self.vertical_layout_ephemeris.setObjectName(u"vertical_layout_ephemeris")
+        self.vertical_layout_ephemeris.setObjectName("vertical_layout_ephemeris")
         self.vertical_layout_ephemeris.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_ephemeris_solve = QHBoxLayout()
-        self.horizontal_layout_ephemeris_solve.setObjectName(u"horizontal_layout_ephemeris_solve")
+        self.horizontal_layout_ephemeris_solve.setObjectName(
+            "horizontal_layout_ephemeris_solve"
+        )
         self.label_static_ephemeris_engine = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_engine.setObjectName(u"label_static_ephemeris_engine")
-
-        self.horizontal_layout_ephemeris_solve.addWidget(self.label_static_ephemeris_engine)
+        self.label_static_ephemeris_engine.setObjectName(
+            "label_static_ephemeris_engine"
+        )
+
+        self.horizontal_layout_ephemeris_solve.addWidget(
+            self.label_static_ephemeris_engine
+        )
 
         self.combo_box_ephemeris_engine = QComboBox(self.verticalLayoutWidget_6)
         self.combo_box_ephemeris_engine.addItem("")
-        self.combo_box_ephemeris_engine.setObjectName(u"combo_box_ephemeris_engine")
+        self.combo_box_ephemeris_engine.setObjectName("combo_box_ephemeris_engine")
 
-        self.horizontal_layout_ephemeris_solve.addWidget(self.combo_box_ephemeris_engine)
+        self.horizontal_layout_ephemeris_solve.addWidget(
+            self.combo_box_ephemeris_engine
+        )
 
         self.push_button_solve_ephemeris = QPushButton(self.verticalLayoutWidget_6)
-        self.push_button_solve_ephemeris.setObjectName(u"push_button_solve_ephemeris")
-
-        self.horizontal_layout_ephemeris_solve.addWidget(self.push_button_solve_ephemeris)
+        self.push_button_solve_ephemeris.setObjectName("push_button_solve_ephemeris")
 
+        self.horizontal_layout_ephemeris_solve.addWidget(
+            self.push_button_solve_ephemeris
+        )
 
         self.vertical_layout_ephemeris.addLayout(self.horizontal_layout_ephemeris_solve)
 
         self.line_13 = QFrame(self.verticalLayoutWidget_6)
-        self.line_13.setObjectName(u"line_13")
+        self.line_13.setObjectName("line_13")
         self.line_13.setFrameShape(QFrame.HLine)
         self.line_13.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_ephemeris.addWidget(self.line_13)
 
         self.grid_layout_ephemeris_results = QGridLayout()
-        self.grid_layout_ephemeris_results.setObjectName(u"grid_layout_ephemeris_results")
-        self.label_static_ephemeris_results_nonsiderial_rates = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_nonsiderial_rates.setObjectName(u"label_static_ephemeris_results_nonsiderial_rates")
-        self.label_static_ephemeris_results_nonsiderial_rates.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_nonsiderial_rates, 0, 1, 1, 9)
-
-        self.push_button_ephemeris_results_update_tcs_rates = QPushButton(self.verticalLayoutWidget_6)
-        self.push_button_ephemeris_results_update_tcs_rates.setObjectName(u"push_button_ephemeris_results_update_tcs_rates")
-
-        self.grid_layout_ephemeris_results.addWidget(self.push_button_ephemeris_results_update_tcs_rates, 5, 1, 1, 9)
-
-        self.label_dynamic_ephemeris_results_first_order_ra_error = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_first_order_ra_error.setObjectName(u"label_dynamic_ephemeris_results_first_order_ra_error")
-        self.label_dynamic_ephemeris_results_first_order_ra_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_first_order_ra_error, 4, 2, 1, 1)
-
-        self.label_static_ephemeris_results_second_order_dec = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_second_order_dec.setObjectName(u"label_static_ephemeris_results_second_order_dec")
-        self.label_static_ephemeris_results_second_order_dec.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_second_order_dec, 2, 8, 1, 2)
-
-        self.label_static_ephemeris_results_first_order_dec = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_first_order_dec.setObjectName(u"label_static_ephemeris_results_first_order_dec")
+        self.grid_layout_ephemeris_results.setObjectName(
+            "grid_layout_ephemeris_results"
+        )
+        self.label_static_ephemeris_results_nonsiderial_rates = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_nonsiderial_rates.setObjectName(
+            "label_static_ephemeris_results_nonsiderial_rates"
+        )
+        self.label_static_ephemeris_results_nonsiderial_rates.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_nonsiderial_rates, 0, 1, 1, 9
+        )
+
+        self.push_button_ephemeris_results_update_tcs_rates = QPushButton(
+            self.verticalLayoutWidget_6
+        )
+        self.push_button_ephemeris_results_update_tcs_rates.setObjectName(
+            "push_button_ephemeris_results_update_tcs_rates"
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.push_button_ephemeris_results_update_tcs_rates, 5, 1, 1, 9
+        )
+
+        self.label_dynamic_ephemeris_results_first_order_ra_error = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_first_order_ra_error.setObjectName(
+            "label_dynamic_ephemeris_results_first_order_ra_error"
+        )
+        self.label_dynamic_ephemeris_results_first_order_ra_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_first_order_ra_error, 4, 2, 1, 1
+        )
+
+        self.label_static_ephemeris_results_second_order_dec = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_second_order_dec.setObjectName(
+            "label_static_ephemeris_results_second_order_dec"
+        )
+        self.label_static_ephemeris_results_second_order_dec.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_second_order_dec, 2, 8, 1, 2
+        )
+
+        self.label_static_ephemeris_results_first_order_dec = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_first_order_dec.setObjectName(
+            "label_static_ephemeris_results_first_order_dec"
+        )
         self.label_static_ephemeris_results_first_order_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_first_order_dec, 2, 3, 1, 2)
-
-        self.label_static_ephemeris_results_second_order_ra = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_second_order_ra.setObjectName(u"label_static_ephemeris_results_second_order_ra")
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_first_order_dec, 2, 3, 1, 2
+        )
+
+        self.label_static_ephemeris_results_second_order_ra = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_second_order_ra.setObjectName(
+            "label_static_ephemeris_results_second_order_ra"
+        )
         self.label_static_ephemeris_results_second_order_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_second_order_ra, 2, 6, 1, 2)
-
-        self.label_static_ephemeris_results_second_order = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_second_order.setObjectName(u"label_static_ephemeris_results_second_order")
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_second_order_ra, 2, 6, 1, 2
+        )
+
+        self.label_static_ephemeris_results_second_order = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_second_order.setObjectName(
+            "label_static_ephemeris_results_second_order"
+        )
         self.label_static_ephemeris_results_second_order.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_second_order, 1, 6, 1, 4)
-
-        self.label_static_ephemeris_results_first_order_ra = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_first_order_ra.setObjectName(u"label_static_ephemeris_results_first_order_ra")
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_second_order, 1, 6, 1, 4
+        )
+
+        self.label_static_ephemeris_results_first_order_ra = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_first_order_ra.setObjectName(
+            "label_static_ephemeris_results_first_order_ra"
+        )
         self.label_static_ephemeris_results_first_order_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_first_order_ra, 2, 1, 1, 2)
-
-        self.label_dynamic_ephemeris_results_second_order_ra_error = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_second_order_ra_error.setObjectName(u"label_dynamic_ephemeris_results_second_order_ra_error")
-        self.label_dynamic_ephemeris_results_second_order_ra_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_second_order_ra_error, 4, 7, 1, 1)
-
-        self.label_dynamic_ephemeris_results_second_order_dec_error = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_second_order_dec_error.setObjectName(u"label_dynamic_ephemeris_results_second_order_dec_error")
-        self.label_dynamic_ephemeris_results_second_order_dec_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_second_order_dec_error, 4, 9, 1, 1)
-
-        self.label_dynamic_ephemeris_results_second_order_dec_rate = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_second_order_dec_rate.setObjectName(u"label_dynamic_ephemeris_results_second_order_dec_rate")
-        self.label_dynamic_ephemeris_results_second_order_dec_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_second_order_dec_rate, 4, 8, 1, 1)
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_first_order_ra, 2, 1, 1, 2
+        )
+
+        self.label_dynamic_ephemeris_results_second_order_ra_error = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_second_order_ra_error.setObjectName(
+            "label_dynamic_ephemeris_results_second_order_ra_error"
+        )
+        self.label_dynamic_ephemeris_results_second_order_ra_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_second_order_ra_error, 4, 7, 1, 1
+        )
+
+        self.label_dynamic_ephemeris_results_second_order_dec_error = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_second_order_dec_error.setObjectName(
+            "label_dynamic_ephemeris_results_second_order_dec_error"
+        )
+        self.label_dynamic_ephemeris_results_second_order_dec_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_second_order_dec_error, 4, 9, 1, 1
+        )
+
+        self.label_dynamic_ephemeris_results_second_order_dec_rate = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_second_order_dec_rate.setObjectName(
+            "label_dynamic_ephemeris_results_second_order_dec_rate"
+        )
+        self.label_dynamic_ephemeris_results_second_order_dec_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_second_order_dec_rate, 4, 8, 1, 1
+        )
 
         self.line_14 = QFrame(self.verticalLayoutWidget_6)
-        self.line_14.setObjectName(u"line_14")
+        self.line_14.setObjectName("line_14")
         self.line_14.setFrameShape(QFrame.VLine)
         self.line_14.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_ephemeris_results.addWidget(self.line_14, 1, 5, 4, 1)
 
-        self.label_static_ephemeris_results_first_order = QLabel(self.verticalLayoutWidget_6)
-        self.label_static_ephemeris_results_first_order.setObjectName(u"label_static_ephemeris_results_first_order")
+        self.label_static_ephemeris_results_first_order = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_static_ephemeris_results_first_order.setObjectName(
+            "label_static_ephemeris_results_first_order"
+        )
         self.label_static_ephemeris_results_first_order.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_ephemeris_results.addWidget(self.label_static_ephemeris_results_first_order, 1, 1, 1, 4)
-
-        self.label_dynamic_ephemeris_results_first_order_dec_error = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_first_order_dec_error.setObjectName(u"label_dynamic_ephemeris_results_first_order_dec_error")
-        self.label_dynamic_ephemeris_results_first_order_dec_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_first_order_dec_error, 4, 4, 1, 1)
-
-        self.label_dynamic_ephemeris_results_first_order_dec_rate = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_first_order_dec_rate.setObjectName(u"label_dynamic_ephemeris_results_first_order_dec_rate")
-        self.label_dynamic_ephemeris_results_first_order_dec_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_first_order_dec_rate, 4, 3, 1, 1)
-
-        self.label_dynamic_ephemeris_results_second_order_ra_rate = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_second_order_ra_rate.setObjectName(u"label_dynamic_ephemeris_results_second_order_ra_rate")
-        self.label_dynamic_ephemeris_results_second_order_ra_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_second_order_ra_rate, 4, 6, 1, 1)
-
-        self.label_dynamic_ephemeris_results_first_order_ra_rate = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_results_first_order_ra_rate.setObjectName(u"label_dynamic_ephemeris_results_first_order_ra_rate")
-        self.label_dynamic_ephemeris_results_first_order_ra_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_ephemeris_results.addWidget(self.label_dynamic_ephemeris_results_first_order_ra_rate, 4, 1, 1, 1)
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_static_ephemeris_results_first_order, 1, 1, 1, 4
+        )
+
+        self.label_dynamic_ephemeris_results_first_order_dec_error = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_first_order_dec_error.setObjectName(
+            "label_dynamic_ephemeris_results_first_order_dec_error"
+        )
+        self.label_dynamic_ephemeris_results_first_order_dec_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_first_order_dec_error, 4, 4, 1, 1
+        )
+
+        self.label_dynamic_ephemeris_results_first_order_dec_rate = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_first_order_dec_rate.setObjectName(
+            "label_dynamic_ephemeris_results_first_order_dec_rate"
+        )
+        self.label_dynamic_ephemeris_results_first_order_dec_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_first_order_dec_rate, 4, 3, 1, 1
+        )
+
+        self.label_dynamic_ephemeris_results_second_order_ra_rate = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_second_order_ra_rate.setObjectName(
+            "label_dynamic_ephemeris_results_second_order_ra_rate"
+        )
+        self.label_dynamic_ephemeris_results_second_order_ra_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_second_order_ra_rate, 4, 6, 1, 1
+        )
+
+        self.label_dynamic_ephemeris_results_first_order_ra_rate = QLabel(
+            self.verticalLayoutWidget_6
+        )
+        self.label_dynamic_ephemeris_results_first_order_ra_rate.setObjectName(
+            "label_dynamic_ephemeris_results_first_order_ra_rate"
+        )
+        self.label_dynamic_ephemeris_results_first_order_ra_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_ephemeris_results.addWidget(
+            self.label_dynamic_ephemeris_results_first_order_ra_rate, 4, 1, 1, 1
+        )
 
         self.line_15 = QFrame(self.verticalLayoutWidget_6)
-        self.line_15.setObjectName(u"line_15")
+        self.line_15.setObjectName("line_15")
         self.line_15.setFrameShape(QFrame.HLine)
         self.line_15.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_ephemeris_results.addWidget(self.line_15, 3, 1, 1, 4)
 
         self.line_16 = QFrame(self.verticalLayoutWidget_6)
-        self.line_16.setObjectName(u"line_16")
+        self.line_16.setObjectName("line_16")
         self.line_16.setFrameShape(QFrame.HLine)
         self.line_16.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_ephemeris_results.addWidget(self.line_16, 3, 6, 1, 4)
 
-
         self.vertical_layout_ephemeris.addLayout(self.grid_layout_ephemeris_results)
 
         self.line_17 = QFrame(self.verticalLayoutWidget_6)
-        self.line_17.setObjectName(u"line_17")
+        self.line_17.setObjectName("line_17")
         self.line_17.setFrameShape(QFrame.HLine)
         self.line_17.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_ephemeris.addWidget(self.line_17)
 
         self.horizontal_layout_ephemeris_forward = QHBoxLayout()
-        self.horizontal_layout_ephemeris_forward.setObjectName(u"horizontal_layout_ephemeris_forward")
-        self.combo_box_ephemeris_forward_datetime = QDateTimeEdit(self.verticalLayoutWidget_6)
-        self.combo_box_ephemeris_forward_datetime.setObjectName(u"combo_box_ephemeris_forward_datetime")
+        self.horizontal_layout_ephemeris_forward.setObjectName(
+            "horizontal_layout_ephemeris_forward"
+        )
+        self.combo_box_ephemeris_forward_datetime = QDateTimeEdit(
+            self.verticalLayoutWidget_6
+        )
+        self.combo_box_ephemeris_forward_datetime.setObjectName(
+            "combo_box_ephemeris_forward_datetime"
+        )
         self.combo_box_ephemeris_forward_datetime.setMinimumSize(QSize(200, 0))
-        self.combo_box_ephemeris_forward_datetime.setMaximumSize(QSize(16777213, 16777215))
-
-        self.horizontal_layout_ephemeris_forward.addWidget(self.combo_box_ephemeris_forward_datetime)
-
-        self.combo_box_ephemeris_forward_timezone = QComboBox(self.verticalLayoutWidget_6)
+        self.combo_box_ephemeris_forward_datetime.setMaximumSize(
+            QSize(16777213, 16777215)
+        )
+
+        self.horizontal_layout_ephemeris_forward.addWidget(
+            self.combo_box_ephemeris_forward_datetime
+        )
+
+        self.combo_box_ephemeris_forward_timezone = QComboBox(
+            self.verticalLayoutWidget_6
+        )
         self.combo_box_ephemeris_forward_timezone.addItem("")
         self.combo_box_ephemeris_forward_timezone.addItem("")
-        self.combo_box_ephemeris_forward_timezone.setObjectName(u"combo_box_ephemeris_forward_timezone")
-
-        self.horizontal_layout_ephemeris_forward.addWidget(self.combo_box_ephemeris_forward_timezone)
-
-        self.push_button_ephemeris_forward_solve = QPushButton(self.verticalLayoutWidget_6)
-        self.push_button_ephemeris_forward_solve.setObjectName(u"push_button_ephemeris_forward_solve")
-
-        self.horizontal_layout_ephemeris_forward.addWidget(self.push_button_ephemeris_forward_solve)
+        self.combo_box_ephemeris_forward_timezone.setObjectName(
+            "combo_box_ephemeris_forward_timezone"
+        )
+
+        self.horizontal_layout_ephemeris_forward.addWidget(
+            self.combo_box_ephemeris_forward_timezone
+        )
+
+        self.push_button_ephemeris_forward_solve = QPushButton(
+            self.verticalLayoutWidget_6
+        )
+        self.push_button_ephemeris_forward_solve.setObjectName(
+            "push_button_ephemeris_forward_solve"
+        )
+
+        self.horizontal_layout_ephemeris_forward.addWidget(
+            self.push_button_ephemeris_forward_solve
+        )
 
         self.line_18 = QFrame(self.verticalLayoutWidget_6)
-        self.line_18.setObjectName(u"line_18")
+        self.line_18.setObjectName("line_18")
         self.line_18.setFrameShape(QFrame.VLine)
         self.line_18.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_ephemeris_forward.addWidget(self.line_18)
 
         self.label_dynamic_ephemeris_forward_ra = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_forward_ra.setObjectName(u"label_dynamic_ephemeris_forward_ra")
+        self.label_dynamic_ephemeris_forward_ra.setObjectName(
+            "label_dynamic_ephemeris_forward_ra"
+        )
         self.label_dynamic_ephemeris_forward_ra.setAlignment(Qt.AlignCenter)
 
-        self.horizontal_layout_ephemeris_forward.addWidget(self.label_dynamic_ephemeris_forward_ra)
+        self.horizontal_layout_ephemeris_forward.addWidget(
+            self.label_dynamic_ephemeris_forward_ra
+        )
 
         self.label_dynamic_ephemeris_forward_dec = QLabel(self.verticalLayoutWidget_6)
-        self.label_dynamic_ephemeris_forward_dec.setObjectName(u"label_dynamic_ephemeris_forward_dec")
+        self.label_dynamic_ephemeris_forward_dec.setObjectName(
+            "label_dynamic_ephemeris_forward_dec"
+        )
         self.label_dynamic_ephemeris_forward_dec.setAlignment(Qt.AlignCenter)
 
-        self.horizontal_layout_ephemeris_forward.addWidget(self.label_dynamic_ephemeris_forward_dec)
-
-
-        self.vertical_layout_ephemeris.addLayout(self.horizontal_layout_ephemeris_forward)
+        self.horizontal_layout_ephemeris_forward.addWidget(
+            self.label_dynamic_ephemeris_forward_dec
+        )
+
+        self.vertical_layout_ephemeris.addLayout(
+            self.horizontal_layout_ephemeris_forward
+        )
 
         self.tab_widget_solutions.addTab(self.tab_ephemeris, "")
         self.tab_propagate = QWidget()
-        self.tab_propagate.setObjectName(u"tab_propagate")
+        self.tab_propagate.setObjectName("tab_propagate")
         self.verticalLayoutWidget_7 = QWidget(self.tab_propagate)
-        self.verticalLayoutWidget_7.setObjectName(u"verticalLayoutWidget_7")
+        self.verticalLayoutWidget_7.setObjectName("verticalLayoutWidget_7")
         self.verticalLayoutWidget_7.setGeometry(QRect(10, 10, 881, 291))
         self.vertical_layout_propagate = QVBoxLayout(self.verticalLayoutWidget_7)
-        self.vertical_layout_propagate.setObjectName(u"vertical_layout_propagate")
+        self.vertical_layout_propagate.setObjectName("vertical_layout_propagate")
         self.vertical_layout_propagate.setContentsMargins(0, 0, 0, 0)
         self.horizontal_layout_propagate_solve = QHBoxLayout()
-        self.horizontal_layout_propagate_solve.setObjectName(u"horizontal_layout_propagate_solve")
+        self.horizontal_layout_propagate_solve.setObjectName(
+            "horizontal_layout_propagate_solve"
+        )
         self.label_static_propagate_engine = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_engine.setObjectName(u"label_static_propagate_engine")
-
-        self.horizontal_layout_propagate_solve.addWidget(self.label_static_propagate_engine)
+        self.label_static_propagate_engine.setObjectName(
+            "label_static_propagate_engine"
+        )
+
+        self.horizontal_layout_propagate_solve.addWidget(
+            self.label_static_propagate_engine
+        )
 
         self.combo_box_propagate_engine = QComboBox(self.verticalLayoutWidget_7)
         self.combo_box_propagate_engine.addItem("")
         self.combo_box_propagate_engine.addItem("")
-        self.combo_box_propagate_engine.setObjectName(u"combo_box_propagate_engine")
+        self.combo_box_propagate_engine.setObjectName("combo_box_propagate_engine")
 
-        self.horizontal_layout_propagate_solve.addWidget(self.combo_box_propagate_engine)
+        self.horizontal_layout_propagate_solve.addWidget(
+            self.combo_box_propagate_engine
+        )
 
         self.push_button_solve_propagation = QPushButton(self.verticalLayoutWidget_7)
-        self.push_button_solve_propagation.setObjectName(u"push_button_solve_propagation")
-
-        self.horizontal_layout_propagate_solve.addWidget(self.push_button_solve_propagation)
-
+        self.push_button_solve_propagation.setObjectName(
+            "push_button_solve_propagation"
+        )
+
+        self.horizontal_layout_propagate_solve.addWidget(
+            self.push_button_solve_propagation
+        )
 
         self.vertical_layout_propagate.addLayout(self.horizontal_layout_propagate_solve)
 
         self.line_22 = QFrame(self.verticalLayoutWidget_7)
-        self.line_22.setObjectName(u"line_22")
+        self.line_22.setObjectName("line_22")
         self.line_22.setFrameShape(QFrame.HLine)
         self.line_22.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_propagate.addWidget(self.line_22)
 
         self.grid_layout_propagate_results = QGridLayout()
-        self.grid_layout_propagate_results.setObjectName(u"grid_layout_propagate_results")
-        self.label_static_propagate_results_nonsiderial_rates = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_nonsiderial_rates.setObjectName(u"label_static_propagate_results_nonsiderial_rates")
-        self.label_static_propagate_results_nonsiderial_rates.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_nonsiderial_rates, 0, 1, 1, 9)
-
-        self.push_button_propagate_results_update_tcs_rates = QPushButton(self.verticalLayoutWidget_7)
-        self.push_button_propagate_results_update_tcs_rates.setObjectName(u"push_button_propagate_results_update_tcs_rates")
-
-        self.grid_layout_propagate_results.addWidget(self.push_button_propagate_results_update_tcs_rates, 5, 1, 1, 9)
-
-        self.label_dynamic_propagate_results_first_order_ra_error = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_first_order_ra_error.setObjectName(u"label_dynamic_propagate_results_first_order_ra_error")
-        self.label_dynamic_propagate_results_first_order_ra_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_first_order_ra_error, 4, 2, 1, 1)
-
-        self.label_static_propagate_results_second_order_dec = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_second_order_dec.setObjectName(u"label_static_propagate_results_second_order_dec")
-        self.label_static_propagate_results_second_order_dec.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_second_order_dec, 2, 8, 1, 2)
-
-        self.label_static_propagate_results_first_order_dec = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_first_order_dec.setObjectName(u"label_static_propagate_results_first_order_dec")
+        self.grid_layout_propagate_results.setObjectName(
+            "grid_layout_propagate_results"
+        )
+        self.label_static_propagate_results_nonsiderial_rates = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_nonsiderial_rates.setObjectName(
+            "label_static_propagate_results_nonsiderial_rates"
+        )
+        self.label_static_propagate_results_nonsiderial_rates.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_nonsiderial_rates, 0, 1, 1, 9
+        )
+
+        self.push_button_propagate_results_update_tcs_rates = QPushButton(
+            self.verticalLayoutWidget_7
+        )
+        self.push_button_propagate_results_update_tcs_rates.setObjectName(
+            "push_button_propagate_results_update_tcs_rates"
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.push_button_propagate_results_update_tcs_rates, 5, 1, 1, 9
+        )
+
+        self.label_dynamic_propagate_results_first_order_ra_error = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_first_order_ra_error.setObjectName(
+            "label_dynamic_propagate_results_first_order_ra_error"
+        )
+        self.label_dynamic_propagate_results_first_order_ra_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_first_order_ra_error, 4, 2, 1, 1
+        )
+
+        self.label_static_propagate_results_second_order_dec = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_second_order_dec.setObjectName(
+            "label_static_propagate_results_second_order_dec"
+        )
+        self.label_static_propagate_results_second_order_dec.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_second_order_dec, 2, 8, 1, 2
+        )
+
+        self.label_static_propagate_results_first_order_dec = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_first_order_dec.setObjectName(
+            "label_static_propagate_results_first_order_dec"
+        )
         self.label_static_propagate_results_first_order_dec.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_first_order_dec, 2, 3, 1, 2)
-
-        self.label_static_propagate_results_second_order_ra = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_second_order_ra.setObjectName(u"label_static_propagate_results_second_order_ra")
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_first_order_dec, 2, 3, 1, 2
+        )
+
+        self.label_static_propagate_results_second_order_ra = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_second_order_ra.setObjectName(
+            "label_static_propagate_results_second_order_ra"
+        )
         self.label_static_propagate_results_second_order_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_second_order_ra, 2, 6, 1, 2)
-
-        self.label_static_propagate_results_second_order = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_second_order.setObjectName(u"label_static_propagate_results_second_order")
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_second_order_ra, 2, 6, 1, 2
+        )
+
+        self.label_static_propagate_results_second_order = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_second_order.setObjectName(
+            "label_static_propagate_results_second_order"
+        )
         self.label_static_propagate_results_second_order.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_second_order, 1, 6, 1, 4)
-
-        self.label_static_propagate_results_first_order_ra = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_first_order_ra.setObjectName(u"label_static_propagate_results_first_order_ra")
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_second_order, 1, 6, 1, 4
+        )
+
+        self.label_static_propagate_results_first_order_ra = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_first_order_ra.setObjectName(
+            "label_static_propagate_results_first_order_ra"
+        )
         self.label_static_propagate_results_first_order_ra.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_first_order_ra, 2, 1, 1, 2)
-
-        self.label_dynamic_propagate_results_second_order_ra_error = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_second_order_ra_error.setObjectName(u"label_dynamic_propagate_results_second_order_ra_error")
-        self.label_dynamic_propagate_results_second_order_ra_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_second_order_ra_error, 4, 7, 1, 1)
-
-        self.label_dynamic_propagate_results_second_order_dec_error = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_second_order_dec_error.setObjectName(u"label_dynamic_propagate_results_second_order_dec_error")
-        self.label_dynamic_propagate_results_second_order_dec_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_second_order_dec_error, 4, 9, 1, 1)
-
-        self.label_dynamic_propagate_results_second_order_dec_rate = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_second_order_dec_rate.setObjectName(u"label_dynamic_propagate_results_second_order_dec_rate")
-        self.label_dynamic_propagate_results_second_order_dec_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_second_order_dec_rate, 4, 8, 1, 1)
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_first_order_ra, 2, 1, 1, 2
+        )
+
+        self.label_dynamic_propagate_results_second_order_ra_error = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_second_order_ra_error.setObjectName(
+            "label_dynamic_propagate_results_second_order_ra_error"
+        )
+        self.label_dynamic_propagate_results_second_order_ra_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_second_order_ra_error, 4, 7, 1, 1
+        )
+
+        self.label_dynamic_propagate_results_second_order_dec_error = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_second_order_dec_error.setObjectName(
+            "label_dynamic_propagate_results_second_order_dec_error"
+        )
+        self.label_dynamic_propagate_results_second_order_dec_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_second_order_dec_error, 4, 9, 1, 1
+        )
+
+        self.label_dynamic_propagate_results_second_order_dec_rate = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_second_order_dec_rate.setObjectName(
+            "label_dynamic_propagate_results_second_order_dec_rate"
+        )
+        self.label_dynamic_propagate_results_second_order_dec_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_second_order_dec_rate, 4, 8, 1, 1
+        )
 
         self.line_19 = QFrame(self.verticalLayoutWidget_7)
-        self.line_19.setObjectName(u"line_19")
+        self.line_19.setObjectName("line_19")
         self.line_19.setFrameShape(QFrame.VLine)
         self.line_19.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_propagate_results.addWidget(self.line_19, 1, 5, 4, 1)
 
-        self.label_static_propagate_results_first_order = QLabel(self.verticalLayoutWidget_7)
-        self.label_static_propagate_results_first_order.setObjectName(u"label_static_propagate_results_first_order")
+        self.label_static_propagate_results_first_order = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_static_propagate_results_first_order.setObjectName(
+            "label_static_propagate_results_first_order"
+        )
         self.label_static_propagate_results_first_order.setAlignment(Qt.AlignCenter)
 
-        self.grid_layout_propagate_results.addWidget(self.label_static_propagate_results_first_order, 1, 1, 1, 4)
-
-        self.label_dynamic_propagate_results_first_order_dec_error = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_first_order_dec_error.setObjectName(u"label_dynamic_propagate_results_first_order_dec_error")
-        self.label_dynamic_propagate_results_first_order_dec_error.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_first_order_dec_error, 4, 4, 1, 1)
-
-        self.label_dynamic_propagate_results_first_order_dec_rate = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_first_order_dec_rate.setObjectName(u"label_dynamic_propagate_results_first_order_dec_rate")
-        self.label_dynamic_propagate_results_first_order_dec_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_first_order_dec_rate, 4, 3, 1, 1)
-
-        self.label_dynamic_propagate_results_second_order_ra_rate = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_second_order_ra_rate.setObjectName(u"label_dynamic_propagate_results_second_order_ra_rate")
-        self.label_dynamic_propagate_results_second_order_ra_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_second_order_ra_rate, 4, 6, 1, 1)
-
-        self.label_dynamic_propagate_results_first_order_ra_rate = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_results_first_order_ra_rate.setObjectName(u"label_dynamic_propagate_results_first_order_ra_rate")
-        self.label_dynamic_propagate_results_first_order_ra_rate.setAlignment(Qt.AlignCenter)
-
-        self.grid_layout_propagate_results.addWidget(self.label_dynamic_propagate_results_first_order_ra_rate, 4, 1, 1, 1)
+        self.grid_layout_propagate_results.addWidget(
+            self.label_static_propagate_results_first_order, 1, 1, 1, 4
+        )
+
+        self.label_dynamic_propagate_results_first_order_dec_error = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_first_order_dec_error.setObjectName(
+            "label_dynamic_propagate_results_first_order_dec_error"
+        )
+        self.label_dynamic_propagate_results_first_order_dec_error.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_first_order_dec_error, 4, 4, 1, 1
+        )
+
+        self.label_dynamic_propagate_results_first_order_dec_rate = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_first_order_dec_rate.setObjectName(
+            "label_dynamic_propagate_results_first_order_dec_rate"
+        )
+        self.label_dynamic_propagate_results_first_order_dec_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_first_order_dec_rate, 4, 3, 1, 1
+        )
+
+        self.label_dynamic_propagate_results_second_order_ra_rate = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_second_order_ra_rate.setObjectName(
+            "label_dynamic_propagate_results_second_order_ra_rate"
+        )
+        self.label_dynamic_propagate_results_second_order_ra_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_second_order_ra_rate, 4, 6, 1, 1
+        )
+
+        self.label_dynamic_propagate_results_first_order_ra_rate = QLabel(
+            self.verticalLayoutWidget_7
+        )
+        self.label_dynamic_propagate_results_first_order_ra_rate.setObjectName(
+            "label_dynamic_propagate_results_first_order_ra_rate"
+        )
+        self.label_dynamic_propagate_results_first_order_ra_rate.setAlignment(
+            Qt.AlignCenter
+        )
+
+        self.grid_layout_propagate_results.addWidget(
+            self.label_dynamic_propagate_results_first_order_ra_rate, 4, 1, 1, 1
+        )
 
         self.line_20 = QFrame(self.verticalLayoutWidget_7)
-        self.line_20.setObjectName(u"line_20")
+        self.line_20.setObjectName("line_20")
         self.line_20.setFrameShape(QFrame.HLine)
         self.line_20.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_propagate_results.addWidget(self.line_20, 3, 1, 1, 4)
 
         self.line_21 = QFrame(self.verticalLayoutWidget_7)
-        self.line_21.setObjectName(u"line_21")
+        self.line_21.setObjectName("line_21")
         self.line_21.setFrameShape(QFrame.HLine)
         self.line_21.setFrameShadow(QFrame.Sunken)
 
         self.grid_layout_propagate_results.addWidget(self.line_21, 3, 6, 1, 4)
 
-
         self.vertical_layout_propagate.addLayout(self.grid_layout_propagate_results)
 
         self.line_25 = QFrame(self.verticalLayoutWidget_7)
-        self.line_25.setObjectName(u"line_25")
+        self.line_25.setObjectName("line_25")
         self.line_25.setFrameShape(QFrame.HLine)
         self.line_25.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_propagate.addWidget(self.line_25)
 
         self.horizontal_layout_propagate_forward = QHBoxLayout()
-        self.horizontal_layout_propagate_forward.setObjectName(u"horizontal_layout_propagate_forward")
-        self.combo_box_propagate_forward_datetime = QDateTimeEdit(self.verticalLayoutWidget_7)
-        self.combo_box_propagate_forward_datetime.setObjectName(u"combo_box_propagate_forward_datetime")
+        self.horizontal_layout_propagate_forward.setObjectName(
+            "horizontal_layout_propagate_forward"
+        )
+        self.combo_box_propagate_forward_datetime = QDateTimeEdit(
+            self.verticalLayoutWidget_7
+        )
+        self.combo_box_propagate_forward_datetime.setObjectName(
+            "combo_box_propagate_forward_datetime"
+        )
         self.combo_box_propagate_forward_datetime.setMinimumSize(QSize(200, 0))
-        self.combo_box_propagate_forward_datetime.setMaximumSize(QSize(16777213, 16777215))
-
-        self.horizontal_layout_propagate_forward.addWidget(self.combo_box_propagate_forward_datetime)
-
-        self.combo_box_propagate_forward_timezone = QComboBox(self.verticalLayoutWidget_7)
+        self.combo_box_propagate_forward_datetime.setMaximumSize(
+            QSize(16777213, 16777215)
+        )
+
+        self.horizontal_layout_propagate_forward.addWidget(
+            self.combo_box_propagate_forward_datetime
+        )
+
+        self.combo_box_propagate_forward_timezone = QComboBox(
+            self.verticalLayoutWidget_7
+        )
         self.combo_box_propagate_forward_timezone.addItem("")
         self.combo_box_propagate_forward_timezone.addItem("")
-        self.combo_box_propagate_forward_timezone.setObjectName(u"combo_box_propagate_forward_timezone")
-
-        self.horizontal_layout_propagate_forward.addWidget(self.combo_box_propagate_forward_timezone)
-
-        self.push_button_propagate_forward_solve = QPushButton(self.verticalLayoutWidget_7)
-        self.push_button_propagate_forward_solve.setObjectName(u"push_button_propagate_forward_solve")
-
-        self.horizontal_layout_propagate_forward.addWidget(self.push_button_propagate_forward_solve)
+        self.combo_box_propagate_forward_timezone.setObjectName(
+            "combo_box_propagate_forward_timezone"
+        )
+
+        self.horizontal_layout_propagate_forward.addWidget(
+            self.combo_box_propagate_forward_timezone
+        )
+
+        self.push_button_propagate_forward_solve = QPushButton(
+            self.verticalLayoutWidget_7
+        )
+        self.push_button_propagate_forward_solve.setObjectName(
+            "push_button_propagate_forward_solve"
+        )
+
+        self.horizontal_layout_propagate_forward.addWidget(
+            self.push_button_propagate_forward_solve
+        )
 
         self.line_24 = QFrame(self.verticalLayoutWidget_7)
-        self.line_24.setObjectName(u"line_24")
+        self.line_24.setObjectName("line_24")
         self.line_24.setFrameShape(QFrame.VLine)
         self.line_24.setFrameShadow(QFrame.Sunken)
 
         self.horizontal_layout_propagate_forward.addWidget(self.line_24)
 
         self.label_dynamic_propagate_forward_ra = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_forward_ra.setObjectName(u"label_dynamic_propagate_forward_ra")
+        self.label_dynamic_propagate_forward_ra.setObjectName(
+            "label_dynamic_propagate_forward_ra"
+        )
         self.label_dynamic_propagate_forward_ra.setAlignment(Qt.AlignCenter)
 
-        self.horizontal_layout_propagate_forward.addWidget(self.label_dynamic_propagate_forward_ra)
+        self.horizontal_layout_propagate_forward.addWidget(
+            self.label_dynamic_propagate_forward_ra
+        )
 
         self.label_dynamic_propagate_forward_dec = QLabel(self.verticalLayoutWidget_7)
-        self.label_dynamic_propagate_forward_dec.setObjectName(u"label_dynamic_propagate_forward_dec")
+        self.label_dynamic_propagate_forward_dec.setObjectName(
+            "label_dynamic_propagate_forward_dec"
+        )
         self.label_dynamic_propagate_forward_dec.setAlignment(Qt.AlignCenter)
 
-        self.horizontal_layout_propagate_forward.addWidget(self.label_dynamic_propagate_forward_dec)
-
-
-        self.vertical_layout_propagate.addLayout(self.horizontal_layout_propagate_forward)
+        self.horizontal_layout_propagate_forward.addWidget(
+            self.label_dynamic_propagate_forward_dec
+        )
+
+        self.vertical_layout_propagate.addLayout(
+            self.horizontal_layout_propagate_forward
+        )
 
         self.tab_widget_solutions.addTab(self.tab_propagate, "")
 
         self.vertical_layout_window.addWidget(self.tab_widget_solutions)
 
         ManualWindow.setCentralWidget(self.central_widget)
 
         self.retranslateUi(ManualWindow)
 
         self.tab_widget_solutions.setCurrentIndex(0)
 
-
         QMetaObject.connectSlotsByName(ManualWindow)
+
     # setupUi
 
     def retranslateUi(self, ManualWindow):
-        ManualWindow.setWindowTitle(QCoreApplication.translate("ManualWindow", u"OpihiExarata Manual Mode", None))
-        self.label_static_dummy_opihi_navbar.setText(QCoreApplication.translate("ManualWindow", u"DUMMY OPIHI IMAGE NAVIGATION BAR", None))
-        self.label_dynamic_target_4_pixel_location.setText(QCoreApplication.translate("ManualWindow", u"(XXXX, YYYY)", None))
-        self.label_static_target_3_location.setText(QCoreApplication.translate("ManualWindow", u"Target 3 Location:", None))
-        self.label_static_target_4_location.setText(QCoreApplication.translate("ManualWindow", u"Target 4 Location:", None))
-        self.push_button_relocate_target_location_1.setText(QCoreApplication.translate("ManualWindow", u"Relocate", None))
-        self.label_dynamic_target_1_pixel_location.setText(QCoreApplication.translate("ManualWindow", u"(XXXX, YYYY)", None))
-        self.push_button_load_filename_3.setText(QCoreApplication.translate("ManualWindow", u"Load", None))
-        self.label_dynamic_filename_3.setText(QCoreApplication.translate("ManualWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None))
-        self.label_dynamic_filename_1.setText(QCoreApplication.translate("ManualWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None))
-        self.label_dynamic_filename_2.setText(QCoreApplication.translate("ManualWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None))
-        self.label_dynamic_filename_4.setText(QCoreApplication.translate("ManualWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None))
-        self.radio_button_primary_file_3.setText(QCoreApplication.translate("ManualWindow", u"3", None))
-        self.radio_button_primary_file_4.setText(QCoreApplication.translate("ManualWindow", u"4", None))
-        self.label_dynamic_target_2_pixel_location.setText(QCoreApplication.translate("ManualWindow", u"(XXXX, YYYY)", None))
-        self.push_button_relocate_target_location_3.setText(QCoreApplication.translate("ManualWindow", u"Relocate", None))
-        self.radio_button_primary_file_1.setText(QCoreApplication.translate("ManualWindow", u"1", None))
-        self.label_dynamic_target_3_pixel_location.setText(QCoreApplication.translate("ManualWindow", u"(XXXX, YYYY)", None))
-        self.radio_button_primary_file_2.setText(QCoreApplication.translate("ManualWindow", u"2", None))
-        self.label_static_target_2_location.setText(QCoreApplication.translate("ManualWindow", u"Target 2 Location:", None))
-        self.push_button_relocate_target_location_2.setText(QCoreApplication.translate("ManualWindow", u"Relocate", None))
-        self.push_button_load_filename_1.setText(QCoreApplication.translate("ManualWindow", u"Load", None))
-        self.push_button_load_filename_2.setText(QCoreApplication.translate("ManualWindow", u"Load", None))
-        self.label_static_target_1_location.setText(QCoreApplication.translate("ManualWindow", u"Target 1 Location:", None))
-        self.push_button_load_filename_4.setText(QCoreApplication.translate("ManualWindow", u"Load", None))
-        self.push_button_relocate_target_location_4.setText(QCoreApplication.translate("ManualWindow", u"Relocate", None))
-        self.push_button_force_reset.setText(QCoreApplication.translate("ManualWindow", u"Reset", None))
-        self.push_button_save_and_reset.setText(QCoreApplication.translate("ManualWindow", u"Save && Reset", None))
-        self.label_static_detected_target_name.setText(QCoreApplication.translate("ManualWindow", u"(Detected) Target Name", None))
-        self.push_button_change_target_name.setText(QCoreApplication.translate("ManualWindow", u"Change", None))
-        self.push_button_send_target_to_tcs.setText(QCoreApplication.translate("ManualWindow", u"Send Target to TCS", None))
-        self.label.setText(QCoreApplication.translate("ManualWindow", u"TextLabel", None))
-        self.tab_widget_solutions.setTabText(self.tab_widget_solutions.indexOf(self.tab_summary), QCoreApplication.translate("ManualWindow", u"Summary", None))
-        self.label_static_astrometry_engine.setText(QCoreApplication.translate("ManualWindow", u"Astrometry Engine", None))
-        self.combo_box_astrometry_engine.setItemText(0, QCoreApplication.translate("ManualWindow", u"Astrometry.net Nova", None))
-        self.combo_box_astrometry_engine.setItemText(1, QCoreApplication.translate("ManualWindow", u"Astrometry.net Host", None))
-
-        self.push_button_solve_astrometry.setText(QCoreApplication.translate("ManualWindow", u"Solve Astrometry", None))
-        self.label_static_astrometry_results_center_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.label_dynamic_astrometry_file_3_target_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_static_astrometry_results_center_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_dynamic_astrometry_file_4_center_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_static_astrometry_results_center.setText(QCoreApplication.translate("ManualWindow", u"Center", None))
-        self.label_dynamic_astrometry_file_4_target_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_3_target_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_4_target_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_2_target_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_3_center_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_4_center_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_2_center_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_static_astrometry_results_target_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.label_static_astrometry_results_target_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_dynamic_astrometry_file_2_target_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_3_center_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_2_center_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_static_astrometry_results_target.setText(QCoreApplication.translate("ManualWindow", u"Target/Asteroid", None))
-        self.label_dynamic_astrometry_file_1_center_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_static_astrometry_results_file_1.setText(QCoreApplication.translate("ManualWindow", u"1", None))
-        self.label_dynamic_astrometry_file_1_target_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.label_dynamic_astrometry_file_1_target_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_static_astrometry_results_file.setText(QCoreApplication.translate("ManualWindow", u"File", None))
-        self.label_dynamic_astrometry_file_1_center_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_static_astrometry_results_file_3.setText(QCoreApplication.translate("ManualWindow", u"3", None))
-        self.label_static_astrometry_results_file_2.setText(QCoreApplication.translate("ManualWindow", u"2", None))
-        self.label_static_astrometry_results_file_4.setText(QCoreApplication.translate("ManualWindow", u"4", None))
-        self.label_static_astrometry_custom_pixel_x.setText(QCoreApplication.translate("ManualWindow", u"Pixel X", None))
-        self.label_static_astrometry_coordinate_solve.setText(QCoreApplication.translate("ManualWindow", u"Coordinate Solve", None))
-        self.label_static_astrometry_custom_pixel_y.setText(QCoreApplication.translate("ManualWindow", u"Pixel Y", None))
-        self.label_static_astrometry_custom_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_static_astrometry_custom_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.push_button_astrometry_custom_solve.setText(QCoreApplication.translate("ManualWindow", u"Solve", None))
-        self.tab_widget_solutions.setTabText(self.tab_widget_solutions.indexOf(self.tab_astrometry), QCoreApplication.translate("ManualWindow", u"Astrometry", None))
-        self.label_static_photometry_engine.setText(QCoreApplication.translate("ManualWindow", u"Photometry Engine", None))
-        self.combo_box_photometry_engine.setItemText(0, QCoreApplication.translate("ManualWindow", u"Pan-STARRS 3pi DR2 MAST", None))
-
-        self.push_button_solve_photometry.setText(QCoreApplication.translate("ManualWindow", u"Solve Photometry", None))
-        self.label_static_photometry_results_file_1.setText(QCoreApplication.translate("ManualWindow", u"1", None))
-        self.label_static_photometry_results_file.setText(QCoreApplication.translate("ManualWindow", u"File", None))
-        self.label_static_photometry_results_file_2.setText(QCoreApplication.translate("ManualWindow", u"2", None))
-        self.label_static_photometry_results_file_4.setText(QCoreApplication.translate("ManualWindow", u"4", None))
-        self.label_static_photometry_results_file_3.setText(QCoreApplication.translate("ManualWindow", u"3", None))
-        self.label_static_photometry_results_zero_point.setText(QCoreApplication.translate("ManualWindow", u"Zero Point", None))
-        self.label_static_photometry_results_file_2_filter_name.setText(QCoreApplication.translate("ManualWindow", u"FF", None))
-        self.label_static_photometry_results_aperture_magnitude.setText(QCoreApplication.translate("ManualWindow", u"Aperture Magnitude", None))
-        self.label_static_photometry_results_filter_name.setText(QCoreApplication.translate("ManualWindow", u"Filter Name", None))
-        self.label_static_photometry_results_file_4_filter_name.setText(QCoreApplication.translate("ManualWindow", u"FF", None))
-        self.label_static_photometry_results_file_1_filter_name.setText(QCoreApplication.translate("ManualWindow", u"FF", None))
-        self.label_static_photometry_results_file_3_filter_name.setText(QCoreApplication.translate("ManualWindow", u"FF", None))
-        self.label_static_photometry_results_file_1_zero_point.setText(QCoreApplication.translate("ManualWindow", u"ZZ.ZZZ + E.EEE", None))
-        self.label_static_photometry_results_file_4_zero_point.setText(QCoreApplication.translate("ManualWindow", u"ZZ.ZZZ + E.EEE", None))
-        self.label_static_photometry_results_file_2_zero_point.setText(QCoreApplication.translate("ManualWindow", u"ZZ.ZZZ + E.EEE", None))
-        self.label_static_photometry_results_file_3_zero_point.setText(QCoreApplication.translate("ManualWindow", u"ZZ.ZZZ + E.EEE", None))
-        self.label_static_photometry_results_file_1_magnitude.setText(QCoreApplication.translate("ManualWindow", u"MM.MMM + E.EEE", None))
-        self.label_static_photometry_results_file_2_magnitude.setText(QCoreApplication.translate("ManualWindow", u"MM.MMM + E.EEE", None))
-        self.label_static_photometry_results_file_3_magnitude.setText(QCoreApplication.translate("ManualWindow", u"MM.MMM + E.EEE", None))
-        self.label_static_photometry_results_file_4_magnitude.setText(QCoreApplication.translate("ManualWindow", u"MM.MMM + E.EEE", None))
-        self.tab_widget_solutions.setTabText(self.tab_widget_solutions.indexOf(self.tab_photometry), QCoreApplication.translate("ManualWindow", u"Photometry", None))
-        self.label_static_orbit_engine.setText(QCoreApplication.translate("ManualWindow", u"Orbit Engine", None))
-        self.combo_box_orbit_engine.setItemText(0, QCoreApplication.translate("ManualWindow", u"OrbFit", None))
-        self.combo_box_orbit_engine.setItemText(1, QCoreApplication.translate("ManualWindow", u"Custom Orbit", None))
-
-        self.push_button_solve_orbit.setText(QCoreApplication.translate("ManualWindow", u"Solve Orbit", None))
-        self.line_edit_orbit_results_ascending_node_error.setText(QCoreApplication.translate("ManualWindow", u"EE.EEEE", None))
-        self.line_edit_orbit_results_ascending_node_value.setText(QCoreApplication.translate("ManualWindow", u"VV.VVVV", None))
-        self.line_edit_orbit_results_mean_anomaly_value.setText(QCoreApplication.translate("ManualWindow", u"VV.VVVV", None))
-        self.line_edit_orbit_results_mean_anomaly_error.setText(QCoreApplication.translate("ManualWindow", u"EE.EEEE", None))
-        self.line_edit_orbit_results_epoch_value.setText(QCoreApplication.translate("ManualWindow", u"EEEEEEE.EEEEE", None))
-        self.label_static_orbit_results_value.setText(QCoreApplication.translate("ManualWindow", u"Value", None))
-        self.label_static_orbit_results_error.setText(QCoreApplication.translate("ManualWindow", u"\u00b1 Error", None))
-        self.label_static_orbit_results_semimajor_axis.setText(QCoreApplication.translate("ManualWindow", u"Semi-major Axis [AU]", None))
-        self.label_static_orbit_results_eccentricity.setText(QCoreApplication.translate("ManualWindow", u"Eccentricity [1]", None))
-        self.label_static_orbit_results_mean_anomaly.setText(QCoreApplication.translate("ManualWindow", u"Mean Anomaly [deg]", None))
-        self.label_static_orbit_results_inclination.setText(QCoreApplication.translate("ManualWindow", u"Inclination [deg]", None))
-        self.label_static_orbit_results_perihelion.setText(QCoreApplication.translate("ManualWindow", u"Perihelion [deg]", None))
-        self.line_edit_orbit_results_semimajor_axis_value.setText(QCoreApplication.translate("ManualWindow", u"VV.VVVV", None))
-        self.line_edit_orbit_results_perihelion_value.setText(QCoreApplication.translate("ManualWindow", u"VV.VVVV", None))
-        self.label_static_orbit_results_ascending_node.setText(QCoreApplication.translate("ManualWindow", u"Ascending Node [deg]", None))
-        self.label_static_orbit_results_epoch.setText(QCoreApplication.translate("ManualWindow", u"Epoch [JD]", None))
-        self.line_edit_orbit_results_inclination_value.setText(QCoreApplication.translate("ManualWindow", u"VV.VVVV", None))
-        self.line_edit_orbit_results_eccentricity_error.setText(QCoreApplication.translate("ManualWindow", u"EE.EEEE", None))
-        self.line_edit_orbit_results_inclination_error.setText(QCoreApplication.translate("ManualWindow", u"EE.EEEE", None))
-        self.line_edit_orbit_results_perihelion_error.setText(QCoreApplication.translate("ManualWindow", u"EE.EEEE", None))
-        self.line_edit_orbit_results_eccentricity_value.setText(QCoreApplication.translate("ManualWindow", u"VV.VVVV", None))
-        self.line_edit_orbit_results_semimajor_axis_error.setText(QCoreApplication.translate("ManualWindow", u"EE.EEEE", None))
-        self.tab_widget_solutions.setTabText(self.tab_widget_solutions.indexOf(self.tab_orbit), QCoreApplication.translate("ManualWindow", u"Orbit", None))
-        self.label_static_ephemeris_engine.setText(QCoreApplication.translate("ManualWindow", u"Ephemeris Engine", None))
-        self.combo_box_ephemeris_engine.setItemText(0, QCoreApplication.translate("ManualWindow", u"JPL Horizons", None))
-
-        self.push_button_solve_ephemeris.setText(QCoreApplication.translate("ManualWindow", u"Solve Ephemeris", None))
-        self.label_static_ephemeris_results_nonsiderial_rates.setText(QCoreApplication.translate("ManualWindow", u"Ephemeris Non-Siderial Rates", None))
-        self.push_button_ephemeris_results_update_tcs_rates.setText(QCoreApplication.translate("ManualWindow", u"Update TCS Rates", None))
-        self.label_dynamic_ephemeris_results_first_order_ra_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_static_ephemeris_results_second_order_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.label_static_ephemeris_results_first_order_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.label_static_ephemeris_results_second_order_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_static_ephemeris_results_second_order.setText(QCoreApplication.translate("ManualWindow", u"<html><head/><body><p>2nd Order [&quot;/s<span style=\" vertical-align:super;\">2</span>]</p></body></html>", None))
-        self.label_static_ephemeris_results_first_order_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_dynamic_ephemeris_results_second_order_ra_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_dynamic_ephemeris_results_second_order_dec_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_dynamic_ephemeris_results_second_order_dec_rate.setText(QCoreApplication.translate("ManualWindow", u"+AA.AAA", None))
-        self.label_static_ephemeris_results_first_order.setText(QCoreApplication.translate("ManualWindow", u"1st Order [\"/s]", None))
-        self.label_dynamic_ephemeris_results_first_order_dec_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_dynamic_ephemeris_results_first_order_dec_rate.setText(QCoreApplication.translate("ManualWindow", u"+VV.VVV", None))
-        self.label_dynamic_ephemeris_results_second_order_ra_rate.setText(QCoreApplication.translate("ManualWindow", u"+AA.AAA", None))
-        self.label_dynamic_ephemeris_results_first_order_ra_rate.setText(QCoreApplication.translate("ManualWindow", u"+VV.VVV", None))
-        self.combo_box_ephemeris_forward_datetime.setDisplayFormat(QCoreApplication.translate("ManualWindow", u"yyyy-MM-dd HH:mm:ss", None))
-        self.combo_box_ephemeris_forward_timezone.setItemText(0, QCoreApplication.translate("ManualWindow", u"UTC+00:00", None))
-        self.combo_box_ephemeris_forward_timezone.setItemText(1, QCoreApplication.translate("ManualWindow", u"HST-10:00", None))
-
-        self.push_button_ephemeris_forward_solve.setText(QCoreApplication.translate("ManualWindow", u"Forward Solve", None))
-        self.label_dynamic_ephemeris_forward_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_dynamic_ephemeris_forward_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.tab_widget_solutions.setTabText(self.tab_widget_solutions.indexOf(self.tab_ephemeris), QCoreApplication.translate("ManualWindow", u"Ephemeris", None))
-        self.label_static_propagate_engine.setText(QCoreApplication.translate("ManualWindow", u"Propagation Engine", None))
-        self.combo_box_propagate_engine.setItemText(0, QCoreApplication.translate("ManualWindow", u"Linear", None))
-        self.combo_box_propagate_engine.setItemText(1, QCoreApplication.translate("ManualWindow", u"Quadratic", None))
-
-        self.push_button_solve_propagation.setText(QCoreApplication.translate("ManualWindow", u"Solve Propagation", None))
-        self.label_static_propagate_results_nonsiderial_rates.setText(QCoreApplication.translate("ManualWindow", u"Propagation Non-Siderial Rates", None))
-        self.push_button_propagate_results_update_tcs_rates.setText(QCoreApplication.translate("ManualWindow", u"Update TCS Rates", None))
-        self.label_dynamic_propagate_results_first_order_ra_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_static_propagate_results_second_order_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.label_static_propagate_results_first_order_dec.setText(QCoreApplication.translate("ManualWindow", u"DEC", None))
-        self.label_static_propagate_results_second_order_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_static_propagate_results_second_order.setText(QCoreApplication.translate("ManualWindow", u"<html><head/><body><p>2nd Order [&quot;/s<span style=\" vertical-align:super;\">2</span>]</p></body></html>", None))
-        self.label_static_propagate_results_first_order_ra.setText(QCoreApplication.translate("ManualWindow", u"RA", None))
-        self.label_dynamic_propagate_results_second_order_ra_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_dynamic_propagate_results_second_order_dec_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_dynamic_propagate_results_second_order_dec_rate.setText(QCoreApplication.translate("ManualWindow", u"+AA.AAA", None))
-        self.label_static_propagate_results_first_order.setText(QCoreApplication.translate("ManualWindow", u"1st Order [\"/s]", None))
-        self.label_dynamic_propagate_results_first_order_dec_error.setText(QCoreApplication.translate("ManualWindow", u"+EE.EEEE", None))
-        self.label_dynamic_propagate_results_first_order_dec_rate.setText(QCoreApplication.translate("ManualWindow", u"+VV.VVV", None))
-        self.label_dynamic_propagate_results_second_order_ra_rate.setText(QCoreApplication.translate("ManualWindow", u"+AA.AAA", None))
-        self.label_dynamic_propagate_results_first_order_ra_rate.setText(QCoreApplication.translate("ManualWindow", u"+VV.VVV", None))
-        self.combo_box_propagate_forward_datetime.setDisplayFormat(QCoreApplication.translate("ManualWindow", u"yyyy-MM-dd HH:mm:ss", None))
-        self.combo_box_propagate_forward_timezone.setItemText(0, QCoreApplication.translate("ManualWindow", u"UTC+00:00", None))
-        self.combo_box_propagate_forward_timezone.setItemText(1, QCoreApplication.translate("ManualWindow", u"HST-10:00", None))
-
-        self.push_button_propagate_forward_solve.setText(QCoreApplication.translate("ManualWindow", u"Forward Solve", None))
-        self.label_dynamic_propagate_forward_ra.setText(QCoreApplication.translate("ManualWindow", u"HH:MM:SS.SS", None))
-        self.label_dynamic_propagate_forward_dec.setText(QCoreApplication.translate("ManualWindow", u"+DD:MM:SS.SS", None))
-        self.tab_widget_solutions.setTabText(self.tab_widget_solutions.indexOf(self.tab_propagate), QCoreApplication.translate("ManualWindow", u"Propagate", None))
-    # retranslateUi
+        ManualWindow.setWindowTitle(
+            QCoreApplication.translate("ManualWindow", "OpihiExarata Manual Mode", None)
+        )
+        self.label_static_dummy_opihi_navbar.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "DUMMY OPIHI IMAGE NAVIGATION BAR", None
+            )
+        )
+        self.label_dynamic_target_4_pixel_location.setText(
+            QCoreApplication.translate("ManualWindow", "(XXXX, YYYY)", None)
+        )
+        self.label_static_target_3_location.setText(
+            QCoreApplication.translate("ManualWindow", "Target 3 Location:", None)
+        )
+        self.label_static_target_4_location.setText(
+            QCoreApplication.translate("ManualWindow", "Target 4 Location:", None)
+        )
+        self.push_button_relocate_target_location_1.setText(
+            QCoreApplication.translate("ManualWindow", "Relocate", None)
+        )
+        self.label_dynamic_target_1_pixel_location.setText(
+            QCoreApplication.translate("ManualWindow", "(XXXX, YYYY)", None)
+        )
+        self.push_button_load_filename_3.setText(
+            QCoreApplication.translate("ManualWindow", "Load", None)
+        )
+        self.label_dynamic_filename_3.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None
+            )
+        )
+        self.label_dynamic_filename_1.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None
+            )
+        )
+        self.label_dynamic_filename_2.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None
+            )
+        )
+        self.label_dynamic_filename_4.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "opi.20XXA999.YYMMDD.AAAAAAAAAA.#####.a.fits", None
+            )
+        )
+        self.radio_button_primary_file_3.setText(
+            QCoreApplication.translate("ManualWindow", "3", None)
+        )
+        self.radio_button_primary_file_4.setText(
+            QCoreApplication.translate("ManualWindow", "4", None)
+        )
+        self.label_dynamic_target_2_pixel_location.setText(
+            QCoreApplication.translate("ManualWindow", "(XXXX, YYYY)", None)
+        )
+        self.push_button_relocate_target_location_3.setText(
+            QCoreApplication.translate("ManualWindow", "Relocate", None)
+        )
+        self.radio_button_primary_file_1.setText(
+            QCoreApplication.translate("ManualWindow", "1", None)
+        )
+        self.label_dynamic_target_3_pixel_location.setText(
+            QCoreApplication.translate("ManualWindow", "(XXXX, YYYY)", None)
+        )
+        self.radio_button_primary_file_2.setText(
+            QCoreApplication.translate("ManualWindow", "2", None)
+        )
+        self.label_static_target_2_location.setText(
+            QCoreApplication.translate("ManualWindow", "Target 2 Location:", None)
+        )
+        self.push_button_relocate_target_location_2.setText(
+            QCoreApplication.translate("ManualWindow", "Relocate", None)
+        )
+        self.push_button_load_filename_1.setText(
+            QCoreApplication.translate("ManualWindow", "Load", None)
+        )
+        self.push_button_load_filename_2.setText(
+            QCoreApplication.translate("ManualWindow", "Load", None)
+        )
+        self.label_static_target_1_location.setText(
+            QCoreApplication.translate("ManualWindow", "Target 1 Location:", None)
+        )
+        self.push_button_load_filename_4.setText(
+            QCoreApplication.translate("ManualWindow", "Load", None)
+        )
+        self.push_button_relocate_target_location_4.setText(
+            QCoreApplication.translate("ManualWindow", "Relocate", None)
+        )
+        self.push_button_force_reset.setText(
+            QCoreApplication.translate("ManualWindow", "Reset", None)
+        )
+        self.push_button_save_and_reset.setText(
+            QCoreApplication.translate("ManualWindow", "Save && Reset", None)
+        )
+        self.label_static_detected_target_name.setText(
+            QCoreApplication.translate("ManualWindow", "(Detected) Target Name", None)
+        )
+        self.push_button_change_target_name.setText(
+            QCoreApplication.translate("ManualWindow", "Change", None)
+        )
+        self.push_button_send_target_to_tcs.setText(
+            QCoreApplication.translate("ManualWindow", "Send Target to TCS", None)
+        )
+        self.label.setText(
+            QCoreApplication.translate("ManualWindow", "TextLabel", None)
+        )
+        self.tab_widget_solutions.setTabText(
+            self.tab_widget_solutions.indexOf(self.tab_summary),
+            QCoreApplication.translate("ManualWindow", "Summary", None),
+        )
+        self.label_static_astrometry_engine.setText(
+            QCoreApplication.translate("ManualWindow", "Astrometry Engine", None)
+        )
+        self.combo_box_astrometry_engine.setItemText(
+            0, QCoreApplication.translate("ManualWindow", "Astrometry.net Nova", None)
+        )
+        self.combo_box_astrometry_engine.setItemText(
+            1, QCoreApplication.translate("ManualWindow", "Astrometry.net Host", None)
+        )
+
+        self.push_button_solve_astrometry.setText(
+            QCoreApplication.translate("ManualWindow", "Solve Astrometry", None)
+        )
+        self.label_static_astrometry_results_center_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.label_dynamic_astrometry_file_3_target_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_center_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_dynamic_astrometry_file_4_center_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_center.setText(
+            QCoreApplication.translate("ManualWindow", "Center", None)
+        )
+        self.label_dynamic_astrometry_file_4_target_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_3_target_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_4_target_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_2_target_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_3_center_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_4_center_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_2_center_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_target_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.label_static_astrometry_results_target_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_dynamic_astrometry_file_2_target_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_3_center_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_2_center_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_target.setText(
+            QCoreApplication.translate("ManualWindow", "Target/Asteroid", None)
+        )
+        self.label_dynamic_astrometry_file_1_center_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_file_1.setText(
+            QCoreApplication.translate("ManualWindow", "1", None)
+        )
+        self.label_dynamic_astrometry_file_1_target_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.label_dynamic_astrometry_file_1_target_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_file.setText(
+            QCoreApplication.translate("ManualWindow", "File", None)
+        )
+        self.label_dynamic_astrometry_file_1_center_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_static_astrometry_results_file_3.setText(
+            QCoreApplication.translate("ManualWindow", "3", None)
+        )
+        self.label_static_astrometry_results_file_2.setText(
+            QCoreApplication.translate("ManualWindow", "2", None)
+        )
+        self.label_static_astrometry_results_file_4.setText(
+            QCoreApplication.translate("ManualWindow", "4", None)
+        )
+        self.label_static_astrometry_custom_pixel_x.setText(
+            QCoreApplication.translate("ManualWindow", "Pixel X", None)
+        )
+        self.label_static_astrometry_coordinate_solve.setText(
+            QCoreApplication.translate("ManualWindow", "Coordinate Solve", None)
+        )
+        self.label_static_astrometry_custom_pixel_y.setText(
+            QCoreApplication.translate("ManualWindow", "Pixel Y", None)
+        )
+        self.label_static_astrometry_custom_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_static_astrometry_custom_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.push_button_astrometry_custom_solve.setText(
+            QCoreApplication.translate("ManualWindow", "Solve", None)
+        )
+        self.tab_widget_solutions.setTabText(
+            self.tab_widget_solutions.indexOf(self.tab_astrometry),
+            QCoreApplication.translate("ManualWindow", "Astrometry", None),
+        )
+        self.label_static_photometry_engine.setText(
+            QCoreApplication.translate("ManualWindow", "Photometry Engine", None)
+        )
+        self.combo_box_photometry_engine.setItemText(
+            0,
+            QCoreApplication.translate("ManualWindow", "Pan-STARRS 3pi DR2 MAST", None),
+        )
+
+        self.push_button_solve_photometry.setText(
+            QCoreApplication.translate("ManualWindow", "Solve Photometry", None)
+        )
+        self.label_static_photometry_results_file_1.setText(
+            QCoreApplication.translate("ManualWindow", "1", None)
+        )
+        self.label_static_photometry_results_file.setText(
+            QCoreApplication.translate("ManualWindow", "File", None)
+        )
+        self.label_static_photometry_results_file_2.setText(
+            QCoreApplication.translate("ManualWindow", "2", None)
+        )
+        self.label_static_photometry_results_file_4.setText(
+            QCoreApplication.translate("ManualWindow", "4", None)
+        )
+        self.label_static_photometry_results_file_3.setText(
+            QCoreApplication.translate("ManualWindow", "3", None)
+        )
+        self.label_static_photometry_results_zero_point.setText(
+            QCoreApplication.translate("ManualWindow", "Zero Point", None)
+        )
+        self.label_static_photometry_results_file_2_filter_name.setText(
+            QCoreApplication.translate("ManualWindow", "FF", None)
+        )
+        self.label_static_photometry_results_aperture_magnitude.setText(
+            QCoreApplication.translate("ManualWindow", "Aperture Magnitude", None)
+        )
+        self.label_static_photometry_results_filter_name.setText(
+            QCoreApplication.translate("ManualWindow", "Filter Name", None)
+        )
+        self.label_static_photometry_results_file_4_filter_name.setText(
+            QCoreApplication.translate("ManualWindow", "FF", None)
+        )
+        self.label_static_photometry_results_file_1_filter_name.setText(
+            QCoreApplication.translate("ManualWindow", "FF", None)
+        )
+        self.label_static_photometry_results_file_3_filter_name.setText(
+            QCoreApplication.translate("ManualWindow", "FF", None)
+        )
+        self.label_static_photometry_results_file_1_zero_point.setText(
+            QCoreApplication.translate("ManualWindow", "ZZ.ZZZ + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_4_zero_point.setText(
+            QCoreApplication.translate("ManualWindow", "ZZ.ZZZ + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_2_zero_point.setText(
+            QCoreApplication.translate("ManualWindow", "ZZ.ZZZ + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_3_zero_point.setText(
+            QCoreApplication.translate("ManualWindow", "ZZ.ZZZ + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_1_magnitude.setText(
+            QCoreApplication.translate("ManualWindow", "MM.MMM + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_2_magnitude.setText(
+            QCoreApplication.translate("ManualWindow", "MM.MMM + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_3_magnitude.setText(
+            QCoreApplication.translate("ManualWindow", "MM.MMM + E.EEE", None)
+        )
+        self.label_static_photometry_results_file_4_magnitude.setText(
+            QCoreApplication.translate("ManualWindow", "MM.MMM + E.EEE", None)
+        )
+        self.tab_widget_solutions.setTabText(
+            self.tab_widget_solutions.indexOf(self.tab_photometry),
+            QCoreApplication.translate("ManualWindow", "Photometry", None),
+        )
+        self.label_static_orbit_engine.setText(
+            QCoreApplication.translate("ManualWindow", "Orbit Engine", None)
+        )
+        self.combo_box_orbit_engine.setItemText(
+            0, QCoreApplication.translate("ManualWindow", "OrbFit", None)
+        )
+        self.combo_box_orbit_engine.setItemText(
+            1, QCoreApplication.translate("ManualWindow", "Custom Orbit", None)
+        )
+
+        self.push_button_solve_orbit.setText(
+            QCoreApplication.translate("ManualWindow", "Solve Orbit", None)
+        )
+        self.line_edit_orbit_results_ascending_node_error.setText(
+            QCoreApplication.translate("ManualWindow", "EE.EEEE", None)
+        )
+        self.line_edit_orbit_results_ascending_node_value.setText(
+            QCoreApplication.translate("ManualWindow", "VV.VVVV", None)
+        )
+        self.line_edit_orbit_results_mean_anomaly_value.setText(
+            QCoreApplication.translate("ManualWindow", "VV.VVVV", None)
+        )
+        self.line_edit_orbit_results_mean_anomaly_error.setText(
+            QCoreApplication.translate("ManualWindow", "EE.EEEE", None)
+        )
+        self.line_edit_orbit_results_epoch_value.setText(
+            QCoreApplication.translate("ManualWindow", "EEEEEEE.EEEEE", None)
+        )
+        self.label_static_orbit_results_value.setText(
+            QCoreApplication.translate("ManualWindow", "Value", None)
+        )
+        self.label_static_orbit_results_error.setText(
+            QCoreApplication.translate("ManualWindow", "\u00b1 Error", None)
+        )
+        self.label_static_orbit_results_semimajor_axis.setText(
+            QCoreApplication.translate("ManualWindow", "Semi-major Axis [AU]", None)
+        )
+        self.label_static_orbit_results_eccentricity.setText(
+            QCoreApplication.translate("ManualWindow", "Eccentricity [1]", None)
+        )
+        self.label_static_orbit_results_mean_anomaly.setText(
+            QCoreApplication.translate("ManualWindow", "Mean Anomaly [deg]", None)
+        )
+        self.label_static_orbit_results_inclination.setText(
+            QCoreApplication.translate("ManualWindow", "Inclination [deg]", None)
+        )
+        self.label_static_orbit_results_perihelion.setText(
+            QCoreApplication.translate("ManualWindow", "Perihelion [deg]", None)
+        )
+        self.line_edit_orbit_results_semimajor_axis_value.setText(
+            QCoreApplication.translate("ManualWindow", "VV.VVVV", None)
+        )
+        self.line_edit_orbit_results_perihelion_value.setText(
+            QCoreApplication.translate("ManualWindow", "VV.VVVV", None)
+        )
+        self.label_static_orbit_results_ascending_node.setText(
+            QCoreApplication.translate("ManualWindow", "Ascending Node [deg]", None)
+        )
+        self.label_static_orbit_results_epoch.setText(
+            QCoreApplication.translate("ManualWindow", "Epoch [JD]", None)
+        )
+        self.line_edit_orbit_results_inclination_value.setText(
+            QCoreApplication.translate("ManualWindow", "VV.VVVV", None)
+        )
+        self.line_edit_orbit_results_eccentricity_error.setText(
+            QCoreApplication.translate("ManualWindow", "EE.EEEE", None)
+        )
+        self.line_edit_orbit_results_inclination_error.setText(
+            QCoreApplication.translate("ManualWindow", "EE.EEEE", None)
+        )
+        self.line_edit_orbit_results_perihelion_error.setText(
+            QCoreApplication.translate("ManualWindow", "EE.EEEE", None)
+        )
+        self.line_edit_orbit_results_eccentricity_value.setText(
+            QCoreApplication.translate("ManualWindow", "VV.VVVV", None)
+        )
+        self.line_edit_orbit_results_semimajor_axis_error.setText(
+            QCoreApplication.translate("ManualWindow", "EE.EEEE", None)
+        )
+        self.tab_widget_solutions.setTabText(
+            self.tab_widget_solutions.indexOf(self.tab_orbit),
+            QCoreApplication.translate("ManualWindow", "Orbit", None),
+        )
+        self.label_static_ephemeris_engine.setText(
+            QCoreApplication.translate("ManualWindow", "Ephemeris Engine", None)
+        )
+        self.combo_box_ephemeris_engine.setItemText(
+            0, QCoreApplication.translate("ManualWindow", "JPL Horizons", None)
+        )
+
+        self.push_button_solve_ephemeris.setText(
+            QCoreApplication.translate("ManualWindow", "Solve Ephemeris", None)
+        )
+        self.label_static_ephemeris_results_nonsiderial_rates.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "Ephemeris Non-Siderial Rates", None
+            )
+        )
+        self.push_button_ephemeris_results_update_tcs_rates.setText(
+            QCoreApplication.translate("ManualWindow", "Update TCS Rates", None)
+        )
+        self.label_dynamic_ephemeris_results_first_order_ra_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_static_ephemeris_results_second_order_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.label_static_ephemeris_results_first_order_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.label_static_ephemeris_results_second_order_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_static_ephemeris_results_second_order.setText(
+            QCoreApplication.translate(
+                "ManualWindow",
+                (
+                    '<html><head/><body><p>2nd Order [&quot;/s<span style="'
+                    ' vertical-align:super;">2</span>]</p></body></html>'
+                ),
+                None,
+            )
+        )
+        self.label_static_ephemeris_results_first_order_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_dynamic_ephemeris_results_second_order_ra_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_dynamic_ephemeris_results_second_order_dec_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_dynamic_ephemeris_results_second_order_dec_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+AA.AAA", None)
+        )
+        self.label_static_ephemeris_results_first_order.setText(
+            QCoreApplication.translate("ManualWindow", '1st Order ["/s]', None)
+        )
+        self.label_dynamic_ephemeris_results_first_order_dec_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_dynamic_ephemeris_results_first_order_dec_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+VV.VVV", None)
+        )
+        self.label_dynamic_ephemeris_results_second_order_ra_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+AA.AAA", None)
+        )
+        self.label_dynamic_ephemeris_results_first_order_ra_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+VV.VVV", None)
+        )
+        self.combo_box_ephemeris_forward_datetime.setDisplayFormat(
+            QCoreApplication.translate("ManualWindow", "yyyy-MM-dd HH:mm:ss", None)
+        )
+        self.combo_box_ephemeris_forward_timezone.setItemText(
+            0, QCoreApplication.translate("ManualWindow", "UTC+00:00", None)
+        )
+        self.combo_box_ephemeris_forward_timezone.setItemText(
+            1, QCoreApplication.translate("ManualWindow", "HST-10:00", None)
+        )
+
+        self.push_button_ephemeris_forward_solve.setText(
+            QCoreApplication.translate("ManualWindow", "Forward Solve", None)
+        )
+        self.label_dynamic_ephemeris_forward_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_dynamic_ephemeris_forward_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.tab_widget_solutions.setTabText(
+            self.tab_widget_solutions.indexOf(self.tab_ephemeris),
+            QCoreApplication.translate("ManualWindow", "Ephemeris", None),
+        )
+        self.label_static_propagate_engine.setText(
+            QCoreApplication.translate("ManualWindow", "Propagation Engine", None)
+        )
+        self.combo_box_propagate_engine.setItemText(
+            0, QCoreApplication.translate("ManualWindow", "Linear", None)
+        )
+        self.combo_box_propagate_engine.setItemText(
+            1, QCoreApplication.translate("ManualWindow", "Quadratic", None)
+        )
+
+        self.push_button_solve_propagation.setText(
+            QCoreApplication.translate("ManualWindow", "Solve Propagation", None)
+        )
+        self.label_static_propagate_results_nonsiderial_rates.setText(
+            QCoreApplication.translate(
+                "ManualWindow", "Propagation Non-Siderial Rates", None
+            )
+        )
+        self.push_button_propagate_results_update_tcs_rates.setText(
+            QCoreApplication.translate("ManualWindow", "Update TCS Rates", None)
+        )
+        self.label_dynamic_propagate_results_first_order_ra_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_static_propagate_results_second_order_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.label_static_propagate_results_first_order_dec.setText(
+            QCoreApplication.translate("ManualWindow", "DEC", None)
+        )
+        self.label_static_propagate_results_second_order_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_static_propagate_results_second_order.setText(
+            QCoreApplication.translate(
+                "ManualWindow",
+                (
+                    '<html><head/><body><p>2nd Order [&quot;/s<span style="'
+                    ' vertical-align:super;">2</span>]</p></body></html>'
+                ),
+                None,
+            )
+        )
+        self.label_static_propagate_results_first_order_ra.setText(
+            QCoreApplication.translate("ManualWindow", "RA", None)
+        )
+        self.label_dynamic_propagate_results_second_order_ra_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_dynamic_propagate_results_second_order_dec_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_dynamic_propagate_results_second_order_dec_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+AA.AAA", None)
+        )
+        self.label_static_propagate_results_first_order.setText(
+            QCoreApplication.translate("ManualWindow", '1st Order ["/s]', None)
+        )
+        self.label_dynamic_propagate_results_first_order_dec_error.setText(
+            QCoreApplication.translate("ManualWindow", "+EE.EEEE", None)
+        )
+        self.label_dynamic_propagate_results_first_order_dec_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+VV.VVV", None)
+        )
+        self.label_dynamic_propagate_results_second_order_ra_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+AA.AAA", None)
+        )
+        self.label_dynamic_propagate_results_first_order_ra_rate.setText(
+            QCoreApplication.translate("ManualWindow", "+VV.VVV", None)
+        )
+        self.combo_box_propagate_forward_datetime.setDisplayFormat(
+            QCoreApplication.translate("ManualWindow", "yyyy-MM-dd HH:mm:ss", None)
+        )
+        self.combo_box_propagate_forward_timezone.setItemText(
+            0, QCoreApplication.translate("ManualWindow", "UTC+00:00", None)
+        )
+        self.combo_box_propagate_forward_timezone.setItemText(
+            1, QCoreApplication.translate("ManualWindow", "HST-10:00", None)
+        )
+
+        self.push_button_propagate_forward_solve.setText(
+            QCoreApplication.translate("ManualWindow", "Forward Solve", None)
+        )
+        self.label_dynamic_propagate_forward_ra.setText(
+            QCoreApplication.translate("ManualWindow", "HH:MM:SS.SS", None)
+        )
+        self.label_dynamic_propagate_forward_dec.setText(
+            QCoreApplication.translate("ManualWindow", "+DD:MM:SS.SS", None)
+        )
+        self.tab_widget_solutions.setTabText(
+            self.tab_widget_solutions.indexOf(self.tab_propagate),
+            QCoreApplication.translate("ManualWindow", "Propagate", None),
+        )
 
+    # retranslateUi
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/qtui_selector.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/qtui_selector.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,259 +4,389 @@
 ## Form generated from reading UI file 'selector.ui'
 ##
 ## Created by: Qt User Interface Compiler version 6.4.2
 ##
 ## WARNING! All changes made in this file will be lost when recompiling UI file!
 ################################################################################
 
-from PySide6.QtCore import (QCoreApplication, QDate, QDateTime, QLocale,
-    QMetaObject, QObject, QPoint, QRect,
-    QSize, QTime, QUrl, Qt)
-from PySide6.QtGui import (QBrush, QColor, QConicalGradient, QCursor,
-    QFont, QFontDatabase, QGradient, QIcon,
-    QImage, QKeySequence, QLinearGradient, QPainter,
-    QPalette, QPixmap, QRadialGradient, QTransform)
-from PySide6.QtWidgets import (QApplication, QCheckBox, QFrame, QGraphicsView,
-    QGridLayout, QHBoxLayout, QLabel, QLineEdit,
-    QPushButton, QSizePolicy, QVBoxLayout, QWidget)
+from PySide6.QtCore import (
+    QCoreApplication,
+    QDate,
+    QDateTime,
+    QLocale,
+    QMetaObject,
+    QObject,
+    QPoint,
+    QRect,
+    QSize,
+    QTime,
+    QUrl,
+    Qt,
+)
+from PySide6.QtGui import (
+    QBrush,
+    QColor,
+    QConicalGradient,
+    QCursor,
+    QFont,
+    QFontDatabase,
+    QGradient,
+    QIcon,
+    QImage,
+    QKeySequence,
+    QLinearGradient,
+    QPainter,
+    QPalette,
+    QPixmap,
+    QRadialGradient,
+    QTransform,
+)
+from PySide6.QtWidgets import (
+    QApplication,
+    QCheckBox,
+    QFrame,
+    QGraphicsView,
+    QGridLayout,
+    QHBoxLayout,
+    QLabel,
+    QLineEdit,
+    QPushButton,
+    QSizePolicy,
+    QVBoxLayout,
+    QWidget,
+)
+
 
 class Ui_SelectorWindow(object):
     def setupUi(self, SelectorWindow):
         if not SelectorWindow.objectName():
-            SelectorWindow.setObjectName(u"SelectorWindow")
+            SelectorWindow.setObjectName("SelectorWindow")
         SelectorWindow.resize(623, 868)
         self.verticalLayoutWidget = QWidget(SelectorWindow)
-        self.verticalLayoutWidget.setObjectName(u"verticalLayoutWidget")
+        self.verticalLayoutWidget.setObjectName("verticalLayoutWidget")
         self.verticalLayoutWidget.setGeometry(QRect(10, 10, 604, 846))
         font = QFont()
-        font.setFamilies([u"Cantarell"])
+        font.setFamilies(["Cantarell"])
         font.setPointSize(12)
         self.verticalLayoutWidget.setFont(font)
         self.vertical_layout_selector = QVBoxLayout(self.verticalLayoutWidget)
-        self.vertical_layout_selector.setObjectName(u"vertical_layout_selector")
+        self.vertical_layout_selector.setObjectName("vertical_layout_selector")
         self.vertical_layout_selector.setContentsMargins(0, 0, 0, 0)
         self.grid_layout_file_selection = QGridLayout()
-        self.grid_layout_file_selection.setObjectName(u"grid_layout_file_selection")
+        self.grid_layout_file_selection.setObjectName("grid_layout_file_selection")
         self.label_dynamic_current_fits_filename = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_current_fits_filename.setObjectName(u"label_dynamic_current_fits_filename")
+        self.label_dynamic_current_fits_filename.setObjectName(
+            "label_dynamic_current_fits_filename"
+        )
         self.label_dynamic_current_fits_filename.setMinimumSize(QSize(400, 0))
         font1 = QFont()
-        font1.setFamilies([u"Cantarell"])
+        font1.setFamilies(["Cantarell"])
         self.label_dynamic_current_fits_filename.setFont(font1)
 
-        self.grid_layout_file_selection.addWidget(self.label_dynamic_current_fits_filename, 0, 1, 1, 1)
+        self.grid_layout_file_selection.addWidget(
+            self.label_dynamic_current_fits_filename, 0, 1, 1, 1
+        )
 
         self.label_dynamic_reference_fits_filename = QLabel(self.verticalLayoutWidget)
-        self.label_dynamic_reference_fits_filename.setObjectName(u"label_dynamic_reference_fits_filename")
+        self.label_dynamic_reference_fits_filename.setObjectName(
+            "label_dynamic_reference_fits_filename"
+        )
         self.label_dynamic_reference_fits_filename.setMinimumSize(QSize(400, 0))
         self.label_dynamic_reference_fits_filename.setFont(font1)
 
-        self.grid_layout_file_selection.addWidget(self.label_dynamic_reference_fits_filename, 1, 1, 1, 1)
-
-        self.push_button_change_reference_filename = QPushButton(self.verticalLayoutWidget)
-        self.push_button_change_reference_filename.setObjectName(u"push_button_change_reference_filename")
+        self.grid_layout_file_selection.addWidget(
+            self.label_dynamic_reference_fits_filename, 1, 1, 1, 1
+        )
+
+        self.push_button_change_reference_filename = QPushButton(
+            self.verticalLayoutWidget
+        )
+        self.push_button_change_reference_filename.setObjectName(
+            "push_button_change_reference_filename"
+        )
         self.push_button_change_reference_filename.setFont(font1)
 
-        self.grid_layout_file_selection.addWidget(self.push_button_change_reference_filename, 1, 2, 1, 1)
+        self.grid_layout_file_selection.addWidget(
+            self.push_button_change_reference_filename, 1, 2, 1, 1
+        )
 
         self.label_static_current_fits_filename = QLabel(self.verticalLayoutWidget)
-        self.label_static_current_fits_filename.setObjectName(u"label_static_current_fits_filename")
+        self.label_static_current_fits_filename.setObjectName(
+            "label_static_current_fits_filename"
+        )
         self.label_static_current_fits_filename.setFont(font1)
 
-        self.grid_layout_file_selection.addWidget(self.label_static_current_fits_filename, 0, 0, 1, 1)
+        self.grid_layout_file_selection.addWidget(
+            self.label_static_current_fits_filename, 0, 0, 1, 1
+        )
 
         self.label_static_reference_fits_filename = QLabel(self.verticalLayoutWidget)
-        self.label_static_reference_fits_filename.setObjectName(u"label_static_reference_fits_filename")
+        self.label_static_reference_fits_filename.setObjectName(
+            "label_static_reference_fits_filename"
+        )
         self.label_static_reference_fits_filename.setFont(font1)
 
-        self.grid_layout_file_selection.addWidget(self.label_static_reference_fits_filename, 1, 0, 1, 1)
-
+        self.grid_layout_file_selection.addWidget(
+            self.label_static_reference_fits_filename, 1, 0, 1, 1
+        )
 
         self.vertical_layout_selector.addLayout(self.grid_layout_file_selection)
 
         self.line_2 = QFrame(self.verticalLayoutWidget)
-        self.line_2.setObjectName(u"line_2")
+        self.line_2.setObjectName("line_2")
         self.line_2.setFont(font1)
         self.line_2.setFrameShape(QFrame.HLine)
         self.line_2.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_selector.addWidget(self.line_2)
 
         self.vertical_layout_image = QVBoxLayout()
-        self.vertical_layout_image.setObjectName(u"vertical_layout_image")
+        self.vertical_layout_image.setObjectName("vertical_layout_image")
         self.dummy_selector_image = QGraphicsView(self.verticalLayoutWidget)
-        self.dummy_selector_image.setObjectName(u"dummy_selector_image")
+        self.dummy_selector_image.setObjectName("dummy_selector_image")
         self.dummy_selector_image.setMinimumSize(QSize(600, 600))
         self.dummy_selector_image.setMaximumSize(QSize(600, 600))
         self.dummy_selector_image.setFont(font1)
 
         self.vertical_layout_image.addWidget(self.dummy_selector_image)
 
         self.dummy_selector_navbar = QLabel(self.verticalLayoutWidget)
-        self.dummy_selector_navbar.setObjectName(u"dummy_selector_navbar")
+        self.dummy_selector_navbar.setObjectName("dummy_selector_navbar")
         self.dummy_selector_navbar.setMinimumSize(QSize(0, 25))
         self.dummy_selector_navbar.setMaximumSize(QSize(16777215, 25))
         self.dummy_selector_navbar.setFont(font1)
         self.dummy_selector_navbar.setAlignment(Qt.AlignCenter)
 
         self.vertical_layout_image.addWidget(self.dummy_selector_navbar)
 
-
         self.vertical_layout_selector.addLayout(self.vertical_layout_image)
 
         self.horizonta_layout_subtraction_mode = QHBoxLayout()
-        self.horizonta_layout_subtraction_mode.setObjectName(u"horizonta_layout_subtraction_mode")
+        self.horizonta_layout_subtraction_mode.setObjectName(
+            "horizonta_layout_subtraction_mode"
+        )
         self.label_static_subtraction_mode = QLabel(self.verticalLayoutWidget)
-        self.label_static_subtraction_mode.setObjectName(u"label_static_subtraction_mode")
+        self.label_static_subtraction_mode.setObjectName(
+            "label_static_subtraction_mode"
+        )
         self.label_static_subtraction_mode.setFont(font1)
 
-        self.horizonta_layout_subtraction_mode.addWidget(self.label_static_subtraction_mode)
+        self.horizonta_layout_subtraction_mode.addWidget(
+            self.label_static_subtraction_mode
+        )
 
         self.line_3 = QFrame(self.verticalLayoutWidget)
-        self.line_3.setObjectName(u"line_3")
+        self.line_3.setObjectName("line_3")
         self.line_3.setFont(font1)
         self.line_3.setFrameShape(QFrame.VLine)
         self.line_3.setFrameShadow(QFrame.Sunken)
 
         self.horizonta_layout_subtraction_mode.addWidget(self.line_3)
 
         self.push_button_mode_none = QPushButton(self.verticalLayoutWidget)
-        self.push_button_mode_none.setObjectName(u"push_button_mode_none")
+        self.push_button_mode_none.setObjectName("push_button_mode_none")
         self.push_button_mode_none.setFont(font1)
 
         self.horizonta_layout_subtraction_mode.addWidget(self.push_button_mode_none)
 
         self.push_button_mode_reference = QPushButton(self.verticalLayoutWidget)
-        self.push_button_mode_reference.setObjectName(u"push_button_mode_reference")
+        self.push_button_mode_reference.setObjectName("push_button_mode_reference")
         self.push_button_mode_reference.setFont(font1)
 
-        self.horizonta_layout_subtraction_mode.addWidget(self.push_button_mode_reference)
+        self.horizonta_layout_subtraction_mode.addWidget(
+            self.push_button_mode_reference
+        )
 
         self.push_button_mode_sidereal = QPushButton(self.verticalLayoutWidget)
-        self.push_button_mode_sidereal.setObjectName(u"push_button_mode_sidereal")
+        self.push_button_mode_sidereal.setObjectName("push_button_mode_sidereal")
         self.push_button_mode_sidereal.setFont(font1)
 
         self.horizonta_layout_subtraction_mode.addWidget(self.push_button_mode_sidereal)
 
         self.push_button_mode_non_sidereal = QPushButton(self.verticalLayoutWidget)
-        self.push_button_mode_non_sidereal.setObjectName(u"push_button_mode_non_sidereal")
+        self.push_button_mode_non_sidereal.setObjectName(
+            "push_button_mode_non_sidereal"
+        )
         self.push_button_mode_non_sidereal.setFont(font1)
 
-        self.horizonta_layout_subtraction_mode.addWidget(self.push_button_mode_non_sidereal)
-
+        self.horizonta_layout_subtraction_mode.addWidget(
+            self.push_button_mode_non_sidereal
+        )
 
         self.vertical_layout_selector.addLayout(self.horizonta_layout_subtraction_mode)
 
         self.horizontal_layout_colorbar_scale = QHBoxLayout()
-        self.horizontal_layout_colorbar_scale.setObjectName(u"horizontal_layout_colorbar_scale")
+        self.horizontal_layout_colorbar_scale.setObjectName(
+            "horizontal_layout_colorbar_scale"
+        )
         self.label_static_scale = QLabel(self.verticalLayoutWidget)
-        self.label_static_scale.setObjectName(u"label_static_scale")
+        self.label_static_scale.setObjectName("label_static_scale")
         self.label_static_scale.setFont(font1)
 
         self.horizontal_layout_colorbar_scale.addWidget(self.label_static_scale)
 
         self.line_edit_dynamic_scale_low = QLineEdit(self.verticalLayoutWidget)
-        self.line_edit_dynamic_scale_low.setObjectName(u"line_edit_dynamic_scale_low")
+        self.line_edit_dynamic_scale_low.setObjectName("line_edit_dynamic_scale_low")
         self.line_edit_dynamic_scale_low.setFont(font1)
 
-        self.horizontal_layout_colorbar_scale.addWidget(self.line_edit_dynamic_scale_low)
+        self.horizontal_layout_colorbar_scale.addWidget(
+            self.line_edit_dynamic_scale_low
+        )
 
         self.line_edit_dynamic_scale_high = QLineEdit(self.verticalLayoutWidget)
-        self.line_edit_dynamic_scale_high.setObjectName(u"line_edit_dynamic_scale_high")
+        self.line_edit_dynamic_scale_high.setObjectName("line_edit_dynamic_scale_high")
         self.line_edit_dynamic_scale_high.setFont(font1)
 
-        self.horizontal_layout_colorbar_scale.addWidget(self.line_edit_dynamic_scale_high)
+        self.horizontal_layout_colorbar_scale.addWidget(
+            self.line_edit_dynamic_scale_high
+        )
 
         self.push_button_scale_1_99 = QPushButton(self.verticalLayoutWidget)
-        self.push_button_scale_1_99.setObjectName(u"push_button_scale_1_99")
+        self.push_button_scale_1_99.setObjectName("push_button_scale_1_99")
         self.push_button_scale_1_99.setFont(font1)
 
         self.horizontal_layout_colorbar_scale.addWidget(self.push_button_scale_1_99)
 
         self.check_box_autoscale_1_99 = QCheckBox(self.verticalLayoutWidget)
-        self.check_box_autoscale_1_99.setObjectName(u"check_box_autoscale_1_99")
+        self.check_box_autoscale_1_99.setObjectName("check_box_autoscale_1_99")
         self.check_box_autoscale_1_99.setFont(font1)
         self.check_box_autoscale_1_99.setChecked(True)
 
         self.horizontal_layout_colorbar_scale.addWidget(self.check_box_autoscale_1_99)
 
         self.check_box_reverse_colorbar = QCheckBox(self.verticalLayoutWidget)
-        self.check_box_reverse_colorbar.setObjectName(u"check_box_reverse_colorbar")
+        self.check_box_reverse_colorbar.setObjectName("check_box_reverse_colorbar")
 
         self.horizontal_layout_colorbar_scale.addWidget(self.check_box_reverse_colorbar)
 
-
         self.vertical_layout_selector.addLayout(self.horizontal_layout_colorbar_scale)
 
         self.line = QFrame(self.verticalLayoutWidget)
-        self.line.setObjectName(u"line")
+        self.line.setObjectName("line")
         self.line.setFont(font)
         self.line.setFrameShape(QFrame.HLine)
         self.line.setFrameShadow(QFrame.Sunken)
 
         self.vertical_layout_selector.addWidget(self.line)
 
         self.horizontal_layout_target_pixel_entry = QHBoxLayout()
-        self.horizontal_layout_target_pixel_entry.setObjectName(u"horizontal_layout_target_pixel_entry")
+        self.horizontal_layout_target_pixel_entry.setObjectName(
+            "horizontal_layout_target_pixel_entry"
+        )
         self.label_static_target_x = QLabel(self.verticalLayoutWidget)
-        self.label_static_target_x.setObjectName(u"label_static_target_x")
+        self.label_static_target_x.setObjectName("label_static_target_x")
         self.label_static_target_x.setFont(font)
 
         self.horizontal_layout_target_pixel_entry.addWidget(self.label_static_target_x)
 
         self.line_edit_dynamic_target_x = QLineEdit(self.verticalLayoutWidget)
-        self.line_edit_dynamic_target_x.setObjectName(u"line_edit_dynamic_target_x")
+        self.line_edit_dynamic_target_x.setObjectName("line_edit_dynamic_target_x")
         self.line_edit_dynamic_target_x.setFont(font)
 
-        self.horizontal_layout_target_pixel_entry.addWidget(self.line_edit_dynamic_target_x)
+        self.horizontal_layout_target_pixel_entry.addWidget(
+            self.line_edit_dynamic_target_x
+        )
 
         self.label_static_target_y = QLabel(self.verticalLayoutWidget)
-        self.label_static_target_y.setObjectName(u"label_static_target_y")
+        self.label_static_target_y.setObjectName("label_static_target_y")
         self.label_static_target_y.setFont(font)
 
         self.horizontal_layout_target_pixel_entry.addWidget(self.label_static_target_y)
 
         self.line_edit_dynamic_target_y = QLineEdit(self.verticalLayoutWidget)
-        self.line_edit_dynamic_target_y.setObjectName(u"line_edit_dynamic_target_y")
+        self.line_edit_dynamic_target_y.setObjectName("line_edit_dynamic_target_y")
         self.line_edit_dynamic_target_y.setFont(font)
 
-        self.horizontal_layout_target_pixel_entry.addWidget(self.line_edit_dynamic_target_y)
+        self.horizontal_layout_target_pixel_entry.addWidget(
+            self.line_edit_dynamic_target_y
+        )
 
         self.push_button_submit_target = QPushButton(self.verticalLayoutWidget)
-        self.push_button_submit_target.setObjectName(u"push_button_submit_target")
+        self.push_button_submit_target.setObjectName("push_button_submit_target")
         self.push_button_submit_target.setFont(font)
 
-        self.horizontal_layout_target_pixel_entry.addWidget(self.push_button_submit_target)
-
-
-        self.vertical_layout_selector.addLayout(self.horizontal_layout_target_pixel_entry)
-
+        self.horizontal_layout_target_pixel_entry.addWidget(
+            self.push_button_submit_target
+        )
+
+        self.vertical_layout_selector.addLayout(
+            self.horizontal_layout_target_pixel_entry
+        )
 
         self.retranslateUi(SelectorWindow)
 
         QMetaObject.connectSlotsByName(SelectorWindow)
+
     # setupUi
 
     def retranslateUi(self, SelectorWindow):
-        SelectorWindow.setWindowTitle(QCoreApplication.translate("SelectorWindow", u"OpihiExarata Target Selector", None))
-        self.label_dynamic_current_fits_filename.setText(QCoreApplication.translate("SelectorWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAA.00001.a.fits", None))
-        self.label_dynamic_reference_fits_filename.setText(QCoreApplication.translate("SelectorWindow", u"opi.20XXA999.YYMMDD.AAAAAAAAA.00001.b.fits", None))
-        self.push_button_change_reference_filename.setText(QCoreApplication.translate("SelectorWindow", u"Change", None))
-        self.label_static_current_fits_filename.setText(QCoreApplication.translate("SelectorWindow", u"Current:", None))
-        self.label_static_reference_fits_filename.setText(QCoreApplication.translate("SelectorWindow", u"Reference:", None))
-        self.dummy_selector_navbar.setText(QCoreApplication.translate("SelectorWindow", u"DUMMY NAVIGATION BAR", None))
-        self.label_static_subtraction_mode.setText(QCoreApplication.translate("SelectorWindow", u"Subtraction Method", None))
-        self.push_button_mode_none.setText(QCoreApplication.translate("SelectorWindow", u"None", None))
-        self.push_button_mode_reference.setText(QCoreApplication.translate("SelectorWindow", u"Reference", None))
-        self.push_button_mode_sidereal.setText(QCoreApplication.translate("SelectorWindow", u"Sidereal", None))
-        self.push_button_mode_non_sidereal.setText(QCoreApplication.translate("SelectorWindow", u"Non-sidereal", None))
-        self.label_static_scale.setText(QCoreApplication.translate("SelectorWindow", u"Scale [Low High]", None))
-        self.push_button_scale_1_99.setText(QCoreApplication.translate("SelectorWindow", u"1 - 99 %", None))
-        self.check_box_autoscale_1_99.setText(QCoreApplication.translate("SelectorWindow", u"Auto", None))
-        self.check_box_reverse_colorbar.setText(QCoreApplication.translate("SelectorWindow", u"Reverse", None))
-        self.label_static_target_x.setText(QCoreApplication.translate("SelectorWindow", u"Target X:", None))
-        self.line_edit_dynamic_target_x.setText(QCoreApplication.translate("SelectorWindow", u"XXXX", None))
-        self.label_static_target_y.setText(QCoreApplication.translate("SelectorWindow", u"Target Y:", None))
-        self.line_edit_dynamic_target_y.setText(QCoreApplication.translate("SelectorWindow", u"YYYY", None))
-        self.push_button_submit_target.setText(QCoreApplication.translate("SelectorWindow", u"Submit", None))
-    # retranslateUi
+        SelectorWindow.setWindowTitle(
+            QCoreApplication.translate(
+                "SelectorWindow", "OpihiExarata Target Selector", None
+            )
+        )
+        self.label_dynamic_current_fits_filename.setText(
+            QCoreApplication.translate(
+                "SelectorWindow", "opi.20XXA999.YYMMDD.AAAAAAAAA.00001.a.fits", None
+            )
+        )
+        self.label_dynamic_reference_fits_filename.setText(
+            QCoreApplication.translate(
+                "SelectorWindow", "opi.20XXA999.YYMMDD.AAAAAAAAA.00001.b.fits", None
+            )
+        )
+        self.push_button_change_reference_filename.setText(
+            QCoreApplication.translate("SelectorWindow", "Change", None)
+        )
+        self.label_static_current_fits_filename.setText(
+            QCoreApplication.translate("SelectorWindow", "Current:", None)
+        )
+        self.label_static_reference_fits_filename.setText(
+            QCoreApplication.translate("SelectorWindow", "Reference:", None)
+        )
+        self.dummy_selector_navbar.setText(
+            QCoreApplication.translate("SelectorWindow", "DUMMY NAVIGATION BAR", None)
+        )
+        self.label_static_subtraction_mode.setText(
+            QCoreApplication.translate("SelectorWindow", "Subtraction Method", None)
+        )
+        self.push_button_mode_none.setText(
+            QCoreApplication.translate("SelectorWindow", "None", None)
+        )
+        self.push_button_mode_reference.setText(
+            QCoreApplication.translate("SelectorWindow", "Reference", None)
+        )
+        self.push_button_mode_sidereal.setText(
+            QCoreApplication.translate("SelectorWindow", "Sidereal", None)
+        )
+        self.push_button_mode_non_sidereal.setText(
+            QCoreApplication.translate("SelectorWindow", "Non-sidereal", None)
+        )
+        self.label_static_scale.setText(
+            QCoreApplication.translate("SelectorWindow", "Scale [Low High]", None)
+        )
+        self.push_button_scale_1_99.setText(
+            QCoreApplication.translate("SelectorWindow", "1 - 99 %", None)
+        )
+        self.check_box_autoscale_1_99.setText(
+            QCoreApplication.translate("SelectorWindow", "Auto", None)
+        )
+        self.check_box_reverse_colorbar.setText(
+            QCoreApplication.translate("SelectorWindow", "Reverse", None)
+        )
+        self.label_static_target_x.setText(
+            QCoreApplication.translate("SelectorWindow", "Target X:", None)
+        )
+        self.line_edit_dynamic_target_x.setText(
+            QCoreApplication.translate("SelectorWindow", "XXXX", None)
+        )
+        self.label_static_target_y.setText(
+            QCoreApplication.translate("SelectorWindow", "Target Y:", None)
+        )
+        self.line_edit_dynamic_target_y.setText(
+            QCoreApplication.translate("SelectorWindow", "YYYY", None)
+        )
+        self.push_button_submit_target.setText(
+            QCoreApplication.translate("SelectorWindow", "Submit", None)
+        )
 
+    # retranslateUi
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/selector.ui` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/selector.ui`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/qtui/window_icon.png` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/qtui/window_icon.png`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/gui/selector.py` & `OpihiExarata-2023.6.8/src/opihiexarata/gui/selector.py`

 * *Files 0% similar despite different names*

```diff
@@ -1183,15 +1183,21 @@
                 p0=guess_y_gaussian,
                 method="trf",
             )
             # We only need the gaussian centers, the asteroid pixel locations.
             search_x = float(x_gaussian_param[0])
             search_y = float(y_gaussian_param[0])
         except Exception:
-            error.warn(warn_class=error.AccuracyWarning, message="The centroid of the star could not be computed using Gaussian cross sections; we are using maximum pixel instead.")
+            error.warn(
+                warn_class=error.AccuracyWarning,
+                message=(
+                    "The centroid of the star could not be computed using Gaussian"
+                    " cross sections; we are using maximum pixel instead."
+                ),
+            )
             # Something happened and for some reason the Gaussian method did
             # not work as intended. We fall back to a far more robust but
             # inaccurate approach of determining the center based on the
             # maximum pixel.
             search_y, search_x = np.unravel_index(
                 np.nanargmax(search_array), search_array.shape
             )
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/__init__.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/__init__.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/config.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/config.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/conversion.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/conversion.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/engine.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/engine.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/error.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/error.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,27 +161,33 @@
 ####################
 
 
 class ExarataWarning(UserWarning):
     """The base warning class which all of the other OpihiExarata warnings
     are derived from."""
 
+
 class AccuracyWarning(ExarataWarning):
-    """This warning is to be used when something is not as accurate as it 
+    """This warning is to be used when something is not as accurate as it
     should be."""
+
+
 class InputWarning(ExarataWarning):
     """This warning is to be used when something was incorrectly input."""
 
+
 class FilterWarning(ExarataWarning):
     """This warning is to be used when improper filters were used."""
 
+
 class SequentialOrderWarning(ExarataWarning):
     """This warning is to be used when something is being done out of order or
     the specific order is not being followed.."""
 
+
 class UnknownWarning(ExarataWarning):
     """This warning is to be used when something was incorrectly input."""
 
 
 def warn(
     warn_class: type[ExarataWarning] = ExarataWarning,
     message: str = "",
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/fits.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/fits.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,14 +189,20 @@
             # Otherwise, we just use the default.
             valuedex = defaultdex
 
         # We type check as FITS header files are picky about the object types
         # they get FITS headers really only support some specific basic types.
         if isinstance(valuedex, (int, float, bool, str)):
             # These are generally accepted types.
+            if np.isfinite(valuedex):
+                # All good.
+                pass
+            else:
+                if np.isnan(valuedex):
+                    valuedex = "NaN"
             pass
         elif valuedex is None:
             # Astropy may be able to handle it.
             pass
         else:
             raise error.InputError(
                 "The input value {v} has a type of {t}. FITS file headers really"
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/hint.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/hint.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/http.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/http.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/image.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/image.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/json.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/json.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/mpcrecord.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/mpcrecord.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/path.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/path.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/phototable.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/phototable.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/tcs.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/tcs.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/library/temporary.py` & `OpihiExarata-2023.6.8/src/opihiexarata/library/temporary.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/opihi/database.py` & `OpihiExarata-2023.6.8/src/opihiexarata/opihi/database.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/opihi/preprocess.py` & `OpihiExarata-2023.6.8/src/opihiexarata/opihi/preprocess.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/opihi/solution.py` & `OpihiExarata-2023.6.8/src/opihiexarata/opihi/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/orbit/custom.py` & `OpihiExarata-2023.6.8/src/opihiexarata/orbit/custom.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/orbit/orbfit.py` & `OpihiExarata-2023.6.8/src/opihiexarata/orbit/orbfit.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/orbit/solution.py` & `OpihiExarata-2023.6.8/src/opihiexarata/orbit/solution.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/photometry/panstarrs.py` & `OpihiExarata-2023.6.8/src/opihiexarata/photometry/panstarrs.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,19 +324,21 @@
         # Check that the data release is supported.
         data_release = str(data_release)
         VALID_PANSTARRS_DATA_RELEASES = ("1", "2")
         if data_release not in VALID_PANSTARRS_DATA_RELEASES:
             raise error.InputError(
                 "The data release version provided is not supported."
             )
-        
+
         # Pan-STARRS only supports a declination of greater than -30 deg.
         if dec <= -30.0:
             raise error.EngineError(
-                "The Pan-STARRS survey does not have any sky coverage lower than declination -30 degrees. The current queried declination is {d} degrees.".format(d=dec)
+                "The Pan-STARRS survey does not have any sky coverage lower than"
+                " declination -30 degrees. The current queried declination is {d}"
+                " degrees.".format(d=dec)
             )
 
         # The MAST API service is a url request. Constructing the URL based on
         # the provided information.
         mast_api_url = (
             "https://catalogs.mast.stsci.edu/api/v0.1/panstarrs/dr{v}/mean.csv?"
             "ra={a}&dec={d}&radius={r}&nDetections.gte={n}&columns={c}&pagesize={l}&"
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/photometry/solution.py` & `OpihiExarata-2023.6.8/src/opihiexarata/photometry/solution.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,15 +512,17 @@
 
         # We filter the stars so that we avoid using stars and targets
         # which otherwise would skew our results.
         # Stars which are too bright saturate our detector. We limit based on
         # the magnitude as specified. A dimmer object has a higher magnitude.
         DIM_MAG = library.config.PHOTOMETRY_ZERO_POINT_DIMMEST_MAGNITUDE
         BRIGHT_MAG = library.config.PHOTOMETRY_ZERO_POINT_BRIGHTEST_MAGNITUDE
-        invalid_filter_magnitude = np.where(np.logical_and(BRIGHT_MAG <= magnitude, magnitude <= DIM_MAG), False, True)
+        invalid_filter_magnitude = np.where(
+            np.logical_and(BRIGHT_MAG <= magnitude, magnitude <= DIM_MAG), False, True
+        )
         # We only can use count data which is actually valid, using invalid
         # count data corrupts our instrument magnitudes and everything else
         # down the line.
         invalid_instrument_magnitude = ~np.logical_and(np.isfinite(counts), counts > 0)
 
         # The valid points that we can use are those not caught with the
         # filter.
@@ -528,17 +530,17 @@
         # Using only the remaining/valid targets for the photometric
         # calculation.
         valid_magnitude = magnitude[valid_points]
         valid_inst_magnitude = inst_magnitude[valid_points]
 
         # Zero points via the definition equation
         zero_points = valid_magnitude - valid_inst_magnitude
-        # Zero points are technically a magnitude so we can only find its 
+        # Zero points are technically a magnitude so we can only find its
         # average by converting to linear space.
-        zero_point = -sqrt5_100 * np.log10(np.nanmedian(10**(-zero_points*0.4)))
+        zero_point = -sqrt5_100 * np.log10(np.nanmedian(10 ** (-zero_points * 0.4)))
         # We use the error on the mean, but instead we use medians and its
         # standard deviation equivalent to be robust to bad data points.
         n_stars = np.sum(np.isfinite(zero_points))
         zero_point_deviation = sp_stats.median_abs_deviation(
             zero_points, nan_policy="omit"
         )
         zero_point_error = zero_point_deviation / np.sqrt(n_stars)
```

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/propagate/polynomial.py` & `OpihiExarata-2023.6.8/src/opihiexarata/propagate/polynomial.py`

 * *Files identical despite different names*

### Comparing `OpihiExarata-2023.6.7/src/opihiexarata/propagate/solution.py` & `OpihiExarata-2023.6.8/src/opihiexarata/propagate/solution.py`

 * *Files identical despite different names*

