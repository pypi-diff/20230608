# Comparing `tmp/etm-dgraham-5.0.6.tar.gz` & `tmp/etm-dgraham-5.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-5.0.6.tar", last modified: Mon Jun  5 16:41:52 2023, max compression
+gzip compressed data, was "etm-dgraham-5.0.7.tar", last modified: Thu Jun  8 12:38:43 2023, max compression
```

## Comparing `etm-dgraham-5.0.6.tar` & `etm-dgraham-5.0.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.498357 etm-dgraham-5.0.6/
--rw-r--r--   0 dag        (501) staff       (20)     2373 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-05 16:41:52.498197 etm-dgraham-5.0.6/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.6/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.6/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.6/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.488544 etm-dgraham-5.0.6/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.493010 etm-dgraham-5.0.6/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.6/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/etm/__version__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.6/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.6/etm/ical.py
--rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.6/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   277830 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.6/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.6/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)    97610 2023-06-05 16:41:33.000000 etm-dgraham-5.0.6/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.495446 etm-dgraham-5.0.6/etm_dgraham.egg-info/
--rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-05 16:41:52.000000 etm-dgraham-5.0.6/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.6/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.6/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/namedcolors.py
--rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.6/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-05 16:41:52.498393 etm-dgraham-5.0.6/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.6/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.495558 etm-dgraham-5.0.6/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.6/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-05 16:41:52.497575 etm-dgraham-5.0.6/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.6/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.6/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.6/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.6/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.760417 etm-dgraham-5.0.7/
+-rw-r--r--   0 dag        (501) staff       (20)     2361 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   129427 2023-06-08 12:38:43.760237 etm-dgraham-5.0.7/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   128515 2023-06-04 22:28:52.000000 etm-dgraham-5.0.7/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-5.0.7/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     3862 2022-11-15 20:51:01.000000 etm-dgraham-5.0.7/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.754487 etm-dgraham-5.0.7/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.756811 etm-dgraham-5.0.7/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    16118 2023-06-03 11:21:41.000000 etm-dgraham-5.0.7/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/etm/__version__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    13339 2023-06-03 11:21:41.000000 etm-dgraham-5.0.7/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    20798 2022-06-28 16:10:19.000000 etm-dgraham-5.0.7/etm/ical.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     4986 2023-06-04 20:44:52.000000 etm-dgraham-5.0.7/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   280674 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    37255 2023-05-23 18:01:39.000000 etm-dgraham-5.0.7/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    23699 2022-12-06 22:09:21.000000 etm-dgraham-5.0.7/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    98299 2023-06-08 12:38:29.000000 etm-dgraham-5.0.7/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.758654 etm-dgraham-5.0.7/etm_dgraham.egg-info/
+-rwxrwxrwx   0 dag        (501) staff       (20)   129427 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      880 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      362 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2023-06-08 12:38:43.000000 etm-dgraham-5.0.7/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-5.0.7/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-5.0.7/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/namedcolors.py
+-rw-rw-rw-   0 dag        (501) staff       (20)    91778 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-5.0.7/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2023-06-08 12:38:43.760473 etm-dgraham-5.0.7/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4828 2022-12-16 21:09:57.000000 etm-dgraham-5.0.7/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.758751 etm-dgraham-5.0.7/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-5.0.7/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2023-06-08 12:38:43.759629 etm-dgraham-5.0.7/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-5.0.7/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2020-07-27 15:42:26.000000 etm-dgraham-5.0.7/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-5.0.7/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-5.0.7/utilities/open_in_mutt
```

### Comparing `etm-dgraham-5.0.6/CHANGES.txt` & `etm-dgraham-5.0.7/CHANGES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,58 +1,62 @@
-Recent tagged changes as of 2023-06-05T12:41:31.118562-04:00:
-- 0 seconds ago (HEAD -> working, tag: 5.0.6) Daniel Graham
+Recent tagged changes as of 2023-06-08T08:38:27.324898-04:00:
+- 0 seconds ago (HEAD -> working, tag: 5.0.7) Daniel Graham
+    b9eccc6 2023-06-08 08:38:27 -0400
+    Tagged version 5.0.7.
+
+- 3 days ago (tag: 5.0.6) Daniel Graham
     345ca4e 2023-06-05 12:41:31 -0400
     Tagged version 5.0.6.
 
