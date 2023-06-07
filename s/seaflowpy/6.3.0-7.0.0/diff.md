# Comparing `tmp/seaflowpy-6.3.0.tar.gz` & `tmp/seaflowpy-7.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaflowpy-6.3.0.tar", last modified: Tue Jun  6 19:55:54 2023, max compression
+gzip compressed data, was "seaflowpy-7.0.0.tar", last modified: Wed Jun  7 22:49:11 2023, max compression
```

## Comparing `seaflowpy-6.3.0.tar` & `seaflowpy-7.0.0.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.083197 seaflowpy-6.3.0/
--rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-6.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-6.3.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     6771 2023-06-06 19:55:54.083197 seaflowpy-6.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-6.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)      245 2023-06-06 19:55:54.085198 seaflowpy-6.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-6.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.021197 seaflowpy-6.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.086197 seaflowpy-6.3.0/src/seaflowpy/
--rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-6.3.0/src/seaflowpy/__init__.py
--rw-r--r--   0 root         (0) root         (0)      497 2023-06-06 19:55:54.086197 seaflowpy-6.3.0/src/seaflowpy/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.041197 seaflowpy-6.3.0/src/seaflowpy/cli/
--rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/__init__.py
--rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-6.3.0/src/seaflowpy/cli/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.044197 seaflowpy-6.3.0/src/seaflowpy/cli/commands/
--rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/dayofyear_cmd.py
--rw-r--r--   0 root         (0) root         (0)     5751 2023-06-06 18:39:22.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/db_cmd.py
--rw-r--r--   0 root         (0) root         (0)    12247 2022-10-28 22:17:48.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/evt_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/filter_cmd.py
--rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/opp_cmd.py
--rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/sfl_cmd.py
--rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/cli/commands/version_cmd.py
--rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-6.3.0/src/seaflowpy/cloud.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.044197 seaflowpy-6.3.0/src/seaflowpy/data/
--rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-6.3.0/src/seaflowpy/data/popcycle.sql
--rw-r--r--   0 root         (0) root         (0)    13751 2023-06-06 18:37:53.000000 seaflowpy-6.3.0/src/seaflowpy/db.py
--rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-6.3.0/src/seaflowpy/errors.py
--rw-r--r--   0 root         (0) root         (0)    13696 2022-08-22 23:54:55.000000 seaflowpy-6.3.0/src/seaflowpy/fileio.py
--rw-r--r--   0 root         (0) root         (0)    13776 2022-04-21 21:40:19.000000 seaflowpy-6.3.0/src/seaflowpy/filterevt.py
--rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-6.3.0/src/seaflowpy/geo.py
--rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-6.3.0/src/seaflowpy/particleops.py
--rw-r--r--   0 root         (0) root         (0)    10280 2022-10-31 23:12:46.000000 seaflowpy-6.3.0/src/seaflowpy/sample.py
--rw-r--r--   0 root         (0) root         (0)     9411 2022-08-18 22:28:13.000000 seaflowpy-6.3.0/src/seaflowpy/seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-6.3.0/src/seaflowpy/sfl.py
--rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-6.3.0/src/seaflowpy/time.py
--rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-6.3.0/src/seaflowpy/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.040197 seaflowpy-6.3.0/src/seaflowpy.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6771 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2961 2023-06-06 19:55:54.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       47 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 19:55:53.000000 seaflowpy-6.3.0/src/seaflowpy.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.050197 seaflowpy-6.3.0/tests/
--rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-6.3.0/tests/file_dates.parquet
--rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-6.3.0/tests/sfl.parquet
--rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-6.3.0/tests/test_evtopp.py
--rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-6.3.0/tests/test_geo.py
--rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-6.3.0/tests/test_sample.py
--rw-r--r--   0 root         (0) root         (0)    18787 2022-02-18 18:39:19.000000 seaflowpy-6.3.0/tests/test_seaflowfile.py
--rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-6.3.0/tests/test_time.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.026198 seaflowpy-6.3.0/tests/testcruise_evt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.064197 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.027197 seaflowpy-6.3.0/tests/testcruise_evt_v2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.079198 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/
--rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
--rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
--rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
--rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
--rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
--rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
--rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
--rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
--rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-6.3.0/tests/testcruise_full_one_param.db
--rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-6.3.0/tests/testcruise_full_plan.db
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.082198 seaflowpy-6.3.0/tests/testcruise_opp_one_param/
--rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 19:55:54.082198 seaflowpy-6.3.0/tests/testcruise_opp_plan/
--rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-6.3.0/tests/testcruise_paramsonly_one_param.db
--rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-6.3.0/tests/testcruise_paramsonly_plan.db
--rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-6.3.0/versioneer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/
+-rw-r--r--   0 root         (0) root         (0)    35147 2016-05-27 19:28:44.000000 seaflowpy-7.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      196 2020-07-31 01:20:45.000000 seaflowpy-7.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     6399 2021-04-02 19:11:59.000000 seaflowpy-7.0.0/README.md
+-rw-r--r--   0 root         (0) root         (0)      245 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      954 2022-10-27 20:07:07.000000 seaflowpy-7.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.809349 seaflowpy-7.0.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/src/seaflowpy/
+-rw-r--r--   0 root         (0) root         (0)      317 2022-10-26 23:57:59.000000 seaflowpy-7.0.0/src/seaflowpy/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-07 22:49:11.856349 seaflowpy-7.0.0/src/seaflowpy/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.823349 seaflowpy-7.0.0/src/seaflowpy/cli/
+-rw-r--r--   0 root         (0) root         (0)       18 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      872 2022-08-19 02:08:17.000000 seaflowpy-7.0.0/src/seaflowpy/cli/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.829349 seaflowpy-7.0.0/src/seaflowpy/cli/commands/
+-rw-r--r--   0 root         (0) root         (0)      192 2022-08-19 02:07:55.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1025 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/dayofyear_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     5751 2023-06-06 18:39:22.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/db_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    13795 2023-06-07 22:00:45.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/evt_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4970 2022-02-21 23:55:50.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/filter_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     4876 2022-08-20 19:35:27.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/opp_cmd.py
+-rw-r--r--   0 root         (0) root         (0)     3999 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)    11035 2022-10-26 19:25:20.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/sfl_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      194 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/cli/commands/version_cmd.py
+-rw-r--r--   0 root         (0) root         (0)      889 2022-10-05 00:55:36.000000 seaflowpy-7.0.0/src/seaflowpy/cloud.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.829349 seaflowpy-7.0.0/src/seaflowpy/data/
+-rw-r--r--   0 root         (0) root         (0)     4882 2022-02-17 23:58:06.000000 seaflowpy-7.0.0/src/seaflowpy/data/popcycle.sql
+-rw-r--r--   0 root         (0) root         (0)    13751 2023-06-06 18:37:53.000000 seaflowpy-7.0.0/src/seaflowpy/db.py
+-rw-r--r--   0 root         (0) root         (0)      405 2022-10-05 00:55:11.000000 seaflowpy-7.0.0/src/seaflowpy/errors.py
+-rw-r--r--   0 root         (0) root         (0)    14404 2023-06-07 21:58:24.000000 seaflowpy-7.0.0/src/seaflowpy/fileio.py
+-rw-r--r--   0 root         (0) root         (0)    13774 2023-06-07 19:22:50.000000 seaflowpy-7.0.0/src/seaflowpy/filterevt.py
+-rw-r--r--   0 root         (0) root         (0)     1802 2020-03-25 18:47:11.000000 seaflowpy-7.0.0/src/seaflowpy/geo.py
+-rw-r--r--   0 root         (0) root         (0)    11203 2022-12-02 21:17:41.000000 seaflowpy-7.0.0/src/seaflowpy/particleops.py
+-rw-r--r--   0 root         (0) root         (0)    10272 2023-06-07 19:22:28.000000 seaflowpy-7.0.0/src/seaflowpy/sample.py
+-rw-r--r--   0 root         (0) root         (0)     9547 2023-06-07 20:00:45.000000 seaflowpy-7.0.0/src/seaflowpy/seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)    19632 2023-03-09 20:38:00.000000 seaflowpy-7.0.0/src/seaflowpy/sfl.py
+-rw-r--r--   0 root         (0) root         (0)      788 2020-06-11 19:02:16.000000 seaflowpy-7.0.0/src/seaflowpy/time.py
+-rw-r--r--   0 root         (0) root         (0)     3779 2022-10-05 00:08:13.000000 seaflowpy-7.0.0/src/seaflowpy/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.823349 seaflowpy-7.0.0/src/seaflowpy.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6771 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2961 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       47 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 22:49:11.000000 seaflowpy-7.0.0/src/seaflowpy.egg-info/zip-safe
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.835349 seaflowpy-7.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4604 2022-02-18 03:14:13.000000 seaflowpy-7.0.0/tests/file_dates.parquet
+-rw-r--r--   0 root         (0) root         (0)    15333 2020-06-30 22:53:10.000000 seaflowpy-7.0.0/tests/sfl.parquet
+-rw-r--r--   0 root         (0) root         (0)    18822 2022-10-31 23:10:56.000000 seaflowpy-7.0.0/tests/test_evtopp.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2020-06-11 19:02:16.000000 seaflowpy-7.0.0/tests/test_geo.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2022-10-31 23:36:27.000000 seaflowpy-7.0.0/tests/test_sample.py
+-rw-r--r--   0 root         (0) root         (0)    19659 2023-06-07 20:55:05.000000 seaflowpy-7.0.0/tests/test_seaflowfile.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2020-06-11 19:02:16.000000 seaflowpy-7.0.0/tests/test_time.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.810349 seaflowpy-7.0.0/tests/testcruise_evt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.847349 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   467922 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   289881 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   467656 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   960015 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)    90000 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   960004 2022-02-18 02:29:25.000000 seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.811349 seaflowpy-7.0.0/tests/testcruise_evt_v2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.854349 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/
+-rw-r--r--   0 root         (0) root         (0)     1468 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   367112 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)        0 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-06-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        4 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-09-02+00-00
+-rw-r--r--   0 root         (0) root         (0)        2 2022-02-18 02:29:29.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-12-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   217413 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   366512 2022-02-18 02:29:29.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz
+-rw-r--r--   0 root         (0) root         (0)   560050 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   559966 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   560008 2022-02-18 02:29:30.000000 seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00
+-rw-r--r--   0 root         (0) root         (0)   110592 2022-02-18 01:48:54.000000 seaflowpy-7.0.0/tests/testcruise_full_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   131072 2022-02-18 01:16:58.000000 seaflowpy-7.0.0/tests/testcruise_full_plan.db
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.855349 seaflowpy-7.0.0/tests/testcruise_opp_one_param/
+-rw-r--r--   0 root         (0) root         (0)    27751 2022-02-18 01:52:34.000000 seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    16329 2022-02-18 01:52:34.000000 seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 22:49:11.855349 seaflowpy-7.0.0/tests/testcruise_opp_plan/
+-rw-r--r--   0 root         (0) root         (0)    26213 2022-02-18 01:18:01.000000 seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)    17096 2022-02-18 01:18:01.000000 seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:48:34.000000 seaflowpy-7.0.0/tests/testcruise_paramsonly_one_param.db
+-rw-r--r--   0 root         (0) root         (0)   102400 2022-02-18 02:47:52.000000 seaflowpy-7.0.0/tests/testcruise_paramsonly_plan.db
+-rw-r--r--   0 root         (0) root         (0)    68611 2019-06-01 00:15:35.000000 seaflowpy-7.0.0/versioneer.py
```

### Comparing `seaflowpy-6.3.0/LICENSE` & `seaflowpy-7.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/PKG-INFO` & `seaflowpy-7.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 6.3.0
+Version: 7.0.0
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `seaflowpy-6.3.0/README.md` & `seaflowpy-7.0.0/README.md`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/setup.py` & `seaflowpy-7.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/cli.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/cli.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/dayofyear_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/dayofyear_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/db_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/db_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/evt_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/evt_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import datetime
 import logging
 import os
 import pathlib
 import sys
