# Comparing `tmp/awstuff-0.111.tar.gz` & `tmp/awstuff-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "awstuff-0.111.tar", last modified: Wed May 17 19:21:09 2023, max compression
+gzip compressed data, was "awstuff-0.2.tar", last modified: Thu Jun  8 18:07:19 2023, max compression
```

## Comparing `awstuff-0.111.tar` & `awstuff-0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-05-17 19:21:09.035664 awstuff-0.111/
--rw-rw-rw-   0        0        0      238 2023-05-17 19:21:09.035664 awstuff-0.111/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-17 19:21:09.015665 awstuff-0.111/awstuff/
--rw-rw-rw-   0        0        0     3459 2023-05-17 19:14:46.000000 awstuff-0.111/awstuff/Functions.py
--rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.111/awstuff/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-17 19:21:09.034663 awstuff-0.111/awstuff.egg-info/
--rw-rw-rw-   0        0        0      238 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      213 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-17 00:31:25.000000 awstuff-0.111/awstuff.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        8 2023-05-17 19:21:08.000000 awstuff-0.111/awstuff.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-17 19:21:09.040666 awstuff-0.111/setup.cfg
--rw-rw-rw-   0        0        0      257 2023-05-17 19:21:02.000000 awstuff-0.111/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:07:19.175033 awstuff-0.2/
+-rw-rw-rw-   0        0        0      236 2023-06-08 18:07:19.175033 awstuff-0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 18:07:19.162997 awstuff-0.2/awstuff/
+-rw-rw-rw-   0        0        0    11817 2023-06-08 17:36:20.000000 awstuff-0.2/awstuff/Functions.py
+-rw-rw-rw-   0        0        0       33 2023-05-17 00:29:39.000000 awstuff-0.2/awstuff/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 18:07:19.174032 awstuff-0.2/awstuff.egg-info/
+-rw-rw-rw-   0        0        0      236 2023-06-08 18:07:19.000000 awstuff-0.2/awstuff.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      213 2023-06-08 18:07:19.000000 awstuff-0.2/awstuff.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 18:07:19.000000 awstuff-0.2/awstuff.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-05-11 16:50:18.000000 awstuff-0.2/awstuff.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        8 2023-06-08 18:07:19.000000 awstuff-0.2/awstuff.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 18:07:19.176034 awstuff-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      255 2023-06-08 18:05:15.000000 awstuff-0.2/setup.py
```

