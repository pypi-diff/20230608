# Comparing `tmp/seaflowpy-7.0.0.tar.gz` & `tmp/seaflowpy-7.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaflowpy-7.0.0.tar", last modified: Wed Jun  7 22:49:11 2023, max compression
+gzip compressed data, was "seaflowpy-7.1.0.tar", last modified: Thu Jun  8 19:20:49 2023, max compression
```

## Comparing `seaflowpy-7.0.0.tar` & `seaflowpy-7.1.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/
--rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-7.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-7.0.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6771 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-7.0.0/README.md
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-7.0.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.809349 seaflowpy-7.0.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/src/seaflowpy/
--rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-7.0.0/src/seaflowpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/src/seaflowpy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.823349 seaflowpy-7.0.0/src/seaflowpy/cli/
--rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-7.0.0/src/seaflowpy/cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.829349 seaflowpy-7.0.0/src/seaflowpy/cli/commands/
--rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/dayofyear_cmd.py
--rw-r--r--   0 root         (0) root         (0)     5751 2023-06-06 18:39:22.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/db_cmd.py
--rw-r--r--   0 root         (0) root         (0)    13795 2023-06-07 22:00:45.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/evt_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/filter_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/opp_cmd.py
--rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/version_cmd.py
--rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-7.0.0/src/seaflowpy/cloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.829349 seaflowpy-7.0.0/src/seaflowpy/data/
--rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-7.0.0/src/seaflowpy/data/popcycle.sql
--rw-r--r--   0 root         (0) root         (0)    13751 2023-06-06 18:37:53.000000 seaflowpy-7.0.0/src/seaflowpy/db.py
--rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-7.0.0/src/seaflowpy/errors.py
--rw-r--r--   0 root         (0) root         (0)    14404 2023-06-07 21:58:24.000000 seaflowpy-7.0.0/src/seaflowpy/fileio.py
--rw-r--r--   0 root         (0) root         (0)    13774 2023-06-07 19:22:50.000000 seaflowpy-7.0.0/src/seaflowpy/filterevt.py
--rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/geo.py
--rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-7.0.0/src/seaflowpy/particleops.py
--rw-r--r--   0 root         (0) root         (0)    10272 2023-06-07 19:22:28.000000 seaflowpy-7.0.0/src/seaflowpy/sample.py
--rw-r--r--   0 root         (0) root         (0)     9547 2023-06-07 20:00:45.000000 seaflowpy-7.0.0/src/seaflowpy/seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-7.0.0/src/seaflowpy/sfl.py
--rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-7.0.0/src/seaflowpy/time.py
--rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-7.0.0/src/seaflowpy/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.823349 seaflowpy-7.0.0/src/seaflowpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6771 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.835349 seaflowpy-7.0.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-7.0.0/tests/file_dates.parquet
--rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-7.0.0/tests/sfl.parquet
--rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-7.0.0/tests/test_evtopp.py
--rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-7.0.0/tests/test_geo.py
--rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-7.0.0/tests/test_sample.py
--rw-r--r--   0 root         (0) root         (0)    19659 2023-06-07 20:55:05.000000 seaflowpy-7.0.0/tests/test_seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-7.0.0/tests/test_time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.810349 seaflowpy-7.0.0/tests/testcruise_evt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.847349 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.811349 seaflowpy-7.0.0/tests/testcruise_evt_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.854349 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
--rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-7.0.0/tests/testcruise_full_one_param.db
--rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-7.0.0/tests/testcruise_full_plan.db
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.855349 seaflowpy-7.0.0/tests/testcruise_opp_one_param/
--rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.855349 seaflowpy-7.0.0/tests/testcruise_opp_plan/
--rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-7.0.0/tests/testcruise_paramsonly_one_param.db
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-7.0.0/tests/testcruise_paramsonly_plan.db
--rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-7.0.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.866804 seaflowpy-7.1.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-7.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-7.1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-06-08 19:20:49.866804 seaflowpy-7.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-7.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-08 19:20:49.867803 seaflowpy-7.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-7.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.836804 seaflowpy-7.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.867803 seaflowpy-7.1.0/src/seaflowpy/
+-rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-7.1.0/src/seaflowpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-08 19:20:49.867803 seaflowpy-7.1.0/src/seaflowpy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.847803 seaflowpy-7.1.0/src/seaflowpy/cli/
+-rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-7.1.0/src/seaflowpy/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-7.1.0/src/seaflowpy/cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.849804 seaflowpy-7.1.0/src/seaflowpy/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/dayofyear_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     5751 2023-06-06 18:39:22.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/db_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    19147 2023-06-08 19:10:43.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/evt_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/filter_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/opp_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-7.1.0/src/seaflowpy/cli/commands/version_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-7.1.0/src/seaflowpy/cloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.849804 seaflowpy-7.1.0/src/seaflowpy/data/
+-rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-7.1.0/src/seaflowpy/data/popcycle.sql
+-rw-r--r--   0 root         (0) root         (0)    13751 2023-06-08 19:09:37.000000 seaflowpy-7.1.0/src/seaflowpy/db.py
+-rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-7.1.0/src/seaflowpy/errors.py
+-rw-r--r--   0 root         (0) root         (0)    15257 2023-06-08 17:44:08.000000 seaflowpy-7.1.0/src/seaflowpy/fileio.py
+-rw-r--r--   0 root         (0) root         (0)    13774 2023-06-07 19:22:50.000000 seaflowpy-7.1.0/src/seaflowpy/filterevt.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-7.1.0/src/seaflowpy/geo.py
+-rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-7.1.0/src/seaflowpy/particleops.py
+-rw-r--r--   0 root         (0) root         (0)    10272 2023-06-07 19:22:28.000000 seaflowpy-7.1.0/src/seaflowpy/sample.py
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-06-07 20:00:45.000000 seaflowpy-7.1.0/src/seaflowpy/seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-7.1.0/src/seaflowpy/sfl.py
+-rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-7.1.0/src/seaflowpy/time.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-7.1.0/src/seaflowpy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.846804 seaflowpy-7.1.0/src/seaflowpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 19:20:49.000000 seaflowpy-7.1.0/src/seaflowpy.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.852804 seaflowpy-7.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-7.1.0/tests/file_dates.parquet
+-rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-7.1.0/tests/sfl.parquet
+-rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-7.1.0/tests/test_evtopp.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-7.1.0/tests/test_geo.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-7.1.0/tests/test_sample.py
+-rw-r--r--   0 root         (0) root         (0)    19659 2023-06-07 20:55:05.000000 seaflowpy-7.1.0/tests/test_seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-7.1.0/tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.838803 seaflowpy-7.1.0/tests/testcruise_evt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.857803 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.838803 seaflowpy-7.1.0/tests/testcruise_evt_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.863803 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-7.1.0/tests/testcruise_full_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-7.1.0/tests/testcruise_full_plan.db
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.864803 seaflowpy-7.1.0/tests/testcruise_opp_one_param/
+-rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-7.1.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-7.1.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 19:20:49.865804 seaflowpy-7.1.0/tests/testcruise_opp_plan/
+-rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-7.1.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-7.1.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-7.1.0/tests/testcruise_paramsonly_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-7.1.0/tests/testcruise_paramsonly_plan.db
+-rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-7.1.0/versioneer.py
```

### Comparing `seaflowpy-7.0.0/LICENSE` & `seaflowpy-7.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/PKG-INFO` & `seaflowpy-7.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 7.0.0
+Version: 7.1.0
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `seaflowpy-7.0.0/README.md` & `seaflowpy-7.1.0/README.md`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/setup.py` & `seaflowpy-7.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/cli.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/dayofyear_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/dayofyear_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/db_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/db_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/evt_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/evt_cmd.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import datetime
 import logging
 import os
 import pathlib
 import sys