+from joblib import Parallel, delayed
 
 import click
 from seaflowpy import errors
 from seaflowpy import seaflowfile
 from seaflowpy import fileio
 from seaflowpy import sample
 from seaflowpy import sfl
@@ -278,15 +279,15 @@
             file_id = sff.file_id
         except errors.FileError:
             # unusual name, no file_id
             pass
 
         # Try to read file as binary EVT
         try:
-            data = fileio.read_evt_labview(filepath)
+            data = fileio.read_evt(filepath)
             version = data['version']
             status = 'OK'
             ok += 1
             events = len(data['df'].index)
         except errors.FileError as e:
             status = str(e)
             bad += 1
@@ -295,18 +296,58 @@
             print('\t'.join(['path', 'file_id', 'version', 'status', 'events']))
             header_printed = True
         if (report_all and status == 'OK') or (status != 'OK'):
             print('\t'.join([filepath, file_id, version, status, str(events)]))
     print('%d/%d files passed validation' % (ok, bad + ok), file=sys.stderr)
 
 
+@evt_cmd.command('parquet')
+@click.option('-n', '--n-jobs', default=1, type=int, help='worker jobs')
+@click.option('-o', '--out-dir', default='.', type=click.Path(path_type=pathlib.Path),
+    help='Output directory')
+@click.argument('paths', nargs=-1, type=click.Path(exists=True, path_type=str))
+def parquet_cmd(n_jobs, out_dir, paths):
+    """
+    Convert binary EVT files to reduced Parquet.
+
+    Output files will be placed in appropriate day of year directories inside
+    out-dir.
+    """
+    in_files = [f for f in expand_file_list(paths)]
+    parquet_files = []
+    for f in in_files:
+        sf = seaflowfile.SeaFlowFile(f)
+        parquet_files.append(str(out_dir / sf.dayofyear / f"{sf.filename_orig}.parquet"))
+    print('Converting %d input EVT files' % (len(in_files),), file=sys.stderr)
+    parallel = Parallel(n_jobs=n_jobs, verbose=1)
+    args = zip(in_files, parquet_files)
+    results = parallel(delayed(_binary_to_parquet)(*a) for a in args)
+    error_lines = [f"  {r[0]}: {r[1]}" for r in results if r[1] is not None]
+    if error_lines:
+        print('Errors:', file=sys.stderr)
+        print(
+            '\n'.join(error_lines),
+            file=sys.stderr
+        )
+    ok = len([r for r in results if r[1] is None])
+    print('Converted %d / %d files' % (ok, len(in_files)), file=sys.stderr)
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
+
+
+def _binary_to_parquet(infile, outfile):
+    try:
+        fileio.binary_to_parquet(infile, outfile)
+    except (errors.FileError, IOError) as e:
+        return (infile, e)
+    return (infile, None)
```

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/filter_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/filter_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/opp_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/opp_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/sds2sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cli/commands/sfl_cmd.py` & `seaflowpy-7.0.0/src/seaflowpy/cli/commands/sfl_cmd.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/cloud.py` & `seaflowpy-7.0.0/src/seaflowpy/cloud.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/data/popcycle.sql` & `seaflowpy-7.0.0/src/seaflowpy/data/popcycle.sql`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/db.py` & `seaflowpy-7.0.0/src/seaflowpy/db.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/fileio.py` & `seaflowpy-7.0.0/src/seaflowpy/fileio.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from contextlib import contextmanager
 import gzip
 import io
 import os
 import zlib
