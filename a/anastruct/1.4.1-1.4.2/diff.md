# Comparing `tmp/anastruct-1.4.1.tar.gz` & `tmp/anastruct-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anastruct-1.4.1.tar", last modified: Mon Feb 20 12:09:47 2023, max compression
+gzip compressed data, was "anastruct-1.4.2.tar", last modified: Thu Jun  8 08:22:47 2023, max compression
```

## Comparing `anastruct-1.4.1.tar` & `anastruct-1.4.2.tar`

### file list

```diff
@@ -1,92 +1,96 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.854042 anastruct-1.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35046 2023-02-20 12:08:49.000000 anastruct-1.4.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-02-20 12:08:49.000000 anastruct-1.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-02-20 12:09:47.854042 anastruct-1.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4323 2023-02-20 12:08:49.000000 anastruct-1.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.846042 anastruct-1.4.1/anastruct/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/basic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.846042 anastruct-1.4.1/anastruct/cython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/cython/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/cython/cbasic.pyx
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.846042 anastruct-1.4.1/anastruct/fem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.846042 anastruct-1.4.1/anastruct/fem/cython/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/cython/celements.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/cython/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    12481 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/elements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.850042 anastruct-1.4.1/anastruct/fem/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_1.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_10_dead_load.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_11.py
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_12.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_13.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_14.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_15.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_16.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_17_gnl.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_18_discretize.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_19_num_displacements.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_1_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      539 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_2.py
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_20_insert_node.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_21_rotate_force.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_22_loadcombination_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_23_sectionbase.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_24_envelope_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_25_high_midspan_point.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_26_deflection.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_3.py
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_4.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_5.py
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_6_fixed_hinge.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_7_rotational_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)      881 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_8_non_linear_portal.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/examples/ex_9_vertical_spring.py
--rw-r--r--   0 runner    (1001) docker     (123)     3245 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.850042 anastruct-1.4.1/anastruct/fem/plotter/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/plotter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4963 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/plotter/element.py
--rw-r--r--   0 runner    (1001) docker     (123)    34898 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/plotter/mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/plotter/null.py
--rw-r--r--   0 runner    (1001) docker     (123)     4246 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/plotter/values.py
--rw-r--r--   0 runner    (1001) docker     (123)    10383 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    59958 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.850042 anastruct-1.4.1/anastruct/fem/system_components/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/system_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10424 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/system_components/assembly.py
--rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/system_components/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5083 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/system_components/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.850042 anastruct-1.4.1/anastruct/fem/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5202 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/fem/util/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.850042 anastruct-1.4.1/anastruct/material/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/material/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/material/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/material/units.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.850042 anastruct-1.4.1/anastruct/sectionbase/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.854042 anastruct-1.4.1/anastruct/sectionbase/data/
--rw-r--r--   0 runner    (1001) docker     (123)  1347014 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/data/sectionbase_AmericanSectionDatabase.xml
--rw-r--r--   0 runner    (1001) docker     (123)   816237 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/data/sectionbase_BritishSectionDatabase.xml
--rw-r--r--   0 runner    (1001) docker     (123)   861354 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/data/sectionbase_EuropeanSectionDatabase.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/properties.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/sectionbase.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/sectionbase/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3159 2023-02-20 12:08:49.000000 anastruct-1.4.1/anastruct/vertex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.846042 anastruct-1.4.1/anastruct.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4697 2023-02-20 12:09:47.000000 anastruct-1.4.1/anastruct.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-02-20 12:09:47.000000 anastruct-1.4.1/anastruct.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-20 12:09:47.000000 anastruct-1.4.1/anastruct.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-20 12:09:47.000000 anastruct-1.4.1/anastruct.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-20 12:09:47.000000 anastruct-1.4.1/anastruct.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-20 12:09:47.854042 anastruct-1.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-02-20 12:08:49.000000 anastruct-1.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-20 12:09:47.854042 anastruct-1.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27911 2023-02-20 12:08:49.000000 anastruct-1.4.1/tests/test_e2e.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-02-20 12:08:49.000000 anastruct-1.4.1/tests/test_plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-02-20 12:08:49.000000 anastruct-1.4.1/tests/test_sectionbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.046922 anastruct-1.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    35046 2023-06-08 08:21:16.000000 anastruct-1.4.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 08:21:16.000000 anastruct-1.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-08 08:22:47.046922 anastruct-1.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4243 2023-06-08 08:21:16.000000 anastruct-1.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-06-08 08:21:16.000000 anastruct-1.4.2/_custom_build.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.022922 anastruct-1.4.2/anastruct/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/basic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.026922 anastruct-1.4.2/anastruct/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   176283 2023-06-08 08:21:27.000000 anastruct-1.4.2/anastruct/cython/basic.c
+-rw-r--r--   0 runner    (1001) docker     (123)      671 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/cython/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/cython/cbasic.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.026922 anastruct-1.4.2/anastruct/fem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.030922 anastruct-1.4.2/anastruct/fem/cython/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/cython/celements.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)   199972 2023-06-08 08:21:27.000000 anastruct-1.4.2/anastruct/fem/cython/elements.c
+-rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/cython/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12582 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/elements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.038922 anastruct-1.4.2/anastruct/fem/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_10_dead_load.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_11.py
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_12.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_13.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_14.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_15.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_16.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_17_gnl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_18_discretize.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_19_num_displacements.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_1_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      539 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_20_insert_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_21_rotate_force.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_22_loadcombination_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_23_sectionbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_24_envelope_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_25_high_midspan_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_26_deflection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_3.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_4.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_6_fixed_hinge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_7_rotational_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)      881 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_8_non_linear_portal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/examples/ex_9_vertical_spring.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.042922 anastruct-1.4.2/anastruct/fem/plotter/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/plotter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/plotter/element.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36997 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/plotter/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/plotter/null.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/plotter/values.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    60197 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.042922 anastruct-1.4.2/anastruct/fem/system_components/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/system_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10715 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/system_components/assembly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4834 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/system_components/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/system_components/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.042922 anastruct-1.4.2/anastruct/fem/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/fem/util/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.046922 anastruct-1.4.2/anastruct/material/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/material/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/material/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/material/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.046922 anastruct-1.4.2/anastruct/sectionbase/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/sectionbase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/sectionbase/properties.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4654 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/sectionbase/sectionbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/sectionbase/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-08 08:21:16.000000 anastruct-1.4.2/anastruct/vertex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.026922 anastruct-1.4.2/anastruct.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5260 2023-06-08 08:22:46.000000 anastruct-1.4.2/anastruct.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-08 08:22:47.000000 anastruct-1.4.2/anastruct.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:22:46.000000 anastruct-1.4.2/anastruct.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 08:22:46.000000 anastruct-1.4.2/anastruct.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 08:22:46.000000 anastruct-1.4.2/anastruct.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 08:21:16.000000 anastruct-1.4.2/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 08:21:16.000000 anastruct-1.4.2/plot_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-06-08 08:21:16.000000 anastruct-1.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 08:21:16.000000 anastruct-1.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:22:47.046922 anastruct-1.4.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 08:21:16.000000 anastruct-1.4.2/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:47.046922 anastruct-1.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    38349 2023-06-08 08:21:16.000000 anastruct-1.4.2/tests/test_e2e.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-08 08:21:16.000000 anastruct-1.4.2/tests/test_plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7306 2023-06-08 08:21:16.000000 anastruct-1.4.2/tests/test_sectionbase.py
```

### Comparing `anastruct-1.4.1/LICENSE.txt` & `anastruct-1.4.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/PKG-INFO` & `anastruct-1.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,10 @@
-Metadata-Version: 2.1
-Name: anastruct
-Version: 1.4.1
-Summary: analyse 2D structures.
-Home-page: https://ritchievink.com
-Download-URL: https://github.com/ritchie46/anaStruct
-Author: Ritchie Vink
-Author-email: ritchie46@gmail.com
-License: GPL-3.0
-Description-Content-Type: text/markdown
-Provides-Extra: plot
-Provides-Extra: test
-Provides-Extra: dev
-License-File: LICENSE.txt
-
 # anaStruct 2D Frames and Trusses
