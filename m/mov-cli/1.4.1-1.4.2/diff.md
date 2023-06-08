# Comparing `tmp/mov_cli-1.4.1.tar.gz` & `tmp/mov_cli-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.1.tar", max compression
+gzip compressed data, was "mov_cli-1.4.2.tar", max compression
```

## Comparing `mov_cli-1.4.1.tar` & `mov_cli-1.4.2.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    35149 2023-05-23 10:46:55.139511 mov_cli-1.4.1/LICENSE
--rw-r--r--   0        0        0     7098 2023-05-23 10:46:55.139511 mov_cli-1.4.1/README.md
--rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/__init__.py
--rw-r--r--   0        0        0     2701 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2238 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     1483 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2731 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1592 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/player.py
--rw-r--r--   0        0        0      941 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8714 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    11020 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4177 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4112 2023-05-23 10:46:55.143511 mov_cli-1.4.1/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1943 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1724 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     3210 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     7122 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/kinox.py
--rw-r--r--   0        0        0     3736 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     2509 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2563 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4662 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4422 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4121 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1622 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2132 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2895 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4516 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3395 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3983 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3503 2023-05-23 10:46:55.147511 mov_cli-1.4.1/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      743 2023-05-23 10:46:55.147511 mov_cli-1.4.1/pyproject.toml
--rw-r--r--   0        0        0     8093 1970-01-01 00:00:00.000000 mov_cli-1.4.1/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-08 17:52:38.724717 mov_cli-1.4.2/LICENSE
+-rw-r--r--   0        0        0     7155 2023-06-08 17:52:38.724717 mov_cli-1.4.2/README.md
+-rw-r--r--   0        0        0      235 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/__init__.py
+-rw-r--r--   0        0        0     2700 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     2559 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1483 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/dbs.py
+-rw-r--r--   0        0        0     2731 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0     6133 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/jsunpack.py
+-rw-r--r--   0        0        0     2269 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1592 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/player.py
+-rw-r--r--   0        0        0      941 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/provider.py
+-rw-r--r--   0        0        0     8714 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0        0 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0    11020 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/actvid.py
+-rw-r--r--   0        0        0     4177 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/animefox.py
+-rw-r--r--   0        0        0     4112 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/dopebox.py
+-rw-r--r--   0        0        0     1943 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/einthusan.py
+-rw-r--r--   0        0        0     1724 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/eja.py
+-rw-r--r--   0        0        0     3210 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/gogoanime.py
+-rw-r--r--   0        0        0     7122 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/kinox.py
+-rw-r--r--   0        0        0     3736 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/kisscartoon.py
+-rw-r--r--   0        0        0     2509 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/openloadmov.py
+-rw-r--r--   0        0        0     2563 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/redundant_kimcartoon.py
+-rw-r--r--   0        0        0     4662 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/remotestream.py
+-rw-r--r--   0        0        0     4422 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/scdn.py
+-rw-r--r--   0        0        0     4121 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/sflix.py
+-rw-r--r--   0        0        0     1622 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/solar.py
+-rw-r--r--   0        0        0     2132 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/tamilyogi.py
+-rw-r--r--   0        0        0     2895 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/turkish123.py
+-rw-r--r--   0        0        0     4516 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/viewasian.py
+-rw-r--r--   0        0        0     3395 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/watchasian.py
+-rw-r--r--   0        0        0     3983 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/wlext.py
+-rw-r--r--   0        0        0     3503 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/yoturkish.py
+-rw-r--r--   0        0        0      743 2023-06-08 17:52:38.728717 mov_cli-1.4.2/pyproject.toml
+-rw-r--r--   0        0        0     8150 1970-01-01 00:00:00.000000 mov_cli-1.4.2/PKG-INFO
```

### Comparing `mov_cli-1.4.1/LICENSE` & `mov_cli-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/README.md` & `mov_cli-1.4.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -24,19 +24,19 @@
 [![MIT License][license-shield]][license-url]
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/mov-cli/mov-cli">
-    <img src="https://user-images.githubusercontent.com/83706294/194960059-a9202d72-f033-46b4-b756-3193dc54fb20.png" alt="Logo" width="80" height="80">
+    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="80" height="80">
   </a>
 
   <p align="center">
-    A cli tool to browse and watch movies/shows.
+ A cli tool to browse and watch Movies/Shows/TV/Sports. 
     <br />
     <br />
     <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
     ·
     <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
   </p>
 </div>
@@ -87,16 +87,17 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 
 
 ### Prerequisites
 
