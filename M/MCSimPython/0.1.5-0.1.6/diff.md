# Comparing `tmp/MCSimPython-0.1.5.tar.gz` & `tmp/MCSimPython-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MCSimPython-0.1.5.tar", last modified: Tue May  9 16:23:37 2023, max compression
+gzip compressed data, was "MCSimPython-0.1.6.tar", last modified: Thu Jun  8 18:46:03 2023, max compression
```

## Comparing `MCSimPython-0.1.5.tar` & `MCSimPython-0.1.6.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.526385 MCSimPython-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-05-09 16:23:02.000000 MCSimPython-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-09 16:23:02.000000 MCSimPython-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-09 16:23:37.526385 MCSimPython-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-09 16:23:02.000000 MCSimPython-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-09 16:23:37.526385 MCSimPython-0.1.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.490386 MCSimPython-0.1.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.490386 MCSimPython-0.1.5/src/MCSimPython/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-09 16:23:30.000000 MCSimPython-0.1.5/src/MCSimPython/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.490386 MCSimPython-0.1.5/src/MCSimPython/control/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/control/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5602 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/control/adaptiveFS.py
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/control/backstepping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5138 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/control/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.490386 MCSimPython-0.1.5/src/MCSimPython/guidance/
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/guidance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2461 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/guidance/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/guidance/path_param.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.494386 MCSimPython-0.1.5/src/MCSimPython/observer/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/observer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10739 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/observer/ekf.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/observer/ltv_kf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/observer/nonlinobs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.494386 MCSimPython-0.1.5/src/MCSimPython/simulator/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/simulator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/simulator/csad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/simulator/gunnerus.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/simulator/thruster_dynamics.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/simulator/vessel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.494386 MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/allocation.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/thruster.py
--rw-r--r--   0 runner    (1001) docker     (123)    45304 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.494386 MCSimPython-0.1.5/src/MCSimPython/vessel_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.494386 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/freqs.npy
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/headings.npy
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/thruster_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
--rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/vessel_json.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.522385 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/gunnerusABC.json
--rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
--rw-r--r--   0 runner    (1001) docker     (123)  5603889 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg2_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config.json
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config_.json
--rw-r--r--   0 runner    (1001) docker     (123)  5611180 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg3_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
--rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/vessel.json
--rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.526385 MCSimPython-0.1.5/src/MCSimPython/waves/
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/waves/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/waves/wave_loads.py
--rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/waves/wave_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/src/MCSimPython/waves/wave_spreading.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.490386 MCSimPython-0.1.5/src/MCSimPython.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-05-09 16:23:37.000000 MCSimPython-0.1.5/src/MCSimPython.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-09 16:23:37.000000 MCSimPython-0.1.5/src/MCSimPython.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 16:23:37.000000 MCSimPython-0.1.5/src/MCSimPython.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-09 16:23:37.000000 MCSimPython-0.1.5/src/MCSimPython.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-09 16:23:37.000000 MCSimPython-0.1.5/src/MCSimPython.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 16:23:37.526385 MCSimPython-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-05-09 16:23:05.000000 MCSimPython-0.1.5/tests/test_wave_spectra.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.475478 MCSimPython-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-08 18:45:34.000000 MCSimPython-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 18:45:34.000000 MCSimPython-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-08 18:46:03.475478 MCSimPython-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-06-08 18:45:34.000000 MCSimPython-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:46:03.475478 MCSimPython-0.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.439478 MCSimPython-0.1.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.439478 MCSimPython-0.1.6/src/MCSimPython/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 18:45:55.000000 MCSimPython-0.1.6/src/MCSimPython/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/control/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/control/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/control/adaptiveFS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/control/backstepping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5198 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/control/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/guidance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/guidance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/guidance/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5539 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/guidance/path_param.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/observer/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/observer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10554 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/observer/ekf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7768 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/observer/ltv_kf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/observer/nonlinobs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/simulator/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/simulator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15957 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/simulator/csad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/simulator/gunnerus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/simulator/thruster_dynamics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/simulator/vessel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/allocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/thruster.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46121 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/vessel_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.443478 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/freqs.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/headings.npy
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/thruster_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4022 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)  1961336 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/vessel_json.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.471478 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/gunnerusABC.json
+-rw-r--r--   0 runner    (1001) docker     (123)  2939897 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2870 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)  5603889 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg2_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config_.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5611180 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg3_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  5568933 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4723068 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/vessel.json
+-rw-r--r--   0 runner    (1001) docker     (123)  4733857 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/vessel_2.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.475478 MCSimPython-0.1.6/src/MCSimPython/waves/
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/waves/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19643 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/waves/wave_loads.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12013 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/waves/wave_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2417 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/src/MCSimPython/waves/wave_spreading.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.439478 MCSimPython-0.1.6/src/MCSimPython.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2686 2023-06-08 18:46:03.000000 MCSimPython-0.1.6/src/MCSimPython.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-08 18:46:03.000000 MCSimPython-0.1.6/src/MCSimPython.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:46:03.000000 MCSimPython-0.1.6/src/MCSimPython.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-08 18:46:03.000000 MCSimPython-0.1.6/src/MCSimPython.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 18:46:03.000000 MCSimPython-0.1.6/src/MCSimPython.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:46:03.475478 MCSimPython-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4258 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2565 2023-06-08 18:45:38.000000 MCSimPython-0.1.6/tests/test_wave_spectra.py
```

### Comparing `MCSimPython-0.1.5/LICENSE` & `MCSimPython-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/PKG-INFO` & `MCSimPython-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MCSimPython-0.1.5/README.md` & `MCSimPython-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/pyproject.toml` & `MCSimPython-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/control/adaptiveFS.py` & `MCSimPython-0.1.6/src/MCSimPython/control/adaptiveFS.py`

 * *Files 8% similar despite different names*

```diff
@@ -32,17 +32,17 @@
         
         # Frequencies to be used in disturbance model 
         w_min = 2*np.pi/20                          # Lower bound
         w_max = 2*np.pi/2                           # Upper bound
         self.set_freqs(w_min, w_max, N)
 
         # Tuning:
