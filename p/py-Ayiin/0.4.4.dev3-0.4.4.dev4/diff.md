# Comparing `tmp/py-Ayiin-0.4.4.dev3.tar.gz` & `tmp/py-Ayiin-0.4.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-Ayiin-0.4.4.dev3.tar", last modified: Thu Jun  8 13:25:57 2023, max compression
+gzip compressed data, was "py-Ayiin-0.4.4.dev4.tar", last modified: Thu Jun  8 13:41:57 2023, max compression
```

## Comparing `py-Ayiin-0.4.4.dev3.tar` & `py-Ayiin-0.4.4.dev4.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.080101 py-Ayiin-0.4.4.dev3/pyAyiin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.084101 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/
--rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/pytgcalls.py
--rw-r--r--   0 runner    (1001) docker     (123)    38642 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/Clients/startup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/assistant.py
--rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.084101 py-Ayiin-0.4.4.dev3/pyAyiin/dB/
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/absen.py
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/admins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistgcast.py
--rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistuser.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/gban.py
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/langs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/logdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/pmpermit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/premium.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/start.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/videocalls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/dB/welcome.py
--rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/decorator.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.088101 py-Ayiin-0.4.4.dev3/pyAyiin/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/_database.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/changer.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/converter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/funcb.py
--rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/hosting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/inlinebot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.088101 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/func.py
--rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/pastebin.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/sections.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/toolbot.py
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/pyAyiin/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/Logo Ayiin.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/Youtube.jpeg
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_music.jpg
--rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_ubot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_userbot.jpg
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/blank.png
--rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/default.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/font.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/resources/font2.ttf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/pyAyiin/xd.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 13:25:57.000000 py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:25:57.092101 py-Ayiin-0.4.4.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-08 13:25:43.000000 py-Ayiin-0.4.4.dev3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.459529 py-Ayiin-0.4.4.dev4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      134 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 13:41:57.459529 py-Ayiin-0.4.4.dev4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.443529 py-Ayiin-0.4.4.dev4/pyAyiin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.447529 py-Ayiin-0.4.4.dev4/pyAyiin/Clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/Clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12525 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/Clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6153 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/Clients/pytgcalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38643 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/Clients/startup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6209 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5126 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.447529 py-Ayiin-0.4.4.dev4/pyAyiin/dB/
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/absen.py
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/admins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2255 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1406 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/blacklistfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/blacklistgcast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      783 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/blacklistuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/gban.py
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/langs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/logdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/pmpermit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/premium.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/start.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/videocalls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/dB/welcome.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33254 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.451529 py-Ayiin-0.4.4.dev4/pyAyiin/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10094 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/_database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1897 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/changer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6909 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6278 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/funcb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8828 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/hosting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6927 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/inlinebot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.451529 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13157 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/func.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/pastebin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/sections.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/toolbot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.455530 py-Ayiin-0.4.4.dev4/pyAyiin/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   281001 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/Logo Ayiin.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    31343 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/Youtube.jpeg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39497 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/ayiin_music.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)  1808670 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/ayiin_ubot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    60539 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/ayiin_userbot.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/blank.png
+-rw-r--r--   0 runner    (1001) docker     (123)    56364 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/default.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   141612 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/font.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   128248 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/resources/font2.ttf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.455530 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.455530 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6803 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17263 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/pyAyiin/xd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:41:57.455530 py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-08 13:41:57.000000 py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-08 13:41:57.000000 py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:41:57.000000 py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      137 2023-06-08 13:41:57.000000 py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 13:41:57.000000 py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 13:41:57.459529 py-Ayiin-0.4.4.dev4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-06-08 13:41:46.000000 py-Ayiin-0.4.4.dev4/setup.py
```

### Comparing `py-Ayiin-0.4.4.dev3/LICENSE` & `py-Ayiin-0.4.4.dev4/LICENSE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/NOTICE` & `py-Ayiin-0.4.4.dev4/NOTICE`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/PKG-INFO` & `py-Ayiin-0.4.4.dev4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev3
+Version: 0.4.4.dev4
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.4.dev3/README.md` & `py-Ayiin-0.4.4.dev4/README.md`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/__init__.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/Clients/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/client.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/Clients/client.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/pytgcalls.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/Clients/pytgcalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/Clients/startup.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/Clients/startup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
 HOSTED_ON = where_hosted()
 Var = Variable()
 Xd = Helpers()
 
 
 async def ayiin_client(client):
     try:
-        await client.join_chat("AyiinChat")
-        await client.join_chat("AyiinSupport")
+        await client.join_chat("AyiinChats")
+        await client.join_chat("AyiinChannel")
         await client.join_chat("StoryAyiin")
     except Exception:
         pass
 
 
 clients = []
 client_id = []
