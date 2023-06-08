# Comparing `tmp/eis1600-0.9.3.tar.gz` & `tmp/eis1600-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eis1600-0.9.3.tar", last modified: Mon Jun  5 10:52:14 2023, max compression
+gzip compressed data, was "eis1600-0.9.4.tar", last modified: Thu Jun  8 09:08:51 2023, max compression
```

## Comparing `eis1600-0.9.3.tar` & `eis1600-0.9.4.tar`

### file list

```diff
@@ -1,84 +1,84 @@
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.530443 eis1600-0.9.3/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.3/LICENSE
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-06-05 10:52:14.530443 eis1600-0.9.3/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7640 2023-05-11 10:42:54.000000 eis1600-0.9.3/README.md
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.510443 eis1600-0.9.3/eis1600/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.3/eis1600/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.514443 eis1600-0.9.3/eis1600/dates/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.3/eis1600/dates/Date.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.3/eis1600/dates/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5860 2023-05-26 10:12:33.000000 eis1600-0.9.3/eis1600/dates/date_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.3/eis1600/dates/methods.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.514443 eis1600-0.9.3/eis1600/gazetteers/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.3/eis1600/gazetteers/Onomastics.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3444 2023-06-05 10:10:23.000000 eis1600-0.9.3/eis1600/gazetteers/Toponyms.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.3/eis1600/gazetteers/__init__.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.518443 eis1600-0.9.3/eis1600/gazetteers/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.3/eis1600/gazetteers/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.3/eis1600/gazetteers/data/onomastic_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.3/eis1600/gazetteers/data/spelling_gazetteer.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264263 2023-06-05 09:15:15.000000 eis1600-0.9.3/eis1600/gazetteers/data/toponyms_gazetteer.csv
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.518443 eis1600-0.9.3/eis1600/helper/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.3/eis1600/helper/EntityTags.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.3/eis1600/helper/Singleton.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.3/eis1600/helper/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.3/eis1600/helper/ar_normalization.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.522443 eis1600-0.9.3/eis1600/helper/data/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.3/eis1600/helper/data/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.3/eis1600/helper/data/entity_tags.csv
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.3/eis1600/helper/fix_miu_annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.3/eis1600/helper/logging.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.3/eis1600/helper/markdown_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3805 2023-05-26 10:16:32.000000 eis1600-0.9.3/eis1600/helper/markdown_patterns.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.3/eis1600/helper/miu_random_revisions.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11237 2023-05-24 09:28:18.000000 eis1600-0.9.3/eis1600/helper/repo.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.3/eis1600/helper/yml_methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1682 2023-05-26 10:17:00.000000 eis1600-0.9.3/eis1600/helper/yml_to_json.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.522443 eis1600-0.9.3/eis1600/markdown/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.3/eis1600/markdown/UIDs.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.3/eis1600/markdown/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.3/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.3/eis1600/markdown/insert_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12991 2023-05-04 08:54:08.000000 eis1600-0.9.3/eis1600/markdown/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.3/eis1600/markdown/update_uids.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.3/eis1600/markdown/update_uids_old_process.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.522443 eis1600-0.9.3/eis1600/miu/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.3/eis1600/miu/HeadingTracker.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8429 2023-05-26 10:49:19.000000 eis1600-0.9.3/eis1600/miu/YAMLHandler.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.3/eis1600/miu/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.3/eis1600/miu/disassemble_into_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9125 2023-05-25 14:09:24.000000 eis1600-0.9.3/eis1600/miu/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.3/eis1600/miu/reassemble_from_miu_files.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8483 2023-05-26 10:07:04.000000 eis1600-0.9.3/eis1600/miu/yml_handling.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/nlp/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.3/eis1600/nlp/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2017 2023-03-31 12:22:46.000000 eis1600-0.9.3/eis1600/nlp/cameltools.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3511 2023-05-26 10:27:39.000000 eis1600-0.9.3/eis1600/nlp/ner_annotate_mius.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2726 2023-04-05 11:18:46.000000 eis1600-0.9.3/eis1600/nlp/utils.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/onomastics/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.3/eis1600/onomastics/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.3/eis1600/onomastics/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10339 2023-05-26 10:07:04.000000 eis1600-0.9.3/eis1600/onomastics/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.3/eis1600/onomastics/re_pattern.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/processing/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.3/eis1600/processing/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4705 2023-05-26 10:08:19.000000 eis1600-0.9.3/eis1600/processing/postprocessing.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4613 2023-05-26 14:04:30.000000 eis1600-0.9.3/eis1600/processing/preprocessing.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/stats/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.3/eis1600/stats/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.3/eis1600/stats/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.3/eis1600/stats/miu_stats.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.526443 eis1600-0.9.3/eis1600/toponyms/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.3/eis1600/toponyms/__init__.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1494 2023-05-26 10:26:52.000000 eis1600-0.9.3/eis1600/toponyms/annotation.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1777 2023-05-17 15:35:46.000000 eis1600-0.9.3/eis1600/toponyms/methods.py
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      856 2023-05-26 12:57:33.000000 eis1600-0.9.3/eis1600/toponyms/toponym_categories.py
-drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-05 10:52:14.514443 eis1600-0.9.3/eis1600.egg-info/
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10053 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/PKG-INFO
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2050 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/SOURCES.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/dependency_links.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      800 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/entry_points.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/requires.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-06-05 10:52:14.000000 eis1600-0.9.3/eis1600.egg-info/top_level.txt
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-06-05 10:52:14.530443 eis1600-0.9.3/setup.cfg
--rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2372 2023-06-05 10:52:09.000000 eis1600-0.9.3/setup.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.148184 eis1600-0.9.4/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1046 2022-09-21 09:22:30.000000 eis1600-0.9.4/LICENSE
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-08 09:08:51.148184 eis1600-0.9.4/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     7967 2023-06-08 08:10:00.000000 eis1600-0.9.4/README.md
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.132184 eis1600-0.9.4/eis1600/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-19 09:55:48.000000 eis1600-0.9.4/eis1600/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.136184 eis1600-0.9.4/eis1600/dates/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      911 2023-04-05 11:10:16.000000 eis1600-0.9.4/eis1600/dates/Date.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.4/eis1600/dates/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5860 2023-05-26 10:12:33.000000 eis1600-0.9.4/eis1600/dates/date_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3924 2023-04-12 06:44:26.000000 eis1600-0.9.4/eis1600/dates/methods.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.136184 eis1600-0.9.4/eis1600/gazetteers/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4245 2023-05-26 10:11:18.000000 eis1600-0.9.4/eis1600/gazetteers/Onomastics.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3448 2023-06-05 11:20:45.000000 eis1600-0.9.4/eis1600/gazetteers/Toponyms.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-09 08:52:31.000000 eis1600-0.9.4/eis1600/gazetteers/__init__.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.136184 eis1600-0.9.4/eis1600/gazetteers/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.4/eis1600/gazetteers/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    96536 2023-04-17 09:44:13.000000 eis1600-0.9.4/eis1600/gazetteers/data/onomastic_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1307 2023-04-03 09:19:01.000000 eis1600-0.9.4/eis1600/gazetteers/data/spelling_gazetteer.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)   264282 2023-06-05 11:33:25.000000 eis1600-0.9.4/eis1600/gazetteers/data/toponyms_gazetteer.csv
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.140184 eis1600-0.9.4/eis1600/helper/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      990 2023-05-25 16:02:00.000000 eis1600-0.9.4/eis1600/helper/EntityTags.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1280 2023-04-24 10:02:09.000000 eis1600-0.9.4/eis1600/helper/Singleton.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-10-20 15:09:05.000000 eis1600-0.9.4/eis1600/helper/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1030 2023-04-06 13:50:26.000000 eis1600-0.9.4/eis1600/helper/ar_normalization.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.140184 eis1600-0.9.4/eis1600/helper/data/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-04-03 10:40:59.000000 eis1600-0.9.4/eis1600/helper/data/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      324 2023-05-17 14:58:12.000000 eis1600-0.9.4/eis1600/helper/data/entity_tags.csv
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1247 2023-05-26 10:15:41.000000 eis1600-0.9.4/eis1600/helper/fix_miu_annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      377 2023-05-26 10:20:20.000000 eis1600-0.9.4/eis1600/helper/logging.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      707 2023-05-10 14:33:13.000000 eis1600-0.9.4/eis1600/helper/markdown_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3805 2023-05-26 10:16:32.000000 eis1600-0.9.4/eis1600/helper/markdown_patterns.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6461 2023-03-09 10:15:31.000000 eis1600-0.9.4/eis1600/helper/miu_random_revisions.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    11212 2023-06-08 08:03:01.000000 eis1600-0.9.4/eis1600/helper/repo.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      383 2023-05-24 09:09:03.000000 eis1600-0.9.4/eis1600/helper/yml_methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1682 2023-05-26 10:17:00.000000 eis1600-0.9.4/eis1600/helper/yml_to_json.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.140184 eis1600-0.9.4/eis1600/markdown/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1822 2023-04-12 07:11:17.000000 eis1600-0.9.4/eis1600/markdown/UIDs.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-09-30 09:01:09.000000 eis1600-0.9.4/eis1600/markdown/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4809 2023-05-26 10:21:31.000000 eis1600-0.9.4/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4589 2023-05-26 10:14:46.000000 eis1600-0.9.4/eis1600/markdown/insert_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    12973 2023-06-08 07:44:43.000000 eis1600-0.9.4/eis1600/markdown/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2875 2023-05-26 10:22:35.000000 eis1600-0.9.4/eis1600/markdown/update_uids.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     5268 2023-05-26 10:25:25.000000 eis1600-0.9.4/eis1600/markdown/update_uids_old_process.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/miu/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3481 2023-05-26 10:15:16.000000 eis1600-0.9.4/eis1600/miu/HeadingTracker.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8429 2023-05-26 10:49:19.000000 eis1600-0.9.4/eis1600/miu/YAMLHandler.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-08 08:28:10.000000 eis1600-0.9.4/eis1600/miu/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2773 2023-05-26 10:23:54.000000 eis1600-0.9.4/eis1600/miu/disassemble_into_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     9595 2023-06-08 09:08:43.000000 eis1600-0.9.4/eis1600/miu/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2605 2023-05-26 10:26:08.000000 eis1600-0.9.4/eis1600/miu/reassemble_from_miu_files.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     8483 2023-05-26 10:07:04.000000 eis1600-0.9.4/eis1600/miu/yml_handling.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/nlp/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-17 12:10:00.000000 eis1600-0.9.4/eis1600/nlp/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2935 2023-06-08 07:49:05.000000 eis1600-0.9.4/eis1600/nlp/cameltools.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     3577 2023-06-08 07:55:51.000000 eis1600-0.9.4/eis1600/nlp/ner_annotate_mius.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     6543 2023-06-08 07:58:41.000000 eis1600-0.9.4/eis1600/nlp/utils.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/onomastics/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-03-02 09:23:30.000000 eis1600-0.9.4/eis1600/onomastics/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1358 2023-05-25 14:13:19.000000 eis1600-0.9.4/eis1600/onomastics/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10544 2023-06-08 08:49:39.000000 eis1600-0.9.4/eis1600/onomastics/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1966 2023-04-17 09:33:17.000000 eis1600-0.9.4/eis1600/onomastics/re_pattern.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/processing/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2022-11-14 11:12:12.000000 eis1600-0.9.4/eis1600/processing/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4724 2023-06-08 07:25:33.000000 eis1600-0.9.4/eis1600/processing/postprocessing.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     4613 2023-05-26 14:04:30.000000 eis1600-0.9.4/eis1600/processing/preprocessing.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.144184 eis1600-0.9.4/eis1600/stats/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-02-17 08:45:10.000000 eis1600-0.9.4/eis1600/stats/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      842 2023-02-17 15:06:29.000000 eis1600-0.9.4/eis1600/stats/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1978 2023-02-17 15:05:56.000000 eis1600-0.9.4/eis1600/stats/miu_stats.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.148184 eis1600-0.9.4/eis1600/toponyms/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        0 2023-05-17 10:52:32.000000 eis1600-0.9.4/eis1600/toponyms/__init__.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     1494 2023-05-26 10:26:52.000000 eis1600-0.9.4/eis1600/toponyms/annotation.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2959 2023-06-08 09:06:21.000000 eis1600-0.9.4/eis1600/toponyms/methods.py
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      856 2023-06-07 09:48:13.000000 eis1600-0.9.4/eis1600/toponyms/toponym_categories.py
+drwxrwxr-x   0 lisbert   (1000) lisbert   (1000)        0 2023-06-08 09:08:51.132184 eis1600-0.9.4/eis1600.egg-info/
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)    10420 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/PKG-INFO
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2050 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/SOURCES.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        1 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/dependency_links.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)      800 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/entry_points.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       83 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/requires.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)        8 2023-06-08 09:08:51.000000 eis1600-0.9.4/eis1600.egg-info/top_level.txt
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)       38 2023-06-08 09:08:51.148184 eis1600-0.9.4/setup.cfg
+-rw-rw-r--   0 lisbert   (1000) lisbert   (1000)     2372 2023-06-08 08:13:11.000000 eis1600-0.9.4/setup.py
```

### Comparing `eis1600-0.9.3/LICENSE` & `eis1600-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/PKG-INFO` & `eis1600-0.9.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.3
+Version: 0.9.4
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
@@ -49,14 +49,16 @@
         ```
         
         In case you have an older version installed, use:
         ```shell
         $ pip install --upgrade eis1600
         ```
         
+        **Note**. You can use `pip freeze` to check the versions of all installed packages, including `eis1600`.
+        
         ## Set Up Virtual Environment and Install the EIS1600 PKG there
         
         To not mess with other python installations, we recommend installing the package in a virual environment.
         To create a new virtual environment with python, run:
         ```shell
         python3 -m venv eis1600_env
         ```
@@ -99,14 +101,15 @@
         The working directory is always the main `EIS1600` directory which is a parent to all the different repositories.
         The `EIS1600` directory has the following structure:
         
         ```
         |
         |---| eis_env
         |---| EIS1600_MIUs
