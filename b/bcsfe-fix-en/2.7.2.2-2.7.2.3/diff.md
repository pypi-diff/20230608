# Comparing `tmp/bcsfe-fix-en-2.7.2.2.tar.gz` & `tmp/bcsfe-fix-en-2.7.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bcsfe-fix-en-2.7.2.2.tar", last modified: Thu Jun  8 09:19:24 2023, max compression
+gzip compressed data, was "bcsfe-fix-en-2.7.2.3.tar", last modified: Thu Jun  8 09:22:44 2023, max compression
```

## Comparing `bcsfe-fix-en-2.7.2.2.tar` & `bcsfe-fix-en-2.7.2.3.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.707142 bcsfe-fix-en-2.7.2.2/
--rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/LICENSE
--rw-rw-r--   0 hayun      (502) staff       (20)       95 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/MANIFEST.in
--rw-r--r--   0 hayun      (502) staff       (20)    10972 2023-06-08 09:19:24.706663 bcsfe-fix-en-2.7.2.2/PKG-INFO
--rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/README.md
--rw-rw-r--   0 hayun      (502) staff       (20)      206 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/pyproject.toml
--rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-08 09:19:24.707320 bcsfe-fix-en-2.7.2.2/setup.cfg
--rw-rw-r--   0 hayun      (502) staff       (20)     1070 2023-06-08 09:18:42.000000 bcsfe-fix-en-2.7.2.2/setup.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.652227 bcsfe-fix-en-2.7.2.2/src/
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.663802 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/
--rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8417 2023-06-08 09:18:34.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/__main__.py
--rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/adb_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    13745 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/config_manager.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/csv_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.664402 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/
--rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/__init__.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.669010 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/
--rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/basic_items.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/catfruit.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/catseyes.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/ototo_base_mats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/talent_orbs.py
--rw-rw-r--   0 hayun      (502) staff       (20)    16533 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/talent_orbs_new.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.675265 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/
--rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/cat_helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/cat_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/chara_drop.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/clear_cat_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/evolve_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/get_remove_cats.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/talents.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/upgrade_blue.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/upgrade_cats.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.678202 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/
--rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/fix_gamatoto.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/gamatoto_xp.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/helpers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/ototo_cat_cannon.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.689308 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/
--rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/aku.py
--rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/allow_filibuster_clearing.py
--rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/behemoth_culling.py
--rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/clear_tutorial.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/enigma_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/event_stages.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/gauntlet.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/itf_timed_scores.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/legend_quest.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/main_story.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/outbreaks.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/story_level_id_selector.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/towers.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/treasures.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/uncanny.py
--rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/unlock_aku_realm.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.698799 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/
--rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/cat_shrine.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/claim_user_rank_rewards.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/create_new_account.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/fix_elsewhere.py
--rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/fix_time_issues.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/get_gold_pass.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7142 2023-06-08 09:12:41.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/meow_medals.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/missions.py
--rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/play_time.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/scheme_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/trade_progress.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/unlock_enemy_guide.py
--rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/unlock_equip_menu.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.703159 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/
--rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/__init__.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/convert.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/load.py
--rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/other.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/server_upload.py
--rw-rw-r--   0 hayun      (502) staff       (20)    12640 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/feature_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     6664 2023-06-08 09:12:37.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/game_data_getter.py
--rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/helper.py
--rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/item.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/locale_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/managed_item.py
--rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/parse_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/patcher.py
--rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/root_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/serialise_save.py
--rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/server_handler.py
--rw-rw-r--   0 hayun      (502) staff       (20)     3544 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/updater.py
--rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/user_info.py
--rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/user_input_handler.py
-drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:19:24.705954 bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/
--rw-r--r--   0 hayun      (502) staff       (20)    10972 2023-06-08 09:19:24.000000 bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/PKG-INFO
--rw-r--r--   0 hayun      (502) staff       (20)     3369 2023-06-08 09:19:24.000000 bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/SOURCES.txt
--rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-08 09:19:24.000000 bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/dependency_links.txt
--rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-08 09:19:24.000000 bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/requires.txt
--rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-08 09:19:24.000000 bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/top_level.txt
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.571862 bcsfe-fix-en-2.7.2.3/
+-rw-rw-r--   0 hayun      (502) staff       (20)     1071 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/LICENSE
+-rw-rw-r--   0 hayun      (502) staff       (20)       95 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/MANIFEST.in
+-rw-r--r--   0 hayun      (502) staff       (20)    10972 2023-06-08 09:22:44.571327 bcsfe-fix-en-2.7.2.3/PKG-INFO
+-rw-rw-r--   0 hayun      (502) staff       (20)    10502 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/README.md
+-rw-rw-r--   0 hayun      (502) staff       (20)      206 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/pyproject.toml
+-rw-r--r--   0 hayun      (502) staff       (20)       38 2023-06-08 09:22:44.572005 bcsfe-fix-en-2.7.2.3/setup.cfg
+-rw-rw-r--   0 hayun      (502) staff       (20)     1070 2023-06-08 09:22:38.000000 bcsfe-fix-en-2.7.2.3/setup.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.477270 bcsfe-fix-en-2.7.2.3/src/
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.496805 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/
+-rw-rw-r--   0 hayun      (502) staff       (20)      283 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7947 2023-06-08 09:21:30.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/__main__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    10151 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/adb_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    13745 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/config_manager.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1501 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/csv_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.497229 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/
+-rw-rw-r--   0 hayun      (502) staff       (20)       67 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/__init__.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.502146 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/
+-rw-rw-r--   0 hayun      (502) staff       (20)      122 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8876 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/basic_items.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1490 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/catfruit.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1931 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/catseyes.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1647 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/ototo_base_mats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3984 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/talent_orbs.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    16533 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/talent_orbs_new.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.518773 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/
+-rw-rw-r--   0 hayun      (502) staff       (20)      179 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8978 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/cat_helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    11121 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/cat_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3249 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/chara_drop.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1068 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/clear_cat_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2844 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/evolve_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1260 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/get_remove_cats.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7933 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/talents.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1900 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/upgrade_blue.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4428 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/upgrade_cats.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.528733 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/
+-rw-rw-r--   0 hayun      (502) staff       (20)       66 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      309 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/fix_gamatoto.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2794 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/gamatoto_xp.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3393 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/helpers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7377 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/ototo_cat_cannon.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.542487 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/
+-rw-rw-r--   0 hayun      (502) staff       (20)      313 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1035 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/aku.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      491 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/allow_filibuster_clearing.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      790 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/behemoth_culling.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      646 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/clear_tutorial.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1121 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/enigma_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6307 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/event_stages.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1873 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/gauntlet.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1027 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/itf_timed_scores.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1469 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/legend_quest.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4408 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/main_story.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2323 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/outbreaks.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3031 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/story_level_id_selector.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1175 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/towers.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8458 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/treasures.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1043 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/uncanny.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      784 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/unlock_aku_realm.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.551476 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/
+-rw-rw-r--   0 hayun      (502) staff       (20)      276 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3878 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/cat_shrine.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1093 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/claim_user_rank_rewards.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1054 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/create_new_account.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/fix_elsewhere.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      659 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/fix_time_issues.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3498 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/get_gold_pass.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7142 2023-06-08 09:12:41.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/meow_medals.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4354 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/missions.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      975 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/play_time.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4568 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/scheme_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1612 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/trade_progress.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1284 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/unlock_enemy_guide.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      326 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/unlock_equip_menu.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.556876 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/
+-rw-rw-r--   0 hayun      (502) staff       (20)       56 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/__init__.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1273 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/convert.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2578 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/load.py
+-rw-rw-r--   0 hayun      (502) staff       (20)      644 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/other.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2073 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2149 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/server_upload.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    12640 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/feature_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     6664 2023-06-08 09:12:37.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/game_data_getter.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    24176 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/helper.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     7470 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3505 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/locale_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1269 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/managed_item.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    72134 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/parse_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     1301 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/patcher.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     2415 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/root_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    55884 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/serialise_save.py
+-rw-rw-r--   0 hayun      (502) staff       (20)    26433 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/server_handler.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     3544 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/updater.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     4515 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/user_info.py
+-rw-rw-r--   0 hayun      (502) staff       (20)     8297 2023-05-30 14:09:53.000000 bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/user_input_handler.py
+drwxr-xr-x   0 hayun      (502) staff       (20)        0 2023-06-08 09:22:44.570002 bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/
+-rw-r--r--   0 hayun      (502) staff       (20)    10972 2023-06-08 09:22:44.000000 bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/PKG-INFO
+-rw-r--r--   0 hayun      (502) staff       (20)     3369 2023-06-08 09:22:44.000000 bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/SOURCES.txt
+-rw-r--r--   0 hayun      (502) staff       (20)        1 2023-06-08 09:22:44.000000 bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/dependency_links.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       72 2023-06-08 09:22:44.000000 bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/requires.txt
+-rw-r--r--   0 hayun      (502) staff       (20)       10 2023-06-08 09:22:44.000000 bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/top_level.txt
```

### Comparing `bcsfe-fix-en-2.7.2.2/LICENSE` & `bcsfe-fix-en-2.7.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/PKG-INFO` & `bcsfe-fix-en-2.7.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcsfe-fix-en
-Version: 2.7.2.2
+Version: 2.7.2.3
 Summary: A battle cats save file editor FIX
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: CintagramABP
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcsfe-fix-en-2.7.2.2/README.md` & `bcsfe-fix-en-2.7.2.3/README.md`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/setup.py` & `bcsfe-fix-en-2.7.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 
 setuptools.setup(
     name="bcsfe-fix-en",
-    version="2.7.2.2",
+    version="2.7.2.3",
     author="CintagramABP",
     description="A battle cats save file editor FIX",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/fieryhenry/BCSFE-Python",
     classifiers=[
         "Programming Language :: Python :: 3",
```

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/__main__.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,29 +69,15 @@
 
     if config_manager.get_config_value_category(
         "SERVER", "WIPE_TRACKED_ITEMS_ON_START"
     ):
         user_info.UserInfo.clear_all_items()
     game_data_getter.check_remove_handler()
 