-- 6 hours ago (tag: 5.0.5) Daniel Graham
+- 3 days ago (tag: 5.0.5) Daniel Graham
     9273685 2023-06-05 06:28:25 -0400
     Tagged version 5.0.5.
 
-- 7 hours ago (tag: 5.0.4) Daniel Graham
+- 3 days ago (tag: 5.0.4) Daniel Graham
     ea199ac 2023-06-05 06:02:56 -0400
     Tagged version 5.0.4.
 
-- 20 hours ago (tag: 5.0.3) Daniel Graham
+- 4 days ago (tag: 5.0.3) Daniel Graham
     e0a0d9e 2023-06-04 16:44:49 -0400
     Tagged version 5.0.3.
 
-- 23 hours ago (tag: 5.0.2) Daniel Graham
+- 4 days ago (tag: 5.0.2) Daniel Graham
     4c5d4bb 2023-06-04 13:26:17 -0400
     Tagged version 5.0.2.
 
-- 24 hours ago (tag: 5.0.1) Daniel Graham
+- 4 days ago (tag: 5.0.1) Daniel Graham
     b30f0ed 2023-06-04 12:47:15 -0400
     Tagged version 5.0.1.
 
-- 2 days ago (tag: 5.0.0) Daniel Graham
+- 5 days ago (tag: 5.0.0) Daniel Graham
     7bc8090 2023-06-03 07:21:38 -0400
     Tagged version 5.0.0. Use pendulum periods for f and elements of h
     instead of datetimes.
 
-- 9 days ago (tag: 4.12.9) Daniel Graham
+- 12 days ago (tag: 4.12.9) Daniel Graham
     b8fbc47 2023-05-27 13:45:19 -0400
     Tagged version 4.12.9.
 
-- 10 days ago (tag: 4.12.8) Daniel Graham
+- 13 days ago (tag: 4.12.8) Daniel Graham
     b0316d5 2023-05-26 13:50:15 -0400
     Tagged version 4.12.8.
 
-- 11 days ago (tag: 4.12.7) Daniel Graham
+- 2 weeks ago (tag: 4.12.7) Daniel Graham
     442ff98 2023-05-25 13:53:52 -0400
     Tagged version 4.12.7.
 
-- 13 days ago (tag: 4.12.6) Daniel Graham
+- 2 weeks ago (tag: 4.12.6) Daniel Graham
     3da7332 2023-05-23 14:01:37 -0400
     Tagged version 4.12.6.
 
-- 2 weeks ago (tag: 4.12.5) Daniel Graham
+- 3 weeks ago (tag: 4.12.5) Daniel Graham
     f0c24d8 2023-05-21 15:08:06 -0400
     Tagged version 4.12.5.
 
-- 2 weeks ago (tag: 4.12.4) Daniel Graham
+- 3 weeks ago (tag: 4.12.4) Daniel Graham
     15b3333 2023-05-20 14:33:40 -0400
     Tagged version 4.12.4.
 
 - 3 weeks ago (tag: 4.12.3) Daniel Graham
     dd49fda 2023-05-17 12:24:12 -0400
     Tagged version 4.12.3.
 
@@ -61,22 +65,18 @@
     Tagged version 4.12.2.
 
 - 3 weeks ago (tag: 4.12.1) Daniel Graham
     68005b7 2023-05-15 14:20:25 -0400
     Tagged version 4.12.1. Added display for all-day events to busy
     view
 
