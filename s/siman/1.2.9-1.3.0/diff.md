# Comparing `tmp/siman-1.2.9.tar.gz` & `tmp/siman-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/siman-1.2.9.tar", last modified: Thu Jun  1 10:25:57 2023, max compression
+gzip compressed data, was "dist/siman-1.3.0.tar", last modified: Thu Jun  8 13:41:32 2023, max compression
```

## Comparing `siman-1.2.9.tar` & `siman-1.3.0.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.138047 siman-1.2.9/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.2.9/LICENSE
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.2.9/MANIFEST.in
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-01 10:25:57.138047 siman-1.2.9/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.2.9/README.md
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-06-01 10:25:57.139047 siman-1.2.9/setup.cfg
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-06-01 10:25:51.000000 siman-1.2.9/setup.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.136047 siman-1.2.9/siman/
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.2.9/siman/3d_plot.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.2.9/siman/SSHTools.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.2.9/siman/__init__.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49532 2022-09-29 10:57:16.000000 siman-1.2.9/siman/analysis.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.2.9/siman/analysis_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.136047 siman-1.2.9/siman/analyze/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/analyze/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.2.9/siman/analyze/segregation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.2.9/siman/approximation.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.2.9/siman/bands.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   125775 2023-05-22 16:36:10.000000 siman-1.2.9/siman/calc_manage.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.2.9/siman/calcul.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.137047 siman-1.2.9/siman/calculators/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/aims.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/gaussian.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/qe.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.2.9/siman/calculators/vasp.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.2.9/siman/calculators/vasp_old.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.137047 siman-1.2.9/siman/chg/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.2.9/siman/chg/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.2.9/siman/chg/chg_func.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.2.9/siman/chg/vasputil_chgarith_module.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.2.9/siman/classes.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.138047 siman-1.2.9/siman/core/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.2.9/siman/core/calculation.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/calculation_old.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.2.9/siman/core/cluster_batch_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/cluster_run_script.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.2.9/siman/core/molecule.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118077 2023-04-18 16:31:52.000000 siman-1.2.9/siman/core/structure.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20209 2022-12-15 17:24:44.000000 siman-1.2.9/siman/database.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.2.9/siman/default_project_conf.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.2.9/siman/dev_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.2.9/siman/dos_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.2.9/siman/fit_hex.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-05-24 11:04:51.000000 siman-1.2.9/siman/functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.2.9/siman/geo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14499 2023-06-01 09:41:19.000000 siman-1.2.9/siman/header.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.2.9/siman/helper_for_writing_beatiful_code.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.2.9/siman/impurity.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.2.9/siman/inout.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.2.9/siman/kpoints_functions.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.138047 siman-1.2.9/siman/mat_prop/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.2.9/siman/mat_prop/__init__.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.2.9/siman/mat_prop/mat_prop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.2.9/siman/matproj_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.2.9/siman/monte.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.2.9/siman/monte_functions.py
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.2.9/siman/neb.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.2.9/siman/pairs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.2.9/siman/picture_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.2.9/siman/plot_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4434 2023-04-06 13:23:01.000000 siman-1.2.9/siman/polaron.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.2.9/siman/polaron_hop.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.2.9/siman/polaron_mod.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.2.9/siman/project_funcs.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.2.9/siman/properties_2d.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.2.9/siman/properties_energy.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.2.9/siman/properties_lattice.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.2.9/siman/set_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.2.9/siman/simanrc.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.2.9/siman/small_classes.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.2.9/siman/small_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.2.9/siman/structure_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.2.9/siman/table_functions.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.2.9/siman/thermo.py
--rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.2.9/siman/workflow_utilities.py
-drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-01 10:25:57.136047 siman-1.2.9/siman.egg-info/
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/PKG-INFO
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/SOURCES.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/dependency_links.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/requires.txt
--rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-06-01 10:25:57.000000 siman-1.2.9/siman.egg-info/top_level.txt
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.328478 siman-1.3.0/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18047 2021-02-17 13:28:25.000000 siman-1.3.0/LICENSE
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       98 2021-02-17 13:28:25.000000 siman-1.3.0/MANIFEST.in
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-08 13:41:32.328478 siman-1.3.0/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      409 2021-02-17 13:28:25.000000 siman-1.3.0/README.md
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       38 2023-06-08 13:41:32.328478 siman-1.3.0/setup.cfg
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      989 2023-06-08 13:41:22.000000 siman-1.3.0/setup.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.324478 siman-1.3.0/siman/
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2473 2022-03-05 17:22:57.000000 siman-1.3.0/siman/3d_plot.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3140 2022-03-05 17:22:57.000000 siman-1.3.0/siman/SSHTools.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)       32 2021-02-17 13:28:25.000000 siman-1.3.0/siman/__init__.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49532 2022-09-29 10:57:16.000000 siman-1.3.0/siman/analysis.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    26024 2022-03-05 17:22:57.000000 siman-1.3.0/siman/analysis_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.325478 siman-1.3.0/siman/analyze/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.0/siman/analyze/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    10970 2022-09-20 15:22:50.000000 siman-1.3.0/siman/analyze/segregation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1160 2022-03-05 17:22:57.000000 siman-1.3.0/siman/approximation.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    16329 2022-03-05 17:22:57.000000 siman-1.3.0/siman/bands.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   126191 2023-06-08 13:23:28.000000 siman-1.3.0/siman/calc_manage.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1085 2022-03-05 17:22:57.000000 siman-1.3.0/siman/calcul.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.326479 siman-1.3.0/siman/calculators/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.0/siman/calculators/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3685 2022-09-20 15:22:50.000000 siman-1.3.0/siman/calculators/aims.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     8718 2022-09-20 15:22:50.000000 siman-1.3.0/siman/calculators/gaussian.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3769 2022-09-20 15:22:50.000000 siman-1.3.0/siman/calculators/qe.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    56510 2023-04-04 10:46:17.000000 siman-1.3.0/siman/calculators/vasp.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    38832 2022-09-20 15:22:50.000000 siman-1.3.0/siman/calculators/vasp_old.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.326479 siman-1.3.0/siman/chg/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2021-02-17 13:28:25.000000 siman-1.3.0/siman/chg/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     6771 2021-02-17 13:28:25.000000 siman-1.3.0/siman/chg/chg_func.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3718 2021-02-17 13:28:25.000000 siman-1.3.0/siman/chg/vasputil_chgarith_module.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    11072 2022-09-20 15:22:50.000000 siman-1.3.0/siman/classes.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.327479 siman-1.3.0/siman/core/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.0/siman/core/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    53303 2023-04-04 10:20:35.000000 siman-1.3.0/siman/core/calculation.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    45277 2022-09-20 15:22:50.000000 siman-1.3.0/siman/core/calculation_old.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    33337 2023-02-13 17:12:02.000000 siman-1.3.0/siman/core/cluster_batch_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     3698 2022-09-20 15:22:50.000000 siman-1.3.0/siman/core/cluster_run_script.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     2127 2022-09-20 15:22:50.000000 siman-1.3.0/siman/core/molecule.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)   118275 2023-06-08 13:38:57.000000 siman-1.3.0/siman/core/structure.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    20209 2022-12-15 17:24:44.000000 siman-1.3.0/siman/database.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3192 2022-03-05 17:22:57.000000 siman-1.3.0/siman/default_project_conf.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    10776 2022-03-05 17:22:57.000000 siman-1.3.0/siman/dev_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    32406 2022-12-09 18:12:22.000000 siman-1.3.0/siman/dos_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     9424 2022-03-05 17:22:57.000000 siman-1.3.0/siman/fit_hex.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    28048 2023-05-24 11:04:51.000000 siman-1.3.0/siman/functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   113841 2023-03-06 17:27:57.000000 siman-1.3.0/siman/geo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    14499 2023-06-01 09:41:19.000000 siman-1.3.0/siman/header.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      286 2022-03-05 17:22:57.000000 siman-1.3.0/siman/helper_for_writing_beatiful_code.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    40223 2022-09-20 15:22:50.000000 siman-1.3.0/siman/impurity.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    80434 2022-09-29 10:57:16.000000 siman-1.3.0/siman/inout.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     4642 2022-03-05 17:22:57.000000 siman-1.3.0/siman/kpoints_functions.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.328478 siman-1.3.0/siman/mat_prop/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        0 2022-09-20 15:22:50.000000 siman-1.3.0/siman/mat_prop/__init__.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1574 2022-09-20 15:22:50.000000 siman-1.3.0/siman/mat_prop/mat_prop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    45055 2022-09-29 10:57:16.000000 siman-1.3.0/siman/matproj_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    17009 2022-09-20 15:22:50.000000 siman-1.3.0/siman/monte.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      980 2022-03-05 17:22:57.000000 siman-1.3.0/siman/monte_functions.py
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)    31643 2022-09-20 15:22:50.000000 siman-1.3.0/siman/neb.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    44420 2021-02-17 13:28:25.000000 siman-1.3.0/siman/pairs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    49712 2023-01-25 18:10:57.000000 siman-1.3.0/siman/picture_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    25262 2022-03-05 17:22:57.000000 siman-1.3.0/siman/plot_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     5224 2023-06-08 13:41:02.000000 siman-1.3.0/siman/polaron.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2406 2022-03-05 17:22:57.000000 siman-1.3.0/siman/polaron_hop.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     3772 2022-09-29 10:57:16.000000 siman-1.3.0/siman/polaron_mod.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)   194580 2022-09-29 10:57:16.000000 siman-1.3.0/siman/project_funcs.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    22880 2022-03-05 17:22:57.000000 siman-1.3.0/siman/properties_2d.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1114 2022-03-05 17:22:57.000000 siman-1.3.0/siman/properties_energy.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1091 2022-03-05 17:22:57.000000 siman-1.3.0/siman/properties_lattice.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    30666 2023-04-04 10:53:58.000000 siman-1.3.0/siman/set_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     1352 2022-03-05 17:22:57.000000 siman-1.3.0/siman/simanrc.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)      174 2022-03-05 17:22:57.000000 siman-1.3.0/siman/small_classes.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     6565 2022-09-29 10:57:16.000000 siman-1.3.0/siman/small_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8328 2022-03-05 17:22:57.000000 siman-1.3.0/siman/structure_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     8854 2022-03-05 17:22:57.000000 siman-1.3.0/siman/table_functions.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)     2780 2022-03-05 17:22:57.000000 siman-1.3.0/siman/thermo.py
+-rwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)    18673 2022-03-05 17:22:57.000000 siman-1.3.0/siman/workflow_utilities.py
+drwxrwxr-x   0 d.aksenov  (1000) d.aksenov  (1000)        0 2023-06-08 13:41:32.325478 siman-1.3.0/siman.egg-info/
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)      935 2023-06-08 13:41:32.000000 siman-1.3.0/siman.egg-info/PKG-INFO
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)     1677 2023-06-08 13:41:32.000000 siman-1.3.0/siman.egg-info/SOURCES.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        1 2023-06-08 13:41:32.000000 siman-1.3.0/siman.egg-info/dependency_links.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)       76 2023-06-08 13:41:32.000000 siman-1.3.0/siman.egg-info/requires.txt
+-rw-rw-r--   0 d.aksenov  (1000) d.aksenov  (1000)        6 2023-06-08 13:41:32.000000 siman-1.3.0/siman.egg-info/top_level.txt
```

### Comparing `siman-1.2.9/LICENSE` & `siman-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/PKG-INFO` & `siman-1.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.2.9
+Version: 1.3.0
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.2.9/setup.py` & `siman-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools, os
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="siman",
-    version="1.2.9",
+    version="1.3.0",
     author="Dmitry Aksenov",
     author_email="dimonaks@gmail.com",
     description="Manager for DFT calculations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/dimonaks/siman",
     license = 'GPL',
