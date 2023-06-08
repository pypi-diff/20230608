# Comparing `tmp/lincs-0.3.7.tar.gz` & `tmp/lincs-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.3.7.tar", last modified: Wed May 31 15:12:03 2023, max compression
+gzip compressed data, was "lincs-0.4.0.tar", last modified: Thu Jun  8 08:00:09 2023, max compression
```

## Comparing `lincs-0.3.7.tar` & `lincs-0.4.0.tar`

### file list

```diff
@@ -1,60 +1,70 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.902400 lincs-0.3.7/
--rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-05-12 12:03:36.000000 lincs-0.3.7/COPYING
--rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-05-12 12:04:16.000000 lincs-0.3.7/COPYING.LESSER
--rw-rw-r--   0 user      (1002) user      (1002)      104 2023-05-12 11:51:00.000000 lincs-0.3.7/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)     4458 2023-05-31 15:12:03.902400 lincs-0.3.7/PKG-INFO
--rw-rw-r--   0 user      (1002) user      (1002)     3574 2023-05-31 15:11:59.000000 lincs-0.3.7/README.rst
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      796 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/__init__.py
--rw-rw-r--   0 user      (1002) user      (1002)      170 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    21977 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     1610 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/classification.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      368 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/classification.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10039 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/generation.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1042 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/generation.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/io/
--rw-rw-r--   0 user      (1002) user      (1002)     2461 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io/alternatives.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1004 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io/alternatives.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2582 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io/domain.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io/domain.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1875 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io/model.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1640 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io/model.hpp
--rw-rw-r--   0 user      (1002) user      (1002)       53 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      186 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/io.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/learning/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     9494 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     2125 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
--rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
--rw-rw-r--   0 user      (1002) user      (1002)     4495 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      922 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
--rw-rw-r--   0 user      (1002) user      (1002)      244 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      682 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     6757 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     3486 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     1727 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      551 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/learning.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    15121 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      245 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/median-and-max.cpp
--rw-rw-r--   0 user      (1002) user      (1002)      751 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/median-and-max.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      776 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/randomness-utils.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     1539 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs/randomness-utils.hpp
--rw-rw-r--   0 user      (1002) user      (1002)    10418 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/liblincs_module_tests.py
--rw-rw-r--   0 user      (1002) user      (1002)      793 2023-05-12 11:51:00.000000 lincs-0.3.7/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-31 15:12:03.898400 lincs-0.3.7/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)     4458 2023-05-31 15:12:03.000000 lincs-0.3.7/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     1875 2023-05-31 15:12:03.000000 lincs-0.3.7/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-31 15:12:03.000000 lincs-0.3.7/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-31 15:12:03.000000 lincs-0.3.7/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-31 15:12:03.000000 lincs-0.3.7/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-31 15:12:03.000000 lincs-0.3.7/lincs.egg-info/top_level.txt
--rw-rw-r--   0 user      (1002) user      (1002)       61 2023-05-12 11:51:00.000000 lincs-0.3.7/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-31 15:12:03.902400 lincs-0.3.7/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     2445 2023-05-31 15:11:43.000000 lincs-0.3.7/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.112882 lincs-0.4.0/
+-rw-rw-r--   0 user      (1002) user      (1002)    35149 2023-06-05 12:32:48.000000 lincs-0.4.0/COPYING
+-rw-rw-r--   0 user      (1002) user      (1002)     7652 2023-06-05 12:32:35.000000 lincs-0.4.0/COPYING.LESSER
+-rw-rw-r--   0 user      (1002) user      (1002)      109 2023-06-05 12:32:35.000000 lincs-0.4.0/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)     4918 2023-06-08 08:00:09.112882 lincs-0.4.0/PKG-INFO
+-rw-rw-r--   0 user      (1002) user      (1002)     4034 2023-06-08 08:00:04.000000 lincs-0.4.0/README.rst
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      955 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/__init__.py
+-rw-rw-r--   0 user      (1002) user      (1002)      170 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    23086 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     1627 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/classification.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      369 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/classification.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    10079 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/generation.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1046 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/generation.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/io/
+-rw-rw-r--   0 user      (1002) user      (1002)     2468 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/alternatives.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1012 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/alternatives.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1886 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/model.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1648 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/model.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2610 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/problem.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1892 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io/problem.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       53 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/io.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      187 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/io.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.104882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/
+-rw-rw-r--   0 user      (1002) user      (1002)     1495 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     9267 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1577 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    14338 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
+-rw-rw-r--   0 user      (1002) user      (1002)     1817 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/
+-rw-rw-r--   0 user      (1002) user      (1002)     4406 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1265 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/
+-rw-rw-r--   0 user      (1002) user      (1002)     3974 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      787 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/
+-rw-rw-r--   0 user      (1002) user      (1002)      244 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      682 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     6764 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     3490 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4697 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      968 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/learning.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    16951 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      245 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/lincs.hpp
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.112882 lincs-0.4.0/lincs/liblincs/linear-programming/
+-rw-rw-r--   0 user      (1002) user      (1002)       57 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/linear-programming/alglib.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2719 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs/linear-programming/alglib.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)       55 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/linear-programming/glop.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1697 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/linear-programming/glop.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1579 2023-06-08 07:34:21.000000 lincs-0.4.0/lincs/liblincs/linear-programming/test.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     2963 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/median-and-max.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)      751 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/median-and-max.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      776 2023-06-05 12:32:35.000000 lincs-0.4.0/lincs/liblincs/randomness-utils.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     1736 2023-06-08 06:59:23.000000 lincs-0.4.0/lincs/liblincs/randomness-utils.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)    13993 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/liblincs_module_tests.py
+-rw-rw-r--   0 user      (1002) user      (1002)     1403 2023-06-08 07:34:07.000000 lincs-0.4.0/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-06-08 08:00:09.108882 lincs-0.4.0/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)     4918 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     2438 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-06-08 08:00:09.000000 lincs-0.4.0/lincs.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1002) user      (1002)       61 2023-06-05 12:32:35.000000 lincs-0.4.0/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-06-08 08:00:09.112882 lincs-0.4.0/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     3897 2023-06-08 07:59:54.000000 lincs-0.4.0/setup.py
```

### Comparing `lincs-0.3.7/COPYING` & `lincs-0.4.0/COPYING`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/COPYING.LESSER` & `lincs-0.4.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/PKG-INFO` & `lincs-0.4.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.7
+Version: 0.4.0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -23,24 +23,24 @@
 
 .. WARNING, this README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
-*lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
-
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.7/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.7/COPYING.LESSER>`_.
-It's available on the `Python package index <https://pypi.org/project/lincs/>`_.
-Its `documentation <http://mics-lab.github.io/lincs/>`_
-and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
+*lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
+Its `documentation <http://mics-lab.github.io/lincs/>`_
+and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
 
 Contributors and previous work
 ==============================
 
 *lincs* is developed by the `MICS <https://mics.centralesupelec.fr/>`_ research team at `CentraleSupélec <https://www.centralesupelec.fr/>`_.
@@ -53,39 +53,43 @@
 - `Wassila Ouerdane <https://wassilaouerdane.github.io/>`_ (domain expertise)
 
 It's based on work by:
 
 - `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
 - Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
+@todo Add links to the fundamental articles for NCS.
+@todo Add links to the articles that define other learning methods we re-implement.
 
 Project goals
 =============
 
 Provide MCDA tools usable out of the box
 ----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
 Just follow the `Get started <#get-started>`_ section below.
 
 Provide a base for developing new MCDA algorithms
 -------------------------------------------------
 
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
-@todo Write doc about that use case.
+See our `contributor guide <https://mics-lab.github.io/lincs/contributor-guide.html>`_ for more details.
 