+from pathlib import Path
+
 import numpy as np
 import pandas as pd
 from . import errors
 from . import particleops
 from .seaflowfile import SeaFlowFile
 from . import util
 
@@ -228,15 +230,15 @@
     Read a raw labview binary SeaFlow data file.
 
     Data will be read from the file at the provided path or preferentially from
     fileobj if provided. If path is provided and ends with '.gz' data will be
     considered gzip compressed even if read from fileobj.
 
     Parameters
-    -----------
+    ----------
     path: str
         File path.
     fileobj: io.BytesIO, optional
         Open file object.
 
     Returns
     -------
@@ -244,14 +246,36 @@
         "version": "v1"|"v2",
         "df": SeaFlow event pandas.DataFrame as numpy.float64 values
     }
     """
     return read_labview(path, columns=None, fileobj=fileobj)
 
 
+def read_evt(path):
+    """
+    Read EVT file as raw binary, gzipped binary, or reduced Parquet.
+
+    Parameters
+    ----------
+    path: str
+        File path.
+
+    Returns
+    -------
+    dict of {
+        "version": "v1"|"v2"|"parquet",
+        "df": SeaFlow event pandas.DataFrame as numpy.float64 values
+    }
+    """
+    if path.endswith(".parquet"):
+        return { "version": "parquet", "df": pd.read_parquet(path) }
+    else:
+        return read_evt_labview(path)
+
+
 def read_filter_params_csv(path):
     """
     Read a filter parameters csv file.
 
     Parameters
     ----------
     path: str
