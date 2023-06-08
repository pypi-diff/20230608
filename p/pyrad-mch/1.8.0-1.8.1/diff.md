# Comparing `tmp/pyrad_mch-1.8.0.tar.gz` & `tmp/pyrad_mch-1.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrad_mch-1.8.0.tar", last modified: Tue May 30 15:41:13 2023, max compression
+gzip compressed data, was "pyrad_mch-1.8.1.tar", last modified: Thu Jun  8 08:46:13 2023, max compression
```

## Comparing `pyrad_mch-1.8.0.tar` & `pyrad_mch-1.8.1.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.980981 pyrad_mch-1.8.0/pyrad/
--rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.980981 pyrad_mch-1.8.0/pyrad/flow/
--rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/flow/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57500 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/flow/flow_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    34809 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/flow/flow_control.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.980981 pyrad_mch-1.8.0/pyrad/graph/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    54994 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13147 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    45068 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_grid.py
--rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_spectra.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    24330 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    70743 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/graph/plots_vol.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.984981 pyrad_mch-1.8.0/pyrad/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9281 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   112893 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/io_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3936 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/mxpol_config.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_dem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9542 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_hzt.py
--rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_iso0_mf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    37831 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_mxpol.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    57335 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_other.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   185474 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_radar.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    78210 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/read_data_sun.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7684 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/trajectory.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    97871 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/io/write_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.984981 pyrad_mch-1.8.0/pyrad/proc/
--rwxr-xr-x   0 runner    (1001) docker     (123)    11666 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_Doppler.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    93122 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_aux.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    92202 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_calib.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38434 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_dem.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    93466 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_echoclass.py
--rw-r--r--   0 runner    (1001) docker     (123)    59766 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_grid.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    89471 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_intercomp.py
--rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_iq.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    62664 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_monitoring.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    43276 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_phase.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    58764 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_retrieve.py
--rw-r--r--   0 runner    (1001) docker     (123)    66245 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_spectra.py
--rw-r--r--   0 runner    (1001) docker     (123)    47217 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_timeseries.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    72382 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/proc/process_traj.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.988981 pyrad_mch-1.8.0/pyrad/prod/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    38966 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_grid_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13183 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_intercomp_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31042 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_monitoring_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    56567 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_product.py
--rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_spectra_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    30674 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_timeseries_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_traj_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   154784 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/process_vol_products.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4392 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/prod/product_aux.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.988981 pyrad_mch-1.8.0/pyrad/util/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/util/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    61246 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/util/radar_utils.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/pyrad/util/stat_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.988981 pyrad_mch-1.8.0/pyrad_mch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-30 15:41:13.000000 pyrad_mch-1.8.0/pyrad_mch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     5799 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/common_colocated_gates.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_precipitation_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_cosmo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_cosmo_rt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_birds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_period.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4434 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_rt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_data_trt.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_euclid_data.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5965 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/main_process_gecsx.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/movie_maker.py
--rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/scripts/rewrite_monitoring.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 15:41:13.992982 pyrad_mch-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-30 15:41:04.000000 pyrad_mch-1.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.114686 pyrad_mch-1.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 08:46:13.114686 pyrad_mch-1.8.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.102686 pyrad_mch-1.8.1/pyrad/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      869 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.102686 pyrad_mch-1.8.1/pyrad/flow/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      386 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/flow/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57500 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/flow/flow_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    34809 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/flow/flow_control.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.102686 pyrad_mch-1.8.1/pyrad/graph/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3205 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    54994 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/plots.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13147 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/plots_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44989 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/plots_grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52389 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/plots_spectra.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    24330 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/plots_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    70743 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/graph/plots_vol.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.106686 pyrad_mch-1.8.1/pyrad/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7748 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9281 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   112893 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/io_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3936 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/mxpol_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15513 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17208 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9542 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_hzt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12230 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_iso0_mf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    37831 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_mxpol.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    57335 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_other.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   185602 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_radar.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    78210 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15042 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/read_data_sun.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7684 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/trajectory.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    97871 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/io/write_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.106686 pyrad_mch-1.8.1/pyrad/proc/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11666 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36329 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_Doppler.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    93122 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_aux.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    92202 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_calib.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38434 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11063 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_dem.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    94520 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_echoclass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59766 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_grid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    89471 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_intercomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26560 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_iq.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    62664 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_monitoring.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    44326 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_phase.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    58764 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_retrieve.py
+-rw-r--r--   0 runner    (1001) docker     (123)    66245 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_spectra.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47217 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_timeseries.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    72382 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/proc/process_traj.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.110686 pyrad_mch-1.8.1/pyrad/prod/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2089 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    38966 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_grid_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13183 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_intercomp_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31042 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_monitoring_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    56567 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47103 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_spectra_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    30674 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_timeseries_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5606 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_traj_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   154891 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/process_vol_products.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4392 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/prod/product_aux.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.110686 pyrad_mch-1.8.1/pyrad/util/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/util/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    61246 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/util/radar_utils.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4908 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/pyrad/util/stat_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-08 08:46:13.000000 pyrad_mch-1.8.1/pyrad/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.110686 pyrad_mch-1.8.1/pyrad_mch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-06-08 08:46:13.000000 pyrad_mch-1.8.1/pyrad_mch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-08 08:46:13.000000 pyrad_mch-1.8.1/pyrad_mch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:46:13.000000 pyrad_mch-1.8.1/pyrad_mch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:46:12.000000 pyrad_mch-1.8.1/pyrad_mch.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 08:46:13.000000 pyrad_mch-1.8.1/pyrad_mch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:46:13.110686 pyrad_mch-1.8.1/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5799 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/common_colocated_gates.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4556 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_precipitation_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_cosmo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_cosmo_rt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6535 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8588 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_data_birds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6393 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_data_period.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4434 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_data_rt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16283 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_data_trt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_euclid_data.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5965 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/main_process_gecsx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/movie_maker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7956 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/scripts/rewrite_monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:46:13.114686 pyrad_mch-1.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-06-08 08:45:59.000000 pyrad_mch-1.8.1/setup.py
```

### Comparing `pyrad_mch-1.8.0/PKG-INFO` & `pyrad_mch-1.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrad_mch
-Version: 1.8.0
+Version: 1.8.1
 Summary:  Python Radar Toolkit
 Home-page: https://github.com/MeteoSwiss/pyrad.git
 Author: MeteoSwiss Pyrad Developers
 Author-email: daniel.wolfensberger@meteoswiss.ch
 Maintainer: MeteoSwiss Pyrad Developers
 Maintainer-email: daniel.wolfensberger@meteoswiss.ch
 License: BSD