+        |---| EIS1600_Pretrained_Models (optional)
         |---| gazetteers
         |---| Master_Chronicle
         |---| OpenITI_EIS1600_Texts
         |---| Training_Data
         ```
         
         Path variables are in the module `eis1600/helper/repo`.
@@ -167,33 +170,35 @@
         Use the `-e` option to process all files from the MIU repo. Must be run from the root of MIU repo.
         ```shell
         $ reassemble_from_miu_files -e <MIU_repo>
         ```
         
         ### Annotation
         
-        NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastics.
+        NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastic information.
+        
+        **Note** Can only be run if package was installed with *NER* flag AND if the ML models are in the [EIS1600_Pretrained_Models](#structure-of-the-working-directory) directory.
+        
+        If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `EIS1600_MIUs/`).
+        ```shell
+        $ annotate_mius -p
+        ```
         
         To annotate all MIU files of a text give the IDs file as argument.
         Can be used with `-p` option to run in parallel.
         ```shell
         $ annotate_mius <uri>.IDs
         ```
         
         To annotate an individual MIU file, give MIU file as argument.
         ```shell
         $ annotate_mius <uri>/MIUs/<uri>.<UID>.EIS1600
         ```
         
-        If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
-        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
-        ```shell
-        $ annotate_mius -p
-        ```
-        
         ### Only Onomastic Annotation
         
         **Only for test purposes!**
         Can be run with `-D` to process one file at a time, otherwise runs in parallel.
         Can be run with `-T` to use gold-standard data as input.
         Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`.
         ```shell
```

