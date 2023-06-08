# Comparing `tmp/SC_BCSFE-1.1.5.tar.gz` & `tmp/SC_BCSFE-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SC_BCSFE-1.1.5.tar", last modified: Thu Jun  8 13:34:06 2023, max compression
+gzip compressed data, was "SC_BCSFE-1.1.6.tar", last modified: Thu Jun  8 13:36:41 2023, max compression
```

## Comparing `SC_BCSFE-1.1.5.tar` & `SC_BCSFE-1.1.6.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.458830 SC_BCSFE-1.1.5/
--rw-r--r--   0 hayun      (502) staff       (20)      712 2023-06-08 13:34:06.459772 SC_BCSFE-1.1.5/PKG-INFO
--rw-rw-rw-   0 hayun      (502) staff       (20)      198 2023-04-27 07:59:41.000000 SC_BCSFE-1.1.5/README.md
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.060468 SC_BCSFE-1.1.5/SC_BCSFE.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)      712 2023-06-08 13:34:05.000000 SC_BCSFE-1.1.5/SC_BCSFE.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     2955 2023-06-08 13:34:05.000000 SC_BCSFE-1.1.5/SC_BCSFE.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-08 13:34:05.000000 SC_BCSFE-1.1.5/SC_BCSFE.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-08 13:34:05.000000 SC_BCSFE-1.1.5/SC_BCSFE.egg-info/top_level.txt
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.173159 SC_BCSFE-1.1.5/SC_Editor/
--rw-rw-rw-   0 hayun      (502) staff       (20)      281 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     8261 2023-06-08 13:28:54.000000 SC_BCSFE-1.1.5/SC_Editor/__main__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    10240 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/adb_handler.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    13764 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/config_manager.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1501 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.177120 SC_BCSFE-1.1.5/SC_Editor/edits/
--rw-rw-rw-   0 hayun      (502) staff       (20)       67 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.220947 SC_BCSFE-1.1.5/SC_Editor/edits/basic/
--rw-rw-rw-   0 hayun      (502) staff       (20)      122 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     8976 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/basic_items.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1490 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/catfruit.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1931 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/catseyes.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1647 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     4041 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/talent_orbs.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    16755 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.274979 SC_BCSFE-1.1.5/SC_Editor/edits/cats/
--rw-rw-rw-   0 hayun      (502) staff       (20)      179 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     8994 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/cat_helper.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    11449 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/cat_id_selector.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3262 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/chara_drop.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1083 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2883 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/evolve_cats.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1277 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/get_remove_cats.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     8065 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/talents.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1900 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/upgrade_blue.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     4634 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.307479 SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/
--rw-rw-rw-   0 hayun      (502) staff       (20)       66 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      333 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2835 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3399 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/helpers.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     4130 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.375074 SC_BCSFE-1.1.5/SC_Editor/edits/levels/
--rw-rw-rw-   0 hayun      (502) staff       (20)      313 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1057 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/aku.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      516 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      869 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/behemoth_culling.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      650 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/clear_tutorial.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1121 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/enigma_stages.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     6389 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/event_stages.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2062 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/gauntlet.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1056 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1481 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/legend_quest.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     4451 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/main_story.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2361 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/outbreaks.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3106 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1227 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/towers.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     8576 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/treasures.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1082 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/uncanny.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      802 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.440153 SC_BCSFE-1.1.5/SC_Editor/edits/other/
--rw-rw-rw-   0 hayun      (502) staff       (20)      276 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3913 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/cat_shrine.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1124 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1054 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/create_new_account.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2236 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/fix_elsewhere.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      698 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/fix_time_issues.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3510 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/get_gold_pass.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7142 2023-06-08 09:12:41.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/meow_medals.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     4384 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/missions.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1016 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/play_time.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     4568 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/scheme_item.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1657 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/trade_progress.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1426 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      356 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:34:06.454683 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/
--rw-rw-rw-   0 hayun      (502) staff       (20)       56 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/__init__.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1308 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/convert.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2795 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/load.py
--rw-rw-rw-   0 hayun      (502) staff       (20)      661 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/other.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2049 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/save.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1906 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/edits/save_management/server_upload.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    13855 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/feature_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6664 2023-06-08 09:12:37.000000 SC_BCSFE-1.1.5/SC_Editor/game_data_getter.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    23001 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/helper.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     7075 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/item.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3505 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/locale_handler.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1269 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/managed_item.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    66980 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/parse_save.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     1301 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/patcher.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     2450 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/root_handler.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    53823 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/serialise_save.py
--rw-rw-rw-   0 hayun      (502) staff       (20)    25211 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/server_handler.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3717 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/tracker.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     3544 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/updater.py
--rw-rw-rw-   0 hayun      (502) staff       (20)     8297 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.5/SC_Editor/user_input_handler.py
--rw-rw-rw-   0 hayun      (502) staff       (20)       38 2023-06-08 13:34:06.464222 SC_BCSFE-1.1.5/setup.cfg
--rw-rw-rw-   0 hayun      (502) staff       (20)      969 2023-06-08 13:34:00.000000 SC_BCSFE-1.1.5/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.974055 SC_BCSFE-1.1.6/
+-rw-r--r--   0 hayun      (502) staff       (20)      712 2023-06-08 13:36:41.974294 SC_BCSFE-1.1.6/PKG-INFO
+-rw-rw-rw-   0 hayun      (502) staff       (20)      198 2023-04-27 07:59:41.000000 SC_BCSFE-1.1.6/README.md
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.859274 SC_BCSFE-1.1.6/SC_BCSFE.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)      712 2023-06-08 13:36:41.000000 SC_BCSFE-1.1.6/SC_BCSFE.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     2955 2023-06-08 13:36:41.000000 SC_BCSFE-1.1.6/SC_BCSFE.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-08 13:36:41.000000 SC_BCSFE-1.1.6/SC_BCSFE.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-08 13:36:41.000000 SC_BCSFE-1.1.6/SC_BCSFE.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.876957 SC_BCSFE-1.1.6/SC_Editor/
+-rw-rw-rw-   0 hayun      (502) staff       (20)      281 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     8201 2023-06-08 13:36:22.000000 SC_BCSFE-1.1.6/SC_Editor/__main__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    10240 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/adb_handler.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    13764 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/config_manager.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1501 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.877375 SC_BCSFE-1.1.6/SC_Editor/edits/
+-rw-rw-rw-   0 hayun      (502) staff       (20)       67 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.887129 SC_BCSFE-1.1.6/SC_Editor/edits/basic/
+-rw-rw-rw-   0 hayun      (502) staff       (20)      122 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     8976 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/basic_items.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1490 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/catfruit.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1931 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/catseyes.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1647 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     4041 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/talent_orbs.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    16755 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.907483 SC_BCSFE-1.1.6/SC_Editor/edits/cats/
+-rw-rw-rw-   0 hayun      (502) staff       (20)      179 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     8994 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/cat_helper.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    11449 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3262 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/chara_drop.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1083 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2883 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/evolve_cats.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1277 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     8065 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/talents.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1900 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     4634 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.916720 SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/
+-rw-rw-rw-   0 hayun      (502) staff       (20)       66 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      333 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2835 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3399 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/helpers.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     4130 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.944299 SC_BCSFE-1.1.6/SC_Editor/edits/levels/
+-rw-rw-rw-   0 hayun      (502) staff       (20)      313 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1057 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/aku.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      516 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      869 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      650 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1121 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/enigma_stages.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     6389 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/event_stages.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2062 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/gauntlet.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1056 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1481 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/legend_quest.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     4451 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/main_story.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2361 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/outbreaks.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3106 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1227 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/towers.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     8576 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/treasures.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1082 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/uncanny.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      802 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.962779 SC_BCSFE-1.1.6/SC_Editor/edits/other/
+-rw-rw-rw-   0 hayun      (502) staff       (20)      276 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3913 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/cat_shrine.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1124 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1054 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/create_new_account.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2236 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      698 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/fix_time_issues.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3510 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/get_gold_pass.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7142 2023-06-08 09:12:41.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/meow_medals.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     4384 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/missions.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1016 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/play_time.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     4568 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/scheme_item.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1657 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/trade_progress.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1426 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      356 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 13:36:41.973252 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/
+-rw-rw-rw-   0 hayun      (502) staff       (20)       56 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/__init__.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1308 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/convert.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2795 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/load.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)      661 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/other.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2049 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/save.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1906 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/edits/save_management/server_upload.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    13855 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/feature_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6664 2023-06-08 09:12:37.000000 SC_BCSFE-1.1.6/SC_Editor/game_data_getter.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    23001 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/helper.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     7075 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/item.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3505 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/locale_handler.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1269 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/managed_item.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    66980 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/parse_save.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     1301 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/patcher.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     2450 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/root_handler.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    53823 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/serialise_save.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)    25211 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/server_handler.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3717 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/tracker.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     3544 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/updater.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)     8297 2023-05-18 13:57:31.000000 SC_BCSFE-1.1.6/SC_Editor/user_input_handler.py
+-rw-rw-rw-   0 hayun      (502) staff       (20)       38 2023-06-08 13:36:41.974953 SC_BCSFE-1.1.6/setup.cfg
+-rw-rw-rw-   0 hayun      (502) staff       (20)      969 2023-06-08 13:36:35.000000 SC_BCSFE-1.1.6/setup.py
```

### Comparing `SC_BCSFE-1.1.5/PKG-INFO` & `SC_BCSFE-1.1.6/SC_BCSFE.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SC_BCSFE
-Version: 1.1.5
+Name: SC-BCSFE
+Version: 1.1.6
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Platform: UNKNOWN
```

### Comparing `SC_BCSFE-1.1.5/SC_BCSFE.egg-info/PKG-INFO` & `SC_BCSFE-1.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: SC-BCSFE
-Version: 1.1.5
+Name: SC_BCSFE
+Version: 1.1.6
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Platform: UNKNOWN
```

### Comparing `SC_BCSFE-1.1.5/SC_BCSFE.egg-info/SOURCES.txt` & `SC_BCSFE-1.1.6/SC_BCSFE.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/__main__.py` & `SC_BCSFE-1.1.6/SC_Editor/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
         helper.colored_text(
             base=helper.RED,
             new=helper.WHITE,
         )
     print()
     helper.colored_text(
         f"{locale_manager.search_key('thanks_title')}\n"
-        + f"{locale_manager.search_key('thanks_title2')}\n"
         + f"{locale_manager.search_key('blacklist')}\n"
         + f"{locale_manager.search_key('lethal_thanks')}\n"
         + f"{locale_manager.search_key('beeven_cse_thanks')}\n"
         + f"{locale_manager.search_key('support_thanks')}\n"
         + locale_manager.search_key("discord_thanks"),
         base=helper.GREEN,
         new=helper.WHITE,
```

### Comparing `SC_BCSFE-1.1.5/SC_Editor/adb_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/adb_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/config_manager.py` & `SC_BCSFE-1.1.6/SC_Editor/config_manager.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/csv_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/csv_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/basic/basic_items.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/basic/catfruit.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/basic/catseyes.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/basic/ototo_base_mats.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/basic/talent_orbs.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/basic/talent_orbs_new.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/cat_helper.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/cat_id_selector.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/chara_drop.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/clear_cat_guide.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/evolve_cats.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/get_remove_cats.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/talents.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/upgrade_blue.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/cats/upgrade_cats.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/gamatoto_xp.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/helpers.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/gamototo/ototo_cat_cannon.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/aku.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/allow_filibuster_clearing.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/behemoth_culling.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/clear_tutorial.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/enigma_stages.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/event_stages.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/gauntlet.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/itf_timed_scores.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/legend_quest.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/main_story.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/outbreaks.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/story_level_id_selector.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/towers.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/treasures.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/uncanny.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/levels/unlock_aku_realm.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/cat_shrine.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/claim_user_rank_rewards.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/create_new_account.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/fix_elsewhere.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/fix_time_issues.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/get_gold_pass.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/meow_medals.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/missions.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/play_time.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/scheme_item.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/trade_progress.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/other/unlock_enemy_guide.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/save_management/convert.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/save_management/load.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/save_management/other.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/save_management/save.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/edits/save_management/server_upload.py` & `SC_BCSFE-1.1.6/SC_Editor/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/feature_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/feature_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/game_data_getter.py` & `SC_BCSFE-1.1.6/SC_Editor/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/helper.py` & `SC_BCSFE-1.1.6/SC_Editor/helper.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/item.py` & `SC_BCSFE-1.1.6/SC_Editor/item.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/locale_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/locale_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/managed_item.py` & `SC_BCSFE-1.1.6/SC_Editor/managed_item.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/parse_save.py` & `SC_BCSFE-1.1.6/SC_Editor/parse_save.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/patcher.py` & `SC_BCSFE-1.1.6/SC_Editor/patcher.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/root_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/root_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/serialise_save.py` & `SC_BCSFE-1.1.6/SC_Editor/serialise_save.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/server_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/server_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/tracker.py` & `SC_BCSFE-1.1.6/SC_Editor/tracker.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/updater.py` & `SC_BCSFE-1.1.6/SC_Editor/updater.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/SC_Editor/user_input_handler.py` & `SC_BCSFE-1.1.6/SC_Editor/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `SC_BCSFE-1.1.5/setup.py` & `SC_BCSFE-1.1.6/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 basedir = path.abspath(path.dirname(__file__))
 with open(path.join(basedir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read().replace('\r\n', '\n')
 
 setup(
     name='SC_BCSFE',
-    version='1.1.5',
+    version='1.1.6',
     description='냥코에디터 한글화',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='익명',
     author_email='',
     url='https://github.com/sharkwodm/koreditor',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
```