-- 3 weeks ago (tag: 4.12.0) Daniel Graham
+- 4 weeks ago (tag: 4.12.0) Daniel Graham
     ce2ab09 2023-05-13 12:46:39 -0400
     Tagged version 4.12.0. Added engaged view
 
 - 4 weeks ago (tag: 4.11.18) Daniel Graham
     cd5482a 2023-05-11 12:20:48 -0400
     Tagged version 4.11.18.
 
 - 4 weeks ago (tag: 4.11.17) Daniel Graham
     8a02515 2023-05-09 10:14:28 -0400
     Tagged version 4.11.17.
-
-- 5 weeks ago (tag: 4.11.16) Daniel Graham
-    b2310ce 2023-05-01 14:43:18 -0400
-    Tagged version 4.11.16.
```

### Comparing `etm-dgraham-5.0.6/PKG-INFO` & `etm-dgraham-5.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.6
+Version: 5.0.7
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.6/README.md` & `etm-dgraham-5.0.7/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/bump.py` & `etm-dgraham-5.0.7/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/docs/index_konnections.md` & `etm-dgraham-5.0.7/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/docs/index_usedtime.md` & `etm-dgraham-5.0.7/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/docs/multiple_timers.md` & `etm-dgraham-5.0.7/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/__main__.py` & `etm-dgraham-5.0.7/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/data.py` & `etm-dgraham-5.0.7/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/ical.py` & `etm-dgraham-5.0.7/etm/ical.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/make_examples.py` & `etm-dgraham-5.0.7/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/model.py` & `etm-dgraham-5.0.7/etm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -656,38 +656,38 @@
         try:
             self.db.remove(doc_ids=[doc_id])
             return True
         except:
             return False
 
 
-    def add_used(self, doc_id, usedtime):
+    def add_used(self, doc_id, period, dt):
         self.item_hsh = self.db.get(doc_id=doc_id)
         self.doc_id = doc_id
         self.created = self.item_hsh['created']
-        ut = [x.strip() for x in usedtime.split(': ')]
-        if len(ut) != 2:
-            return False
-
-        per_ok, per = parse_duration(ut[0])
-        if not per_ok:
-            return False
-        dt_ok, dt, z = parse_datetime(ut[1])
-        if not dt_ok:
-            return False
+        # ut = [x.strip() for x in usedtime.split(': ')]
+        # if len(ut) != 2:
+        #     return False, f"The entry '{usedtime}' is invalid"
+
+        # per_ok, per = parse_duration(ut[0])
+        # if not per_ok:
+        #     return False, f"The entry '{ut[0]}' is not a valid period"
+        # dt_ok, dt, z = parse_datetime(ut[1])
+        # if not dt_ok:
+        #     return False, f"The entry '{ut[1]}' is not a valid datetime"
 
         used_times = self.item_hsh.get("u", [])
-        used_times.append([per, dt])
+        used_times.append([period, dt])
         self.item_hsh['u'] = used_times
         self.item_hsh['created'] = self.created
         self.item_hsh['modified'] = pendulum.now('local')
         # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
         self.do_update()
 
-        return True
+        return True, ""
 
 
 
     def schedule_new(self, doc_id, new_dt):
         self.item_hsh = self.db.get(doc_id=doc_id)
         self.doc_id = doc_id
         self.created = self.item_hsh['created']
@@ -2043,25 +2043,25 @@
 class NDict(dict):
     """
     Constructed from rows of (path, values) tuples. The path will be split using 'split_char' to produce the nodes leading to 'values'. The last element in values is presumed to be the 'id' of the item that generated the row.
     """
 
     tab = 2
 
-    def __init__(self, split_char='/', compact=False):
+    def __init__(self, split_char='/', compact=False, width=None):
+        self.compact = compact
+        self.width = width if width else shutil.get_terminal_size()[0]-2
         self.split_char = split_char
-        self.width = shutil.get_terminal_size()[0]-2
         self.row = 0
-        self.compact = compact
         self.row2id = {}
         self.output = []
         self.flag_len = 4 # gkptp
 
     def __missing__(self, key):
-        self[key] = NDict()
+        self[key] = NDict(compact=self.compact, width=self.width)
         return self[key]
 
     def as_dict(self):
         return self
 
     def leaf_detail(self, detail, depth):
         dindent = NDict.tab * (depth + 1) * " "