-*lincs* also provides a benchmark framework to compare algorithms (@todo Write and document).
+*lincs* also provides a benchmark framework to compare algorithms (@todo Implement and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
 
 Get started
 ===========
 
 Depending on your favorite approach, you can either start with our `hands-on "Get started" guide <https://mics-lab.github.io/lincs/get-started.html>`_
 or with our `conceptual overview documentation <https://mics-lab.github.io/lincs/conceptual-overview.html>`_.
+The former will show you how to use our tools, the latter will explain the concepts behind them: what's MCDA, what are NCS models, *etc.*
+If in doubt, start with the conceptual overview.
 We highly recommend you read the other one just after.
 
 Once you've used *lincs* a bit, you can follow up with our `user guide <https://mics-lab.github.io/lincs/user-guide.html>`_
 and `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_.
 
 
 Develop *lincs* itself
```

### Comparing `lincs-0.3.7/README.rst` & `lincs-0.4.0/README.rst`

 * *Files 9% similar despite different names*

```diff
@@ -2,24 +2,24 @@
 
 .. WARNING, this README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
-*lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
+*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
 *lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <COPYING>`_ and `COPYING.LESSER <COPYING.LESSER>`_.
-It's available on the `Python package index <https://pypi.org/project/lincs/>`_.
-Its `documentation <http://mics-lab.github.io/lincs/>`_
-and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
-
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
+*lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
+Its `documentation <http://mics-lab.github.io/lincs/>`_
+and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
 
 Contributors and previous work
 ==============================
 
 *lincs* is developed by the `MICS <https://mics.centralesupelec.fr/>`_ research team at `CentraleSupélec <https://www.centralesupelec.fr/>`_.
@@ -32,39 +32,43 @@
 - `Wassila Ouerdane <https://wassilaouerdane.github.io/>`_ (domain expertise)
 
 It's based on work by:
 
 - `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
 - Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
+@todo Add links to the fundamental articles for NCS.
+@todo Add links to the articles that define other learning methods we re-implement.
 
 Project goals
 =============
 
 Provide MCDA tools usable out of the box
 ----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
 Just follow the `Get started <#get-started>`_ section below.
 
 Provide a base for developing new MCDA algorithms
 -------------------------------------------------
 
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
-@todo Write doc about that use case.
+See our `contributor guide <https://mics-lab.github.io/lincs/contributor-guide.html>`_ for more details.
 
-*lincs* also provides a benchmark framework to compare algorithms (@todo Write and document).
+*lincs* also provides a benchmark framework to compare algorithms (@todo Implement and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
 
 Get started
 ===========
 
 Depending on your favorite approach, you can either start with our `hands-on "Get started" guide <https://mics-lab.github.io/lincs/get-started.html>`_
 or with our `conceptual overview documentation <https://mics-lab.github.io/lincs/conceptual-overview.html>`_.
+The former will show you how to use our tools, the latter will explain the concepts behind them: what's MCDA, what are NCS models, *etc.*
+If in doubt, start with the conceptual overview.
 We highly recommend you read the other one just after.
 
 Once you've used *lincs* a bit, you can follow up with our `user guide <https://mics-lab.github.io/lincs/user-guide.html>`_
 and `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_.
 
 
 Develop *lincs* itself
```

### Comparing `lincs-0.3.7/lincs/__init__.py` & `lincs-0.4.0/lincs/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 # Copyright 2023 Vincent Jacques
 
-from liblincs import ValueType, CategoryCorrelation, Criterion, Category, Domain, load_domain, generate_domain
+from liblincs import ValueType, CategoryCorrelation, Criterion, Category, Problem, load_problem, generate_problem
 from liblincs import SufficientCoalitionsKind, SufficientCoalitions, Boundary, Model, load_model, generate_mrsort_model
 from liblincs import Alternative, Alternatives, load_alternatives, generate_alternatives, classify_alternatives
 from liblincs import ProfilesInitializationStrategy, InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion
-from liblincs import WeightsOptimizationStrategy, OptimizeWeightsUsingGlop
-from liblincs import ProfilesImprovementStrategy, ImproveProfilesWithAccuracyHeuristic
+from liblincs import WeightsOptimizationStrategy, OptimizeWeightsUsingGlop, OptimizeWeightsUsingAlglib
+from liblincs import ProfilesImprovementStrategy, ImproveProfilesWithAccuracyHeuristicOnCpu, ImproveProfilesWithAccuracyHeuristicOnGpu
 from liblincs import TerminationStrategy, TerminateAtAccuracy
-from liblincs import make_models, WeightsProfilesBreedMrSortLearning
+from liblincs import make_models, make_gpu_models, WeightsProfilesBreedMrSortLearning
+
+# @todo Accept learning and training set as Pandas DataFrame?
```

### Comparing `lincs-0.3.7/lincs/command_line_interface.py` & `lincs-0.4.0/lincs/command_line_interface.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright 2023 Vincent Jacques
 
 from __future__ import annotations
 import math
+import os
 import random
 import subprocess
 import sys
 
 import click
 
 import lincs
@@ -14,28 +15,38 @@
 
 def options_tree(name, kwds, dependents):
     """
     Ad-hoc decorator for a tree dependent of click.options.
     Options down the tree are only valid if the options up the tree are set to specific values.
     Think of them as sub-options of the previous ones.
     """
+
     def decorator(command):
         def walk(
             option_name_prefix_,
             parameter_name_prefix_,
             conditions_,
             name_,
             kwds_,
             dependents_,
         ):
             if conditions_:
-                conditions__ = "\n\n\b\nOnly valid if:\n"
+                # \b prevents rewrapping of the paragraph by Click
+                # (https://click.palletsprojects.com/en/8.1.x/api/#click.wrap_text)
+                conditions__ = f"\n\n\b\nOnly valid if:\n"
+                if os.environ.get("LINCS_GENERATING_SPHINX_DOC") == "1":
+                    conditions__ += "\n"
+                    quote = "``"
+                else:
+                    quote = "'"
                 for (k, v) in conditions_:
-                    conditions__ += f" - '{k}' is '{v}'\n"
-                conditions__ += "\n\n*"
+                    conditions__ += f"- {quote}{k}{quote} is {quote}{v}{quote}\n"
+                # This non-blocking space ensures Click does not put the default
+                # value on the same line as the last condition
+                conditions__ += f"\n\n "
 
             for value__, dependents__ in dependents_.items():
                 for name___, kwds___, dependents___ in reversed(dependents__):
                     walk(
                         f"{option_name_prefix_}{value__}.",
                         f"{parameter_name_prefix_}{value__.replace('-', '_')}__",
                         conditions_ + [(f"--{option_name_prefix_}{name_}", value__)],
@@ -107,15 +118,15 @@
         print("=" * len(f"lincs.{obj_name}"))
         print()
         if obj.__doc__:
             print(obj.__doc__)
             print()
         if isinstance(obj, type):
             for attr_name in sorted(dir(obj)):
-                if attr_name.startswith("_"):  # @todo Include __init__ and some other dunders
+                if attr_name.startswith("_") and attr_name not in ["__init__"]:  # @todo Include some other dunders
                     continue
                 if (
                     obj_name in {"CategoryCorrelation", "SufficientCoalitionsKind", "ValueType"}
                     and
                     attr_name in {"as_integer_ratio", "bit_count", "bit_length", "conjugate", "denominator", "from_bytes", "imag", "numerator", "to_bytes", "attr_name", "name", "names", "values"}
                 ):
                     continue
@@ -139,62 +150,62 @@
 )
 def generate():
     pass
 
 
 @generate.command(
     help="""
-        Generate a synthetic classification domain.
+        Generate a synthetic classification problem.
 
-        The generated domain has CRITERIA_COUNT criteria and CATEGORIES_COUNT categories.
+        The generated problem has CRITERIA_COUNT criteria and CATEGORIES_COUNT categories.
     """,
 )
 @click.argument(
     "criteria-count",
     type=click.IntRange(min=1),
 )
 @click.argument(
     "categories-count",
     type=click.IntRange(min=1),
 )
 @click.option(
-    "--output-domain",
+    "--output-problem",
     type=click.File(mode="w"),
     default="-",
-    help="Write generated domain to this file instead of standard output.",
+    help="Write generated problem to this file instead of standard output.",
 )
 @click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
     default=random.randrange(2**30),
 )
-def classification_domain(
+def classification_problem(
     criteria_count,
     categories_count,
-    output_domain,
+    output_problem,
     random_seed
 ):
-    domain = lincs.generate_domain(
+    problem = lincs.generate_problem(
         criteria_count,
         categories_count,
         random_seed=random_seed,
     )
-    domain.dump(output_domain)
+    problem.dump(output_problem)
 
 
 @generate.command(
     help="""
         Generate a synthetic classification model.
 
-        DOMAIN is a *classification domain* file describing the domain to generate a model for.
+        PROBLEM is a *classification problem* file describing the problem to generate a model for.
     """,
 )
 @click.argument(
-    "domain",
+    "problem",
     type=click.File(mode="r"),
 )
 @click.option(
     "--output-model",
     type=click.File(mode="w"),
     default="-",
     help="Write generated model to this file instead of standard output.",
@@ -225,40 +236,40 @@
                 ),
                 {},
             ),
         ],
     },
 )
 def classification_model(
-    domain,
+    problem,
     output_model,
     random_seed,
     model_type,
     mrsort__fixed_weights_sum,
 ):
-    domain = lincs.load_domain(domain)
+    problem = lincs.load_problem(problem)
     assert model_type == "mrsort"
     model = lincs.generate_mrsort_model(
-        domain,
+        problem,
         random_seed=random_seed,
         fixed_weights_sum=mrsort__fixed_weights_sum,
     )
     model.dump(output_model)
 
 
 @generate.command(
     help="""
         Generate synthetic classified alternatives.
 
-        DOMAIN is a *classification domain* file describing the domain to generate alternatives for.
-        MODEL is a *classification model* file for that domain describing the model to use to classify the generated alternatives.
+        PROBLEM is a *classification problem* file describing the problem to generate alternatives for.
+        MODEL is a *classification model* file for that problem describing the model to use to classify the generated alternatives.
     """,
 )
 @click.argument(
-    "domain",
+    "problem",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.argument(
@@ -280,25 +291,25 @@
 @click.option(
     "--random-seed",
     help="The random seed to use.",
     type=click.IntRange(min=0),
     default=random.randrange(2**30),
 )
 def classified_alternatives(
-    domain,
+    problem,
     model,
     alternatives_count,
     output_classified_alternatives,
     max_imbalance,
     random_seed,
 ):
-    domain = lincs.load_domain(domain)
-    model = lincs.load_model(domain, model)
+    problem = lincs.load_problem(problem)
+    model = lincs.load_model(problem, model)
     alternatives = lincs.generate_alternatives(
-        domain,
+        problem,
         model,
         alternatives_count,
         random_seed=random_seed,
         max_imbalance=max_imbalance,
     )
     alternatives.dump(output_classified_alternatives)
 
@@ -310,21 +321,21 @@
     pass
 
 
 @visualize.command(
     help="""
         Visualize a classification model.
 
-        DOMAIN is a *classification domain* file.
-        MODEL is a *classification model* file for that domain describing the model to visualize.
+        PROBLEM is a *classification problem* file.
+        MODEL is a *classification model* file for that problem describing the model to visualize.
         The generated image is written to the OUTPUT file in PNG format.
     """,
 )
 @click.argument(
-    "domain",
+    "problem",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.option(
@@ -338,45 +349,45 @@
     help="Add only this number of alternatives.",
 )
 @click.argument(
     "output",
     type=click.File(mode="wb"),
 )
 def classification_model(
-    domain,
+    problem,
     model,
     alternatives,
     alternatives_count,
     output,
 ):
-    domain = lincs.load_domain(domain)
-    model = lincs.load_model(domain, model)
+    problem = lincs.load_problem(problem)
+    model = lincs.load_model(problem, model)
     if alternatives is not None:
-        alternatives = lincs.load_alternatives(domain, alternatives)
-    lincs.visualization.visualize_model(domain, model, alternatives, alternatives_count, output)
+        alternatives = lincs.load_alternatives(problem, alternatives)
+    lincs.visualization.visualize_model(problem, model, alternatives, alternatives_count, output)
 
 
 @main.group(
     help="Learn a model.",
 )
 def learn():
     pass
 
 
 @learn.command(
     help="""
         Learn a classification model.
 
-        DOMAIN is a *classification domain* file describing the domain to learn a model for.
-        LEARNING_SET is a *classified alternatives* file for that domain.
+        PROBLEM is a *classification problem* file describing the problem to learn a model for.
+        LEARNING_SET is a *classified alternatives* file for that problem.
         It's used as a source of truth to learn the model.
     """,
 )
 @click.argument(
-    "domain",
+    "problem",
     type=click.File(mode="r"),
 )
 @click.argument(
     "learning-set",
     type=click.File(mode="r"),
 )
 @click.option(
@@ -456,15 +467,15 @@
                             ),
                             {
                                 "linear-program": [
                                     (
                                         "solver",
                                         dict(
                                             help="The solver to use to solve the linear programs. See (@todo Add link to doc) for details of available solvers.",
-                                            type=click.Choice(["glop"]),
+                                            type=click.Choice(["glop", "alglib"]),
                                             default="glop",
                                             show_default=True,
                                         ),
                                         {},
                                     ),
                                 ],
                             },
@@ -488,15 +499,15 @@
                                         ),
                                         {},
                                     ),
                                     (
                                         "processor",
                                         dict(
                                             help="The processor to use to improve the profiles of the MRSort models.",
-                                            type=click.Choice(["cpu"]),
+                                            type=click.Choice(["cpu", "gpu"]),
                                             default="cpu",
                                             show_default=True,
                                         ),
                                         {},
                                     ),
                                 ],
                             },
@@ -527,15 +538,15 @@
                     ],
                 },
             ),
         ],
     },
 )
 def classification_model(
-    domain,
+    problem,
     learning_set,
     output_model,
     model_type,
     mrsort__strategy,
     mrsort__weights_profiles_breed__target_accuracy,
     mrsort__weights_profiles_breed__max_iterations,
     mrsort__weights_profiles_breed__models_count,
@@ -544,34 +555,39 @@
     mrsort__weights_profiles_breed__linear_program__solver,
     mrsort__weights_profiles_breed__profiles_strategy,
     mrsort__weights_profiles_breed__accuracy_heuristic__random_seed,
     mrsort__weights_profiles_breed__accuracy_heuristic__processor,
     mrsort__weights_profiles_breed__breed_strategy,
     mrsort__weights_profiles_breed__reinitialize_least_accurate__portion,
 ):
