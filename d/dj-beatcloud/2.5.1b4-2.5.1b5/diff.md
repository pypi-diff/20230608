# Comparing `tmp/dj_beatcloud-2.5.1b4.tar.gz` & `tmp/dj_beatcloud-2.5.1b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj_beatcloud-2.5.1b4.tar", last modified: Tue Jun  6 00:00:48 2023, max compression
+gzip compressed data, was "dj_beatcloud-2.5.1b5.tar", last modified: Thu Jun  8 15:18:58 2023, max compression
```

## Comparing `dj_beatcloud-2.5.1b4.tar` & `dj_beatcloud-2.5.1b5.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.279925 dj_beatcloud-2.5.1b4/
--rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b4/LICENSE
--rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.5.1b4/MANIFEST.in
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-06 00:00:48.280005 dj_beatcloud-2.5.1b4/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.5.1b4/README.md
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.268879 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/
--rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/PKG-INFO
--rw-r--r--   0 alrichards   (502) staff       (20)     1853 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/SOURCES.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/dependency_links.txt
--rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/entry_points.txt
--rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/requires.txt
--rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-06-06 00:00:48.000000 dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/top_level.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.269653 dj_beatcloud-2.5.1b4/djtools/
--rw-r--r--   0 alrichards   (502) staff       (20)     2495 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b4/djtools/__main__.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.271382 dj_beatcloud-2.5.1b4/djtools/configs/
--rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/configs/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3691 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1214 2023-06-05 23:59:18.000000 dj_beatcloud-2.5.1b4/djtools/configs/config.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)    13601 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/configs/logging.conf
--rw-r--r--   0 alrichards   (502) staff       (20)     1028 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/rekordbox_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/configs/spotify_playlists.yaml
--rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-26 18:48:19.000000 dj_beatcloud-2.5.1b4/djtools/configs/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4790 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/configs/test_helpers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.271521 dj_beatcloud-2.5.1b4/djtools/logs/
--rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/logs/empty.txt
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.275032 dj_beatcloud-2.5.1b4/djtools/rekordbox/
--rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1726 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5865 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)    21727 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_combiner.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3483 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/tag_parsers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_copy_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5802 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5296 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_shuffle_playlists.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/rekordbox/test_tag_parsers.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.276614 dj_beatcloud-2.5.1b4/djtools/spotify/
--rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/spotify/playlist_builder.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2288 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/spotify/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/spotify/test_playlist_builder.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.277904 dj_beatcloud-2.5.1b4/djtools/sync/
--rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/sync/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b4/djtools/sync/sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/sync/test_sync_operations.py
--rw-r--r--   0 alrichards   (502) staff       (20)      669 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/test_main.py
-drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-06 00:00:48.279709 dj_beatcloud-2.5.1b4/djtools/utils/
--rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/__init__.py
--rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/config.py
--rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_check_tracks.py
--rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_config.py
--rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_helpers.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/test_url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b4/djtools/utils/url_download.py
--rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-06-05 23:59:58.000000 dj_beatcloud-2.5.1b4/djtools/version.py
--rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b4/pyproject.toml
--rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-06-06 00:00:48.280278 dj_beatcloud-2.5.1b4/setup.cfg
--rw-r--r--   0 alrichards   (502) staff       (20)     2425 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b4/setup.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.838005 dj_beatcloud-2.5.1b5/
+-rw-r--r--   0 alrichards   (502) staff       (20)    35148 2022-06-16 01:40:44.000000 dj_beatcloud-2.5.1b5/LICENSE
+-rw-r--r--   0 alrichards   (502) staff       (20)       56 2023-05-26 19:42:57.000000 dj_beatcloud-2.5.1b5/MANIFEST.in
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-08 15:18:58.838113 dj_beatcloud-2.5.1b5/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1319 2023-05-26 21:16:19.000000 dj_beatcloud-2.5.1b5/README.md
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.823467 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2604 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/PKG-INFO
+-rw-r--r--   0 alrichards   (502) staff       (20)     1853 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        1 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)       41 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/entry_points.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)      264 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/requires.txt
+-rw-r--r--   0 alrichards   (502) staff       (20)        8 2023-06-08 15:18:58.000000 dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/top_level.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.824475 dj_beatcloud-2.5.1b5/djtools/
+-rw-r--r--   0 alrichards   (502) staff       (20)     2495 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1741 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b5/djtools/__main__.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.827400 dj_beatcloud-2.5.1b5/djtools/configs/
+-rw-r--r--   0 alrichards   (502) staff       (20)      496 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/configs/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3691 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1214 2023-06-08 15:18:00.000000 dj_beatcloud-2.5.1b5/djtools/configs/config.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)    13601 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      484 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/configs/logging.conf
+-rw-r--r--   0 alrichards   (502) staff       (20)     1028 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/rekordbox_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/configs/spotify_playlists.yaml
+-rw-r--r--   0 alrichards   (502) staff       (20)     2424 2023-05-26 18:48:19.000000 dj_beatcloud-2.5.1b5/djtools/configs/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4790 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/configs/test_helpers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.827637 dj_beatcloud-2.5.1b5/djtools/logs/
+-rw-r--r--   0 alrichards   (502) staff       (20)        0 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/logs/empty.txt
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.831062 dj_beatcloud-2.5.1b5/djtools/rekordbox/
+-rw-r--r--   0 alrichards   (502) staff       (20)     1333 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1726 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4117 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6989 2023-06-08 15:09:39.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    21533 2023-06-08 14:34:28.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    11626 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_combiner.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2839 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3483 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/tag_parsers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1326 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1481 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_copy_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6848 2023-06-08 15:14:05.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5326 2023-06-08 14:59:58.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1563 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_shuffle_playlists.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4224 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/rekordbox/test_tag_parsers.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.833481 dj_beatcloud-2.5.1b5/djtools/spotify/
+-rw-r--r--   0 alrichards   (502) staff       (20)      718 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3233 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    16593 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6051 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/spotify/playlist_builder.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2288 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/spotify/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    19216 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     6568 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/spotify/test_playlist_builder.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.835711 dj_beatcloud-2.5.1b5/djtools/sync/
+-rw-r--r--   0 alrichards   (502) staff       (20)      772 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/sync/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3365 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8258 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4678 2023-05-05 16:05:21.000000 dj_beatcloud-2.5.1b5/djtools/sync/sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     2820 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     8572 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     4758 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/sync/test_sync_operations.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      669 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/test_main.py
+drwxr-xr-x   0 alrichards   (502) staff       (20)        0 2023-06-08 15:18:58.837839 dj_beatcloud-2.5.1b5/djtools/utils/
+-rw-r--r--   0 alrichards   (502) staff       (20)      821 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/__init__.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     3660 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1259 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)    10158 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     5668 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_check_tracks.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      510 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_config.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     9077 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_helpers.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1745 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/test_url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)     1654 2023-05-05 16:01:07.000000 dj_beatcloud-2.5.1b5/djtools/utils/url_download.py
+-rw-r--r--   0 alrichards   (502) staff       (20)       92 2023-06-08 15:18:27.000000 dj_beatcloud-2.5.1b5/djtools/version.py
+-rw-r--r--   0 alrichards   (502) staff       (20)      225 2023-05-04 18:27:17.000000 dj_beatcloud-2.5.1b5/pyproject.toml
+-rw-r--r--   0 alrichards   (502) staff       (20)      125 2023-06-08 15:18:58.838456 dj_beatcloud-2.5.1b5/setup.cfg
+-rw-r--r--   0 alrichards   (502) staff       (20)     2425 2023-06-05 23:58:40.000000 dj_beatcloud-2.5.1b5/setup.py
```

### Comparing `dj_beatcloud-2.5.1b4/LICENSE` & `dj_beatcloud-2.5.1b5/LICENSE`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/PKG-INFO` & `dj_beatcloud-2.5.1b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj_beatcloud
-Version: 2.5.1b4
+Version: 2.5.1b5
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b4 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj_beatcloud Version: 2.5.1b5 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b4/README.md` & `dj_beatcloud-2.5.1b5/README.md`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/PKG-INFO` & `dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-beatcloud
-Version: 2.5.1b4
+Version: 2.5.1b5
 Summary: DJ Tools is a library for managing a collection of music and Rekordbox XML files.
 Home-page: https://github.com/a-rich/DJ-tools
 Author: Alex Richards
 Author-email: alex.richards006@gmail.com
 License: GNU GPLv3
 Keywords: MP3 Rekordbox XML spotify reddit aws s3
 Classifier: Development Status :: 4 - Beta
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b4 Summary: DJ Tools is
+Metadata-Version: 2.1 Name: dj-beatcloud Version: 2.5.1b5 Summary: DJ Tools is
 a library for managing a collection of music and Rekordbox XML files. Home-
 page: https://github.com/a-rich/DJ-tools Author: Alex Richards Author-email:
 alex.richards006@gmail.com License: GNU GPLv3 Keywords: MP3 Rekordbox XML
 spotify reddit aws s3 Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: Intended Audience :: End Users/
 Desktop Classifier: Intended Audience :: Other Audience Classifier: License ::
 OSI Approved :: GNU General Public License v3 (GPLv3) Classifier: Natural