@@ -2096,15 +2096,15 @@
                 self = self[key]
             elif keys_left:
                 self.setdefault("/".join(keys[j:]), []).append(values)
                 break
 
     def as_tree(self, t={}, depth = 0, level=0):
         """ return an indented tree """
-        self.width = shutil.get_terminal_size()[0]-2
+        # self.width = shutil.get_terminal_size()[0]-2
         for k in t.keys():
             indent = NDict.tab * depth * " "
             # replace any newlines in the title with spaces
             K = re.sub(' *\n+ *', ' ', k)
             self.output.append(f"{indent}{K}")
             self.row += 1
             depth += 1
@@ -2188,14 +2188,15 @@
         self.report_view = ""
         self.report_text = ""
         self.report_items = []
         self.cal_locale = None
         self.history_view = ""
         self.cache = {}
         self.itemcache = {}
+        self.current_hsh = {}
         self.used_summary = {}
         self.used_details = {}
         self.used_details2id = {}
         self.effort_details = {}
         self.currMonth()
         self.completions = []
         self.konnections_from = {}
@@ -2272,19 +2273,24 @@
     def set_etmdir(self, etmdir):
         self.etmdir = etmdir
         self.backupdir = os.path.join(self.etmdir, 'backups')
         # need these files for backups
         self.dbfile = os.path.normpath(os.path.join(etmdir, 'etm.json'))
         self.cfgfile = os.path.normpath(os.path.join(etmdir, 'cfg.yaml'))
         self.settings = settings
-        if 'keep_current' in self.settings and self.settings['keep_current']:
+        # if 'keep_current' in self.settings and self.settings['keep_current']:
+        if 'keep_current' in self.settings and self.settings['keep_current'][0]:
+            # weeks is not zero
+            self.mk_current = True
             self.currfile = os.path.normpath(os.path.join(etmdir, 'current.txt'))
         else:
             self.currfile = None
+            self.mk_current = False
         if 'keep_next' in self.settings and self.settings['keep_next']:
+            # keep_next is true
             self.nextfile = os.path.normpath(os.path.join(etmdir, 'next.txt'))
         else:
             self.nextfile = None
 
         if 'locale' in self.settings:
             locale_str = settings['locale']
             # locale_str should have the format "en_US"
@@ -2799,30 +2805,30 @@
         self.agenda_view, self.done_view, self.engaged_view, self.busy_view, self.row2id, self.done2id, self.engaged2id, self.busy_details = self.cache[self.activeYrWk]
 
 
     def refreshCurrent(self):
         """
         Agenda for the current and following 'keep_current' weeks
         """
-        if self.currfile is not None:
+        if self.mk_current and self.currfile is not None:
             weeks = []
             self.set_now()
             curr_lines = []
             this_week = getWeekNum(self.now)
             num_weeks = self.settings['keep_current'][0]
             for _ in range(num_weeks):
                 # weeks corresponding to 0, ..., num_weeks-1
                 weeks.append(this_week)
                 this_week = nextWeek(this_week)
 
-            tmp_cache = self.cache
+            # tmp_cache = self.cache
             for week in weeks:
-                if week in self.cache:
+                if week in current_hsh:
                     # append the agenda component
-                    curr_lines.append(self.cache[week][0])
+                    curr_lines.append(current_hsh[week])
                 else:
                     logger.debug(f"week {week} missing from cache")
             if curr_lines:
                 with open(self.currfile, 'w', encoding='utf-8') as fo:
                     fo.write("\n\n".join([x.strip() for x in curr_lines]))
                 logger.info(f"saved {len(curr_lines)} weeks from current schedule to {self.currfile}")
             else:
@@ -5600,14 +5606,19 @@
                         # td > 0m => earlier than startdt; dt < 0m => later than startdt
                         possible_alerts.append([td, cmd])
 
             # this catches all alerts and beginbys for the item
             if all_tds:
                 instance_interval = [today + min(all_tds), tomorrow + max(all_tds)]
 