-![tests and fmt](https://github.com/ritchie46/anaStruct/workflows/tests%20and%20fmt/badge.svg)
+[![Python tests](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml/badge.svg)](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml)
 [![Documentation Status](https://readthedocs.org/projects/anastruct/badge/?version=latest)](http://anastruct.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/anaStruct/lobby.svg)](https://gitter.im/anaStruct/lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 Analyse 2D Frames and trusses for slender structures. Determine the bending moments, shear forces, axial forces and displacements.
 
 ## Installation
 
 For the actively developed version:
 ```
```

### Comparing `anastruct-1.4.1/README.md` & `anastruct-1.4.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,35 @@
+Metadata-Version: 2.1
+Name: anastruct
+Version: 1.4.2
+Summary: Finite element analysis of 2D structures
+Author-email: Ritchie Vink <ritchie46@gmail.com>
+Maintainer-email: Brooks Smith <smith120bh@gmail.com>
+License: GPL-3.0
+Project-URL: homepage, https://github.com/ritchie46/anaStruct
+Project-URL: documentation, http://anastruct.readthedocs.io
+Project-URL: author, https://ritchievink.com
+Keywords: FEA,finite element,structural engineering,structural analysis
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Provides-Extra: plot
+Provides-Extra: test
+Provides-Extra: dev
+License-File: LICENSE.txt
+
 # anaStruct 2D Frames and Trusses
-![tests and fmt](https://github.com/ritchie46/anaStruct/workflows/tests%20and%20fmt/badge.svg)
+[![Python tests](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml/badge.svg)](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml)
 [![Documentation Status](https://readthedocs.org/projects/anastruct/badge/?version=latest)](http://anastruct.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/anaStruct/lobby.svg)](https://gitter.im/anaStruct/lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 Analyse 2D Frames and trusses for slender structures. Determine the bending moments, shear forces, axial forces and displacements.
 
 ## Installation
 
 For the actively developed version:
 ```
```

### Comparing `anastruct-1.4.1/anastruct/basic.py` & `anastruct-1.4.2/anastruct/basic.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,77 +1,88 @@
 import collections.abc
+from typing import Any, Sequence, Tuple
+
 import numpy as np
 
 try:
     from anastruct.cython.cbasic import (  # type: ignore # pylint: disable=unused-import
-        converge,
         angle_x_axis,
+        converge,
     )
 except ImportError:
-    from anastruct.cython.basic import converge, angle_x_axis  # type: ignore
+    from anastruct.cython.basic import angle_x_axis, converge
 
 
-def find_nearest(array, value):
+def find_nearest(array: np.ndarray, value: float) -> Tuple[float, int]:
     """
     :param array: (numpy array object)
     :param value: (float) value searched for
     :return: (tuple) nearest value, index
     """
     # Subtract the value of the value's in the array. Make the values absolute.
     # The lowest value is the nearest.
     index = (np.abs(array - value)).argmin()
     return array[index], index
 
 
-def integrate_array(y, dx):
+def integrate_array(y: np.ndarray, dx: float) -> np.ndarray:
     """
     integrate array y * dx
     """
-    return np.cumsum(y) * dx
+    return np.cumsum(y) * dx  # type: ignore
 
 
 class FEMException(Exception):
-    def __init__(self, type_, message):
+    def __init__(self, type_: str, message: str):
         self.type = type_
         self.message = message
 
 
-def args_to_lists(*args):
+def arg_to_list(arg: Any, n: int) -> list:
+    if isinstance(arg, Sequence) and not isinstance(arg, str) and len(arg) == n:
+        return list(arg)
+    elif isinstance(arg, Sequence) and not isinstance(arg, str) and len(arg) == 1:
+        return [arg[0] for _ in range(n)]
+    else:
+        return [arg for _ in range(n)]
+
+
+def args_to_lists(*args: list) -> list:
     arg_lists = []
     for arg in args:
         if isinstance(arg, collections.abc.Iterable) and not isinstance(arg, str):
             arg_lists.append(arg)
         else:
             arg_lists.append([arg])
     lengths = list(map(len, arg_lists))
     n = max(lengths)
     if n == 1:
         return arg_lists
 
-    args = []
+    args_return = []
     for arg, l in zip(arg_lists, lengths):
         if l == n:
-            args.append(arg)
+            args_return.append(arg)
         else:
-            args.append([arg[0] for _ in range(n)])
-    return args
+            args_return.append([arg[0] for _ in range(n)])
+    return args_return
 
 
-def rotation_matrix(angle):
+def rotation_matrix(angle: float) -> np.ndarray:
     """
 
     :param angle: (flt) angle in radians
     :return: rotated euclidean xy matrix
     """
     s = np.sin(angle)
     c = np.cos(angle)
     return np.array([[c, -s], [s, c]])
 
 
-def rotate_xy(a, angle):
+def rotate_xy(a: np.ndarray, angle: float) -> np.ndarray:
     b = np.array(a)
     b[:, 0] -= a[0, 0]
     b[:, 1] -= a[0, 1]
     b = np.dot(b, rotation_matrix(angle))
     b[:, 0] += a[0, 0]
     b[:, 1] += a[0, 1]
     return b
```

### Comparing `anastruct-1.4.1/anastruct/cython/basic.py` & `anastruct-1.4.2/anastruct/cython/cbasic.pyx`

 * *Files 16% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-import math
+from libc.stdlib cimport abs
+from libc.math cimport acos, sqrt, pi, abs
 
-
-def converge(lhs, rhs):
+cpdef converge(double lhs, double rhs):
     """
     Determine convergence factor.
 
     :param lhs: (flt)
     :param rhs: (flt)
     :param div: (flt)
     :return: multiplication factor (flt) ((lhs / rhs) - 1) / div + 1
     """
     lhs = abs(lhs)
     rhs = abs(rhs)
-    div = max(lhs, rhs) / min(lhs, rhs) * 2
-
-    return (rhs / lhs - 1) / div + 1
-
+    # cdef double div
+    div = max(lhs, rhs) / min(lhs, rhs) * 2.0
+    return (abs(rhs) / abs(lhs) - 1.0) / div + 1.0
 
-def angle_x_axis(delta_x, delta_z):
+cpdef angle_x_axis(double delta_x, double delta_z):
+    cdef double ai
     # dot product v_x = [1, 0] ; v = [delta_x, delta_z]
     # dot product = 1 * delta_x + 0 * delta_z -> delta_x
-    ai = math.acos(delta_x / math.sqrt(delta_x**2 + delta_z**2))
+    ai = acos(delta_x / sqrt(delta_x**2 + delta_z**2))
     if delta_z < 0:
-        ai = 2 * math.pi - ai
+        ai = 2 * pi - ai
 
-    return ai
+    return ai
```

### Comparing `anastruct-1.4.1/anastruct/fem/cython/celements.pyx` & `anastruct-1.4.2/anastruct/fem/cython/celements.pyx`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/anastruct/fem/cython/elements.py` & `anastruct-1.4.2/anastruct/fem/cython/elements.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from functools import lru_cache
 
 
 @lru_cache(32000)
-def det_moment(kl, kr, qi, q, x, EI, L):
+def det_moment(
+    kl: float, kr: float, qi: float, q: float, x: float, EI: float, L: float
+) -> float:
     """
     See notebook in: anastruct/fem/background/primary_m_v.ipynb
 
     :param kl: (flt) rotational stiffness left
     :param kr: (flt) rotational stiffness right
     :param q: (flt)
     :param x: (flt) Location of bending moment
@@ -43,15 +45,17 @@
         )
         - qi * x**2 / (2 * EI)
         - x**3 * (q - qi) / (6 * EI * L)
     )
 
 
 @lru_cache(32000)
-def det_shear(kl, kr, qi, q, x, EI, L):
+def det_shear(
+    kl: float, kr: float, qi: float, q: float, x: float, EI: float, L: float
+) -> float:
     """
     See notebook in: anastruct/fem/background/primary_m_v.ipynb
 
     :param kl: (flt) rotational stiffness left
     :param kr: (flt) rotational stiffness right
     :param q: (flt)
     :param x: (flt) Location of bending moment
@@ -79,15 +83,15 @@
         )
         - qi * x / EI
         - x**2 * (q - qi) / (2 * EI * L)
     )
 
 
 @lru_cache(32000)
-def det_axial(qi, q, x, EA, L):
+def det_axial(qi: float, q: float, x: float, EA: float, L: float) -> float:
     """
     See notebook in: anastruct/fem/background/distributed_ax_force.ipynb
 
     :param q: (flt)
     :param x: (flt) Location of the axial force
     :param EA: (flt)
     :param L: (flt) Length of the beam
```

### Comparing `anastruct-1.4.1/anastruct/fem/elements.py` & `anastruct-1.4.2/anastruct/fem/elements.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 from __future__ import annotations
-from math import sin, cos
-from functools import lru_cache
+
 import copy
-from typing import TYPE_CHECKING, Dict, Optional, List
+from functools import lru_cache
+from math import cos, sin
+from typing import TYPE_CHECKING, Dict, List, Optional
+
 import numpy as np
-from anastruct.basic import FEMException
 
+from anastruct.basic import FEMException
 
 if TYPE_CHECKING:
-    from anastruct.vertex import Vertex
     from anastruct.fem.node import Node
     from anastruct.fem.system import Spring
+    from anastruct.vertex import Vertex
 
 try:
-    from anastruct.fem.cython.celements import (  # type: ignore # pylint: disable=unused-import
-        det_shear,
-        det_moment,
+    from anastruct.fem.cython.celements import (  # pylint: disable=unused-import
         det_axial,
+        det_moment,
+        det_shear,
     )
 except ImportError:
-    from anastruct.fem.cython.elements import det_shear, det_moment, det_axial
+    from anastruct.fem.cython.elements import det_axial, det_moment, det_shear
 
 """
 The matrices underneath are for slender beams, where the most deformation occurs due to bending.
 Shear deformation is not taken into account.
 """
 
 CACHE_BOUND = 32000
@@ -37,15 +39,15 @@
         EI: float,
         l: float,
         angle: float,
         vertex_1: Vertex,
         vertex_2: Vertex,
         type_: str,
         section_name: str,
-        spring: Spring = None,
+        spring: Optional[Spring] = None,
     ):
         """
         :param id_: integer representing the elements ID
         :param EA: Young's modulus * Area
         :param EI: Young's modulus * Moment of Inertia
         :param l: length
         :param angle: angle between element and x-axis
@@ -150,53 +152,54 @@
 
     def determine_force_vector(self) -> Optional[np.ndarray]:
         self.element_force_vector = np.dot(
             self.stiffness_matrix, self.element_displacement_vector
         )
         return self.element_force_vector
 
-    def compile_stiffness_matrix(self):
+    def compile_stiffness_matrix(self) -> None:
         self.stiffness_matrix = stiffness_matrix(
             self.constitutive_matrix, self.kinematic_matrix
         )
 
-    def compile_kinematic_matrix(self, a1: float, a2: float, l: float):
+    def compile_kinematic_matrix(self, a1: float, a2: float, l: float) -> None:
         self.kinematic_matrix = kinematic_matrix(a1, a2, l)
 
     def compile_constitutive_matrix(
         self,
         EA: float,
         EI: float,
         l: float,
         spring: Optional[Dict[int, float]] = None,
         node_1_hinge: Optional[bool] = False,
         node_2_hinge: Optional[bool] = False,
-    ):
+    ) -> None:
         self.constitutive_matrix = constitutive_matrix(
             EA, EI, l, spring, node_1_hinge, node_2_hinge
         )
 
-    def update_stiffness(self, factor: float, node: int):
+    def update_stiffness(self, factor: float, node: int) -> None:
         if node == 1:
             self.constitutive_matrix[1][1] *= factor
             self.constitutive_matrix[1][2] *= factor
             self.constitutive_matrix[2][1] *= factor
         elif node == 2:
             self.constitutive_matrix[1][2] *= factor
             self.constitutive_matrix[2][1] *= factor
             self.constitutive_matrix[2][2] *= factor
         self.compile_stiffness_matrix()
 
-    def compile_geometric_non_linear_stiffness_matrix(self):
+    def compile_geometric_non_linear_stiffness_matrix(self) -> None:
         self.compile_stiffness_matrix()
+        assert self.N_1 is not None
         self.stiffness_matrix += geometric_stiffness_matrix(
             self.l, self.N_1, self.a1, self.a2
         )
 
-    def reset(self):
+    def reset(self) -> None:
         self.element_displacement_vector = np.zeros(6)
         self.element_primary_force_vector = np.zeros(6)
 
     def __add__(self, other: Element) -> Element:
         if self.id != other.id:
             raise FEMException(
                 "Wrong element:", "only elements with the same id can be added."
@@ -304,18 +307,18 @@
 
     return matrix
 
 
 def stiffness_matrix(
     var_constitutive_matrix: np.ndarray, var_kinematic_matrix: np.ndarray
 ) -> np.ndarray:
-    kinematic_transposed_times_constitutive = np.dot(
-        var_kinematic_matrix.transpose(), var_constitutive_matrix
+    kinematic_transposed_times_constitutive = (
+        var_kinematic_matrix.transpose() @ var_constitutive_matrix
     )
-    return np.dot(kinematic_transposed_times_constitutive, var_kinematic_matrix)
+    return kinematic_transposed_times_constitutive @ var_kinematic_matrix  # type: ignore
 
 
 def geometric_stiffness_matrix(l: float, N: float, a1: float, a2: float) -> np.ndarray:
     """
 
     :param l: (float) Length.
     :param N: (float) Axial force.
@@ -323,15 +326,15 @@
     :return: (array)
     """
     c1 = cos(a1)
     s1 = sin(a1)
     c2 = cos(a2)
     s2 = sin(a2)
     # http://people.duke.edu/~hpgavin/cee421/frame-finite-def.pdf
-    return (
+    return (  # type: ignore
         N
         / l
         * np.array(
             [
                 [
                     6 / 5 * s1**2,
                     -6 / 5 * s1 * c1,
```

### Comparing `anastruct-1.4.1/anastruct/fem/examples/ex_1_2.py` & `anastruct-1.4.2/anastruct/fem/examples/ex_1_2.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from anastruct.fem import system as se
 
 
-def run():
+def run() -> None:
     system = se.SystemElements()
     system.add_element(location=[[3, 4], [0, 0]], EA=5e9, EI=8000)
     system.add_element(location=[[8, 4], [3, 4]], EA=5e9, EI=4000)
     system.show_structure()
 
     system.q_load(element_id=2, q=-10)
```

### Comparing `anastruct-1.4.1/anastruct/fem/examples/ex_2.py` & `anastruct-1.4.2/anastruct/fem/examples/ex_2.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/anastruct/fem/examples/ex_22_loadcombination_doc.py` & `anastruct-1.4.2/anastruct/fem/examples/ex_22_loadcombination_doc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import matplotlib.pyplot as plt
 import numpy as np
-from anastruct.fem.system import SystemElements
+
 from anastruct import LoadCase, LoadCombination
+from anastruct.fem.system import SystemElements
 
 ss = SystemElements()
 
 height = 10
 
 x = np.cumsum([0, 4, 7, 7, 4])
 y = np.zeros(x.shape)
```

### Comparing `anastruct-1.4.1/anastruct/fem/examples/ex_3.py` & `anastruct-1.4.2/anastruct/fem/examples/ex_3.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/anastruct/fem/examples/ex_8_non_linear_portal.py` & `anastruct-1.4.2/anastruct/fem/examples/ex_8_non_linear_portal.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/anastruct/fem/node.py` & `anastruct-1.4.2/anastruct/fem/node.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 from __future__ import annotations
-from typing import Dict, TYPE_CHECKING
+
+from typing import TYPE_CHECKING, Dict, Optional
+
 from anastruct.vertex import Vertex
 
 if TYPE_CHECKING:
     from anastruct.fem.elements import Element
 
 
 class Node:
     def __init__(
         self,
         id: int,  # pylint: disable=redefined-builtin
         Fx: float = 0.0,
         Fz: float = 0.0,
         Ty: float = 0.0,
-        ux: float = 0.0,
-        uz: float = 0.0,
-        phi_y: float = 0,
+        ux: Optional[float] = 0.0,
+        uz: Optional[float] = 0.0,
+        phi_y: Optional[float] = 0,
         vertex: Vertex = Vertex(0, 0),
         hinge: bool = False,
     ):
         """
         :param id: ID of the node, integer
         :param Fx: Value of Fx
         :param Fz: Value of Fz
@@ -43,15 +45,15 @@
         self.hinge = hinge
         self.elements: Dict[int, Element] = {}
 
     @property
     def Fy(self) -> float:
         return -self.Fz
 
-    def __str__(self):
+    def __str__(self) -> str:
         if self.vertex:
             return (
                 f"[id = {self.id}, Fx = {self.Fx}, Fz = {self.Fz}, Ty = {self.Ty}, ux = {self.ux}, "
                 f"uz = {self.uz}, phi_y = {self.phi_y}, x = {self.vertex.x}, y = {self.vertex.y}]"
             )
         else:
             return (
@@ -95,21 +97,27 @@
             self.ux,
             self.uz,
             self.phi_y,
             self.vertex,
             hinge=self.hinge,
         )
 
-    def reset(self):
+    def reset(self) -> None:
         self.Fx = self.Fz = self.Ty = self.ux = self.uz = self.phi_y = 0
         self.hinge = False
 
-    def add_results(self, other: Node):
+    def add_results(self, other: Node) -> None:
         assert (
             self.id == other.id
         ), "Cannot add nodes as the ID's don't match. The nodes positions don't match."
+        assert self.phi_y is not None
+        assert self.ux is not None
+        assert self.uz is not None
+        assert other.phi_y is not None
+        assert other.ux is not None
+        assert other.uz is not None
         self.Fx = self.Fx + other.Fx
         self.Fz = self.Fz + other.Fz
         self.Ty = self.Ty + other.Ty
         self.ux = self.ux + other.ux
         self.uz = self.uz + other.uz
         self.phi_y = self.phi_y + other.phi_y
```

### Comparing `anastruct-1.4.1/anastruct/fem/plotter/element.py` & `anastruct-1.4.2/anastruct/fem/plotter/element.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,19 @@
 import math
+from typing import TYPE_CHECKING, Tuple
+
 import numpy as np
 
+if TYPE_CHECKING:
+    from anastruct.fem.elements import Element
+
 
-def plot_values_deflection(element, factor, linear=False):
+def plot_values_deflection(
+    element: "Element", factor: float, linear: bool = False
+) -> Tuple[np.ndarray, np.ndarray]:
     """
     Determine the plotting values for deflection
 
     :param element: (fem.Element)
     :param factor: (flt) Factor by which to multiply the plotting values perpendicular
                    to the elements axis.
     :param linear: (bool) If True, the bending in between the elements is determined.
@@ -33,15 +40,17 @@
     else:  # truss element has no bending
         x_val = np.array([x1, x2])
         y_val = np.array([y1, y2])
 
     return x_val, y_val
 
 
-def plot_values_bending_moment(element, factor, n):
+def plot_values_bending_moment(
+    element: "Element", factor: float, n: int
+) -> Tuple[np.ndarray, np.ndarray]:
     """
     :param element: (object) of the Element class
     :param factor: (float) scaling the plot
     :param n: (integer) amount of x-values
     :return:
     """
 
@@ -82,15 +91,17 @@
     y_val = np.append(y_val, -element.vertex_2.z)
     x_val = np.insert(x_val, 0, element.vertex_1.x)
     y_val = np.insert(y_val, 0, -element.vertex_1.z)
 
     return x_val, y_val
 
 
-def plot_values_axial_force(element, factor, n):
+def plot_values_axial_force(
+    element: "Element", factor: float, n: int
+) -> Tuple[np.ndarray, np.ndarray]:
     """
     :param element: (object) of the Element class
     :param factor: (float) scaling the plot
     :param n: (integer) amount of x-values
     :return:
     """
 
@@ -127,15 +138,17 @@
     y_val = np.append(y_val, -element.vertex_2.z)
     x_val = np.insert(x_val, 0, element.vertex_1.x)
     y_val = np.insert(y_val, 0, -element.vertex_1.z)
 
     return x_val, y_val
 
 
-def plot_values_shear_force(element, factor):
+def plot_values_shear_force(
+    element: "Element", factor: float
+) -> Tuple[np.ndarray, np.ndarray]:
     x1 = element.vertex_1.x
     y1 = -element.vertex_1.z
     x2 = element.vertex_2.x
     y2 = -element.vertex_2.z
 
     n = len(element.shear_force)
 
@@ -157,11 +170,11 @@
     y_val = np.append(y_val, -element.vertex_2.z)
     x_val = np.insert(x_val, 0, element.vertex_1.x)
     y_val = np.insert(y_val, 0, -element.vertex_1.z)
 
     return x_val, y_val
 
 
-def plot_values_element(element):
-    x_val = [element.vertex_1.x, element.vertex_2.x]
-    y_val = [-element.vertex_1.z, -element.vertex_2.z]
+def plot_values_element(element: "Element") -> Tuple[np.ndarray, np.ndarray]:
+    x_val = np.array([element.vertex_1.x, element.vertex_2.x])
+    y_val = np.array([-element.vertex_1.z, -element.vertex_2.z])
     return x_val, y_val
```

### Comparing `anastruct-1.4.1/anastruct/fem/plotter/mpl.py` & `anastruct-1.4.2/anastruct/fem/plotter/mpl.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,72 +1,83 @@
 import math
+from typing import TYPE_CHECKING, Optional, Sequence, Tuple
+
+import matplotlib.patches as mpatches
+import matplotlib.pyplot as plt
 import numpy as np
-import matplotlib.pyplot as plt  # type: ignore
-import matplotlib.patches as mpatches  # type: ignore
+
 from anastruct.basic import find_nearest, rotate_xy
 from anastruct.fem.plotter.values import (
     PlottingValues,
     det_scaling_factor,
     plot_values_axial_force,
     plot_values_bending_moment,
     plot_values_deflection,
     plot_values_element,
     plot_values_shear_force,
 )
 
+if TYPE_CHECKING:
+    from matplotlib.axes import Axes
+    from matplotlib.figure import Figure
+
+    from anastruct.fem.node import Node
+    from anastruct.fem.system import SystemElements
+
+
 PATCH_SIZE = 0.03
 
 
 class Plotter(PlottingValues):
-    def __init__(self, system, mesh):
+    def __init__(self, system: "SystemElements", mesh: int):
         super(Plotter, self).__init__(system, mesh)
-        self.system = system
-        self.one_fig = None
-        self.max_q = 0
-        self.max_qn = 0
-        self.max_system_point_load = 0
-        self.fig = None
+        self.system: "SystemElements" = system
+        self.one_fig: Optional["Axes"] = None
+        self.max_q: float = 0
+        self.max_qn: float = 0
+        self.max_system_point_load: float = 0
+        self.fig: Optional["Figure"] = None
 
-    def __start_plot(self, figsize):
+    def __start_plot(self, figsize: Optional[Sequence[float]]) -> None:
         plt.close("all")
         self.fig = plt.figure(figsize=figsize)
         self.one_fig = self.fig.add_subplot(111)
         plt.tight_layout()
 
-    def __fixed_support_patch(self, max_val):
+    def __fixed_support_patch(self, max_val: float) -> None:
         """
         :param max_val: max scale of the plot
         """
         width = height = PATCH_SIZE * max_val
         for node in self.system.supports_fixed:
             support_patch = mpatches.Rectangle(
                 (node.vertex.x - width * 0.5, -node.vertex.z - width * 0.5),
                 width,
                 height,
                 color="r",
                 zorder=9,
             )
             self.one_fig.add_patch(support_patch)
 
-    def __hinged_support_patch(self, max_val):
+    def __hinged_support_patch(self, max_val: float) -> None:
         """
         :param max_val: max scale of the plot
         """
         radius = PATCH_SIZE * max_val
         for node in self.system.supports_hinged:
             support_patch = mpatches.RegularPolygon(
                 (node.vertex.x, node.vertex.y - radius),
                 numVertices=3,
                 radius=radius,
                 color="r",
                 zorder=9,
             )
             self.one_fig.add_patch(support_patch)
 
-    def __rotational_support_patch(self, max_val):
+    def __rotational_support_patch(self, max_val: float) -> None:
         """
         :param max_val: max scale of the plot
         """
         width = height = PATCH_SIZE * max_val
         for node in self.system.supports_rotational:
             support_patch = mpatches.Rectangle(
                 (node.vertex.x - width * 0.5, -node.vertex.z - width * 0.5),
@@ -74,15 +85,15 @@
                 height,
                 color="r",
                 zorder=9,
                 fill=False,
             )
             self.one_fig.add_patch(support_patch)
 
-    def __roll_support_patch(self, max_val):
+    def __roll_support_patch(self, max_val: float) -> None:
         """
         :param max_val: max scale of the plot
         """
         radius = PATCH_SIZE * max_val
         count = 0
         for node in self.system.supports_roll:
             direction = self.system.supports_roll_direction[count]
@@ -108,15 +119,15 @@
                 self.one_fig.plot(
                     triangle[1:, 0] - 0.5 * radius * np.sin(angle),
                     triangle[1:, 1] - 0.5 * radius * np.cos(angle),
                     color="r",
                 )
                 if not rotate:
                     rect_patch = mpatches.RegularPolygon(
-                        (node.vertex.x, node - node.vertex.y),
+                        (node.vertex.x, radius - node.vertex.y),
                         numVertices=4,
                         radius=radius,
                         orientation=angle,
                         color="r",
                         zorder=9,
                         fill=False,
                     )
@@ -165,15 +176,15 @@
                         color="r",
                         zorder=9,
                         fill=False,
                     )
                     self.one_fig.add_patch(rect_patch)
             count += 1
 
-    def __rotating_spring_support_patch(self, max_val):
+    def __rotating_spring_support_patch(self, max_val: float) -> None:
         """
         :param max_val: max scale of the plot
         """
         radius = PATCH_SIZE * max_val
 
         for node, _ in self.system.supports_spring_y:
             r = np.arange(0, radius, 0.001)
@@ -188,15 +199,15 @@
                 numVertices=3,
                 radius=radius * 0.9,
                 color="r",
                 zorder=9,
             )
             self.one_fig.add_patch(support_patch)
 
-    def __spring_support_patch(self, max_val):
+    def __spring_support_patch(self, max_val: float) -> None:
         """
         :param max_val: max scale of the plot
         """
         h = PATCH_SIZE * max_val
         left = -0.5 * h
         right = 0.5 * h
         dh = 0.2 * h
@@ -233,37 +244,37 @@
                 numVertices=3,
                 radius=h * 0.9,
                 color="r",
                 zorder=10,
             )
             self.one_fig.add_patch(support_patch)
 
-    def __q_load_patch(self, max_val, verbosity):
+    def __q_load_patch(self, max_val: float, verbosity: int) -> None:
         """
         :param max_val: max scale of the plot
 
         xn1;yn1  q-load   xn1;yn1
         -------------------
         |__________________|
         x1;y1  element    x2;y2
         """
 
         def __plot_patch(
-            h1,
-            h2,
-            x1,
-            y1,
-            x2,
-            y2,
-            ai,
-            qi,
-            q,
-            direction,
-            el_angle,  # pylint: disable=unused-argument
-        ):
+            h1: float,
+            h2: float,
+            x1: float,
+            y1: float,
+            x2: float,
+            y2: float,
+            ai: float,
+            qi: float,
+            q: float,
+            direction: float,
+            el_angle: float,  # pylint: disable=unused-argument
+        ) -> None:
             # - value, because the positive z of the system is opposite of positive y of the plotter
             xn1 = x1 + np.sin(ai) * h1 * direction
             yn1 = y1 + np.cos(ai) * h1 * direction
             xn2 = x2 + np.sin(ai) * h2 * direction
             yn2 = y2 + np.cos(ai) * h2 * direction
             coordinates = ([x1, xn1, xn2, x2], [y1, yn1, yn2, y2])
             self.one_fig.plot(*coordinates, color="g")
@@ -360,15 +371,17 @@
                 h2 = 0.05 * max_val * abs(q) / self.max_q
 
                 ai = -el.q_angle
                 el_angle = el.angle
                 __plot_patch(h1, h2, x1, y1, x2, y2, ai, qi, q, direction, el_angle)
 
     @staticmethod
-    def __arrow_patch_values(Fx, Fz, node, h):
+    def __arrow_patch_values(
+        Fx: float, Fz: float, node: "Node", h: float
+    ) -> Tuple[float, float, float, float, float]:
         """
         :param Fx: (float)
         :param Fz: (float)
         :param node: (Node object)
         :param h: (float) Is a scale variable
         :return: Variables for the matplotlib plotter
         """
@@ -377,15 +390,15 @@
         len_x = Fx / F * h
         len_y = -Fz / F * h
         x = node.vertex.x - len_x * 1.2
         y = node.vertex.y - len_y * 1.2
 
         return x, y, len_x, len_y, F
 
-    def __point_load_patch(self, max_plot_range, verbosity=0):
+    def __point_load_patch(self, max_plot_range: float, verbosity: int = 0) -> None:
         """
         :param max_plot_range: max scale of the plot
         """
 
         for k in self.system.loads_point:
             Fx, Fz = self.system.loads_point[k]
             F = (Fx**2 + Fz**2) ** 0.5
@@ -403,15 +416,15 @@
                 ec="b",
                 fc="orange",
                 zorder=11,
             )
             if verbosity == 0:
                 self.one_fig.text(x, y, f"F={F}", color="k", fontsize=9, zorder=10)
 
-    def __moment_load_patch(self, max_val):
+    def __moment_load_patch(self, max_val: float) -> None:
         h = 0.2 * max_val
         for k, v in self.system.loads_moment.items():
             node = self.system.node_map[k]
             if v > 0:
                 self.one_fig.plot(
                     node.vertex.x,
                     -node.vertex.z,
@@ -434,23 +447,23 @@
                 color="k",
                 fontsize=9,
                 zorder=10,
             )
 
     def plot_structure(
         self,
-        figsize,
-        verbosity,
-        show=False,
-        supports=True,
-        scale=1,
-        offset=(0, 0),
-        gridplot=False,
-        annotations=True,
-    ):
+        figsize: Optional[Sequence[float]],
+        verbosity: int,
+        show: bool = False,
+        supports: bool = True,
+        scale: float = 1,
+        offset: Sequence[float] = (0, 0),
+        gridplot: bool = False,
+        annotations: bool = True,
+    ) -> Optional["Figure"]:
         """
         :param show: (boolean) if True, plt.figure will plot.
         :param supports: (boolean) if True, supports are plotted.
         :param annotations: (boolean) if True, structure annotations are plotted.
                             It includes section name.
         :return:
         """
@@ -531,18 +544,26 @@
             # add_loads
             self.__q_load_patch(max_plot_range, verbosity)
             self.__point_load_patch(max_plot_range, verbosity)
             self.__moment_load_patch(max_plot_range)
 
         if show:
             self.plot()
+            return None
         else:
             return self.fig
 
-    def _add_node_values(self, x_val, y_val, value_1, value_2, digits):
+    def _add_node_values(
+        self,
+        x_val: np.ndarray,
+        y_val: np.ndarray,
+        value_1: float,
+        value_2: float,
+        digits: int,
+    ) -> None:
         offset = self.max_val_structure * 0.015
 
         # add value to plot
         self.one_fig.text(
             x_val[1] - offset,
             y_val[1] + offset,
             f"{round(value_1, digits)}",
@@ -555,59 +576,66 @@
             y_val[-2] + offset,
             f"{round(value_2, digits)}",
             fontsize=9,
             ha="center",
             va="center",
         )
 
-    def _add_element_values(self, x_val, y_val, value, index, digits=2):
+    def _add_element_values(
+        self,
+        x_val: np.ndarray,
+        y_val: np.ndarray,
+        value: float,
+        index: int,
+        digits: int = 2,
+    ) -> None:
         self.one_fig.text(
             x_val[index],
             y_val[index],
             f"{round(value, digits)}",
             fontsize=9,
             ha="center",
             va="center",
         )
 
     def plot_result(
         self,
-        axis_values,
-        force_1=None,
-        force_2=None,
-        digits=2,
-        node_results=True,
-        fill_polygon=True,
-        color=0,
-    ):
+        axis_values: Sequence,
+        force_1: Optional[float] = None,
+        force_2: Optional[float] = None,
+        digits: int = 2,
+        node_results: bool = True,
+        fill_polygon: bool = True,
+        color: int = 0,
+    ) -> None:
         if fill_polygon:
             rec = plt.Polygon(np.vstack(axis_values).T, color=f"C{color}", alpha=0.3)
             self.one_fig.add_patch(rec)
         # plot force
         x_val = axis_values[0]
         y_val = axis_values[1]
 
         self.one_fig.plot(x_val, y_val, color=f"C{color}")
 
         if node_results:
             self._add_node_values(x_val, y_val, force_1, force_2, digits)
 
-    def plot(self):
+    def plot(self) -> None:
         plt.show()
 
     def axial_force(
         self,
-        factor=None,
-        figsize=None,
-        verbosity=0,
-        scale=1,
-        offset=(0, 0),
-        show=True,
-        gridplot=False,
-    ):
+        factor: Optional[float] = None,
+        figsize: Optional[Sequence[float]] = None,
+        verbosity: int = 0,
+        scale: float = 1,
+        offset: Sequence[float] = (0, 0),
+        show: bool = True,
+        gridplot: bool = False,
+    ) -> Optional["Figure"]:
         self.plot_structure(figsize, 1, scale=scale, offset=offset, gridplot=gridplot)
         con = len(self.system.element_map[1].axial_force)
 
         if factor is None:
             max_force = max(
                 map(
                     lambda el: max(
@@ -673,27 +701,28 @@
                             va="center",
                             fontsize=14,
                             color="b",
                         )
 
         if show:
             self.plot()
+            return None
         else:
             return self.fig
 
     def bending_moment(
         self,
-        factor=None,
-        figsize=None,
-        verbosity=0,
-        scale=1,
-        offset=(0, 0),
-        show=True,
-        gridplot=False,
-    ):
+        factor: Optional[float] = None,
+        figsize: Optional[Sequence[float]] = None,
+        verbosity: int = 0,
+        scale: float = 1,
+        offset: Sequence[float] = (0, 0),
+        show: bool = True,
+        gridplot: bool = False,
+    ) -> Optional["Figure"]:
         self.plot_structure(figsize, 1, scale=scale, offset=offset, gridplot=gridplot)
         con = len(self.system.element_map[1].bending_moment)
         if factor is None:
             # maximum moment determined by comparing the node's moments and the sagging moments.
             max_moment = max(
                 map(
                     lambda el: max(
@@ -729,44 +758,45 @@
                 abs(el.node_2.Ty),
                 node_results=node_results,
             )
 
             if el.all_qp_load:
                 m_sag = min(el.bending_moment)
                 index = find_nearest(el.bending_moment, m_sag)[1]
-                offset = self.max_val_structure * -0.05
+                offset1 = self.max_val_structure * -0.05
 
                 if verbosity == 0:
-                    x = axis_values[0][index] + np.sin(-el.angle) * offset
-                    y = axis_values[1][index] + np.cos(-el.angle) * offset
+                    x = axis_values[0][index] + np.sin(-el.angle) * offset1
+                    y = axis_values[1][index] + np.cos(-el.angle) * offset1
                     self.one_fig.text(x, y, f"{round(m_sag, 1)}", fontsize=9)
         if show:
             self.plot()
+            return None
         else:
             return self.fig
 
     def shear_force(
         self,
-        factor=None,
-        figsize=None,
-        verbosity=0,
-        scale=1,
-        offset=(0, 0),
-        show=True,
-        gridplot=False,
-        include_structure=True,
-    ):
+        factor: Optional[float] = None,
+        figsize: Optional[Sequence[float]] = None,
+        verbosity: int = 0,
+        scale: float = 1,
+        offset: Sequence[float] = (0, 0),
+        show: bool = True,
+        gridplot: bool = False,
+        include_structure: bool = True,
+    ) -> Optional["Figure"]:
         if include_structure:
             self.plot_structure(
                 figsize, 1, scale=scale, offset=offset, gridplot=gridplot
             )
         if factor is None:
             max_force = max(
                 map(
-                    lambda el: np.max(np.abs(el.shear_force)),
+                    lambda el: np.max(np.abs(el.shear_force)),  # type: ignore
                     self.system.element_map.values(),
                 )
             )
             factor = det_scaling_factor(max_force, self.max_val_structure)
 
         for el in self.system.element_map.values():
             if (
@@ -783,18 +813,27 @@
             shear_2 = el.shear_force[-1]
 
             self.plot_result(
                 axis_values, shear_1, shear_2, node_results=not bool(verbosity)
             )
         if show:
             self.plot()
+            return None
         else:
             return self.fig
 
-    def reaction_force(self, figsize, verbosity, scale, offset, show, gridplot=False):
+    def reaction_force(
+        self,
+        figsize: Optional[Sequence[float]],
+        verbosity: int,
+        scale: float,
+        offset: Sequence[float],
+        show: bool,
+        gridplot: bool = False,
+    ) -> Optional["Figure"]:
         self.plot_structure(
             figsize, 1, supports=False, scale=scale, offset=offset, gridplot=gridplot
         )
 
         h = 0.2 * self.max_val_structure
         max_force = max(
             map(
@@ -894,28 +933,29 @@
                         f"T={round(node.Ty, 2)}",
                         color="k",
                         fontsize=9,
                         zorder=10,
                     )
         if show:
             self.plot()
+            return None
         else:
             return self.fig
 
-    def displacements(  # pylint: disable=arguments-renamed
+    def displacements(  # type: ignore  # pylint: disable=arguments-renamed
         self,
-        factor=None,
-        figsize=None,
-        verbosity=0,
-        scale=1,
-        offset=(0, 0),
-        show=True,
-        linear=False,
-        gridplot=False,
-    ):
+        factor: Optional[float] = None,
+        figsize: Optional[Sequence[float]] = None,
+        verbosity: int = 0,
+        scale: float = 1,
+        offset: Sequence[float] = (0, 0),
+        show: bool = True,
+        linear: bool = False,
+        gridplot: bool = False,
+    ) -> Optional["Figure"]:
         self.plot_structure(figsize, 1, scale=scale, offset=offset, gridplot=gridplot)
         if factor is None:
             # needed to determine the scaling factor
             max_displacement = max(
                 map(
                     lambda el: max(
                         abs(el.node_1.ux), abs(el.node_1.uz), el.max_deflection
@@ -933,31 +973,39 @@
 
             if el.type == "general":
                 # index of the max deflection
                 x = np.linspace(el.vertex_1.x, el.vertex_2.x, el.deflection.size)
                 y = np.linspace(el.vertex_1.y, el.vertex_2.y, el.deflection.size)
                 xd, yd = plot_values_deflection(el, 1.0, linear)
                 deflection = ((xd - x) ** 2 + (yd - y) ** 2) ** 0.5
-                index = np.argmax(np.abs(deflection))
+                index = int(np.argmax(np.abs(deflection)))
 
                 if verbosity == 0:
                     if index != 0 or index != el.deflection.size:
                         self._add_element_values(
                             axis_values[0],
                             axis_values[1],
                             deflection[index],
                             index,
                             3,
                         )
         if show:
             self.plot()
+            return None
         else:
             return self.fig
 
-    def results_plot(self, figsize, verbosity, scale, offset, show):
+    def results_plot(
+        self,
+        figsize: Optional[Sequence[float]],
+        verbosity: int,
+        scale: float,
+        offset: Sequence[float],
+        show: bool,
+    ) -> Optional["Figure"]:
         """
         Aggregate all the plots in one grid plot.
 
         :param figsize: (tpl)
         :param verbosity: (int)
         :param scale: (flt)
         :param offset: (tpl)
@@ -986,9 +1034,10 @@
         self.displacements(None, figsize, verbosity, scale, offset, False, False, True)
         self.one_fig = self.fig.add_subplot(a + 6)
         plt.title("reaction force")
         self.reaction_force(figsize, verbosity, scale, offset, False, True)
 
         if show:
             self.plot()
+            return None
         else:
             return self.fig
```

### Comparing `anastruct-1.4.1/anastruct/fem/postprocess.py` & `anastruct-1.4.2/anastruct/fem/postprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 import copy
 import math
 from typing import TYPE_CHECKING
+
 import numpy as np
-from anastruct.fem.node import Node
-from anastruct.basic import integrate_array
 
+from anastruct.basic import integrate_array
+from anastruct.fem.node import Node
 
 if TYPE_CHECKING:
-    from anastruct.fem.system import SystemElements
     from anastruct.fem.elements import Element
+    from anastruct.fem.system import SystemElements
 
 
 class SystemLevel:
     def __init__(self, system: "SystemElements"):
         self.system = system
         # post processor element level
         self.post_el = ElementLevel(self.system)
 
-    def node_results_elements(self):
+    def node_results_elements(self) -> None:
         """
         Determines the node results on the system level.
         Results placed in SystemElements class: self.node_objects (list).
         """
 
         for el in self.system.element_map.values():
             # post processor element level
             self.post_el.node_results(el)
 
-    def node_results_system(self):
+    def node_results_system(self) -> None:
         for k, v in self.system.node_element_map.items():
             # reset nodes in case of iterative calculation
             self.system.node_map[k].reset()
 
             if k in self.system.loads_moment:
                 self.system.node_map[k].Ty += self.system.loads_moment[k]
 
@@ -40,20 +41,24 @@
                 self.system.node_map[k].Fx += Fx
                 self.system.node_map[k].Fz += Fz
 
             for vi in v:
                 node = vi.node_map[k]
                 self.system.node_map[k] -= node
 
+                assert node.ux is not None
+                assert node.uz is not None
+                assert node.phi_y is not None
+
                 # The displacements are not summarized. Should be assigned only once
                 self.system.node_map[k].ux = -node.ux
                 self.system.node_map[k].uz = -node.uz
                 self.system.node_map[k].phi_y = -node.phi_y
 
-    def reaction_forces(self):
+    def reaction_forces(self) -> None:
         supports = []
         for node in self.system.supports_fixed:
             supports.append(node.id)
         for node in self.system.supports_hinged:
             supports.append(node.id)
         for node in self.system.supports_roll:
             supports.append(node.id)
@@ -73,15 +78,15 @@
             node.Fx *= -1
             node.Fz *= -1
             node.Ty *= -1
             node.ux = None
             node.uz = None
             node.phi_y = None
 
-    def element_results(self):
+    def element_results(self) -> None:
         """
         Determines the element results for all elements in the system on element level.
         """
 
         for el in self.system.element_map.values():
             con = self.system.plotter.mesh
             self.post_el.determine_axial_force(el, con)
@@ -90,15 +95,15 @@
             self.post_el.determine_displacements(el, con)
 
 
 class ElementLevel:
     def __init__(self, system: "SystemElements"):
         self.system = system
 
-    def node_results(self, element: "Element"):
+    def node_results(self, element: "Element") -> None:
         """
         Determine node results on the element level.
         """
         assert element.element_force_vector is not None
         assert element.element_primary_force_vector is not None
 
         # Check for hinges
@@ -150,15 +155,15 @@
                 uz = node.uz
                 node.Fz = c * Fz + s * Fx
                 node.Fx = -(c * Fx + s * Fz)
                 node.ux = c * ux + s * uz
                 node.uz = c * uz + s * ux
 
     @staticmethod
-    def determine_axial_force(element: "Element", con: int):
+    def determine_axial_force(element: "Element", con: int) -> None:
         N_1 = (math.sin(element.angle) * element.node_1.Fz) + -(
             math.cos(element.angle) * element.node_1.Fx
         )
         N_2 = -(math.sin(element.angle) * element.node_2.Fz) + (
             math.cos(element.angle) * element.node_2.Fx
         )
 
@@ -175,15 +180,15 @@
             qn = element.all_qn_load[1]
             qn_part = (qn - qni) / (2 * element.l) * (element.l - x) * x
             n_val += qn_part
 
         element.axial_force = n_val
 
     @staticmethod
-    def determine_bending_moment(element: "Element", con: int):
+    def determine_bending_moment(element: "Element", con: int) -> None:
         dT = -(element.node_2.Ty + element.node_1.Ty)  # T2 - (-T1)
 
         iteration_factor = np.linspace(0, 1, con)
         x = iteration_factor * element.l
         m_val = element.node_1.Ty + iteration_factor * dT
         if element.all_qp_load:
             qi = element.all_qp_load[0]
@@ -194,27 +199,27 @@
                 - (((2 * qi) + q) / 6) * element.l * x
             )
             m_val += q_part
 
         element.bending_moment = m_val
 
     @staticmethod
-    def determine_shear_force(element: "Element", con: int):
+    def determine_shear_force(element: "Element", con: int) -> None:
         """
         Determines the shear force by differentiating the bending moment.
         :param element: (object) of the Element class
         """
         iteration_factor = np.linspace(0, 1, con)
         x = iteration_factor * element.l
         eq = np.polyfit(x, element.bending_moment, 3)
         shear_force = eq[0] * 3 * x**2 + eq[1] * 2 * x + eq[2]
         element.shear_force = shear_force
 
     @staticmethod
-    def determine_displacements(element: "Element", con: int):
+    def determine_displacements(element: "Element", con: int) -> None:
         """
         Determines the displacement by integrating the bending moment.
         :param element: (object) of the Element class
 
         w = -M''
 
         This gives you the formula
@@ -249,14 +254,15 @@
 
             # Angle between last w and elements axis. The w array will be corrected so that
             # this angle == 0.
             alpha2 = np.arctan(w2[-1] / element.l)
             w2 = w2[::-1] - lx[::-1] * np.tan(alpha2)
 
             element.deflection = -(w1 + w2) / 2.0
+            assert element.deflection is not None
             element.max_deflection = np.max(np.abs(element.deflection))
 
         # Extension
         assert element.axial_force is not None
         dx = element.l / (len(element.axial_force) - 1)
         lx = np.linspace(0, element.l, con)
```

### Comparing `anastruct-1.4.1/anastruct/fem/system.py` & `anastruct-1.4.2/anastruct/fem/system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,36 +1,39 @@
-import math
-import re
 import collections.abc
 import copy
+import math
+import re
 from typing import (
-    Tuple,
-    Union,
+    TYPE_CHECKING,
+    Any,
+    Collection,
+    Dict,
     List,
     Optional,
-    Dict,
-    Set,
-    TYPE_CHECKING,
     Sequence,
-    cast,
-    Collection,
-    Any,
+    Set,
+    Tuple,
+    Union,
 )
+
 import numpy as np
-from anastruct.basic import FEMException, args_to_lists
-from anastruct.fem.postprocess import SystemLevel as post_sl
-from anastruct.fem.elements import Element
-from anastruct.vertex import Vertex
+
+from anastruct.basic import FEMException, arg_to_list
 from anastruct.fem import plotter
-from anastruct.vertex import vertex_range
-from anastruct.sectionbase import properties
+from anastruct.fem.elements import Element
+from anastruct.fem.postprocess import SystemLevel as post_sl
 from anastruct.fem.util.load import LoadCase
+from anastruct.sectionbase import properties
+from anastruct.vertex import Vertex, vertex_range
+
 from . import system_components
 
 if TYPE_CHECKING:
+    from matplotlib.figure import Figure
+
     from anastruct.fem.node import Node
 
 
 Spring = Dict[int, float]
 MpType = Dict[int, float]
 
 
@@ -168,16 +171,16 @@
         x: Union[List[float], np.ndarray],
         y: Union[List[float], np.ndarray],
         EA: Optional[Union[List[float], np.ndarray]] = None,
         EI: Optional[Union[List[float], np.ndarray]] = None,
         g: Optional[Union[List[float], np.ndarray]] = None,
         mp: Optional[MpType] = None,
         spring: Optional[Spring] = None,
-        **kwargs,
-    ):
+        **kwargs: dict,
+    ) -> None:
         """
         Add multiple elements defined by two containers with coordinates.
 
         :param x: x coordinates.
         :param y: y coordinates.
         :param EA: See 'add_element' method
         :param EI: See 'add_element' method
@@ -211,16 +214,16 @@
             )
 
     def add_truss_element(
         self,
         location: Union[
             Sequence[Sequence[float]], Sequence[Vertex], Sequence[float], Vertex
         ],
-        EA: float = None,
-        **kwargs,
+        EA: Optional[float] = None,
+        **kwargs: dict,
     ) -> int:
         """
         .. highlight:: python
 
         Add an element that only has axial force.
 
         :param location: The two nodes of the element or the next node of the element.
@@ -233,27 +236,36 @@
                    location=[Vertex, Vertex]
                    location=[x, y]
                    location=Vertex
 
         :param EA: EA
         :return: Elements ID.
         """
-        return self.add_element(location, EA, element_type="truss", **kwargs)
+        return self.add_element(
+            location,
+            EA,
+            EI=None,
+            g=0,
+            mp=None,
+            sprint=None,
+            element_type="truss",
+            **kwargs,
+        )
 
     def add_element(
         self,
         location: Union[
             Sequence[Sequence[float]], Sequence[Vertex], Sequence[float], Vertex
         ],
-        EA: float = None,
-        EI: float = None,
+        EA: Optional[float] = None,
+        EI: Optional[float] = None,
         g: float = 0,
         mp: Optional[MpType] = None,
         spring: Optional[Spring] = None,
-        **kwargs,
+        **kwargs: Any,
     ) -> int:
         """
         :param location: The two nodes of the element or the next node of the element.
 
             :Example:
 
             .. code-block:: python
@@ -335,18 +347,14 @@
             point_1, point_2, node_id1, node_id2, spring, mp
         )
 
         system_components.util.append_node_id(
             self, point_1, point_2, node_id1, node_id2
         )
 
-        # Only for typing purposes
-        EA = cast(float, EA)
-        EI = cast(float, EI)
-
         # add element
         element = Element(
             id_=self.count,
             EA=EA,
             EI=EI,
             l=(point_2 - point_1).modulus(),
             angle=angle,
@@ -387,21 +395,21 @@
     def add_multiple_elements(
         self,
         location: Union[
             Sequence[Sequence[float]], Sequence[Vertex], Sequence[float], Vertex
         ],
         n: Optional[int] = None,
         dl: Optional[float] = None,
-        EA: float = None,
-        EI: float = None,
+        EA: Optional[float] = None,
+        EI: Optional[float] = None,
         g: float = 0,
         mp: Optional[MpType] = None,
         spring: Optional[Spring] = None,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> List[int]:
         """
         Add multiple elements defined by the first and the last point.
 
         :param location: See 'add_element' method
         :param n: Number of elements.
         :param dl: Distance between the elements nodes.
         :param EA: See 'add_element' method
@@ -510,16 +518,16 @@
         )
         return elements
 
     def insert_node(
         self,
         element_id: int,
         location: Union[Sequence[float], Vertex, None] = None,
-        factor=None,
-    ):
+        factor: Optional[float] = None,
+    ) -> None:
         """
         Insert a node into an existing structure.
         This can be done by adding a new Vertex at any given location, or by setting
         a factor of the elements length. E.g. if you want a node at 40% of the elements
         length, you pass factor = 0.4.
 
         Note: this method completely rebuilds the SystemElements object and is therefore
@@ -600,16 +608,16 @@
 
     def solve(
         self,
         force_linear: bool = False,
         verbosity: int = 0,
         max_iter: int = 200,
         geometrical_non_linear: int = False,
-        **kwargs,
-    ):
+        **kwargs: Any,
+    ) -> np.ndarray:
         """
         Compute the results of current model.
 
         :param force_linear: Force a linear calculation. Even when the system has non linear nodes.
         :param verbosity: 0. Log calculation outputs. 1. silence.
         :param max_iter: Maximum allowed iterations.
         :param geometrical_non_linear: Calculate second order effects and determine the
@@ -629,14 +637,15 @@
         #                naked (bool) Default = False, if True force lines won't be computed.
 
         for node_id in self.node_map:
             system_components.util.check_internal_hinges(self, node_id)
 
         if self.system_displacement_vector is None:
             system_components.assembly.process_supports(self)
+            assert self.system_displacement_vector is not None
 
         naked = kwargs.get("naked", False)
 
         if not naked:
             if not self.validate():
                 if all(
                     ["general" in element.type for element in self.element_map.values()]
@@ -671,14 +680,16 @@
                 discretize_kwargs=discretize_kwargs,
             )
             return self.system_displacement_vector
 
         system_components.assembly.process_conditions(self)
 
         # solution of the reduced system (reduced due to support conditions)
+        assert self.reduced_system_matrix is not None
+        assert self.reduced_force_vector is not None
         reduced_displacement_vector = np.linalg.solve(
             self.reduced_system_matrix, self.reduced_force_vector
         )
 
         # add the solution of the reduced system in the complete system displacement vector
         assert self.shape_system_matrix is not None
         self.system_displacement_vector = np.zeros(self.shape_system_matrix)
@@ -737,45 +748,45 @@
         system_components.assembly.assemble_system_matrix(ss)
 
         system_components.assembly.process_conditions(ss)
 
         w, _ = np.linalg.eig(ss.reduced_system_matrix)
         return bool(np.all(w > min_eigen))
 
-    def add_support_hinged(self, node_id: Union[int, Sequence[int]]):
+    def add_support_hinged(self, node_id: Union[int, Sequence[int]]) -> None:
         """
         Model a hinged support at a given node.
 
         :param node_id: Represents the nodes ID
         """
         if not isinstance(node_id, collections.abc.Iterable):
             node_id = [node_id]
 
         for id_ in node_id:
             id_ = _negative_index_to_id(id_, self.node_map.keys())
 
             # add the support to the support list for the plotter
             self.supports_hinged.append(self.node_map[id_])
 
-    def add_support_rotational(self, node_id: Union[int, Sequence[int]]):
+    def add_support_rotational(self, node_id: Union[int, Sequence[int]]) -> None:
         """
         Model a rotational support at a given node.
 
         :param node_id: Represents the nodes ID
         """
         if not isinstance(node_id, collections.abc.Iterable):
             node_id = [node_id]
 
         for id_ in node_id:
             id_ = _negative_index_to_id(id_, self.node_map.keys())
 
             # add the support to the support list for the plotter
             self.supports_rotational.append(self.node_map[id_])
 
-    def add_internal_hinge(self, node_id: Union[int, Sequence[int]]):
+    def add_internal_hinge(self, node_id: Union[int, Sequence[int]]) -> None:
         """
         Model an internal hinge at a given node.
         This may alternately be done by setting spring={n: 0} when creating elements
         but this can be an easier method of doing so
 
         :param node_id: Represents the nodes ID
         """
@@ -790,15 +801,15 @@
 
     def add_support_roll(
         self,
         node_id: Union[Sequence[int], int],
         direction: Union[Sequence[Union[str, int]], Union[str, int]] = "x",
         angle: Union[Sequence[Optional[float]], Optional[float]] = None,
         rotate: Union[Sequence[bool], bool] = True,
-    ):
+    ) -> None:
         """
         Adds a rolling support at a given node.
 
         :param node_id: Represents the nodes ID
         :param direction: Represents the direction that is free: 'x', 'y'
         :param angle: Angle in degrees relative to global x-axis.
                                 If angle is given, the support will be inclined.
@@ -833,15 +844,15 @@
             self.supports_roll.append(self.node_map[id_])
             self.supports_roll_direction.append(direction_i)
             self.supports_roll_rotate.append(rotate_)
 
     def add_support_fixed(
         self,
         node_id: Union[Sequence[int], int],
-    ):
+    ) -> None:
         """
         Add a fixed support at a given node.
 
         :param node_id: Represents the nodes ID
         """
         if not isinstance(node_id, collections.abc.Iterable):
             node_id = [
@@ -857,15 +868,15 @@
 
     def add_support_spring(
         self,
         node_id: Union[Sequence[int], int],
         translation: Union[Sequence[int], int],
         k: Union[Sequence[float], float],
         roll: Union[Sequence[bool], bool] = False,
-    ):
+    ) -> None:
         """
         Add a translational support at a given node.
 
         :param translation: Represents the prevented translation.
 
             **Note**
 
@@ -913,118 +924,116 @@
     def q_load(
         self,
         q: Union[float, Sequence[float]],
         element_id: Union[int, Sequence[int]],
         direction: Union[str, Sequence[str]] = "element",
         rotation: Optional[Union[float, Sequence[float]]] = None,
         q_perp: Union[float, Sequence[float]] = None,
-    ):
+    ) -> None:
         """
         Apply a q-load to an element.
 
         :param element_id: representing the element ID
         :param q: value of the q-load
         :param direction: "element", "x", "y", "parallel"
         :param rotation: Rotate the force clockwise. Rotation is in degrees
         :param q_perp: value of any q-load perpendicular to the indication direction/rotation
         """
-        # TODO! this function is a duck typing hell. redesign.
+        q_arr: Sequence[Sequence[float]]
+        q_perp_arr: Sequence[Sequence[float]]
+        if isinstance(q, Sequence):
+            q_arr = [q]
+        elif isinstance(q, (int, float)):
+            q_arr = [[q, q]]
         if q_perp is None:
-            q_perp = [0, 0]
-        if not isinstance(q, Sequence):
-            q = [q, q]
-        if not isinstance(q_perp, Sequence):
-            q_perp = [q_perp, q_perp]
-        q = [q]  # type: ignore
-        q_perp = [q_perp]  # type: ignore
+            q_perp_arr = [[0, 0]]
+        elif isinstance(q_perp, Sequence):
+            q_perp_arr = [q_perp]
+        elif isinstance(q_perp, (int, float)):
+            q_perp_arr = [[q_perp, q_perp]]
+
         if rotation is None:
             direction_flag = True
         else:
             direction_flag = False
-        (  # pylint: disable=unbalanced-tuple-unpacking
-            q,
-            element_id,
-            direction,
-            rotation,
-            q_perp,
-        ) = args_to_lists(q, element_id, direction, rotation, q_perp)
-
-        assert len(q) == len(element_id)  # type: ignore
-        assert len(q) == len(direction)  # type: ignore
-        assert len(q) == len(rotation)  # type: ignore
-        assert len(q) == len(q_perp)  # type: ignore
 
-        for i, element_idi in enumerate(element_id):  # type: ignore
-            id_ = _negative_index_to_id(element_idi, self.element_map.keys())  # type: ignore
+        n_elems = len(element_id) if isinstance(element_id, Sequence) else 1
+        element_id = arg_to_list(element_id, n_elems)
+        direction = arg_to_list(direction, n_elems)
+        rotation = arg_to_list(rotation, n_elems)
+        q_arr = arg_to_list(q_arr, n_elems)
+        q_perp_arr = arg_to_list(q_perp_arr, n_elems)
+
+        for i, element_idi in enumerate(element_id):
+            id_ = _negative_index_to_id(element_idi, self.element_map.keys())
             self.plotter.max_q = max(
                 self.plotter.max_q,
-                (q[i][0] ** 2 + q_perp[i][0] ** 2) ** 0.5,  # type: ignore
-                (q[i][1] ** 2 + q_perp[i][1] ** 2) ** 0.5,  # type: ignore
+                (q_arr[i][0] ** 2 + q_perp_arr[i][0] ** 2) ** 0.5,
+                (q_arr[i][1] ** 2 + q_perp_arr[i][1] ** 2) ** 0.5,
             )
 
             if direction_flag:
                 if direction[i] == "x":
-                    rotation[i] = 0  # type: ignore
+                    rotation[i] = 0
                 elif direction[i] == "y":
-                    rotation[i] = np.pi / 2  # type: ignore
+                    rotation[i] = np.pi / 2
                 elif direction[i] == "parallel":
-                    rotation[i] = self.element_map[element_id[i]].angle  # type: ignore
+                    rotation[i] = self.element_map[element_id[i]].angle
                 else:
-                    rotation[i] = np.pi / 2 + self.element_map[element_id[i]].angle  # type: ignore
+                    rotation[i] = np.pi / 2 + self.element_map[element_id[i]].angle
             else:
-                rotation[i] = math.radians(rotation[i])  # type: ignore
-                direction[i] = "angle"  # type: ignore
+                rotation[i] = math.radians(rotation[i])
+                direction[i] = "angle"
 
-            cos = math.cos(rotation[i])  # type: ignore
-            sin = math.sin(rotation[i])  # type: ignore
+            cos = math.cos(rotation[i])
+            sin = math.sin(rotation[i])
             self.loads_q[id_] = [
                 (
-                    (q_perp[i][0] * cos + q[i][0] * sin) * self.load_factor,  # type: ignore
-                    (q[i][0] * self.orientation_cs * cos + q_perp[i][0] * sin)  # type: ignore
+                    (q_perp_arr[i][0] * cos + q_arr[i][0] * sin) * self.load_factor,
+                    (q_arr[i][0] * self.orientation_cs * cos + q_perp_arr[i][0] * sin)
                     * self.load_factor,
                 ),
                 (
-                    (q_perp[i][1] * cos + q[i][1] * sin) * self.load_factor,  # type: ignore
-                    (q[i][1] * self.orientation_cs * cos + q_perp[i][1] * sin)  # type: ignore
+                    (q_perp_arr[i][1] * cos + q_arr[i][1] * sin) * self.load_factor,
+                    (q_arr[i][1] * self.orientation_cs * cos + q_perp_arr[i][1] * sin)
                     * self.load_factor,
                 ),
             ]
             el = self.element_map[id_]
-            el.q_load = [i * self.orientation_cs * self.load_factor for i in q[i]]  # type: ignore
-            el.q_perp_load = [i * self.load_factor for i in q_perp[i]]  # type: ignore
-            el.q_direction = direction[i]  # type: ignore
-            el.q_angle = rotation[i]  # type: ignore
+            el.q_load = (
+                self.orientation_cs * self.load_factor * q_arr[i][0],
+                self.orientation_cs * self.load_factor * q_arr[i][1],
+            )
+            el.q_perp_load = (
+                q_perp_arr[i][0] * self.load_factor,
+                q_perp_arr[i][1] * self.load_factor,
+            )
+            el.q_direction = direction[i]
+            el.q_angle = rotation[i]
 
     def point_load(
         self,
         node_id: Union[int, Sequence[int]],
         Fx: Union[float, Sequence[float]] = 0.0,
         Fy: Union[float, Sequence[float]] = 0.0,
         rotation: Union[float, Sequence[float]] = 0,
-    ):
+    ) -> None:
         """
         Apply a point load to a node.
 
         :param node_id: Nodes ID.
         :param Fx: Force in global x direction.
         :param Fy: Force in global x direction.
         :param rotation: Rotate the force clockwise. Rotation is in degrees.
         """
-        (  # pylint: disable=unbalanced-tuple-unpacking
-            node_id,
-            Fx,
-            Fy,
-            rotation,
-        ) = args_to_lists(node_id, Fx, Fy, rotation)
-        node_id = cast(Sequence[int], node_id)
-        Fx = cast(Sequence[float], Fx)
-        Fy = cast(Sequence[float], Fy)
-        rotation = cast(Sequence[float], rotation)
-
-        assert len(node_id) == len(Fx) == len(Fy) == len(rotation)
+        n = len(node_id) if isinstance(node_id, Sequence) else 1
+        node_id = arg_to_list(node_id, n)
+        Fx = arg_to_list(Fx, n)
+        Fy = arg_to_list(Fy, n)
+        rotation = arg_to_list(rotation, n)
 
         for i, node_idi in enumerate(node_id):
             id_ = _negative_index_to_id(node_idi, self.node_map.keys())
             if (
                 id_ in self.inclined_roll
                 and np.mod(self.inclined_roll[id_], np.pi / 2) != 0
             ):
@@ -1041,28 +1050,24 @@
             self.loads_point[id_] = (
                 (Fx[i] * cos + Fy[i] * sin) * self.load_factor,
                 (Fy[i] * self.orientation_cs * cos + Fx[i] * sin) * self.load_factor,
             )
 
     def moment_load(
         self, node_id: Union[int, Sequence[int]], Ty: Union[float, Sequence[float]]
-    ):
+    ) -> None:
         """
         Apply a moment on a node.
 
         :param node_id: Nodes ID.
         :param Ty: Moments acting on the node.
         """
-        node_id, Ty = args_to_lists(  # pylint: disable=unbalanced-tuple-unpacking
-            node_id, Ty
-        )
-        node_id = cast(Sequence[int], node_id)
-        Ty = cast(Sequence[float], Ty)
-
-        assert len(node_id) == len(Ty)
+        n = len(node_id) if isinstance(node_id, Sequence) else 1
+        node_id = arg_to_list(node_id, n)
+        Ty = arg_to_list(Ty, n)
 
         for i, node_idi in enumerate(node_id):
             id_ = _negative_index_to_id(node_idi, self.node_map.keys())
             self.loads_moment[id_] = Ty[i] * self.load_factor
 
     def show_structure(
         self,
@@ -1070,15 +1075,15 @@
         scale: float = 1.0,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
         show: bool = True,
         supports: bool = True,
         values_only: bool = False,
         annotations: bool = False,
-    ):
+    ) -> Union[Tuple[np.ndarray, np.ndarray], Optional["Figure"]]:
         """
         Plot the structure.
 
         :param factor: Influence the plotting scale.
         :param verbosity:  0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
@@ -1101,15 +1106,15 @@
         factor: Optional[float] = None,
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Tuple[float, float] = None,
         show: bool = True,
         values_only: bool = False,
-    ):
+    ) -> Union[Tuple[np.ndarray, np.ndarray], Optional["Figure"]]:
         """
         Plot the bending moment.
 
         :param factor: Influence the plotting scale.
         :param verbosity:  0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
@@ -1130,15 +1135,15 @@
         factor: Optional[float] = None,
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
         show: bool = True,
         values_only: bool = False,
-    ):
+    ) -> Union[Tuple[np.ndarray, np.ndarray], Optional["Figure"]]:
         """
         Plot the axial force.
 
         :param factor: Influence the plotting scale.
         :param verbosity:  0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
@@ -1157,15 +1162,15 @@
         factor: Optional[float] = None,
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
         show: bool = True,
         values_only: bool = False,
-    ):
+    ) -> Union[Tuple[np.ndarray, np.ndarray], Optional["Figure"]]:
         """
         Plot the shear force.
 
         :param factor: Influence the plotting scale.
         :param verbosity:  0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
@@ -1182,15 +1187,15 @@
     def show_reaction_force(
         self,
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
         show: bool = True,
-    ):
+    ) -> Union[Tuple[np.ndarray, np.ndarray], Optional["Figure"]]:
         """
         Plot the reaction force.
 
         :param verbosity: 0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
         :param figsize: Change the figure size.
@@ -1205,15 +1210,15 @@
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
         show: bool = True,
         linear: bool = False,
         values_only: bool = False,
-    ):
+    ) -> Union[Tuple[np.ndarray, np.ndarray], Optional["Figure"]]:
         """
         Plot the displacement.
 
         :param factor: Influence the plotting scale.
         :param verbosity:  0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
@@ -1233,15 +1238,15 @@
     def show_results(
         self,
         verbosity: int = 0,
         scale: float = 1,
         offset: Tuple[float, float] = (0, 0),
         figsize: Optional[Tuple[float, float]] = None,
         show: bool = True,
-    ):
+    ) -> Optional["Figure"]:
         """
         Plot all the results in one window.
 
         :param verbosity: 0: All information, 1: Suppress information.
         :param scale: Scale of the plot.
         :param offset: Offset the plots location on the figure.
         :param figsize: Change the figure size.