```

### Comparing `dj_beatcloud-2.5.1b4/dj_beatcloud.egg-info/SOURCES.txt` & `dj_beatcloud-2.5.1b5/dj_beatcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/__init__.py` & `dj_beatcloud-2.5.1b5/djtools/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/__main__.py` & `dj_beatcloud-2.5.1b5/djtools/__main__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/configs/config.py` & `dj_beatcloud-2.5.1b5/djtools/configs/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/configs/config.yaml` & `dj_beatcloud-2.5.1b5/djtools/configs/config.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/configs/helpers.py` & `dj_beatcloud-2.5.1b5/djtools/configs/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/configs/rekordbox_playlists.yaml` & `dj_beatcloud-2.5.1b5/djtools/configs/rekordbox_playlists.yaml`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/configs/test_config.py` & `dj_beatcloud-2.5.1b5/djtools/configs/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/configs/test_helpers.py` & `dj_beatcloud-2.5.1b5/djtools/configs/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/__init__.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/config.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/copy_playlists.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/helpers.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/helpers.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """This module contains helpers for the rekordbox package."""
+from collections import defaultdict
 from operator import itemgetter
 from pathlib import Path
 import re
 import shutil
 from typing import Any, Dict, List, Optional, Set, Tuple
 from urllib.parse import unquote
 
@@ -136,20 +137,49 @@
         if str(track).strip() and track["Key"] not in seen_tracks
     ]
     seen_tracks.update(playlist_tracks)
 
     return playlist_tracks
 
 
+def print_playlists_tag_statistics(
+    playlist_tracks: Dict[str, Set[str]],
+    track_lookup: Dict[str, Set[str]],
+    parser_tracks: Dict[str, Dict[str, List[Tuple[str, List[str]]]]],
+) -> None:
+    """Prints tag statistics for Combiner playlists.
+
+    Statistics are split out by Combiner playlist and then by TagParser type.
+
+    Args:
+        playlist_tracks: Combiner playlists mapped to track IDs.
+        track_lookup: Track IDs mapped to set of tags.
+        parser_tracks: Parser type mapped to tags mapped to list of
+            (track ID, tag list) tuples.
+    """
+    for playlist, _tracks in playlist_tracks.items():
+        if not _tracks:
+            continue
+        print(f"\n{playlist} tag statistics:")
+        playlist_tags = defaultdict(int)
+        for track in _tracks:
+            for tag in track_lookup[track]:
+                playlist_tags[tag] += 1
+        for parser, parser_tags in parser_tracks.items():
+            print(f"\n{parser}:")
+            print_data({k: playlist_tags[k] for k in parser_tags})
+
+
 def print_data(data: Dict[str, int]):
     """Prints an ASCII histogram of tag data.
 
     Args:
         data: Tag names to tag counts.
     """
+    data = {k: v for k, v in data.items() if v}
     scaled_data = scale_data(data)
     row_width = 0
     width_pad = 1
     row = max(scaled_data.items(), key=itemgetter(1))[1]
     output = ""
     while row > 0:
         output += "|"
```

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_builder.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import bs4
 from bs4 import BeautifulSoup
 import yaml
 
 from djtools.configs.config import BaseConfig
 from djtools.rekordbox import tag_parsers