-from joblib import Parallel, delayed
+from functools import partial
 
 import click
+import pandas as pd
+from joblib import Parallel, delayed
 from seaflowpy import errors
 from seaflowpy import seaflowfile
 from seaflowpy import fileio
 from seaflowpy import sample
 from seaflowpy import sfl
 from seaflowpy import time
 
 
+
 def validate_file_fraction(ctx, param, value):
     if value <= 0 or value > 1:
         raise click.BadParameter('must be a number > 0 and <= 1.')
     return value
 
 
 def validate_positive(ctx, param, value):
@@ -242,112 +245,254 @@
     if len(evt):
         print(f"{evt.date.min().isoformat()} {evt.date.max().isoformat()}")
 
 
 @evt_cmd.command('validate')
 @click.option('-a', '--all', 'report_all', is_flag=True,
     help='Show information for all files. If not specified then only files errors are printed.')
-@click.argument('files', nargs=-1, type=click.Path(exists=True))
-def validate_evt_cmd(report_all, files):
+@click.option('--hash', 'hash_', is_flag=True,
+    help='Hash the contents of each EVT with joblib.hash()')
+@click.option('-n', '--n-jobs', default=1, type=int, help='worker jobs')
+@click.option('-r', '--reduced-columns', is_flag=True,
+    help=f'Hash on the reduced column set {fileio.REDUCED_COLS}')
+@click.option('-p', '--progress', is_flag=True,
+    help='Print progress')
+@click.argument('paths', nargs=-1, type=click.Path(exists=True))
+def validate_evt_cmd(report_all, hash_, n_jobs, reduced_columns, progress, paths):
     """
     Examines EVT files.
 
     If any of the file arguments are directories all EVT files within those
     directories will be recursively found and examined. Prints file validation
     report to STDOUT. Print summary of files passing validation to STDERR.
     """