```

### Comparing `pyrad_mch-1.8.0/pyrad/__init__.py` & `pyrad_mch-1.8.1/pyrad/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/flow/flow_aux.py` & `pyrad_mch-1.8.1/pyrad/flow/flow_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/flow/flow_control.py` & `pyrad_mch-1.8.1/pyrad/flow/flow_control.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/graph/__init__.py` & `pyrad_mch-1.8.1/pyrad/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/graph/plots.py` & `pyrad_mch-1.8.1/pyrad/graph/plots.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/graph/plots_aux.py` & `pyrad_mch-1.8.1/pyrad/graph/plots_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/graph/plots_grid.py` & `pyrad_mch-1.8.1/pyrad/graph/plots_grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,61 +113,63 @@
     if exact_limits:
         lon_lines = np.arange(min_lon, max_lon + lonstep, lonstep)
         lat_lines = np.arange(min_lat, max_lat + latstep, latstep)
     else:
         lon_lines = np.arange(np.floor(min_lon), np.ceil(max_lon)+1, lonstep)
         lat_lines = np.arange(np.floor(min_lat), np.ceil(max_lat)+1, latstep)
 
+    if use_basemap:
+        resolution = prdcfg['gridMapImageConfig'].get('mapres', 'l')
+        if resolution not in ('c', 'l', 'i', 'h', 'f'):
+            warn('Unknown map resolution: '+resolution)
+            resolution = 'l'
+
+        if resolution == 'c':
+            area_thresh = 10000
+        elif resolution == 'l':
+            area_thresh = 1000
+        elif resolution == 'i':
+            area_thresh = 100
+        elif resolution == 'h':
+            area_thresh = 10
+        elif resolution == 'f':
+            area_thresh = 1
+    else:
+        resolution = prdcfg['gridMapImageConfig'].get('mapres', '110m')
+        # Map from basemap to cartopy notation
+        if resolution == 'l':
+            resolution = '110m'
+        elif resolution == 'i':
+            resolution = '50m'
+        elif resolution == 'h':
+            resolution = '10m'
+
+        if resolution not in ('110m', '50m', '10m'):
+            warn('Unknown map resolution: '+resolution)
+            resolution = '110m'
+        background_zoom = prdcfg['gridMapImageConfig'].get(
+            'background_zoom', 8)
+        maps_list = prdcfg['gridMapImageConfig'].get('maps', [])
+
     if fig is None:
         fig = plt.figure(figsize=[xsize, ysize], dpi=dpi)
 
         if use_basemap:
-            resolution = prdcfg['gridMapImageConfig'].get('mapres', 'l')
-            if resolution not in ('c', 'l', 'i', 'h', 'f'):
-                warn('Unknown map resolution: '+resolution)
-                resolution = 'l'
-
-            if resolution == 'c':
-                area_thresh = 10000
-            elif resolution == 'l':
-                area_thresh = 1000
-            elif resolution == 'i':
-                area_thresh = 100
-            elif resolution == 'h':
-                area_thresh = 10
-            elif resolution == 'f':
-                area_thresh = 1
-
             display = pyart.graph.GridMapDisplayBasemap(grid)
             display.plot_basemap(
                 lat_lines=lat_lines, lon_lines=lon_lines,
                 resolution=resolution, area_thresh=area_thresh,
                 auto_range=False, min_lon=min_lon, max_lon=max_lon,
                 min_lat=min_lat, max_lat=max_lat)
             display.plot_grid(
                 field_name, level=level, norm=norm, ticks=ticks, title=titl,
                 ticklabs=ticklabs, mask_outside=mask_outside, vmin=vmin,
                 vmax=vmax, alpha=alpha, fig=fig)
         else:
-            resolution = prdcfg['gridMapImageConfig'].get('mapres', '110m')
             projection = cartopy.crs.PlateCarree()
-            # Map from basemap to cartopy notation
-            if resolution == 'l':
-                resolution = '110m'
-            elif resolution == 'i':
-                resolution = '50m'
-            elif resolution == 'h':
-                resolution = '10m'
-
-            if resolution not in ('110m', '50m', '10m'):
-                warn('Unknown map resolution: '+resolution)
-                resolution = '110m'
-            background_zoom = prdcfg['gridMapImageConfig'].get(
-                'background_zoom', 8)
-            maps_list = prdcfg['gridMapImageConfig'].get('maps', [])
 
             display = pyart.graph.GridMapDisplay(grid)
             display.plot_grid(
                 field_name, level=level, norm=norm, ticks=ticks,
                 ticklabs=ticklabs, lat_lines=lat_lines, projection=projection,
                 lon_lines=lon_lines, vmin=vmin, embellish=False,
                 add_grid_lines=True, vmax=vmax, mask_outside=mask_outside,
@@ -183,15 +185,15 @@
                 lat_lines=lat_lines, lon_lines=lon_lines, title=titl,
                 ticklabs=ticklabs, colorbar_flag=False, embellish=False,
                 vmin=vmin, vmax=vmax, mask_outside=mask_outside,
                 alpha=alpha, ax=ax, fig=fig)
         else:
             display.plot_grid(
                 field_name, level=level, norm=norm, ticks=ticks,
-                projection=projection, lat_lines=lat_lines,
+                projection=ax.projection, lat_lines=lat_lines,
                 lon_lines=lon_lines, ticklabs=ticklabs, colorbar_flag=False,
                 embellish=False, vmin=vmin, vmax=vmax,
                 mask_outside=mask_outside, alpha=alpha, title=titl, ax=ax,
                 fig=fig)
 
     if embellish:
         ax = plt.gca()
