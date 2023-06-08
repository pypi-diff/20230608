# Comparing `tmp/py-Ayiin-0.4.4.dev2.tar.gz` & `tmp/py-Ayiin-0.4.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.4.dev2.tar", last modified: Fri Jun  2 05:22:58 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.4.dev3.tar", last modified: Thu Jun  8 13:25:57 2023, max compression
```

## Comparing `py-Ayiin-0.4.4.dev2.tar` & `py-Ayiin-0.4.4.dev3.tar`

### file list

```diff
@@ -1,85 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.372465 py-Ayiin-0.4.4.dev2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-02 05:22:58.372465 py-Ayiin-0.4.4.dev2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1479 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.364465 py-Ayiin-0.4.4.dev2/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.364465 py-Ayiin-0.4.4.dev2/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.364465 py-Ayiin-0.4.4.dev2/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.368465 py-Ayiin-0.4.4.dev2/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.368465 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.368465 py-Ayiin-0.4.4.dev2/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.372465 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.372465 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 05:22:58.372465 py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-02 05:22:58.000000 py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-06-02 05:22:58.000000 py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 05:22:58.000000 py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-02 05:22:58.000000 py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 05:22:58.000000 py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 05:22:58.372465 py-Ayiin-0.4.4.dev2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-02 05:22:42.000000 py-Ayiin-0.4.4.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.080101 py-Ayiin-0.4.4.dev3/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.084101 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.084101 py-Ayiin-0.4.4.dev3/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.088101 py-Ayiin-0.4.4.dev3/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.088101 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/setup.py
```

### Comparing `py-Ayiin-0.4.4.dev2/LICENSE` & `py-Ayiin-0.4.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/NOTICE` & `py-Ayiin-0.4.4.dev3/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/PKG-INFO` & `py-Ayiin-0.4.4.dev3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev2
+Version: 0.4.4.dev3
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
@@ -17,36 +17,43 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Py - Ayiin Library
+<p align="center">
+  <img src="https://telegra.ph//file/897863d5713e6b0b5ec58.jpg">
+</p>
 
-Core library of [The AyiinXd](https://github.com/AyiinXd/AyiinXd), a Pyrogram And Telethon based for your userbot.
 
+### Core library of [py-Ayiin](https://github.com/AyiinXd)
+Pyrogram And Telethon based for your userbot.
 
+
+#
 [![PyPI - Version](https://img.shields.io/pypi/v/py-Ayiin?style=round)](https://pypi.org/project/py-Ayiin)    
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ayiin?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ayiin)    
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ayiin?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ayiin/)    
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/AyiinXd/AyiinXd/graphs/commit-activity)
 [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/AyiinXd/AyiinXd)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 # Installation
 ```bash
 pip3 install -U py-Ayiin
 ```
+#
 
+## Made with ✨ by
 