-    # TODO: expand to calculate hash for binary EVT
-    # and OPP parquet files with an extra flag. OPP parquet should produce hashes for
-    # each file_id in the whole file (e.g. by group_by)
-    if not files:
+    if not paths:
         return
 
-    # dirs to file paths
-    files = expand_file_list(files)
+    if reduced_columns:
+        cols = fileio.REDUCED_COLS
+    else:
+        cols = None
 
-    header_printed = False
-    ok, bad = 0, 0
+    # dirs to file paths
+    files = expand_file_list(paths)
 
+    file_ids = []
     for filepath in files:
-        # Default values
-        version = '-'
-        file_id = '-'
-        events = 0
-
         # Try to parse filename as SeaFlow file
         try:
             sff = seaflowfile.SeaFlowFile(filepath)
-            file_id = sff.file_id
         except errors.FileError:
             # unusual name, no file_id
-            pass
+            file_ids.append('-')
+        else:
+            file_ids.append(sff.file_id)
+    work = pd.DataFrame({'id': file_ids, 'path': files})
+    if progress:
+        verbose = 1
+    else:
+        verbose = 0
+    parallel = Parallel(n_jobs=n_jobs, verbose=verbose)
+    work_func = partial(_validate_evt_file, checksum=hash_, cols=cols)
+    results = pd.DataFrame(parallel(delayed(work_func)(r[1]) for r in work.iterrows()))
+    results.sort_values(by='id', key=_idkey, inplace=True)
+
+    if len(results):
+        print(
+            '%d/%d files passed validation' % (results['err'].isna().sum(), len(results)),
+            file=sys.stderr
+        )
+    if report_all:
+        results_output = results
+    else:
+        results_output = results.loc[results['err'] == '']
 
-        # Try to read file as binary EVT
+    if len(results_output):
+        results_output.to_string(index=False, buf=sys.stdout)
+    print()
+
+
+def _validate_evt_file(s, checksum=True, cols=None):
+    s = s.copy()
+    data = fileio.validate_evt_file(s['path'], checksum=checksum, cols=cols)
+    s['hash'] = data['hash']
+    s['count'] = data['count']
+    s['version'] = data['version']
+    s['err'] = data['err']
+    return s
+
+
+def _idkey(id_series):
+    """pandas.DataFrame.sort_values key callable"""
+    def make_key(id_):
         try:
-            data = fileio.read_evt(filepath)
-            version = data['version']
-            status = 'OK'
-            ok += 1
-            events = len(data['df'].index)
-        except errors.FileError as e:
-            status = str(e)
-            bad += 1
-
-        if not header_printed:
-            print('\t'.join(['path', 'file_id', 'version', 'status', 'events']))
-            header_printed = True
-        if (report_all and status == 'OK') or (status != 'OK'):
-            print('\t'.join([filepath, file_id, version, status, str(events)]))
-    print('%d/%d files passed validation' % (ok, bad + ok), file=sys.stderr)
+            sf = seaflowfile.SeaFlowFile(id_)
+        except errors.FileError:
+            return id_
+        else:
+            return sf.sort_key
+
+    return id_series.apply(make_key)
 
 
 @evt_cmd.command('parquet')
 @click.option('-n', '--n-jobs', default=1, type=int, help='worker jobs')
 @click.option('-o', '--out-dir', default='.', type=click.Path(path_type=pathlib.Path),
     help='Output directory')
+@click.option('-p', '--progress', is_flag=True,
+    help='Print progress')
 @click.argument('paths', nargs=-1, type=click.Path(exists=True, path_type=str))
-def parquet_cmd(n_jobs, out_dir, paths):
+def parquet_cmd(n_jobs, out_dir, progress, paths):
     """
     Convert binary EVT files to reduced Parquet.
 
     Output files will be placed in appropriate day of year directories inside
     out-dir.
     """
     in_files = [f for f in expand_file_list(paths)]
     parquet_files = []
     for f in in_files:
         sf = seaflowfile.SeaFlowFile(f)
         parquet_files.append(str(out_dir / sf.dayofyear / f"{sf.filename_orig}.parquet"))
     print('Converting %d input EVT files' % (len(in_files),), file=sys.stderr)
-    parallel = Parallel(n_jobs=n_jobs, verbose=1)
+    if progress:
+        verbose = 1
+    else:
+        verbose = 0
+    parallel = Parallel(n_jobs=n_jobs, verbose=verbose)
     args = zip(in_files, parquet_files)
     results = parallel(delayed(_binary_to_parquet)(*a) for a in args)
     error_lines = [f"  {r[0]}: {r[1]}" for r in results if r[1] is not None]
     if error_lines:
         print('Errors:', file=sys.stderr)
         print(
             '\n'.join(error_lines),
             file=sys.stderr
         )
     ok = len([r for r in results if r[1] is None])
     print('Converted %d / %d files' % (ok, len(in_files)), file=sys.stderr)
 
 