```

### Comparing `pyrad_mch-1.8.0/pyrad/graph/plots_spectra.py` & `pyrad_mch-1.8.1/pyrad/graph/plots_spectra.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/graph/plots_timeseries.py` & `pyrad_mch-1.8.1/pyrad/graph/plots_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/graph/plots_vol.py` & `pyrad_mch-1.8.1/pyrad/graph/plots_vol.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/__init__.py` & `pyrad_mch-1.8.1/pyrad/io/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/config.py` & `pyrad_mch-1.8.1/pyrad/io/config.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/io_aux.py` & `pyrad_mch-1.8.1/pyrad/io/io_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/mxpol_config.py` & `pyrad_mch-1.8.1/pyrad/io/mxpol_config.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_cosmo.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_dem.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_dem.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_hzt.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_hzt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_iso0_mf.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_iso0_mf.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_mxpol.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_mxpol.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_other.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_other.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_radar.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_radar.py`

 * *Files 0% similar despite different names*

```diff
@@ -2459,17 +2459,17 @@
 
     Returns
     -------
     radar : Radar
         radar object
 
     """
-    field_names = []
+    field_names = {}
     for datatype in datatype_list:
-        field_names.append(get_fieldname_pyart(datatype))
+        field_names[datatype] = (get_fieldname_pyart(datatype))
 
     radar = None
     dayinfo = voltime.strftime('%y%j')
     timeinfo = voltime.strftime('%H%M')
     if radar_name is not None and radar_res is not None:
         basename = 'M'+radar_res+radar_name+dayinfo
     if cfg['path_convention'][ind_rad] == 'LTE':
@@ -2564,21 +2564,22 @@
             filename = []
             for filename_aux in filenames:
                 fdatetime = find_date_in_file_name(
                     filename_aux, date_format=fdate_strf)
                 if fdatetime == voltime:
                     filename = [filename_aux]
                     break
+        elif cfg['path_convention'][ind_rad] == 'RADARV':
+            filename = glob.glob(datapath+'/'+voltime.strftime(fpath_strf)+'/*')
         else:
             filename = glob.glob(datapath+basename+timeinfo+'*'+scan+'*')
         if not filename:
             warn('No file found in '+datapath+basename+timeinfo+'*.'+scan)
         else:
-            radar_aux = pyart.io.read_cfradial2(
-                filename[0], field_names=field_names)
+            radar_aux = pyart.io.read_cfradial2(filename[0], field_names=field_names)
             if radar_aux is None:
                 continue
 
             if radar is None:
                 radar = radar_aux
             else:
                 radar = pyart.util.radar_utils.join_radar(radar, radar_aux)
```

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_sensor.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_sensor.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/read_data_sun.py` & `pyrad_mch-1.8.1/pyrad/io/read_data_sun.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/timeseries.py` & `pyrad_mch-1.8.1/pyrad/io/timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/trajectory.py` & `pyrad_mch-1.8.1/pyrad/io/trajectory.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/io/write_data.py` & `pyrad_mch-1.8.1/pyrad/io/write_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/__init__.py` & `pyrad_mch-1.8.1/pyrad/proc/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_Doppler.py` & `pyrad_mch-1.8.1/pyrad/proc/process_Doppler.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_aux.py` & `pyrad_mch-1.8.1/pyrad/proc/process_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_calib.py` & `pyrad_mch-1.8.1/pyrad/proc/process_calib.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_cosmo.py` & `pyrad_mch-1.8.1/pyrad/proc/process_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_dem.py` & `pyrad_mch-1.8.1/pyrad/proc/process_dem.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_echoclass.py` & `pyrad_mch-1.8.1/pyrad/proc/process_echoclass.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,14 +61,23 @@
         Processing status: 0 initializing, 1 processing volume,
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
+        wind_size : int
+            Size of the moving window used to compute the ray texture
+            (number of gates). Default 7
+        max_textphi, max_textrhv, max_textzdr, max_textrefl : float
+            Maximum value for the texture of the differential phase, texture
+            of RhoHV, texture of Zdr and texture of reflectivity. Gates in
+            these. Default 20, 0.3, 2.85, 8
+        min_rhv : float
+            Minimum value for the RhoHV. Default 0.6
     radar_list : list of Radar objects
         Optional. list of radar objects
 
     Returns
     -------
     new_dataset : dict
         dictionary containing the output
@@ -106,21 +115,29 @@
             (rhv_field not in radar.fields) or
             (phi_field not in radar.fields)):
         warn('Unable to create radar_echo_id dataset. Missing data')
         return None, None
 
     echo_id = np.ma.zeros((radar.nrays, radar.ngates), dtype=np.uint8)+3
 
+    # user defined parameters
+    wind_size = dscfg.get('wind_size', 7)
+    max_textphi = dscfg.get('max_textphi', 20.)
+    max_textrhv = dscfg.get('max_textrhv', 0.3)
+    max_textzdr = dscfg.get('max_textzdr', 2.85)
+    max_textrefl = dscfg.get('max_textrefl', 8.)
+    min_rhv = dscfg.get('min_rhv', 0.6)
+
     # look for clutter
     gatefilter = pyart.filters.moment_and_texture_based_gate_filter(
         radar, zdr_field=zdr_field, rhv_field=rhv_field, phi_field=phi_field,
         refl_field=refl_field, textzdr_field=None, textrhv_field=None,
-        textphi_field=None, textrefl_field=None, wind_size=7,
-        max_textphi=20., max_textrhv=0.3, max_textzdr=2.85,
-        max_textrefl=8., min_rhv=0.6)
+        textphi_field=None, textrefl_field=None, wind_size=wind_size,
+        max_textphi=max_textphi, max_textrhv=max_textrhv,
+        max_textzdr=max_textzdr, max_textrefl=max_textrefl, min_rhv=min_rhv)
 
     is_clutter = gatefilter.gate_excluded == 1
     echo_id[is_clutter] = 2
 
     # look for noise
     is_noise = radar.fields[refl_field]['data'].data == (
         pyart.config.get_fillvalue())
@@ -508,14 +525,17 @@
             mask, radar_field['data'])
 
         if field_name.startswith('corrected_'):
             new_field_name = field_name
         elif field_name.startswith('uncorrected_'):
             new_field_name = field_name.replace(
                 'uncorrected_', 'corrected_', 1)
+        elif field_name.startswith('unfiltered_'):
+            new_field_name = field_name.replace(
+                'unfiltered_', 'corrected_', 1)
         else:
             new_field_name = 'corrected_'+field_name
         new_dataset['radar_out'].add_field(new_field_name, radar_field)
 
     if not new_dataset['radar_out'].fields:
         return None, None
 
@@ -631,15 +651,15 @@
     """
 
     if procstatus != 1:
         return None, None
 
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
-        if datatype in ('SNRh', 'SNRv', 'SNR','CNR'):
+        if datatype in ('SNRh', 'SNRv', 'SNR', 'CNR'):
             snr_field = get_fieldname_pyart(datatype)
             break
 
     ind_rad = int(radarnr[5:8])-1
     if radar_list[ind_rad] is None:
         warn('No valid radar')
         return None, None
@@ -667,15 +687,14 @@
         if ((min_snr is not None or max_snr is not None) and
                 (snr_field in radar_aux.fields)):
             gatefilter.exclude_masked(snr_field)
             gatefilter.exclude_invalid(snr_field)
             if min_snr is not None:
                 gatefilter.exclude_below(snr_field, min_snr)
 
-
     is_low_snr = gatefilter.gate_excluded == 1
 
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
 
         if datatype in ('SNRh', 'SNRv', 'SNR'):
             continue
@@ -819,15 +838,15 @@
         return None, None
 
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
         if datatype == 'VIS':
             vis_field = get_fieldname_pyart(datatype)
             break
-        elif 'visibility_polar' in datatype: # from GECSX
+        elif 'visibility_polar' in datatype:  # from GECSX
             vis_field = get_fieldname_pyart('visibility_polar')
 
     ind_rad = int(radarnr[5:8])-1
     if radar_list[ind_rad] is None:
         warn('No valid radar')
         return None, None
     radar = radar_list[ind_rad]
@@ -1060,16 +1079,16 @@
     for datatypedescr in dscfg['datatype']:
         radarnr, _, datatype, _, _ = get_datatype_fields(datatypedescr)
         if datatype == 'VOL2BIRD_CLASS':
             continue
 
         field_name = get_fieldname_pyart(datatype)
         if field_name not in radar.fields:
-            warn('Unable to filter {} according to VOL2BIRD_CLASS. No valid input fields'.format(
-                 field_name))
+            warn(f'Unable to filter {field_name} according to VOL2BIRD_CLASS.'
+                 f' No valid input fields')
             continue
         radar_field = deepcopy(radar.fields[field_name])
         radar_field['data'] = np.ma.masked_where(
             mask, radar_field['data'])
 
         if field_name.startswith('corrected_'):
             new_field_name = field_name