@@ -1451,19 +1456,19 @@
         :param unit:
             - 'shear'
             - 'moment'
             - 'axial'
 
         """
         if unit == "shear":
-            return [el.shear_force[0] for el in self.element_map.values()]  # type: ignore
+            return [el.shear_force[0] for el in self.element_map.values()]
         elif unit == "moment":
-            return [el.bending_moment[0] for el in self.element_map.values()]  # type: ignore
+            return [el.bending_moment[0] for el in self.element_map.values()]
         elif unit == "axial":
-            return [el.axial_force[0] for el in self.element_map.values()]  # type: ignore
+            return [el.axial_force[0] for el in self.element_map.values()]
         else:
             raise NotImplementedError
 
     def get_node_result_range(self, unit: str) -> List[float]:
         """
         Query a list with node results.
 
@@ -1485,21 +1490,21 @@
         """
         Retrieve the ID of a certain location.
 
         :param vertex:  Vertex_xz, [x, y], (x, y)
         :return:  id of the node at the location of the vertex
         """
         if isinstance(vertex, (list, tuple)):
-            vertex = Vertex(vertex)
+            vertex_v = Vertex(vertex)
         try:
             tol = 1e-9
-            return next(  # type: ignore
+            return next(
                 filter(
-                    lambda x: math.isclose(x.vertex.x, vertex.x, abs_tol=tol)  # type: ignore
-                    and math.isclose(x.vertex.y, vertex.y, abs_tol=tol),  # type: ignore
+                    lambda x: math.isclose(x.vertex.x, vertex_v.x, abs_tol=tol)
+                    and math.isclose(x.vertex.y, vertex_v.y, abs_tol=tol),
                     self.node_map.values(),
                 )
             ).id
         except StopIteration:
             return None
 
     def nodes_range(
@@ -1532,28 +1537,26 @@
         Retrieve the nearest node ID.
 
         :param dimension: "both", 'x', 'y' or 'z'
         :param val: Value of the dimension.
         :return:  ID of the node.
         """
         if dimension == "both" and isinstance(val, Sequence):
-            match = list(
-                map(
-                    lambda x: x[1],  # type: ignore
-                    filter(
-                        lambda x: x[0][0] == val[0] and x[0][1] == val[1],  # type: ignore
-                        zip(self.nodes_range("both"), self.node_map.keys()),
-                    ),
+            return int(
+                np.argmin(
+                    np.sqrt(
+                        (np.array(self.nodes_range("x")) - val[0]) ** 2
+                        + (np.array(self.nodes_range("y")) - val[1]) ** 2
+                    )
                 )
             )
-            return match[0] if len(match) > 0 else None
         else:
             return int(np.argmin(np.abs(np.array(self.nodes_range(dimension)) - val)))
 
-    def discretize(self, n: int = 10):
+    def discretize(self, n: int = 10) -> None:
         """
         Takes an already defined :class:`.SystemElements` object and increases the number
         of elements.
 
         :param n: Divide the elements into n sub-elements.
         """
         ss = SystemElements(
@@ -1614,15 +1617,15 @@
                 element_id=element_id,
                 direction="y",
                 q_perp=[i[0] / self.load_factor for i in forces_q],
             )
 
         self.__dict__ = ss.__dict__.copy()
 
-    def remove_loads(self, dead_load: bool = False):
+    def remove_loads(self, dead_load: bool = False) -> None:
         """
         Remove all the applied loads from the structure.
 
         :param dead_load: Remove the dead load.
         """
 
         self.loads_point = {}
@@ -1632,34 +1635,34 @@
         for k in self.element_map:  # pylint: disable=consider-using-dict-items
             self.element_map[k].q_load = (0.0, 0.0)
             if dead_load:
                 self.element_map[k].dead_load = 0
         if dead_load:
             self.loads_dead_load = set()
 
-    def apply_load_case(self, loadcase: LoadCase):
+    def apply_load_case(self, loadcase: LoadCase) -> None:
         for method, kwargs in loadcase.spec.items():
             method = method.split("-")[0]
             kwargs = re.sub(r"[{}]", "", str(kwargs))
             # pass the groups that match back to the replace
             kwargs = re.sub(r".??(\w+).?:", r"\1=", kwargs)
 
             exec(f"self.{method}({kwargs})")  # pylint: disable=exec-used
 
-    def __deepcopy__(self, memo):
+    def __deepcopy__(self, _: str) -> "SystemElements":
         system = copy.copy(self)
         mesh = self.plotter.mesh
         system.plotter = None
         system.post_processor = None
         system.plot_values = None
 
         system.__dict__ = copy.deepcopy(system.__dict__)
         system.plotter = plotter.Plotter(system, mesh)
         system.post_processor = post_sl(system)
-        system.plot_values = plotter.PlottingValues
+        system.plot_values = plotter.PlottingValues(system, mesh)
 
         return system
 
 
 def _negative_index_to_id(idx: int, collection: Collection[int]) -> int:
     if idx > 0:
         return idx
```

### Comparing `anastruct-1.4.1/anastruct/fem/system_components/assembly.py` & `anastruct-1.4.2/anastruct/fem/system_components/assembly.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import math
 from typing import TYPE_CHECKING, List, Tuple
+
 import numpy as np
-from anastruct.fem.elements import det_moment, det_shear, det_axial
 
+from anastruct.fem.elements import det_axial, det_moment, det_shear
 
 if TYPE_CHECKING:
-    from anastruct.fem.system import SystemElements
     from anastruct.fem.elements import Element
+    from anastruct.fem.system import SystemElements
 
 
 def set_force_vector(
     system: "SystemElements", force_list: List[Tuple[int, int, float]]
-):
+) -> np.ndarray:
     """
     :param force_list: list containing tuples with the
     1. number of the node,
     2. the number of the direction (1 = x, 2 = z, 3 = y)
     3. the force
     [(1, 3, 1000)] node=1, direction=3 (y), force=1000
     list may contain multiple tuples
@@ -24,43 +25,43 @@
     assert system.system_force_vector is not None
     for id_, direction, force in force_list:
         system.system_force_vector[(id_ - 1) * 3 + direction - 1] += force
 
     return system.system_force_vector
 
 
-def prep_matrix_forces(system: "SystemElements"):
+def prep_matrix_forces(system: "SystemElements") -> None:
     system.system_force_vector = system.system_force_vector = np.zeros(
         len(system._vertices) * 3
     )
     apply_perpendicular_q_load(system)
     apply_parallel_qn_load(system)
     apply_point_load(system)
     apply_moment_load(system)
 
 
-def apply_moment_load(system: "SystemElements"):
+def apply_moment_load(system: "SystemElements") -> None:
     for node_id, Ty in system.loads_moment.items():
         set_force_vector(system, [(node_id, 3, Ty)])
 
 
-def apply_point_load(system: "SystemElements"):
+def apply_point_load(system: "SystemElements") -> None:
     for node_id in system.loads_point:
         Fx, Fz = system.loads_point[node_id]
         # system force vector.
         set_force_vector(
             system,
             [
                 (node_id, 1, Fx),
                 (node_id, 2, Fz),
             ],
         )
 
 
-def apply_perpendicular_q_load(system: "SystemElements"):
+def apply_perpendicular_q_load(system: "SystemElements") -> None:
     for element_id in system.loads_dead_load:
         element = system.element_map[element_id]
         qi_perpendicular = element.all_qp_load[0]
         q_perpendicular = element.all_qp_load[1]
         if q_perpendicular == 0 and qi_perpendicular == 0:
             continue
 
@@ -102,15 +103,15 @@
             (element.node_id1 - 1) * 3 : (element.node_id1 - 1) * 3 + 3
         ] += primary_force[0:3]
         system.system_force_vector[
             (element.node_id2 - 1) * 3 : (element.node_id2 - 1) * 3 + 3
         ] += primary_force[3:]
 
 
-def apply_parallel_qn_load(system: "SystemElements"):
+def apply_parallel_qn_load(system: "SystemElements") -> None:
     for element_id in system.loads_dead_load:
         element = system.element_map[element_id]
         qni_parallel = element.all_qn_load[0]
         qn_parallel = element.all_qn_load[1]
         if qn_parallel == 0 and qni_parallel == 0:
             continue
 
@@ -136,22 +137,22 @@
                 (element.node_2.id, 2, rright_z),
                 (element.node_1.id, 1, rleft_x),
                 (element.node_2.id, 1, rright_x),
             ],
         )
 
 