-    domain = lincs.load_domain(domain)
-    learning_set = lincs.load_alternatives(domain, learning_set)
+    problem = lincs.load_problem(problem)
+    learning_set = lincs.load_alternatives(problem, learning_set)
 
     if model_type == "mrsort":
         if mrsort__strategy == "weights-profiles-breed":
-            models = lincs.make_models(domain, learning_set, mrsort__weights_profiles_breed__models_count, mrsort__weights_profiles_breed__accuracy_heuristic__random_seed)
+            models = lincs.make_models(problem, learning_set, mrsort__weights_profiles_breed__models_count, mrsort__weights_profiles_breed__accuracy_heuristic__random_seed)
 
             assert mrsort__weights_profiles_breed__max_iterations is None
             termination_strategy = lincs.TerminateAtAccuracy(math.ceil(mrsort__weights_profiles_breed__target_accuracy * len(learning_set.alternatives)))
 
             if mrsort__weights_profiles_breed__initialization_strategy == "maximize-discrimination-per-criterion":
                 profiles_initialization_strategy = lincs.InitializeProfilesForProbabilisticMaximalDiscriminationPowerPerCriterion(models)
 
             if mrsort__weights_profiles_breed__weights_strategy == "linear-program":
                 if mrsort__weights_profiles_breed__linear_program__solver == "glop":
                     weights_optimization_strategy = lincs.OptimizeWeightsUsingGlop(models)
+                elif mrsort__weights_profiles_breed__linear_program__solver == "alglib":
+                    weights_optimization_strategy = lincs.OptimizeWeightsUsingAlglib(models)
 
             if mrsort__weights_profiles_breed__profiles_strategy == "accuracy-heuristic":
                 if mrsort__weights_profiles_breed__accuracy_heuristic__processor == "cpu":