-See more working plugins on [the offical repository](https://github.com/AyiinXd/AyiinXd)!
-
-> Made with ✨ by [@AyiinXd](https://t.me/AyiinXd).    
-
-
+[![Ayiin](https://img.shields.io/static/v1?label=Github&message=AyiinXd&color=critical)](https://github.com/AyiinXd)   
+[![Ayiin](https://img.shields.io/static/v1?label=Telegram&message=AyiinXd&color=aqua)](https://t.me/AyiinXd)
+#
 # License
 [![License](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)](LICENSE)   
-AyiinXd is licensed under [GNU General Public License](https://www.gnu.org/licenses/agpl-3.0.html) v3 or later.
-
+py-Ayiin is licensed under [GNU General Public License](https://www.gnu.org/licenses/agpl-3.0.html) v3 or later.
+#
 # Credits
-*  [![Ayiin](https://img.shields.io/static/v1?label=Ayiin&message=Devs&color=critical)](https://t.me/AyiinXd)
+*  [AyiinXd](https://github.com/AyiinXd) for [py-Ayiin](https://github.com/AyiinXd)
 *  [Dan](https://github.com/delivrance) for [Pyrogram](https://github.com/pyrogram/pyrogram)
 *  [Lonami](https://github.com/LonamiWebs/) for [Telethon](https://github.com/LonamiWebs/Telethon)
+#
```

### Comparing `py-Ayiin-0.4.4.dev2/README.md` & `py-Ayiin-0.4.4.dev3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # Py - Ayiin Library
+<p align="center">
+  <img src="https://telegra.ph//file/897863d5713e6b0b5ec58.jpg">
+</p>
 
-Core library of [The AyiinXd](https://github.com/AyiinXd/AyiinXd), a Pyrogram And Telethon based for your userbot.
 
+### Core library of [py-Ayiin](https://github.com/AyiinXd)
+Pyrogram And Telethon based for your userbot.
 
+
+#
 [![PyPI - Version](https://img.shields.io/pypi/v/py-Ayiin?style=round)](https://pypi.org/project/py-Ayiin)    
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ayiin?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ayiin)    
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ayiin?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ayiin/)    
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/AyiinXd/AyiinXd/graphs/commit-activity)
 [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/AyiinXd/AyiinXd)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 # Installation
 ```bash
 pip3 install -U py-Ayiin
 ```
+#
 
+## Made with ✨ by
 
-See more working plugins on [the offical repository](https://github.com/AyiinXd/AyiinXd)!
-
-> Made with ✨ by [@AyiinXd](https://t.me/AyiinXd).    
-
-
+[![Ayiin](https://img.shields.io/static/v1?label=Github&message=AyiinXd&color=critical)](https://github.com/AyiinXd)   
+[![Ayiin](https://img.shields.io/static/v1?label=Telegram&message=AyiinXd&color=aqua)](https://t.me/AyiinXd)
+#
 # License
 [![License](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)](LICENSE)   
-AyiinXd is licensed under [GNU General Public License](https://www.gnu.org/licenses/agpl-3.0.html) v3 or later.
-
+py-Ayiin is licensed under [GNU General Public License](https://www.gnu.org/licenses/agpl-3.0.html) v3 or later.
+#
 # Credits
-*  [![Ayiin](https://img.shields.io/static/v1?label=Ayiin&message=Devs&color=critical)](https://t.me/AyiinXd)
+*  [AyiinXd](https://github.com/AyiinXd) for [py-Ayiin](https://github.com/AyiinXd)
 *  [Dan](https://github.com/delivrance) for [Pyrogram](https://github.com/pyrogram/pyrogram)
 *  [Lonami](https://github.com/LonamiWebs/) for [Telethon](https://github.com/LonamiWebs/Telethon)
+#
```

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/startup.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/__init__.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.4.dev02"
+__version__ = "0.4.4.dev03"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
@@ -143,14 +143,15 @@
     from .decorator import *
     from .config import *
 
     print("\n\n" + __copyright__ + "\n" + __license__)
     print(start_bot)
 
     CMD_HELP = {}
+    adB = AyiinDB()
     aiosession = ClientSession()
     loop = asyncio.get_event_loop()
     HOSTED_ON = where_hosted()
     Yins = VcTools()
 else:
     print(suc_msg)
     print(__copyright__ + "\n" + __license__ + "\n\n")
```

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/__main__.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/assistant.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/assistant.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/config.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/start.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/decorator.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/exceptions.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # t.me/AyiinChat & t.me/AyiinSupport
 
 
 # ========================×========================
 #            Jangan Hapus Credit Ngentod
 # ========================×========================
 
+from ._database import AyiinDB
 from ._misc import _Misc
 from .changer import Changers
 from .converter import Convert
 from .func import Funci
 from .funcb import FuncBot
 from .helpers import Helpers, run_async
 from .hosting import where_hosted
```

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/func.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/funcb.py`

 * *Files 21% similar despite different names*

```diff
@@ -26,66 +26,68 @@
 
 
 class FuncBot(object):
     async def approve_pmpermit(
         self,
         cb,
         user_ids,
+        chat_id,
         OLD_MSG,
     ):
         from ..dB.pmpermit import approve_pmpermit, is_pmpermit_approved
 
         
         if isinstance(cb, CallbackQuery):
-            if await is_pmpermit_approved(user_ids):
+            if await is_pmpermit_approved(user_ids, chat_id):
                 await cb.answer("Pengguna Ini Sudah Ada Di Database.", show_alert=True)
                 return
-            await approve_pmpermit(user_ids)
+            await approve_pmpermit(user_ids, chat_id)
             await cb.edit_message_text("Pesan Anda Diterima Tod")
-            if str(user_ids) in OLD_MSG:
-                await OLD_MSG[str(user_ids)].delete()
+            if str(chat_id) in OLD_MSG:
+                await OLD_MSG[str(chat_id)].delete()
         elif isinstance(cb, Message):
-            if await is_pmpermit_approved(user_ids):
+            if await is_pmpermit_approved(user_ids, chat_id):
                 await cb.edit("Pengguna Ini Sudah Ada Di Database.", show_alert=True)
                 return
-            await approve_pmpermit(user_ids)
+            await approve_pmpermit(user_ids, chat_id)
             await cb.edit("Pesan Anda Diterima Tod")
-            if str(user_ids) in OLD_MSG:
-                await OLD_MSG[str(user_ids)].delete()
+            if str(chat_id) in OLD_MSG:
+                await OLD_MSG[str(chat_id)].delete()
         
     async def disapprove_pmpermit(
         self,
         cb,
         user_ids,
+        chat_id,
     ):
         from ..dB.pmpermit import disapprove_pmpermit, is_pmpermit_approved
         
         if isinstance(cb, CallbackQuery):
-            if not await is_pmpermit_approved(user_ids):
+            if not await is_pmpermit_approved(user_ids, chat_id):
                 return await cb.answer("Pengguna Ini Tidak Ada Di Database")
-            await disapprove_pmpermit(user_ids)
+            await disapprove_pmpermit(user_ids, chat_id)
             await cb.edit_message_text("Pesan Anda Ditolak Tod")
         elif isinstance(cb, Message):
-            if not await is_pmpermit_approved(user_ids):
+            if not await is_pmpermit_approved(user_ids, chat_id):
                 return await cb.edit("Pengguna Ini Tidak Ada Di Database")
-            await disapprove_pmpermit(user_ids)
+            await disapprove_pmpermit(user_ids, chat_id)
             await cb.edit("Pesan Anda Ditolak Tod")
 
 
     async def logger(
         self,
         client,
         pepek,
     ):
-        from pyAyiin.Clients.client import Var, tgbot
+        from pyAyiin.Clients.client import tgbot
 
         if pepek.text:
             try:
                 x = await tgbot.send_message(
-                    Var.LOG_CHAT,
+                    client.me.id,
                     f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}\nPesan:\n{pepek.text}",
                     reply_markup=InlineKeyboardMarkup(
                         [
                             [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                         ]
                     ),
                     disable_web_page_preview=True,
@@ -94,15 +96,15 @@
                 await asyncio.sleep(e.value)
             except BaseException:
                 pass
         if pepek.photo:
             try:
                 file = await client.download_media(pepek.photo)
                 x = await tgbot.send_photo(
-                    Var.LOG_CHAT,
+                    client.me.id,
                     photo=file,
                     caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
                     reply_markup=InlineKeyboardMarkup(
                         [
                             [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                         ]
                     ),
@@ -112,15 +114,15 @@
                 await asyncio.sleep(e.value)
             except BaseException:
                 pass
         if pepek.video:
             try:
                 file = await client.download_media(pepek.video)
                 x = await tgbot.send_video(
-                    Var.LOG_CHAT,
+                    client.me.id,
                     video=file,
                     caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
                     reply_markup=InlineKeyboardMarkup(
                         [
                             [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                         ]
                     ),
@@ -130,15 +132,15 @@
                 await asyncio.sleep(e.value)
             except BaseException:
                 pass
         if pepek.voice:
             try:
                 file = await client.download_media(pepek.voice)
                 x = await tgbot.send_voice(
-                    Var.LOG_CHAT,
+                    client.me.id,
                     voice=file,
                     caption=f"Logs: {client.me.first_name}\nPesan Dari: {pepek.from_user.first_name}",
                     reply_markup=InlineKeyboardMarkup(
                         [
                             [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                         ]
                     ),
@@ -148,15 +150,15 @@
                 await asyncio.sleep(e.value)
             except BaseException:
                 pass
         if pepek.sticker:
             try:
                 file = await client.download_media(pepek.sticker)
                 x = await tgbot.send_sticker(
-                    Var.LOG_CHAT,
+                    client.me.id,
                     sticker=file,
                     reply_markup=InlineKeyboardMarkup(
                         [
                             [InlineKeyboardButton("💌 Pengirim 💌", url=f"tg://openmessage?user_id={pepek.from_user.id}")],
                         ]
                     ),
                 )
```

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/inlinebot.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,16 +24,16 @@
 )
 
 from ..config import Var
 from ..pyrogram.toolbot import ToolBot
 
 
 class InlineBot(Var, ToolBot):
-    async def inline_pmpermit(self, ids):
-        from pyAyiin.dB.variable import get_var
+    async def inline_pmpermit(self, user_id, ids):
+        from pyAyiin.dB.pmpermit import all_pmpermit
         
         button = [
             [
                 InlineKeyboardButton(
                     text='• Approve •',
                     callback_data=f'terima_{ids}',
                 ),
@@ -45,49 +45,49 @@
             [
                 InlineKeyboardButton(
                     text='• Close •',
                     callback_data=f'close',
                 ),
             ]
         ]
-        PERMIT_PIC = await get_var('PERMIT_PIC')
+        pm_message, media_message, limit = all_pmpermit(user_id)
         endsw = (".mp4", ".gif")
-        if PERMIT_PIC is not None: # Jika database HELP_PIC tidak kosong
-            if PERMIT_PIC.endswith(endsw): # jika format video atau gif 
+        if media_message: # Jika database HELP_PIC tidak kosong
+            if media_message.endswith(endsw): # jika format video atau gif 
                 pm_results = [
                     (
                         InlineQueryResultVideo(
-                            video_url=PERMIT_PIC,
-                            thumb_url=PERMIT_PIC,
+                            video_url=media_message,
+                            thumb_url=media_message,
                             title="PmPermit",
                             description="inline AyiinUbot.",
-                            caption=self.PERMIT_MSG,
+                            caption=pm_message,
                             reply_markup=InlineKeyboardMarkup(button),
                         )
                     )
                 ]
             else: # Format foto
                 pm_results = [
                     (
                         InlineQueryResultPhoto(
-                            photo_url=PERMIT_PIC,
+                            photo_url=media_message,
                             title="PmPermit",
                             description="inline AyiinUbot.",
-                            caption=self.PERMIT_MSG,
+                            caption=pm_message,
                             reply_markup=InlineKeyboardMarkup(button),
                         )
                     )
                 ]
         else: # Jika database HELP_PIC kosong akan menjadi teks biasa tanpa foto atau video
             pm_results = [
                 (
                     InlineQueryResultArticle(
                         title='PmPermit Ayiin Ubot!',
                         reply_markup=InlineKeyboardMarkup(button),
-                        input_message_content=InputTextMessageContent(self.PERMIT_MSG),
+                        input_message_content=InputTextMessageContent(pm_message),
                     )
                 )
             ]
         
         return pm_results
     
     async def inline_help(self, output):
```

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.4.dev3/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/pyAyiin/xd.py` & `py-Ayiin-0.4.4.dev3/pyAyiin/xd.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev2
+Version: 0.4.4.dev3
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
@@ -17,36 +17,43 @@
 Classifier: Operating System :: OS Independent
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # Py - Ayiin Library
+<p align="center">
+  <img src="https://telegra.ph//file/897863d5713e6b0b5ec58.jpg">
+</p>
 
-Core library of [The AyiinXd](https://github.com/AyiinXd/AyiinXd), a Pyrogram And Telethon based for your userbot.
 
+### Core library of [py-Ayiin](https://github.com/AyiinXd)
+Pyrogram And Telethon based for your userbot.
 
+
+#
 [![PyPI - Version](https://img.shields.io/pypi/v/py-Ayiin?style=round)](https://pypi.org/project/py-Ayiin)    
-[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ayiin?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ayiin)    
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/py-Ayiin?label=DOWNLOADS&style=round)](https://pypi.org/project/py-Ayiin/)    
 [![Maintenance](https://img.shields.io/badge/Maintained%3F-yes-green.svg)](https://github.com/AyiinXd/AyiinXd/graphs/commit-activity)
 [![Open Source Love svg2](https://badges.frapsoft.com/os/v2/open-source.svg?v=103)](https://github.com/AyiinXd/AyiinXd)
 [![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](https://makeapullrequest.com)
 
 # Installation
 ```bash
 pip3 install -U py-Ayiin
 ```
+#
 
+## Made with ✨ by
 
-See more working plugins on [the offical repository](https://github.com/AyiinXd/AyiinXd)!
-
-> Made with ✨ by [@AyiinXd](https://t.me/AyiinXd).    
-
-
+[![Ayiin](https://img.shields.io/static/v1?label=Github&message=AyiinXd&color=critical)](https://github.com/AyiinXd)   
+[![Ayiin](https://img.shields.io/static/v1?label=Telegram&message=AyiinXd&color=aqua)](https://t.me/AyiinXd)
+#
 # License
 [![License](https://www.gnu.org/graphics/gplv3-with-text-136x68.png)](LICENSE)   
-AyiinXd is licensed under [GNU General Public License](https://www.gnu.org/licenses/agpl-3.0.html) v3 or later.
-
+py-Ayiin is licensed under [GNU General Public License](https://www.gnu.org/licenses/agpl-3.0.html) v3 or later.
+#
 # Credits
-*  [![Ayiin](https://img.shields.io/static/v1?label=Ayiin&message=Devs&color=critical)](https://t.me/AyiinXd)
+*  [AyiinXd](https://github.com/AyiinXd) for [py-Ayiin](https://github.com/AyiinXd)
 *  [Dan](https://github.com/delivrance) for [Pyrogram](https://github.com/pyrogram/pyrogram)
 *  [Lonami](https://github.com/LonamiWebs/) for [Telethon](https://github.com/LonamiWebs/Telethon)
+#
```

### Comparing `py-Ayiin-0.4.4.dev2/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 pyAyiin/xd.py
 pyAyiin/Clients/__init__.py
 pyAyiin/Clients/client.py
 pyAyiin/Clients/pytgcalls.py
 pyAyiin/Clients/startup.py
 pyAyiin/dB/__init__.py
 pyAyiin/dB/_core.py
+pyAyiin/dB/_session.py
 pyAyiin/dB/absen.py
 pyAyiin/dB/admins.py
 pyAyiin/dB/auth.py
 pyAyiin/dB/blacklistfilter.py
 pyAyiin/dB/blacklistgcast.py
 pyAyiin/dB/blacklistuser.py
 pyAyiin/dB/gban.py
@@ -30,14 +31,15 @@
 pyAyiin/dB/premium.py
 pyAyiin/dB/start.py
 pyAyiin/dB/sudo.py
 pyAyiin/dB/variable.py
 pyAyiin/dB/videocalls.py
 pyAyiin/dB/welcome.py
 pyAyiin/methods/__init__.py
+pyAyiin/methods/_database.py
 pyAyiin/methods/_misc.py
 pyAyiin/methods/changer.py
 pyAyiin/methods/converter.py
 pyAyiin/methods/func.py
 pyAyiin/methods/funcb.py
 pyAyiin/methods/helpers.py
 pyAyiin/methods/hosting.py
@@ -48,14 +50,15 @@
 pyAyiin/pyrogram/_wrappers.py
 pyAyiin/pyrogram/func.py
 pyAyiin/pyrogram/misc.py
 pyAyiin/pyrogram/pastebin.py
 pyAyiin/pyrogram/sections.py
 pyAyiin/pyrogram/toolbot.py
 pyAyiin/pyrogram/tools.py
+pyAyiin/resources/Logo Ayiin.jpg
 pyAyiin/resources/Youtube.jpeg
 pyAyiin/resources/__init__.py
 pyAyiin/resources/ayiin_music.jpg
 pyAyiin/resources/ayiin_ubot.jpg
 pyAyiin/resources/ayiin_userbot.jpg
 pyAyiin/resources/blank.png
 pyAyiin/resources/default.ttf
```

### Comparing `py-Ayiin-0.4.4.dev2/setup.py` & `py-Ayiin-0.4.4.dev3/setup.py`

 * *Files identical despite different names*

