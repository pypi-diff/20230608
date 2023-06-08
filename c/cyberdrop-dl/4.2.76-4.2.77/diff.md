# Comparing `tmp/cyberdrop-dl-4.2.76.tar.gz` & `tmp/cyberdrop-dl-4.2.77.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberdrop-dl-4.2.76.tar", last modified: Thu Jun  8 00:42:47 2023, max compression
+gzip compressed data, was "cyberdrop-dl-4.2.77.tar", last modified: Thu Jun  8 03:09:50 2023, max compression
```

## Comparing `cyberdrop-dl-4.2.76.tar` & `cyberdrop-dl-4.2.77.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.470865 cyberdrop-dl-4.2.76/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 00:42:47.470865 cyberdrop-dl-4.2.76/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.466865 cyberdrop-dl-4.2.76/cyberdrop_dl/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.466865 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/base_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/config_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/error_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/sorting_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/sql_helper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.466865 cyberdrop-dl-4.2.76/cyberdrop_dl/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.470865 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Anonfiles_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     8128 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Bunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Coomeno_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/CyberFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/EHentai_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Erome_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Fapello_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Gfycat_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/GoFile_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/HGameCG_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/ImgBox_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/LoveFap_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/PixelDrain_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/PostImg_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Saint_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/ShareX_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/XBunkr_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Xenforo_Spider.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.470865 cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/downloader_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20925 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/old_downloaders.py
--rw-r--r--   0 runner    (1001) docker     (123)    18641 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/progress_definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    22124 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.470865 cyberdrop-dl-4.2.76/cyberdrop_dl/scraper/
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/scraper/JDownloader_Integration.py
--rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/scraper/Scraper.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/cyberdrop_dl/scraper/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:42:47.466865 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 00:42:47.000000 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-08 00:42:47.000000 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:42:47.000000 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 00:42:47.000000 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 00:42:47.000000 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 00:42:47.000000 cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-08 00:42:47.470865 cyberdrop-dl-4.2.76/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:42:38.000000 cyberdrop-dl-4.2.76/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.513206 cyberdrop-dl-4.2.77/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 03:09:50.513206 cyberdrop-dl-4.2.77/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.509206 cyberdrop-dl-4.2.77/cyberdrop_dl/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.509206 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/base_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3033 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/config_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/error_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/sorting_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/sql_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.509206 cyberdrop-dl-4.2.77/cyberdrop_dl/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9967 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.513206 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Anonfiles_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8221 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Bunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Coomeno_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12903 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/CyberFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3042 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Cyberdrop_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3089 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/EHentai_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4239 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Erome_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Fapello_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Gfycat_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5940 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/GoFile_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/HGameCG_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/ImgBox_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3676 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/LoveFap_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4454 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/NSFWXXX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2918 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/PimpAndHost_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/PixelDrain_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3008 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/PostImg_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Saint_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9182 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/ShareX_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/XBunkr_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13903 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Xenforo_Spider.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.513206 cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/downloader_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20946 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/old_downloaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18693 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/progress_definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22948 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.513206 cyberdrop-dl-4.2.77/cyberdrop_dl/scraper/
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/scraper/JDownloader_Integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20796 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/scraper/Scraper.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/cyberdrop_dl/scraper/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:09:50.509206 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18708 2023-06-08 03:09:50.000000 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-06-08 03:09:50.000000 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:09:50.000000 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 03:09:50.000000 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-08 03:09:50.000000 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 03:09:50.000000 cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-08 03:09:50.517207 cyberdrop-dl-4.2.77/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 03:09:40.000000 cyberdrop-dl-4.2.77/setup.py
```

### Comparing `cyberdrop-dl-4.2.76/LICENSE` & `cyberdrop-dl-4.2.77/LICENSE`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/PKG-INFO` & `cyberdrop-dl-4.2.77/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.76
+Version: 4.2.77
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.76 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.77 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.76/README.md` & `cyberdrop-dl-4.2.77/README.md`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/base_functions.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/base_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/config_manager.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/config_manager.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/config_schema.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/config_schema.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/data_classes.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/data_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/error_classes.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/error_classes.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/sorting_functions.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/sorting_functions.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/base_functions/sql_helper.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/base_functions/sql_helper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/client/client.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/client/client.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Anonfiles_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Anonfiles_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Bunkr_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Bunkr_Spider.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,27 @@
         self.SQL_Helper = SQL_Helper
         self.remove_bunkr_id = remove_bunkr_id
         self.limiter = AsyncLimiter(20, 1)
 
         self.error_writer = error_writer
 
     async def get_stream_link(self, url: URL):