```

### Comparing `siman-1.2.9/siman/3d_plot.py` & `siman-1.3.0/siman/3d_plot.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/SSHTools.py` & `siman-1.3.0/siman/SSHTools.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/analysis.py` & `siman-1.3.0/siman/analysis.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/analysis_functions.py` & `siman-1.3.0/siman/analysis_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/analyze/segregation.py` & `siman-1.3.0/siman/analyze/segregation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/approximation.py` & `siman-1.3.0/siman/approximation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/bands.py` & `siman-1.3.0/siman/bands.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/calc_manage.py` & `siman-1.3.0/siman/calc_manage.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,14 +630,15 @@
             using *scale_region*  and *n_scale_images* (see *scale_cell_uniformly()*)
             The copies are available as versions from 1 to *n_scale_images* and
             suffix .su, .sc, or .sm appended to *it* name
             Copies to cluster *fit* utility that finds volume corresp. to energy minimum, creates 100.POSCAR and continues run 
             - 'monte' - Monte-Carlo functionality
 
             - 'polaron' - polaron hopping, only input_st is supported
+                - put here all parameters
 
             - 'atat' - create all input for ATAT
                 params['atat']
                     - 'active_atoms' - now dictionary of elements, which can be substituted by what e.g. {'Li':'Vac'}
                     please improve that Li0 can be used, to consider only symmetrically non-equivalent position for this element
                     - 'exclude_atoms_n' - exclude specific atoms from cluster expansion
                     - 'subatom' -  a string for choosing different POTCAR, e.g. 's/K/K_pv/g'
