# Comparing `tmp/Shark sac Korean editor-1.1.0.tar.gz` & `tmp/Shark sac Korean editor-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Shark sac Korean editor-1.1.0.tar", last modified: Thu May 18 14:19:03 2023, max compression
+gzip compressed data, was "Shark sac Korean editor-1.1.1.tar", last modified: Thu Jun  8 13:52:53 2023, max compression
```

## Comparing `Shark sac Korean editor-1.1.0.tar` & `Shark sac Korean editor-1.1.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.709972 Shark sac Korean editor-1.1.0/
--rw-rw-rw-   0        0        0      731 2023-05-18 14:19:03.709972 Shark sac Korean editor-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-1.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.645940 Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/
--rw-rw-rw-   0        0        0      731 2023-05-18 14:19:03.000000 Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2689 2023-05-18 14:19:03.000000 Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 14:19:03.000000 Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 14:19:03.000000 Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.660538 Shark sac Korean editor-1.1.0/modkr/
--rw-rw-rw-   0        0        0      281 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/__init__.py
--rw-rw-rw-   0        0        0     9149 2023-05-18 14:14:41.000000 Shark sac Korean editor-1.1.0/modkr/__main__.py
--rw-rw-rw-   0        0        0    10240 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/adb_handler.py
--rw-rw-rw-   0        0        0    13764 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/config_manager.py
--rw-rw-rw-   0        0        0     1501 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/csv_handler.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.662011 Shark sac Korean editor-1.1.0/modkr/edits/
--rw-rw-rw-   0        0        0       67 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.667910 Shark sac Korean editor-1.1.0/modkr/edits/basic/
--rw-rw-rw-   0        0        0      122 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/__init__.py
--rw-rw-rw-   0        0        0     8976 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/basic_items.py
--rw-rw-rw-   0        0        0     1490 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/catfruit.py
--rw-rw-rw-   0        0        0     1931 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/catseyes.py
--rw-rw-rw-   0        0        0     1647 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/ototo_base_mats.py
--rw-rw-rw-   0        0        0     4041 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/talent_orbs.py
--rw-rw-rw-   0        0        0    16755 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/basic/talent_orbs_new.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.676332 Shark sac Korean editor-1.1.0/modkr/edits/cats/
--rw-rw-rw-   0        0        0      179 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/__init__.py
--rw-rw-rw-   0        0        0     8994 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/cat_helper.py
--rw-rw-rw-   0        0        0    11449 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/cat_id_selector.py
--rw-rw-rw-   0        0        0     3262 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/chara_drop.py
--rw-rw-rw-   0        0        0     1083 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/clear_cat_guide.py
--rw-rw-rw-   0        0        0     2883 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/evolve_cats.py
--rw-rw-rw-   0        0        0     1277 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/get_remove_cats.py
--rw-rw-rw-   0        0        0     8065 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/talents.py
--rw-rw-rw-   0        0        0     1900 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/upgrade_blue.py
--rw-rw-rw-   0        0        0     4634 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/cats/upgrade_cats.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.680318 Shark sac Korean editor-1.1.0/modkr/edits/gamototo/
--rw-rw-rw-   0        0        0       66 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/gamototo/__init__.py
--rw-rw-rw-   0        0        0      333 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/gamototo/fix_gamatoto.py
--rw-rw-rw-   0        0        0     2835 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/gamototo/gamatoto_xp.py
--rw-rw-rw-   0        0        0     3399 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/gamototo/helpers.py
--rw-rw-rw-   0        0        0     4130 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/gamototo/ototo_cat_cannon.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.693222 Shark sac Korean editor-1.1.0/modkr/edits/levels/
--rw-rw-rw-   0        0        0      313 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/aku.py
--rw-rw-rw-   0        0        0      516 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/allow_filibuster_clearing.py
--rw-rw-rw-   0        0        0      869 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/behemoth_culling.py
--rw-rw-rw-   0        0        0      650 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/clear_tutorial.py
--rw-rw-rw-   0        0        0     1121 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/enigma_stages.py
--rw-rw-rw-   0        0        0     6389 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/event_stages.py
--rw-rw-rw-   0        0        0     2062 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/gauntlet.py
--rw-rw-rw-   0        0        0     1056 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/itf_timed_scores.py
--rw-rw-rw-   0        0        0     1481 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/legend_quest.py
--rw-rw-rw-   0        0        0     4451 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/main_story.py
--rw-rw-rw-   0        0        0     2361 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/outbreaks.py
--rw-rw-rw-   0        0        0     3106 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/story_level_id_selector.py
--rw-rw-rw-   0        0        0     1227 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/towers.py
--rw-rw-rw-   0        0        0     8576 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/treasures.py
--rw-rw-rw-   0        0        0     1082 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/uncanny.py
--rw-rw-rw-   0        0        0      802 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/levels/unlock_aku_realm.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.705182 Shark sac Korean editor-1.1.0/modkr/edits/other/
--rw-rw-rw-   0        0        0      276 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/__init__.py
--rw-rw-rw-   0        0        0     3913 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/cat_shrine.py
--rw-rw-rw-   0        0        0     1124 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/claim_user_rank_rewards.py
--rw-rw-rw-   0        0        0     1054 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/create_new_account.py
--rw-rw-rw-   0        0        0     2236 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/fix_elsewhere.py
--rw-rw-rw-   0        0        0      698 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/fix_time_issues.py
--rw-rw-rw-   0        0        0     3510 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/get_gold_pass.py
--rw-rw-rw-   0        0        0     7140 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/meow_medals.py
--rw-rw-rw-   0        0        0     4384 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/missions.py
--rw-rw-rw-   0        0        0     1016 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/play_time.py
--rw-rw-rw-   0        0        0     4568 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/scheme_item.py
--rw-rw-rw-   0        0        0     1657 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/trade_progress.py
--rw-rw-rw-   0        0        0     1426 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/unlock_enemy_guide.py
--rw-rw-rw-   0        0        0      356 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/other/unlock_equip_menu.py
-drwxrwxrwx   0        0        0        0 2023-05-18 14:19:03.709972 Shark sac Korean editor-1.1.0/modkr/edits/save_management/
--rw-rw-rw-   0        0        0       56 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/save_management/__init__.py
--rw-rw-rw-   0        0        0     1308 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/save_management/convert.py
--rw-rw-rw-   0        0        0     2795 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/save_management/load.py
--rw-rw-rw-   0        0        0      661 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/save_management/other.py
--rw-rw-rw-   0        0        0     2049 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/save_management/save.py
--rw-rw-rw-   0        0        0     1906 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/edits/save_management/server_upload.py
--rw-rw-rw-   0        0        0    13855 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/feature_handler.py
--rw-rw-rw-   0        0        0     4822 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/game_data_getter.py
--rw-rw-rw-   0        0        0    23001 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/helper.py
--rw-rw-rw-   0        0        0     7075 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/item.py
--rw-rw-rw-   0        0        0     3505 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/locale_handler.py
--rw-rw-rw-   0        0        0     1269 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/managed_item.py
--rw-rw-rw-   0        0        0    66980 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/parse_save.py
--rw-rw-rw-   0        0        0     1301 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/patcher.py
--rw-rw-rw-   0        0        0     2450 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/root_handler.py
--rw-rw-rw-   0        0        0    53823 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/serialise_save.py
--rw-rw-rw-   0        0        0    25211 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/server_handler.py
--rw-rw-rw-   0        0        0     3717 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/tracker.py
--rw-rw-rw-   0        0        0     3544 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/updater.py
--rw-rw-rw-   0        0        0     8297 2023-05-18 13:57:31.000000 Shark sac Korean editor-1.1.0/modkr/user_input_handler.py
--rw-rw-rw-   0        0        0       42 2023-05-18 14:19:03.709972 Shark sac Korean editor-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-05-18 14:17:41.000000 Shark sac Korean editor-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.407198 Shark sac Korean editor-1.1.1/
+-rw-rw-rw-   0        0        0      731 2023-06-08 13:52:53.407198 Shark sac Korean editor-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      198 2023-04-27 07:59:41.000000 Shark sac Korean editor-1.1.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.338556 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/
+-rw-rw-rw-   0        0        0      731 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2689 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 13:52:53.000000 Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.354627 Shark sac Korean editor-1.1.1/modkr/
+-rw-rw-rw-   0        0        0      281 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/__init__.py
+-rw-rw-rw-   0        0        0     9149 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/__main__.py
+-rw-rw-rw-   0        0        0    10240 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/adb_handler.py
+-rw-rw-rw-   0        0        0    13764 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/config_manager.py
+-rw-rw-rw-   0        0        0     1501 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/csv_handler.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.355623 Shark sac Korean editor-1.1.1/modkr/edits/
+-rw-rw-rw-   0        0        0       67 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.361501 Shark sac Korean editor-1.1.1/modkr/edits/basic/
+-rw-rw-rw-   0        0        0      122 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/__init__.py
+-rw-rw-rw-   0        0        0     8976 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/basic_items.py
+-rw-rw-rw-   0        0        0     1490 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/catfruit.py
+-rw-rw-rw-   0        0        0     1931 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/catseyes.py
+-rw-rw-rw-   0        0        0     1647 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/ototo_base_mats.py
+-rw-rw-rw-   0        0        0     4041 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs.py
+-rw-rw-rw-   0        0        0    16755 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs_new.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.370337 Shark sac Korean editor-1.1.1/modkr/edits/cats/
+-rw-rw-rw-   0        0        0      179 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/__init__.py
+-rw-rw-rw-   0        0        0     8994 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_helper.py
+-rw-rw-rw-   0        0        0    11449 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_id_selector.py
+-rw-rw-rw-   0        0        0     3262 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/chara_drop.py
+-rw-rw-rw-   0        0        0     1083 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/clear_cat_guide.py
+-rw-rw-rw-   0        0        0     2883 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/evolve_cats.py
+-rw-rw-rw-   0        0        0     1277 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/get_remove_cats.py
+-rw-rw-rw-   0        0        0     8065 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/talents.py
+-rw-rw-rw-   0        0        0     1900 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_blue.py
+-rw-rw-rw-   0        0        0     4634 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_cats.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.373830 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/
+-rw-rw-rw-   0        0        0       66 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/__init__.py
+-rw-rw-rw-   0        0        0      333 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/fix_gamatoto.py
+-rw-rw-rw-   0        0        0     2835 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/gamatoto_xp.py
+-rw-rw-rw-   0        0        0     3399 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/helpers.py
+-rw-rw-rw-   0        0        0     4130 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/gamototo/ototo_cat_cannon.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.389190 Shark sac Korean editor-1.1.1/modkr/edits/levels/
+-rw-rw-rw-   0        0        0      313 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/aku.py
+-rw-rw-rw-   0        0        0      516 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/allow_filibuster_clearing.py
+-rw-rw-rw-   0        0        0      869 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/behemoth_culling.py
+-rw-rw-rw-   0        0        0      650 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/clear_tutorial.py
+-rw-rw-rw-   0        0        0     1121 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/enigma_stages.py
+-rw-rw-rw-   0        0        0     6389 2023-06-08 13:45:09.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/event_stages.py
+-rw-rw-rw-   0        0        0     2062 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/gauntlet.py
+-rw-rw-rw-   0        0        0     1056 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/itf_timed_scores.py
+-rw-rw-rw-   0        0        0     1481 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/legend_quest.py
+-rw-rw-rw-   0        0        0     4451 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/main_story.py
+-rw-rw-rw-   0        0        0     2361 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/outbreaks.py
+-rw-rw-rw-   0        0        0     3106 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/story_level_id_selector.py
+-rw-rw-rw-   0        0        0     1227 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/towers.py
+-rw-rw-rw-   0        0        0     8576 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/treasures.py
+-rw-rw-rw-   0        0        0     1082 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/uncanny.py
+-rw-rw-rw-   0        0        0      802 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/levels/unlock_aku_realm.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.401219 Shark sac Korean editor-1.1.1/modkr/edits/other/
+-rw-rw-rw-   0        0        0      276 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/__init__.py
+-rw-rw-rw-   0        0        0     3913 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/cat_shrine.py
+-rw-rw-rw-   0        0        0     1124 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/claim_user_rank_rewards.py
+-rw-rw-rw-   0        0        0     1054 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/create_new_account.py
+-rw-rw-rw-   0        0        0     2236 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/fix_elsewhere.py
+-rw-rw-rw-   0        0        0      698 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/fix_time_issues.py
+-rw-rw-rw-   0        0        0     3510 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/get_gold_pass.py
+-rw-rw-rw-   0        0        0     7142 2023-06-08 13:49:33.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/meow_medals.py
+-rw-rw-rw-   0        0        0     4384 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/missions.py
+-rw-rw-rw-   0        0        0     1016 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/play_time.py
+-rw-rw-rw-   0        0        0     4568 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/scheme_item.py
+-rw-rw-rw-   0        0        0     1657 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/trade_progress.py
+-rw-rw-rw-   0        0        0     1426 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/unlock_enemy_guide.py
+-rw-rw-rw-   0        0        0      356 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/other/unlock_equip_menu.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:52:53.406199 Shark sac Korean editor-1.1.1/modkr/edits/save_management/
+-rw-rw-rw-   0        0        0       56 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/__init__.py
+-rw-rw-rw-   0        0        0     1308 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/convert.py
+-rw-rw-rw-   0        0        0     2795 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/load.py
+-rw-rw-rw-   0        0        0      661 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/other.py
+-rw-rw-rw-   0        0        0     2049 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/save.py
+-rw-rw-rw-   0        0        0     1906 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/edits/save_management/server_upload.py
+-rw-rw-rw-   0        0        0    13855 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/feature_handler.py
+-rw-rw-rw-   0        0        0     6664 2023-06-08 13:50:04.000000 Shark sac Korean editor-1.1.1/modkr/game_data_getter.py
+-rw-rw-rw-   0        0        0    23001 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/helper.py
+-rw-rw-rw-   0        0        0     7075 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/item.py
+-rw-rw-rw-   0        0        0     3505 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/locale_handler.py
+-rw-rw-rw-   0        0        0     1269 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/managed_item.py
+-rw-rw-rw-   0        0        0    66980 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/parse_save.py
+-rw-rw-rw-   0        0        0     1301 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/patcher.py
+-rw-rw-rw-   0        0        0     2450 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/root_handler.py
+-rw-rw-rw-   0        0        0    53823 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/serialise_save.py
+-rw-rw-rw-   0        0        0    25211 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/server_handler.py
+-rw-rw-rw-   0        0        0     3717 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/tracker.py
+-rw-rw-rw-   0        0        0     3544 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/updater.py
+-rw-rw-rw-   0        0        0     8297 2023-05-18 14:19:34.000000 Shark sac Korean editor-1.1.1/modkr/user_input_handler.py
+-rw-rw-rw-   0        0        0       42 2023-06-08 13:52:53.407198 Shark sac Korean editor-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-06-08 13:51:19.000000 Shark sac Korean editor-1.1.1/setup.py
```

### Comparing `Shark sac Korean editor-1.1.0/PKG-INFO` & `Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Shark sac Korean editor
-Version: 1.1.0
+Name: Shark-sac-Korean-editor
+Version: 1.1.1
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/PKG-INFO` & `Shark sac Korean editor-1.1.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: Shark-sac-Korean-editor
-Version: 1.1.0
+Name: Shark sac Korean editor
+Version: 1.1.1
 Summary: 냥코에디터 한글화
 Home-page: https://github.com/sharkwodm/koreditor
 Author: 익명
 Author-email: 
 License: MIT
 Keywords: python,template
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Shark sac Korean editor-1.1.0/Shark_sac_Korean_editor.egg-info/SOURCES.txt` & `Shark sac Korean editor-1.1.1/Shark_sac_Korean_editor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/__main__.py` & `Shark sac Korean editor-1.1.1/modkr/__main__.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/adb_handler.py` & `Shark sac Korean editor-1.1.1/modkr/adb_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/config_manager.py` & `Shark sac Korean editor-1.1.1/modkr/config_manager.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/csv_handler.py` & `Shark sac Korean editor-1.1.1/modkr/csv_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/basic/basic_items.py` & `Shark sac Korean editor-1.1.1/modkr/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/basic/catfruit.py` & `Shark sac Korean editor-1.1.1/modkr/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/basic/catseyes.py` & `Shark sac Korean editor-1.1.1/modkr/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/basic/ototo_base_mats.py` & `Shark sac Korean editor-1.1.1/modkr/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/basic/talent_orbs.py` & `Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/basic/talent_orbs_new.py` & `Shark sac Korean editor-1.1.1/modkr/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/cat_helper.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/cat_id_selector.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/chara_drop.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/clear_cat_guide.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/evolve_cats.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/get_remove_cats.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/talents.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/upgrade_blue.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/cats/upgrade_cats.py` & `Shark sac Korean editor-1.1.1/modkr/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/gamototo/gamatoto_xp.py` & `Shark sac Korean editor-1.1.1/modkr/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/gamototo/helpers.py` & `Shark sac Korean editor-1.1.1/modkr/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/gamototo/ototo_cat_cannon.py` & `Shark sac Korean editor-1.1.1/modkr/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/aku.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/allow_filibuster_clearing.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/allow_filibuster_clearing.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/behemoth_culling.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/clear_tutorial.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/enigma_stages.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/event_stages.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/gauntlet.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/itf_timed_scores.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/legend_quest.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/main_story.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/outbreaks.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/story_level_id_selector.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/towers.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/treasures.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/uncanny.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/levels/unlock_aku_realm.py` & `Shark sac Korean editor-1.1.1/modkr/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/cat_shrine.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/claim_user_rank_rewards.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/create_new_account.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/fix_elsewhere.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/fix_time_issues.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/get_gold_pass.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/meow_medals.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/meow_medals.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 def get_medal_names(is_jp: bool) -> Optional[list[str]]:
     """Get all medal names"""
 
     file_data = game_data_getter.get_file_latest("resLocal", "medalname.tsv", is_jp)
     if file_data is None:
-        helper.error_text("메달 이름을 가져오지 못했습니다.")
+        helper.error_text("Failed to get medal names")
         return None
     medal_names = file_data.decode("utf-8").splitlines()
     names: list[str] = []
     for line in medal_names:
         line_split = line.split("\t")
         name = (
             line_split[0]
@@ -165,15 +165,15 @@
         self.actions = actions
         self.stages = stages
 
 
 def get_medal_data(is_jp: bool) -> Optional[Medals]:
     """Get the medal data"""
 
-    file_data = game_data_getter.get_file_latest("DataLocal", "medallist.json", is_jp)
+    file_data = game_data_getter.get_file_latest_fix("DataLocal", "medallist.json", is_jp)
     if file_data is None:
         helper.error_text("Failed to get medal data")
         return None
     medal_data = json.loads(file_data.decode("utf-8"))["iconID"]
 
     treasures: list[TreasureMedal] = []
     characters: list[CharacterMedal] = []
@@ -213,14 +213,16 @@
                     medal["line"],
                     ActionTypes(medal["action"]),
                 )
             )
         else:
             if "star" not in medal:
                 medal["star"] = None
+            if "map" not in medal:
+                medal["map"] = None
             stages.append(
                 StageMedal(
                     i,
                     medal["grade"],
                     medal["line"],
                     medal["map"],
                     medal["condition"],
@@ -233,30 +235,30 @@
 
 def medals(save_stats: dict[str, Any]) -> dict[str, Any]:
     """Handler for editting meow medals"""
 
     medal_stats = save_stats["medals"]
     remove = (
         user_input_handler.colored_input(
-            "메달을 추가하거나 제거하시겠습니까? (&a&/&r&):"
+            "Do you want to add or remove medals? (&a&/&r&):"
         )
         == "r"
     )
 
     names = get_medal_names(helper.check_data_is_jp(save_stats))
     if names is None:
         return save_stats
     helper.colored_list(names)
 
     ids = user_input_handler.get_range(
         user_input_handler.colored_input(
-            "메달 ID 입력(&all&, 예: &1&-&50& 또는 공백으로 구분된 ID(예: &5 4 7&)을 얻으려면 모두 입력할 수 있습니다.):"
+            "Enter medal ids (You can enter all to get &all&, a range e.g &1&-&50&, or ids separate by spaces e.g &5 4 7&):"
         ),
         len(names) + 1,
     )
     if remove:
         medal_stats = remove_medals(medal_stats, ids)
     else:
         medal_stats = set_medals(medal_stats, ids)
     save_stats["medals"] = medal_stats
-    print(f"성공적으로 {'얻어짐' if not remove else '제거됨'} medals")
+    print(f"Successfully {'gave' if not remove else 'removed'} medals")
     return save_stats
```

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/missions.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/play_time.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/scheme_item.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/trade_progress.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/other/unlock_enemy_guide.py` & `Shark sac Korean editor-1.1.1/modkr/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/save_management/convert.py` & `Shark sac Korean editor-1.1.1/modkr/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/save_management/load.py` & `Shark sac Korean editor-1.1.1/modkr/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/save_management/other.py` & `Shark sac Korean editor-1.1.1/modkr/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/save_management/save.py` & `Shark sac Korean editor-1.1.1/modkr/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/edits/save_management/server_upload.py` & `Shark sac Korean editor-1.1.1/modkr/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/feature_handler.py` & `Shark sac Korean editor-1.1.1/modkr/feature_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/game_data_getter.py` & `Shark sac Korean editor-1.1.1/modkr/game_data_getter.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,55 @@
 from typing import Optional
 import requests
 
 from . import helper
 
 URL = "https://raw.githubusercontent.com/fieryhenry/BCData/master/"
 
+def download_file_en_fix(
+    game_version: str,
+    pack_name: str,
+    file_name: str,
+    get_data: bool = True,
+    print_progress: bool = True,
+) -> bytes:
+    """
+    Downloads the file.
+
+    Args:
+        game_version (str): The game version to download from.
+        pack_name (str): The pack name to download from.
+        file_name (str): The file name to download.
+        get_data (bool, optional): Whether to return the data. Defaults to True.
+        print_progress (bool, optional): Whether to print the progress. Defaults to True.
+
+    Returns:
+        bytes: The data of the file.
+    """
+
+    path = helper.get_file(os.path.join("game_data", game_version, pack_name))
+    file_path = os.path.join(path, file_name)
+    if os.path.exists(file_path):
+        if get_data:
+            return helper.read_file_bytes(file_path)
+        return b""
+
+    if print_progress:
+        helper.colored_text(
+            f"Downloading game data file &{file_name}& from &{pack_name}& with game version &{game_version}&",
+            helper.GREEN,
+            helper.WHITE,
+        )
+    url = "https://raw.githubusercontent.com/cintagram/BCData_Fix/main/medallist.json"
+    response = requests.get(url)
+
+    helper.create_dirs(path)
+    helper.write_file_bytes(file_path, response.content)
+    return response.content
+
 
 def download_file(
     game_version: str,
     pack_name: str,
     file_name: str,
     get_data: bool = True,
     print_progress: bool = True,
@@ -97,14 +138,31 @@
         Optional[bytes]: The data of the file.
     """
     version = get_latest_version(is_jp)
     if version is None:
         return None
     return download_file(version, pack_name, file_name)
 
+def get_file_latest_fix(pack_name: str, file_name: str, is_jp: bool) -> Optional[bytes]:
+    """
+    Gets the latest version of the file.
+
+    Args:
+        pack_name (str): The pack name to find.
+        file_name (str): The file name to find.
+        is_jp (bool): Whether to get the japanese version.
+
+    Returns:
+        Optional[bytes]: The data of the file.
+    """
+    version = get_latest_version(is_jp)
+    if version is None:
+        return None
+    return download_file_en_fix(version, pack_name, file_name)
+
 
 def get_file_latest_path(path: str, is_jp: bool) -> Optional[bytes]:
     """
     Gets the latest version of the file.
 
     Args:
         path (str): The path to find.
```

### Comparing `Shark sac Korean editor-1.1.0/modkr/helper.py` & `Shark sac Korean editor-1.1.1/modkr/helper.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/item.py` & `Shark sac Korean editor-1.1.1/modkr/item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/locale_handler.py` & `Shark sac Korean editor-1.1.1/modkr/locale_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/managed_item.py` & `Shark sac Korean editor-1.1.1/modkr/managed_item.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/parse_save.py` & `Shark sac Korean editor-1.1.1/modkr/parse_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/patcher.py` & `Shark sac Korean editor-1.1.1/modkr/patcher.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/root_handler.py` & `Shark sac Korean editor-1.1.1/modkr/root_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/serialise_save.py` & `Shark sac Korean editor-1.1.1/modkr/serialise_save.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/server_handler.py` & `Shark sac Korean editor-1.1.1/modkr/server_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/tracker.py` & `Shark sac Korean editor-1.1.1/modkr/tracker.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/updater.py` & `Shark sac Korean editor-1.1.1/modkr/updater.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/modkr/user_input_handler.py` & `Shark sac Korean editor-1.1.1/modkr/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `Shark sac Korean editor-1.1.0/setup.py` & `Shark sac Korean editor-1.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 basedir = path.abspath(path.dirname(__file__))
 with open(path.join(basedir, 'README.md'), encoding='utf-8') as file:
     long_description = file.read().replace('\r\n', '\n')
 
 setup(
     name='Shark sac Korean editor',
-    version='1.1.0',
+    version='1.1.1',
     description='냥코에디터 한글화',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='익명',
     author_email='',
     url='https://github.com/sharkwodm/koreditor',
     packages=find_packages(exclude=['contrib', 'docs', 'tests']),
```