-def dead_load(system: "SystemElements", g: float, element_id: int):
+def dead_load(system: "SystemElements", g: float, element_id: int) -> None:
     system.loads_dead_load.add(element_id)
     system.element_map[element_id].dead_load = g
 
 
 def assemble_system_matrix(
     system: "SystemElements", validate: bool = False, geometric_matrix: bool = False
-):
+) -> None:
     """
     Shape of the matrix = n nodes * n d.o.f.
     Shape = n * 3
     """
     system._remainder_indexes = []
     if not geometric_matrix:
         shape = len(system.node_map) * 3
@@ -198,15 +199,17 @@
         system.system_matrix[n2 : n2 + 3, n2 : n2 + 3] += element_matrix[3:6, 3:]
 
     # returns True if symmetrical.
     if validate:
         assert np.allclose((system.system_matrix.transpose()), system.system_matrix)
 
 
-def set_displacement_vector(system, nodes_list):
+def set_displacement_vector(
+    system: "SystemElements", nodes_list: List[Tuple[int, int]]
+) -> np.ndarray:
     """
     :param nodes_list: list containing tuples with
     1.the node
     2. the d.o.f. that is set
     :return: Vector with the displacements of the nodes (If displacement is not known,
              the value is set
     to NaN)
@@ -224,32 +227,34 @@
                 e,
                 "This often occurs if you set supports before the all the elements are modelled. "
                 "First finish the model.",
             ) from e
     return system.system_displacement_vector
 
 
-def process_conditions(system):
+def process_conditions(system: "SystemElements") -> None:
     indexes = []
     # remove the unsolvable values from the matrix and vectors
+    assert system.shape_system_matrix is not None
+    assert system.system_displacement_vector is not None
     for i in range(system.shape_system_matrix):
         if system.system_displacement_vector[i] == 0:
             indexes.append(i)
         else:
             system._remainder_indexes.append(i)
 
     system.system_displacement_vector = np.delete(
         system.system_displacement_vector, indexes, 0
     )
     system.reduced_force_vector = np.delete(system.system_force_vector, indexes, 0)
     system.reduced_system_matrix = np.delete(system.system_matrix, indexes, 0)
     system.reduced_system_matrix = np.delete(system.reduced_system_matrix, indexes, 1)
 
 
-def process_supports(system):
+def process_supports(system: "SystemElements") -> None:
     for node in system.supports_hinged:
         set_displacement_vector(system, [(node.id, 1), (node.id, 2)])
 
     for i, supports_rolli in enumerate(system.supports_roll):
         if not system.supports_roll_rotate[i]:
             set_displacement_vector(
                 system,
```

### Comparing `anastruct-1.4.1/anastruct/fem/system_components/solver.py` & `anastruct-1.4.2/anastruct/fem/system_components/solver.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/anastruct/fem/system_components/util.py` & `anastruct-1.4.2/anastruct/fem/system_components/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Dict, Optional, Sequence, Tuple, Union
+
+from anastruct.basic import FEMException, angle_x_axis
 from anastruct.fem.node import Node
 from anastruct.vertex import Vertex
-from anastruct.basic import FEMException, angle_x_axis
-
 
 if TYPE_CHECKING:
-    from anastruct.fem.system import SystemElements, Spring
+    from anastruct.fem.system import Spring, SystemElements
 
 
-def check_internal_hinges(system: "SystemElements", node_id: int):
+def check_internal_hinges(system: "SystemElements", node_id: int) -> None:
     """
     Identify internal hinges, set their hinge status
 
     Parameters
     ----------
     node_id
         Id of the node in the system