-from djtools.rekordbox.helpers import print_data
+from djtools.rekordbox.helpers import print_playlists_tag_statistics
 from djtools.rekordbox.playlist_combiner import Combiner
 
 
 logger = logging.getLogger(__name__)
 
 
 class PlaylistBuilder:
@@ -61,27 +61,31 @@
         be specified by separating two integers with a dash.
     """
     def __init__(
         self,
         rekordbox_database: Path,
         playlist_config: Path,
         playlist_remainder_type: str = "",
+        verbosity: int = 0,
     ):
         """Constructor.
 
         Args:
             rekordbox_database: Path to Rekordbox XML.
             playlist_config: Playlist taxonomy.
             playlist_remainder_type: Whether unspecified tags are grouped into
                 a "folder" or "playlist".
+            verbosity: Whether or not to print playlist tag statistics.
 
         Raises:
             AttributeError: Configured TagParser must be implemented in
                 "tag_parsers.py".
         """
+        self.verbosity = verbosity
+
         # Load Rekordbox database from XML.
         self._database_path = rekordbox_database
         with open(self._database_path, mode="r", encoding="utf-8") as _file:
             self._database = BeautifulSoup(_file.read(), "xml")
 
         # Get playlist root node.
         self._playlists_root = self._database.find_all(
@@ -211,25 +215,18 @@
             )
             merged_tracks.update(playlist_mapping)
 
             # Evaluate the boolean logic of the Combiner playlists.
             tracks = self._combiner_parser(merged_tracks)
 
             # Print tag statistics for each Combiner playlist.
-            for playlist, _tracks in tracks.items():
-                if not _tracks:
-                    continue
-                print(f"\n{playlist} tag statistics:")
-                playlist_tags = defaultdict(int)
-                for track in _tracks:
-                    for tag in track_lookup[track]:
-                        playlist_tags[tag] += 1
-                for parser, parser_tags in parser_tracks.items():
-                    print(f"\n{parser}:")
-                    print_data({k: playlist_tags[k] for k in parser_tags})
+            if self.verbosity:
+                print_playlists_tag_statistics(
+                    tracks, track_lookup, parser_tracks
+                )
 
             self._add_tracks(
                 soup=self._database,
                 playlists=combiner_playlists,
                 tracks=tracks,
             )
 
@@ -513,9 +510,10 @@
     playlist_config = (
         Path(__file__).parent.parent / "configs" / "rekordbox_playlists.yaml"
     )
     playlist_builder = PlaylistBuilder(
         rekordbox_database=config.XML_PATH,
         playlist_config=playlist_config,
         playlist_remainder_type=config.BUILD_PLAYLISTS_REMAINDER,
+        verbosity=config.VERBOSITY,
     )
     playlist_builder()
```

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/playlist_combiner.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/playlist_combiner.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/shuffle_playlists.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/tag_parsers.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_config.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_copy_playlists.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/test_copy_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_helpers.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/test_helpers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Testing for the helpers module."""
 import inspect
 from pathlib import Path
 import re