+            # FIXME
+            # r and +      :
+            # r but not +  :
+            # + but not r  :
+
             if 'r' in item or '+' in item:
                 lofh = item.get('r', [])
                 rset = rruleset()
 
                 for hsh in lofh:
                     freq, kwd = rrule_args(hsh)
                     kwd['dtstart'] = dtstart
@@ -5618,22 +5629,34 @@
                         print('  ', freq, kwd)
                         print(e)
                         print(item)
                         break
 
                 if '-' in item:
                     for dt in item['-']:
-                        if type(dt) == pendulum.Date:
-                            dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
+                        dt = date_to_datetime(dt)
+                        # if type(dt) == pendulum.Date:
+                        #     dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
                         rset.exdate(dt)
 
                 if '+' in item:
+                    # tmp = [dtstart]
+                    # tmp.extend(item['+'])
+                    # tmp = [date_to_datetime(x) for x in tmp]
+                    # tmp.sort()
+                    # aft = [x for x in tmp if x >= today]
+                    # bef = [x for x in tmp if x < today]
+                    # if aft:
+                    #     relevant = aft[0]
+                    # else:
+                    #     relevant = bef[-1]
                     for dt in item['+']:
-                        if type(dt) == pendulum.Date:
-                            dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
+                        dt = date_to_datetime(dt)
+                        # if type(dt) == pendulum.Date:
+                        #     dt = pendulum.datetime(year=dt.year, month=dt.month, day=dt.day, hour=0, minute=0, tz='local')
                         rset.rdate(dt)
 
                 if item['itemtype'] == '-':
                     switch = item.get('o', 'k')
                     relevant = rset.after(today, inc=True)
                     if switch == 's':
                         if relevant and item['s'] != pendulum.instance(relevant):
@@ -6656,24 +6679,34 @@
     return ret
 
 def wkday2row(wkday):
     # week day number in 1, ..., 7 to row number in busy view
     # 1 -> 5, ..., 6 -> 15, 0 -> 17  (pendulum thinks Sunday is first)
     return 3+ 2*wkday if wkday else 17
 
-def schedule(db, yw=getWeekNum(), current=[], now=pendulum.now(), weeks_before=0, weeks_after=0, pinned_list=[], link_list=[], konnect_list=[], timers={}, mk_current=False):
+def schedule(db, yw=getWeekNum(), current=[], now=pendulum.now(), weeks_before=0, weeks_after=0, pinned_list=[], link_list=[], konnect_list=[], timers={}):
+    global current_hsh
     wkday_fmt = "ddd D MMM" if settings['dayfirst'] else "ddd MMM D"
     timer_schedule = TimeIt('***SCHEDULE***')
-    if mk_current:
-        weeks_after = settings['keep_current'][0]
-        width = settings['keep_current'][1]-1
-        compact = True
-    else:
-        width = shutil.get_terminal_size()[0]-3
-        compact = False
+    #
+
+    width = shutil.get_terminal_size()[0]-3
+    compact = False
+    weeks_after = settings['keep_current'][0]
+    mk_current = weeks_after > 0
+    current_width = settings['keep_current'][1] - 1
+    current_hsh = {}
+
+    # if weeks_after > 0:
+    #     width = settings['keep_current'][1]-1
+    #     compact = True
+    # else:
+    #     width = shutil.get_terminal_size()[0]-3
+    #     compact = False
+
     ampm = settings['ampm']
     omit = settings['omit_extent']
     UT_MIN = settings.get('usedtime_minutes', 1)
     # yw will be the active week, but now will be the current moment
     LL = {}
     for hour in range(24):
         if hour % 6 == 0:
@@ -6691,18 +6724,16 @@
         else:
             LL[hour] = ' '.rjust(6, ' ')
 
     # xx:xxam-xx:xxpm
     rhc_width = 15 if ampm else 11
     flag_width = 6
     indent_to_summary = 6