@@ -56,64 +56,95 @@
 
 def append_node_id(
     system: "SystemElements",
     point_1: Vertex,
     point_2: Vertex,
     node_id1: int,
     node_id2: int,
-):
+) -> None:
     if node_id1 not in system.node_map:
         system.node_map[node_id1] = Node(node_id1, vertex=point_1)
     if node_id2 not in system.node_map:
         system.node_map[node_id2] = Node(node_id2, vertex=point_2)
 
 
-def det_vertices(system, location_list):
+def det_vertices(
+    system: "SystemElements",
+    location_list: Union[
+        Vertex,
+        Sequence[Vertex],
+        Sequence[int],
+        Sequence[float],
+        Sequence[Sequence[float]],
+    ],
+) -> Tuple[Vertex, Vertex]:
     if isinstance(location_list, Vertex):
         point_1 = system._previous_point
         point_2 = Vertex(location_list)
-    elif len(location_list) == 1:
+    elif len(location_list) == 1 and isinstance(location_list[0], Sequence):
         point_1 = system._previous_point
         point_2 = Vertex(location_list[0][0], location_list[0][1])
-    elif isinstance(location_list[0], (int, float)):
+    elif isinstance(location_list[0], (int, float)) and isinstance(
+        location_list[1], (int, float)
+    ):
         point_1 = system._previous_point
         point_2 = Vertex(location_list[0], location_list[1])