@@ -1359,16 +1378,17 @@
                 'AG', 'CR', 'LR', 'RP', 'RN', 'VI', 'WS', 'MH', 'IH/HDG')
             var_names = ('dBZ', 'ZDR', 'KDP', 'RhoHV', 'H_ISO0')
 
         ARM_VERSION = False
         try:
             fields_dict = pyart.retrieve.hydroclass_semisupervised(
                 radar, hydro_names=hydro_names, var_names=var_names,
-                mass_centers=mass_centers, weights=weights, refl_field=refl_field,
-                zdr_field=zdr_field, rhv_field=rhv_field, kdp_field=kdp_field,
+                mass_centers=mass_centers, weights=weights,
+                refl_field=refl_field, zdr_field=zdr_field,
+                rhv_field=rhv_field, kdp_field=kdp_field,
                 temp_field=temp_field, iso0_field=iso0_field, hydro_field=None,
                 entropy_field=None, temp_ref=temp_ref,
                 compute_entropy=compute_entropy,
                 output_distances=output_distances, vectorize=vectorize)
         except TypeError as e:
             ARM_VERSION = True
             warn('Hydroclass method could not parse all inputs')
@@ -2177,17 +2197,19 @@
                     for fname in flist:
                         radar_ml = pyart.io.read_cfradial(fname)
                         if radar_ml is None:
                             warn('Unable to use retrieved melting layer data')
                             continue
 
                         ml_top = (
-                            radar_ml.fields['melting_layer_height']['data'][:, 1])
+                            radar_ml.fields['melting_layer_height']['data'][
+                                :, 1])
                         ml_bottom = (
-                            radar_ml.fields['melting_layer_height']['data'][:, 0])
+                            radar_ml.fields['melting_layer_height']['data'][
+                                :, 0])
                         ml_thickness = ml_top-ml_bottom
                         ml_bottom_arr = np.ma.append(
                             ml_bottom_arr,
                             np.ma.zeros(radar_ml.nsweeps)+ml_bottom)
                         ml_thickness_arr = np.ma.append(
                             ml_thickness_arr,
                             np.ma.zeros(radar_ml.nsweeps)+ml_thickness)