-    if mk_current:
-        summary_width = width - indent_to_summary - rhc_width
-    else:
-        summary_width = width - indent_to_summary - flag_width - rhc_width
+    current_summary_width = current_width - indent_to_summary - rhc_width
+    summary_width = width - indent_to_summary - flag_width - rhc_width
 
     d = iso_to_gregorian((yw[0], yw[1], 1))
     dt = pendulum.datetime(d.year, d.month, d.day, 0, 0, 0, tz='local')
     week_numbers = getWeekNumbers(dt, weeks_before, weeks_after)
     if yw not in week_numbers:
         week_numbers.append(yw)
         week_numbers.sort()
@@ -7125,15 +7156,15 @@
                 week2day2heading[week][row] = lst.pop(0)
                 day_ = row
                 allday_details[week][row] = f"\n  ".join([f"{x}" for x in lst])
 
     for week, items in groupby(rows, key=itemgetter('week')):
         weeks.add(week)
         week2day2heading.setdefault(week, {})
-        rdict = NDict(compact=compact)
+        rdict = NDict(compact=False)
         busy_details.setdefault(week, {})
         wk_fmt = fmt_week(week).center(width, ' ').rstrip()
         for row in items:
             doc_id = row['id']
             day_ = row['day'][0]
             dayofweek = row.get('dayofweek', 1)
             if day_ == today:
@@ -7155,25 +7186,56 @@
                     busy_row = f"{values[0]} {summary} {wrapped:^15}".rstrip()
                     if settings['connecting_dots']:
                         busy_row = f"  {busy_row}".replace('   ', LINEDOT)
 
                     busy_details[week].setdefault(row, [f"Busy"]).append(
                             busy_row
                             )
-
             rdict.add(path, values)
-
         for d, v in busy_details[week].items():
             busy_details[week][d] = "\n".join([x.rstrip() for x in v])
 
 
         tree, row2id = rdict.as_tree(rdict, level=0)
         agenda_hsh[week] = tree
         row2id_hsh[week] = row2id
 
+    if mk_current:
+        cweeks = set([])
+        for week, items in groupby(rows, key=itemgetter('week')):
+            cweeks.add(week)
+            week2day2heading.setdefault(week, {})
+            cdict = NDict(compact=True, width=settings['keep_current'][1])
+            wk_fmt = fmt_week(week).center(width, ' ').rstrip()
+            for row in items:
+                doc_id = row['id']
+                day_ = row['day'][0]
+                dayofweek = row.get('dayofweek', 1)
+                if day_ == today:
+                    day_ += " (Today)"
+                elif day_ == tomorrow:
+                    day_ += " (Tomorrow)"
+                path = f"{wk_fmt}/{day_}"
+                values = row['columns']
+                # heading = f"Busy periods for {day_}"
+                if values[0] in ["*", "-"]:
+                    values[1] = re.sub(' *\n+ *', ' ', values[1])
+                    # busyperiod = row.get('busyperiod', "")
+                    # if busyperiod:
+                    #     wrap = row.get('wrap', [])
+                    #     wrapped = row.get('wrapped', "")
+                    #     row = wkday2row(dayofweek)
+                    #     week2day2heading[week][row] = day_
+                    #     summary = values[1].ljust(current_summary_width-20, ' ')
+                    #     busy_row = f"{values[0]} {summary} {wrapped:^15}".rstrip()
+                cdict.add(path, values)
+
+            ctree, crow2id = cdict.as_tree(cdict, level=0)
+            current_hsh[week] = ctree
+
     busyday_details = {}
     for week in allday_details:
         busyday_details.setdefault(week, {})
         for day in allday_details[week]:
             busyday_details[week].setdefault(day, []).append(allday_details[week][day])
     for week in busy_details:
         busyday_details.setdefault(week, {})