-        self._K1 = np.diag([.1, 1., .1])
-        self._K2 = np.diag([.1, 1., .1])*10
-        self._gamma = np.eye((2*self._N +1)*3) * 5
+        self._K1 = np.diag([.1, 1., .0001])*1e-11
+        self._K2 = np.diag([.1, 1., .0001])*1e-11
+        self._gamma = np.eye((2*self._N +1)*3) * 1e-15
         self._kappa = 1                             # Must be positive
 
 
 
     def get_tau(self, eta, eta_d, nu, eta_d_dot, eta_d_ddot, t, calculate_bias=False):
         '''
         Calculate controller output based on the adaptive update law. 
@@ -88,25 +88,28 @@
         z2 = nu - alpha 
 
         # Differentiate
         z1_dot = -S@z1 + z2 -(self._K1 + self._kappa*np.eye(3))@z1
         alpha_dot = -(self._K1 + self._kappa*np.eye(3))@z1_dot - S@R.T@eta_d_dot + R.T@eta_d_ddot        
 
         # Adaptive update law
-        theta_hat_dot = self._gamma@Phi@z2                                                                  # @z1?
+        theta_hat_dot = self._gamma@Phi@z2                                                                 
         self.theta_hat  += (theta_hat_dot * self._dt)
 
         # Control law
-        tau = -self._K2@z2 + self._D@alpha + self._M@alpha_dot - Phi.T@self.theta_hat
-        # tau = R@tau                              # Ref frame of tau?
+        tau = -self._K2@z2 + self._D@alpha + self._M@alpha_dot - Phi.T@self.theta_hat         
+       
 
         # Calculate bias
         if calculate_bias:
             b_hat = Phi.T@self.theta_hat
-            return tau, b_hat
+            tau_z2 = -self._K2@z2
+            tau_alpha = self._D@alpha
+            tau_alpha_dot = self._M@alpha_dot
+            return tau, b_hat, tau_z2, tau_alpha, tau_alpha_dot
         
         return tau
 
     def get_regressor(self, t):
         '''
         get_regressor:
         Extract a (2*N+1)-dimensional regressor defined as [1   cos(w1*t)   sin(w1*t)   cos(w2*t)   ...   sin(wN*t)].