-- [`mpv`](https://mpv.io) - Player used for Windows, Linux and Android
+- [`mpv`](https://mpv.io) - player used for Windows, Linux and Android
 - [`iina`](https://iina.io) - player used for MacOS
+- [`Outplayer`](https://outplayer.app/) - player used for iOS
 - [`ffmpeg`](https://github.com/FFmpeg/FFmpeg) - For downloads 
 - [`fzf`](https://github.com/junegunn/fzf) - The selection Menu
 
 
 ## Installation
 <!-- WIN AND LINUX -->
 ### Windows / Linux
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
       [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]]
 [issues-url] [![MIT License][license-shield]][license-url]
                                     [Logo]
-                 A cli tool to browse and watch movies/shows.
+            A cli tool to browse and watch Movies/Shows/TV/Sports.
 
                          Report_Bug Â· Request_Feature
  ### Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Prerequisites
           o Installation
@@ -21,17 +21,18 @@
    9. inspiration
  ## About The Project mov-cli is a Commandline Tool to watch and download shows
 and movies. Shows and Movies are scraped from Streaming Sites. mov-cli
 currently scrapes 15 Providers: ``` Actvid Â· SFlix Â· Solar Â· DopeBox Â·
 WLEXT Â· KinoX Â· StreamBlasters Â· TamilYogi Â· Einthusan Â· ViewAsian Â·
 Watchasian Â· GogoAnime Â· Eja Â· KimCartoon Â· Turkish123 ```
    (back_to_top)!-- GETTING STARTED --> ## Getting Started ### Prerequisites -
-[`mpv`](https://mpv.io) - Player used for Windows, Linux and Android - [`iina`]
-     (https://iina.io) - player used for MacOS - [`ffmpeg`](https://github.com/
-FFmpeg/FFmpeg) - For downloads - [`fzf`](https://github.com/junegunn/fzf) - The
+[`mpv`](https://mpv.io) - player used for Windows, Linux and Android - [`iina`]
+             (https://iina.io) - player used for MacOS - [`Outplayer`](https://
+  outplayer.app/) - player used for iOS - [`ffmpeg`](https://github.com/FFmpeg/
+       FFmpeg) - For downloads - [`fzf`](https://github.com/junegunn/fzf) - The
   selection Menu ## Installation  ### Windows / Linux - Run this Command inside
   your Terminal ``` pip install mov-cli ``` - Optional ``` pip install lxml ```
               ### Android - Make sure [MPV](https://play.google.com/store/apps/
         details?id=is.xyz.mpv) and [Termux](https://play.google.com/store/apps/
    details?id=com.termux) are installed. - Install ``mov-cli``. ``` pip install
 mov-cli ``` - Optional ``` apt-get install libxml2 libxslt pip install lxml ```
        ### iOS - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/
```

### Comparing `mov_cli-1.4.1/mov_cli/__main__.py` & `mov_cli-1.4.2/mov_cli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,29 +35,28 @@
     "dopebox": [dopebox, "https://dopebox.to"],
     "viewasian": [viewasian, "https://viewasian.co"],
     "gogoanime": [gogoanime, "https://gogoanime.cl"],
     "watchasian": [watchasian, "https://www1.watchasian.id"],
     "wlext": [wlext, "https://wlext.is"],
     "streamblasters": [streamblasters, "https://streamblasters.pro"],
     "kinox": [kinox, "https://ww17.kinox.to"],
-    "tamilyogi": [tamilyogi, "https://tamilyogi.how"],
+    "tamilyogi": [tamilyogi, "https://tamilyogi.cash"],
     "einthusan": [einthusan, "https://einthusan.tv"],
     "turkish123": [turkish123, "https://turkish123.ac"],
     "animefox": [animefox, "https://animefox.to"],
     "scdn": [scdn, ""],
     "openloadmov": [openloadmov, "https://openloadmov.com"],
     "remotestream": [remotestream, "https://remotestre.am"],
     "kisscartoon": [kisscartoon, "https://thekisscartoon.com"],
     "yoturkish": [yoturkish, "https://www1.yoturkish.com"],
 }
 
 if platform.system() == "Windows":
     os.system("color FF")  # Fixes colour in Windows 10 CMD terminal
 
-
 def movcli():  # TODO add regex
     try:
         provider = ask()
         provider_data = calls.get(provider, calls["actvid"])
         provider: WebScraper = provider_data[0](provider_data[1])
         # provider.redo(query) if query is not None else provider.redo()
         provider.redo()  # if result else provider.redo(query)
```

### Comparing `mov_cli-1.4.1/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.2/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.2/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.2/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.2/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.2/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.2/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.2/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/players/player.py` & `mov_cli-1.4.2/mov_cli/players/player.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import sys
 import subprocess
-import time
-
 
+from .. import CMD_ARGS
 from ..utils.player import Player, PlayerNotFound
 
 
 class ply(Player):
     """A class to start the Player."""
 
     def __init__(self, webscraper_class: object) -> None:
@@ -36,22 +35,29 @@
             print(f'\033]8;;outplayer://{url}\033\\-------------------------\n- Tap to open Outplayer -\n-------------------------\033]8;;\033\\\n')
 
             sys.exit(1)
 
         else:  # Windows, Linux and Other
             try:
                 if self.os == "Linux" or self.os == "Windows":
+                    mpv_args = [
+                        f"--referrer={referrer}",
+                        f"{url}",
+                        f"--force-media-title=mov-cli:{media_title}",
+                        "--no-terminal",
+                    ]
+
+                    if CMD_ARGS.flatpak_mpv and self.os == "Linux": # Support for MPV on Flatpak.
+                        print("Using flatpak installation of MPV.")
+                        return subprocess.Popen(
+                            ["flatpak", "run", "io.mpv.Mpv"] + mpv_args
+                        )
+
                     return subprocess.Popen(
-                        [
-                            "mpv",
-                            f"--referrer={referrer}",
-                            f"{url}",
-                            f"--force-media-title=mov-cli:{media_title}",
-                            "--no-terminal",
-                        ]
+                        ["mpv"] + mpv_args
                     )
 
                 elif self.os == "Darwin":
                     return subprocess.Popen(
                         [
                             "iina",
                             "--no-stdin",
```

### Comparing `mov_cli-1.4.1/mov_cli/utils/dbs.py` & `mov_cli-1.4.2/mov_cli/utils/dbs.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/utils/httpclient.py` & `mov_cli-1.4.2/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/utils/jsunpack.py` & `mov_cli-1.4.2/mov_cli/utils/jsunpack.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/utils/lang.py` & `mov_cli-1.4.2/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/utils/player.py` & `mov_cli-1.4.2/mov_cli/utils/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/utils/provider.py` & `mov_cli-1.4.2/mov_cli/utils/provider.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/utils/scraper.py` & `mov_cli-1.4.2/mov_cli/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/actvid.py` & `mov_cli-1.4.2/mov_cli/websites/actvid.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/animefox.py` & `mov_cli-1.4.2/mov_cli/websites/animefox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/dopebox.py` & `mov_cli-1.4.2/mov_cli/websites/dopebox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/einthusan.py` & `mov_cli-1.4.2/mov_cli/websites/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/eja.py` & `mov_cli-1.4.2/mov_cli/websites/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/gogoanime.py` & `mov_cli-1.4.2/mov_cli/websites/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/kinox.py` & `mov_cli-1.4.2/mov_cli/websites/kinox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/kisscartoon.py` & `mov_cli-1.4.2/mov_cli/websites/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/openloadmov.py` & `mov_cli-1.4.2/mov_cli/websites/openloadmov.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.4.2/mov_cli/websites/redundant_kimcartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/remotestream.py` & `mov_cli-1.4.2/mov_cli/websites/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/scdn.py` & `mov_cli-1.4.2/mov_cli/websites/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/sflix.py` & `mov_cli-1.4.2/mov_cli/websites/sflix.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/solar.py` & `mov_cli-1.4.2/mov_cli/websites/solar.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/streamblasters.py` & `mov_cli-1.4.2/mov_cli/websites/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/tamilyogi.py` & `mov_cli-1.4.2/mov_cli/websites/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/turkish123.py` & `mov_cli-1.4.2/mov_cli/websites/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/viewasian.py` & `mov_cli-1.4.2/mov_cli/websites/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/watchasian.py` & `mov_cli-1.4.2/mov_cli/websites/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/wlext.py` & `mov_cli-1.4.2/mov_cli/websites/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/mov_cli/websites/yoturkish.py` & `mov_cli-1.4.2/mov_cli/websites/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.1/pyproject.toml` & `mov_cli-1.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.1"
+version = "1.4.2"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
 maintainers = ["Ananas <ananas@historylifeonline.xyz>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
```

### Comparing `mov_cli-1.4.1/PKG-INFO` & `mov_cli-1.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.1
+Version: 1.4.2
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
 Maintainer-email: ananas@historylifeonline.xyz
@@ -50,19 +50,19 @@
 [![MIT License][license-shield]][license-url]
 
 
 <!-- PROJECT LOGO -->
 <br />
 <div align="center">
   <a href="https://github.com/mov-cli/mov-cli">
-    <img src="https://user-images.githubusercontent.com/83706294/194960059-a9202d72-f033-46b4-b756-3193dc54fb20.png" alt="Logo" width="80" height="80">
+    <img src="https://github.com/mov-cli/mov-cli/assets/132799819/a23bec13-881d-41b9-b596-b31c6698b89e" alt="Logo" width="80" height="80">
   </a>
 
   <p align="center">
-    A cli tool to browse and watch movies/shows.
+ A cli tool to browse and watch Movies/Shows/TV/Sports. 
     <br />
     <br />
     <a href="https://github.com/mov-cli/mov-cli/issues">Report Bug</a>
     ·
     <a href="https://github.com/mov-cli/mov-cli/issues">Request Feature</a>
   </p>
 </div>
@@ -113,16 +113,17 @@
 <!-- GETTING STARTED -->
 ## Getting Started
 
 
 
 ### Prerequisites
 
-- [`mpv`](https://mpv.io) - Player used for Windows, Linux and Android
+- [`mpv`](https://mpv.io) - player used for Windows, Linux and Android
 - [`iina`](https://iina.io) - player used for MacOS
+- [`Outplayer`](https://outplayer.app/) - player used for iOS
 - [`ffmpeg`](https://github.com/FFmpeg/FFmpeg) - For downloads 
 - [`fzf`](https://github.com/junegunn/fzf) - The selection Menu
 
 
 ## Installation
 <!-- WIN AND LINUX -->
 ### Windows / Linux
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.1 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.2 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas Maintainer-email: ananas@historylifeonline.xyz Requires-
 Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
@@ -10,15 +10,15 @@
 py (>=0.0.4,<0.0.5) Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist:
 six (>=1.16.0,<2.0.0) Requires-Dist: tldextract (>=3.4.3,<4.0.0) Project-URL:
 Bug Tracker, https://github.com/mov-cli/mov-cli/issues Project-URL: Repository,
 https://github.com/mov-cli/mov-cli Description-Content-Type: text/markdown
 [![Stargazers][stars-shield]][stars-url] [![Issues][issues-shield]][issues-url]
 [![MIT License][license-shield]][license-url]
                                     [Logo]
-                 A cli tool to browse and watch movies/shows.
+            A cli tool to browse and watch Movies/Shows/TV/Sports.
 
                          Report_Bug Â· Request_Feature
  ### Table of Contents
    1. About_The_Project
    2. Getting_Started
           o Prerequisites
           o Installation
@@ -34,17 +34,18 @@
    9. inspiration
  ## About The Project mov-cli is a Commandline Tool to watch and download shows
 and movies. Shows and Movies are scraped from Streaming Sites. mov-cli
 currently scrapes 15 Providers: ``` Actvid Â· SFlix Â· Solar Â· DopeBox Â·
 WLEXT Â· KinoX Â· StreamBlasters Â· TamilYogi Â· Einthusan Â· ViewAsian Â·
 Watchasian Â· GogoAnime Â· Eja Â· KimCartoon Â· Turkish123 ```
    (back_to_top)!-- GETTING STARTED --> ## Getting Started ### Prerequisites -
-[`mpv`](https://mpv.io) - Player used for Windows, Linux and Android - [`iina`]
-     (https://iina.io) - player used for MacOS - [`ffmpeg`](https://github.com/
-FFmpeg/FFmpeg) - For downloads - [`fzf`](https://github.com/junegunn/fzf) - The
+[`mpv`](https://mpv.io) - player used for Windows, Linux and Android - [`iina`]
+             (https://iina.io) - player used for MacOS - [`Outplayer`](https://
+  outplayer.app/) - player used for iOS - [`ffmpeg`](https://github.com/FFmpeg/
+       FFmpeg) - For downloads - [`fzf`](https://github.com/junegunn/fzf) - The
   selection Menu ## Installation  ### Windows / Linux - Run this Command inside
   your Terminal ``` pip install mov-cli ``` - Optional ``` pip install lxml ```
               ### Android - Make sure [MPV](https://play.google.com/store/apps/
         details?id=is.xyz.mpv) and [Termux](https://play.google.com/store/apps/
    details?id=com.termux) are installed. - Install ``mov-cli``. ``` pip install
 mov-cli ``` - Optional ``` apt-get install libxml2 libxslt pip install lxml ```
        ### iOS - Make sure [Outplayer](https://apps.apple.com/us/app/outplayer/
```