+def _binary_to_parquet(infile, outfile):
+    try:
+        fileio.binary_to_parquet(infile, outfile)
+    except (errors.FileError, IOError) as e:
+        return (infile, e)
+    return (infile, None)
+
+
+@evt_cmd.command('compare')
+@click.option('-a', '--all', 'report_all', is_flag=True,
+    help='Show information for all files. If not specified then only file that differ are printed.')
+@click.option('-n', '--n-jobs', default=1, type=int, help='worker jobs')
+@click.option('-p', '--progress', is_flag=True,
+    help='Print progress')
+@click.option('-r', '--reduced-columns', is_flag=True,
+    help=f'Hash on the reduced column set {fileio.REDUCED_COLS}')
+@click.argument('paths', nargs=2, type=click.Path(exists=True, path_type=pathlib.Path))
+def compare_evt_cmd(report_all, n_jobs, progress, reduced_columns, paths):
+    """
+    Compare EVT files for equality.
+
+    paths can either be two EVT files or two directories of EVT files. If
+    arguments are directories, EVT files are matched by canonical SeaFlow file
+    ID, and files with unparsable names are ignored. If both arguments are files
+    then file name parsing is not performed.
+
+    Equality is determined by joblib.hash() output. A TSV table of results is
+    printed to STDOUT for EVT dataframes that differ. If --all, all files are
+    reported, even those that match. Read and parsing errors are printed to
+    STDERR.
+    """
+    if paths[0].is_file() and paths[1].is_file():
+        # Ignore IDs to allow comparison between files with arbitrary names
+        x_files = pd.DataFrame({"id": ["-"], "path": [str(paths[0])]})
+        y_files = pd.DataFrame({"id": ["-"], "path": [str(paths[1])]})
+    elif paths[0].is_dir() and paths[1].is_dir():
+        x_ids, x_paths = [], []
+        y_ids, y_paths = [], []
+        for f in expand_file_list([str(paths[0])]):
+            try:
+                sf = seaflowfile.SeaFlowFile(f)
+            except errors.FileError as e:
+                print('error parsing file name for %s: %s' % (f, str(e)))
+            else:
+                x_ids.append(sf.file_id)
+                x_paths.append(f)
+        for f in expand_file_list([str(paths[1])]):
+            try:
+                sf = seaflowfile.SeaFlowFile(f)
+            except errors.FileError as e:
+                print('error parsing file name for %s: %s' % (f, str(e)))
+            else:
+                y_ids.append(sf.file_id)
+                y_paths.append(f)
+        x_files = pd.DataFrame({"id": x_ids, "path": x_paths})
+        y_files = pd.DataFrame({"id": y_ids, "path": y_paths})
+    else:
+        raise click.ClickException('path arguments must be two files or two directories')
+
+    if reduced_columns:
+        cols = fileio.REDUCED_COLS
+    else:
+        cols = None
+
+    m = x_files.merge(y_files, how='outer', on='id', indicator=True)
+    if m['id'].duplicated().any():
+        print('the following File IDs were duplicated in at least one dir and will be ignored', file=sys.stderr)
+        m.loc[m['id'].duplicated(), ['id', 'path_x', 'path_y']].to_string(index=False, bug=sys.stderr)
+        m = m.loc[~m['id'].duplicated()]
+
+    if progress:
+        verbose = 1
+    else:
+        verbose = 0
+    parallel = Parallel(n_jobs=n_jobs, verbose=verbose)
+    work_func = partial(_compare_two_files, cols=cols)
+    m_hashed = pd.DataFrame(parallel(delayed(work_func)(r[1]) for r in m.iterrows()))
+    m_hashed.sort_values(by='id', key=_idkey, inplace=True)
+
+    if report_all:
+        m_output = m_hashed
+    else:
+        m_output = m_hashed.loc[~m_hashed['equal']]
+    if len(m_output):
+        m_output.to_string(index=False, buf=sys.stdout)
+    print()
+
+
+def _compare_two_files(s, cols=None):
+    s = s.copy()
+
+    if pd.isna(s["path_x"]):
+        x = pd.Series({ "version": "-", "err": None, "hash": "-", "count": 0 })
+    else:
+        x = fileio.validate_evt_file(s["path_x"], checksum=True, cols=cols)
+    if pd.isna(s["path_y"]):
+        y = pd.Series({ "version": "-", "err": None, "hash": "-", "count": 0 })
+    else:
+        y = fileio.validate_evt_file(s["path_y"], checksum=True, cols=cols)
+
+    s["equal"] = (x["hash"] == y["hash"]) and (x["hash"] != "-") and (y["hash"] != "-")
+    s["hash_x"] = x["hash"]
+    s["hash_y"] = y["hash"]
+    s["count_x"] = x["count"]
+    s["count_y"] = y["count"]
+    s["version_x"] = x["version"]
+    s["version_y"] = y["version"]
+    s["err_x"] = x["err"]
+    s["err_y"] = y["err"]
+
+    return s
+
+
 def expand_file_list(files_and_dirs):
     """Convert directories in file list to EVT file paths."""
     # Find files in directories
     dirs = [f for f in files_and_dirs if os.path.isdir(f)]
     files = [f for f in files_and_dirs if os.path.isfile(f)]
 
     dfiles = []
     for d in dirs:
         dfiles = dfiles + seaflowfile.find_evt_files(d)
 
     return files + dfiles
-
-
-def _binary_to_parquet(infile, outfile):
-    try:
-        fileio.binary_to_parquet(infile, outfile)
-    except (errors.FileError, IOError) as e:
-        return (infile, e)
-    return (infile, None)
```

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/filter_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/filter_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/opp_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/opp_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cli/commands/sfl_cmd.py` & `seaflowpy-7.1.0/src/seaflowpy/cli/commands/sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/cloud.py` & `seaflowpy-7.1.0/src/seaflowpy/cloud.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/data/popcycle.sql` & `seaflowpy-7.1.0/src/seaflowpy/data/popcycle.sql`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/db.py` & `seaflowpy-7.1.0/src/seaflowpy/db.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/fileio.py` & `seaflowpy-7.1.0/src/seaflowpy/fileio.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 from contextlib import contextmanager
 import gzip
 import io
 import os
 import zlib
 from pathlib import Path
 