@@ -870,17 +871,25 @@
                 section_folder = struct_des[it].sfolder
 
             add_des(struct_des, it_new, section_folder, 'scale: scaled "images" for '+it+'.'+str(setlist)+'.'+str(v)   )
 
 
 
         if ('polaron' in calc_method) or ('polaron2' in calc_method):
+            """
+            if existing then magmom_polaron1 and magmom_polaron2 are not working 
+
+
+            """
             pm = params['polaron']
             am = abs(pm['amp']) # amplitude of polaron, the sign is not important here
 
+            magmom_polaron1 = pm.get('magmom_polaron1') # magnetic moment on TM atom after creation of polaron
+            magmom_polaron2 = pm.get('magmom_polaron2') # magnetic moment on TM atom after creation of polaron
+
             existing = pm.get('polaron_status') and 'ex' in pm.get('polaron_status') 
             nn = pm.get('nn') or 6
             # if pm.get('st1') and pm.get('st2'):
 
             if pm['polaron_type'] == 'electron':
                 if existing:
                     ''
@@ -926,16 +935,16 @@
             else:
                 if existing:
                     st1 = copy.deepcopy(input_st)
                     st2 = input_st.localize_polaron(pm['iend'], am, nn)
                     st2 = st2.localize_polaron(pm['istart'], -am, nn) # return back existing polaron to normal
 
                 else:
-                    st1 = input_st.localize_polaron(pm['istart'],  am, nn)
-                    st2 = input_st.localize_polaron(pm['iend'], am, nn)
+                    st1 = input_st.localize_polaron(pm['istart'],  am, nn, magmom_polaron1 )
+                    st2 = input_st.localize_polaron(pm['iend'], am, nn, magmom_polaron2)
 
 
 
                 st1_vis = st1.replace_atoms([pm['istart']], 'U')
                 st2_vis = st2.replace_atoms([pm['iend']], 'U')
             st1_vis.write_poscar('xyz/'+it+'/1.POSCAR')
             st2_vis.write_poscar('xyz/'+it+'/100.POSCAR')
```

### Comparing `siman-1.2.9/siman/calcul.py` & `siman-1.3.0/siman/calcul.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/calculators/aims.py` & `siman-1.3.0/siman/calculators/aims.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/calculators/gaussian.py` & `siman-1.3.0/siman/calculators/gaussian.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/calculators/qe.py` & `siman-1.3.0/siman/calculators/qe.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/calculators/vasp.py` & `siman-1.3.0/siman/calculators/vasp.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/calculators/vasp_old.py` & `siman-1.3.0/siman/calculators/vasp_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/chg/chg_func.py` & `siman-1.3.0/siman/chg/chg_func.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/chg/vasputil_chgarith_module.py` & `siman-1.3.0/siman/chg/vasputil_chgarith_module.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/classes.py` & `siman-1.3.0/siman/classes.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/core/calculation.py` & `siman-1.3.0/siman/core/calculation.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/core/calculation_old.py` & `siman-1.3.0/siman/core/calculation_old.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/core/cluster_batch_script.py` & `siman-1.3.0/siman/core/cluster_batch_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/core/cluster_run_script.py` & `siman-1.3.0/siman/core/cluster_run_script.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/core/molecule.py` & `siman-1.3.0/siman/core/molecule.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/core/structure.py` & `siman-1.3.0/siman/core/structure.py`

 * *Files 0% similar despite different names*

```diff
@@ -3014,22 +3014,23 @@
 
 
 
 
 
 
 