```

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/__init__.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 
 
 logs = logging.getLogger(__name__)
 
 
 __copyright__ = "Copyright (C) 2022-present AyiinXd <https://github.com/AyiinXd>"
 __license__ = "GNU General Public License v3.0 (GPL-3.0)"
-__version__ = "0.4.4.dev03"
+__version__ = "0.4.4.dev04"
 ayiin_ver = "0.1.1"
 
 
 DEVS = [
     607067484, # Ayiin
     997461844, #Ayang_Ayiin
     2130526178, # Alfa
```

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/__main__.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/__main__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/assistant.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/assistant.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
             if "me" in from_users:
                 from_users.remove("me")
                 for bot in Bots:
                     mebot = await bot.get_me()
                     from_users.append(mebot.id)
             if client_only and cq.from_user.id not in client_id:
                 return await cq.answer(
-                    "Ini Bukan Userbot Anda, Silahkan Buat Userbot Anda Di @AyiinChat",
+                    "Ini Bukan Userbot Anda, Silahkan Buat Userbot Anda Di @AyiinChats",
                     show_alert=True,
                 )
             if admins and not await is_admin_or_owner(
                 cq.message, from_users
             ):
                 return await cq.answer(
                     "Lu Bukan Admin Di Gc Ini Tod...",
```

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/config.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/config.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/__init__.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/absen.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/absen.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/admins.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/admins.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/auth.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/auth.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistfilter.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/blacklistfilter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistgcast.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/blacklistgcast.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/blacklistuser.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/blacklistuser.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/gban.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/gban.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/langs.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/langs.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/logdb.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/logdb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/pmpermit.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/pmpermit.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/premium.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/premium.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/start.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/start.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/sudo.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/sudo.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/variable.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/variable.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/videocalls.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/videocalls.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/dB/welcome.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/dB/welcome.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/decorator.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/decorator.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/exceptions.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/__init__.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/_database.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/_database.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/_misc.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/_misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/changer.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/changer.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/converter.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/converter.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/func.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/funcb.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/funcb.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/helpers.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/helpers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/hosting.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/hosting.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/inlinebot.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/inlinebot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/queue.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/queue.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/methods/thumbnail.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/__init__.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/__init__.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/_wrappers.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/func.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/func.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/misc.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/pastebin.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/pastebin.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/sections.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/sections.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/toolbot.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/toolbot.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/pyrogram/tools.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/pyrogram/tools.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/Logo Ayiin.jpg` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/Logo Ayiin.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/Youtube.jpeg` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/Youtube.jpeg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_music.jpg` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/ayiin_music.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_ubot.jpg` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/ayiin_ubot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/ayiin_userbot.jpg` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/ayiin_userbot.jpg`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/blank.png` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/blank.png`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/default.ttf` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/default.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/font.ttf` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/font.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/resources/font2.ttf` & `py-Ayiin-0.4.4.dev4/pyAyiin/resources/font2.ttf`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/_wrappers.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/_wrappers.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/events.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/events.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/telethon/ayiin/misc.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/telethon/ayiin/misc.py`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/pyAyiin/xd.py` & `py-Ayiin-0.4.4.dev4/pyAyiin/xd.py`

 * *Files 1% similar despite different names*

```diff
@@ -347,29 +347,29 @@
             pass
         await self.cek_client(client)
         await client.disconnect()
         return string_session
 
 
     async def cek_client(self, client):
-        gocheck = str(pybase64.b64decode("QEF5aWluU3VwcG9ydA=="))[2:15]
-        checker = str(pybase64.b64decode("QEF5aWluQ2hhdA=="))[2:12]
+        gocheck = str(pybase64.b64decode("QEF5aWluQ2hhbm5lbA=="))[2:15]
+        checker = str(pybase64.b64decode("QEF5aWluQ2hhdHM="))[2:11]
         checkxd = str(pybase64.b64decode("QFN0b3J5QXlpaW4="))[2:13]
         if client:
             try:
                 await client.join_chat(gocheck)
                 await client.join_chat(checker)
                 await client.join_chat(checkxd)
             except BaseException:
                 pass
 
 
     async def cekclient(self, client):
-        gocheck = str(pybase64.b64decode("QEF5aWluU3VwcG9ydA=="))[2:15]
-        checker = str(pybase64.b64decode("QEF5aWluQ2hhdA=="))[2:12]
+        gocheck = str(pybase64.b64decode("QEF5aWluQ2hhbm5lbA=="))[2:15]
+        checker = str(pybase64.b64decode("QEF5aWluQ2hhdHM="))[2:11]
         checkxd = str(pybase64.b64decode("QFN0b3J5QXlpaW4="))[2:13]
         if client:
             try:
                 await client(Get(gocheck))
                 await client(Get(checker))
                 await client(Get(checkxd))
             except BaseException:
```

### Comparing `py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/PKG-INFO` & `py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-Ayiin
-Version: 0.4.4.dev3
+Version: 0.4.4.dev4
 Summary: A Secure and Powerful Python-Telethon Based and Python-Pyrogram Based Library For Your Userbot Module.
 Home-page: https://github.com/AyiinXd/AyiinXd
 Author: AyiinXd
 Author-email: ayingaming98@gmail.com
 License: GNU General Public License v3.0 (GPL-3.0)
 Project-URL: Bug Tracker, https://github.com/AyiinXd/AyiinXd/issues
 Project-URL: Source Code, https://github.com/AyiinXd/AyiinXd
```

### Comparing `py-Ayiin-0.4.4.dev3/py_Ayiin.egg-info/SOURCES.txt` & `py-Ayiin-0.4.4.dev4/py_Ayiin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-Ayiin-0.4.4.dev3/setup.py` & `py-Ayiin-0.4.4.dev4/setup.py`

 * *Files identical despite different names*