-        cdn_possibilities = r"(?:cdn.bunkr...|cdn..bunkr...|cdn...bunkr...|media-files.bunkr...|media-files..bunkr...|media-files...bunkr...)"
+        cdn_possibilities = r"(?:cdn.bunkrr...|media-files.bunkrr...|media-files..bunkrr...|media-files...bunkrr...|cdn.bunkr...|cdn..bunkr...|cdn...bunkr...|media-files.bunkr...|media-files..bunkr...|media-files...bunkr...)"
         ext = '.' + url.parts[-1].split('.')[-1]
         if ext:
             ext = ext.lower()
         else:
             return url
 
         if ext in FILE_FORMATS['Images']:
             url = URL(str(url).replace("https://cdn", "https://i"))
         elif ext in FILE_FORMATS['Videos']:
-            url = URL(re.sub(cdn_possibilities, "bunkr.la/v", str(url)))
+            url = URL(re.sub(cdn_possibilities, "bunkrr.su/v", str(url)))
         else:
-            url = URL(re.sub(cdn_possibilities, "bunkr.la/d", str(url)))
+            url = URL(re.sub(cdn_possibilities, "bunkrr.su/d", str(url)))
         return url
 
     async def fetch(self, session: ScrapeSession, url: URL) -> AlbumItem:
         """Scraper for Bunkr"""
         album_obj = AlbumItem("Loose Bunkr Files", [])
         log(f"Starting: {url}", quiet=self.quiet, style="green")
 
@@ -109,15 +109,15 @@
             url = url.with_host(url_host)
         return url
 
     async def get_file(self, session: ScrapeSession, url: URL):
         """Gets the media item from the supplied url"""
 
         ### Temp Fix ###
-        url = url.with_host("bunkr.la")
+        url = url.with_host("bunkrr.su")
 
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             head = soup.select_one("head")
             scripts = head.select('script[type="text/javascript"]')
             link = None
@@ -139,23 +139,23 @@
             await self.SQL_Helper.fix_bunkr_entries(link, original_filename)
             complete = await self.SQL_Helper.check_complete_singular("bunkr", link)
             return MediaItem(link, url, complete, filename, ext, original_filename)
 
         except Exception as e:
             logger.debug("Error encountered while handling %s", url, exc_info=True)
             log(f"Error: {url}", quiet=self.quiet, style="red")
-            await self.error_writer.write_errored_scrape(f"{url},{e}")
+            await self.error_writer.write_errored_scrape(url, e, self.quiet)
             logger.debug(e)
             return MediaItem(url, url, False, "", "", "")
 
     async def get_album(self, session: ScrapeSession, url: URL):
         """Iterates through an album and creates the media items"""
 
         ### Temp Fix ###
-        url = url.with_host("bunkr.la")
+        url = url.with_host("bunkrr.su")
 
         album = AlbumItem(url.name, [])
         try:
             async with self.limiter:
                 soup = await session.get_BS4(url)
             title = soup.select_one('h1[class="text-[24px] font-bold text-dark dark:text-white"]')
             for elem in title.find_all("span"):