@@ -403,7 +427,13 @@
     if df["file_id"].dtype.name != "category":
         df["file_id"] = df["file_id"].astype("category")
     if df["filter_id"].dtype.name != "category":
         df["filter_id"] = df["filter_id"].astype("category")
 
     # Write parquet
     df.to_parquet(outpath, compression="snappy", index=False, engine="pyarrow")
+
+
+def binary_to_parquet(infile, outfile):
+    df = read_evt(infile)["df"][["D1", "D2", "fsc_small", "pe", "chl_small"]]
+    Path(outfile).parent.mkdir(parents=True, exist_ok=True)
+    df.to_parquet(outfile)
```

### Comparing `seaflowpy-6.3.0/src/seaflowpy/filterevt.py` & `seaflowpy-7.0.0/src/seaflowpy/filterevt.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,17 +132,17 @@
                 "opp": None,
                 "file_id": row["file_id"],
                 "path": row["path"]
             }
 
             filter_params = work["filter_params"][row["file_id"]].reset_index(drop=True)
             try:
-                data = fileio.read_evt_labview(path=row["path"])
+                data = fileio.read_evt(row["path"])
                 evt_df = data["df"]
-            except errors.FileError as e:
+            except (errors.FileError, IOError) as e:
                 result["error"] = f"Could not parse file {row['path']}: {e}"
                 evt_df = particleops.empty_df()  # doesn't matter if v1 or v2 column composition
             except Exception as e:
                 result["error"] = f"Unexpected error when parsing file {row['path']}: {e}"
                 evt_df = particleops.empty_df()  # doesn't matter if v1 or v2 column composition
 
             try:
```

### Comparing `seaflowpy-6.3.0/src/seaflowpy/geo.py` & `seaflowpy-7.0.0/src/seaflowpy/geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/particleops.py` & `seaflowpy-7.0.0/src/seaflowpy/particleops.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/sample.py` & `seaflowpy-7.0.0/src/seaflowpy/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,15 +221,15 @@
     """
     columns = ["D1", "D2", "fsc_small", "pe", "chl_small"]
     results = []
 
     for f in evtpaths:
         msg = ""
         try:
-            data = fileio.read_evt_labview(f)
+            data = fileio.read_evt(f)
             df = data["df"]
         except Exception as e:
             msg = "{}: {}".format(type(e).__name__, str(e))
             df = particleops.empty_df()
         result = sample_one(
             df,
             n,
```

### Comparing `seaflowpy-6.3.0/src/seaflowpy/seaflowfile.py` & `seaflowpy-7.0.0/src/seaflowpy/seaflowfile.py`

 * *Files 10% similar despite different names*

```diff
@@ -23,25 +23,27 @@
         will be raised.
         """
         self.path = path
 
         parts = parse_path(self.path)
         self.filename = parts["file"]
         if parts["file"].endswith(".gz"):