-    def localize_polaron(self, i, d, nn = 6):
+    def localize_polaron(self, i, d, nn = 6, magmom = None):
         """
         Localize small polaron at transition metal by adjusting TM-A distances
 
         INPUT:
             - i (int) - number of transition atom, from 0
             - d (float) - shift in angstrom; positive increase TM-O, negative reduce TM-O distance
             - nn (int) - number of neigbours
+            - magmom (float) - magnetic moment on atom with polaron
 
         RETURN:
 
             - st (Structure) - structure with localized polaron at atom i
 
         AUTHOR:
 
@@ -3078,14 +3079,19 @@
         st.update_xred()
 
         dic = st.nn(i, nn, from_one = 0, silent = silent)
         printlog('Average '+TM_name+'-'+str(unique_neighbours_els)+' distance after localization is {:.2f} A'.format(dic['av']), imp = 'n')
 
         st.name+='pol'+str(i+1)
 
+        if magmom and len(st.magmom) == st.natom:
+            print(st.magmom)
+            st.magmom[i] = magmom
+
+
         return st
 
     def localize_ox_polaron(self, i, d_a, d_tm, nn = 6, mag = None):
         """
         Localize small polaron at oxygen atom by adjusting distances
         i - number of oxygen, from 0
         d_a - shift in angstrom; positive increase Li-O bonds, negative reduce Li-O bonds