-    check_updates = config_manager.get_config_value_category(
-        "START_UP", "CHECK_FOR_UPDATES"
-    )
-    show_start = not config_manager.get_config_value_category(
-        "START_UP", "HIDE_START_TEXT"
-    )
-
-    if show_start or check_updates:
-        print()
-        helper.print_line_seperator(helper.CYAN, length=200)
     
-    if show_start:
-        print_start_up()
-    if show_start or check_updates:
-        helper.print_line_seperator(helper.CYAN, length=200)
     normal_start_up()
 
 
 def normal_start_up(default_op: bool = True) -> None:
     """Display and handle options for downloading save data, pulling save data, selecting save data"""
 
     default_start_option = config_manager.get_config_value_category(
```

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/adb_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/adb_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/config_manager.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/config_manager.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/csv_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/csv_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/basic_items.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/basic_items.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/catfruit.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/catfruit.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/catseyes.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/catseyes.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/ototo_base_mats.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/ototo_base_mats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/talent_orbs.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/talent_orbs.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/basic/talent_orbs_new.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/basic/talent_orbs_new.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/cat_helper.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/cat_helper.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/cat_id_selector.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/cat_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/chara_drop.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/chara_drop.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/clear_cat_guide.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/clear_cat_guide.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/evolve_cats.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/evolve_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/get_remove_cats.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/get_remove_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/talents.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/talents.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/upgrade_blue.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/upgrade_blue.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/cats/upgrade_cats.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/cats/upgrade_cats.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/gamatoto_xp.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/gamatoto_xp.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/helpers.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/helpers.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/gamototo/ototo_cat_cannon.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/gamototo/ototo_cat_cannon.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/aku.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/aku.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/behemoth_culling.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/behemoth_culling.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/clear_tutorial.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/clear_tutorial.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/enigma_stages.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/enigma_stages.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/event_stages.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/event_stages.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/gauntlet.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/gauntlet.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/itf_timed_scores.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/itf_timed_scores.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/legend_quest.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/legend_quest.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/main_story.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/main_story.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/outbreaks.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/outbreaks.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/story_level_id_selector.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/story_level_id_selector.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/towers.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/towers.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/treasures.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/treasures.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/uncanny.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/uncanny.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/levels/unlock_aku_realm.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/levels/unlock_aku_realm.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/cat_shrine.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/cat_shrine.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/claim_user_rank_rewards.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/claim_user_rank_rewards.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/create_new_account.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/create_new_account.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/fix_elsewhere.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/fix_elsewhere.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/fix_time_issues.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/fix_time_issues.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/get_gold_pass.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/get_gold_pass.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/meow_medals.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/meow_medals.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/missions.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/missions.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/play_time.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/play_time.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/scheme_item.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/scheme_item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/trade_progress.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/trade_progress.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/other/unlock_enemy_guide.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/other/unlock_enemy_guide.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/convert.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/convert.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/load.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/load.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/other.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/other.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/save.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/edits/save_management/server_upload.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/edits/save_management/server_upload.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/feature_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/feature_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/game_data_getter.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/game_data_getter.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/helper.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/helper.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/item.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/locale_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/locale_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/managed_item.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/managed_item.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/parse_save.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/parse_save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/patcher.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/patcher.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/root_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/root_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/serialise_save.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/serialise_save.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/server_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/server_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/updater.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/updater.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/user_info.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/user_info.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/BCSFE_FIX/user_input_handler.py` & `bcsfe-fix-en-2.7.2.3/src/BCSFE_FIX/user_input_handler.py`

 * *Files identical despite different names*

### Comparing `bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/PKG-INFO` & `bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bcsfe-fix-en
-Version: 2.7.2.2
+Version: 2.7.2.3
 Summary: A battle cats save file editor FIX
 Home-page: https://github.com/fieryhenry/BCSFE-Python
 Author: CintagramABP
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `bcsfe-fix-en-2.7.2.2/src/bcsfe_fix_en.egg-info/SOURCES.txt` & `bcsfe-fix-en-2.7.2.3/src/bcsfe_fix_en.egg-info/SOURCES.txt`

 * *Files identical despite different names*