-    elif isinstance(location_list[0], Vertex):
+    elif isinstance(location_list[0], Vertex) and isinstance(location_list[1], Vertex):
         point_1 = location_list[0]
         point_2 = location_list[1]
-    else:
+    elif isinstance(location_list[0], Sequence) and isinstance(
+        location_list[1], Sequence
+    ):
         point_1 = Vertex(location_list[0][0], location_list[0][1])
         point_2 = Vertex(location_list[1][0], location_list[1][1])
     system._previous_point = point_2
 
     return point_1, point_2
 
 
-def det_node_ids(system, point_1, point_2):
+def det_node_ids(
+    system: "SystemElements", point_1: Vertex, point_2: Vertex
+) -> Tuple[int, int]:
     node_ids = []
     for p in (point_1, point_2):
-        k = str(p)
+        # k = str(p)
+        k = p
         if k in system._vertices:
             node_id = system._vertices[k]
         else:
             node_id = len(system._vertices) + 1
             system._vertices[k] = node_id
         node_ids.append(node_id)
     return node_ids[0], node_ids[1]
 
 
-def support_check(system, node_id):
+def support_check(system: "SystemElements", node_id: int) -> None:
     if system.node_map[node_id].hinge:
         raise FEMException(
             "Flawed inputs",
             "You cannot add a rotation-restraining support to a hinged node.",
         )
 
 
