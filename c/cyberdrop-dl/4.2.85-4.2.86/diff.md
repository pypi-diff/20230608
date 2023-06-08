# Comparing `tmp/cyberdrop-dl-4.2.85.tar.gz` & `tmp/cyberdrop-dl-4.2.86.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.85.tar", last modified: Thu Jun  8 16:16:58 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.86.tar", last modified: Thu Jun  8 16:19:56 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.85.tar` & `cyberdrop-dl-4.2.86.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.828501 cyberdrop-dl-4.2.85/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 16:16:58.828501 cyberdrop-dl-4.2.85/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.820500 cyberdrop-dl-4.2.85/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.824501 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.824501 cyberdrop-dl-4.2.85/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.828501 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.828501 cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22995 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.828501 cyberdrop-dl-4.2.85/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:16:58.820500 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 16:16:58.000000 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-08 16:16:58.000000 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:16:58.000000 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 16:16:58.000000 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-08 16:16:58.000000 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 16:16:58.000000 cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-08 16:16:58.832502 cyberdrop-dl-4.2.85/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:16:45.000000 cyberdrop-dl-4.2.85/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.862835 cyberdrop-dl-4.2.86/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 16:19:56.862835 cyberdrop-dl-4.2.86/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.858835 cyberdrop-dl-4.2.86/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.858835 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7290 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.858835 cyberdrop-dl-4.2.86/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.862835 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.862835 cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20999 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18922 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22995 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.862835 cyberdrop-dl-4.2.86/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:19:56.858835 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 16:19:56.000000 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-08 16:19:56.000000 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:19:56.000000 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 16:19:56.000000 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-08 16:19:56.000000 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 16:19:56.000000 cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-08 16:19:56.866835 cyberdrop-dl-4.2.86/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:19:45.000000 cyberdrop-dl-4.2.86/setup.py
```

### Comparing `cyberdrop-dl-4.2.85/LICENSE` & `cyberdrop-dl-4.2.86/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/PKG-INFO` & `cyberdrop-dl-4.2.86/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.85
+Version: 4.2.86
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.85 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.86 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.85/README.md` & `cyberdrop-dl-4.2.86/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/main.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.86/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.85
+Version: 4.2.86
 Summary: Bulk downloader for multiple file hosts and forum sites
 Home-page: https://github.com/Jules-WinnfieldX/CyberDropDownloader
 Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com
 Project-URL: Bug Tracker, https://github.com/Jules-WinnfieldX/CyberDropDownloader/issues
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.85 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.86 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.85/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.86/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.85/setup.cfg` & `cyberdrop-dl-4.2.86/setup.cfg`

 * *Files identical despite different names*