-                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristic(models)
+                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristicOnCpu(models)
+                elif mrsort__weights_profiles_breed__accuracy_heuristic__processor == "gpu":
+                    gpu_models = lincs.make_gpu_models(models)
+                    profiles_improvement_strategy = lincs.ImproveProfilesWithAccuracyHeuristicOnGpu(models, gpu_models)
 
             assert mrsort__weights_profiles_breed__breed_strategy == "reinitialize-least-accurate"
             assert mrsort__weights_profiles_breed__reinitialize_least_accurate__portion == 0.5
 
             learning = lincs.WeightsProfilesBreedMrSortLearning(
                 models,
                 profiles_initialization_strategy,
@@ -584,21 +600,21 @@
     model.dump(output_model)
 
 
 @main.command(
     help="""
         Classify alternatives.
 
-        DOMAIN is a *classification domain* file.
-        MODEL is a *classification model* file for that domain.
-        ALTERNATIVES is an *unclassified alternatives* file for that domain.
+        PROBLEM is a *classification problem* file.
+        MODEL is a *classification model* file for that problem.
+        ALTERNATIVES is an *unclassified alternatives* file for that problem.
     """,
 )
 @click.argument(
-    "domain",
+    "problem",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.argument(
@@ -608,52 +624,52 @@
 @click.option(
     "--output-classified-alternatives",
     type=click.File(mode="w"),
     default="-",
     help="Write classified alternatives to this file instead of standard output.",
 )
 def classify(
-    domain,
+    problem,
     model,
     alternatives,
     output_classified_alternatives,
 ):
-    domain = lincs.load_domain(domain)
-    model = lincs.load_model(domain, model)
-    alternatives = lincs.load_alternatives(domain, alternatives)
-    lincs.classify_alternatives(domain, model, alternatives)
+    problem = lincs.load_problem(problem)
+    model = lincs.load_model(problem, model)
+    alternatives = lincs.load_alternatives(problem, alternatives)
+    lincs.classify_alternatives(problem, model, alternatives)
     alternatives.dump(output_classified_alternatives)
 
 
 @main.command(
     help="""
         Compute a classification accuracy.
 
-        DOMAIN is a *classification domain* file.
-        MODEL is a *classification model* file for that domain.
-        TESTING_SET is a *classified alternatives* file for that domain.
+        PROBLEM is a *classification problem* file.
+        MODEL is a *classification model* file for that problem.
+        TESTING_SET is a *classified alternatives* file for that problem.
 
         The classification accuracy is written to standard output as an integer between 0 and the number of alternatives.
     """,
 )
 @click.argument(
-    "domain",
+    "problem",
     type=click.File(mode="r"),
 )
 @click.argument(
     "model",
     type=click.File(mode="r"),
 )
 @click.argument(
     "testing-set",
     type=click.File(mode="r"),
 )
 def classification_accuracy(
-    domain,
+    problem,
     model,
     testing_set,
 ):
-    domain = lincs.load_domain(domain)
-    model = lincs.load_model(domain, model)
-    testing_set = lincs.load_alternatives(domain, testing_set)
-    result = lincs.classify_alternatives(domain, model, testing_set)
+    problem = lincs.load_problem(problem)
+    model = lincs.load_model(problem, model)
+    testing_set = lincs.load_alternatives(problem, testing_set)
+    result = lincs.classify_alternatives(problem, model, testing_set)
     print(f"{result.unchanged}/{result.changed + result.unchanged}")
```

### Comparing `lincs-0.3.7/lincs/liblincs/classification.cpp` & `lincs-0.4.0/lincs/liblincs/classification.cpp`

 * *Files 13% similar despite different names*

```diff
@@ -3,42 +3,42 @@
 #include "classification.hpp"
 
 #include <cassert>
 
 
 namespace lincs {
 
-ClassificationResult classify_alternatives(const Domain& domain, const Model& model, Alternatives* alternatives) {
-  assert(&(model.domain) == &domain);
-  assert(&(alternatives->domain) == &domain);
+ClassificationResult classify_alternatives(const Problem& problem, const Model& model, Alternatives* alternatives) {
+  assert(&(model.problem) == &problem);
+  assert(&(alternatives->problem) == &problem);
 
-  const unsigned criteria_count = domain.criteria.size();
-  const unsigned categories_count = domain.categories.size();
+  const unsigned criteria_count = problem.criteria.size();
+  const unsigned categories_count = problem.categories.size();
 
   ClassificationResult result{0, 0};
 
   for (auto& alternative: alternatives->alternatives) {
-    uint category_index;
+    unsigned category_index;
     for (category_index = categories_count - 1; category_index != 0; --category_index) {
       const auto& boundary = model.boundaries[category_index - 1];
       assert(boundary.sufficient_coalitions.kind == Model::SufficientCoalitions::Kind::weights);
       float weight_at_or_above_profile = 0;
-      for (uint criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
+      for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
         const float alternative_value = alternative.profile[criterion_index];
         const float profile_value = boundary.profile[criterion_index];
         if (alternative_value >= profile_value) {
           weight_at_or_above_profile += boundary.sufficient_coalitions.criterion_weights[criterion_index];
         }
       }
       if (weight_at_or_above_profile >= 1.f) {
         break;
       }
     }
 
-    const std::string& category = domain.categories[category_index].name;
+    const std::string& category = problem.categories[category_index].name;
     if (alternative.category == category) {
       ++result.unchanged;
     } else {
       alternative.category = category;
       ++result.changed;
     }
   }
```

### Comparing `lincs-0.3.7/lincs/liblincs/generation.cpp` & `lincs-0.4.0/lincs/liblincs/generation.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -7,58 +7,58 @@
 #include <random>
 
 #include "classification.hpp"
 
 
 namespace lincs {
 
-Domain generate_domain(const unsigned criteria_count, const unsigned categories_count, const unsigned random_seed) {
+Problem generate_problem(const unsigned criteria_count, const unsigned categories_count, const unsigned random_seed) {
   // There is nothing random yet. There will be when other value types and category correlations are added.
 
-  std::vector<Domain::Criterion> criteria;
+  std::vector<Problem::Criterion> criteria;
   criteria.reserve(criteria_count);
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
     criteria.emplace_back(
       "Criterion " + std::to_string(criterion_index + 1),
-      Domain::Criterion::ValueType::real,
-      Domain::Criterion::CategoryCorrelation::growing
+      Problem::Criterion::ValueType::real,
+      Problem::Criterion::CategoryCorrelation::growing
     );
   }
 
-  std::vector<Domain::Category> categories;
+  std::vector<Problem::Category> categories;
   categories.reserve(categories_count);
   for (unsigned category_index = 0; category_index != categories_count; ++category_index) {
     categories.emplace_back(
       "Category " + std::to_string(category_index + 1)
     );
   }
 
-  return Domain{criteria, categories};
+  return Problem{criteria, categories};
 }
 
-Model generate_mrsort_model(const Domain& domain, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
-  const unsigned categories_count = domain.categories.size();
-  const unsigned criteria_count = domain.criteria.size();
+Model generate_mrsort_model(const Problem& problem, const unsigned random_seed, const std::optional<float> fixed_weights_sum) {
+  const unsigned categories_count = problem.categories.size();
+  const unsigned criteria_count = problem.criteria.size();
 
   std::mt19937 gen(random_seed);
 
   // Profile can take any values. We arbitrarily generate them uniformly
   std::uniform_real_distribution<float> values_distribution(0.01f, 0.99f);
   // (Values clamped strictly inside ']0, 1[' to make it easier to generate balanced learning sets)
   std::vector<std::vector<float>> profiles(categories_count - 1, std::vector<float>(criteria_count));
-  for (uint crit_index = 0; crit_index != criteria_count; ++crit_index) {
+  for (unsigned crit_index = 0; crit_index != criteria_count; ++crit_index) {
     // Profiles must be ordered on each criterion, so we generate a random column...
     std::vector<float> column(categories_count - 1);
     std::generate(
       column.begin(), column.end(),
       [&values_distribution, &gen]() { return values_distribution(gen); });
     // ... sort it...
     std::sort(column.begin(), column.end());
     // ... and assign that column across all profiles.
-    for (uint profile_index = 0; profile_index != categories_count - 1; ++profile_index) {
+    for (unsigned profile_index = 0; profile_index != categories_count - 1; ++profile_index) {
       profiles[profile_index][crit_index] = column[profile_index];
     }
   }
 
   // Weights are a bit trickier.
   // We first generate partial sums of weights...
   std::uniform_real_distribution<float> partial_sums_distribution(0.0f, 1.f);
@@ -93,47 +93,47 @@
 
   std::vector<Model::Boundary> boundaries;
   boundaries.reserve(categories_count - 1);
   for (unsigned category_index = 0; category_index != categories_count - 1; ++category_index) {
     boundaries.emplace_back(profiles[category_index], coalitions);
   }
 
-  return Model(domain, boundaries);
+  return Model(problem, boundaries);
 }
 
 Alternatives generate_uniform_alternatives(
-  const Domain& domain,
+  const Problem& problem,
   const Model& model,
   const unsigned alternatives_count,
   std::mt19937& gen
 ) {
-  const unsigned criteria_count = domain.criteria.size();
+  const unsigned criteria_count = problem.criteria.size();
 
   std::vector<Alternative> alternatives;
   alternatives.reserve(alternatives_count);
 
   // We don't do anything to ensure homogeneous repartition amongst categories.
   // We just generate random profiles uniformly in [0, 1]
   std::uniform_real_distribution<float> values_distribution(0.0f, 1.0f);
 
-  for (uint alt_index = 0; alt_index != alternatives_count; ++alt_index) {
+  for (unsigned alt_index = 0; alt_index != alternatives_count; ++alt_index) {
     std::vector<float> criteria_values(criteria_count);
     std::generate(
       criteria_values.begin(), criteria_values.end(),
       [&values_distribution, &gen]() { return values_distribution(gen); });
 
     alternatives.push_back(Alternative{
       "Alternative " + std::to_string(alt_index + 1),
       criteria_values,
       std::nullopt,
     });
   }
 
-  Alternatives alts{domain, alternatives};
-  classify_alternatives(domain, model, &alts);
+  Alternatives alts{problem, alternatives};
+  classify_alternatives(problem, model, &alts);
 
   return alts;
 }
 
 unsigned min_category_size(const unsigned alternatives_count, const unsigned categories_count, const float max_imbalance) {
   assert(max_imbalance >= 0);
   assert(max_imbalance <= 1);
@@ -145,24 +145,24 @@
   assert(max_imbalance >= 0);
   assert(max_imbalance <= 1);
 
   return std::ceil(alternatives_count * (1 + max_imbalance) / categories_count);
 }
 
 Alternatives generate_balanced_alternatives(
-  const Domain& domain,
+  const Problem& problem,
   const Model& model,
   const unsigned alternatives_count,
   const float max_imbalance,
   std::mt19937& gen
 ) {
   assert(max_imbalance >= 0);
   assert(max_imbalance <= 1);
 
-  const unsigned categories_count = domain.categories.size();
+  const unsigned categories_count = problem.categories.size();
 
   // These parameters are somewhat arbitrary and not really critical,
   // but changing there values *does* change the generated set, because of the two-steps process below:
   // the same alternatives are generated in the same order, but they treated differently here.
 
   // How long to insist before accepting failure when we can't find any alternative for a given category
   const int max_iterations_with_no_effect_with_empty_category = 100;
@@ -176,27 +176,27 @@
 
   const unsigned min_size = min_category_size(alternatives_count, categories_count, max_imbalance);
   const unsigned max_size = max_category_size(alternatives_count, categories_count, max_imbalance);
 
   std::vector<Alternative> alternatives;
   alternatives.reserve(alternatives_count);
   std::map<std::string, unsigned> histogram;
-  for (const auto& category : domain.categories) {
+  for (const auto& category : problem.categories) {
     histogram[category.name] = 0;
   }
 
   int max_iterations_with_no_effect = max_iterations_with_no_effect_with_empty_category;
 
   // Step 1: fill all categories to exactly the min size
   // (skip if min size is zero)
   int iterations_with_no_effect = 0;
   while (min_size > 0) {
     ++iterations_with_no_effect;
 
-    Alternatives candidates = generate_uniform_alternatives(domain, model, multiplier * alternatives_count, gen);
+    Alternatives candidates = generate_uniform_alternatives(problem, model, multiplier * alternatives_count, gen);
 
     for (const auto& candidate : candidates.alternatives) {
       assert(candidate.category);
       const std::string& category = *candidate.category;
       if (histogram[category] < min_size) {
         alternatives.push_back(candidate);
         ++histogram[category];
@@ -219,49 +219,49 @@
   }
 
   // Step 2: reach target size, keeping all categories below or at the max size
   iterations_with_no_effect = 0;
   while (true) {
     ++iterations_with_no_effect;
 
-    Alternatives candidates = generate_uniform_alternatives(domain, model, multiplier * alternatives_count, gen);
+    Alternatives candidates = generate_uniform_alternatives(problem, model, multiplier * alternatives_count, gen);
 
     for (const auto& candidate : candidates.alternatives) {
       assert(candidate.category);
       const std::string& category = *candidate.category;
       if (histogram[category] < max_size) {
         alternatives.push_back(candidate);
         ++histogram[category];
         iterations_with_no_effect = 0;
       }
 
       if (alternatives.size() == alternatives_count) {
         assert(std::all_of(
           histogram.begin(), histogram.end(),
           [min_size, max_size](const auto it) { return it.second >= min_size && it.second <= max_size; }));
-        return Alternatives(domain, alternatives);
+        return Alternatives(problem, alternatives);
       }
     }
 
     if (iterations_with_no_effect > max_iterations_with_no_effect) {
       throw BalancedAlternativesGenerationException(histogram);
     }
   }
 }
 
 Alternatives generate_alternatives(
-  const Domain& domain,
+  const Problem& problem,
   const Model& model,
   const unsigned alternatives_count,
   const unsigned random_seed,
   const std::optional<float> max_imbalance
 ) {
   std::mt19937 gen(random_seed);
 
   if (max_imbalance) {
-    return generate_balanced_alternatives(domain, model, alternatives_count, *max_imbalance, gen);
+    return generate_balanced_alternatives(problem, model, alternatives_count, *max_imbalance, gen);
   } else {
-    return generate_uniform_alternatives(domain, model, alternatives_count, gen);
+    return generate_uniform_alternatives(problem, model, alternatives_count, gen);
   }
 }
 
 } // namespace lincs
```

### Comparing `lincs-0.3.7/lincs/liblincs/generation.hpp` & `lincs-0.4.0/lincs/liblincs/generation.hpp`

 * *Files 9% similar despite different names*

```diff
@@ -6,31 +6,31 @@
 #include <map>
 
 #include "io.hpp"
 
 
 namespace lincs {
 
-Domain generate_domain(unsigned criteria_count, unsigned categories_count, unsigned random_seed);
+Problem generate_problem(unsigned criteria_count, unsigned categories_count, unsigned random_seed);
 
-Model generate_mrsort_model(const Domain&, unsigned random_seed, std::optional<float> fixed_weights_sum = std::nullopt);
+Model generate_mrsort_model(const Problem&, unsigned random_seed, std::optional<float> fixed_weights_sum = std::nullopt);
 
 class BalancedAlternativesGenerationException : public std::exception {
  public:
   explicit BalancedAlternativesGenerationException(const std::map<std::string, unsigned>& histogram_) : histogram(histogram_) {}
 
   const char* what() const noexcept override {
     return "Unable to generate balanced alternatives. Try increasing the allowed imbalance, or use a more lenient model?";
   }
 
   std::map<std::string, unsigned> histogram;
 };
 
 Alternatives generate_alternatives(
-  const Domain&,
+  const Problem&,
   const Model&,
   unsigned alternatives_count,
   unsigned random_seed,
   std::optional<float> max_imbalance = std::nullopt
 );
 
 } // namespace lincs
```

### Comparing `lincs-0.3.7/lincs/liblincs/io/alternatives.cpp` & `lincs-0.4.0/lincs/liblincs/io/alternatives.cpp`

 * *Files 9% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 #include <rapidcsv.h>
 
 
 namespace lincs {
 
 void Alternatives::dump(std::ostream& os) const {
-  const unsigned criteria_count = domain.criteria.size();
+  const unsigned criteria_count = problem.criteria.size();
   const unsigned alternatives_count = alternatives.size();
 
   rapidcsv::Document doc;
 
   doc.SetColumnName(0, "name");
   for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
-    doc.SetColumnName(criterion_index + 1, domain.criteria[criterion_index].name);
+    doc.SetColumnName(criterion_index + 1, problem.criteria[criterion_index].name);
   }
   doc.SetColumnName(criteria_count + 1, "category");
 
   for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
     const Alternative& alternative = alternatives[alternative_index];
     doc.SetCell<std::string>(0, alternative_index, alternative.name);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
@@ -29,16 +29,16 @@
       doc.SetCell<std::string>(criteria_count + 1, alternative_index, *alternative.category);
     }
   }
 
   doc.Save(os);
 }
 
-Alternatives Alternatives::load(const Domain& domain, std::istream& is) {
-  const unsigned criteria_count = domain.criteria.size();
+Alternatives Alternatives::load(const Problem& problem, std::istream& is) {
+  const unsigned criteria_count = problem.criteria.size();
 
   // I don't know why constructing the rapidcsv::Document directly from 'is' sometimes results in an empty document.
   // So, read the whole stream into a string and construct the document from that.
   std::string s(std::istreambuf_iterator<char>(is), {});
   std::istringstream iss(s);
   rapidcsv::Document doc(iss);
 
@@ -46,20 +46,20 @@
   const unsigned alternatives_count = doc.GetRowCount();
   alternatives.reserve(alternatives_count);
   for (unsigned row_index = 0; row_index != alternatives_count; ++row_index) {
     Alternative alternative;
     alternative.name = doc.GetCell<std::string>("name", row_index);
     alternative.profile.reserve(criteria_count);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
-      alternative.profile.push_back(doc.GetCell<float>(domain.criteria[criterion_index].name, row_index));
+      alternative.profile.push_back(doc.GetCell<float>(problem.criteria[criterion_index].name, row_index));
     }
     std::string category = doc.GetCell<std::string>("category", row_index);
     if (category != "") {
       alternative.category = category;
     }
     alternatives.push_back(alternative);
   }
 
-  return Alternatives{domain, alternatives};
+  return Alternatives{problem, alternatives};
 }
 
 }  // namespace lincs
```

### Comparing `lincs-0.3.7/lincs/liblincs/io/alternatives.hpp` & `lincs-0.4.0/lincs/liblincs/io/alternatives.hpp`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 // Copyright 2023 Vincent Jacques
 
 #ifndef LINCS__IO__ALTERNATIVES_HPP
 #define LINCS__IO__ALTERNATIVES_HPP
 
 #include <optional>
 
-#include "domain.hpp"
+#include "problem.hpp"
 
 
 namespace lincs {
 
 struct Alternative {
   std::string name;
   std::vector<float> profile;
@@ -18,19 +18,19 @@
   Alternative() {}
   Alternative(const std::string& name_, const std::vector<float>& profile_, const std::optional<std::string>& category_): name(name_), profile(profile_), category(category_) {}
 
   bool operator==(const Alternative& other) const { return name == other.name && profile == other.profile && category == other.category; }
 };
 
 struct Alternatives {
-  const Domain& domain;
+  const Problem& problem;
   std::vector<Alternative> alternatives;
 
-  Alternatives(const Domain& domain_, const std::vector<Alternative>& alternatives_): domain(domain_), alternatives(alternatives_) {}
+  Alternatives(const Problem& problem_, const std::vector<Alternative>& alternatives_): problem(problem_), alternatives(alternatives_) {}
 
   void dump(std::ostream&) const;
-  static Alternatives load(const Domain&, std::istream&);
+  static Alternatives load(const Problem&, std::istream&);
 };
 
 }  // namespace lincs
 
 #endif  // LINCS__IO__ALTERNATIVES_HPP
```

### Comparing `lincs-0.3.7/lincs/liblincs/io/domain.cpp` & `lincs-0.4.0/lincs/liblincs/io/problem.cpp`

 * *Files 21% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 // Copyright 2023 Vincent Jacques
 
-#include "domain.hpp"
+#include "problem.hpp"
 
 #include <cassert>
 
 #include <magic_enum.hpp>
 #include <yaml-cpp/yaml.h>
 
 #include <doctest.h>  // Keep last because it defines really common names like CHECK that we don't want injected into other headers
 
 
 namespace YAML {
 
 template<>
-struct convert<lincs::Domain::Category> {
-  static Node encode(const lincs::Domain::Category& category) {
+struct convert<lincs::Problem::Category> {
+  static Node encode(const lincs::Problem::Category& category) {
     Node node;
     node["name"] = category.name;
 
     return node;
   }
 
-  static bool decode(const Node& node, lincs::Domain::Category& category) {
+  static bool decode(const Node& node, lincs::Problem::Category& category) {
     category.name = node["name"].as<std::string>();
 
     return true;
   }
 };
 
 template<>
-struct convert<lincs::Domain::Criterion> {
-  static Node encode(const lincs::Domain::Criterion& criterion) {
+struct convert<lincs::Problem::Criterion> {
+  static Node encode(const lincs::Problem::Criterion& criterion) {
     Node node;
     node["name"] = criterion.name;
     node["value_type"] = std::string(magic_enum::enum_name(criterion.value_type));
     node["category_correlation"] = std::string(magic_enum::enum_name(criterion.category_correlation));
 
     return node;
   }
 
-  static bool decode(const Node& node, lincs::Domain::Criterion& criterion) {
+  static bool decode(const Node& node, lincs::Problem::Criterion& criterion) {
     criterion.name = node["name"].as<std::string>();
     // @todo Handle error where value_type category_correlation does not properly convert back to enum
-    criterion.value_type = magic_enum::enum_cast<lincs::Domain::Criterion::ValueType>(node["value_type"].as<std::string>()).value();
-    criterion.category_correlation = magic_enum::enum_cast<lincs::Domain::Criterion::CategoryCorrelation>(node["category_correlation"].as<std::string>()).value();
+    criterion.value_type = magic_enum::enum_cast<lincs::Problem::Criterion::ValueType>(node["value_type"].as<std::string>()).value();
+    criterion.category_correlation = magic_enum::enum_cast<lincs::Problem::Criterion::CategoryCorrelation>(node["category_correlation"].as<std::string>()).value();
 
     return true;
   }
 };
 
 }  // namespace YAML
 
 namespace lincs {
 
-void Domain::dump(std::ostream& os) const {
+void Problem::dump(std::ostream& os) const {
   YAML::Node node;
-  node["kind"] = "classification-domain";
+  node["kind"] = "classification-problem";
   node["format_version"] = 1;
   node["criteria"] = criteria;
   node["categories"] = categories;
 
   os << node << '\n';
 }
 
-Domain Domain::load(std::istream& is) {
+Problem Problem::load(std::istream& is) {
   YAML::Node node = YAML::Load(is);
 
-  assert(node["kind"].as<std::string>() == "classification-domain");
+  assert(node["kind"].as<std::string>() == "classification-problem");
   assert(node["format_version"].as<int>() == 1);
 
-  return Domain(
+  return Problem(
     node["criteria"].as<std::vector<Criterion>>(),
     node["categories"].as<std::vector<Category>>()
   );
 }
 
-TEST_CASE("dumping then loading domain preserves data") {
-  Domain domain{
-    {{"Criterion 1", Domain::Criterion::ValueType::real, Domain::Criterion::CategoryCorrelation::growing}},
+TEST_CASE("dumping then loading problem preserves data") {
+  Problem problem{
+    {{"Criterion 1", Problem::Criterion::ValueType::real, Problem::Criterion::CategoryCorrelation::growing}},
     {{"Category 1"}, {"Category 2"}},
   };
 
   std::stringstream ss;
-  domain.dump(ss);
+  problem.dump(ss);
 
-  Domain domain2 = Domain::load(ss);
-  CHECK(domain2.criteria == domain.criteria);
-  CHECK(domain2.categories == domain.categories);
+  Problem problem2 = Problem::load(ss);
+  CHECK(problem2.criteria == problem.criteria);
+  CHECK(problem2.categories == problem.categories);
 }
 
 }  // namespace lincs
```

### Comparing `lincs-0.3.7/lincs/liblincs/io/domain.hpp` & `lincs-0.4.0/lincs/liblincs/io/problem.hpp`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__IO__DOMAIN_HPP
-#define LINCS__IO__DOMAIN_HPP
+#ifndef LINCS__IO__PROBLEM_HPP
+#define LINCS__IO__PROBLEM_HPP
 
 #include <string>
 #include <vector>
 
 
 namespace lincs {
 
-struct Domain {
+struct Problem {
   struct Criterion {
     std::string name;
 
     enum class ValueType {
       real,
       // @todo Add integer
       // @todo Add enumerated
@@ -50,17 +50,17 @@
     Category(const std::string& name_): name(name_) {}
 
     bool operator==(const Category& other) const { return name == other.name; }
   };
 
   std::vector<Category> categories;
 
-  Domain(const std::vector<Criterion>& criteria_, const std::vector<Category>& categories_): criteria(criteria_), categories(categories_) {}
+  Problem(const std::vector<Criterion>& criteria_, const std::vector<Category>& categories_): criteria(criteria_), categories(categories_) {}
 
   void dump(std::ostream&) const;
-  static Domain load(std::istream&);
+  static Problem load(std::istream&);
 
 };
 
 }  // namespace lincs
 
-#endif  // LINCS__IO__DOMAIN_HPP
+#endif  // LINCS__IO__PROBLEM_HPP
```

### Comparing `lincs-0.3.7/lincs/liblincs/io/model.cpp` & `lincs-0.4.0/lincs/liblincs/io/model.cpp`

 * *Files 6% similar despite different names*

```diff
@@ -48,24 +48,24 @@
 
 }  // namespace YAML
 
 namespace lincs {
 
 void Model::dump(std::ostream& os) const {
   YAML::Node node;
-  node["kind"] = "classification-model";
+  node["kind"] = "ncs-classification-model";
   node["format_version"] = 1;
   node["boundaries"] = boundaries;
 
   os << node << '\n';
 }
 
-Model Model::load(const Domain& domain, std::istream& is) {
+Model Model::load(const Problem& problem, std::istream& is) {
   YAML::Node node = YAML::Load(is);
 
-  assert(node["kind"].as<std::string>() == "classification-model");
+  assert(node["kind"].as<std::string>() == "ncs-classification-model");
   assert(node["format_version"].as<int>() == 1);
 
-  return Model(domain, node["boundaries"].as<std::vector<Boundary>>());
+  return Model(problem, node["boundaries"].as<std::vector<Boundary>>());
 }
 
 }  // namespace lincs
```

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -1,49 +1,50 @@
 // Copyright 2023 Vincent Jacques
 
-#include "accuracy-heuristic.hpp"
+#include "accuracy-heuristic-on-cpu.hpp"
+#include "../../../randomness-utils.hpp"
 
 
 namespace lincs {
 
-void ImproveProfilesWithAccuracyHeuristic::improve_profiles() {
+void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles() {
   #pragma omp parallel for
   for (unsigned model_index = 0; model_index != models.models_count; ++model_index) {
     improve_model_profiles(model_index);
   }
 }
 
-void ImproveProfilesWithAccuracyHeuristic::improve_model_profiles(const unsigned model_index) {
+void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profiles(const unsigned model_index) {
   Array1D<Host, unsigned> criterion_indexes(models.criteria_count, uninitialized);
   // Not worth parallelizing because models.criteria_count is typically small
   for (unsigned crit_idx_idx = 0; crit_idx_idx != models.criteria_count; ++crit_idx_idx) {
     criterion_indexes[crit_idx_idx] = crit_idx_idx;
   }
 
   // Not parallel because iteration N+1 relies on side effect in iteration N
   // (We could challenge this aspect of the algorithm described by Sobrie)
   for (unsigned profile_index = 0; profile_index != models.categories_count - 1; ++profile_index) {
-    shuffle<unsigned>(model_index, ref(criterion_indexes));
+    shuffle(models.urbgs[model_index], ref(criterion_indexes));
     improve_model_profile(model_index, profile_index, criterion_indexes);
   }
 }
 
-void ImproveProfilesWithAccuracyHeuristic::improve_model_profile(
+void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profile(
   const unsigned model_index,
   const unsigned profile_index,
   ArrayView1D<Host, const unsigned> criterion_indexes
 ) {
   // Not parallel because iteration N+1 relies on side effect in iteration N
   // (We could challenge this aspect of the algorithm described by Sobrie)
   for (unsigned crit_idx_idx = 0; crit_idx_idx != models.criteria_count; ++crit_idx_idx) {
     improve_model_profile(model_index, profile_index, criterion_indexes[crit_idx_idx]);
   }
 }
 
-void ImproveProfilesWithAccuracyHeuristic::improve_model_profile(
+void ImproveProfilesWithAccuracyHeuristicOnCpu::improve_model_profile(
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index
 ) {
   // WARNING: We're assuming all criteria have values in [0, 1]
   // @todo Can we relax this assumption?
   // This is consistent with our comment in the header file, but slightly less generic than Sobrie's thesis
@@ -80,47 +81,45 @@
     // but "most existing implementations have a bug where they may occasionally" return it,
     // so we work around that bug by calling it again until it doesn't.
     // Ref: https://en.cppreference.com/w/cpp/numeric/random/uniform_real_distribution
     while (destination == highest_destination) {
       destination = std::uniform_real_distribution<float>(lowest_destination, highest_destination)(models.urbgs[model_index]);
     }
     const float desirability = compute_move_desirability(
-      models, model_index, profile_index, criterion_index, destination).value();
+      model_index, profile_index, criterion_index, destination).value();
     // Single-key reduce (divide and conquer?) (atomic compare-and-swap?)
     if (desirability > best_desirability) {
       best_desirability = desirability;
       best_destination = destination;
     }
   }
 
   // @todo Desirability can be as high as 2. The [0, 1] interval is a weird choice.
   if (std::uniform_real_distribution<float>(0, 1)(models.urbgs[model_index]) <= best_desirability) {
     models.profiles[criterion_index][profile_index][model_index] = best_destination;
   }
 }
 
-ImproveProfilesWithAccuracyHeuristic::Desirability ImproveProfilesWithAccuracyHeuristic::compute_move_desirability(
-  const Models& models,
+Desirability ImproveProfilesWithAccuracyHeuristicOnCpu::compute_move_desirability(
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index,
   const float destination
 ) {
   Desirability d;
 
   for (unsigned alternative_index = 0; alternative_index != models.learning_alternatives_count; ++alternative_index) {
     update_move_desirability(
-      models, model_index, profile_index, criterion_index, destination, alternative_index, &d);
+      model_index, profile_index, criterion_index, destination, alternative_index, &d);
   }
 
   return d;
 }
 
-void ImproveProfilesWithAccuracyHeuristic::update_move_desirability(
-  const Models& models,
+void ImproveProfilesWithAccuracyHeuristicOnCpu::update_move_desirability(
   const unsigned model_index,
   const unsigned profile_index,
   const unsigned criterion_index,
   const float destination,
   const unsigned alternative_index,
   Desirability* desirability
 ) {
@@ -230,16 +229,8 @@
       && destination < value
       && value <= current_position) {
         ++desirability->t;
     }
   }
 }
 
-float ImproveProfilesWithAccuracyHeuristic::Desirability::value() const {
-  if (v + w + t + q + r == 0) {
-    return zero_value;
-  } else {
-    return (2 * v + w + 0.1 * t) / (v + w + t + 5 * q + r);
-  }
-}
-
 }  // namespace lincs
```

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,26 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_HPP
-#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_HPP
+#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
+#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
 
 #include "../../weights-profiles-breed-mrsort.hpp"
+#include "accuracy-heuristic/desirability.hpp"
 
 
 namespace lincs {
 
-class ImproveProfilesWithAccuracyHeuristic : public WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy {
+class ImproveProfilesWithAccuracyHeuristicOnCpu : public WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy {
  public:
-  explicit ImproveProfilesWithAccuracyHeuristic(Models& models_) : models(models_) {}
+  explicit ImproveProfilesWithAccuracyHeuristicOnCpu(Models& models_) : models(models_) {}
 
  public:
   void improve_profiles() override;
 
  private:
-  struct Desirability {
-    // Value for moves with no impact.
-    // @todo Verify with Vincent Mousseau that this is the correct value.
-    static constexpr float zero_value = 0;
-
-    unsigned v = 0;
-    unsigned w = 0;
-    unsigned q = 0;
-    unsigned r = 0;
-    unsigned t = 0;
-
-    float value() const;
-  };
-
   void improve_model_profiles(const unsigned model_index);
 
   void improve_model_profile(
     const unsigned model_index,
     const unsigned profile_index,
     ArrayView1D<Host, const unsigned> criterion_indexes
   );
@@ -41,38 +28,29 @@
   void improve_model_profile(
     const unsigned model_index,
     const unsigned profile_index,
     const unsigned criterion_index
   );
 
   Desirability compute_move_desirability(
-    const Models& models,
     const unsigned model_index,
     const unsigned profile_index,
     const unsigned criterion_index,
     const float destination
   );
 
   void update_move_desirability(
-    const Models& models,
     const unsigned model_index,
     const unsigned profile_index,
     const unsigned criterion_index,
     const float destination,
     const unsigned alternative_index,
     Desirability* desirability
   );
 
-  template<typename T>
-  void shuffle(const unsigned model_index, ArrayView1D<Host, T> m) {
-    for (unsigned i = 0; i != m.s0(); ++i) {
-      std::swap(m[i], m[std::uniform_int_distribution<unsigned int>(0, m.s0() - 1)(models.urbgs[model_index])]);
-    }
-  }
-
  private:
   Models& models;
 };
 
 }  // namespace lincs
 
-#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_HPP
+#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__IMPROVE_PROFILES__ACCURACY_HEURISTIC_ON_CPU_HPP
```

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,28 @@
 // Copyright 2023 Vincent Jacques
 
-#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__OPTIMIZE_WEIGHTS__GLOP_HPP
-#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__OPTIMIZE_WEIGHTS__GLOP_HPP
-
-#include <memory>
+#ifndef LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__OPTIMIZE_WEIGHTS__LINEAR_PROGRAM_HPP
+#define LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__OPTIMIZE_WEIGHTS__LINEAR_PROGRAM_HPP
 
 #include "../../weights-profiles-breed-mrsort.hpp"
 
 
 namespace lincs {
 
-class OptimizeWeightsUsingGlop : public WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy {
+template<typename LinearProgram>
+class OptimizeWeightsUsingLinearProgram : public WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy {
  public:
-  OptimizeWeightsUsingGlop(Models& models_) : models(models_) {}
+  OptimizeWeightsUsingLinearProgram(Models& models_) : models(models_) {}
 
  public:
   void optimize_weights() override;
 
  private:
   void optimize_model_weights(unsigned model_index);
 
-  struct LinearProgram;
-
-  std::shared_ptr<LinearProgram> make_internal_linear_program(const float epsilon, unsigned model_index);
-
-  auto solve_linear_program(std::shared_ptr<LinearProgram> lp);
-
  private:
   Models& models;
 };
 
 }  // namespace lincs
 
-#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__OPTIMIZE_WEIGHTS__GLOP_HPP
+#endif  // LINCS__LEARNING__WEIGHTS_PROFILES_BREED_MRSORT__OPTIMIZE_WEIGHTS__LINEAR_PROGRAM_HPP
```

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 #include <map>
 
 #include "../median-and-max.hpp"
 
 
 namespace lincs {
 
-WeightsProfilesBreedMrSortLearning::Models WeightsProfilesBreedMrSortLearning::Models::make(const Domain& domain, const Alternatives& learning_set, const unsigned models_count, const unsigned random_seed) {
+WeightsProfilesBreedMrSortLearning::Models WeightsProfilesBreedMrSortLearning::Models::make(const Problem& problem, const Alternatives& learning_set, const unsigned models_count, const unsigned random_seed) {
   std::map<std::string, unsigned> category_indexes;
-  for (const auto& category: domain.categories) {
+  for (const auto& category: problem.categories) {
     category_indexes[category.name] = category_indexes.size();
   }
 
-  const unsigned criteria_count = domain.criteria.size();
-  const unsigned categories_count = domain.categories.size();
+  const unsigned criteria_count = problem.criteria.size();
+  const unsigned categories_count = problem.categories.size();
   const unsigned alternatives_count = learning_set.alternatives.size();
 
   Array2D<Host, float> alternatives(criteria_count, alternatives_count, uninitialized);
   Array1D<Host, unsigned> assignments(alternatives_count, uninitialized);
 
   for (unsigned alternative_index = 0; alternative_index != alternatives_count; ++alternative_index) {
     const Alternative& alt = learning_set.alternatives[alternative_index];
@@ -37,15 +37,15 @@
 
   std::vector<std::mt19937> urbgs(models_count);
   for (unsigned model_index = 0; model_index != models_count; ++model_index) {
     urbgs[model_index].seed(random_seed * (model_index + 1));
   }
 
   return {
-    domain,
+    problem,
     categories_count,
     criteria_count,
     alternatives_count,
     std::move(alternatives),
     std::move(assignments),
     models_count,
     std::move(weights),
@@ -71,15 +71,15 @@
     boundary_profile.reserve(criteria_count);
     for (unsigned criterion_index = 0; criterion_index != criteria_count; ++criterion_index) {
       boundary_profile.push_back(profiles[criterion_index][cat_index][model_index]);
     }
     boundaries.emplace_back(boundary_profile, coalitions);
   }
 
-  return Model{domain, boundaries};
+  return Model{problem, boundaries};
 }
 
 Model WeightsProfilesBreedMrSortLearning::perform() {
   std::vector<unsigned> model_indexes(models.models_count, 0);
   std::iota(model_indexes.begin(), model_indexes.end(), 0);
   profiles_initialization_strategy.initialize_profiles(model_indexes.begin(), model_indexes.end());
```

### Comparing `lincs-0.3.7/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp` & `lincs-0.4.0/lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp`

 * *Files 3% similar despite different names*

```diff
@@ -52,26 +52,26 @@
   ProfilesInitializationStrategy& profiles_initialization_strategy;
   WeightsOptimizationStrategy& weights_optimization_strategy;
   ProfilesImprovementStrategy& profiles_improvement_strategy;
   TerminationStrategy& termination_strategy;
 };
 
 struct WeightsProfilesBreedMrSortLearning::Models {
-  const Domain& domain;
+  const Problem& problem;
   unsigned categories_count;
   unsigned criteria_count;
   unsigned learning_alternatives_count;
   Array2D<Host, float> learning_alternatives;
   Array1D<Host, unsigned> learning_assignments;
   unsigned models_count;
   Array2D<Host, float> weights;
   Array3D<Host, float> profiles;
   std::vector<std::mt19937> urbgs;
 
-  static Models make(const Domain& domain, const Alternatives& learning_set, const unsigned models_count, const unsigned random_seed);
+  static Models make(const Problem& problem, const Alternatives& learning_set, const unsigned models_count, const unsigned random_seed);
 
   Model get_model(const unsigned model_index) const;
 };
 
 struct WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy {
   typedef WeightsProfilesBreedMrSortLearning::Models Models;
```

### Comparing `lincs-0.3.7/lincs/liblincs/liblincs_module.cpp` & `lincs-0.4.0/lincs/liblincs/liblincs_module.cpp`

 * *Files 8% similar despite different names*

```diff
@@ -31,17 +31,17 @@
     return n;
   }
 
   private:
   bp::object out_file;
 };
 
-void dump_domain(const lincs::Domain& domain, bp::object& out_file) {
+void dump_problem(const lincs::Problem& problem, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
-  domain.dump(out_stream);
+  problem.dump(out_stream);
 }
 
 void dump_model(const lincs::Model& model, bp::object& out_file) {
   boost::iostreams::stream<PythonOutputDevice> out_stream(out_file);
   model.dump(out_stream);
 }
 
@@ -61,27 +61,27 @@
     return str.size();
   }
 
   private:
   bp::object in_file;
 };
 
-lincs::Domain load_domain(bp::object& in_file) {
+lincs::Problem load_problem(bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
-  return lincs::Domain::load(in_stream);
+  return lincs::Problem::load(in_stream);
 }
 
-lincs::Model load_model(const lincs::Domain& domain, bp::object& in_file) {
+lincs::Model load_model(const lincs::Problem& problem, bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
-  return lincs::Model::load(domain, in_stream);
+  return lincs::Model::load(problem, in_stream);
 }
 
-lincs::Alternatives load_alternatives(const lincs::Domain& domain, bp::object& in_file) {
+lincs::Alternatives load_alternatives(const lincs::Problem& problem, bp::object& in_file) {
   boost::iostreams::stream<PythonInputDevice> in_stream(in_file);
-  return lincs::Alternatives::load(domain, in_stream);
+  return lincs::Alternatives::load(problem, in_stream);
 }
 
 // @todo Thoroughly review all conversions between Python and C++ types.
 // - read Boost.Python doc in details and understand the contract
 // - homogenize converters (some were copy-pasted from SO answers and even ChatGPT)
 // - double-check if/when we need to increment reference counts on Python objects
 // https://stackoverflow.com/a/15940413/905845
@@ -127,15 +127,15 @@
       return bp::incref(bp::object().ptr());
     }
   }
 
   static void* convertible(PyObject* obj) {
     if (obj == Py_None) {
       return new std::optional<T>();
-    } else if (PyNumber_Check(obj)) {
+    } else if (PyNumber_Check(obj) || PyUnicode_Check(obj)) {
       return new std::optional<T>(bp::extract<T>(obj));
     } else {
       return nullptr;
     }
   }
 
   static void construct(PyObject* obj, bp::converter::rvalue_from_python_stage1_data* data) {
@@ -151,21 +151,36 @@
       &std_optional_converter<T>::construct,
       bp::type_id<std::optional<T>>()
     );
   }
 };
 
 lincs::WeightsProfilesBreedMrSortLearning::Models* make_models(
-  const lincs::Domain& domain,
+  const lincs::Problem& problem,
   const lincs::Alternatives& learning_set,
   const unsigned models_count,
   const unsigned random_seed
 ) {
   return new lincs::WeightsProfilesBreedMrSortLearning::Models(std::move(
-    lincs::WeightsProfilesBreedMrSortLearning::Models::make(domain, learning_set, models_count, random_seed)));
+    lincs::WeightsProfilesBreedMrSortLearning::Models::make(problem, learning_set, models_count, random_seed)));
+}
+
+lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels* make_gpu_models(
+  const lincs::WeightsProfilesBreedMrSortLearning::Models& models
+) {
+  return new lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels(std::move(
+    lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels::make(models)));
+}
+
+std::optional<std::string> get_alternative_category(const lincs::Alternative& alt) {
+  return alt.category;
+}
+
+void set_alternative_category(lincs::Alternative& alt, std::optional<std::string> category) {
+  alt.category = category;
 }
 
 }  // namespace
 
 template <typename T>
 void auto_enum(const std::string& name) {
   auto e = bp::enum_<T>(name.c_str());
@@ -173,66 +188,67 @@
     e.value(std::string(magic_enum::enum_name(value)).c_str(), value);
   }
 }
 
 BOOST_PYTHON_MODULE(liblincs) {
   iterable_converter()
     .from_python<std::vector<float>>()
-    .from_python<std::vector<lincs::Domain::Category>>()
-    .from_python<std::vector<lincs::Domain::Criterion>>()
+    .from_python<std::vector<lincs::Problem::Category>>()
+    .from_python<std::vector<lincs::Problem::Criterion>>()
     .from_python<std::vector<lincs::Model::Boundary>>()
     .from_python<std::vector<lincs::Model::SufficientCoalitions>>()
     .from_python<std::vector<lincs::Alternative>>()
   ;
 
   std_optional_converter<float>::enroll();
+  std_optional_converter<std::string>::enroll();
 
   // @todo Decide wether we nest types or not, use the same nesting in Python and C++
-  auto_enum<lincs::Domain::Criterion::ValueType>("ValueType");
-  auto_enum<lincs::Domain::Criterion::CategoryCorrelation>("CategoryCorrelation");
+  auto_enum<lincs::Problem::Criterion::ValueType>("ValueType");
+  auto_enum<lincs::Problem::Criterion::CategoryCorrelation>("CategoryCorrelation");
   auto_enum<lincs::Model::SufficientCoalitions::Kind>("SufficientCoalitionsKind");
 
-  bp::class_<lincs::Domain::Criterion>("Criterion", bp::init<std::string, lincs::Domain::Criterion::ValueType, lincs::Domain::Criterion::CategoryCorrelation>())
-    .def_readwrite("name", &lincs::Domain::Criterion::name)
-    .def_readwrite("value_type", &lincs::Domain::Criterion::value_type)
-    .def_readwrite("category_correlation", &lincs::Domain::Criterion::category_correlation)
+  bp::class_<lincs::Problem::Criterion>("Criterion", bp::init<std::string, lincs::Problem::Criterion::ValueType, lincs::Problem::Criterion::CategoryCorrelation>())
+    .def_readwrite("name", &lincs::Problem::Criterion::name)
+    .def_readwrite("value_type", &lincs::Problem::Criterion::value_type)
+    .def_readwrite("category_correlation", &lincs::Problem::Criterion::category_correlation)
   ;
 
-  bp::class_<lincs::Domain::Category>("Category", bp::init<std::string>())
-    .def_readwrite("name", &lincs::Domain::Category::name)
+  bp::class_<lincs::Problem::Category>("Category", bp::init<std::string>())
+    .def_readwrite("name", &lincs::Problem::Category::name)
   ;
 
-  bp::class_<std::vector<lincs::Domain::Category>>("categories_vector")
-    .def(bp::vector_indexing_suite<std::vector<lincs::Domain::Category>>())
+  bp::class_<std::vector<lincs::Problem::Category>>("categories_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Problem::Category>>())
   ;
-  bp::class_<std::vector<lincs::Domain::Criterion>>("criteria_vector")
-    .def(bp::vector_indexing_suite<std::vector<lincs::Domain::Criterion>>())
+  bp::class_<std::vector<lincs::Problem::Criterion>>("criteria_vector")
+    .def(bp::vector_indexing_suite<std::vector<lincs::Problem::Criterion>>())
   ;
-  bp::class_<lincs::Domain>("Domain", bp::init<std::vector<lincs::Domain::Criterion>, std::vector<lincs::Domain::Category>>())
-    .def_readwrite("criteria", &lincs::Domain::criteria)
-    .def_readwrite("categories", &lincs::Domain::categories)
+  bp::class_<lincs::Problem>("Problem", bp::init<std::vector<lincs::Problem::Criterion>, std::vector<lincs::Problem::Category>>())
+    .def_readwrite("criteria", &lincs::Problem::criteria)
+    .def_readwrite("categories", &lincs::Problem::categories)
     .def(
       "dump",
-      &dump_domain,
+      &dump_problem,
       (bp::arg("self"), "out"),
-      "Dump the domain to the provided `.write()`-supporting file-like object, in YAML format."
+      "Dump the problem to the provided `.write()`-supporting file-like object, in YAML format."
     )
   ;
   // @todo Make these 'staticmethod's of Alternatives. Same for other load and generate functions.
   bp::def(
-    "load_domain",
-    &load_domain,
+    "load_problem",
+    &load_problem,
     (bp::arg("in")),
-    "Load a domain from the provided `.read()`-supporting file-like object, in YAML format."
+    "Load a problem from the provided `.read()`-supporting file-like object, in YAML format."
   );
   bp::def(
-    "generate_domain",
-    &lincs::generate_domain,
+    "generate_problem",
+    &lincs::generate_problem,
     (bp::arg("criteria_count"), "categories_count", "random_seed"),
-    "Generate a domain with `criteria_count` criteria and `categories_count` categories."
+    "Generate a problem with `criteria_count` criteria and `categories_count` categories."
   );
 
   bp::class_<lincs::Model::SufficientCoalitions>("SufficientCoalitions", bp::init<lincs::Model::SufficientCoalitions::Kind, std::vector<float>>())
     .def_readwrite("kind", &lincs::Model::SufficientCoalitions::kind)
     .def_readwrite("criterion_weights", &lincs::Model::SufficientCoalitions::criterion_weights)
   ;
 
@@ -242,74 +258,79 @@
   bp::class_<lincs::Model::Boundary>("Boundary", bp::init<std::vector<float>, lincs::Model::SufficientCoalitions>())
     .def_readwrite("profile", &lincs::Model::Boundary::profile)
     .def_readwrite("sufficient_coalitions", &lincs::Model::Boundary::sufficient_coalitions)
   ;
   bp::class_<std::vector<lincs::Model::Boundary>>("boundaries_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Model::Boundary>>())
   ;
-  bp::class_<lincs::Model>("Model", bp::init<const lincs::Domain&, const std::vector<lincs::Model::Boundary>&>())
+  bp::class_<lincs::Model>("Model", bp::init<const lincs::Problem&, const std::vector<lincs::Model::Boundary>&>())
     .def_readwrite("boundaries", &lincs::Model::boundaries)
     .def(
       "dump",
       &dump_model,
       (bp::arg("self"), "out"),
       "Dump the model to the provided `.write()`-supporting file-like object, in YAML format."
     )
   ;
   bp::def(
     "load_model",
     &load_model,
-    (bp::arg("domain"), "in"),
-    "Load a model for the provided `domain`, from the provided `.read()`-supporting file-like object, in YAML format."
+    (bp::arg("problem"), "in"),
+    "Load a model for the provided `problem`, from the provided `.read()`-supporting file-like object, in YAML format."
   );
   bp::def(
     "generate_mrsort_model",
     &lincs::generate_mrsort_model,
-    (bp::arg("domain"), "random_seed", bp::arg("fixed_weights_sum")=std::optional<float>()),
-    "Generate an MR-Sort model for the provided `domain`."
+    (bp::arg("problem"), "random_seed", bp::arg("fixed_weights_sum")=std::optional<float>()),
+    "Generate an MR-Sort model for the provided `problem`."
   );
 
-  bp::class_<lincs::Alternative>("Alternative", bp::init<std::string, std::vector<float>, std::string>())
+  bp::class_<lincs::Alternative>(
+    "Alternative",
+    bp::init<std::string, std::vector<float>, std::optional<std::string>>(
+      (bp::arg("name"), "profile", (bp::arg("category")=std::optional<std::string>()))
+    )
+  )
     .def_readwrite("name", &lincs::Alternative::name)
     .def_readwrite("profile", &lincs::Alternative::profile)
-    .def_readwrite("category", &lincs::Alternative::category)
+    .add_property("category", &get_alternative_category, &set_alternative_category)
   ;
   bp::class_<std::vector<lincs::Alternative>>("alternatives_vector")
     .def(bp::vector_indexing_suite<std::vector<lincs::Alternative>>())
   ;
-  bp::class_<lincs::Alternatives>("Alternatives", bp::init<const lincs::Domain&, const std::vector<lincs::Alternative>&>())
+  bp::class_<lincs::Alternatives>("Alternatives", bp::init<const lincs::Problem&, const std::vector<lincs::Alternative>&>())
     .def_readwrite("alternatives", &lincs::Alternatives::alternatives)
     .def(
       "dump",
       &dump_alternatives,
       (bp::arg("self"), "out"),
       "Dump the set of alternatives to the provided `.write()`-supporting file-like object, in CSV format."
     )
   ;
   bp::def(
     "load_alternatives",
     &load_alternatives,
-    (bp::arg("domain"), "in"),
+    (bp::arg("problem"), "in"),
     "Load a set of alternatives (classified or not) from the provided `.read()`-supporting file-like object, in CSV format."
   );
   bp::def(
     "generate_alternatives",
     &lincs::generate_alternatives,
-    (bp::arg("domain"), "model", "alternatives_count", "random_seed", bp::arg("max_imbalance")=std::optional<float>()),
-    "Generate a set of `alternatives_count` pseudo-random alternatives for the provided `domain`, classified according to the provided `model`."
+    (bp::arg("problem"), "model", "alternatives_count", "random_seed", bp::arg("max_imbalance")=std::optional<float>()),
+    "Generate a set of `alternatives_count` pseudo-random alternatives for the provided `problem`, classified according to the provided `model`."
   );
 
   bp::class_<lincs::ClassificationResult>("ClassificationResult", bp::no_init)
     .def_readonly("changed", &lincs::ClassificationResult::changed)
     .def_readonly("unchanged", &lincs::ClassificationResult::unchanged)
   ;
   bp::def(
     "classify_alternatives",
     &lincs::classify_alternatives,
-    (bp::arg("domain"), "model", "alternatives"),
+    (bp::arg("problem"), "model", "alternatives"),
     "Classify the provided `alternatives` according to the provided `model`."
   );
 
   bp::class_<lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy, boost::noncopyable>("ProfilesInitializationStrategy", bp::no_init)
     .def("initialize_profiles", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy::initialize_profiles));
 
   bp::class_<
@@ -329,42 +350,62 @@
     bp::bases<lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy>
   >(
     "OptimizeWeightsUsingGlop",
     bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
   )
     .def("optimize_weights", &lincs::OptimizeWeightsUsingGlop::optimize_weights);
 
+  bp::class_<
+    lincs::OptimizeWeightsUsingAlglib,
+    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy>
+  >(
+    "OptimizeWeightsUsingAlglib",
+    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
+  )
+    .def("optimize_weights", &lincs::OptimizeWeightsUsingAlglib::optimize_weights);
+
   bp::class_<lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy, boost::noncopyable>("ProfilesImprovementStrategy", bp::no_init)
     .def("improve_profiles", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy::improve_profiles));
 
   bp::class_<
-    lincs::ImproveProfilesWithAccuracyHeuristic,
+    lincs::ImproveProfilesWithAccuracyHeuristicOnCpu,
     bp::bases<lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy>
   >(
-    "ImproveProfilesWithAccuracyHeuristic",
+    "ImproveProfilesWithAccuracyHeuristicOnCpu",
     bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&>()
   )
-    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristic::improve_profiles);
+    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnCpu::improve_profiles);
+
+  bp::class_<
+    lincs::ImproveProfilesWithAccuracyHeuristicOnGpu,
+    bp::bases<lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy>
+  >(
+    "ImproveProfilesWithAccuracyHeuristicOnGpu",
+    bp::init<lincs::WeightsProfilesBreedMrSortLearning::Models&, lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels&>()
+  )
+    .def("improve_profiles", &lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::improve_profiles);
 
   struct TerminationStrategyWrap : lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy, bp::wrapper<lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy> {
     bool terminate(unsigned iteration_index, unsigned best_accuracy) override {
       return this->get_override("terminate")(iteration_index, best_accuracy);
     }
   };
 
   bp::class_<TerminationStrategyWrap, boost::noncopyable>("TerminationStrategy")
     .def("terminate", bp::pure_virtual(&lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy::terminate));
 
   bp::class_<lincs::TerminateAtAccuracy, bp::bases<lincs::WeightsProfilesBreedMrSortLearning::TerminationStrategy>>("TerminateAtAccuracy", bp::init<unsigned>())
     .def("terminate", &lincs::TerminateAtAccuracy::terminate);
 
   bp::class_<lincs::WeightsProfilesBreedMrSortLearning::Models, boost::noncopyable>("Models", bp::no_init);
-
   bp::def("make_models", &make_models, bp::return_value_policy<bp::manage_new_object>());
 
+  bp::class_<lincs::ImproveProfilesWithAccuracyHeuristicOnGpu::GpuModels, boost::noncopyable>("GpuModels", bp::no_init);
+  bp::def("make_gpu_models", &make_gpu_models, bp::return_value_policy<bp::manage_new_object>());
+
   bp::class_<lincs::WeightsProfilesBreedMrSortLearning>(
     "WeightsProfilesBreedMrSortLearning",
     bp::init<
       lincs::WeightsProfilesBreedMrSortLearning::Models&,
       lincs::WeightsProfilesBreedMrSortLearning::ProfilesInitializationStrategy&,
       lincs::WeightsProfilesBreedMrSortLearning::WeightsOptimizationStrategy&,
       lincs::WeightsProfilesBreedMrSortLearning::ProfilesImprovementStrategy&,
```

### Comparing `lincs-0.3.7/lincs/liblincs/median-and-max.cpp` & `lincs-0.4.0/lincs/liblincs/median-and-max.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/lincs/liblincs/median-and-max.hpp` & `lincs-0.4.0/lincs/liblincs/median-and-max.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/lincs/liblincs/randomness-utils.cpp` & `lincs-0.4.0/lincs/liblincs/randomness-utils.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.3.7/lincs/liblincs/randomness-utils.hpp` & `lincs-0.4.0/lincs/liblincs/randomness-utils.hpp`

 * *Files 5% similar despite different names*

```diff
@@ -48,8 +48,15 @@
   }
 
  private:
   std::vector<T> values;
   mutable std::discrete_distribution<unsigned> distribution;
 };
 
+template<typename T>
+void shuffle(std::mt19937& urbg, T m) {
+  for (unsigned i = 0; i != m.s0(); ++i) {
+    std::swap(m[i], m[std::uniform_int_distribution<unsigned>(0, m.s0() - 1)(urbg)]);
+  }
+}
+
 #endif  // LINCS__RANDOMNESS_UTILS_HPP
```

### Comparing `lincs-0.3.7/lincs.egg-info/PKG-INFO` & `lincs-0.4.0/lincs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.3.7
+Version: 0.4.0
 Summary: Learn and Infer Non Compensatory Sortings
 Home-page: https://github.com/MICS-Lab/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 License: LGPLv3
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
@@ -23,24 +23,24 @@
 
 .. WARNING, this README is rendered to HTML in several places
     - on GitHub (https://github.com/mics-lab/lincs/)
     - on PyPI after publication of the package (https://pypi.org/project/lincs/)
     - on GitHub Pages (https://mics-lab.github.io/lincs/)
     So when you change it, take care to check all those places.
 
-*lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
-
-*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.3.7/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.3.7/COPYING.LESSER>`_.
-It's available on the `Python package index <https://pypi.org/project/lincs/>`_.
-Its `documentation <http://mics-lab.github.io/lincs/>`_
-and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+*lincs* (Learn and Infer Non Compensatory Sortings) is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
+*lincs* is licensed under the GNU Lesser General Public License v3.0 as indicated by the two files `COPYING <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING>`_ and `COPYING.LESSER <https://github.com/MICS-Lab/lincs/blob/v0.4.0/COPYING.LESSER>`_.
 
 @todo (When we have a paper to actually cite) Add a note asking academics to kindly cite our work.
 
+*lincs* is available for install from the `Python package index <https://pypi.org/project/lincs/>`_.
+Its `documentation <http://mics-lab.github.io/lincs/>`_
+and its `source code <https://github.com/mics-lab/lincs/>`_ are on GitHub.
+
 Questions? Remarks? Bugs? Want to contribute? Open `an issue <https://github.com/MICS-Lab/lincs/issues>`_ or `a discussion <https://github.com/MICS-Lab/lincs/discussions>`_!
 
 
 Contributors and previous work
 ==============================
 
 *lincs* is developed by the `MICS <https://mics.centralesupelec.fr/>`_ research team at `CentraleSupélec <https://www.centralesupelec.fr/>`_.
@@ -53,39 +53,43 @@
 - `Wassila Ouerdane <https://wassilaouerdane.github.io/>`_ (domain expertise)
 
 It's based on work by:
 
 - `Olivier Sobrie <http://olivier.sobrie.be/>`_ (The "weights, profiles, breed" learning strategy for MR-Sort models, and the profiles improvement heuristic, developed in his `Ph.D thesis <http://olivier.sobrie.be/papers/phd_2016_sobrie.pdf>`_, and `implemented in Python <https://github.com/oso/pymcda>`_)
 - Emma Dixneuf, Thibault Monsel and Thomas Vindard (`C++ implementation of Sobrie's heuristic <https://github.com/Mostah/fastPL/>`_)
 
+@todo Add links to the fundamental articles for NCS.
+@todo Add links to the articles that define other learning methods we re-implement.
 
 Project goals
 =============
 
 Provide MCDA tools usable out of the box
 ----------------------------------------
 
 You should be able to use *lincs* without being a specialist of MCDA and/or NCS models.
 Just follow the `Get started <#get-started>`_ section below.
 
 Provide a base for developing new MCDA algorithms
 -------------------------------------------------
 
 *lincs* is designed to be easy to extend with new algorithms of even replace parts of existing algorithms.
-@todo Write doc about that use case.
+See our `contributor guide <https://mics-lab.github.io/lincs/contributor-guide.html>`_ for more details.
 
-*lincs* also provides a benchmark framework to compare algorithms (@todo Write and document).
+*lincs* also provides a benchmark framework to compare algorithms (@todo Implement and document).
 This should make it easier to understand the relative strengths and weaknesses of each algorithm.
 
 
 Get started
 ===========
 
 Depending on your favorite approach, you can either start with our `hands-on "Get started" guide <https://mics-lab.github.io/lincs/get-started.html>`_
 or with our `conceptual overview documentation <https://mics-lab.github.io/lincs/conceptual-overview.html>`_.
+The former will show you how to use our tools, the latter will explain the concepts behind them: what's MCDA, what are NCS models, *etc.*
+If in doubt, start with the conceptual overview.
 We highly recommend you read the other one just after.
 
 Once you've used *lincs* a bit, you can follow up with our `user guide <https://mics-lab.github.io/lincs/user-guide.html>`_
 and `reference documentation <https://mics-lab.github.io/lincs/reference.html>`_.
 
 
 Develop *lincs* itself
```

### Comparing `lincs-0.3.7/lincs.egg-info/SOURCES.txt` & `lincs-0.4.0/lincs.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -27,21 +27,29 @@
 lincs/liblincs/lincs.hpp
 lincs/liblincs/median-and-max.cpp
 lincs/liblincs/median-and-max.hpp
 lincs/liblincs/randomness-utils.cpp
 lincs/liblincs/randomness-utils.hpp
 lincs/liblincs/io/alternatives.cpp
 lincs/liblincs/io/alternatives.hpp
-lincs/liblincs/io/domain.cpp
-lincs/liblincs/io/domain.hpp
 lincs/liblincs/io/model.cpp
 lincs/liblincs/io/model.hpp
+lincs/liblincs/io/problem.cpp
+lincs/liblincs/io/problem.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort.cpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort.hpp
-lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.cpp
-lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic.hpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.cpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-cpu.hpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.cu
+lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic-on-gpu.hpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/improve-profiles/accuracy-heuristic/desirability.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.cpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/initialize-profiles/probabilistic-maximal-discrimination-power-per-criterion.hpp
-lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.cpp
-lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/glop.hpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.cpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/optimize-weights/linear-program.hpp
 lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.cpp
-lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+lincs/liblincs/learning/weights-profiles-breed-mrsort/terminate/at-accuracy.hpp
+lincs/liblincs/linear-programming/alglib.cpp
+lincs/liblincs/linear-programming/alglib.hpp
+lincs/liblincs/linear-programming/glop.cpp
+lincs/liblincs/linear-programming/glop.hpp
+lincs/liblincs/linear-programming/test.cpp
```