```

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_grid.py` & `pyrad_mch-1.8.1/pyrad/proc/process_grid.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_intercomp.py` & `pyrad_mch-1.8.1/pyrad/proc/process_intercomp.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_iq.py` & `pyrad_mch-1.8.1/pyrad/proc/process_iq.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_monitoring.py` & `pyrad_mch-1.8.1/pyrad/proc/process_monitoring.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_phase.py` & `pyrad_mch-1.8.1/pyrad/proc/process_phase.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,23 +43,24 @@
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         rmin : float. Dataset keyword
-            The minimum range where to look for valid data [m]
+            The minimum range where to look for valid data [m]. Default 1000.
         rmax : float. Dataset keyword
-            The maximum range where to look for valid data [m]
+            The maximum range where to look for valid data [m]. Default 50000.
         rcell : float. Dataset keyword
-            The length of a continuous cell to consider it valid precip [m]
+            The length of a continuous cell to consider it valid precip [m].
+            Default 1000.
         Zmin : float. Dataset keyword
-            The minimum reflectivity [dBZ]
+            The minimum reflectivity [dBZ]. Default 20.
         Zmax : float. Dataset keyword
-            The maximum reflectivity [dBZ]
+            The maximum reflectivity [dBZ]. Default 40.
     radar_list : list of Radar objects
         Optional. list of radar objects
 
     Returns
     -------
     new_dataset : dict
         dictionary containing the output
@@ -90,37 +91,44 @@
         return None, None
     radar = radar_list[ind_rad]
 
     if (refl_field not in radar.fields) or (psidp_field not in radar.fields):
         warn('Unable to correct PhiDP system offset. Missing data')
         return None, None
 
-    ind_rmin = np.where(radar.range['data'] > dscfg['rmin'])[0][0]
-    ind_rmax = np.where(radar.range['data'] < dscfg['rmax'])[0][-1]
+    # user defined parameters
+    rmin = dscfg.get('rmin', 1000.)
+    rmax = dscfg.get('rmax', 50000.)
+    rcell = dscfg.get('rcell', 1000.)
+    zmin = dscfg.get('Zmin', 20.)
+    zmax = dscfg.get('Zmax', 40.)
+
+    ind_rmin = np.where(radar.range['data'] > rmin)[0][0]
+    ind_rmax = np.where(radar.range['data'] < rmax)[0][-1]
     r_res = radar.range['data'][1]-radar.range['data'][0]
-    min_rcons = int(dscfg['rcell']/r_res)
+    min_rcons = int(rcell/r_res)
 
     if psidp_field.startswith('corrected_'):
         phidp_field = psidp_field
     elif psidp_field.startswith('uncorrected_'):
         phidp_field = psidp_field.replace('uncorrected_', 'corrected_', 1)
     else:
         phidp_field = 'corrected_'+psidp_field
 
     try:
         phidp = pyart.correct.correct_sys_phase(
             radar, ind_rmin=ind_rmin, ind_rmax=ind_rmax, min_rcons=min_rcons,
-            zmin=dscfg['Zmin'], zmax=dscfg['Zmax'], psidp_field=psidp_field,
+            zmin=zmin, zmax=zmax, psidp_field=psidp_field,
             refl_field=refl_field, phidp_field=phidp_field)
     except AttributeError as e:
         warn('Could not find correct_sys_phase function...')
         warn('Skipping system phase correction...')
         warn('Please use PyART-MCH to get this functionality')
         phidp = radar.fields[phidp_field]
-     
+
     # prepare for exit
     new_dataset = {'radar_out': deepcopy(radar)}
     new_dataset['radar_out'].fields = dict()
     new_dataset['radar_out'].add_field(phidp_field, phidp)
 
     return new_dataset, ind_rad
 
@@ -136,25 +144,26 @@
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         rmin : float. Dataset keyword
-            The minimum range where to look for valid data [m]
+            The minimum range where to look for valid data [m]. Default 1000.
         rmax : float. Dataset keyword
-            The maximum range where to look for valid data [m]
+            The maximum range where to look for valid data [m]. Default 50000.
         rcell : float. Dataset keyword
-            The length of a continuous cell to consider it valid precip [m]
+            The length of a continuous cell to consider it valid precip [m].
+            Default 1000.
         rwind : float. Dataset keyword
-            The length of the smoothing window [m]
+            The length of the smoothing window [m]. Default 6000.
         Zmin : float. Dataset keyword
-            The minimum reflectivity [dBZ]
+            The minimum reflectivity [dBZ]. Default 20.
         Zmax : float. Dataset keyword
-            The maximum reflectivity [dBZ]
+            The maximum reflectivity [dBZ]. Default 40.
     radar_list : list of Radar objects
         Optional. list of radar objects
 
     Returns
     -------
     new_dataset : dict
         dictionary containing the output
@@ -185,31 +194,39 @@
         return None, None
     radar = radar_list[ind_rad]
 
     if (refl_field not in radar.fields) or (psidp_field not in radar.fields):
         warn('Unable to smooth PhiDP. Missing data')
         return None, None
 
-    ind_rmin = np.where(radar.range['data'] > dscfg['rmin'])[0][0]
-    ind_rmax = np.where(radar.range['data'] < dscfg['rmax'])[0][-1]
+    # user defined parameters
+    rmin = dscfg.get('rmin', 1000.)
+    rmax = dscfg.get('rmax', 50000.)
+    rcell = dscfg.get('rcell', 1000.)
+    zmin = dscfg.get('Zmin', 20.)
+    zmax = dscfg.get('Zmax', 40.)
+    rwind = dscfg.get('rwind', 6000.)
+
+    ind_rmin = np.where(radar.range['data'] > rmin)[0][0]
+    ind_rmax = np.where(radar.range['data'] < rmax)[0][-1]
     r_res = radar.range['data'][1]-radar.range['data'][0]
-    min_rcons = int(dscfg['rcell']/r_res)
-    wind_len = int(dscfg['rwind']/r_res)
+    min_rcons = int(rcell/r_res)
+    wind_len = int(rwind/r_res)
     min_valid = int(wind_len/2+1)
 
     if psidp_field.startswith('corrected_'):
         phidp_field = psidp_field
     elif psidp_field.startswith('uncorrected_'):
         phidp_field = psidp_field.replace('uncorrected_', 'corrected_', 1)
     else:
         phidp_field = 'corrected_'+psidp_field
 
     phidp = pyart.correct.smooth_phidp_single_window(
         radar, ind_rmin=ind_rmin, ind_rmax=ind_rmax, min_rcons=min_rcons,
-        zmin=dscfg['Zmin'], zmax=dscfg['Zmax'], wind_len=wind_len,
+        zmin=zmin, zmax=zmax, wind_len=wind_len,
         min_valid=min_valid, psidp_field=psidp_field, refl_field=refl_field,
         phidp_field=phidp_field)
 
     # prepare for exit
     new_dataset = {'radar_out': deepcopy(radar)}
     new_dataset['radar_out'].fields = dict()
     new_dataset['radar_out'].add_field(phidp_field, phidp)
@@ -281,35 +298,45 @@
         return None, None
     radar = radar_list[ind_rad]
 
     if (refl_field not in radar.fields) or (psidp_field not in radar.fields):
         warn('Unable to smooth PhiDP. Missing data')
         return None, None
 
-    ind_rmin = np.where(radar.range['data'] > dscfg['rmin'])[0][0]
-    ind_rmax = np.where(radar.range['data'] < dscfg['rmax'])[0][-1]
+    # user defined parameters
+    rmin = dscfg.get('rmin', 1000.)
+    rmax = dscfg.get('rmax', 50000.)
+    rcell = dscfg.get('rcell', 1000.)
+    zmin = dscfg.get('Zmin', 20.)
+    zmax = dscfg.get('Zmax', 40.)
+    rwinds = dscfg.get('rwinds', 2000.)
+    rwindl = dscfg.get('rwindl', 6000.)
+    zthr = dscfg.get('Zthr', 40.)
+
+    ind_rmin = np.where(radar.range['data'] > rmin)[0][0]
+    ind_rmax = np.where(radar.range['data'] < rmax)[0][-1]
     r_res = radar.range['data'][1]-radar.range['data'][0]
-    min_rcons = int(dscfg['rcell']/r_res)
-    swind_len = int(dscfg['rwinds']/r_res)
+    min_rcons = int(rcell/r_res)
+    swind_len = int(rwinds/r_res)
     smin_valid = int(swind_len/2+1)
-    lwind_len = int(dscfg['rwindl']/r_res)
+    lwind_len = int(rwindl/r_res)
     lmin_valid = int(lwind_len/2+1)
 
     if psidp_field.startswith('corrected_'):
         phidp_field = psidp_field
     elif psidp_field.startswith('uncorrected_'):
         phidp_field = psidp_field.replace('uncorrected_', 'corrected_', 1)
     else:
         phidp_field = 'corrected_'+psidp_field
 
     phidp = pyart.correct.smooth_phidp_double_window(
         radar, ind_rmin=ind_rmin, ind_rmax=ind_rmax, min_rcons=min_rcons,
-        zmin=dscfg['Zmin'], zmax=dscfg['Zmax'], swind_len=swind_len,
+        zmin=zmin, zmax=zmax, swind_len=swind_len,
         smin_valid=smin_valid, lwind_len=lwind_len, lmin_valid=lmin_valid,
-        zthr=dscfg['Zthr'], psidp_field=psidp_field, refl_field=refl_field,
+        zthr=zthr, psidp_field=psidp_field, refl_field=refl_field,
         phidp_field=phidp_field)
 
     # prepare for exit
     new_dataset = {'radar_out': deepcopy(radar)}
     new_dataset['radar_out'].fields = dict()
     new_dataset['radar_out'].add_field(phidp_field, phidp)
 
@@ -328,23 +355,24 @@
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         rmin : float. Dataset keyword
-            The minimum range where to look for valid data [m]
+            The minimum range where to look for valid data [m]. Default 1000.
         rmax : float. Dataset keyword
-            The maximum range where to look for valid data [m]
+            The maximum range where to look for valid data [m]. Default 50000.
         rcell : float. Dataset keyword
-            The length of a continuous cell to consider it valid precip [m]
+            The length of a continuous cell to consider it valid precip [m].
+            Default 1000.
         Zmin : float. Dataset keyword
-            The minimum reflectivity [dBZ]
+            The minimum reflectivity [dBZ]. Default 20
         Zmax : float. Dataset keyword
-            The maximum reflectivity [dBZ]
+            The maximum reflectivity [dBZ]. Default 40
         fzl : float. Dataset keyword
             The freezing level height [m]. Default 2000.
         ml_thickness : float. Dataset keyword
             The melting layer thickness in meters. Default 700.
         beamwidth : float. Dataset keyword
             the antenna beamwidth [deg]. If None that of the keys
             radar_beam_width_h or radar_beam_width_v in attribute
@@ -392,14 +420,22 @@
 
     if ((refl_field not in radar.fields) or
             (psidp_field not in radar.fields)):
         warn('Unable to retrieve PhiDP KDP using the Maesaka approach. ' +
              'Missing data')
         return None, None
 
+    # user defined parameters
+    rmin = dscfg.get('rmin', 1000.)
+    rmax = dscfg.get('rmax', 50000.)
+    rcell = dscfg.get('rcell', 1000.)
+    zmin = dscfg.get('Zmin', 20.)
+    zmax = dscfg.get('Zmax', 40.)
+    thickness = dscfg.get('ml_thickness', 700.)
+
     # determine which freezing level reference
     temp_ref = 'temperature'
     if temp_field is None and iso0_field is None:
         warn('Field to obtain the freezing level was not specified. ' +
              'Using fixed freezing level height')
         temp_ref = 'fixed_fzl'
     elif temp_field is not None:
@@ -421,66 +457,61 @@
         if 'fzl' in dscfg:
             fzl = dscfg['fzl']
         else:
             fzl = 2000.
             warn('Freezing level height not defined. Using default ' +
                  str(fzl)+' m')
 
-    thickness = 700.
-    if 'ml_thickness' in dscfg:
-        thickness = dscfg['ml_thickness']
-
     phidp_field = 'corrected_differential_phase'
     kdp_field = 'corrected_specific_differential_phase'
 
     radar_aux = deepcopy(radar)
 
     # correct PhiDP0
-    ind_rmin = np.where(radar_aux.range['data'] > dscfg['rmin'])[0][0]
-    ind_rmax = np.where(radar_aux.range['data'] < dscfg['rmax'])[0][-1]
+    ind_rmin = np.where(radar_aux.range['data'] > rmin)[0][0]
+    ind_rmax = np.where(radar_aux.range['data'] < rmax)[0][-1]
     r_res = radar_aux.range['data'][1]-radar_aux.range['data'][0]
-    min_rcons = int(dscfg['rcell']/r_res)
+    min_rcons = int(rcell/r_res)
 
     try:
         phidp = pyart.correct.correct_sys_phase(
-            radar_aux, ind_rmin=ind_rmin, ind_rmax=ind_rmax, min_rcons=min_rcons,
-            zmin=dscfg['Zmin'], zmax=dscfg['Zmax'], psidp_field=psidp_field,
-            refl_field=refl_field, phidp_field=phidp_field)
+            radar_aux, ind_rmin=ind_rmin, ind_rmax=ind_rmax,
+            min_rcons=min_rcons, zmin=zmin, zmax=zmax,
+            psidp_field=psidp_field, refl_field=refl_field,
+            phidp_field=phidp_field)
     except AttributeError as e:
         warn('Could not find correct_sys_phase function...')
         warn('Skipping system phase correction...')
         warn('Please use PyART-MCH to get this functionality')
         phidp = radar_aux.fields[phidp_field]
-        
+
     # filter out data in an above the melting layer
     mask = np.ma.getmaskarray(phidp['data'])
 
     beamwidth = dscfg.get('beamwidth', None)
     if beamwidth is None:
         if radar.instrument_parameters is not None:
             if 'radar_beam_width_h' in radar.instrument_parameters:
                 beamwidth = radar.instrument_parameters['radar_beam_width_h'][
                     'data'][0]
             elif 'radar_beam_width_v' in radar.instrument_parameters:
                 beamwidth = radar.instrument_parameters['radar_beam_width_v'][
                     'data'][0]
     if beamwidth is None:
         warn('Antenna beam width unknown.')
-        
+
     try:
         mask_fzl, _ = pyart.correct.get_mask_fzl(
             radar_aux, fzl=fzl, doc=15, min_temp=0., max_h_iso0=0.,
             thickness=thickness, beamwidth=beamwidth, temp_field=temp_field,
             iso0_field=iso0_field, temp_ref=temp_ref)
         mask = np.logical_or(mask, mask_fzl)
     except AttributeError as e:
         warn("Masking above FZL is only available in PyART-MCH")
         warn("Please use this library instead of ARM's version")
-    
-        
 
     # filter out data with invalid reflectivity
     mask_refl = np.ma.getmaskarray(radar_aux.fields[refl_field]['data'])
     mask = np.logical_or(mask, mask_refl)
 
     phidp['data'] = np.ma.masked_where(mask, phidp['data'])
     fill_value = pyart.config.get_fillvalue()
@@ -608,22 +639,19 @@
         if 'fzl' in dscfg:
             fzl = dscfg['fzl']
         else:
             fzl = 2000.
             warn('Freezing level height not defined. Using default ' +
                  str(fzl)+' m')
 
-    thickness = 700.
-    if 'ml_thickness' in dscfg:
-        thickness = dscfg['ml_thickness']
-
     radar_aux = deepcopy(radar)
 
     # user config
     LP_solver = dscfg.get('LP_solver', 'cvxopt')
+    thickness = dscfg.get('ml_thickness', 700.)
 
     # filter out data in an above the melting layer
     mask = np.ma.getmaskarray(radar_aux.fields[psidp_field]['data'])
     beamwidth = dscfg.get('beamwidth', None)
     if beamwidth is None:
         if radar.instrument_parameters is not None:
             if 'radar_beam_width_h' in radar.instrument_parameters:
@@ -683,15 +711,16 @@
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         rwind : float. Dataset keyword
-            The length of the segment for the least square method [m]
+            The length of the segment for the least square method [m].
+            Default 6000.
         vectorize : bool. Dataset keyword
             Whether to vectorize the KDP processing. Default false
     radar_list : list of Radar objects
         Optional. list of radar objects
 
     Returns
     -------
@@ -720,19 +749,22 @@
     radar = radar_list[ind_rad]
 
     if phidp_field not in radar.fields:
         warn('Unable to retrieve KDP from PhiDP using least square. ' +
              'Missing data')
         return None, None
 
+    # user defined parameters
+    rwind = dscfg.get('rwind', 6000.)
+    vectorize = dscfg.get('vectorize', False)
+
     r_res = radar.range['data'][1]-radar.range['data'][0]
-    wind_len = int(dscfg['rwind']/r_res)
+    wind_len = int(rwind/r_res)
     min_valid = int(wind_len/2+1)
     kdp_field = 'corrected_specific_differential_phase'
-    vectorize = dscfg.get('vectorize', False)
 
     kdp = pyart.retrieve.kdp_leastsquare_single_window(
         radar, wind_len=wind_len, min_valid=min_valid, phidp_field=phidp_field,
         kdp_field=kdp_field, vectorize=vectorize)
 
     # prepare for exit
     new_dataset = {'radar_out': deepcopy(radar)}
@@ -753,17 +785,19 @@
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         rwinds : float. Dataset keyword
-            The length of the short segment for the least square method [m]
+            The length of the short segment for the least square method [m].
+            Default 2000.
         rwindl : float. Dataset keyword
-            The length of the long segment for the least square method [m]
+            The length of the long segment for the least square method [m].
+            Default 6000.
         Zthr : float. Dataset keyword
             The threshold defining which estimated data to use [dBZ]
         vectorize : Bool. Dataset keyword
             Whether to vectorize the KDP processing. Default false
     radar_list : list of Radar objects
         Optional. list of radar objects
 
@@ -798,26 +832,31 @@
     radar = radar_list[ind_rad]
 
     if (phidp_field not in radar.fields) or (refl_field not in radar.fields):
         warn('Unable to retrieve KDP from PhiDP using least square. ' +
              'Missing data')
         return None, None
 
+    # user defined parameters
+    rwinds = dscfg.get('rwinds', 2000.)
+    rwindl = dscfg.get('rwindl', 6000.)
+    zthr = dscfg.get('Zthr', 40.)
+    vectorize = dscfg.get('vectorize', False)
+
     r_res = radar.range['data'][1]-radar.range['data'][0]
-    swind_len = int(dscfg['rwinds']/r_res)
+    swind_len = int(rwinds/r_res)
     smin_valid = int(swind_len/2+1)
-    lwind_len = int(dscfg['rwindl']/r_res)
+    lwind_len = int(rwindl/r_res)
     lmin_valid = int(lwind_len/2+1)
-    vectorize = dscfg.get('vectorize', False)
 
     kdp_field = 'corrected_specific_differential_phase'
 
     kdp = pyart.retrieve.kdp_leastsquare_double_window(
         radar, swind_len=swind_len, smin_valid=smin_valid,
-        lwind_len=lwind_len, lmin_valid=lmin_valid, zthr=dscfg['Zthr'],
+        lwind_len=lwind_len, lmin_valid=lmin_valid, zthr=zthr,
         phidp_field=phidp_field, refl_field=refl_field, kdp_field=kdp_field,
         vectorize=vectorize)
 
     # prepare for exit
     new_dataset = {'radar_out': deepcopy(radar)}
     new_dataset['radar_out'].fields = dict()
     new_dataset['radar_out'].add_field(kdp_field, kdp)
@@ -838,25 +877,25 @@
         2 post-processing
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         rwind : float. Dataset keyword
-            The length of the segment [m]
+            The length of the segment [m]. Default 2000.
         n_iter : int. Dataset keyword
-            number of iterations
+            number of iterations. Default 3.
         interp : boolean. Dataset keyword
             if set non valid values are interpolated using neighbouring valid
-            values
+            values. Default 0 (False)
         parallel : boolean. Dataset keyword
-            if set use parallel computing
+            if set use parallel computing. Default 1 (True)
         get_phidp : boolean. Datset keyword
             if set the PhiDP computed by integrating the resultant KDP is
-            added to the radar field
+            added to the radar field. Default 0 (False)
         frequency : float. Dataset keyword
             the radar frequency [Hz]. If None that of the key
             frequency in attribute instrument_parameters of the radar
             object will be used. If the key or the attribute are not present
             it will be assumed that the radar is C band
     radar_list : list of Radar objects
         Optional. list of radar objects
@@ -888,40 +927,27 @@
     radar = radar_list[ind_rad]
 
     if phidp_field not in radar.fields:
         warn('Unable to retrieve KDP from PhiDP using least square. ' +
              'Missing data')
         return None, None
 
-    # number of iterations
-    n_iter = 3
-    if 'n_iter' in dscfg:
-        n_iter = dscfg['n_iter']
+    # user defined parameters
+    n_iter = dscfg.get('n_iter', 3)
+    rwind = dscfg.get('rwind', 2000.)
+    interp = dscfg.get('interp', 0)
+    parallel = dscfg.get('parallel', 1)
+    get_phidp = dscfg.get('get_phidp', 0)
 
     # window length (must be even)
     r_res = radar.range['data'][1]-radar.range['data'][0]
-    wind_len = int(dscfg['rwind']/r_res)
+    wind_len = int(rwind/r_res)
     if wind_len % 2 == 1:
         wind_len += 1
 
-    # interpolate invalid values?
-    interp = 0
-    if 'interp' in dscfg:
-        interp = dscfg['interp']
-
-    # parallel computing?
-    parallel = 1
-    if 'parallel' in dscfg:
-        parallel = dscfg['parallel']
-
-    # get PhiDP computed from KDP?
-    get_phidp = 0
-    if 'get_phidp' in dscfg:
-        get_phidp = dscfg['get_phidp']
-
     # get band
     freq = dscfg.get('frequency', None)
     if freq is None:
         if (radar.instrument_parameters is not None and
                 'frequency' in radar.instrument_parameters):
             freq = radar.instrument_parameters['frequency']['data'][0]
 
@@ -1072,15 +1098,15 @@
     dscfg : dictionary of dictionaries
         data set configuration. Accepted Configuration Keywords::
 
         datatype : list of string. Dataset keyword
             The input data types
         ATT_METHOD : float. Dataset keyword
             The attenuation estimation method used. One of the following:
-            ZPhi, Philin
+            ZPhi, Philin. Default ZPhi
         fzl : float. Dataset keyword
             The default freezing level height. It will be used if no
             temperature field name is specified or the temperature field is
             not in the radar object. Default 2000.
     radar_list : list of Radar objects
         Optional. list of radar objects
```

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_retrieve.py` & `pyrad_mch-1.8.1/pyrad/proc/process_retrieve.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_spectra.py` & `pyrad_mch-1.8.1/pyrad/proc/process_spectra.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_timeseries.py` & `pyrad_mch-1.8.1/pyrad/proc/process_timeseries.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/proc/process_traj.py` & `pyrad_mch-1.8.1/pyrad/proc/process_traj.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/__init__.py` & `pyrad_mch-1.8.1/pyrad/prod/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_grid_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_grid_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_intercomp_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_intercomp_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_monitoring_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_monitoring_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_product.py` & `pyrad_mch-1.8.1/pyrad/prod/process_product.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_spectra_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_spectra_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_timeseries_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_timeseries_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_traj_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_traj_products.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/prod/process_vol_products.py` & `pyrad_mch-1.8.1/pyrad/prod/process_vol_products.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,32 +118,34 @@
                 altitude: flt
                     CAPPI altitude [m MSL]
                 wfunc: str
                     The function used to produce the CAPPI as defined in
                     pyart.map.grid_from_radars. Default 'NEAREST'
                 cappi_res: float
                     The CAPPI resolution [m]. Default 500.