### Comparing `eis1600-0.9.3/README.md` & `eis1600-0.9.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -41,14 +41,16 @@
 ```
 
 In case you have an older version installed, use:
 ```shell
 $ pip install --upgrade eis1600
 ```
 
+**Note**. You can use `pip freeze` to check the versions of all installed packages, including `eis1600`.
+
 ## Set Up Virtual Environment and Install the EIS1600 PKG there
 
 To not mess with other python installations, we recommend installing the package in a virual environment.
 To create a new virtual environment with python, run:
 ```shell
 python3 -m venv eis1600_env
 ```
@@ -91,14 +93,15 @@
 The working directory is always the main `EIS1600` directory which is a parent to all the different repositories.
 The `EIS1600` directory has the following structure:
 
 ```
 |
 |---| eis_env
 |---| EIS1600_MIUs
+|---| EIS1600_Pretrained_Models (optional)
 |---| gazetteers
 |---| Master_Chronicle
 |---| OpenITI_EIS1600_Texts
 |---| Training_Data
 ```
 
 Path variables are in the module `eis1600/helper/repo`.
@@ -159,33 +162,35 @@
 Use the `-e` option to process all files from the MIU repo. Must be run from the root of MIU repo.
 ```shell
 $ reassemble_from_miu_files -e <MIU_repo>
 ```
 
 ### Annotation
 
-NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastics.
+NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastic information.
+
+**Note** Can only be run if package was installed with *NER* flag AND if the ML models are in the [EIS1600_Pretrained_Models](#structure-of-the-working-directory) directory.
+
+If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
+Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `EIS1600_MIUs/`).
+```shell
+$ annotate_mius -p
+```
 
 To annotate all MIU files of a text give the IDs file as argument.
 Can be used with `-p` option to run in parallel.
 ```shell
 $ annotate_mius <uri>.IDs
 ```
 
 To annotate an individual MIU file, give MIU file as argument.
 ```shell
 $ annotate_mius <uri>/MIUs/<uri>.<UID>.EIS1600
 ```
 
-If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
-Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
-```shell
-$ annotate_mius -p
-```
-
 ### Only Onomastic Annotation
 
 **Only for test purposes!**
 Can be run with `-D` to process one file at a time, otherwise runs in parallel.
 Can be run with `-T` to use gold-standard data as input.
 Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`.
 ```shell
```

