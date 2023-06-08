# Comparing `tmp/scorecovid-0.0.8.tar.gz` & `tmp/scorecovid-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scorecovid-0.0.8.tar", last modified: Mon Jun 21 06:54:15 2021, max compression
+gzip compressed data, was "scorecovid-0.0.9.tar", last modified: Thu Jun  8 10:14:51 2023, max compression
```

## Comparing `scorecovid-0.0.8.tar` & `scorecovid-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-21 06:54:15.761425 scorecovid-0.0.8/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4002 2021-06-21 06:54:15.759936 scorecovid-0.0.8/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     3452 2021-06-13 12:59:26.000000 scorecovid-0.0.8/README.md
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       38 2021-06-21 06:54:15.761425 scorecovid-0.0.8/setup.cfg
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      976 2021-06-21 02:55:10.000000 scorecovid-0.0.8/setup.py
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-21 06:54:15.740566 scorecovid-0.0.8/src/
-drwxr-xr-x   0 takefuji  (1000) takefuji  (1000)        0 2021-06-21 06:54:15.758510 scorecovid-0.0.8/src/scorecovid.egg-info/
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     4002 2021-06-21 06:54:15.000000 scorecovid-0.0.8/src/scorecovid.egg-info/PKG-INFO
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)      229 2021-06-21 06:54:15.000000 scorecovid-0.0.8/src/scorecovid.egg-info/SOURCES.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)        1 2021-06-21 06:54:15.000000 scorecovid-0.0.8/src/scorecovid.egg-info/dependency_links.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       48 2021-06-21 06:54:15.000000 scorecovid-0.0.8/src/scorecovid.egg-info/entry_points.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)       11 2021-06-21 06:54:15.000000 scorecovid-0.0.8/src/scorecovid.egg-info/top_level.txt
--rw-r--r--   0 takefuji  (1000) takefuji  (1000)     2253 2021-06-21 06:54:11.000000 scorecovid-0.0.8/src/scorecovid.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-08 10:14:51.505041 scorecovid-0.0.9/
+-rw-r--r--   0 yt        (1000) yt        (1000)     6281 2023-06-08 10:14:51.505041 scorecovid-0.0.9/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)     5731 2023-06-08 10:13:37.000000 scorecovid-0.0.9/README.md
+-rw-r--r--   0 yt        (1000) yt        (1000)       38 2023-06-08 10:14:51.505041 scorecovid-0.0.9/setup.cfg
+-rw-r--r--   0 yt        (1000) yt        (1000)      976 2023-06-08 07:40:32.000000 scorecovid-0.0.9/setup.py
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-08 10:14:51.489407 scorecovid-0.0.9/src/
+drwxr-xr-x   0 yt        (1000) yt        (1000)        0 2023-06-08 10:14:51.505041 scorecovid-0.0.9/src/scorecovid.egg-info/
+-rw-r--r--   0 yt        (1000) yt        (1000)     6281 2023-06-08 10:14:50.000000 scorecovid-0.0.9/src/scorecovid.egg-info/PKG-INFO
+-rw-r--r--   0 yt        (1000) yt        (1000)      229 2023-06-08 10:14:50.000000 scorecovid-0.0.9/src/scorecovid.egg-info/SOURCES.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)        1 2023-06-08 10:14:50.000000 scorecovid-0.0.9/src/scorecovid.egg-info/dependency_links.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       48 2023-06-08 10:14:50.000000 scorecovid-0.0.9/src/scorecovid.egg-info/entry_points.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)       11 2023-06-08 10:14:50.000000 scorecovid-0.0.9/src/scorecovid.egg-info/top_level.txt
+-rw-r--r--   0 yt        (1000) yt        (1000)     1906 2023-06-08 09:55:52.000000 scorecovid-0.0.9/src/scorecovid.py
```

### Comparing `scorecovid-0.0.8/setup.py` & `scorecovid-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="scorecovid",
-    version="0.0.8",
+    version="0.0.9",
     author="yoshiyasu takefuji",
     author_email="takefuji@keio.jp",
     description="A package for scoring policies of covid-19",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ytakefuji/score-covid-19-policy",
     project_urls={
```