+from unittest import mock
 from urllib.parse import unquote
 
 import pytest
 
 from djtools.rekordbox.helpers import (
     BooleanNode,
     copy_file,
     get_playlist_tracks,
     print_data,
+    print_playlists_tag_statistics,
     scale_data,
     set_track_number,
 )
 
 
 @pytest.mark.parametrize(
     "node_attributes",
@@ -105,53 +107,86 @@
 
 
 def test_print_data(capsys):
     """Test for the print_data function."""
     data = {
         "Aggro": 30,
         "Bounce": 2,
-        "Chill": 1,
+        "Chill": 0,
         "Dark": 19,
         "Melodic": 9,
         "Rave": 13,
     }
     expected = (
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                                            \n" +
-        "|   *                      *                     \n" +
-        "|   *                      *                     \n" +
-        "|   *                      *                     \n" +
-        "|   *                      *                     \n" +
-        "|   *                      *                     \n" +
-        "|   *                      *                 *   \n" +
-        "|   *                      *                 *   \n" +
-        "|   *                      *                 *   \n" +
-        "|   *                      *        *        *   \n" +
-        "|   *                      *        *        *   \n" +
-        "|   *                      *        *        *   \n" +
-        "|   *                      *        *        *   \n" +
-        "|   *                      *        *        *   \n" +
-        "|   *                      *        *        *   \n" +
-        "|   *       *              *        *        *   \n" +
-        "|   *       *       *      *        *        *   \n" +
-        "-------------------------------------------------\n" +
-        "  Aggro   Bounce   Chill   Dark   Melodic   Rave  \n"
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *                                     \n" +
+        "|   *               *                     \n" +
+        "|   *               *                     \n" +
+        "|   *               *                     \n" +
+        "|   *               *                     \n" +
+        "|   *               *                     \n" +
+        "|   *               *                 *   \n" +
+        "|   *               *                 *   \n" +
+        "|   *               *                 *   \n" +
+        "|   *               *        *        *   \n" +
+        "|   *               *        *        *   \n" +
+        "|   *               *        *        *   \n" +
+        "|   *               *        *        *   \n" +
+        "|   *               *        *        *   \n" +
+        "|   *               *        *        *   \n" +
+        "|   *       *       *        *        *   \n" +
+        "|   *       *       *        *        *   \n" +
+        "------------------------------------------\n" +
+        "  Aggro   Bounce   Dark   Melodic   Rave  \n"
     )
     print_data(data)
     cap = capsys.readouterr()
     assert cap.out == expected
 
 
+@mock.patch("djtools.rekordbox.helpers.print_data")
+def test_print_playlists_tag_statistics(mock_print_data, capsys):
+    """Test for the print_playlists_tag_statistics function."""
+    playlist_tracks = {
+        "Dubstep | Techno": {"1", "3"},
+        "Eurodance & Hip Hop": {},
+    }
+    track_lookup = {
+        "1": {"Dark", "Dubstep"}, "3": {"Minimal Deep Tech", "Techno"}
+    }
+    parser_tracks = {
+        "GenreTagParser": {
+            "Dubstep": [("1", ["Dark", "Dubstep"])],
+            "Minimal Deep Tech": [("3", ["Minimal Deep Tech", "Techno"])],
+            "Techno": [("3", ["Minimal Deep Tech", "Techno"])],
+        },
+        "MyTagParser": {
+            "Dark": [("1", ["Dark", "Dubstep"])],
+        },
+    }
+    print_playlists_tag_statistics(
+        playlist_tracks, track_lookup, parser_tracks
+    )
+    cap = capsys.readouterr()
+    for playlist, tracks in playlist_tracks.items():
+        if not tracks:
+            continue
+        assert f"\n{playlist} tag statistics:" in cap.out
+        for parser, parser_tags in parser_tracks.items():
+            assert f"\n{parser}" in cap.out
+    assert mock_print_data.call_count == len(parser_tracks)
+
+
 def test_scale_output():
     """Test for the scale_output function."""
     data = {
         "Aggro": 30,
         "Bounce": 2,
         "Chill": 1,
         "Dark": 19,
```

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_playlist_builder.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/test_playlist_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     build_playlists, PlaylistBuilder
 )
 
 
 def test_build_playlists(test_config, test_xml):
     """Test for the build_playlists function."""
     test_config.XML_PATH = Path(test_xml)
+    test_config.VERBOSITY = 1
     build_playlists(test_config)
 
 
 @pytest.mark.parametrize(
     "remainder_type", ["", "folder", "playlist", "invalid"]
 )
 def test_playlistbuilder(remainder_type, test_xml, test_playlist_config):
```

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_shuffle_playlists.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/test_shuffle_playlists.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/rekordbox/test_tag_parsers.py` & `dj_beatcloud-2.5.1b5/djtools/rekordbox/test_tag_parsers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/__init__.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/config.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/helpers.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/playlist_builder.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/test_config.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/test_helpers.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/spotify/test_playlist_builder.py` & `dj_beatcloud-2.5.1b5/djtools/spotify/test_playlist_builder.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/__init__.py` & `dj_beatcloud-2.5.1b5/djtools/sync/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/config.py` & `dj_beatcloud-2.5.1b5/djtools/sync/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/helpers.py` & `dj_beatcloud-2.5.1b5/djtools/sync/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/sync_operations.py` & `dj_beatcloud-2.5.1b5/djtools/sync/sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/test_config.py` & `dj_beatcloud-2.5.1b5/djtools/sync/test_config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/test_helpers.py` & `dj_beatcloud-2.5.1b5/djtools/sync/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/sync/test_sync_operations.py` & `dj_beatcloud-2.5.1b5/djtools/sync/test_sync_operations.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/test_main.py` & `dj_beatcloud-2.5.1b5/djtools/test_main.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/__init__.py` & `dj_beatcloud-2.5.1b5/djtools/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/check_tracks.py` & `dj_beatcloud-2.5.1b5/djtools/utils/check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/config.py` & `dj_beatcloud-2.5.1b5/djtools/utils/config.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/helpers.py` & `dj_beatcloud-2.5.1b5/djtools/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/test_check_tracks.py` & `dj_beatcloud-2.5.1b5/djtools/utils/test_check_tracks.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/test_helpers.py` & `dj_beatcloud-2.5.1b5/djtools/utils/test_helpers.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/test_url_download.py` & `dj_beatcloud-2.5.1b5/djtools/utils/test_url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/djtools/utils/url_download.py` & `dj_beatcloud-2.5.1b5/djtools/utils/url_download.py`

 * *Files identical despite different names*

### Comparing `dj_beatcloud-2.5.1b4/setup.py` & `dj_beatcloud-2.5.1b5/setup.py`

 * *Files identical despite different names*