-        'CROSS_SECTION' : Plots a cross-section of polar data through arbitrary coordinates
+        'CROSS_SECTION' : Plots a cross-section of polar data through
+            arbitrary coordinates
             User defined parameters:
                 coord1, coord2, ..., coordN: dict
                     The two lat-lon coordinates marking the limits. They have
-                    the keywords 'lat' and 'lon' [degree]. 
+                    the keywords 'lat' and 'lon' [degree].
                 step : int
                     Step in meters to use between reference points to calculate
                     the cross-section (i.e horizontal resolution).
                 vert_res : int
-                    Vertical resolution in meters used to calculate the cross-section 
+                    Vertical resolution in meters used to calculate the
+                    cross-section
                 alt_max : int
-                    Maximum altitude of the vertical cross-section 
+                    Maximum altitude of the vertical cross-section
                 beamwidth : float
-                    3dB beamwidth in degrees to be used in the calculations, if not provided
-                    will be read from the loc file
+                    3dB beamwidth in degrees to be used in the calculations,
+                    if not provided will be read from the loc file
                 demfile : str
-                    Name of the DEM file to use to plot the topography, it must be in the 
-                    dempath specified in the main config file
+                    Name of the DEM file to use to plot the topography, it
+                    must be in the dempath specified in the main config file
         'FIELD_COVERAGE': Gets the field coverage over a certain sector
             User defined parameters:
                 threshold: float or None
                     Minimum value to consider the data valid. Default None
                 nvalid_min: float
                     Minimum number of valid gates in the ray to consider it
                     valid. Default 5