```

### Comparing `etm-dgraham-5.0.6/etm/options.py` & `etm-dgraham-5.0.7/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/report.py` & `etm-dgraham-5.0.7/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm/view.py` & `etm-dgraham-5.0.7/etm/view.py`

 * *Files 2% similar despite different names*

```diff
@@ -941,29 +941,48 @@
             label_text=f"selected:\n  {hsh['itemtype']} {hsh['summary']}\n  @i {hsh.get('i', '~')}{timer}\n\nused time format:\n    period: datetime\n",
             default=entry,
             )
         usedtime = yield from show_dialog_as_float(dialog)
 
         if not usedtime:
             # None (cancelled) or null string
-            return
+            return None
 
-        changed = item.add_used(doc_id, usedtime)
+        msg = []
+        ut = [x.strip() for x in usedtime.split(': ')]
+        if len(ut) != 2:
+            ok = False
+            msg.append(f"The entry '{usedtime}' is invalid")
 
+        else:
+            ok, per = model.parse_duration(ut[0])
+            if not ok:
+                msg.append(f"The entry '{ut[0]}' is not a valid period")
+
+            ok, dt, z = model.parse_datetime(ut[1])
+            if not ok:
+                msg.append(f"The entry '{ut[1]}' is not a valid datetime"
+                           )
+        if msg:
+            msg = "\n   ".join(msg)
+            show_message('add used time', f"Cancelled,\n   {msg}")
+            return
+
+        changed, msg = item.add_used(doc_id, per, dt)
         if changed:
             dataview.timer_clear(doc_id)
 
             if doc_id in dataview.itemcache:
                 del dataview.itemcache[doc_id]
             application.layout.focus(text_area)
             set_text(dataview.show_active_view())
             loop = asyncio.get_event_loop()
             loop.call_later(0, data_changed, loop)
         else:
-            show_message('add used time', f"Cancelled, '{usedtime}' is invalid.\nThe required entry format is:\n   period: datetime")
+            show_message('add used time', f"Cancelled, {msg}")
 
 
     asyncio.ensure_future(coroutine())
 
 
 today = pendulum.today()
 calyear = today.year
@@ -2384,15 +2403,16 @@
            return
         if file_path.strip().lower() == 'lorem':
             logger.debug(f"calling import_file")
             ok, msg = import_file('lorem')
             if ok:
                 dataview.refreshRelevant()
                 dataview.refreshAgenda()
-                dataview.refreshCurrent()
+                if dataview.mk_current:
+                    dataview.refreshCurrent()
                 dataview.refreshKonnections()
                 loop = asyncio.get_event_loop()
                 loop.call_later(0, data_changed, loop)
             show_message('import lorem', msg)
 
         else:
             if file_path:
@@ -2403,15 +2423,16 @@
 
                     if os.path.dirname(file_path) == etm_dir:
                         os.remove(file_path)
                         filehome = os.path.join("~", os.path.split(file_path)[1])
                         msg += f"\n and removed {filehome}"
                     dataview.refreshRelevant()
                     dataview.refreshAgenda()
-                    dataview.refreshCurrent()
+                    if dataview.mk_current:
+                        dataview.refreshCurrent()
                     dataview.refreshKonnections()
                     loop = asyncio.get_event_loop()
                     loop.call_later(0, data_changed, loop)
                 show_message('import file', msg)
 
     asyncio.ensure_future(coroutine())
```

### Comparing `etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 5.0.6
+Version: 5.0.7
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-5.0.6/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-5.0.7/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-5.0.7/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etmlogo.png` & `etm-dgraham-5.0.7/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etmlogo_small.png` & `etm-dgraham-5.0.7/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/etmview_agenda.png` & `etm-dgraham-5.0.7/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/namedcolors.py` & `etm-dgraham-5.0.7/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/new.png` & `etm-dgraham-5.0.7/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/setup.py` & `etm-dgraham-5.0.7/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/test/test_parser.py` & `etm-dgraham-5.0.7/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/utilities/colons_to_slashes.py` & `etm-dgraham-5.0.7/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/utilities/etm_in` & `etm-dgraham-5.0.7/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/utilities/inbasket` & `etm-dgraham-5.0.7/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-5.0.6/utilities/open_in_mutt` & `etm-dgraham-5.0.7/utilities/open_in_mutt`

 * *Files identical despite different names*