### Comparing `eis1600-0.9.3/eis1600/dates/Date.py` & `eis1600-0.9.4/eis1600/dates/Date.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/dates/date_patterns.py` & `eis1600-0.9.4/eis1600/dates/date_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/dates/methods.py` & `eis1600-0.9.4/eis1600/dates/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/gazetteers/Onomastics.py` & `eis1600-0.9.4/eis1600/gazetteers/Onomastics.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/gazetteers/Toponyms.py` & `eis1600-0.9.4/eis1600/gazetteers/Toponyms.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
             prefixed_variations = [prefix + top for prefix in prefixes for top in variations]
             return variations + prefixed_variations
 
         df['toponyms'] = df['toponyms'].apply(get_all_variations)
 
         topos = df.explode('toponyms', ignore_index=True)
 
-        Toponyms.__settlements = topos.loc[topos['type_label'] != 'region', 'toponyms'].to_list()
-        Toponyms.__provinces = topos.loc[topos['type_label'] == 'region', 'toponyms'].to_list()
+        Toponyms.__settlements = topos.loc[topos['type_label'] != 'province', 'toponyms'].to_list()
+        Toponyms.__provinces = topos.loc[topos['type_label'] == 'province', 'toponyms'].to_list()
         Toponyms.__df = topos
         Toponyms.__df.mask(isna(Toponyms.__df), '', inplace=True)
 
         Toponyms.__total = Toponyms.__settlements + Toponyms.__provinces
         Toponyms.__rpl = [(elem, elem.replace(' ', '_')) for elem in Toponyms.__total if ' ' in elem]
 
     @staticmethod
```

### Comparing `eis1600-0.9.3/eis1600/gazetteers/data/onomastic_gazetteer.csv` & `eis1600-0.9.4/eis1600/gazetteers/data/onomastic_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/gazetteers/data/spelling_gazetteer.csv` & `eis1600-0.9.4/eis1600/gazetteers/data/spelling_gazetteer.csv`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/gazetteers/data/toponyms_gazetteer.csv` & `eis1600-0.9.4/eis1600/gazetteers/data/toponyms_gazetteer.csv`

 * *Files 0% similar despite different names*

```diff
@@ -2244,26 +2244,26 @@
 ZIFTAJAWAD_312E307N_S,Ziftā Ǧawād,زفتا جواد,زفتا جواد,MISR_305E292N_R,towns,Point,"(31.21094, 30.70718)"
 ZIRADABADH_553E366N_S,Ziradābāḏ,زرداباذ,زرداباذ، زرداباذ,NW_IRAN_515E356N_R,waystations,Point,"(55.30802, 36.65798)"
 ZIYADABADHZIYADAWADH_532E298N_S,ZiyādābāḏZiyādāwāḏ,زياداباذزياداواذ,زياداباذزياداواذ,,waystations,Point,"(53.22441, 29.83708)"
 ZUBALA_435E294N_S,Zubālaŧ,زبالة,زبالة,CENTRAL_ARABIA_416E227N_R,waystations,Point,"(43.5639, 29.40521)"
 ZUBAYDIYYA_468E342N_S,al-Zubaydiyyaŧ,الزبيدية,الزبيدية,NW_IRAN_515E356N_R,waystations,Point,"(46.85168, 34.23099)"
 ZUBAYDIYYA_469E344N_S,al-Zubaydiyyaŧ,الزبيدية,الزبيدية,NW_IRAN_515E356N_R,waystations,Point,"(46.93427, 34.43457)"
 ZUZAN_598E343N_S,Zūzan,زوزن,زوزن,NE_IRAN_606E351N_R,towns,Point,"(59.86207, 34.3105)"
-ANDALUS_040E398N_R,al-Andalus,الأندلس,الأندلس,,regions,Point,"(-4.0521, 39.88926)"
-BARQA_221E314N_R,Barqaŧ,برقة,برقة,,regions,Point,"(22.1, 31.4)"
-CENTRAL_ARABIA_416E227N_R,al-Ḥijāz+,الجزيرة,الجزيرة، أقور,,regions,Point,"(41.65725, 22.78726)"
-IFRIQIYYA_78E349N_R,Ifriqiyyā,إفريقية,إفريقية,,regions,Point,"(7.8, 34.9)"
-IRAQ_459E319N_R,al-ʿIrāq,العراق,العراق,,regions,Point,"(45.96, 31.9)"
-JAZIRA_420E364N_R,al-Jazīraŧ,جزيرة,جزيرة، جزيرة العرب,,regions,Point,"(42.05, 36.41)"
-MAGHRIB_045E323N_R,al-Maġrib,المغرب,المغرب,,regions,Point,"(-4.52149, 32.30201)"
-MAWARANNAHR_656E401N_R,Mā warāʾ al-nahr,ما وراء النهر,ما وراء النهر,,regions,Point,"(65.61472, 40.1917)"
-MISR_305E292N_R,Miṣr,مصر,مصر، الديار المصرية,,regions,Point,"(30.52, 29.23)"
-NE_IRAN_606E351N_R,Ḫurāsān,خراسان,خراسان,,regions,Point,"(60.61524, 35.17917)"
-NW_IRAN_515E356N_R,al-Jibāl+,الجبال,الجبال، الجبل,,regions,Point,"(51.50831, 35.62754)"
-QABQ_457E413N_R,al-Riḥāb,الرحاب,الرحاب,,regions,Point,"(45.79, 41.33)"
-RUM_335E392N_R,al-Rūm,الروم,الروم، بلد الروم,,regions,Point,"(33.57, 39.21)"
-SE_ARABIA_556E220N_R,ʿUmān+,,,,regions,Point,"(55.67, 22.01)"
-SE_IRAN_656E286N_R,Sījīstān+,سجستان,سجستان، سيستان,,regions,Point,"(65.61472, 28.62665)"
-SHAM_363E335N_R,al-Šām,الشام,الشام، شام,,regions,Point,"(36.30199, 33.51843)"
-SIQILIYYA_145E375N_R,Ṣiqiliyyaŧ,,,,regions,Point,"(14.5, 37.57)"
-SW_ARABIA_456E158N_R,al-Yaman,اليمن,اليمن,,regions,Point,"(45.68, 15.82)"
-SW_IRAN_540E294N_R,Fārs+,فارس,فارس,,regions,Point,"(54.00, 29.43)"
+ANDALUS_040E398N_R,al-Andalus,الأندلس,الأندلس,,province,Point,"(-4.0521, 39.88926)"
+BARQA_221E314N_R,Barqaŧ,برقة,برقة,,province,Point,"(22.1, 31.4)"
+CENTRAL_ARABIA_416E227N_R,al-Ḥijāz+,الجزيرة,الجزيرة، أقور,,province,Point,"(41.65725, 22.78726)"
+IFRIQIYYA_78E349N_R,Ifriqiyyā,إفريقية,إفريقية,,province,Point,"(7.8, 34.9)"
+IRAQ_459E319N_R,al-ʿIrāq,العراق,العراق,,province,Point,"(45.96, 31.9)"
+JAZIRA_420E364N_R,al-Jazīraŧ,جزيرة,جزيرة، جزيرة العرب,,province,Point,"(42.05, 36.41)"
+MAGHRIB_045E323N_R,al-Maġrib,المغرب,المغرب,,province,Point,"(-4.52149, 32.30201)"
+MAWARANNAHR_656E401N_R,Mā warāʾ al-nahr,ما وراء النهر,ما وراء النهر,,province,Point,"(65.61472, 40.1917)"
+MISR_305E292N_R,Miṣr,مصر,مصر، الديار المصرية,,province,Point,"(30.52, 29.23)"
+NE_IRAN_606E351N_R,Ḫurāsān,خراسان,خراسان,,province,Point,"(60.61524, 35.17917)"
+NW_IRAN_515E356N_R,al-Jibāl+,الجبال,الجبال، الجبل,,province,Point,"(51.50831, 35.62754)"
+QABQ_457E413N_R,al-Riḥāb,الرحاب,الرحاب,,province,Point,"(45.79, 41.33)"
+RUM_335E392N_R,al-Rūm,الروم,الروم، بلد الروم,,province,Point,"(33.57, 39.21)"
+SE_ARABIA_556E220N_R,ʿUmān+,,,,province,Point,"(55.67, 22.01)"
+SE_IRAN_656E286N_R,Sījīstān+,سجستان,سجستان، سيستان,,province,Point,"(65.61472, 28.62665)"
+SHAM_363E335N_R,al-Šām,الشام,الشام، شام,,province,Point,"(36.30199, 33.51843)"
+SIQILIYYA_145E375N_R,Ṣiqiliyyaŧ,,,,province,Point,"(14.5, 37.57)"
+SW_ARABIA_456E158N_R,al-Yaman,اليمن,اليمن,,province,Point,"(45.68, 15.82)"
+SW_IRAN_540E294N_R,Fārs+,فارس,فارس,,province,Point,"(54.00, 29.43)"
```