-def force_elements_orientation(point_1, point_2, node_id1, node_id2, spring, mp):
+def force_elements_orientation(
+    point_1: Vertex,
+    point_2: Vertex,
+    node_id1: int,
+    node_id2: int,
+    spring: Optional[Dict[int, float]],
+    mp: Optional[Dict[int, float]],
+) -> Tuple[
+    Vertex,
+    Vertex,
+    int,
+    int,
+    Optional[Dict[int, float]],
+    Optional[Dict[int, float]],
+    float,
+]:
     """
     Forces the elements to be in the first and the last quadrant of the unity circle.
     Meaning the first node is always left and the last node is always right. Or they
     are both on one vertical line.
 
     The angle of the element will thus always be between -90 till +90 degrees.
     :return: point_1, point_2, node_id1, node_id2, spring, mp, ai
```

### Comparing `anastruct-1.4.1/anastruct/fem/util/load.py` & `anastruct-1.4.2/anastruct/fem/util/load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,114 +1,136 @@
-import pprint
 import copy
-from typing import Sequence
-from anastruct.basic import args_to_lists
+import pprint
+from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Union
+
+from anastruct.basic import arg_to_list
+
+if TYPE_CHECKING:
+    from anastruct.fem.system import SystemElements
 
 
 class LoadCase:
     """
     Group different loads in a load case
     """
 
-    def __init__(self, name):
+    def __init__(self, name: str):
         """
         :param name: (str) Name of the load case
         """
-        self.name = name
-        self.spec = dict()
-        self.c = 0
+        self.name: str = name
+        self.spec: dict = dict()
+        self.c: int = 0
 
-    def q_load(self, q, element_id, direction="element", rotation=None, q_perp=None):
+    def q_load(
+        self,
+        q: Union[float, Sequence[float]],
+        element_id: Union[int, Sequence[int]],
+        direction: Union[str, Sequence[str]] = "element",
+        rotation: Optional[Union[float, Sequence[float]]] = None,
+        q_perp: Optional[Union[float, Sequence[float]]] = None,
+    ) -> None:
         """
         Apply a q-load to an element.
 
         :param element_id: (int/ list) representing the element ID
         :param q: (flt) value of the q-load
         :param direction: (str) "element", "x", "y", "parallel"
         """
-        if q_perp is None:
-            q_perp = [0, 0]
-        if not isinstance(q, Sequence):
-            q = [q, q]
-        if not isinstance(q_perp, Sequence):
-            q_perp = [q_perp, q_perp]
         self.c += 1
         self.spec[f"q_load-{self.c}"] = dict(
             q=q,
             element_id=element_id,
             direction=direction,
             rotation=rotation,
             q_perp=q_perp,
         )
 
-    def point_load(self, node_id, Fx=0, Fy=0, rotation=0):
+    def point_load(
+        self,
+        node_id: Union[int, Sequence[int]],
+        Fx: Union[float, Sequence[float]] = 0,
+        Fy: Union[float, Sequence[float]] = 0,
+        rotation: Union[float, Sequence[float]] = 0,
+    ) -> None:
         """
         Apply a point load to a node.
 
         :param node_id: (int/ list) Nodes ID.
         :param Fx: (flt/ list) Force in global x direction.
         :param Fy: (flt/ list) Force in global x direction.
         :param rotation: (flt/ list) Rotate the force clockwise. Rotation is in degrees.
         """
         self.c += 1
         self.spec[f"point_load-{self.c}"] = dict(
             node_id=node_id, Fx=Fx, Fy=Fy, rotation=rotation
         )
 
-    def moment_load(self, node_id, Ty):
+    def moment_load(
+        self, node_id: Union[int, Sequence[int]], Ty: Union[float, Sequence[float]]
+    ) -> None:
         """
         Apply a moment on a node.
 
         :param node_id: (int/ list) Nodes ID.
         :param Ty: (flt/ list) Moments acting on the node.
         """
         self.c += 1
         self.spec[f"moment_load-{self.c}"] = dict(node_id=node_id, Ty=Ty)
 
-    def dead_load(self, element_id, g):
+    def dead_load(
+        self, element_id: Union[int, Sequence[int]], g: Union[float, Sequence[float]]
+    ) -> None:
         """
         Apply a dead load in kN/m on elements.
 
         :param element_id: (int/ list) representing the element ID
         :param g: (flt/ list) Weight per meter. [kN/m] / [N/m]
         """
         self.c += 1
         self.spec[f"dead_load-{self.c}"] = dict(element_id=element_id, g=g)
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Loadcase {self.name}:\n" + pprint.pformat(self.spec)
 
 
 class LoadCombination:
-    def __init__(self, name):
-        self.name = name
-        self.spec = dict()
+    def __init__(self, name: str):
+        self.name: str = name
+        self.spec: dict = dict()
 
-    def add_load_case(self, lc, factor):
+    def add_load_case(
+        self,
+        lc: Union[LoadCase, Sequence[LoadCase]],
+        factor: Union[float, Sequence[float]],
+    ) -> None:
         """
         Add a load case to the load combination.
 
         :param lc: (:class:`anastruct.fem.util.LoadCase`)
         :param factor: (flt) Multiply all the loads in this LoadCase with this factor.
         """
-        lc, factor = args_to_lists(  # pylint: disable=unbalanced-tuple-unpacking
-            lc, factor
-        )
+        if isinstance(lc, LoadCase):
+            n = 1
+        else:
+            n = len(lc)
+        lc = arg_to_list(lc, n)
+        factor = arg_to_list(factor, n)
         for i, lci in enumerate(lc):
             self.spec[lci.name] = [lci, factor[i]]
 
     def solve(
         self,
-        system,
-        force_linear=False,
-        verbosity=0,
-        max_iter=200,
-        geometrical_non_linear=False,
-        **kwargs,
-    ):
+        system: "SystemElements",
+        force_linear: bool = False,
+        verbosity: int = 0,
+        max_iter: int = 200,
+        geometrical_non_linear: bool = False,
+        **kwargs: Any,
+    ) -> Dict[str, "SystemElements"]:
         """
         Evaluate the Load Combination.
 
         :param system: (:class:`anastruct.fem.system.SystemElements`) Structure to apply loads on.
         :param force_linear: (bool) Force a linear calculation. Even when the system has non
                              linear nodes.
         :param verbosity: (int) 0: Log calculation outputs. 1: silence.
```

### Comparing `anastruct-1.4.1/anastruct/material/profile.py` & `anastruct-1.4.2/anastruct/material/profile.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import csv
 import io
-
+from typing import Dict
 
 s_hea = """profiel,G,A,h,b,tw,tf,AL,Iy,Wy,Iz,Wz
 nr.,kg/m,mm2,mm,mm,mm,mm,m2/m,mm4,mm3,mm4,mm3
 100,17.0,2124,96,100,5,8,0.561,349,72.8,134,26.8
 120,20.3,2534,114,120,5,8,0.677,606,106,231,38.5
 140,25.1,3142,133,140,5.5,8.5,0.794,1033,155,389,55.6
 160,31.0,3877,152,160,6,9,0.906,1673,220,616,76.9
@@ -48,15 +48,15 @@
 400,67,8446,400,180,8.6,13.5,1.47,23128,1156,1318,146
 450,79,9882,450,190,9.4,14.6,1.61,33743,1500,1676,176
 500,92,11552,500,200,10.2,16,1.74,48199,1928,2142,214
 550,108,13442,550,210,11.1,17.2,1.88,67117,2441,2668,254
 600,125,15598,600,220,12,19,2.01,92083,3069,3387,308"""
 
 
-def load(st):
+def load(st: str) -> Dict[int, dict]:
     with io.StringIO(st) as f:
         r = csv.reader(f)
         profile = {}
 
         headers = next(r)
         next(r)  # units not needed
         for row in r:
```

### Comparing `anastruct-1.4.1/anastruct/vertex.py` & `anastruct-1.4.2/anastruct/vertex.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 from __future__ import annotations
+
 import math
-from typing import Union, Sequence
+from typing import Sequence, Union
+
 import numpy as np
 
 
 class Vertex:
     """
     Utility point in 2D.
     """
 
     def __init__(
         self,
-        x: Union[Vertex, Sequence[int], Sequence[float], int, float],
+        x: Union[Vertex, Sequence[int], Sequence[float], np.ndarray, int, float],
         y: Union[int, float, None] = None,
     ):
         """
         :param x: Can be any of int, float, coordinate list, or other vertex.
         :param y: (int, flt)
         """
         if isinstance(x, (Sequence)):
@@ -39,72 +41,81 @@
     def z(self) -> float:
         return float(self.coordinates[1] * -1)
 
     def modulus(self) -> float:
         return float(np.sqrt(np.sum(self.coordinates**2)))
 
     def unit(self) -> Vertex:
-        return 1 / self.modulus() * self
+        return (1 / self.modulus()) * self
 
-    def displace_polar(self, alpha, radius, inverse_z_axis=False):
+    def displace_polar(
+        self, alpha: float, radius: float, inverse_z_axis: bool = False
+    ) -> None:
         if inverse_z_axis:
             self.coordinates[0] += math.cos(alpha) * radius
             self.coordinates[1] -= math.sin(alpha) * radius
         else:
             self.coordinates[0] += math.cos(alpha) * radius
             self.coordinates[1] += math.sin(alpha) * radius
 
-    def __add__(self, other):
+    def __add__(self, other: Union[Vertex, tuple, list, np.ndarray, float]) -> Vertex:
         if isinstance(other, (tuple, list)):
             other = np.asarray(other)
         if isinstance(other, Vertex):
             other = other.coordinates
 
         coordinates = self.coordinates + other
         return Vertex(coordinates)
 
-    def __radd__(self, other):
+    def __radd__(self, other: Union[Vertex, tuple, list, np.ndarray, float]) -> Vertex:
         return self.__add__(other)
 
-    def __sub__(self, other):
+    def __sub__(self, other: Union[Vertex, tuple, list, np.ndarray, float]) -> Vertex:
         if isinstance(other, (tuple, list)):
             other = np.asarray(other)
         if isinstance(other, Vertex):
             other = other.coordinates
 
         coordinates = self.coordinates - other
         return Vertex(coordinates)
 
-    def __rsub__(self, other):
+    def __rsub__(self, other: Union[Vertex, tuple, list, np.ndarray, float]) -> Vertex:
         return self.__sub__(other)
 
-    def __mul__(self, other):
+    def __mul__(self, other: Union[Vertex, tuple, list, np.ndarray, float]) -> Vertex:
         if isinstance(other, (tuple, list)):
             other = np.asarray(other)
         if isinstance(other, Vertex):
             other = other.coordinates
 
         coordinates = self.coordinates * other
         return Vertex(coordinates)
 
-    def __rmul__(self, other):
+    def __rmul__(self, other: Union[Vertex, tuple, list, np.ndarray, float]) -> Vertex:
         return self.__mul__(other)
 
-    def __truediv__(self, other):
+    def __truediv__(
+        self, other: Union[Vertex, tuple, list, np.ndarray, float]
+    ) -> Vertex:
         if isinstance(other, (tuple, list)):
             other = np.asarray(other)
         if isinstance(other, Vertex):
             other = other.coordinates
 
         coordinates = self.coordinates / other
         return Vertex(coordinates)
 
-    def __eq__(self, other):
-        return self.x == other.x and self.y == other.y
+    def __eq__(self, other: object) -> bool:
+        if isinstance(other, Vertex):
+            return self.x == other.x and self.y == other.y
+        return NotImplemented
 
-    def __str__(self):
+    def __str__(self) -> str:
         return f"Vertex({self.x}, {self.y})"
 
+    def __hash__(self) -> int:
+        return hash(str(self))
+
 
-def vertex_range(v1, v2, n):
+def vertex_range(v1: Vertex, v2: Vertex, n: int) -> list:
     dv = v2 - v1
     return [v1 + dv * i / n for i in range(n + 1)]
```

### Comparing `anastruct-1.4.1/anastruct.egg-info/PKG-INFO` & `anastruct-1.4.2/anastruct.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,35 @@
 Metadata-Version: 2.1
 Name: anastruct