@@ -2098,39 +2100,39 @@
                 ' Field type ' + field_name +
                 ' not available in data set. Skipping product ' +
                 prdcfg['type'])
             return None
 
         vmin = prdcfg.get('vmin', None)
         vmax = prdcfg.get('vmax', None)
-        
+
         step = prdcfg.get('step', 1000)
         vert_res = prdcfg.get('vert_res', 100)
         alt_max = prdcfg.get('alt_max', 10000)
         beamwidth = prdcfg.get('beamwidth', None)
-        if beamwidth == None:
+        if beamwidth is None:
             if 'RadarBeamwidth' in prdcfg:
                 beamwidth = prdcfg['RadarBeamwidth']
             else:
                 warn('Radar beamwidth not provided, assuming 1 deg')
                 beamwidth = 1
         demfile = prdcfg.get('demfile', None)
 
-        if demfile != None:
+        if demfile is not None:
             demproj = None
             if 'demproj' in prdcfg.keys():
                 demproj = prdcfg['demproj']
                 try:
                     demproj = int(demproj)
                 except ValueError:
                     # demproj is not an EPSG int
                     pass
 
             fname = prdcfg['dempath'][0] + prdcfg['demfile']
-            dem = read_dem(fname, projparams = demproj)
+            dem = read_dem(fname, projparams=demproj)
         else:
             dem = None
 
         # user defined values
         ref_pts = []
         i = 1
         while True:
@@ -2141,34 +2143,34 @@
                     coord_pt.append(prdcfg[coord]['lon'])
                 if 'lat' in prdcfg[coord]:
                     coord_pt.append(prdcfg[coord]['lat'])
                 ref_pts.append(coord_pt)
             else:
                 break
             i += 1
-        
-        ref_pts_str = '_'.join(['{:2.1f}-{:2.1f}'.format(pt[0], pt[1])
-             for pt in ref_pts])
+
+        ref_pts_str = '_'.join(
+            ['{:2.1f}-{:2.1f}'.format(pt[0], pt[1]) for pt in ref_pts])
         savedir = get_save_dir(
             prdcfg['basepath'], prdcfg['procname'], dssavedir,
             prdsavedir, timeinfo=prdcfg['timeinfo'])
 
         fname_list = make_filename(
             'cross_section', prdcfg['dstype'], prdcfg['voltype'],
             prdcfg['imgformat'],
             prdcfginfo='refpts_'+'{:s}'.format(ref_pts_str),
             timeinfo=prdcfg['timeinfo'], runinfo=prdcfg['runinfo'])
 
         for i, fname in enumerate(fname_list):
-                fname_list[i] = savedir+fname
+            fname_list[i] = savedir+fname
 
         plot_xsection(
             dataset['radar_out'], field_name, ref_pts, step, vert_res,
-            alt_max, beamwidth, dem, prdcfg, fname_list, vmin = vmin, 
-            vmax = vmax)
+            alt_max, beamwidth, dem, prdcfg, fname_list, vmin=vmin,
+            vmax=vmax)
 
         print('----- save to '+' '.join(fname_list))
 
         return fname_list
 
     if prdcfg['type'] == 'FIXED_RNG_IMAGE':
         field_name = get_fieldname_pyart(prdcfg['voltype'])
@@ -2518,14 +2520,16 @@
             warn(
                 ' Field type ' + field_name +
                 ' not available in data set. Skipping product ' +
                 prdcfg['type'])
             return None
 
         step = prdcfg.get('step', None)
+        vmin = prdcfg.get('vmin', None)
+        vmax = prdcfg.get('vmax', None)
         write_data = prdcfg.get('write_data', 0)
 
         savedir = get_save_dir(
             prdcfg['basepath'], prdcfg['procname'], dssavedir,
             prdsavedir, timeinfo=prdcfg['timeinfo'])
 
         fname_list = make_filename(
@@ -2534,15 +2538,15 @@
             timeinfo=prdcfg['timeinfo'], runinfo=prdcfg['runinfo'])
 
         for i, fname in enumerate(fname_list):
             fname_list[i] = savedir+fname
 
         bin_edges, values = compute_histogram(
             dataset['radar_out'].fields[field_name]['data'], field_name,
-            step=step)
+            step=step, vmin=vmin, vmax=vmax)
 
         titl = (
             pyart.graph.common.generate_radar_time_begin(
                 dataset['radar_out']).isoformat() + 'Z' + '\n' +
             get_field_name(
                 dataset['radar_out'].fields[field_name], field_name))
```

### Comparing `pyrad_mch-1.8.0/pyrad/prod/product_aux.py` & `pyrad_mch-1.8.1/pyrad/prod/product_aux.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/util/__init__.py` & `pyrad_mch-1.8.1/pyrad/util/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/util/radar_utils.py` & `pyrad_mch-1.8.1/pyrad/util/radar_utils.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad/util/stat_utils.py` & `pyrad_mch-1.8.1/pyrad/util/stat_utils.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/pyrad_mch.egg-info/PKG-INFO` & `pyrad_mch-1.8.1/pyrad_mch.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrad-mch
-Version: 1.8.0
+Version: 1.8.1
 Summary:  Python Radar Toolkit
 Home-page: https://github.com/MeteoSwiss/pyrad.git
 Author: MeteoSwiss Pyrad Developers
 Author-email: daniel.wolfensberger@meteoswiss.ch
 Maintainer: MeteoSwiss Pyrad Developers
 Maintainer-email: daniel.wolfensberger@meteoswiss.ch
 License: BSD
```

### Comparing `pyrad_mch-1.8.0/pyrad_mch.egg-info/SOURCES.txt` & `pyrad_mch-1.8.1/pyrad_mch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/common_colocated_gates.py` & `pyrad_mch-1.8.1/scripts/common_colocated_gates.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_precipitation_comparison.py` & `pyrad_mch-1.8.1/scripts/main_precipitation_comparison.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_cosmo.py` & `pyrad_mch-1.8.1/scripts/main_process_cosmo.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_cosmo_rt.py` & `pyrad_mch-1.8.1/scripts/main_process_cosmo_rt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_data.py` & `pyrad_mch-1.8.1/scripts/main_process_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_data_birds.py` & `pyrad_mch-1.8.1/scripts/main_process_data_birds.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_data_period.py` & `pyrad_mch-1.8.1/scripts/main_process_data_period.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_data_rt.py` & `pyrad_mch-1.8.1/scripts/main_process_data_rt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_data_trt.py` & `pyrad_mch-1.8.1/scripts/main_process_data_trt.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_euclid_data.py` & `pyrad_mch-1.8.1/scripts/main_process_euclid_data.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/main_process_gecsx.py` & `pyrad_mch-1.8.1/scripts/main_process_gecsx.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/movie_maker.py` & `pyrad_mch-1.8.1/scripts/movie_maker.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/scripts/rewrite_monitoring.py` & `pyrad_mch-1.8.1/scripts/rewrite_monitoring.py`

 * *Files identical despite different names*

### Comparing `pyrad_mch-1.8.0/setup.py` & `pyrad_mch-1.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 URL = "https://github.com/MeteoSwiss/pyrad.git"
 DOWNLOAD_URL = "https://github.com/MeteoSwiss/pyrad.git"
 LICENSE = 'BSD'
 CLASSIFIERS = list(filter(None, CLASSIFIERS.split('\n')))
 PLATFORMS = ["Linux"]
 MAJOR = 1
 MINOR = 8
-MICRO = 0
+MICRO = 1
 ISRELEASED = True
 VERSION = '%d.%d.%d' % (MAJOR, MINOR, MICRO)
 SCRIPTS = glob.glob('scripts/*')
 COMPILE_DATE_TIME = datetime.utcnow().strftime("%Y-%m-%d %H:%M")
 USERNAME = getpass.getuser()
```