### Comparing `eis1600-0.9.3/eis1600/helper/EntityTags.py` & `eis1600-0.9.4/eis1600/helper/EntityTags.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/Singleton.py` & `eis1600-0.9.4/eis1600/helper/Singleton.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/ar_normalization.py` & `eis1600-0.9.4/eis1600/helper/ar_normalization.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/fix_miu_annotation.py` & `eis1600-0.9.4/eis1600/helper/fix_miu_annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/markdown_methods.py` & `eis1600-0.9.4/eis1600/helper/markdown_methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/markdown_patterns.py` & `eis1600-0.9.4/eis1600/helper/markdown_patterns.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/miu_random_revisions.py` & `eis1600-0.9.4/eis1600/helper/miu_random_revisions.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/helper/repo.py` & `eis1600-0.9.4/eis1600/helper/repo.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,15 +256,14 @@
     else:
         out_path = '../'
 
         if 'data' in infile:
             out_path += infile.split('data')[0][2:]
         elif infile != './':
             depth = len(infile.split('/'))
-            print(depth)
             if depth == 1:
                 out_path += '../../../../'
             elif depth == 2:
                 out_path += '../../../'
             elif depth == 3:
                 out_path += '../../'
             else:
```

### Comparing `eis1600-0.9.3/eis1600/helper/yml_to_json.py` & `eis1600-0.9.4/eis1600/helper/yml_to_json.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/markdown/UIDs.py` & `eis1600-0.9.4/eis1600/markdown/UIDs.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py` & `eis1600-0.9.4/eis1600/markdown/convert_mARkdown_to_EIS1600TMP.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/markdown/insert_uids.py` & `eis1600-0.9.4/eis1600/markdown/insert_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/markdown/methods.py` & `eis1600-0.9.4/eis1600/markdown/methods.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
     elif md == '$CHR_EVE$':
         return NORMALIZE_BIO_CHR_MD_PATTERN.sub('# @', paragraph)
     elif md == '$CHR_RAW$':
         return NORMALIZE_BIO_CHR_MD_PATTERN.sub('# @@@', paragraph)
     elif md == '@ RAW':
         return NORMALIZE_BIO_CHR_MD_PATTERN.sub('# @@@', paragraph)
     else:
-        print(md)
         return paragraph
 
 
 def convert_to_EIS1600TMP(infile: str, output_dir: Optional[str] = None, verbose: bool = False) -> None:
     """Coverts a file to EIS1600TMP for review process.
 
     Converts mARkdown, inProgress, completed file to light EIS1600TMP for the review process. Creates the file with the
```

### Comparing `eis1600-0.9.3/eis1600/markdown/update_uids.py` & `eis1600-0.9.4/eis1600/markdown/update_uids.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/markdown/update_uids_old_process.py` & `eis1600-0.9.4/eis1600/markdown/update_uids_old_process.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/miu/HeadingTracker.py` & `eis1600-0.9.4/eis1600/miu/HeadingTracker.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/miu/YAMLHandler.py` & `eis1600-0.9.4/eis1600/miu/YAMLHandler.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/miu/disassemble_into_miu_files.py` & `eis1600-0.9.4/eis1600/miu/disassemble_into_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/miu/methods.py` & `eis1600-0.9.4/eis1600/miu/methods.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,18 +4,19 @@
 from pathlib import Path
 
 from eis1600.dates.methods import date_annotate_miu_text
 from eis1600.helper.markdown_patterns import CATEGORY_PATTERN, HEADER_END_PATTERN, HEADING_PATTERN, MIU_TAG_PATTERN, \
     MIU_UID_PATTERN, PAGE_TAG_PATTERN
 from eis1600.miu.HeadingTracker import HeadingTracker
 from eis1600.miu.yml_handling import create_yml_header, extract_yml_header_and_text
-from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text
+from eis1600.nlp.utils import camel2md_as_list, annotate_miu_text, insert_nasab_tag, insert_onomastic_tags
 from eis1600.onomastics.methods import nasab_annotate_miu
 from eis1600.processing.postprocessing import write_updated_miu_to_file
 from eis1600.processing.preprocessing import get_yml_and_miu_df
+from eis1600.toponyms.methods import toponym_category_annotate_miu
 
 
 def disassemble_text(infile: str, out_path: str, verbose: Optional[bool] = None) -> None:
     """Disassemble text into MIU files.
 
     Retrieve MIU files by disassembling the text based on the EIS1600 mARkdown.
     :param str infile: Path to the file which is to be disassembled.
@@ -172,31 +173,39 @@
 
         # 3. convert cameltools labels format to markdown format
         df['NER_TAGS'] = camel2md_as_list(df['NER_LABELS'].tolist())
 
         # 4. annotate dates
         df['DATE_TAGS'] = date_annotate_miu_text(df[['TOKENS']], yml_handler)
 
-        # 5. annotate onomastic information
-        # TODO Needs to be run after the NASAB END tag was inserted
-        df['NASAB_TAGS'] = nasab_annotate_miu(df, yml_handler, path)
+        # 5. insert BNASAB and ENASAB tags with the pretrained transformer model
+        df['NASAB_TAGS'] = insert_nasab_tag(df)
+
+        # 6. annotate onomastic information
+        df['ONONMASTIC_TAGS'] = insert_onomastic_tags(df)
+
+        # 5. annotate onomastic information (Rule-Based model, an alternative to ML model insert_onomastic_tags
+        # df['ONONMASTIC_TAGS'] = nasab_annotate_miu(df, yml_handler, path)
 
         # TODO 6. disambiguation of toponyms (same toponym, different places) --> replace ambigious toponyms flag
-        # TODO 7. toponym categorization
+
+        # 7. toponym categorization
+        df['NER_TAGS'] = toponym_category_annotate_miu(df['TOKENS'], df['NER_TAGS'])
+
         # TODO 8. assign roles for persons
         # TODO 9. get frequencies of unidentified entities (toponyms, nisbas)
 
-        # 6. save csv file
+        # 10. save csv file
         df.to_csv(tsv_path, index=False, sep='\t')
 
-        # 7. reconstruct the text, populate yml with annotated entities and save it to the output file
+        # 11. reconstruct the text, populate yml with annotated entities and save it to the output file
         if output_path == path:
             write_updated_miu_to_file(
                 miu_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NER_TAGS',
-                                                 'DATE_TAGS', 'NASAB_TAGS']]
+                                                 'DATE_TAGS', 'NASAB_TAGS', 'ONONMASTIC_TAGS']]
                 )
         else:
             with open(output_path, 'w', encoding='utf-8') as out_file_object:
                 write_updated_miu_to_file(
                         out_file_object, yml_handler, df[['SECTIONS', 'TOKENS', 'TAGS_LISTS', 'NER_TAGS',
-                                                         'DATE_TAGS', 'NASAB_TAGS']]
+                                                         'DATE_TAGS', 'NASAB_TAGS', 'ONONMASTIC_TAGS']]
                 )
```

### Comparing `eis1600-0.9.3/eis1600/miu/reassemble_from_miu_files.py` & `eis1600-0.9.4/eis1600/miu/reassemble_from_miu_files.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/miu/yml_handling.py` & `eis1600-0.9.4/eis1600/miu/yml_handling.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/nlp/cameltools.py` & `eis1600-0.9.4/eis1600/nlp/cameltools.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,56 @@
 from camel_tools.ner import NERecognizer
 from camel_tools.tokenizers.word import simple_word_tokenize
 from camel_tools.disambig.mle import MLEDisambiguator
 from camel_tools.tagger.default import DefaultTagger
 from camel_tools.utils.dediac import dediac_ar
-
 from typing import Union
 
 
 class CamelToolsModels:
     __pos_tagger = None
     __mled_disambiguator = None
     __lemmatizer = None
     __ner_tagger = None
+    __nasab_tagger = None
+    __onomastic_tagger = None
+    __NASAB_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_nasab/"
+    __NER_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_ner/"
+    __ONOMASTIC_MODEL_PATH = "EIS1600_Pretrained_Models/camelbert-ca-finetuned_onomastic/"
 
     @staticmethod
     def getInstance():
         """ Static access method. """
         if CamelToolsModels.__ner_tagger is None or CamelToolsModels.__lemmatizer is None:
             CamelToolsModels()
         return CamelToolsModels.__ner_tagger, CamelToolsModels.__lemmatizer, CamelToolsModels.__pos_tagger
 
+    @staticmethod
+    def getNasabModel():
+        """ Static access method. """
+        if CamelToolsModels.__nasab_tagger is None:
+            CamelToolsModels.__nasab_tagger = NERecognizer(CamelToolsModels.__NASAB_MODEL_PATH)
+        return CamelToolsModels.__nasab_tagger
+
+    @staticmethod
+    def getOnomasticModel():
+        """ Static access method. """
+        if CamelToolsModels.__onomastic_tagger is None:
+            CamelToolsModels.__onomastic_tagger = NERecognizer(CamelToolsModels.__ONOMASTIC_MODEL_PATH)
+        return CamelToolsModels.__onomastic_tagger
+
     def __init__(self):
         """ Virtually private constructor. """
         if CamelToolsModels.__ner_tagger is not None:
             raise Exception("This class is a singleton!")
         else:
             CamelToolsModels.__mled_disambiguator = MLEDisambiguator.pretrained()
             CamelToolsModels.__lemmatizer = DefaultTagger(CamelToolsModels.__mled_disambiguator, 'lex')
             CamelToolsModels.__pos_tagger = DefaultTagger(CamelToolsModels.__mled_disambiguator, 'pos')