```

### Comparing `siman-1.2.9/siman/database.py` & `siman-1.3.0/siman/database.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/default_project_conf.py` & `siman-1.3.0/siman/default_project_conf.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/dev_functions.py` & `siman-1.3.0/siman/dev_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/dos_functions.py` & `siman-1.3.0/siman/dos_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/fit_hex.py` & `siman-1.3.0/siman/fit_hex.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/functions.py` & `siman-1.3.0/siman/functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/geo.py` & `siman-1.3.0/siman/geo.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/header.py` & `siman-1.3.0/siman/header.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/impurity.py` & `siman-1.3.0/siman/impurity.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/inout.py` & `siman-1.3.0/siman/inout.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/kpoints_functions.py` & `siman-1.3.0/siman/kpoints_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/mat_prop/mat_prop.py` & `siman-1.3.0/siman/mat_prop/mat_prop.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/matproj_functions.py` & `siman-1.3.0/siman/matproj_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/monte.py` & `siman-1.3.0/siman/monte.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/monte_functions.py` & `siman-1.3.0/siman/monte_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/neb.py` & `siman-1.3.0/siman/neb.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/pairs.py` & `siman-1.3.0/siman/pairs.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/picture_functions.py` & `siman-1.3.0/siman/picture_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/plot_functions.py` & `siman-1.3.0/siman/plot_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/polaron.py` & `siman-1.3.0/siman/polaron_mod.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,30 +14,32 @@
 42+images - polaron at final position, deformation at start position (SP)
 43:43+images -  intermediate deformation between end and start  (SP)
 
 
 """
 
 import sys, json, os, glob, copy
+print('Python version is', sys.version)
 from shutil import copyfile
 import random
 
 from os.path import expanduser
 home = expanduser("~")
+print(home)
 sys.path.append(home+'/tools/') # for numpy libraries
+sys.path.append(home+'/tools/siman/') # 
 import numpy as np
-
 from siman import header
 from siman.monte_functions import metropolis
 from siman.header import runBash, printlog
 from siman.header import ALKALI_ION_ELEMENTS as AM
 from siman.header import TRANSITION_ELEMENTS as TM
 from siman.classes import CalculationVasp, Structure
 from siman.inout import read_poscar
-from siman.functions import invert
+from siman.functions import invert, update_incar
 from siman.analysis import suf_en
 from siman.monte import vasp_run
 from siman.geo import interpolate
 debug2 = 0
 
 
 def copy_vasp_files(v):
@@ -64,77 +66,58 @@
 
 
     debug = 0
 
     header.warnings = 'yY'
     # header.warnings = 'neyY'
     header.verbose_log = 1
-    printlog('Python version is', sys.version)
 
     printlog('\n\n\nStarting Polaron hop script!\n', imp = 'y')
     
     """0. Read configuration file """
     if os.path.exists('conf.json'):
         with open('conf.json', 'r') as fp:
             params = json.load(fp)
     else:
         printlog('Warning! no configuration file conf.json, exiting')
         sys.exit()
         params = {}
 
+  
     vasprun_command = params.get('vasp_run') or 'vasp'
     images = params.get('images') or 3 # number of images
-    mode   = params.get('mode') or 'inherit' # mode type
+    mode   = params.get('mode') or 'inherit' # number of images
     magmom = params.get('magmom') or None
 
-    printlog('Choosing mode', mode, imp = 'y')
 
+    for i in [1,2]:
+        path_i = params.get(f'path{i}')
+        for pp in ['charge','output']:
+            path_ii = path_i[pp]
+            ftype = path_ii.split('.')[-1]              
+            runBash(f'cp {home}/{path_ii} {i}.{ftype}')
+
+
+    cl1 = CalculationVasp(output = '1.OUTCAR')
+    cl1.read_results(show = 'fo')
+
+    cl2 = CalculationVasp(output = '2.OUTCAR')
+    cl2.read_results(show = 'fo')
+
+
+    update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
+    runBash('cp 1.CHGCAR  CHGCAR')
+    interpolate(cl1.end, cl2.end, images, 21, omit_edges = 0)
+    for v in range(21, 21+images):
+        vasp_step(v, 'Intermediate position'+str(v), rm = 0 )
 
+    runBash('rm CHGCAR WAVECAR;  cp 2.CHGCAR CHGCAR')
 
-    if mode =='independent':
-        if 1:
-            """1. Calculate (relax) initial and final positions """
-            
-
-            cl1 = vasp_step(1, 'Start position', 1)
-            cl2 = vasp_step(2, 'End position', 1 )
-            
-        else:
-            cl1 = CalculationVasp(output = '1.OUTCAR')
-            cl1.read_results(show = 'fo')
-            cl2 = CalculationVasp(output = '2.OUTCAR')
-            cl2.read_results(show = 'fo')
-
-        """2. Create intermediate steps"""
-        interpolate(cl1.end, cl2.end, images, 3)
-        printlog('Interpolation was successful!\n', imp = 'y')
-
-        """3. Calculate energies of intermediate steps"""
-        cl1.update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
-        
-        for v in range(3, 3+images):
-
-            vasp_step(v, 'Intermediate position '+str(v), 1 )
-
-    elif mode =='inherit':
-
-        #from initial to last
-        cl2 = vasp_step(2, 'End position', 1 )
-        cl1 = vasp_step(1, 'Start position', 0)
-        # copyfile(str(v)+'.POSCAR', 'POSCAR')
-        cl1.update_incar(parameter = 'NSW', value = 0, run = 1, write = 0)
-        
-        interpolate(cl1.end, cl2.end, images, 21, omit_edges = 0)
-        for v in range(21, 21+images):
-            vasp_step(v, 'Intermediate position '+str(v), rm = 0 )
-
-        runBash('rm CHGCAR WAVECAR; gunzip 2.CHGCAR.gz; mv 2.CHGCAR CHGCAR')
-
-        interpolate(cl2.end, cl1.end, images, 42, omit_edges = 0)
-        for v in range(42, 42+images):
-            vasp_step(v, 'Intermediate position'+str(v), rm = 0 )
+    interpolate(cl2.end, cl1.end, images, 42, omit_edges = 0)
+    for v in range(42, 42+images):
+        vasp_step(v, 'Intermediate position'+str(v), rm = 0 )
 
 
 
 
     runBash('rm CHG WAVECAR')
-    printlog('PH simulation finished!', imp = 'y')
+    printlog('PH simulation finished!', imp = 'y')
```

### Comparing `siman-1.2.9/siman/polaron_hop.py` & `siman-1.3.0/siman/polaron_hop.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/project_funcs.py` & `siman-1.3.0/siman/project_funcs.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/properties_2d.py` & `siman-1.3.0/siman/properties_2d.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/properties_energy.py` & `siman-1.3.0/siman/properties_energy.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/properties_lattice.py` & `siman-1.3.0/siman/properties_lattice.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/set_functions.py` & `siman-1.3.0/siman/set_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/simanrc.py` & `siman-1.3.0/siman/simanrc.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/small_functions.py` & `siman-1.3.0/siman/small_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/structure_functions.py` & `siman-1.3.0/siman/structure_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/table_functions.py` & `siman-1.3.0/siman/table_functions.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/thermo.py` & `siman-1.3.0/siman/thermo.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman/workflow_utilities.py` & `siman-1.3.0/siman/workflow_utilities.py`

 * *Files identical despite different names*

### Comparing `siman-1.2.9/siman.egg-info/PKG-INFO` & `siman-1.3.0/siman.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: siman
-Version: 1.2.9
+Version: 1.3.0
 Summary: Manager for DFT calculations
 Home-page: https://github.com/dimonaks/siman
 Author: Dmitry Aksenov
 Author-email: dimonaks@gmail.com
 License: GPL
 Keywords: DFT VASP Density Functional Theory NEB DFT+U PAW GGA Monte-Carlo
 Platform: UNKNOWN
```

### Comparing `siman-1.2.9/siman.egg-info/SOURCES.txt` & `siman-1.3.0/siman.egg-info/SOURCES.txt`

 * *Files identical despite different names*