@@ -144,17 +147,18 @@
         self._N = N
         try:
             dw = (w_max-w_min)/ self._N
             self._freqs = np.arange(w_min, w_max, dw)
         except ZeroDivisionError:
             self._freqs = np.array([])
             
-
     def set_tuning_params(self, K1: list, K2: list, gamma: list):
         self._K1 = np.diag(K1)
         self._K2 = np.diag(K2)
         #self._gamma = np.eye((2*self._N +1)*3) * gamma
         if len(gamma) != (2*self._N +1)*3:
             raise ValueError
         self._gamma = np.diag(gamma)
 
 
+    def get_theta(self):
+        return self.theta_hat
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython/control/backstepping.py` & `MCSimPython-0.1.6/src/MCSimPython/control/backstepping.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/control/basic.py` & `MCSimPython-0.1.6/src/MCSimPython/control/basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,15 @@
     def __init__(self, kp: list, kd: list, ki: list, dt: float = 0.01):
         self.Kp = np.diag(kp)
         self.Kd = np.diag(kd)
         self.Ki = np.diag(ki)
         self.zi = np.zeros(3)
         self.dt = dt
 
+
     def get_tau(self, eta, eta_d, nu, nu_d):
         """Calculate control loads.
         
         Parameters
         ----------
         eta : array_like
             Vessel pose in surge, sway and yaw.
@@ -89,14 +90,15 @@
         psi = eta[-1]
         z1 = Rz(psi).T@(eta - eta_d)
         z1[2] = pipi(eta[2] - eta_d[2])
         z2 = nu - nu_d
 
         self.zi[:2] += self.dt*(eta[:2] - eta_d[:2])
         self.zi[2] += self.dt*pipi(eta[2] - eta_d[2])
+        
         return -self.Kp@z1 - self.Kd@z2 - Rz(psi).T@self.Ki@self.zi
 
 
 class PI:
     """Proportional control with integral action."""
 
     def __init__(self, kp: list, ki: list, dt: float = 0.01):
@@ -151,20 +153,22 @@
             Desired vessel pose in surge, sway and yaw (NED-frame).
         nu : array_like
             Vessel velocity in surge, sway, and yaw (body-frame).
         nu_d : array_like
             Desired vessel velocity in surge, sway and yaw (body-frame).
         b : array_like
             Estimated bias in surge, sway and yaw (body-frame)
+
+        Remark: Reference frame of bias!
         '''
         psi = eta[-1]
         z1 = Rz(psi).T@(eta-eta_d)              # P
         z1[2] = pipi(eta[2] - eta_d[2])
         z2 = nu - nu_d                          # D
-        zb = Rz(psi).T@b                        # bias
+        zb = Rz(psi).T@b                        # bias in body
         return -self.Kp@z1 - self.Kd@z2 - zb
     
     def set_kd(self, kd: list):
         self.Kd = np.diag(kd)
     
     def set_kp(self, kp: list):
         self.Kp = np.diag(kp)
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython/guidance/__init__.py` & `MCSimPython-0.1.6/src/MCSimPython/guidance/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/guidance/filter.py` & `MCSimPython-0.1.6/src/MCSimPython/guidance/filter.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
     def __init__(self, dt, omega=[0.3, 0.3, 0.3]):
         self._dt = dt
         self.eta_d = np.zeros(3)
         self.eta_d_dot = np.zeros(3)
         self.eta_d_ddot = np.zeros(3)
         self._eta_r = np.zeros(3)
-        self._x = np.zeros(9)
+        self._x = np.concatenate([self.eta_d, self.eta_d_dot, self.eta_d_ddot], axis=None)
         self._delta = np.eye(3)
         self._w = np.diag(omega)
         O3x3 = np.zeros((3, 3))
         self.Ad = np.block([
             [O3x3, np.eye(3), O3x3],
             [O3x3, O3x3, np.eye(3)],
             [-self._w**3, -(2*self._delta + np.eye(3))@self._w**2, - (2*self._delta + np.eye(3))@self._w]
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython/guidance/path_param.py` & `MCSimPython-0.1.6/src/MCSimPython/guidance/path_param.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/observer/__init__.py` & `MCSimPython-0.1.6/src/MCSimPython/observer/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/observer/ekf.py` & `MCSimPython-0.1.6/src/MCSimPython/observer/ekf.py`

 * *Files 1% similar despite different names*

```diff
@@ -363,20 +363,8 @@
         return self._Phat
     
     def get_eta_hat(self):
         return self._xhat[6:9]
     
     def get_nu_hat(self):
         return self._xhat[12:15] 
-        
-
-'''
-"Tuning factors":
-    - Q and R
-    - Tp in A_w
-    - zeta in A_w
-    - diag(Kw,Kw,Kw) in E
-    - Eb in E (njæ)
-    - Adjustment of noise
-    - Time step
-    - Initial values
-'''
+
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython/observer/ltv_kf.py` & `MCSimPython-0.1.6/src/MCSimPython/observer/ltv_kf.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
             [-omega**2*np.eye(3),   -2*zeta*omega*np.eye(3)]
         ])
         
         self._Bd = np.zeros((15,3))
         self._Bd[12:15, 0:3] = self._Minv * self._dt
 
         self._Ed = np.zeros((15,6))
-        self._Ed[3:6,0:3], self._Ed[9:12,3:6] = np.diag([1,1,1])*self._dt, np.eye(3)*self._dt
+        self._Ed[3:6,0:3], self._Ed[9:12,3:6] = np.diag([1,1,1])*self._dt, np.eye(3)*self._dt   # Multipliy with .01
 
         self._H = np.zeros((3,15))
         self._H[0:3,3:6], self._H[0:3,6:9] = np.eye(3), np.eye(3)
 
 
     def update(self, tau, y, psi_m, asynchronous = False, dead_reckoning = False):
         '''
@@ -133,41 +133,49 @@
             - asynchronous: True if measurement interval and simulation time step are asynchrounous. Set to false as default.
         '''
 
         if asynchronous:
             self.update_async(tau, y, psi_m)
             return None
         
+        y, tau = np.asarray(y), np.asarray(tau) # ROS check
+
+
         # Correct
         self.corrector(y, dead_reckoning)
         # Predict        
         self.predictor(tau, psi_m)
     
 
     def update_async(self, tau, y, psi_m):
         raise NotImplementedError
     
         
     
     def predictor(self, tau, psi_m):
         Ad =  self.Ad(psi_m)   # Get the time-varying state matrix
 
+        tau = tau.reshape((3,)) # ROS check
+
         self.xbar = Ad@self.xhat + self._Bd@tau
         self.Pbar = Ad@self.Phat@Ad.T + self._Ed@self.Qd@self._Ed.T
 
     
     def corrector(self, y, dead_reckoning):
         if dead_reckoning:    # If dead reckoning: Set corrector equal to predictor (Dead reckoning)
             self.Phat = self.Pbar
             self.xhat = self.xbar
         else:
             K = self.KF_gain
+            y = y.reshape((3,)) # ROS check
+
             prediction_error = y - (self._H@self.xbar)
             prediction_error[2] = pipi(prediction_error[2])   # Smallest signed angle modification
 
+            
             parenthesis = np.eye(15) - K @ self._H
 
             self.Phat = parenthesis @ self.Pbar @ parenthesis.T + K @ self.Rd @ K.T
             self.xhat = self.xbar + K @ prediction_error
 
 
     @property
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython/observer/nonlinobs.py` & `MCSimPython-0.1.6/src/MCSimPython/observer/nonlinobs.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/simulator/__init__.py` & `MCSimPython-0.1.6/src/MCSimPython/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/simulator/csad.py` & `MCSimPython-0.1.6/src/MCSimPython/simulator/csad.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/simulator/gunnerus.py` & `MCSimPython-0.1.6/src/MCSimPython/simulator/gunnerus.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/simulator/thruster_dynamics.py` & `MCSimPython-0.1.6/src/MCSimPython/simulator/thruster_dynamics.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/simulator/vessel.py` & `MCSimPython-0.1.6/src/MCSimPython/simulator/vessel.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/allocation.py` & `MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/allocation.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/constraints.py` & `MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/constraints.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/thrust_allocation/thruster.py` & `MCSimPython-0.1.6/src/MCSimPython/thrust_allocation/thruster.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/utils.py` & `MCSimPython-0.1.6/src/MCSimPython/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,17 @@
 import re
 import os
 import json
 
 from scipy.signal import TransferFunction
 from scipy.optimize import least_squares
 
+from scipy.signal import TransferFunction
+from scipy.optimize import least_squares
+
 
 dof3_matrix_mask = np.ix_([0, 1, 5], [0, 1 ,5])
 dof3_array = np.ix_([0, 1, 5])
 
 def complex_to_polar(complex_values):
     """Complex value to polar coordinates.
     