```

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Coomeno_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Coomeno_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/CyberFile_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/CyberFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Cyberdrop_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Cyberdrop_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/EHentai_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/EHentai_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Erome_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Erome_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Fapello_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Fapello_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Gfycat_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Gfycat_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/GoFile_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/GoFile_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/HGameCG_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/HGameCG_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/ImgBox_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/ImgBox_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/LoveFap_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/LoveFap_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/NSFWXXX_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/NSFWXXX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/PimpAndHost_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/PimpAndHost_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/PixelDrain_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/PixelDrain_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/PostImg_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/PostImg_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Saint_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Saint_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/ShareX_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/ShareX_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/XBunkr_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/XBunkr_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/crawlers/Xenforo_Spider.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/crawlers/Xenforo_Spider.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/downloader_utils.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/downloader_utils.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/downloaders.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/downloaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,19 @@
 
         self.download_session = DownloadSession(CDL_Helper.client)
 
         self.CDL_Helper = CDL_Helper
         self.Progress_Master = Progress_Master
 
     async def download(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
-        async with self._semaphore:
-            await self.download_file(album, media, url_path, album_task)
+        try:
+            async with self._semaphore:
+                await self.download_file(album, media, url_path, album_task)
+        except RuntimeError as e:
+            return
 
     @retry
     async def download_file(self, album: str, media: MediaItem, url_path: str, album_task: TaskID) -> None:
         """File downloader"""
         if not await check_free_space(self.CDL_Helper.required_free_space, self.CDL_Helper.download_dir):
             log("We've run out of free space.", quiet=True)
             await self.CDL_Helper.files.add_skipped()
@@ -246,16 +249,15 @@
         except (aiohttp.client_exceptions.ClientPayloadError, aiohttp.client_exceptions.ClientOSError,
                 aiohttp.client_exceptions.ServerDisconnectedError, asyncio.TimeoutError,
                 aiohttp.client_exceptions.ClientResponseError, aiohttp.client_exceptions.ServerTimeoutError,
                 DownloadFailure, FileNotFoundError, PermissionError) as e:
             if await self.CDL_Helper.File_Lock.check_lock(filename):
                 await self.CDL_Helper.File_Lock.remove_lock(filename)
 
-            with contextlib.suppress(Exception):
-                await self.Progress_Master.FileProgress.remove_file(file_task)
+            await self.Progress_Master.FileProgress.remove_file(file_task)
 
             if hasattr(e, "message"):
                 logging.debug(f"\n{media.url} ({e.message})")
 
             if hasattr(e, "code"):
                 if await is_4xx_client_error(e.code) and e.code != HTTPStatus.TOO_MANY_REQUESTS:
                     logger.debug("We ran into a 400 level error: %s", e.code)
```

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/old_downloaders.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/old_downloaders.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/downloader/progress_definitions.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/downloader/progress_definitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -332,15 +332,16 @@
     async def update_file_length(self, task_id: TaskID, length: int) -> None:
         await self.progress.update_total(task_id, length)
 
     async def advance_file(self, task_id: TaskID, increment: int) -> None:
         await self.progress.advance_task(task_id, increment)
 
     async def remove_file(self, task_id: TaskID) -> None:
-        await self.progress.remove_task(task_id)
+        if task_id in self.file_progress.tasks:
+            await self.progress.remove_task(task_id)
         await self.progress.redraw()
 
     async def mark_file_completed(self, task_id: TaskID) -> None:
         await self.progress.mark_task_completed(task_id)
         await self.progress.redraw()