+import joblib
 import numpy as np
 import pandas as pd
 from . import errors
 from . import particleops
 from .seaflowfile import SeaFlowFile
 from . import util
 
+# Reduced column set for Parquet EVT files
+REDUCED_COLS = ["D1", "D2", "fsc_small", "pe", "chl_small"]
 
 @contextmanager
 def file_open_r(path, fileobj=None, as_text=False):
     """
     Open path or fileobj for reading as a context manager.
 
     Data read from the return value of this function will come from path or
@@ -433,7 +436,35 @@
     df.to_parquet(outpath, compression="snappy", index=False, engine="pyarrow")
 
 
 def binary_to_parquet(infile, outfile):
     df = read_evt(infile)["df"][["D1", "D2", "fsc_small", "pe", "chl_small"]]
     Path(outfile).parent.mkdir(parents=True, exist_ok=True)
     df.to_parquet(outfile)
+
+
+def validate_evt_file(f, checksum=True, cols=None):
+    data = {
+        "version": "-",
+        "err": None,
+        "hash": "-",
+        "count": 0
+    }
+
+    try:
+        file_data = read_evt(f)
+    except (errors.FileError, IOError) as e:
+        data["err"] = str(e)
+    else:
+        df = file_data["df"]
+        data["version"] = file_data["version"]
+        data["count"] = len(df.index)
+        if checksum:
+            if cols:
+                try:
+                    data["hash"] = joblib.hash(df[cols].reset_index(drop=True))
+                except KeyError as e:
+                    data["err"] = str(e)
+            else:
+                data["hash"] = joblib.hash(df.reset_index(drop=True))
+
+    return pd.Series(data)
```

### Comparing `seaflowpy-7.0.0/src/seaflowpy/filterevt.py` & `seaflowpy-7.1.0/src/seaflowpy/filterevt.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/geo.py` & `seaflowpy-7.1.0/src/seaflowpy/geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/particleops.py` & `seaflowpy-7.1.0/src/seaflowpy/particleops.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/sample.py` & `seaflowpy-7.1.0/src/seaflowpy/sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/seaflowfile.py` & `seaflowpy-7.1.0/src/seaflowpy/seaflowfile.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/sfl.py` & `seaflowpy-7.1.0/src/seaflowpy/sfl.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/time.py` & `seaflowpy-7.1.0/src/seaflowpy/time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy/util.py` & `seaflowpy-7.1.0/src/seaflowpy/util.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/src/seaflowpy.egg-info/PKG-INFO` & `seaflowpy-7.1.0/src/seaflowpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 7.0.0
+Version: 7.1.0
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `seaflowpy-7.0.0/src/seaflowpy.egg-info/SOURCES.txt` & `seaflowpy-7.1.0/src/seaflowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/file_dates.parquet` & `seaflowpy-7.1.0/tests/file_dates.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/sfl.parquet` & `seaflowpy-7.1.0/tests/sfl.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/test_evtopp.py` & `seaflowpy-7.1.0/tests/test_evtopp.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/test_geo.py` & `seaflowpy-7.1.0/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/test_sample.py` & `seaflowpy-7.1.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/test_seaflowfile.py` & `seaflowpy-7.1.0/tests/test_seaflowfile.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/test_time.py` & `seaflowpy-7.1.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-7.1.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_full_one_param.db` & `seaflowpy-7.1.0/tests/testcruise_full_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_full_plan.db` & `seaflowpy-7.1.0/tests/testcruise_full_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.1.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.1.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.1.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.1.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_paramsonly_one_param.db` & `seaflowpy-7.1.0/tests/testcruise_paramsonly_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/tests/testcruise_paramsonly_plan.db` & `seaflowpy-7.1.0/tests/testcruise_paramsonly_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-7.0.0/versioneer.py` & `seaflowpy-7.1.0/versioneer.py`

 * *Files identical despite different names*