@@ -1321,8 +1324,37 @@
     if np.abs(R[2, 0]) > 1.0:
         raise RuntimeError('Solution is singular for pitch of +- 90 degrees')
 
     roll = np.arctan2(R[2, 1], R[2, 2])
     pitch = -np.arcsin(R[2, 0])
     yaw = np.arctan2(R[1, 0], R[0, 0])
 
-    return np.array([roll, pitch, yaw])
+    return np.array([roll, pitch, yaw])
+
+
+def quat2eul(w, x, y, z):
+    """
+    Returns the ZYX roll-pitch-yaw angles from a quaternion.
+    """
+    q = np.array((w, x, y, z))
+    #if np.abs(np.linalg.norm(q) - 1) > 1e-6:
+    #   raise RuntimeError('Norm of the quaternion must be equal to 1')
+
+    eta = q[0]
+    eps = q[1:]
+
+    S = np.array([
+        [0, -eps[2], eps[1]],
+        [eps[2], 0, -eps[0]],
+        [-eps[1], eps[0], 0]
+    ])
+
+    R = np.eye(3) + 2 * eta * S + 2 * np.linalg.matrix_power(S, 2)
+
+    if np.abs(R[2, 0]) > 1.0:
+        raise RuntimeError('Solution is singular for pitch of +- 90 degrees')
+
+    roll = np.arctan2(R[2, 1], R[2, 2])
+    pitch = -np.arcsin(R[2, 0])
+    yaw = np.arctan2(R[1, 0], R[0, 0])
+
+    return np.array([roll, pitch, yaw])
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/vesselABC_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/CSAD/vessel_json.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/CSAD/vessel_json.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/gunnerusABC.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/gunnerusABC.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/gunnerus_veres.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/parV_RVG3DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/parV_RVG6DOF.pkl`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg2_config.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg2_config.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config_.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg3ABC_config_.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg3_config.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg3_config.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/rvg_config.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/rvg_config.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/vessel.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/vessel.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/vessel_data/gunnerus/vessel_2.json` & `MCSimPython-0.1.6/src/MCSimPython/vessel_data/gunnerus/vessel_2.json`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/waves/wave_loads.py` & `MCSimPython-0.1.6/src/MCSimPython/waves/wave_loads.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/waves/wave_spectra.py` & `MCSimPython-0.1.6/src/MCSimPython/waves/wave_spectra.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython/waves/wave_spreading.py` & `MCSimPython-0.1.6/src/MCSimPython/waves/wave_spreading.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/src/MCSimPython.egg-info/PKG-INFO` & `MCSimPython-0.1.6/src/MCSimPython.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MCSimPython
-Version: 0.1.5
+Version: 0.1.6
 Summary: Python vessel simulation environment
 Author-email: Jan-Erik Hygen <janereh@stud.ntnu.no>
 Keywords: mcsim,MCSimPython,DP,dynamic positioning,Marine Cybernetics
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `MCSimPython-0.1.5/src/MCSimPython.egg-info/SOURCES.txt` & `MCSimPython-0.1.6/src/MCSimPython.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/tests/test_utils.py` & `MCSimPython-0.1.6/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `MCSimPython-0.1.5/tests/test_wave_spectra.py` & `MCSimPython-0.1.6/tests/test_wave_spectra.py`

 * *Files identical despite different names*