-Version: 1.4.1
-Summary: analyse 2D structures.
-Home-page: https://ritchievink.com
-Download-URL: https://github.com/ritchie46/anaStruct
-Author: Ritchie Vink
-Author-email: ritchie46@gmail.com
+Version: 1.4.2
+Summary: Finite element analysis of 2D structures
+Author-email: Ritchie Vink <ritchie46@gmail.com>
+Maintainer-email: Brooks Smith <smith120bh@gmail.com>
 License: GPL-3.0
+Project-URL: homepage, https://github.com/ritchie46/anaStruct
+Project-URL: documentation, http://anastruct.readthedocs.io
+Project-URL: author, https://ritchievink.com
+Keywords: FEA,finite element,structural engineering,structural analysis
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Physics
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Intended Audience :: Science/Research
+Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: plot
 Provides-Extra: test
 Provides-Extra: dev
 License-File: LICENSE.txt
 
 # anaStruct 2D Frames and Trusses
-![tests and fmt](https://github.com/ritchie46/anaStruct/workflows/tests%20and%20fmt/badge.svg)
+[![Python tests](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml/badge.svg)](https://github.com/ritchie46/anaStruct/actions/workflows/test.yaml)
 [![Documentation Status](https://readthedocs.org/projects/anastruct/badge/?version=latest)](http://anastruct.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/anaStruct/lobby.svg)](https://gitter.im/anaStruct/lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
 
 Analyse 2D Frames and trusses for slender structures. Determine the bending moments, shear forces, axial forces and displacements.
 
 ## Installation
 
 For the actively developed version:
 ```
```

### Comparing `anastruct-1.4.1/anastruct.egg-info/SOURCES.txt` & `anastruct-1.4.2/anastruct.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 LICENSE.txt
 MANIFEST.in
 README.md
-setup.py
+_custom_build.py
+dev_requirements.txt
+plot_requirements.txt
+pyproject.toml
+requirements.txt
+test_requirements.txt
 anastruct/__init__.py
 anastruct/_version.py
 anastruct/basic.py
+anastruct/py.typed
 anastruct/vertex.py
 anastruct.egg-info/PKG-INFO
 anastruct.egg-info/SOURCES.txt
 anastruct.egg-info/dependency_links.txt
 anastruct.egg-info/requires.txt
 anastruct.egg-info/top_level.txt
 anastruct/cython/__init__.py
+anastruct/cython/basic.c
 anastruct/cython/basic.py
 anastruct/cython/cbasic.pyx
 anastruct/fem/__init__.py
 anastruct/fem/elements.py
 anastruct/fem/node.py
 anastruct/fem/postprocess.py
 anastruct/fem/system.py
 anastruct/fem/cython/__init__.py
 anastruct/fem/cython/celements.pyx
+anastruct/fem/cython/elements.c
 anastruct/fem/cython/elements.py
 anastruct/fem/examples/__init__.py
 anastruct/fem/examples/ex_1.py
 anastruct/fem/examples/ex_10_dead_load.py
 anastruct/fem/examples/ex_11.py
 anastruct/fem/examples/ex_12.py
 anastruct/fem/examples/ex_13.py
@@ -64,13 +72,10 @@
 anastruct/material/__init__.py
 anastruct/material/profile.py
 anastruct/material/units.py
 anastruct/sectionbase/__init__.py
 anastruct/sectionbase/properties.py
 anastruct/sectionbase/sectionbase.py
 anastruct/sectionbase/units.py
-anastruct/sectionbase/data/sectionbase_AmericanSectionDatabase.xml
-anastruct/sectionbase/data/sectionbase_BritishSectionDatabase.xml
-anastruct/sectionbase/data/sectionbase_EuropeanSectionDatabase.xml
 tests/test_e2e.py
 tests/test_plotter.py
 tests/test_sectionbase.py
```

### Comparing `anastruct-1.4.1/tests/test_e2e.py` & `anastruct-1.4.2/tests/test_e2e.py`

 * *Files 27% similar despite different names*

```diff
@@ -718,7 +718,291 @@
             )
             assert results["combination"].get_node_results_system(5)["Fx"] == approx(
                 wind_Fx + cables_Fx
             )
             assert results["combination"].get_node_results_system(5)["Fy"] == approx(
                 wind_Fy + cables_Fy
             )
+
+
+def describe_analytical_validation_tests():
+    @pspec_context("Validation tests of results, based upon analytical equations")
+    def describe():
+        pass
+
+    def context_simply_supported_beam_validation():
+        @pspec_context("Simply-supported beam with UDL validation")
+        def describe():
+            pass
+
+        w = 1
+        l = 2
+        EI = 10000
+        EA = 1000
+
+        system = SystemElements(EI=EI, EA=EA, mesh=10000)
+        system.add_element([[0, 0], [l, 0]])
+        system.add_support_hinged([1, 2])
+        system.q_load(w, element_id=1)
+        system.solve()
+
+        def it_results_in_correct_moment_shear():
+            assert system.get_element_results(1)["Mmax"] == approx(w * l**2 / 8)
+            assert system.get_element_results(1)["Qmax"] == approx(w * l / 2)
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(w * l / 2)
+            assert system.get_node_results_system(2)["Fy"] == approx(w * l / 2)
+
+        def it_results_in_correct_deflections():
+            assert system.get_element_results(1)["wmax"] == approx(
+                -5 * w * l**4 / (384 * EI)
+            )
+
+    def context_simply_supported_two_point_loads():
+        @pspec_context("Validation tests of results, based upon analytical equations")
+        def describe():
+            pass
+
+        p = 80
+        l = 5
+        a = l / 3
+        EI = 14000
+
+        system = SystemElements(EI=EI, mesh=10000)
+        system.add_element([[0, 0], [a, 0]])
+        system.add_element([[a, 0], [2 * a, 0]])
+        system.add_element([[2 * a, 0], [l, 0]])
+        system.add_support_hinged([1, 4])
+        system.point_load(node_id=2, Fy=p)
+        system.point_load(node_id=3, Fy=p)
+        system.solve()
+
+        def it_results_in_correct_moment_shear():
+            assert system.get_element_results(2)["Mmax"] == approx(p * a)
+            assert system.get_element_results(1)["Qmax"] == approx(p)
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(p)
+            assert system.get_node_results_system(4)["Fy"] == approx(p)
+
+        def it_results_in_correct_deflections():
+            assert system.get_node_results_system(3)["uy"] + system.get_element_results(
+                2
+            )["wmax"] == approx(-((p * a) / (24 * EI)) * (3 * (l**2) - 4 * (a**2)))
+
+    def context_simply_supported_beam_point_load_validation():
+        @pspec_context("Simply-supported beam with point load at center validation")
+        def describe():
+            pass
+
+        w = 1
+        l = 2
+        EI = 10000
+        EA = 1000
+        p = 1
+
+        system = SystemElements(EI=EI, EA=EA, mesh=10000)
+        system.add_element([[0, 0], [l / 2, 0]])
+        system.add_element([[l / 2, 0], [l, 0]])
+        system.add_support_hinged([1, 3])
+        system.point_load(2, Fx=0, Fy=p, rotation=0)
+        system.solve()
+
+        def it_results_in_correct_moment_shear():
+            assert system.get_element_results(1)["Mmax"] == approx(p * l / 4)
+            assert system.get_element_results(1)["Qmax"] == approx(p / 2)
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(p / 2)
+            assert system.get_node_results_system(3)["Fy"] == approx(p / 2)
+
+        def it_results_in_correct_deflections():
+            assert system.get_node_results_system(2)["uy"] == approx(
+                -p * l**3 / (48 * EI)
+            )
+
+    def context_fixed_ends_beam_point_load_validation():
+        @pspec_context("Beam fixed at both ends with concentrated load at center")
+        def describe():
+            pass
+
+        p = 200
+        l = 8
+        x = 3
+        EI = 23000
+
+        system = SystemElements(EI=EI, mesh=9000)
+        system.add_element([[0, 0], [x, 0]])
+        system.add_element([[x, 0], [l / 2, 0]])
+        system.add_element([[l / 2, 0], [l, 0]])
+        system.add_support_fixed([1, 4])
+        system.point_load(3, Fx=0, Fy=200, rotation=0)
+        system.solve()
+
+        def it_results_in_correct_moment_shear():
+            assert system.get_element_results(2)["Mmin"] == approx(p / 8 * (4 * x - l))
+            assert system.get_element_results(2)["Qmax"] == approx(p / 2)
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(p / 2)
+            assert system.get_node_results_system(4)["Fy"] == approx(p / 2)
+
+        def it_results_in_correct_deflections():
+            assert system.get_node_results_system(2)["uy"] == approx(
+                -p * x**2 / (48 * EI) * (3 * l - 4 * x)
+            )
+
+    def context_3_span_continuous_beam_2_UDL_loads_validation():
+        @pspec_context(
+            "Continuous Beam spanning over three supports with two UDL in the outer spans"
+        )
+        def describe():
+            pass
+
+        w = 70
+        l = 5
+        EI = 15000
+
+        system = SystemElements(EI=EI, mesh=20000)
+        system.add_element([[0, 0], [l, 0]])
+        system.add_element([[l, 0], [2 * l, 0]])
+        system.add_element([[2 * l, 0], [3 * l, 0]])
+        system.add_support_hinged([1, 2, 3, 4])
+        system.q_load(w, element_id=1)
+        system.q_load(w, element_id=3)
+        system.solve()
+
+        def it_results_in_correct_moment_shear():
+            assert system.get_element_results(1)["Mmax"] == approx(0.10125 * w * l**2)
+            assert system.get_element_results(2)["Mmax"] == approx(-0.050 * w * l**2)
+            assert system.get_element_results(1)["Qmin"] == approx(-0.55 * w * l)
+            assert system.get_element_results(2)["Qmax"] == approx(0)
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(0.45 * w * l)
+            assert system.get_node_results_system(3)["Fy"] == approx(0.55 * w * l)
+
+        def it_results_in_correct_deflections():
+            assert system.get_element_results(1)["wmax"] == approx(
+                -0.009917469 * w * l**4 / EI
+            )
+
+            def it_results_in_correct_deflections():
+                assert system.get_node_results_system(2)["uy"] == approx(
+                    -p * l**3 / (48 * EI)
+                )
+
+    def context_fixed1end_simplySupported_UDL_validation():
+        @pspec_context(
+            "beam fixed at one end and simply supported at the other with UDL"
+        )
+        def describe():
+            pass
+
+        EA = 3420000  # KN.m/m
+        EI = 83100  # KN.m^2
+        w = 1  # KN/m
+        l = 2  # m
+
+        system = SystemElements(EA=EA, EI=EI)
+        system.add_element([[0, 0], [l, 0]])
+        system.add_support_hinged(1)
+        system.add_support_fixed(2)
+        system.q_load(w, element_id=1)
+        system.solve()
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(3 * w * l / 8)
+            assert system.get_node_results_system(2)["Fy"] == approx(5 * w * l / 8)
+            assert system.get_node_results_system(2)["Ty"] == approx(-w * (l**2) / 8)
+
+        def it_results_in_correct_deflections():
+            assert system.get_element_results(1)["wmax"] == approx(
+                -w * (l**4) / (185 * EI), rel=1e-3
+            )
+
+    def context_fixed1end_simplySupported_pointLoad_validation():
+        @pspec_context(
+            "beam fixed at one end and simply supported on other with point load at the middle"
+        )
+        def describe():
+            pass
+
+        EA = 3420000  # KN.m/m
+        EI = 83100  # KN.m^2
+        p = 1  # KN
+        l = 2  # m
+
+        system = SystemElements(EA=EA, EI=EI, mesh=10000)
+        system.add_element([[0, 0], [l * (1 / 5) ** 0.5, 0]])
+        system.add_element([[l * (1 / 5) ** 0.5, 0], [l / 2, 0]])
+        system.add_element([[l / 2, 0], [l, 0]])
+        system.add_support_hinged(1)
+        system.add_support_fixed(4)
+        system.point_load(3, Fx=0, Fy=p, rotation=0)
+        system.solve()
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(5 * p / 16)
+            assert system.get_node_results_system(4)["Fy"] == approx(11 * p / 16)
+            assert system.get_node_results_system(4)["Ty"] == approx(-3 * p * l / 16)
+
+        def it_results_in_correct_deflections():
+            assert system.get_node_results_system(2)["uy"] == approx(
+                -p * (l**3) / (48 * EI * 5**0.5)
+            )
+
+    def context_beam_fixed_on_both_ends_UDL():
+        @pspec_context("beam with fixed supports at both ends and UDL")
+        def describe():
+            pass
+
+        EA = 3420000  # KN.m/m
+        EI = 83100  # KN.m^2
+        w = 1  # KN/m
+        l = 2  # m
+
+        system = SystemElements(EA=EA, EI=EI, mesh=2000)
+        system.add_element([[0, 0], [l, 0]])
+        system.add_support_fixed([1, 2])
+        system.q_load(w, 1)
+        system.solve()
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(1)["Fy"] == approx(w * l / 2)
+            assert system.get_node_results_system(2)["Fy"] == approx(w * l / 2)
+            assert system.get_node_results_system(1)["Ty"] == approx(w * l**2 / 12)
+            assert system.get_node_results_system(2)["Ty"] == approx(-w * l**2 / 12)
+
+        def it_results_in_correct_deflections():
+            assert system.get_element_results(1)["wmax"] == approx(
+                -w * l**4 / (384 * EI)
+            )
+
+    def context_cantilever_UDL_validation():
+        @pspec_context("Cantilever beam with UDL validation")
+        def describe():
+            pass
+
+        w = 10
+        l = 3
+        EI = 10000
+        EA = 1000
+
+        system = SystemElements(EI=EI, EA=EA, mesh=100)
+        system.add_element([[0, 0], [l, 0]])
+        system.add_support_fixed([2])
+        system.q_load(w, element_id=1)
+        system.solve()
+
+        def it_results_in_correct_moment_shear():
+            assert system.get_element_results(1)["Mmin"] == approx(-w * l**2 / 2)
+            assert system.get_element_results(1)["Qmin"] == approx(-w * l)
+
+        def it_results_in_correct_reactions():
+            assert system.get_node_results_system(2)["Fy"] == approx(w * l)
+
+        def it_results_in_correct_deflections():
+            assert system.get_node_results_system(1)["uy"] == approx(
+                -w * l**4 / (8 * EI)
+            )
```

### Comparing `anastruct-1.4.1/tests/test_plotter.py` & `anastruct-1.4.2/tests/test_plotter.py`

 * *Files identical despite different names*

### Comparing `anastruct-1.4.1/tests/test_sectionbase.py` & `anastruct-1.4.2/tests/test_sectionbase.py`

 * *Files identical despite different names*