-            CamelToolsModels.__ner_tagger = NERecognizer.pretrained()
+            CamelToolsModels.__ner_tagger = NERecognizer(CamelToolsModels.__NER_MODEL_PATH) # .pretrained
 
 
 def lemmatize_and_tag_ner(tokens: Union[str, list]) -> list:
     """Lemmatize the text and annotate named-entities.
 
         Lemmatize the text and annotated named-entities using Camel Tools models.
         :param tokens: a  string or a list of tokens to be annotated
```

### Comparing `eis1600-0.9.3/eis1600/nlp/ner_annotate_mius.py` & `eis1600-0.9.4/eis1600/nlp/ner_annotate_mius.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 -----
 Give an IDs file or a single MIU file as input
 otherwise 
 all files in the MIU directory are batch processed.
 '''
         )
     arg_parser.add_argument('-v', '--verbose', action='store_true')
+    arg_parser.add_argument('-D', '--debug', action='store_true')
     arg_parser.add_argument('-p', '--parallel', help='parallel processing', action='store_true')
     arg_parser.add_argument('-f', '--force', help='force re-annotation', action='store_true')
     arg_parser.add_argument(
         'input', type=str, nargs='?',
         help='IDs or MIU file to process',
         action=CheckFileEndingAction
         )
```

### Comparing `eis1600-0.9.3/eis1600/onomastics/annotation.py` & `eis1600-0.9.4/eis1600/onomastics/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/onomastics/methods.py` & `eis1600-0.9.4/eis1600/onomastics/methods.py`

 * *Files 2% similar despite different names*

```diff
@@ -163,15 +163,16 @@
 
         m = SPELLING.search(text_updated, m.end() + len(tag))
 
     return text_updated
 
 
 def nasab_annotate_miu(
-        df: DataFrame, yml_handler: YAMLHandler,
+        df: DataFrame,
+        yml_handler: YAMLHandler,
         file: str,
         test: Optional[bool] = False
 ) -> Series:
     """Onomastic analysis of the nasab part of the MIU.
 
     :param DataFrame df: DataFrame of the MIU.
     :param YAMLHandler yml_handler: YAMLHandler of the MIU.
@@ -201,15 +202,15 @@
     blacklist = ['(', ')', '[', ']', '"', "'", '.', '،', '؟', '!', ':', '؛', ',', ';', '?', '|']
     nasab_idx = df.loc[df['TOKENS'].notna() & ~df['TOKENS'].isin(blacklist) & df.index.isin(df.iloc[:idx].index)].index
 
     text = ' '.join(df['TOKENS'].loc[nasab_idx])
 
     tagged_spelling = tag_spelling(text)
     ar_tokens, tags = get_tokens_and_tags(tagged_spelling)
-    df.loc[nasab_idx, 'NASAB_TAGS'] = tags
+    df.loc[nasab_idx, 'ONONMASTIC_TAGS'] = tags
 
     count = 0
     spl_idcs = []
     for row in df.loc[nasab_idx].itertuples():
         if notna(row[4]):
             count = int(row[4][-1])
         if count > 0:
@@ -218,25 +219,29 @@
 
     nasab_idx = df.loc[nasab_idx.difference(spl_idcs)].index
     text = ' '.join(df['TOKENS'].loc[nasab_idx])
 
     text_w_mnpld_nas = get_nas(text)
     tagged_onomastics = tag_nasab(text_w_mnpld_nas)
     ar_tokens, tags = get_tokens_and_tags(tagged_onomastics)
-    df.loc[nasab_idx, 'NASAB_TAGS'] = tags
+    df.loc[nasab_idx, 'ONONMASTIC_TAGS'] = tags
 
     if idx != len(df):
         # TODO make NASAB stay on same line
         df.loc[idx - 1, 'NASAB_END'] = 'NASAB'
 
-    return df['NASAB_TAGS'].to_list()
+    return df['ONONMASTIC_TAGS'].to_list()
 
 
-def nasab_annotation(file: str, test: bool):
-    """Only used for onomastic_annotation cmdline script."""
+def nasab_annotation(file: str, test: Optional[bool] = False):
+    """Helper to run onomastic annotation standalone as cmdline script.
+
+    :param str file: Path of the miu file to annotate.
+    :param bool test: Indicating if the script is run with test data, defaults to false.
+    """
     with open(file, 'r', encoding='utf-8') as miu_file_object:
         yml_handler, df = get_yml_and_miu_df(miu_file_object)
     if test:
         # Only used if run on training_data batch because this information is missing there
         if '$' not in df.iloc[0]['SECTIONS'] or '$$$' in df.iloc[0]['SECTIONS'] or not yml_handler.is_reviewed():
             df['NASAB_TAGS'] = Series([nan] * len(df))
         else:
```

### Comparing `eis1600-0.9.3/eis1600/onomastics/re_pattern.py` & `eis1600-0.9.4/eis1600/onomastics/re_pattern.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/processing/postprocessing.py` & `eis1600-0.9.4/eis1600/processing/postprocessing.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     :param TextIO miu_file_object: Path to the MIU file to write
     :param YAMLHandler yml_handler: The YAMLHandler of the MIU.
     :param DataFrame df: df containing the columns ['SECTIONS', 'TOKENS', 'TAGS_LISTS'] and optional 'ÜTAGS_LISTS'.
     :return None:
     """
     if not yml_handler.is_reviewed():
-        columns_of_automated_tags = ['NER_TAGS', 'DATE_TAGS', 'NASAB_TAGS']
+        columns_of_automated_tags = ['NER_TAGS', 'DATE_TAGS', 'NASAB_TAGS', 'ONONMASTIC_TAGS']
         df['ÜTAGS'] = df['TAGS_LISTS']
         for col in columns_of_automated_tags:
             if col in df.columns:
                 df['ÜTAGS'] = df.apply(lambda x: merge_tagslists(x['ÜTAGS'], x[col]), axis=1)
         df_subset = df[['SECTIONS', 'TOKENS', 'ÜTAGS']]
     else:
         df_subset = df[['SECTIONS', 'TOKENS', 'TAGS_LISTS']]
```

### Comparing `eis1600-0.9.3/eis1600/processing/preprocessing.py` & `eis1600-0.9.4/eis1600/processing/preprocessing.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/stats/methods.py` & `eis1600-0.9.4/eis1600/stats/methods.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/stats/miu_stats.py` & `eis1600-0.9.4/eis1600/stats/miu_stats.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/toponyms/annotation.py` & `eis1600-0.9.4/eis1600/toponyms/annotation.py`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600/toponyms/toponym_categories.py` & `eis1600-0.9.4/eis1600/toponyms/toponym_categories.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,13 +8,13 @@
 TOPONYM_CATEGORIES = {
         'ولد': 'B', 'مولد': 'B',
         'مات': 'D', 'موت': 'D', 'توفي': 'D', 'وفاة': 'D',
         'حج': 'P',
         'سمع': 'K', 'روى': 'K', 'روا': 'K', 'قرا': 'K', 'اجاز': 'K',
         'استقر': 'O', 'انفصل': 'O', 'ولي': 'O', 'قاضي': 'O', 'أعمال': 'O',
         'لقي': 'M',
-        'سكن': 'L', 'نزل': 'L', 'نزيل': 'L', 'من اهل': 'L', 'استوطن': 'L', 'كان من': 'L'
+        'سكن': 'R', 'نزل': 'R', 'نزيل': 'R', 'من اهل': 'R', 'استوطن': 'R', 'كان من': 'R'
 }
 TOPONYM_CATEGORIES_NOR = normalize_dict(TOPONYM_CATEGORIES)
 
 AR_TOPONYM_CATEGORIES = '|'.join([denormalize(key) for key in TOPONYM_CATEGORIES.keys()])
 TOPONYM_CATEGORY_PATTERN = compile(r'\s[وف]?(?P<topo_category>' + AR_TOPONYM_CATEGORIES + r')')
```

### Comparing `eis1600-0.9.3/eis1600.egg-info/PKG-INFO` & `eis1600-0.9.4/eis1600.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eis1600
-Version: 0.9.3
+Version: 0.9.4
 Summary: EIS1600 project tools and utilities
 Home-page: https://github.com/EIS1600/eis1600-pkg
 Author: Lisa Mischer
 Author-email: mischer.lisa@gmail.com
 License: MIT License
 Description: # EIS1600 Tools
         
@@ -49,14 +49,16 @@
         ```
         
         In case you have an older version installed, use:
         ```shell
         $ pip install --upgrade eis1600
         ```
         
+        **Note**. You can use `pip freeze` to check the versions of all installed packages, including `eis1600`.
+        
         ## Set Up Virtual Environment and Install the EIS1600 PKG there
         
         To not mess with other python installations, we recommend installing the package in a virual environment.
         To create a new virtual environment with python, run:
         ```shell
         python3 -m venv eis1600_env
         ```
@@ -99,14 +101,15 @@
         The working directory is always the main `EIS1600` directory which is a parent to all the different repositories.
         The `EIS1600` directory has the following structure:
         
         ```
         |
         |---| eis_env
         |---| EIS1600_MIUs
+        |---| EIS1600_Pretrained_Models (optional)
         |---| gazetteers
         |---| Master_Chronicle
         |---| OpenITI_EIS1600_Texts
         |---| Training_Data
         ```
         
         Path variables are in the module `eis1600/helper/repo`.
@@ -167,33 +170,35 @@
         Use the `-e` option to process all files from the MIU repo. Must be run from the root of MIU repo.
         ```shell
         $ reassemble_from_miu_files -e <MIU_repo>
         ```
         
         ### Annotation
         
-        NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastics.
+        NER annotation for persons, toponyms, misc, and also dates, beginning and ending of onomastic information (*NASAB*), and onomastic information.
+        
+        **Note** Can only be run if package was installed with *NER* flag AND if the ML models are in the [EIS1600_Pretrained_Models](#structure-of-the-working-directory) directory.
+        
+        If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
+        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `EIS1600_MIUs/`).
+        ```shell
+        $ annotate_mius -p
+        ```
         
         To annotate all MIU files of a text give the IDs file as argument.
         Can be used with `-p` option to run in parallel.
         ```shell
         $ annotate_mius <uri>.IDs
         ```
         
         To annotate an individual MIU file, give MIU file as argument.
         ```shell
         $ annotate_mius <uri>/MIUs/<uri>.<UID>.EIS1600
         ```
         
-        If no input is given, annotation is run for the whole repository. Can be used with `-p` option for parallelization.
-        Run from the [parent directory](#structure-of-the-working-directory) `EIS1600` (internally used path starts with: `OpenITI_EIS1600_MIUs/`).
-        ```shell
-        $ annotate_mius -p
-        ```
-        
         ### Only Onomastic Annotation
         
         **Only for test purposes!**
         Can be run with `-D` to process one file at a time, otherwise runs in parallel.
         Can be run with `-T` to use gold-standard data as input.
         Run from the [parent directory](#structure-of-the-working-directory) `EIS1600`.
         ```shell
```

### Comparing `eis1600-0.9.3/eis1600.egg-info/SOURCES.txt` & `eis1600-0.9.4/eis1600.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/eis1600.egg-info/entry_points.txt` & `eis1600-0.9.4/eis1600.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `eis1600-0.9.3/setup.py` & `eis1600-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(name='eis1600',
-      version='0.9.3',
+      version='0.9.4',
       description='EIS1600 project tools and utilities',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/EIS1600/eis1600-pkg',
       author='Lisa Mischer',
       author_email='mischer.lisa@gmail.com',
       license='MIT License',
```