```

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/main.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 import argparse
 import asyncio
+import atexit
 import contextlib
 import logging
 import re
 from pathlib import Path
 from typing import Dict, List
 
 import aiofiles
+import aiorun as aiorun
 from yarl import URL
 
 from cyberdrop_dl.base_functions.base_functions import ErrorFileWriter, clear, log, purge_dir
 from cyberdrop_dl.base_functions.config_manager import document_args, run_args
 from cyberdrop_dl.base_functions.config_schema import config_default
 from cyberdrop_dl.base_functions.sorting_functions import Sorter
 from cyberdrop_dl.base_functions.sql_helper import SQLHelper
-from cyberdrop_dl.client.client import Client
+from cyberdrop_dl.client.client import Client, ScrapeSession
 from cyberdrop_dl.downloader.downloader_utils import check_free_space
 from cyberdrop_dl.downloader.downloaders import DownloadDirector
 from cyberdrop_dl.downloader.old_downloaders import old_download_forums
 from cyberdrop_dl.scraper.Scraper import ScrapeMapper
 
 from . import __version__ as VERSION
 from .base_functions.data_classes import ForumItem, SkipData
@@ -238,14 +240,27 @@
         await Forums.add_thread("Loose Files/Albums", Cascade)
 
     log("", quiet=quiet)
     log("Finished Scrape", quiet=quiet, style="green")
     return Forums
 
 
+async def check_outdated(client: Client):
+    session = ScrapeSession(client)
+    url = URL('https://pypi.python.org/pypi/cyberdrop-dl/json')
+    try:
+        response = await session.get_json(url)
+        if response['info']['version'] != VERSION:
+            log(f"\nYour version of Cyberdrop Downloader is outdated. \nYou are running version {VERSION}."
+                f"\nPlease update to version {response['info']['version']}"
+                f"\nYou can find out how to do that here: https://github.com/Jules-WinnfieldX/CyberDropDownloader/wiki/Frequently-Asked-Questions#how-to-update", style="red")
+    except Exception as e:
+        pass
+
+
 async def director(args: Dict, links: List) -> None:
     """This is the overarching director coordinator for CDL."""
     await clear()
     await document_args(args)
     log(f"We are running version {VERSION} of Cyberdrop Downloader")
     error_writer = await file_management(args, links)
 
@@ -294,34 +309,37 @@
             if partial_downloads:
                 log('There are partial downloads in the downloads folder.', style="yellow")
             if temp_downloads:
                 log('There are partial downloads from this run, please re-run the program.', style="yellow")
 
         log('Finished downloading. Enjoy :)')
 
-    log('')
-    log("If you enjoy using this program, please consider buying the developer a coffee :)\nhttps://www.buymeacoffee.com/juleswinnft", style="green")
+    await check_outdated(client)
+    log("\nIf you enjoy using this program, please consider buying the developer a coffee :)"
+        "\nhttps://www.buymeacoffee.com/juleswinnft", style="green")
+    asyncio.get_event_loop().stop()
 
 
 def main(args=None):
     if not args:
         args = parse_args()
 
+    atexit.register(lambda: print("\x1b[?25h"))
+
     links = args.links
     args = run_args(args.config_file, argparse.Namespace(**vars(args)).__dict__)
 
     logging.basicConfig(
         filename=args["Files"]["log_file"],
         level=logging.DEBUG,
         format="%(asctime)s:%(levelname)s:%(module)s:%(filename)s:%(lineno)d:%(message)s",
         filemode="w"
     )
 
-    with contextlib.suppress(RuntimeError):
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(director(args, links))
+    with contextlib.suppress(RuntimeError, asyncio.CancelledError):
+        aiorun.run(director(args, links), stop_on_unhandled_errors=True)
 
 
 if __name__ == '__main__':
     print("""STOP! If you're just trying to download files, check the README.md file for instructions.
     If you're developing this project, use start.py instead.""")
     exit()
```

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/scraper/JDownloader_Integration.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/scraper/JDownloader_Integration.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl/scraper/Scraper.py` & `cyberdrop-dl-4.2.77/cyberdrop_dl/scraper/Scraper.py`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/PKG-INFO` & `cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyberdrop-dl
-Version: 4.2.76
+Version: 4.2.77
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
-Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.76 Summary: Bulk
+Metadata-Version: 2.1 Name: cyberdrop-dl Version: 4.2.77 Summary: Bulk
 downloader for multiple file hosts and forum sites Home-page: https://
 github.com/Jules-WinnfieldX/CyberDropDownloader Author: Jules-WinnfieldX
 Author-email: JulesWinnfieldII@protonmail.com Project-URL: Bug Tracker, https:/
 /github.com/Jules-WinnfieldX/CyberDropDownloader/issues Requires-Python: >=3.7
 Description-Content-Type: text/markdown License-File: LICENSE # `cyberdrop-dl`
 **Bulk downloader for multiple file hosts** [![PyPI version](https://
 badge.fury.io/py/cyberdrop-dl.svg)](https://badge.fury.io/py/cyberdrop-dl) [!
```

### Comparing `cyberdrop-dl-4.2.76/cyberdrop_dl.egg-info/SOURCES.txt` & `cyberdrop-dl-4.2.77/cyberdrop_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cyberdrop-dl-4.2.76/setup.cfg` & `cyberdrop-dl-4.2.77/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 python_requires = >=3.7
 include_package_data = True
 packages = find:
 install_requires = 
 	aiofiles>=23.1.0
 	aiohttp>=3.8.4
 	aiolimiter>=1.1.0
+	aiorun>=2022.11.1
 	beautifulsoup4>=4.12.2
 	certifi>=2023.5.7
 	myjdapi>=1.1.6
 	PyYAML>=6.0
 	rich>=13.3.5
 	setuptools>=67.8.0
 	tqdm>=4.65.0
```