-            self.filename_nogz = self.filename[:-3]
+            self.filename_orig = self.filename[:-len(".gz")]
+        elif parts["file"].endswith(".parquet"):
+            self.filename_orig = self.filename[:-len(".parquet")]
         else:
-            self.filename_nogz = self.filename
+            self.filename_orig = self.filename
 
         if not (self.is_old_style or self.is_new_style):
             raise errors.FileError("Filename doesn't look like a SeaFlow EVT file")
 
         if self.is_new_style:
             err = None
             try:
-                timestamp = timestamp_from_filename(self.filename_nogz)
+                timestamp = timestamp_from_filename(self.filename_orig)
                 self.date = time.parse_date(timestamp)
             except ValueError as e:
                 err = e
             if err:
                 raise errors.FileError(str(err))
             if date is not None and self.date != date:
                 raise ValueError(
@@ -56,33 +58,33 @@
         # YYYY_dayofyear directory found in file path and parsed
         # from file datestmap
         self.path_dayofyear = parts["dayofyear"]
 
         # Identifer to match EVT/SFL files
         # Should be something like 2014_142/42.evt for old files.
         # Should be something like 2014_342/2014-12-08T22-53-34+00-00 for new
-        # files. Note no extension including .gz.
+        # files. Note no extension including .gz or .parquet.
         # The day of year directory will be based on parsed datestamp in
         # filename when possible, not the given path. The file ID based on
         # the given path is stored in path_file_id.
         if self.is_old_style:
             # path_file_id and file_id are always the same for old-style
             # filenames since we can't parse dates to calculate a day of year
             # directory
             if self.path_dayofyear:
-                self.file_id = "{}/{}".format(self.path_dayofyear, self.filename_nogz)
+                self.file_id = "{}/{}".format(self.path_dayofyear, self.filename_orig)
             else:
-                self.file_id = self.filename_nogz
+                self.file_id = self.filename_orig
             self.path_file_id = self.file_id
         else:
-            self.file_id = "{}/{}".format(self.dayofyear, self.filename_nogz)
+            self.file_id = "{}/{}".format(self.dayofyear, self.filename_orig)
             if self.path_dayofyear:
-                self.path_file_id = "{}/{}".format(self.path_dayofyear, self.filename_nogz)
+                self.path_file_id = "{}/{}".format(self.path_dayofyear, self.filename_orig)
             else:
-                self.path_file_id = self.filename_nogz
+                self.path_file_id = self.filename_orig
 
     def __str__(self):
         return "SeaFlowFile: {}, {}".format(self.file_id, self.path)
 
     @property
     def dayofyear(self):
         """Return day of year based on date."""
@@ -92,20 +94,20 @@
     def isgz(self):
         """Is file gzipped?"""
         return self.path and self.filename.endswith(".gz")
 
     @property
     def is_old_style(self):
         """Is this old style file? e.g. 2014_185/1.evt."""
-        return bool(re.match(old_file_re, self.filename_nogz))
+        return bool(re.match(old_file_re, self.filename_orig))
 
     @property
     def is_new_style(self):
         """Is this a new style file? e.g. 2018_082/2018-03-23T00-00-00+00-00.gz"""
-        return bool(re.match(new_file_re, self.filename_nogz))
+        return bool(re.match(new_file_re, self.filename_orig))
 
     @property
     def rfc3339(self):
         """Return RFC 3339 YYYY-MM-DDThh:mm:ss[+-]hh:mm parsed from filename"""
         if self.date:
             return self.date.isoformat(timespec='seconds')
         return ''
@@ -118,17 +120,17 @@
         elif self.path_dayofyear:
             year, day = [int(x) for x in self.path_dayofyear.split("_")]
         else:
             year, day = 0, 0
         if self.is_old_style:
             # Number part of basename, necessary because number isn't
             # zero-filled
-            file_key = int(self.filename_nogz.split(".")[0])
+            file_key = int(self.filename_orig.split(".")[0])
         else:
-            file_key = self.filename_nogz
+            file_key = self.filename_orig
         return (year, day, file_key)
 
 
 def create_dayofyear_directory(dt):
     """Create SeaFlow day of year directory from a datetime object"""
     if dt:
         return "{}_{}".format(dt.year, dt.strftime('%j'))
```

### Comparing `seaflowpy-6.3.0/src/seaflowpy/sfl.py` & `seaflowpy-7.0.0/src/seaflowpy/sfl.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/time.py` & `seaflowpy-7.0.0/src/seaflowpy/time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy/util.py` & `seaflowpy-7.0.0/src/seaflowpy/util.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/src/seaflowpy.egg-info/PKG-INFO` & `seaflowpy-7.0.0/src/seaflowpy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaflowpy
-Version: 6.3.0
+Version: 7.0.0
 Summary: A Python library for SeaFlow data.
 Home-page: https://github.com/armbrustlab/seaflowpy
 Author: Chris T. Berthiaume
 Author-email: chrisbee@uw.edu
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Requires-Python: >=3.7.1
 Description-Content-Type: text/markdown
```

### Comparing `seaflowpy-6.3.0/src/seaflowpy.egg-info/SOURCES.txt` & `seaflowpy-7.0.0/src/seaflowpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/file_dates.parquet` & `seaflowpy-7.0.0/tests/file_dates.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/sfl.parquet` & `seaflowpy-7.0.0/tests/sfl.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/test_evtopp.py` & `seaflowpy-7.0.0/tests/test_evtopp.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/test_geo.py` & `seaflowpy-7.0.0/tests/test_geo.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/test_sample.py` & `seaflowpy-7.0.0/tests/test_sample.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/test_seaflowfile.py` & `seaflowpy-7.0.0/tests/test_seaflowfile.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,138 +21,149 @@
     with pytest.raises(sfp.errors.FileError):
         _ = sfp.seaflowfile.SeaFlowFile("2014-07-32T00-00-02+00-00")
 
 def test_new_style():
     f = sfp.seaflowfile.SeaFlowFile("2014-07-04T00-00-02+00-00")
     assert f.path == "2014-07-04T00-00-02+00-00"
     assert f.filename == "2014-07-04T00-00-02+00-00"
-    assert f.filename_nogz == "2014-07-04T00-00-02+00-00"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
     assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.path_file_id == "2014-07-04T00-00-02+00-00"
     assert f.dayofyear == "2014_185"
     assert f.path_dayofyear == ''
     assert f.is_old_style is False
     assert f.is_new_style is True
 
     f = sfp.seaflowfile.SeaFlowFile("2014_185/2014-07-04T00-00-02+00-00")
     assert f.path == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.filename == "2014-07-04T00-00-02+00-00"
-    assert f.filename_nogz == "2014-07-04T00-00-02+00-00"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
     assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.path_file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.dayofyear == "2014_185"
     assert f.path_dayofyear == "2014_185"
     assert f.is_old_style is False
     assert f.is_new_style is True
 
     f = sfp.seaflowfile.SeaFlowFile("foo/2014-07-04T00-00-02+00-00")
     assert f.path == "foo/2014-07-04T00-00-02+00-00"
     assert f.filename == "2014-07-04T00-00-02+00-00"
-    assert f.filename_nogz == "2014-07-04T00-00-02+00-00"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
     assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.path_file_id == "2014-07-04T00-00-02+00-00"
     assert f.dayofyear == "2014_185"
     assert f.path_dayofyear == ''
     assert f.is_old_style is False
     assert f.is_new_style is True
 
     f = sfp.seaflowfile.SeaFlowFile("foo/2014_185/2014-07-04T00-00-02+00-00")
     assert f.path == "foo/2014_185/2014-07-04T00-00-02+00-00"
     assert f.filename == "2014-07-04T00-00-02+00-00"
-    assert f.filename_nogz == "2014-07-04T00-00-02+00-00"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
     assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.path_file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.dayofyear == "2014_185"
     assert f.path_dayofyear == "2014_185"
     assert f.is_old_style is False
     assert f.is_new_style is True
 
     f = sfp.seaflowfile.SeaFlowFile("foo/bar/2014-07-04T00-00-02+00-00")
     assert f.path == "foo/bar/2014-07-04T00-00-02+00-00"
     assert f.filename == "2014-07-04T00-00-02+00-00"
-    assert f.filename_nogz == "2014-07-04T00-00-02+00-00"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
     assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.path_file_id == "2014-07-04T00-00-02+00-00"
     assert f.dayofyear == "2014_185"
     assert f.path_dayofyear == ''
     assert f.is_old_style is False
     assert f.is_new_style is True
 
     f = sfp.seaflowfile.SeaFlowFile("foo/bar/2014-07-04T00-00-02+00-00.gz")
     assert f.path == "foo/bar/2014-07-04T00-00-02+00-00.gz"
     assert f.filename == "2014-07-04T00-00-02+00-00.gz"
-    assert f.filename_nogz == "2014-07-04T00-00-02+00-00"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
+    assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
+    assert f.path_file_id == "2014-07-04T00-00-02+00-00"
+    assert f.dayofyear == "2014_185"
+    assert f.path_dayofyear == ''
+    assert f.is_old_style is False
+    assert f.is_new_style is True
+
+    f = sfp.seaflowfile.SeaFlowFile("foo/bar/2014-07-04T00-00-02+00-00.parquet")
+    assert f.path == "foo/bar/2014-07-04T00-00-02+00-00.parquet"
+    assert f.filename == "2014-07-04T00-00-02+00-00.parquet"
+    assert f.filename_orig == "2014-07-04T00-00-02+00-00"
     assert f.file_id == "2014_185/2014-07-04T00-00-02+00-00"
     assert f.path_file_id == "2014-07-04T00-00-02+00-00"
     assert f.dayofyear == "2014_185"
     assert f.path_dayofyear == ''
     assert f.is_old_style is False
     assert f.is_new_style is True
 
 
 def test_old_style():
     f = sfp.seaflowfile.SeaFlowFile("42.evt")
     assert f.path == "42.evt"
     assert f.filename == "42.evt"
-    assert f.filename_nogz == "42.evt"
+    assert f.filename_orig == "42.evt"
     assert f.file_id == "42.evt"
     assert f.path_file_id == f.file_id
     assert f.dayofyear == ''
     assert f.path_dayofyear == ''
     assert f.is_old_style is True
     assert f.is_new_style is False
 
     f = sfp.seaflowfile.SeaFlowFile("2014_185/42.evt")
     assert f.path == "2014_185/42.evt"
     assert f.filename == "42.evt"
-    assert f.filename_nogz == "42.evt"
+    assert f.filename_orig == "42.evt"
     assert f.file_id == "2014_185/42.evt"
     assert f.path_file_id == f.file_id
     assert f.dayofyear == ''
     assert f.path_dayofyear == "2014_185"
     assert f.is_old_style is True
     assert f.is_new_style is False
 
     f = sfp.seaflowfile.SeaFlowFile("foo/42.evt")
     assert f.path == "foo/42.evt"
     assert f.filename == "42.evt"
-    assert f.filename_nogz == "42.evt"
+    assert f.filename_orig == "42.evt"
     assert f.path_file_id == f.file_id
     assert f.file_id == "42.evt"
     assert f.dayofyear == ''
     assert f.path_dayofyear == ''
     assert f.is_old_style is True
     assert f.is_new_style is False
 
     f = sfp.seaflowfile.SeaFlowFile("foo/2014_185/42.evt")
     assert f.path == "foo/2014_185/42.evt"
     assert f.filename == "42.evt"
-    assert f.filename_nogz == "42.evt"
+    assert f.filename_orig == "42.evt"
     assert f.file_id == "2014_185/42.evt"
     assert f.path_file_id == f.file_id
     assert f.dayofyear == ''
     assert f.path_dayofyear == "2014_185"
     assert f.is_old_style is True
     assert f.is_new_style is False
 
     f = sfp.seaflowfile.SeaFlowFile("foo/bar/42.evt")
     assert f.path == "foo/bar/42.evt"
     assert f.filename == "42.evt"
-    assert f.filename_nogz == "42.evt"
+    assert f.filename_orig == "42.evt"
     assert f.file_id == "42.evt"
     assert f.path_file_id == f.file_id
     assert f.dayofyear == ''
     assert f.path_dayofyear == ''
     assert f.is_old_style is True
     assert f.is_new_style is False
 
     f = sfp.seaflowfile.SeaFlowFile("foo/bar/42.evt.gz")
     assert f.path == "foo/bar/42.evt.gz"
     assert f.filename == "42.evt.gz"
-    assert f.filename_nogz == "42.evt"
+    assert f.filename_orig == "42.evt"
     assert f.file_id == "42.evt"
     assert f.path_file_id == f.file_id
     assert f.dayofyear == ''
     assert f.path_dayofyear == ''
     assert f.is_old_style is True
     assert f.is_new_style is False
 
@@ -220,15 +231,15 @@
     assert sfp.seaflowfile.sorted_files(unsorted_files) == sorted_files
 
 
 def test_date_from_file_name():
     files = [
         "2014-07-06T00-00-05+00-00",
         "2014-07-06T00-00-05-00-00",
-        "2014-07-06T00-00-05-07-00",  # all dates assumed UTC, even if non-UTC TZ offset
+        "2014-07-06T00-00-05-07-00.parquet",  # all dates assumed UTC, even if non-UTC TZ offset
         "2014-07-06T00-00-05+00-00.gz"
     ]
     answers = [
         "2014-07-06T00:00:05+00:00",
         "2014-07-06T00:00:05+00:00",
         "2014-07-06T00:00:05+00:00",  # all dates assumed UTC, even if non-UTC TZ offset
         "2014-07-06T00:00:05+00:00"
@@ -238,19 +249,19 @@
         assert s.rfc3339 == answers[i]
 
 
 def test_dayofyear_from_filename():
     files = [
         "2014-07-06T00-00-05+00-00",
         "2014-07-06T00-00-05-00-00",
-        "2014-07-06T00-00-05-07-00",
+        "2014-07-06T00-00-05-07-00.parquet",
         "2014-07-06T00-00-05+00-00.gz",
         "2014_001/2014-07-06T00-00-05+00-00",
         "2014_001/2014-07-06T00-00-05-00-00",
-        "2014_001/2014-07-06T00-00-05-07-00",
+        "2014_001/2014-07-06T00-00-05-07-00.parquet",
         "2014_001/2014-07-06T00-00-05+00-00.gz"
     ]
     dayofyear_answer = "2014_187"
     path_dayofyear_answer = "2014_001"
 
     for f in files[0:4]:
         s = sfp.seaflowfile.SeaFlowFile(f)
@@ -263,22 +274,26 @@
         assert s.path_dayofyear == path_dayofyear_answer
 
 def test_parse_path():
     files = [
         "2014_187/2014-07-06T00-00-05-00-00",
         "2014-07-06T00-00-05-00-00",
         "2014_187/2014-07-06T00-00-05-00-00.gz",
-        "2014-07-06T00-00-05-00-00.gz"
+        "2014-07-06T00-00-05-00-00.gz",
+        "2014_187/2014-07-06T00-00-05-00-00.parquet",
+        "2014-07-06T00-00-05-00-00.parquet"
     ]
 
     answers = [
         {"file": "2014-07-06T00-00-05-00-00", "dayofyear": "2014_187"},
         {"file": "2014-07-06T00-00-05-00-00", "dayofyear": ''},
         {"file": "2014-07-06T00-00-05-00-00.gz", "dayofyear": "2014_187"},
-        {"file": "2014-07-06T00-00-05-00-00.gz", "dayofyear": ''}
+        {"file": "2014-07-06T00-00-05-00-00.gz", "dayofyear": ''},
+        {"file": "2014-07-06T00-00-05-00-00.parquet", "dayofyear": "2014_187"},
+        {"file": "2014-07-06T00-00-05-00-00.parquet", "dayofyear": ''}
     ]
 
     for i, f in enumerate(files):
         assert sfp.seaflowfile.parse_path(f) == answers[i]
 
 def test_fix_file_id():
     origid = "2014_001/2014-12-08T22-53-34+00-00"
@@ -289,15 +304,15 @@
 
 def test_file_list_filter():
     files = [
         "tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00",
         "tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz",
         "tests/testcruise_evt/2014_185/2014-07-04T00-06-02+00-00",
         "tests/testcruise_evt/2014_185/2014-07-04T00-09-02+00-00",
-        "tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00",
+        "tests/testcruise_evt/2014_185/2014-07-04T00-12-02+00-00.parquet",
         "tests/testcruise_evt/2014_185/2014-07-04T00-15-02+00-00.gz",
         "tests/testcruise_evt/2014_185/2014-07-04T00-17-02+00-00.gz",
         "tests/testcruise_evt/2014_185/2014-07-04T00-21-02+00-00"
     ]
     filter_list = [
         "2014_185/2014-07-04T00-00-02+00-00",
         "testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz",
@@ -317,14 +332,15 @@
 def test_keep_evt_files():
     files = [
         "testcruise/2014_185/100.evt",
         "testcruise/2014_185/200.evt.gz",
         "not_evt_file",
         "testcruise/2014_185/2014-07-04T00-00-02+00-00",
         "testcruise/2014_185/2014-07-04T00-03-02+00-00.gz",
+        "testcruise/2014_185/2014-07-04T00-06-02+00-00.parquet",
     ]
     parsed = sfp.seaflowfile.keep_evt_files(files)
     assert parsed == (files[:2] + files[3:])
 
 def test_find_evt_files():
     files = sfp.seaflowfile.find_evt_files("tests/testcruise_evt")
     answer = [
```

### Comparing `seaflowpy-6.3.0/tests/test_time.py` & `seaflowpy-7.0.0/tests/test_time.py`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-00+00-00.sfl`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-00-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T00-03-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-15-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-17-02+00-00.gz`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-21-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-27-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00` & `seaflowpy-7.0.0/tests/testcruise_evt_v2/2014_185/2014-07-04T01-30-02+00-00`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_full_one_param.db` & `seaflowpy-7.0.0/tests/testcruise_full_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_full_plan.db` & `seaflowpy-7.0.0/tests/testcruise_full_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.0.0/tests/testcruise_opp_one_param/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T00-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet` & `seaflowpy-7.0.0/tests/testcruise_opp_plan/2014-07-04T01-00-00+00-00.1H.opp.parquet`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_paramsonly_one_param.db` & `seaflowpy-7.0.0/tests/testcruise_paramsonly_one_param.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/tests/testcruise_paramsonly_plan.db` & `seaflowpy-7.0.0/tests/testcruise_paramsonly_plan.db`

 * *Files identical despite different names*

### Comparing `seaflowpy-6.3.0/versioneer.py` & `seaflowpy-7.0.0/versioneer.py`

 * *Files identical despite different names*

