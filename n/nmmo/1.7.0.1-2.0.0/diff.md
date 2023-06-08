# Comparing `tmp/nmmo-1.7.0.1.tar.gz` & `tmp/nmmo-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nmmo-1.7.0.1.tar", last modified: Mon Mar 20 03:15:07 2023, max compression
+gzip compressed data, was "nmmo-2.0.0.tar", last modified: Thu Jun  8 02:48:16 2023, max compression
```

## Comparing `nmmo-1.7.0.1.tar` & `nmmo-2.0.0.tar`

### file list

```diff
@@ -1,121 +1,127 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/
--rw-r--r--   0 root         (0) root         (0)     1083 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      839 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1105 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.721782 nmmo-1.7.0.1/nmmo/
--rw-r--r--   0 root         (0) root         (0)     1491 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/core/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)      512 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/agent.py
--rw-r--r--   0 root         (0) root         (0)    20161 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/config.py
--rw-r--r--   0 root         (0) root         (0)    13399 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/env.py
--rw-r--r--   0 root         (0) root         (0)     5550 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/log_helper.py
--rw-r--r--   0 root         (0) root         (0)     2125 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/map.py
--rw-r--r--   0 root         (0) root         (0)    14126 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/observation.py
--rw-r--r--   0 root         (0) root         (0)     5776 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/realm.py
--rw-r--r--   0 root         (0) root         (0)     1763 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/render_helper.py
--rw-r--r--   0 root         (0) root         (0)     1488 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/replay.py
--rw-r--r--   0 root         (0) root         (0)      928 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/replay_helper.py
--rw-r--r--   0 root         (0) root         (0)     9022 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/terrain.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/core/tile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/datastore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/datastore/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2736 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/datastore/datastore.py
--rw-r--r--   0 root         (0) root         (0)      465 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/datastore/id_allocator.py
--rw-r--r--   0 root         (0) root         (0)     2228 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/datastore/numpy_datastore.py
--rw-r--r--   0 root         (0) root         (0)     3468 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/datastore/serialized.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/entity/
--rw-r--r--   0 root         (0) root         (0)       76 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/entity/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8782 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/entity/entity.py
--rw-r--r--   0 root         (0) root         (0)     3848 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/entity/entity_manager.py
--rw-r--r--   0 root         (0) root         (0)     5223 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/entity/npc.py
--rw-r--r--   0 root         (0) root         (0)     4162 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/entity/player.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/io/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16542 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/io/action.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/lib/
--rw-r--r--   0 root         (0) root         (0)       49 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4180 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/colors.py
--rw-r--r--   0 root         (0) root         (0)      802 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/log.py
--rw-r--r--   0 root         (0) root         (0)     4538 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/material.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/overlay.py
--rw-r--r--   0 root         (0) root         (0)     1545 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/priorityqueue.py
--rw-r--r--   0 root         (0) root         (0)     3134 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/rating.py
--rw-r--r--   0 root         (0) root         (0)     3031 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/spawn.py
--rw-r--r--   0 root         (0) root         (0)     8303 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/task.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/lib/utils.py
--rw-r--r--   0 root         (0) root         (0)     5071 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/overlay.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/resource/
--rw-r--r--   0 root         (0) root         (0)    37256 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/crystal.png
--rw-r--r--   0 root         (0) root         (0)    28697 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/fish.png
--rwxr-xr-x   0 root         (0) root         (0)    28492 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/forest.png
--rw-r--r--   0 root         (0) root         (0)    36844 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/fragment.png
--rw-r--r--   0 root         (0) root         (0)    37053 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/grass.png
--rwxr-xr-x   0 root         (0) root         (0)    37775 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/herb.png
--rw-r--r--   0 root         (0) root         (0)    30438 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/lava.png
--rw-r--r--   0 root         (0) root         (0)    27391 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/ocean.png
--rw-r--r--   0 root         (0) root         (0)    41374 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/ore.png
--rwxr-xr-x   0 root         (0) root         (0)    21812 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/scrub.png
--rw-r--r--   0 root         (0) root         (0)    31640 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/slag.png
--rw-r--r--   0 root         (0) root         (0)    29419 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/spawn.png
--rw-r--r--   0 root         (0) root         (0)    45012 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/stone.png
--rw-r--r--   0 root         (0) root         (0)    34925 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/stump.png
--rw-r--r--   0 root         (0) root         (0)    36481 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/tree.png
--rw-r--r--   0 root         (0) root         (0)    25708 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/water.png
--rwxr-xr-x   0 root         (0) root         (0)    36222 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/resource/weeds.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.731782 nmmo-1.7.0.1/nmmo/systems/
--rw-r--r--   0 root         (0) root         (0)       25 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/__init__.py
--rw-r--r--   0 root         (0) root         (0)      921 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/achievement.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/nmmo/systems/ai/
--rw-r--r--   0 root         (0) root         (0)       74 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/ai/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2266 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/ai/behavior.py
--rw-r--r--   0 root         (0) root         (0)     1556 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/ai/move.py
--rw-r--r--   0 root         (0) root         (0)      806 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/ai/policy.py
--rw-r--r--   0 root         (0) root         (0)     4371 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/ai/utils.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/combat.py
--rw-r--r--   0 root         (0) root         (0)     1204 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/droptable.py
--rw-r--r--   0 root         (0) root         (0)     5991 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/exchange.py
--rw-r--r--   0 root         (0) root         (0)      348 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/experience.py
--rw-r--r--   0 root         (0) root         (0)     5663 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/inventory.py
--rw-r--r--   0 root         (0) root         (0)    12223 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/item.py
--rw-r--r--   0 root         (0) root         (0)     8039 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/systems/skill.py
--rw-r--r--   0 root         (0) root         (0)       24 2023-03-20 03:14:58.000000 nmmo-1.7.0.1/nmmo/version.py
--rw-r--r--   0 root         (0) root         (0)     4564 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/nmmo/websocket.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.721782 nmmo-1.7.0.1/nmmo.egg-info/
--rw-r--r--   0 root         (0) root         (0)      839 2023-03-20 03:15:07.000000 nmmo-1.7.0.1/nmmo.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2372 2023-03-20 03:15:07.000000 nmmo-1.7.0.1/nmmo.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-20 03:15:07.000000 nmmo-1.7.0.1/nmmo.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      593 2023-03-20 03:15:07.000000 nmmo-1.7.0.1/nmmo.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-03-20 03:15:07.000000 nmmo-1.7.0.1/nmmo.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/scripted/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/scripted/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1142 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/scripted/attack.py
--rw-r--r--   0 root         (0) root         (0)    15180 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/scripted/baselines.py
--rw-r--r--   0 root         (0) root         (0)     2276 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/scripted/behavior.py
--rw-r--r--   0 root         (0) root         (0)     8077 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/scripted/move.py
--rw-r--r--   0 root         (0) root         (0)      618 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/scripted/utils.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1987 2023-03-20 03:14:46.000000 nmmo-1.7.0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      399 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/tests/datastore/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/datastore/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1077 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/datastore/test_datastore.py
--rw-r--r--   0 root         (0) root         (0)     1576 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/datastore/test_id_allocator.py
--rw-r--r--   0 root         (0) root         (0)     1216 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/datastore/test_numpy_datastore.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/tests/entity/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/entity/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2455 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/entity/test_entity.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-20 03:15:07.741782 nmmo-1.7.0.1/tests/lib/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/lib/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1362 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/lib/test_serialized.py
--rw-r--r--   0 root         (0) root         (0)      192 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_client.py
--rw-r--r--   0 root         (0) root         (0)     2969 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_determinism.py
--rw-r--r--   0 root         (0) root         (0)     6045 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_deterministic_replay.py
--rw-r--r--   0 root         (0) root         (0)     4508 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_performance.py
--rw-r--r--   0 root         (0) root         (0)      349 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_pettingzoo.py
--rw-r--r--   0 root         (0) root         (0)      257 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_rollout.py
--rw-r--r--   0 root         (0) root         (0)     3733 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/test_task.py
--rw-r--r--   0 root         (0) root         (0)    12098 2023-03-19 21:23:47.000000 nmmo-1.7.0.1/tests/testhelpers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-06-08 02:46:50.000000 nmmo-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 02:46:50.000000 nmmo-2.0.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-08 02:48:16.129083 nmmo-2.0.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      853 2023-06-08 02:46:50.000000 nmmo-2.0.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo/
+-rw-r--r--   0 root         (0) root         (0)     1439 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17317 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/action.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/agent.py
+-rw-r--r--   0 root         (0) root         (0)    20097 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/config.py
+-rw-r--r--   0 root         (0) root         (0)    15082 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/env.py
+-rw-r--r--   0 root         (0) root         (0)     4895 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/log_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2397 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/map.py
+-rw-r--r--   0 root         (0) root         (0)    14336 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/observation.py
+-rw-r--r--   0 root         (0) root         (0)     6098 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/realm.py
+-rw-r--r--   0 root         (0) root         (0)     9313 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/terrain.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/core/tile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo/datastore/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/datastore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2736 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/datastore/datastore.py
+-rw-r--r--   0 root         (0) root         (0)      465 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/datastore/id_allocator.py
+-rw-r--r--   0 root         (0) root         (0)     2228 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/datastore/numpy_datastore.py
+-rw-r--r--   0 root         (0) root         (0)     3468 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/datastore/serialized.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo/entity/
+-rw-r--r--   0 root         (0) root         (0)       76 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/entity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9204 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/entity/entity.py
+-rw-r--r--   0 root         (0) root         (0)     4415 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/entity/entity_manager.py
+-rw-r--r--   0 root         (0) root         (0)     5192 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/entity/npc.py
+-rw-r--r--   0 root         (0) root         (0)     4275 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/entity/player.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo/lib/
+-rw-r--r--   0 root         (0) root         (0)       49 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4180 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/colors.py
+-rw-r--r--   0 root         (0) root         (0)     5732 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/event_log.py
+-rw-r--r--   0 root         (0) root         (0)     1435 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/log.py
+-rw-r--r--   0 root         (0) root         (0)     4555 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/material.py
+-rw-r--r--   0 root         (0) root         (0)     1545 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/priorityqueue.py
+-rw-r--r--   0 root         (0) root         (0)     3878 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/spawn.py
+-rw-r--r--   0 root         (0) root         (0)     1385 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/team_helper.py
+-rw-r--r--   0 root         (0) root         (0)     1876 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/lib/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo/render/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/render/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4385 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/render/overlay.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/render/render_client.py
+-rw-r--r--   0 root         (0) root         (0)     2634 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/render/render_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2605 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/render/replay_helper.py
+-rw-r--r--   0 root         (0) root         (0)     4623 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/render/websocket.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/nmmo/resource/
+-rw-r--r--   0 root         (0) root         (0)    37256 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/crystal.png
+-rw-r--r--   0 root         (0) root         (0)    28697 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/fish.png
+-rwxr-xr-x   0 root         (0) root         (0)    28492 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/foilage.png
+-rw-r--r--   0 root         (0) root         (0)    36844 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/fragment.png
+-rw-r--r--   0 root         (0) root         (0)    37053 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/grass.png
+-rwxr-xr-x   0 root         (0) root         (0)    37775 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/herb.png
+-rw-r--r--   0 root         (0) root         (0)    27391 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/ocean.png
+-rw-r--r--   0 root         (0) root         (0)    41374 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/ore.png
+-rwxr-xr-x   0 root         (0) root         (0)    21812 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/scrub.png
+-rw-r--r--   0 root         (0) root         (0)    31640 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/slag.png
+-rw-r--r--   0 root         (0) root         (0)    29419 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/spawn.png
+-rw-r--r--   0 root         (0) root         (0)    45012 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/stone.png
+-rw-r--r--   0 root         (0) root         (0)    34925 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/stump.png
+-rw-r--r--   0 root         (0) root         (0)    36481 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/tree.png
+-rw-r--r--   0 root         (0) root         (0)    30438 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/void.png
+-rw-r--r--   0 root         (0) root         (0)    25708 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/water.png
+-rwxr-xr-x   0 root         (0) root         (0)    36222 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/resource/weeds.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/nmmo/systems/
+-rw-r--r--   0 root         (0) root         (0)       25 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/nmmo/systems/ai/
+-rw-r--r--   0 root         (0) root         (0)       74 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/ai/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2266 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/ai/behavior.py
+-rw-r--r--   0 root         (0) root         (0)     1558 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/ai/move.py
+-rw-r--r--   0 root         (0) root         (0)      806 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/ai/policy.py
+-rw-r--r--   0 root         (0) root         (0)     4372 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/ai/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4732 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/combat.py
+-rw-r--r--   0 root         (0) root         (0)     1078 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/droptable.py
+-rw-r--r--   0 root         (0) root         (0)     6317 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/exchange.py
+-rw-r--r--   0 root         (0) root         (0)      348 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/experience.py
+-rw-r--r--   0 root         (0) root         (0)     5690 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/inventory.py
+-rw-r--r--   0 root         (0) root         (0)    12849 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/item.py
+-rw-r--r--   0 root         (0) root         (0)     8791 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/systems/skill.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/nmmo/task/
+-rw-r--r--   0 root         (0) root         (0)       79 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12896 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/base_predicates.py
+-rw-r--r--   0 root         (0) root         (0)     6226 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/constraint.py
+-rw-r--r--   0 root         (0) root         (0)     7083 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/game_state.py
+-rw-r--r--   0 root         (0) root         (0)     2600 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/group.py
+-rw-r--r--   0 root         (0) root         (0)    10583 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/predicate_api.py
+-rw-r--r--   0 root         (0) root         (0)     6843 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/task/task_api.py
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-08 02:46:50.000000 nmmo-2.0.0/nmmo/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.119083 nmmo-2.0.0/nmmo.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      964 2023-06-08 02:48:16.000000 nmmo-2.0.0/nmmo.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2542 2023-06-08 02:48:16.000000 nmmo-2.0.0/nmmo.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 02:48:16.000000 nmmo-2.0.0/nmmo.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      512 2023-06-08 02:48:16.000000 nmmo-2.0.0/nmmo.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 02:48:16.000000 nmmo-2.0.0/nmmo.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/scripted/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/scripted/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1142 2023-06-08 02:46:50.000000 nmmo-2.0.0/scripted/attack.py
+-rw-r--r--   0 root         (0) root         (0)    15180 2023-06-08 02:46:50.000000 nmmo-2.0.0/scripted/baselines.py
+-rw-r--r--   0 root         (0) root         (0)     2276 2023-06-08 02:46:50.000000 nmmo-2.0.0/scripted/behavior.py
+-rw-r--r--   0 root         (0) root         (0)     8144 2023-06-08 02:46:50.000000 nmmo-2.0.0/scripted/move.py
+-rw-r--r--   0 root         (0) root         (0)      618 2023-06-08 02:46:50.000000 nmmo-2.0.0/scripted/utils.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 02:48:16.129083 nmmo-2.0.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1873 2023-06-08 02:46:50.000000 nmmo-2.0.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      399 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/tests/datastore/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/datastore/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/datastore/test_datastore.py
+-rw-r--r--   0 root         (0) root         (0)     1576 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/datastore/test_id_allocator.py
+-rw-r--r--   0 root         (0) root         (0)     1216 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/datastore/test_numpy_datastore.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/tests/entity/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/entity/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2299 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/entity/test_entity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 02:48:16.129083 nmmo-2.0.0/tests/lib/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/lib/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1362 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/lib/test_serialized.py
+-rw-r--r--   0 root         (0) root         (0)     2950 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_determinism.py
+-rw-r--r--   0 root         (0) root         (0)     6040 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_deterministic_replay.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_eventlog.py
+-rw-r--r--   0 root         (0) root         (0)     4508 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_performance.py
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_pettingzoo.py
+-rw-r--r--   0 root         (0) root         (0)      257 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_rollout.py
+-rw-r--r--   0 root         (0) root         (0)     1722 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/test_team_spawn.py
+-rw-r--r--   0 root         (0) root         (0)    13512 2023-06-08 02:46:50.000000 nmmo-2.0.0/tests/testhelpers.py
```

### Comparing `nmmo-1.7.0.1/LICENSE` & `nmmo-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/PKG-INFO` & `nmmo-2.0.0/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: nmmo
-Version: 1.7.0.1
+Version: 2.0.0
 Summary: Neural MMO is a platform for multiagent intelligence research inspired by Massively Multiplayer Online (MMO) role-playing games. Documentation hosted at neuralmmo.github.io.
 Home-page: https://github.com/neuralmmo/environment
 Author: Joseph Suarez
 Author-email: jsuarez@mit.edu
 License: MIT
 Keywords: Neural MMO,MMO
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: cleanrl
 Provides-Extra: all
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `nmmo-1.7.0.1/nmmo/__init__.py` & `nmmo-2.0.0/nmmo/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 import logging
 
 from .version import __version__
 
 from .lib import material, spawn
-from .overlay import Overlay, OverlayRegistry
-from .io import action
-from .io.action import Action
-from .core import config, agent
+from .render.overlay import Overlay, OverlayRegistry
+from .core import config, agent, action
+from .core.action import Action
 from .core.agent import Agent
 from .core.env import Env
-from .systems.achievement import Task
 from .core.terrain import MapGenerator, Terrain
 
 MOTD = rf'''      ___           ___           ___           ___
      /__/\         /__/\         /__/\         /  /\      Version {__version__:<8}
      \  \:\       |  |::\       |  |::\       /  /::\
       \  \:\      |  |:|:\      |  |:|:\     /  /:/\:\    An open source
   _____\__\:\   __|__|:|\:\   __|__|:|\:\   /  /:/  \:\   project originally
@@ -22,13 +20,13 @@
   \  \:\  ~~~   \  \:\        \  \:\        \  \:\  /:/
    \  \:\        \  \:\        \  \:\        \  \:\/:/    Now developed and
     \  \:\        \  \:\        \  \:\        \  \::/     maintained at MIT in
      \__\/         \__\/         \__\/         \__\/      Phillip Isola's lab '''
 
 __all__ = ['Env', 'config', 'agent', 'Agent', 'MapGenerator', 'Terrain',
         'action', 'Action', 'material', 'spawn',
-        'Task', 'Overlay', 'OverlayRegistry']
+        'Overlay', 'OverlayRegistry']
 
 try:
   __all__.append('OpenSkillRating')
 except RuntimeError:
   logging.error('Warning: OpenSkill not installed. Ignore if you do not need this feature')
```

### Comparing `nmmo-1.7.0.1/nmmo/core/config.py` & `nmmo-2.0.0/nmmo/core/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -141,29 +141,20 @@
 
   ############################################################################
   ### Meta-Parameters
   def game_system_enabled(self, name) -> bool:
     return hasattr(self, name)
 
 
-  RENDER                       = False
-  '''Flag used by render mode'''
-
-  SAVE_REPLAY                  = False
-  '''Flag used to save replays'''
-
-  PROVIDE_ACTION_TARGETS       = False
+  PROVIDE_ACTION_TARGETS       = True
   '''Flag used to provide action targets mask'''
 
   PLAYERS                      = [Agent]
   '''Player classes from which to spawn'''
 
-  TASKS                        = []
-  '''Tasks for which to compute rewards'''
-
   ############################################################################
   ### Emulation Parameters
 
   EMULATE_FLAT_OBS       = False
   '''Emulate a flat observation space'''
 
   EMULATE_FLAT_ATN       = False
@@ -222,15 +213,15 @@
   PLAYER_DEATH_FOG             = None
   '''How long before spawning death fog. None for no death fog'''
 
 
   ############################################################################
   ### Agent Parameters
   IMMORTAL = False
-  '''Debug parameter: prevents agents from dying except by lava'''
+  '''Debug parameter: prevents agents from dying except by void'''
 
   BASE_HEALTH                = 10
   '''Initial Constitution level and agent health'''
 
   PLAYER_DEATH_FOG_SPEED       = 1
   '''Number of tiles per tick that the fog moves in'''
 
@@ -262,15 +253,15 @@
     '''Number of distinct tile observations'''
     return int(self.PLAYER_VISION_DIAMETER ** 2)
 
   MAP_CENTER                   = None
   '''Size of each map (number of tiles along each side)'''
 
   MAP_BORDER                   = 16
-  '''Number of lava border tiles surrounding each side of the map'''
+  '''Number of void border tiles surrounding each side of the map'''
 
   @property
   def MAP_SIZE(self):
     return int(self.MAP_CENTER + 2*self.MAP_BORDER)
 
   MAP_GENERATOR                = MapGenerator
   '''Specifies a user map generator. Uses default generator if unspecified.'''
@@ -331,50 +322,50 @@
 
   TERRAIN_LOG_INTERPOLATE_MAX  = 0
   '''Maximum interpolation log-strength for noise frequencies'''
 
   TERRAIN_TILES_PER_OCTAVE     = 8
   '''Number of octaves sampled from log2 spaced TERRAIN_FREQUENCY range'''
 
-  TERRAIN_LAVA                 = 0.0
-  '''Noise threshold for lava generation'''
+  TERRAIN_VOID                 = 0.0
+  '''Noise threshold for void generation'''
 
   TERRAIN_WATER                = 0.30
   '''Noise threshold for water generation'''
 
   TERRAIN_GRASS                = 0.70
   '''Noise threshold for grass'''
 
-  TERRAIN_FOREST               = 0.85
-  '''Noise threshold for forest'''
+  TERRAIN_FOILAGE              = 0.85
+  '''Noise threshold for foilage (food tile)'''
 
 
 class Resource:
   '''Resource Game System'''
 
   RESOURCE_SYSTEM_ENABLED             = True
   '''Game system flag'''
 
   RESOURCE_BASE                       = 100
-  '''Initial level and capacity for Hunting + Fishing resource skills'''
+  '''Initial level and capacity for food and water'''
 
   RESOURCE_DEPLETION_RATE             = 5
   '''Depletion rate for food and water'''
 
   RESOURCE_STARVATION_RATE            = 10
   '''Damage per tick without food'''
 
   RESOURCE_DEHYDRATION_RATE           = 10
   '''Damage per tick without water'''
 
-  RESOURCE_FOREST_CAPACITY            = 1
-  '''Maximum number of harvests before a forest tile decays'''
+  RESOURCE_FOILAGE_CAPACITY            = 1
+  '''Maximum number of harvests before a foilage tile decays'''
 
-  RESOURCE_FOREST_RESPAWN             = 0.025
-  '''Probability that a harvested forest tile will regenerate each tick'''
+  RESOURCE_FOILAGE_RESPAWN             = 0.025
+  '''Probability that a harvested foilage tile will regenerate each tick'''
 
   RESOURCE_HARVEST_RESTORE_FRACTION   = 1.0
   '''Fraction of maximum capacity restored upon collecting a resource'''
 
   RESOURCE_HEALTH_REGEN_THRESHOLD     = 0.5
   '''Fraction of maximum resource capacity required to regen health'''
 
@@ -384,20 +375,21 @@
 
 class Combat:
   '''Combat Game System'''
 
   COMBAT_SYSTEM_ENABLED              = True
   '''Game system flag'''
 
-  COMBAT_FRIENDLY_FIRE               = True
-  '''Whether agents with the same population index can hit each other'''
-
   COMBAT_SPAWN_IMMUNITY              = 20
   '''Agents older than this many ticks cannot attack agents younger than this many ticks'''
 
+  COMBAT_STATUS_DURATION             = 3
+  '''Combat status lasts for this many ticks after the last combat event.
+     Combat events include both attacking and being attacked.'''
+
   COMBAT_WEAKNESS_MULTIPLIER         = 1.5
   '''Multiplier for super-effective attacks'''
 
   def COMBAT_DAMAGE_FORMULA(self, offense, defense, multiplier):
     '''Damage formula'''
     return int(multiplier * (offense * (15 / (15 + defense))))
 
@@ -434,14 +426,17 @@
 
   PROGRESSION_AMMUNITION_XP_SCALE   = 1
   '''Multiplier on top of XP_SCALE for Prospecting, Carving, and Alchemy'''
 
   PROGRESSION_CONSUMABLE_XP_SCALE   = 5
   '''Multiplier on top of XP_SCALE for Fishing and Herbalism'''
 
+  PROGRESSION_BASE_LEVEL            = 1
+  '''Initial skill level'''
+
   PROGRESSION_LEVEL_MAX             = 10
   '''Max skill level'''
 
   PROGRESSION_MELEE_BASE_DAMAGE     = 0
   '''Base Melee attack damage'''
 
   PROGRESSION_MELEE_LEVEL_DAMAGE    = 5
@@ -514,16 +509,16 @@
 
   ITEM_N                              = 17
   '''Number of unique base item classes'''
 
   ITEM_INVENTORY_CAPACITY             = 12
   '''Number of inventory spaces'''
 
-  ITEM_GIVE_TO_FRIENDLY               = True
-  '''Whether agents with the same population index can give gold/item to each other'''
+  ITEM_ALLOW_GIFT               = True
+  '''Whether agents can give gold/item to each other'''
 
   @property
   def INVENTORY_N_OBS(self):
     '''Number of distinct item observations'''
     return self.ITEM_INVENTORY_CAPACITY
 
 
@@ -605,14 +600,17 @@
 
 class Exchange:
   '''Exchange Game System'''
 
   EXCHANGE_SYSTEM_ENABLED             = True
   '''Game system flag'''
 
+  EXCHANGE_BASE_GOLD                  = 1
+  '''Initial gold amount'''
+
   EXCHANGE_LISTING_DURATION           = 5
   '''The number of ticks, during which the item is listed for sale'''
 
   @property
   def MARKET_N_OBS(self):
     # TODO(kywch): This is a hack. Check if the limit is reached
     # pylint: disable=no-member
```

### Comparing `nmmo-1.7.0.1/nmmo/core/env.py` & `nmmo-2.0.0/nmmo/core/env.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,47 +1,53 @@
 import functools
 import random
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Callable
+from collections import defaultdict
 from ordered_set import OrderedSet
 
 import gym
 import numpy as np
 from pettingzoo.utils.env import AgentID, ParallelEnv
 
 import nmmo
+from nmmo.core import realm
 from nmmo.core.config import Default
 from nmmo.core.observation import Observation
 from nmmo.core.tile import Tile
 from nmmo.entity.entity import Entity
 from nmmo.systems.item import Item
-from nmmo.core import realm
+from nmmo.task import task_api
+from nmmo.task.game_state import GameStateGenerator
 from scripted.baselines import Scripted
 
-
 class Env(ParallelEnv):
-  '''Environment wrapper for Neural MMO using the Parallel PettingZoo API
-
-  Neural MMO provides complex environments featuring structured observations/actions,
-  variably sized agent populations, and long time horizons. Usage in conjunction
-  with RLlib as demonstrated in the /projekt wrapper is highly recommended.'''
+  # Environment wrapper for Neural MMO using the Parallel PettingZoo API
 
+  #pylint: disable=no-value-for-parameter
   def __init__(self,
-    config: Default = nmmo.config.Default(), seed=None):
+               config: Default = nmmo.config.Default(),
+               seed = None):
     self._init_random(seed)
 
     super().__init__()
 
     self.config = config
     self.realm = realm.Realm(config)
     self.obs = None
 
     self.possible_agents = list(range(1, config.PLAYER_N + 1))
-    self._dead_agents = OrderedSet()
+    self._dead_agents = set()
+    self._episode_stats = defaultdict(lambda: defaultdict(float))
     self.scripted_agents = OrderedSet()
 
+    self._gamestate_generator = GameStateGenerator(self.realm, self.config)
+    self.game_state = None
+    # Default task: rewards 1 each turn agent is alive
+    self.tasks = task_api.nmmo_default_task(self.possible_agents)
+
   # pylint: disable=method-cache-max-size-none
   @functools.lru_cache(maxsize=None)
   def observation_space(self, agent: int):
     '''Neural MMO Observation Space
 
     Args:
         agent: Agent ID
@@ -56,16 +62,18 @@
     def box(rows, cols):
       return gym.spaces.Box(
           low=-2**20, high=2**20,
           shape=(rows, cols),
           dtype=np.float32)
 
     obs_space = {
+      "CurrentTick": gym.spaces.Discrete(1),
+      "AgentId": gym.spaces.Discrete(1),
       "Tile": box(self.config.MAP_N_OBS, Tile.State.num_attributes),
-      "Entity": box(self.config.PLAYER_N_OBS, Entity.State.num_attributes)
+      "Entity": box(self.config.PLAYER_N_OBS, Entity.State.num_attributes),
     }
 
     if self.config.ITEM_SYSTEM_ENABLED:
       obs_space["Inventory"] = box(self.config.INVENTORY_N_OBS, Item.State.num_attributes)
 
     if self.config.EXCHANGE_SYSTEM_ENABLED:
       obs_space["Market"] = box(self.config.MARKET_N_OBS, Item.State.num_attributes)
@@ -108,22 +116,24 @@
     return gym.spaces.Dict(actions)
 
   ############################################################################
   # Core API
 
   # TODO: This doesn't conform to the PettingZoo API
   # pylint: disable=arguments-renamed
-  def reset(self, map_id=None, seed=None, options=None):
+  def reset(self, map_id=None, seed=None, options=None,
+            make_task_fn: Callable=None):
     '''OpenAI Gym API reset function
 
     Loads a new game map and returns initial observations
 
     Args:
-        idx: Map index to load. Selects a random map by default
-
+        map_id: Map index to load. Selects a random map by default
+        seed: random seed to use
+        make_task_fn: A function to make tasks
 
     Returns:
         observations, as documented by _compute_observations()
 
     Notes:
         Neural MMO simulates a persistent world. Ideally, you should reset
         the environment only once, upon creation. In practice, this approach
@@ -132,22 +142,30 @@
         therefore recommend the standard approach of resetting after a long
         but finite horizon: ~1000 timesteps for small maps and
         5000+ timesteps for large maps
     '''
 
     self._init_random(seed)
     self.realm.reset(map_id)
-    self._dead_agents = OrderedSet()
+    self._dead_agents = set()
+    self._episode_stats.clear()
 
     # check if there are scripted agents
     for eid, ent in self.realm.players.items():
       if isinstance(ent.agent, Scripted):
         self.scripted_agents.add(eid)
 
     self.obs = self._compute_observations()
+    self._gamestate_generator = GameStateGenerator(self.realm, self.config)
+
+    if make_task_fn is not None:
+      self.tasks = make_task_fn()
+    else:
+      for task in self.tasks:
+        task.reset()
 
     return {a: o.to_gym() for a,o in self.obs.items()}
 
   def step(self, actions: Dict[int, Dict[str, Dict[str, Any]]]):
     '''Simulates one game tick or timestep
 
     Args:
@@ -236,45 +254,52 @@
                 agent_2: None,
                 ...
               }
 
           Provided for conformity with PettingZoo
     '''
     assert self.obs is not None, 'step() called before reset'
-
     # Add in scripted agents' actions, if any
     if self.scripted_agents:
       actions = self._compute_scripted_agent_actions(actions)
 
     # Drop invalid actions of BOTH neural and scripted agents
     #   we don't need _deserialize_scripted_actions() anymore
     actions = self._validate_actions(actions)
-
     # Execute actions
     self.realm.step(actions)
-
     dones = {}
     for eid in self.possible_agents:
-      if eid not in self.realm.players and eid not in self._dead_agents:
-        self._dead_agents.add(eid)
-        dones[eid] = True
+      if eid not in self.realm.players or self.realm.tick >= self.config.HORIZON:
+        if eid not in self._dead_agents:
+          self._dead_agents.add(eid)
+          self._episode_stats[eid]["death_tick"] = self.realm.tick
+          dones[eid] = True
 
     # Store the observations, since actions reference them
     self.obs = self._compute_observations()
     gym_obs = {a: o.to_gym() for a,o in self.obs.items()}
 
     rewards, infos = self._compute_rewards(self.obs.keys(), dones)
+    for k,r in rewards.items():
+      self._episode_stats[k]['reward'] += r
+
+    # When the episode ends, add the episode stats to the info of one of
+    # the last dagents
+    if len(self._dead_agents) == len(self.possible_agents):
+      for agent_id, stats in self._episode_stats.items():
+        if agent_id not in infos:
+          infos[agent_id] = {}
+        infos[agent_id]["episode_stats"] = stats
 
     return gym_obs, rewards, dones, infos
 
   def _validate_actions(self, actions: Dict[int, Dict[str, Dict[str, Any]]]):
     '''Deserialize action arg values and validate actions
        For now, it does a basic validation (e.g., value is not none).
-
-       TODO(kywch): add sophisticated validation like use/sell/give on the same item
     '''
     validated_actions = {}
 
     for ent_id, atns in actions.items():
       if ent_id not in self.realm.players:
         #assert ent_id in self.realm.players, f'Entity {ent_id} not in realm'
         continue # Entity not in the realm -- invalid actions
@@ -306,15 +331,15 @@
 
     return validated_actions
 
   def _compute_scripted_agent_actions(self, actions: Dict[int, Dict[str, Dict[str, Any]]]):
     '''Compute actions for scripted agents and add them into the action dict'''
     for eid in self.scripted_agents:
       # remove the dead scripted agent from the list
-      if eid not in self.realm.players:
+      if eid in self._dead_agents or eid not in self.realm.players:
         self.scripted_agents.discard(eid)
         continue
 
       # override the provided scripted agents' actions
       actions[eid] = self.realm.players[eid].agent(self.obs[eid])
 
     return actions
@@ -326,14 +351,15 @@
         agents: List of agents to return observations for. If None, returns
         observations for all agents
 
     Returns:
         obs: Dictionary of observations for each agent
         obs[agent_id] = {
           "Entity": [e1, e2, ...],
+          "Task": [encoded_task],
           "Tile": [t1, t2, ...],
           "Inventory": [i1, i2, ...],
           "Market": [m1, m2, ...],
           "ActionTargets": {
               "Attack": [a1, a2, ...],
               "Sell": [s1, s2, ...],
               "Buy": [b1, b2, ...],
@@ -341,16 +367,16 @@
           }
         '''
 
     obs = {}
 
     market = Item.Query.for_sale(self.realm.datastore)
 
-    for agent in self.realm.players.values():
-      agent_id = agent.id.val
+    for agent_id in self.agents:
+      agent = self.realm.players.get(agent_id)
       agent_r = agent.row.val
       agent_c = agent.col.val
 
       visible_entities = Entity.Query.window(
           self.realm.datastore,
           agent_r, agent_c,
           self.config.PLAYER_VISION_RADIUS
@@ -358,17 +384,20 @@
       visible_tiles = Tile.Query.window(
           self.realm.datastore,
           agent_r, agent_c,
           self.config.PLAYER_VISION_RADIUS)
 
       inventory = Item.Query.owned_by(self.realm.datastore, agent_id)
 
-      obs[agent_id] = Observation(
-        self.config, agent_id, visible_tiles, visible_entities, inventory, market)
-
+      obs[agent_id] = Observation(self.config,
+                                  self.realm.tick,
+                                  agent_id,
+                                  visible_tiles,
+                                  visible_entities,
+                                  inventory, market)
     return obs
 
   def _compute_rewards(self, agents: List[AgentID], dones: Dict[AgentID, bool]):
     '''Computes the reward for the specified agent
 
     Override this method to create custom reward functions. You have full
     access to the environment state via self.realm. Our baselines do not
@@ -378,45 +407,46 @@
         player: player object
 
     Returns:
         reward:
           The reward for the actions on the previous timestep of the
           entity identified by ent_id.
     '''
-    infos = {}
-    rewards = { eid: -1 for eid in dones }
-
-    for agent_id in agents:
-      infos[agent_id] = {}
-      agent = self.realm.players.get(agent_id)
-      assert agent is not None, f'Agent {agent_id} not found'
-
-      infos[agent_id] =  {'population': agent.population}
-
-      if agent.diary is None:
-        rewards[agent_id] = 0
-        continue
-
-      rewards[agent_id] = sum(agent.diary.rewards.values())
-      infos[agent_id].update(agent.diary.rewards)
+    # Initialization
+    infos = {agent_id: {'task': {}} for agent_id in agents}
+    rewards = defaultdict(int)
+    agents = set(agents)
+    reward_cache = {}
+
+    # Compute Rewards and infos
+    self.game_state = self._gamestate_generator.generate(self.realm, self.obs)
+    for task in self.tasks:
+      if task in reward_cache:
+        task_rewards, task_infos = reward_cache[task]
+      else:
+        task_rewards, task_infos = task.compute_rewards(self.game_state)
+        reward_cache[task] = (task_rewards, task_infos)
+      for agent_id, reward in task_rewards.items():
+        if agent_id in agents and agent_id not in dones:
+          rewards[agent_id] = rewards.get(agent_id,0) + reward
+          infos[agent_id]['task'][task.name] = task_infos[agent_id] # progress
 
     return rewards, infos
 
-
   ############################################################################
   # PettingZoo API
   ############################################################################
 
   def render(self, mode='human'):
     '''For conformity with the PettingZoo API only; rendering is external'''
 
   @property
   def agents(self) -> List[AgentID]:
     '''For conformity with the PettingZoo API only; rendering is external'''
-    return list(self.realm.players.keys())
+    return list(set(self.realm.players.keys()) - self._dead_agents)
 
   def close(self):
     '''For conformity with the PettingZoo API only; rendering is external'''
 
   def seed(self, seed=None):
     return self._init_random(seed)
```

### Comparing `nmmo-1.7.0.1/nmmo/core/log_helper.py` & `nmmo-2.0.0/nmmo/core/log_helper.py`

 * *Files 8% similar despite different names*

```diff
@@ -76,21 +76,14 @@
 
   def _register_player_stat(self, name: str, func: callable):
     assert name not in self._player_stats_funcs
     self._player_stats_funcs[name] = func
 
   def _register_player_stats(self):
     self._register_player_stat('Basic/TimeAlive', lambda player: player.history.time_alive.val)
-
-    if self.config.TASKS:
-      self._register_player_stat('Task/Completed', lambda player: player.diary.completed)
-      self._register_player_stat('Task/Reward' , lambda player: player.diary.cumulative_reward)
-    else:
-      self._register_player_stat('Task/Completed', lambda player: player.history.time_alive.val)
-
     # Skills
     if self.config.PROGRESSION_SYSTEM_ENABLED:
       if self.config.COMBAT_SYSTEM_ENABLED:
         self._register_player_stat('Skill/Mage', lambda player: player.skills.mage.level.val)
         self._register_player_stat('Skill/Range', lambda player: player.skills.range.level.val)
         self._register_player_stat('Skill/Melee', lambda player: player.skills.melee.level.val)
       if self.config.PROFESSION_SYSTEM_ENABLED:
@@ -133,20 +126,10 @@
   def _player_stats(self, player: Agent) -> Dict[str, float]:
     stats = {}
     policy = player.policy
 
     for key, stat_func in self._player_stats_funcs.items():
       stats[f'{key}_{policy}'] = stat_func(player)
 
-    stats['Task_Reward'] = player.history.time_alive.val
-
-    # If diary is enabled, log task and achievement stats
-    if player.diary:
-      stats['Task_Reward'] = player.diary.cumulative_reward
-
-      for achievement in player.diary.achievements:
-        stats["Achievement_{achievement.name}"] = float(achievement.completed)
-
-    # Used for SR
-    stats['PolicyID'] = player.population
+    stats['Time_Alive'] = player.history.time_alive.val
 
     return stats
```

### Comparing `nmmo-1.7.0.1/nmmo/core/map.py` & `nmmo-2.0.0/nmmo/core/map.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,15 +34,15 @@
       missing_resources.append(e.pos)
     return missing_resources
 
   @property
   def repr(self):
     '''Flat matrix of tile material indices'''
     if not self._repr:
-      self._repr = [[t.mat.index for t in row] for row in self.tiles]
+      self._repr = [[t.material.index for t in row] for row in self.tiles]
 
     return self._repr
 
   def reset(self, map_id):
     '''Reuse the current tile objects to load a new map'''
     config = self.config
     self.update_list = OrderedSet()
@@ -53,20 +53,26 @@
     try:
       map_file = np.load(f_path)
     except FileNotFoundError:
       logging.error('Maps not found')
       raise
 
     materials = {mat.index: mat for mat in material.All}
+    r, c = 0, 0
     for r, row in enumerate(map_file):
       for c, idx in enumerate(row):
         mat  = materials[idx]
         tile = self.tiles[r, c]
         tile.reset(mat, config)
 
+    assert c == config.MAP_SIZE - 1
+    assert r == config.MAP_SIZE - 1
+
+    self._repr = None
+
   def step(self):
     '''Evaluate updatable tiles'''
     self.realm.log_milestone('Resource_Depleted', len(self.update_list),
         f'RESOURCE: Depleted {len(self.update_list)} resource tiles')
 
     for e in self.update_list.copy():
       if not e.depleted:
@@ -76,7 +82,11 @@
   def harvest(self, r, c, deplete=True):
     '''Called by actions that harvest a resource tile'''
 
     if deplete:
       self.update_list.add(self.tiles[r, c])
 
     return self.tiles[r, c].harvest(deplete)
+
+  def is_valid_pos(self, row, col):
+    '''Check if a position is valid'''
+    return 0 <= row < self.config.MAP_SIZE and 0 <= col < self.config.MAP_SIZE
```

### Comparing `nmmo-1.7.0.1/nmmo/core/observation.py` & `nmmo-2.0.0/nmmo/core/observation.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 import numpy as np
 
 from nmmo.core.tile import TileState
 from nmmo.entity.entity import EntityState
 from nmmo.systems.item import ItemState
 import nmmo.systems.item as item_system
-from nmmo.io import action
+from nmmo.core import action
 from nmmo.lib import material, utils
 
 
 class BasicObs:
   def __init__(self, values, id_col):
     self.values = values
     self.ids = values[:, id_col]
@@ -36,27 +36,36 @@
     idx = np.nonzero((self.inv_type == item.ITEM_TYPE_ID) & (self.inv_level == level))[0]
     return idx[0] if len(idx) else None
 
 
 class Observation:
   def __init__(self,
     config,
+    current_tick: int,
     agent_id: int,
     tiles,
     entities,
     inventory,
     market) -> None:
 
     self.config = config
+    self.current_tick = current_tick
     self.agent_id = agent_id
 
     self.tiles = tiles[0:config.MAP_N_OBS]
     self.entities = BasicObs(entities[0:config.PLAYER_N_OBS],
                               EntityState.State.attr_name_to_col["id"])
 
+    if config.COMBAT_SYSTEM_ENABLED:
+      latest_combat_tick = self.agent().latest_combat_tick
+      self.agent_in_combat = False if latest_combat_tick == 0 else \
+        (current_tick - latest_combat_tick) < config.COMBAT_STATUS_DURATION
+    else:
+      self.agent_in_combat = False
+
     if config.ITEM_SYSTEM_ENABLED:
       self.inventory = InventoryObs(inventory[0:config.INVENTORY_N_OBS],
                                     ItemState.State.attr_name_to_col["id"])
     else:
       assert inventory.size == 0
 
     if config.EXCHANGE_SYSTEM_ENABLED:
@@ -74,17 +83,25 @@
         r_delta: row offset from current agent
         c_delta: col offset from current agent
 
     Returns:
         Vector corresponding to the specified tile
     '''
     agent = self.agent()
-    r_cond = (self.tiles[:,TileState.State.attr_name_to_col["row"]] == agent.row + r_delta)
-    c_cond = (self.tiles[:,TileState.State.attr_name_to_col["col"]] == agent.col + c_delta)
-    return TileState.parse_array(self.tiles[r_cond & c_cond][0])
+    center = self.config.PLAYER_VISION_RADIUS
+    tile_dim = self.config.PLAYER_VISION_DIAMETER
+    mat_map = self.tiles[:,2].reshape(tile_dim,tile_dim)
+    new_row = agent.row + r_delta
+    new_col = agent.col + c_delta
+    if (0 <= new_row < self.config.MAP_SIZE) & \
+       (0 <= new_col < self.config.MAP_SIZE):
+      return TileState.parse_array([new_row, new_col, mat_map[center+r_delta,center+c_delta]])
+
+    # return a dummy void tile at (inf, inf)
+    return TileState.parse_array([np.inf, np.inf, material.Void.index])
 
   # pylint: disable=method-cache-max-size-none
   @lru_cache(maxsize=None)
   def entity(self, entity_id):
     rows = self.entities.values[self.entities.ids == entity_id]
     if rows.size == 0:
       return None
@@ -94,48 +111,43 @@
   @lru_cache(maxsize=None)
   def agent(self):
     return self.entity(self.agent_id)
 
   def to_gym(self):
     '''Convert the observation to a format that can be used by OpenAI Gym'''
 
+    tiles = np.zeros((self.config.MAP_N_OBS, self.tiles.shape[1]))
+    tiles[:self.tiles.shape[0],:] = self.tiles
+
+    entities = np.zeros((self.config.PLAYER_N_OBS, self.entities.values.shape[1]))
+    entities[:self.entities.values.shape[0],:] = self.entities.values
+
     gym_obs = {
-      "Tile": np.vstack([
-        self.tiles,
-        np.zeros((self.config.MAP_N_OBS - self.tiles.shape[0], self.tiles.shape[1]))
-      ]),
-      "Entity": np.vstack([
-        self.entities.values, np.zeros((
-          self.config.PLAYER_N_OBS - self.entities.values.shape[0],
-          self.entities.values.shape[1]))
-      ]),
+      "CurrentTick": np.array([self.current_tick]),
+      "AgentId": np.array([self.agent_id]),
+      "Tile": tiles,
+      "Entity": entities,
     }
 
     if self.config.ITEM_SYSTEM_ENABLED:
-      gym_obs["Inventory"] = np.vstack([
-        self.inventory.values, np.zeros((
-          self.config.INVENTORY_N_OBS - self.inventory.values.shape[0],
-          self.inventory.values.shape[1]))
-      ])
+      inventory = np.zeros((self.config.INVENTORY_N_OBS, self.inventory.values.shape[1]))
+      inventory[:self.inventory.values.shape[0],:] = self.inventory.values
+      gym_obs["Inventory"] = inventory
 
     if self.config.EXCHANGE_SYSTEM_ENABLED:
-      gym_obs["Market"] = np.vstack([
-        self.market.values, np.zeros((
-          self.config.MARKET_N_OBS - self.market.values.shape[0],
-          self.market.values.shape[1]))
-      ])
+      market = np.zeros((self.config.MARKET_N_OBS, self.market.values.shape[1]))
+      market[:self.market.values.shape[0],:] = self.market.values
+      gym_obs["Market"] = market
 
     if self.config.PROVIDE_ACTION_TARGETS:
       gym_obs["ActionTargets"] = self._make_action_targets()
 
     return gym_obs
 
   def _make_action_targets(self):
-    # TODO(kywch): return all-0 masks for buy/sell/give during combat
-
     masks = {}
     masks[action.Move] = {
       action.Direction: self._make_move_mask()
     }
 
     if self.config.COMBAT_SYSTEM_ENABLED:
       masks[action.Attack] = {
@@ -173,190 +185,188 @@
         action.Token: np.ones(len(action.Token.edges), dtype=np.int8)
       }
 
     return masks
 
   def _make_move_mask(self):
     # pylint: disable=not-an-iterable
-    return np.array(
-      [self.tile(*d.delta).material_id in material.Habitable
-       for d in action.Direction.edges], dtype=np.int8)
+    return np.array([self.tile(*d.delta).material_id in material.Habitable.indices
+                     for d in action.Direction.edges], dtype=np.int8)
 
   def _make_attack_mask(self):
-    # TODO: Currently, all attacks have the same range
+    # NOTE: Currently, all attacks have the same range
     #   if we choose to make ranges different, the masks
     #   should be differently generated by attack styles
     assert self.config.COMBAT_MELEE_REACH == self.config.COMBAT_RANGE_REACH
     assert self.config.COMBAT_MELEE_REACH == self.config.COMBAT_MAGE_REACH
     assert self.config.COMBAT_RANGE_REACH == self.config.COMBAT_MAGE_REACH
 
     attack_range = self.config.COMBAT_MELEE_REACH
 
     agent = self.agent()
-    entities_pos = self.entities.values[:, [EntityState.State.attr_name_to_col["row"],
-                                            EntityState.State.attr_name_to_col["col"]]]
-    within_range = utils.linf(entities_pos, (agent.row, agent.col)) <= attack_range
+    entities_pos = self.entities.values[:,[EntityState.State.attr_name_to_col["row"],
+                                           EntityState.State.attr_name_to_col["col"]]]
+    within_range = utils.linf(entities_pos,(agent.row, agent.col)) <= attack_range
 
     immunity = self.config.COMBAT_SPAWN_IMMUNITY
     if 0 < immunity < agent.time_alive:
       # ids > 0 equals entity.is_player
       spawn_immunity = (self.entities.ids > 0) & \
         (self.entities.values[:,EntityState.State.attr_name_to_col["time_alive"]] < immunity)
     else:
-      spawn_immunity = np.ones(self.entities.len, dtype=np.int8)
+      spawn_immunity = np.ones(self.entities.len, dtype=bool)
 
-    if not self.config.COMBAT_FRIENDLY_FIRE:
-      population = self.entities.values[:,EntityState.State.attr_name_to_col["population_id"]]
-      no_friendly_fire = population != agent.population_id # this automatically masks self
-    else:
-      # allow friendly fire but no self shooting
-      no_friendly_fire = np.ones(self.entities.len, dtype=np.int8)
-      no_friendly_fire[self.entities.index(agent.id)] = 0 # mask self
+    # allow friendly fire but no self shooting
+    not_me = self.entities.ids != agent.id
 
-    return np.concatenate([within_range & no_friendly_fire & spawn_immunity,
-      np.zeros(self.config.PLAYER_N_OBS - self.entities.len, dtype=np.int8)])
+    attack_mask = np.zeros(self.config.PLAYER_N_OBS, dtype=np.int8)
+    attack_mask[:self.entities.len] = within_range & not_me & spawn_immunity
+    return attack_mask
 
   def _make_use_mask(self):
     # empty inventory -- nothing to use
-    if not (self.config.ITEM_SYSTEM_ENABLED and self.inventory.len > 0):
-      return np.zeros(self.config.INVENTORY_N_OBS, dtype=np.int8)
+    use_mask = np.zeros(self.config.INVENTORY_N_OBS, dtype=np.int8)
+    if not (self.config.ITEM_SYSTEM_ENABLED and self.inventory.len > 0) or self.agent_in_combat:
+      return use_mask
 
     item_skill = self._item_skill()
 
     not_listed = self.inventory.values[:,ItemState.State.attr_name_to_col["listed_price"]] == 0
     item_type = self.inventory.values[:,ItemState.State.attr_name_to_col["type_id"]]
     item_level = self.inventory.values[:,ItemState.State.attr_name_to_col["level"]]
 
     # level limits are differently applied depending on item types
-    type_flt = np.tile ( np.array(list(item_skill.keys())), (self.inventory.len,1) )
-    level_flt = np.tile ( np.array(list(item_skill.values())), (self.inventory.len,1) )
-    item_type = np.tile( np.transpose(np.atleast_2d(item_type)), (1, len(item_skill)))
-    item_level = np.tile( np.transpose(np.atleast_2d(item_level)), (1, len(item_skill)))
-    level_satisfied = np.any((item_type == type_flt) & (item_level <= level_flt), axis=1)
+    type_flt = np.tile(np.array(list(item_skill.keys())), (self.inventory.len,1))
+    level_flt = np.tile(np.array(list(item_skill.values())), (self.inventory.len,1))
+    item_type = np.tile(np.transpose(np.atleast_2d(item_type)), (1, len(item_skill)))
+    item_level = np.tile(np.transpose(np.atleast_2d(item_level)), (1, len(item_skill)))
+    level_satisfied = np.any((item_type==type_flt) & (item_level<=level_flt), axis=1)
 
-    return np.concatenate([not_listed & level_satisfied,
-      np.zeros(self.config.INVENTORY_N_OBS - self.inventory.len, dtype=np.int8)])
+    use_mask[:self.inventory.len] = not_listed & level_satisfied
+    return use_mask
 
   def _item_skill(self):
     agent = self.agent()
 
     # the minimum agent level is 1
     level = max(1, agent.melee_level, agent.range_level, agent.mage_level,
                 agent.fishing_level, agent.herbalism_level, agent.prospecting_level,
                 agent.carving_level, agent.alchemy_level)
     return {
       item_system.Hat.ITEM_TYPE_ID: level,
       item_system.Top.ITEM_TYPE_ID: level,
       item_system.Bottom.ITEM_TYPE_ID: level,
-      item_system.Sword.ITEM_TYPE_ID: agent.melee_level,
+      item_system.Spear.ITEM_TYPE_ID: agent.melee_level,
       item_system.Bow.ITEM_TYPE_ID: agent.range_level,
       item_system.Wand.ITEM_TYPE_ID: agent.mage_level,
       item_system.Rod.ITEM_TYPE_ID: agent.fishing_level,
       item_system.Gloves.ITEM_TYPE_ID: agent.herbalism_level,
       item_system.Pickaxe.ITEM_TYPE_ID: agent.prospecting_level,
-      item_system.Chisel.ITEM_TYPE_ID: agent.carving_level,
-      item_system.Arcane.ITEM_TYPE_ID: agent.alchemy_level,
-      item_system.Scrap.ITEM_TYPE_ID: agent.melee_level,
-      item_system.Shaving.ITEM_TYPE_ID: agent.range_level,
-      item_system.Shard.ITEM_TYPE_ID: agent.mage_level,
+      item_system.Axe.ITEM_TYPE_ID: agent.carving_level,
+      item_system.Chisel.ITEM_TYPE_ID: agent.alchemy_level,
+      item_system.Whetstone.ITEM_TYPE_ID: agent.melee_level,
+      item_system.Arrow.ITEM_TYPE_ID: agent.range_level,
+      item_system.Runes.ITEM_TYPE_ID: agent.mage_level,
       item_system.Ration.ITEM_TYPE_ID: level,
-      item_system.Poultice.ITEM_TYPE_ID: level
+      item_system.Potion.ITEM_TYPE_ID: level
     }
 
   def _make_destroy_item_mask(self):
+    destroy_mask = np.zeros(self.config.INVENTORY_N_OBS, dtype=np.int8)
     # empty inventory -- nothing to destroy
-    if not (self.config.ITEM_SYSTEM_ENABLED and self.inventory.len > 0):
-      return np.zeros(self.config.INVENTORY_N_OBS, dtype=np.int8)
+    if not (self.config.ITEM_SYSTEM_ENABLED and self.inventory.len > 0) or self.agent_in_combat:
+      return destroy_mask
 
+    # not equipped items in the inventory can be destroyed
     not_equipped = self.inventory.values[:,ItemState.State.attr_name_to_col["equipped"]] == 0
 
-    # not equipped items in the inventory can be destroyed
-    return np.concatenate([not_equipped,
-      np.zeros(self.config.INVENTORY_N_OBS - self.inventory.len, dtype=np.int8)])
+    destroy_mask[:self.inventory.len] = not_equipped
+    return destroy_mask
 
   def _make_give_target_mask(self):
+    give_mask = np.zeros(self.config.PLAYER_N_OBS, dtype=np.int8)
     # empty inventory -- nothing to give
-    if not (self.config.ITEM_SYSTEM_ENABLED and self.inventory.len > 0):
-      return np.zeros(self.config.PLAYER_N_OBS, dtype=np.int8)
+    if not (self.config.ITEM_SYSTEM_ENABLED and self.inventory.len > 0) or self.agent_in_combat:
+      return give_mask
 
     agent = self.agent()
-    entities_pos = self.entities.values[:, [EntityState.State.attr_name_to_col["row"],
-                                            EntityState.State.attr_name_to_col["col"]]]
+    entities_pos = self.entities.values[:,[EntityState.State.attr_name_to_col["row"],
+                                           EntityState.State.attr_name_to_col["col"]]]
     same_tile = utils.linf(entities_pos, (agent.row, agent.col)) == 0
-    same_team_not_me = (self.entities.ids != agent.id) & (agent.population_id == \
-                self.entities.values[:, EntityState.State.attr_name_to_col["population_id"]])
+    not_me = self.entities.ids != self.agent_id
+    player = (self.entities.values[:,EntityState.State.attr_name_to_col["npc_type"]] == 0)
 
-    return np.concatenate([same_tile & same_team_not_me,
-      np.zeros(self.config.PLAYER_N_OBS - self.entities.len, dtype=np.int8)])
+    give_mask[:self.entities.len] = same_tile & player & not_me
+    return give_mask
 
   def _make_give_gold_mask(self):
     gold = int(self.agent().gold)
     mask = np.zeros(self.config.PRICE_N_OBS, dtype=np.int8)
 
-    if gold:
+    if gold and not self.agent_in_combat:
       mask[:gold] = 1 # NOTE that action.Price starts from Discrete_1
 
     return mask
 
   def _make_sell_mask(self):
+    sell_mask = np.zeros(self.config.INVENTORY_N_OBS, dtype=np.int8)
     # empty inventory -- nothing to sell
-    if not (self.config.EXCHANGE_SYSTEM_ENABLED and self.inventory.len > 0):
-      return np.zeros(self.config.INVENTORY_N_OBS, dtype=np.int8)
+    if not (self.config.EXCHANGE_SYSTEM_ENABLED and self.inventory.len > 0) \
+      or self.agent_in_combat:
+      return sell_mask
 
     not_equipped = self.inventory.values[:,ItemState.State.attr_name_to_col["equipped"]] == 0
     not_listed = self.inventory.values[:,ItemState.State.attr_name_to_col["listed_price"]] == 0
 
-    return np.concatenate([not_equipped & not_listed,
-      np.zeros(self.config.INVENTORY_N_OBS - self.inventory.len, dtype=np.int8)])
+    sell_mask[:self.inventory.len] = not_equipped & not_listed
+    return sell_mask
 
   def _make_buy_mask(self):
-    if not self.config.EXCHANGE_SYSTEM_ENABLED:
-      return np.zeros(self.config.MARKET_N_OBS, dtype=np.int8)
+    buy_mask = np.zeros(self.config.MARKET_N_OBS, dtype=np.int8)
+    if not self.config.EXCHANGE_SYSTEM_ENABLED or self.agent_in_combat:
+      return buy_mask
 
-    market_flt = np.ones(self.market.len, dtype=np.int8)
-    full_inventory = self.inventory.len >= self.config.ITEM_INVENTORY_CAPACITY
+    agent = self.agent()
+    market_items = self.market.values
+    not_mine = market_items[:,ItemState.State.attr_name_to_col["owner_id"]] != self.agent_id
 
     # if the inventory is full, one can only buy existing ammo stack
     #   otherwise, one can buy anything owned by other, having enough money
-    if full_inventory:
+    if self.inventory.len >= self.config.ITEM_INVENTORY_CAPACITY:
       exist_ammo_listings = self._existing_ammo_listings()
       if not np.any(exist_ammo_listings):
         return np.zeros(self.config.MARKET_N_OBS, dtype=np.int8)
-      market_flt = exist_ammo_listings
+      not_mine &= exist_ammo_listings
 
-    agent = self.agent()
-    market_items = self.market.values
     enough_gold = market_items[:,ItemState.State.attr_name_to_col["listed_price"]] <= agent.gold
-    not_mine = market_items[:,ItemState.State.attr_name_to_col["owner_id"]] != self.agent_id
-
-    return np.concatenate([market_flt & enough_gold & not_mine,
-      np.zeros(self.config.MARKET_N_OBS - self.market.len, dtype=np.int8)])
+    buy_mask[:self.market.len] = not_mine & enough_gold
+    return buy_mask
 
   def _existing_ammo_listings(self):
     sig_col = (ItemState.State.attr_name_to_col["type_id"],
                ItemState.State.attr_name_to_col["level"])
     ammo_id = [ammo.ITEM_TYPE_ID for ammo in
-              [item_system.Scrap, item_system.Shaving, item_system.Shard]]
+              [item_system.Whetstone, item_system.Arrow, item_system.Runes]]
 
     # search ammo stack from the inventory
-    type_flt = np.tile( np.array(ammo_id), (self.inventory.len,1))
+    type_flt = np.tile(np.array(ammo_id), (self.inventory.len,1))
     item_type = np.tile(
       np.transpose(np.atleast_2d(self.inventory.values[:,sig_col[0]])),
       (1, len(ammo_id)))
     exist_ammo = self.inventory.values[np.any(item_type == type_flt, axis=1)]
 
     # self does not have ammo
     if exist_ammo.shape[0] == 0:
-      return np.zeros(self.market.len, dtype=np.int8)
+      return np.zeros(self.market.len, dtype=bool)
 
     # search the existing ammo stack from the market that's not mine
-    type_flt = np.tile( np.array(exist_ammo[:,sig_col[0]]), (self.market.len,1))
-    level_flt = np.tile( np.array(exist_ammo[:,sig_col[1]]), (self.market.len,1))
-    item_type = np.tile( np.transpose(np.atleast_2d(self.market.values[:,sig_col[0]])),
-      (1, exist_ammo.shape[0]))
-    item_level = np.tile( np.transpose(np.atleast_2d(self.market.values[:,sig_col[1]])),
-      (1, exist_ammo.shape[0]))
-    exist_ammo_listings = np.any((item_type == type_flt) & (item_level == level_flt), axis=1)
+    type_flt = np.tile(np.array(exist_ammo[:,sig_col[0]]), (self.market.len,1))
+    level_flt = np.tile(np.array(exist_ammo[:,sig_col[1]]), (self.market.len,1))
+    item_type = np.tile(np.transpose(np.atleast_2d(self.market.values[:,sig_col[0]])),
+                        (1, exist_ammo.shape[0]))
+    item_level = np.tile(np.transpose(np.atleast_2d(self.market.values[:,sig_col[1]])),
+                         (1, exist_ammo.shape[0]))
+    exist_ammo_listings = np.any((item_type==type_flt) & (item_level==level_flt), axis=1)
 
     not_mine = self.market.values[:,ItemState.State.attr_name_to_col["owner_id"]] != self.agent_id
 
     return exist_ammo_listings & not_mine
```

### Comparing `nmmo-1.7.0.1/nmmo/core/realm.py` & `nmmo-2.0.0/nmmo/core/realm.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from typing import Dict
 
 import numpy as np
 
 import nmmo
 from nmmo.core.log_helper import LogHelper
 from nmmo.core.map import Map
-from nmmo.core.render_helper import RenderHelper
-from nmmo.core.replay_helper import ReplayHelper
 from nmmo.core.tile import TileState
+from nmmo.core.action import Action, Buy
 from nmmo.entity.entity import EntityState
 from nmmo.entity.entity_manager import NPCManager, PlayerManager
-from nmmo.io.action import Action, Buy
 from nmmo.datastore.numpy_datastore import NumpyDatastore
 from nmmo.systems.exchange import Exchange
 from nmmo.systems.item import Item, ItemState
+from nmmo.lib.event_log import EventLogger, EventState
+from nmmo.render.replay_helper import ReplayHelper
 
 def prioritized(entities: Dict, merged: Dict):
   """Sort actions into merged according to priority"""
   for idx, actions in entities.items():
     for atn, args in actions.items():
       merged[atn.priority].append((idx, (atn, args.values())))
   return merged
@@ -38,85 +38,91 @@
 
     Action.hook(config)
 
     # Generate maps if they do not exist
     config.MAP_GENERATOR(config).generate_all_maps()
 
     self.datastore = NumpyDatastore()
-    for s in [TileState, EntityState, ItemState]:
+    for s in [TileState, EntityState, ItemState, EventState]:
       self.datastore.register_object_type(s._name, s.State.num_attributes)
 
-    self.tick = 0
+    self.tick = None # to use as a "reset" checker
     self.exchange = None
 
     # Load the world file
     self.map = Map(config, self)
 
-    self.replay_helper = ReplayHelper.create(self)
-    self.render_helper = RenderHelper.create(self)
     self.log_helper = LogHelper.create(self)
+    self.event_log = EventLogger(self)
 
     # Entity handlers
     self.players = PlayerManager(self)
     self.npcs = NPCManager(self)
 
     # Global item registry
     self.items = {}
 
+    # Replay helper
+    self._replay_helper = None
+
     # Initialize actions
     nmmo.Action.init(config)
 
   def reset(self, map_id: int = None):
     """Reset the environment and load the specified map
 
     Args:
         idx: Map index to load
     """
     self.log_helper.reset()
-    self.map.reset(map_id or np.random.randint(self.config.MAP_N) + 1)
+    self.event_log.reset()
+
+    map_id = map_id or np.random.randint(self.config.MAP_N) + 1
+    self.map.reset(map_id)
+    self.tick = 0
 
     # EntityState and ItemState tables must be empty after players/npcs.reset()
     self.players.reset()
     self.npcs.reset()
     assert EntityState.State.table(self.datastore).is_empty(), \
         "EntityState table is not empty"
+    assert ItemState.State.table(self.datastore).is_empty(), \
+        "ItemState table is not empty"
 
-    # TODO(kywch): ItemState table is not empty after players/npcs.reset()
-    #   but should be. Will fix this while debugging the item system.
-    # assert ItemState.State.table(self.datastore).is_empty(), \
-    #     "ItemState table is not empty"
+    # DataStore id allocator must be reset to be deterministic
+    EntityState.State.table(self.datastore).reset()
     ItemState.State.table(self.datastore).reset()
 
     self.players.spawn()
     self.npcs.spawn()
-    self.tick = 0
 
     # Global item exchange
     self.exchange = Exchange(self)
 
     # Global item registry
     Item.INSTANCE_ID = 0
     self.items = {}
 
-    self.replay_helper.update()
+    if self._replay_helper is not None:
+      self._replay_helper.reset()
 
   def packet(self):
     """Client packet"""
     return {
       "environment": self.map.repr,
       "border": self.config.MAP_BORDER,
       "size": self.config.MAP_SIZE,
       "resource": self.map.packet,
       "player": self.players.packet,
       "npc": self.npcs.packet,
       "market": self.exchange.packet,
   }
 
   @property
-  def population(self):
+  def num_players(self):
     """Number of player agents"""
     return len(self.players.entities)
 
   def entity(self, ent_id):
     e = self.entity_or_none(ent_id)
     assert e is not None, f"Entity {ent_id} does not exist"
     return e
@@ -155,44 +161,50 @@
     #  - 20: Buy - exchange while sellers, items, buyers are all intact
     #  - 30: Give, GiveGold - transfer while both are alive and at the same tile
     #  - 40: Destroy - use with SELL/GIVE, if not gone, destroy and recover space
     #  - 50: Attack
     #  - 60: Move
     #  - 70: Sell - to guarantee the listed items are available to buy
     #  - 99: Comm
+
     for priority in sorted(merged):
       # TODO: we should be randomizing these, otherwise the lower ID agents
       # will always go first. --> ONLY SHUFFLE BUY
       if priority == Buy.priority:
         np.random.shuffle(merged[priority])
 
       # CHECK ME: do we need this line?
       # ent_id, (atn, args) = merged[priority][0]
       for ent_id, (atn, args) in merged[priority]:
         ent = self.entity(ent_id)
         if ent.alive:
           atn.call(self, ent, *args)
-
     dead = self.players.cull()
     self.npcs.cull()
 
     # Update map
     self.map.step()
     self.exchange.step(self.tick)
     self.log_helper.update(dead)
+    if self._replay_helper is not None:
+      self._replay_helper.update()
 
     self.tick += 1
 
-    self.replay_helper.update()
-
     return dead
 
   def log_milestone(self, category: str, value: float, message: str = None, tags: Dict = None):
     self.log_helper.log_milestone(category, value)
     self.log_helper.log_event(category, value)
 
     if self.config.LOG_VERBOSE:
       # TODO: more general handling of tags, if necessary
       if tags and 'player_id' in tags:
         logging.info("Milestone (Player %d): %s %s %s", tags['player_id'], category, value, message)
       else:
         logging.info("Milestone: %s %s %s", category, value, message)
+
+  def record_replay(self, replay_helper: ReplayHelper) -> ReplayHelper:
+    self._replay_helper = replay_helper
+    self._replay_helper.set_realm(self)
+
+    return replay_helper
```

### Comparing `nmmo-1.7.0.1/nmmo/core/terrain.py` & `nmmo-2.0.0/nmmo/core/terrain.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 
 import os
 import random
 import logging
 
 import numpy as np
 import vec_noise
-from imageio import imread, imsave
+from imageio.v2 import imread, imsave
 from scipy import stats
-from tqdm import tqdm
 
 from nmmo import material
 
 
 def sharp(noise):
   '''Exponential noise sharpener for perlin ridges'''
   return 2 * (0.5 - abs(0.5 - noise))
@@ -126,41 +125,47 @@
     for y in range(size):
       for x in range(size):
         v = val[y, x]
         if v <= config.TERRAIN_WATER:
           mat = Terrain.WATER
         elif v <= config.TERRAIN_GRASS:
           mat = Terrain.GRASS
-        elif v <= config.TERRAIN_FOREST:
-          mat = Terrain.FOREST
+        elif v <= config.TERRAIN_FOILAGE:
+          mat = Terrain.FOILAGE
         else:
           mat = Terrain.STONE
         matl[y, x] = mat
 
-    #Lava and grass border
-    matl[l1 > size/2 - border]   = Terrain.LAVA
+    # Void and grass border
+    matl[l1 > size/2 - border]   = Terrain.VOID
     matl[l1 == size//2 - border] = Terrain.GRASS
 
     edge  = l1 == size//2 - border - 1
     stone = (matl == Terrain.STONE) | (matl == Terrain.WATER)
-    matl[edge & stone] = Terrain.FOREST
+    matl[edge & stone] = Terrain.FOILAGE
 
     return val, matl, interpolaters
 
-def fish(config, tiles, mat, mmin, mmax):
-  r = random.randint(mmin, mmax)
-  c = random.randint(mmin, mmax)
-
+def place_fish(tiles):
+  placed = False
   allow = {Terrain.GRASS}
-  if (tiles[r, c] not in {Terrain.WATER} or
-          (tiles[r-1, c] not in allow and tiles[r+1, c] not in allow and
-          tiles[r, c-1] not in allow and tiles[r, c+1] not in allow)):
-    fish(config, tiles, mat, mmin, mmax)
-  else:
-    tiles[r, c] = mat
+
+  water_loc = np.where(tiles == Terrain.WATER)
+  water_loc = list(zip(water_loc[0], water_loc[1]))
+  random.shuffle(water_loc)
+
+  for r, c in water_loc:
+    if tiles[r-1, c] in allow or tiles[r+1, c] in allow or \
+       tiles[r, c-1] in allow or tiles[r, c+1] in allow:
+      tiles[r, c] = Terrain.FISH
+      placed = True
+      break
+
+  if not placed:
+    raise RuntimeError('Could not find the water tile to place fish.')
 
 def uniform(config, tiles, mat, mmin, mmax):
   r = random.randint(mmin, mmax)
   c = random.randint(mmin, mmax)
 
   if tiles[r, c] not in {Terrain.GRASS}:
     uniform(config, tiles, mat, mmin, mmax)
@@ -196,15 +201,15 @@
   for _ in range(config.PROGRESSION_SPAWN_CLUSTERS):
     cluster(config, tiles, Terrain.ORE, mmin, mmax)
     cluster(config, tiles, Terrain.TREE, mmin, mmax)
     cluster(config, tiles, Terrain.CRYSTAL, mmin, mmax)
 
   for _ in range(config.PROGRESSION_SPAWN_UNIFORMS):
     uniform(config, tiles, Terrain.HERB, mmin, mmax)
-    fish(config, tiles, Terrain.FISH, mmin, mmax)
+    place_fish(tiles)
 
 class MapGenerator:
   '''Procedural map generation'''
   def __init__(self, config):
     self.config = config
     self.load_textures()
     self.interpolaters = None
@@ -227,21 +232,28 @@
     Provides additional utilities for saving to .npy and rendering png previews'''
 
     config = self.config
 
     #Only generate if maps are not cached
     path_maps = os.path.join(config.PATH_CWD, config.PATH_MAPS)
     os.makedirs(path_maps, exist_ok=True)
-    if not config.MAP_FORCE_GENERATION and os.listdir(path_maps):
-      return
+
+    existing_maps = set(map_dir + '/map.npy' for map_dir in os.listdir(path_maps))
+    if not config.MAP_FORCE_GENERATION and existing_maps:
+      required_maps = {
+        f'map{idx}/map.npy' for idx in range(1, config.MAP_N+1)
+      }
+      missing = required_maps - existing_maps
+      if not missing:
+        return
 
     if __debug__:
       logging.info('Generating %s maps', str(config.MAP_N))
 
-    for idx in tqdm(range(config.MAP_N)):
+    for idx in range(config.MAP_N):
       path = path_maps + '/map' + str(idx+1)
       os.makedirs(path, exist_ok=True)
 
       terrain, tiles = self.generate_map(idx)
 
       #Save/render
       Save.as_numpy(tiles, path)
@@ -276,13 +288,13 @@
 
       for r in range(size):
         for c in range(size):
           linf = max(abs(r - size//2), abs(c - size//2))
           if linf <= size//2 - config.MAP_BORDER:
             tiles[r, c] = Terrain.GRASS
           else:
-            tiles[r, c] = Terrain.LAVA
+            tiles[r, c] = Terrain.VOID
 
     if config.PROFESSION_SYSTEM_ENABLED:
       spawn_profession_resources(config, tiles)
 
     return terrain, tiles
```

### Comparing `nmmo-1.7.0.1/nmmo/core/tile.py` & `nmmo-2.0.0/nmmo/core/tile.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     return self.material in material.Habitable
 
   @property
   def impassible(self):
     return self.material in material.Impassible
 
   @property
-  def lava(self):
-    return self.material == material.Lava
+  def void(self):
+    return self.material == material.Void
 
   def reset(self, mat, config):
     self.state = mat(config)
     self.material = mat(config)
     self.material_id.update(self.state.index)
 
     self.depleted = False
```

### Comparing `nmmo-1.7.0.1/nmmo/datastore/datastore.py` & `nmmo-2.0.0/nmmo/datastore/datastore.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/datastore/numpy_datastore.py` & `nmmo-2.0.0/nmmo/datastore/numpy_datastore.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/datastore/serialized.py` & `nmmo-2.0.0/nmmo/datastore/serialized.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/entity/entity.py` & `nmmo-2.0.0/nmmo/entity/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 
 import math
 from types import SimpleNamespace
 
 import numpy as np
 
 from nmmo.core.config import Config
-from nmmo.lib import utils
 from nmmo.datastore.serialized import SerializedState
 from nmmo.systems import inventory
+from nmmo.lib.log import EventCode
 
 # pylint: disable=no-member
 EntityState = SerializedState.subclass(
   "Entity", [
     "id",
-    "population_id",
+    "npc_type", # 1 - passive, 2 - neutral, 3 - aggressive
     "row",
     "col",
 
     # Status
     "damage",
     "time_alive",
     "freeze",
     "item_level",
     "attacker_id",
+    "latest_combat_tick",
     "message",
 
     # Resources
     "gold",
     "health",
     "food",
     "water",
@@ -43,22 +44,23 @@
     "carving_level",
     "alchemy_level",
   ])
 
 EntityState.Limits = lambda config: {
   **{
     "id": (-math.inf, math.inf),
-    "population_id": (-3, config.PLAYER_POLICIES-1),
+    "npc_type": (0, 4),
     "row": (0, config.MAP_SIZE-1),
     "col": (0, config.MAP_SIZE-1),
     "damage": (0, math.inf),
     "time_alive": (0, math.inf),
     "freeze": (0, 3),
     "item_level": (0, 5*config.NPC_LEVEL_MAX),
     "attacker_id": (-np.inf, math.inf),
+    "latest_combat_tick": (0, math.inf),
     "health": (0, config.PLAYER_BASE_HEALTH),
   },
   **({
     "message": (0, config.COMMUNICATION_NUM_TOKENS),
   } if config.COMMUNICATION_SYSTEM_ENABLED else {}),
   **({
     "gold": (0, math.inf),
@@ -127,17 +129,17 @@
       self.health.decrement(self.config.RESOURCE_STARVATION_RATE)
 
     if self.water.empty:
       self.health.decrement(self.config.RESOURCE_DEHYDRATION_RATE)
 
   def packet(self):
     data = {}
-    data['health'] = self.health.val
-    data['food'] = self.food.val
-    data['water'] = self.water.val
+    data['health'] = { 'val': self.health.val, 'max': self.config.PLAYER_BASE_HEALTH }
+    data['food'] = { 'val': self.food.val, 'max': self.config.RESOURCE_BASE }
+    data['water'] = { 'val': self.water.val, 'max': self.config.RESOURCE_BASE }
     return data
 
 class Status:
   def __init__(self, ent):
     self.freeze = ent.freeze
 
   def update(self):
@@ -146,14 +148,15 @@
 
   def packet(self):
     data = {}
     data['freeze'] = self.freeze.val
     return data
 
 
+# NOTE: History.packet() is actively used in visulazing attacks
 class History:
   def __init__(self, ent):
     self.actions = {}
     self.attack = None
 
     self.starting_position = ent.pos
     self.exploration = 0
@@ -171,65 +174,63 @@
     self.attack = None
     self.damage.update(0)
 
     self.actions = {}
     if entity.ent_id in actions:
       self.actions = actions[entity.ent_id]
 
-    exploration = utils.linf(entity.pos, self.starting_position)
-    self.exploration = max(exploration, self.exploration)
-
     self.time_alive.increment()
 
   def packet(self):
     data = {}
     data['damage'] = self.damage.val
     data['timeAlive'] = self.time_alive.val
     data['damage_inflicted'] = self.damage_inflicted
     data['damage_received'] = self.damage_received
 
     if self.attack is not None:
       data['attack'] = self.attack
 
-    actions = {}
-    for atn, args in self.actions.items():
-      atn_packet = {}
-
-      # Avoid recursive player packet
-      if atn.__name__ == 'Attack':
-        continue
-
-      for key, val in args.items():
-        if hasattr(val, 'packet'):
-          atn_packet[key.__name__] = val.packet
-        else:
-          atn_packet[key.__name__] = val.__name__
-      actions[atn.__name__] = atn_packet
-    data['actions'] = actions
+    # NOTE: the client seems to use actions for visualization
+    #   but produces errors with the new actions. So we comment out these for now
+    # actions = {}
+    # for atn, args in self.actions.items():
+    #   atn_packet = {}
+
+    #   # Avoid recursive player packet
+    #   if atn.__name__ == 'Attack':
+    #     continue
+
+    #   for key, val in args.items():
+    #     if hasattr(val, 'packet'):
+    #       atn_packet[key.__name__] = val.packet
+    #     else:
+    #       atn_packet[key.__name__] = val.__name__
+    #   actions[atn.__name__] = atn_packet
+    # data['actions'] = actions
+    data['actions'] = {}
 
     return data
 
 # pylint: disable=no-member
 class Entity(EntityState):
-  def __init__(self, realm, pos, entity_id, name, color, population_id):
+  def __init__(self, realm, pos, entity_id, name):
     super().__init__(realm.datastore, EntityState.Limits(realm.config))
 
     self.realm = realm
     self.config: Config = realm.config
 
     self.policy = name
     self.entity_id = entity_id
     self.repr = None
 
     self.name = name + str(entity_id)
-    self.color = color
 
     self.row.update(pos[0])
     self.col.update(pos[1])
-    self.population_id.update(population_id)
     self.id.update(entity_id)
 
     self.vision = self.config.PLAYER_VISION_RADIUS
 
     self.attacker = None
     self.target = None
     self.closest = None
@@ -254,18 +255,14 @@
     data['alive'] = self.alive
     data['base'] = {
       'r': self.row.val,
       'c': self.col.val,
       'name': self.name,
       'level': self.attack_level,
       'item_level': self.item_level.val,
-      'color': self.color.packet(),
-      'population': self.population,
-      # FIXME: Don't know what it does. Previous nmmo entities all returned 1
-      # 'self': self.self.val,
     }
 
     return data
 
   def update(self, realm, actions):
     '''Update occurs after actions, e.g. does not include history'''
     if self.history.damage == 0:
@@ -286,26 +283,27 @@
 
     if self.alive:
       return True
 
     # at this point, self is dead
     if source:
       source.history.player_kills += 1
+      self.realm.event_log.record(EventCode.PLAYER_KILL, source, target=self)
 
     # if self is dead, unlist its items from the market regardless of looting
     if self.config.EXCHANGE_SYSTEM_ENABLED:
       for item in list(self.inventory.items):
         self.realm.exchange.unlist_item(item)
 
     # if self is dead but no one can loot, destroy its items
     if source is None or not source.is_player: # nobody or npcs cannot loot
       if self.config.ITEM_SYSTEM_ENABLED:
         for item in list(self.inventory.items):
           item.destroy()
-      return True
+      return False
 
     # now, source can loot the dead self
     return False
 
   # pylint: disable=unused-argument
   def apply_damage(self, dmg, style):
     self.history.damage_inflicted += dmg
@@ -334,9 +332,13 @@
     melee = self.skills.melee.level.val
     ranged = self.skills.range.level.val
     mage = self.skills.mage.level.val
 
     return int(max(melee, ranged, mage))
 
   @property
-  def population(self):
-    return self.population_id.val
+  def in_combat(self) -> bool:
+    # NOTE: the initial latest_combat_tick is 0, and valid values are greater than 0
+    if not self.config.COMBAT_SYSTEM_ENABLED or self.latest_combat_tick.val == 0:
+      return False
+
+    return (self.realm.tick - self.latest_combat_tick.val) < self.config.COMBAT_STATUS_DURATION
```

### Comparing `nmmo-1.7.0.1/nmmo/entity/entity_manager.py` & `nmmo-2.0.0/nmmo/entity/entity_manager.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from collections.abc import Mapping
-from typing import Dict, Set
+from typing import Dict
 
 import numpy as np
 from ordered_set import OrderedSet
 
 from nmmo.entity.entity import Entity
 from nmmo.entity.npc import NPC
 from nmmo.entity.player import Player
-from nmmo.lib import colors, spawn
+from nmmo.lib import spawn
 from nmmo.systems import combat
 
 
 class EntityGroup(Mapping):
   def __init__(self, realm):
     self.datastore = realm.datastore
     self.realm = realm
     self.config = realm.config
 
-    self.entities: Dict[int, Entity]  = {}
-    self.dead: Set(int) = {}
+    self.entities: Dict[int, Entity] = {}
+    self.dead_this_tick: Dict[int, Entity] = {}
 
   def __len__(self):
     return len(self.entities)
 
   def __contains__(self, e):
     return e in self.entities
 
@@ -33,46 +33,57 @@
     yield from self.entities
 
   def items(self):
     return self.entities.items()
 
   @property
   def corporeal(self):
-    return {**self.entities, **self.dead}
+    return {**self.entities, **self.dead_this_tick}
 
   @property
   def packet(self):
     return {k: v.packet() for k, v in self.corporeal.items()}
 
   def reset(self):
     for ent in self.entities.values():
+      # destroy the items
+      if self.config.ITEM_SYSTEM_ENABLED:
+        for item in list(ent.inventory.items):
+          item.destroy()
       ent.datastore_record.delete()
 
     self.entities = {}
-    self.dead     = {}
+    self.dead_this_tick = {}
 
   def spawn(self, entity):
     pos, ent_id = entity.pos, entity.id.val
     self.realm.map.tiles[pos].add_entity(entity)
     self.entities[ent_id] = entity
 
   def cull(self):
-    self.dead = {}
+    self.dead_this_tick = {}
     for ent_id in list(self.entities):
       player = self.entities[ent_id]
       if not player.alive:
         r, c  = player.pos
         ent_id = player.ent_id
-        self.dead[ent_id] = player
+        self.dead_this_tick[ent_id] = player
 
         self.realm.map.tiles[r, c].remove_entity(ent_id)
+
+        # destroy the remaining items (of starved/dehydrated players)
+        #    of the agents who don't go through receive_damage()
+        if self.config.ITEM_SYSTEM_ENABLED:
+          for item in list(player.inventory.items):
+            item.destroy()
+
         self.entities[ent_id].datastore_record.delete()
         del self.entities[ent_id]
 
-    return self.dead
+    return self.dead_this_tick
 
   def update(self, actions):
     for entity in self.entities.values():
       entity.update(self.realm, actions)
 
 
 class NPCManager(EntityGroup):
@@ -113,45 +124,48 @@
     if self.spawn_dangers:
       self.spawn_dangers.pop()
 
   def cull(self):
     for entity in super().cull().values():
       self.spawn_dangers.append(entity.spawn_danger)
 
+    # refill npcs to target config.NPC_N, within config.NPC_SPAWN_ATTEMPTS
+    self.spawn()
+
   def actions(self, realm):
     actions = {}
     for idx, entity in self.entities.items():
       actions[idx] = entity.decide(realm)
     return actions
 
 class PlayerManager(EntityGroup):
   def __init__(self, realm):
     super().__init__(realm)
-    self.palette = colors.Palette()
-    self.loader  = self.realm.config.PLAYER_LOADER
-    self.agents = None
+    self.loader_class = self.realm.config.PLAYER_LOADER
+    self._agent_loader: spawn.SequentialLoader = None
     self.spawned = None
 
   def reset(self):
     super().reset()
-    self.agents  = self.loader(self.config)
+    self._agent_loader = self.loader_class(self.config)
     self.spawned = OrderedSet()
 
   def spawn_individual(self, r, c, idx):
-    pop, agent = next(self.agents)
+    agent = next(self._agent_loader)
     agent      = agent(self.config, idx)
-    player     = Player(self.realm, (r, c), agent, self.palette.color(pop), pop)
+    player     = Player(self.realm, (r, c), agent)
     super().spawn(player)
+    self.spawned.add(idx)
 
   def spawn(self):
     idx = 0
-    for r, c in spawn.spawn_concurrent(self.config):
+    while idx < self.config.PLAYER_N:
       idx += 1
+      r, c = self._agent_loader.get_spawn_position(idx)
 
       if idx in self.entities:
         continue
 
       if idx in self.spawned:
         continue
 
-      self.spawned.add(idx)
       self.spawn_individual(r, c, idx)
```

### Comparing `nmmo-1.7.0.1/nmmo/entity/npc.py` & `nmmo-2.0.0/nmmo/entity/npc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 
 import random
 
 from nmmo.entity import entity
-from nmmo.io import action as Action
-from nmmo.lib.colors import Neon
+from nmmo.core import action as Action
 from nmmo.systems import combat, droptable
 from nmmo.systems.ai import policy
 from nmmo.systems import item as Item
 from nmmo.systems import skill
 from nmmo.systems.inventory import EquipmentSlot
 
 
@@ -42,23 +41,25 @@
     packet['melee_defense'] = self.melee_defense
     packet['range_defense'] = self.range_defense
     packet['mage_defense']  = self.mage_defense
 
     return packet
 
 
+# pylint: disable=no-member
 class NPC(entity.Entity):
-  def __init__(self, realm, pos, iden, name, color, pop):
-    super().__init__(realm, pos, iden, name, color, pop)
+  def __init__(self, realm, pos, iden, name, npc_type):
+    super().__init__(realm, pos, iden, name)
     self.skills = skill.Combat(realm, self)
     self.realm = realm
     self.last_action = None
     self.droptable = None
     self.spawn_danger = None
     self.equipment = None
+    self.npc_type.update(npc_type)
 
   def update(self, realm, actions):
     super().update(realm, actions)
 
     if not self.alive:
       return
 
@@ -72,27 +73,30 @@
 
     # run the next lines if the npc is killed
     # source receive gold & items in the droptable
     # pylint: disable=no-member
     source.gold.increment(self.gold.val)
     self.gold.update(0)
 
-    # TODO(kywch): make source receive the highest-level items first
-    #   because source cannot take it if the inventory is full
-    #   Also, destroy the remaining items if the source cannot take those
     for item in self.droptable.roll(self.realm, self.attack_level):
-      if source.inventory.space:
+      if source.is_player and source.inventory.space:
         source.inventory.receive(item)
+      else:
+        item.destroy()
 
     return False
 
   @staticmethod
   def spawn(realm, pos, iden):
     config = realm.config
 
+    # check the position
+    if realm.map.tiles[pos].impassible:
+      return None
+
     # Select AI Policy
     danger = combat.danger(config, pos)
     if danger >= config.NPC_SPAWN_AGGRESSIVE:
       ent = Aggressive(realm, pos, iden)
     elif danger >= config.NPC_SPAWN_NEUTRAL:
       ent = PassiveAggressive(realm, pos, iden)
     elif danger >= config.NPC_SPAWN_PASSIVE:
@@ -138,44 +142,45 @@
 
       ent.equipment = Equipment(ilvl, offense, offense, offense, defense, defense, defense)
 
       armor =  [Item.Hat, Item.Top, Item.Bottom]
       ent.droptable.add(random.choice(armor))
 
     if config.PROFESSION_SYSTEM_ENABLED:
-      tools =  [Item.Rod, Item.Gloves, Item.Pickaxe, Item.Chisel, Item.Arcane]
+      tools =  [Item.Rod, Item.Gloves, Item.Pickaxe, Item.Axe, Item.Chisel]
       ent.droptable.add(random.choice(tools))
 
     return ent
 
   def packet(self):
     data = super().packet()
 
     data['skills']   = self.skills.packet()
-    data['resource'] = {'health': self.resources.health.val}
+    data['resource'] = { 'health': {
+      'val': self.resources.health.val, 'max': self.config.PLAYER_BASE_HEALTH } }
 
     return data
 
   @property
   def is_npc(self) -> bool:
     return True
 
 class Passive(NPC):
   def __init__(self, realm, pos, iden):
-    super().__init__(realm, pos, iden, 'Passive', Neon.GREEN, -1)
+    super().__init__(realm, pos, iden, 'Passive', 1)
 
   def decide(self, realm):
     return policy.passive(realm, self)
 
 class PassiveAggressive(NPC):
   def __init__(self, realm, pos, iden):
-    super().__init__(realm, pos, iden, 'Neutral', Neon.ORANGE, -2)
+    super().__init__(realm, pos, iden, 'Neutral', 2)
 
   def decide(self, realm):
     return policy.neutral(realm, self)
 
 class Aggressive(NPC):
   def __init__(self, realm, pos, iden):
-    super().__init__(realm, pos, iden, 'Hostile', Neon.RED, -3)
+    super().__init__(realm, pos, iden, 'Hostile', 3)
 
   def decide(self, realm):
     return policy.hostile(realm, self)
```

### Comparing `nmmo-1.7.0.1/nmmo/entity/player.py` & `nmmo-2.0.0/nmmo/entity/player.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,47 +1,46 @@
+import numpy as np
+
 from nmmo.systems.skill import Skills
-from nmmo.systems.achievement import Diary
 from nmmo.entity import entity
 
 # pylint: disable=no-member
 class Player(entity.Entity):
-  def __init__(self, realm, pos, agent, color, pop):
-    super().__init__(realm, pos, agent.iden, agent.policy, color, pop)
+  def __init__(self, realm, pos, agent):
+    super().__init__(realm, pos, agent.iden, agent.policy)
 
     self.agent    = agent
-    self.pop      = pop
     self.immortal = realm.config.IMMORTAL
 
     # Scripted hooks
     self.target = None
     self.vision = 7
 
     # Logs
     self.buys                     = 0
     self.sells                    = 0
     self.ration_consumed          = 0
     self.poultice_consumed        = 0
     self.ration_level_consumed    = 0
     self.poultice_level_consumed  = 0
 
-    # Submodules
+    # initialize skills with the base level
     self.skills = Skills(realm, self)
+    if realm.config.PROGRESSION_SYSTEM_ENABLED:
+      for skill in self.skills.skills:
+        skill.level.update(realm.config.PROGRESSION_BASE_LEVEL)
 
-    # Gold: initialize with 1 gold, like the old nmmo
+    # Gold: initialize with 1 gold (EXCHANGE_BASE_GOLD).
+    # If the base amount is more than 1, alss check the npc's init gold.
     if realm.config.EXCHANGE_SYSTEM_ENABLED:
-      self.gold.update(1)
-
-    self.diary  = None
-    tasks = realm.config.TASKS
-    if tasks:
-      self.diary = Diary(self, tasks)
+      self.gold.update(realm.config.EXCHANGE_BASE_GOLD)
 
   @property
   def serial(self):
-    return self.population_id, self.ent_id
+    return self.ent_id
 
   @property
   def is_player(self) -> bool:
     return True
 
   @property
   def level(self) -> int:
@@ -63,40 +62,44 @@
     if super().receive_damage(source, dmg):
       return True
 
     if not self.config.ITEM_SYSTEM_ENABLED:
       return False
 
     # starting from here, source receive gold & inventory items
-    if self.config.EXCHANGE_SYSTEM_ENABLED:
+    if self.config.EXCHANGE_SYSTEM_ENABLED and source is not None:
       source.gold.increment(self.gold.val)
       self.gold.update(0)
 
-    # TODO(kywch): make source receive the highest-level items first
+    # TODO: make source receive the highest-level items first
     #   because source cannot take it if the inventory is full
-    #   Also, destroy the remaining items if the source cannot take those
-    for item in list(self.inventory.items):
+    item_list = list(self.inventory.items)
+    np.random.shuffle(item_list)
+    for item in item_list:
       self.inventory.remove(item)
 
-      # if source doesn't have space, inventory.receive() destroys the item
-      source.inventory.receive(item)
+      # if source is None or NPC, destroy the item
+      if source.is_player:
+        # if source doesn't have space, inventory.receive() destroys the item
+        source.inventory.receive(item)
+      else:
+        item.destroy()
 
     # CHECK ME: this is an empty function. do we still need this?
     self.skills.receive_damage(dmg)
     return False
 
   @property
   def equipment(self):
     return self.inventory.equipment
 
   def packet(self):
     data = super().packet()
 
     data['entID']     = self.ent_id
-    data['annID']     = self.population
 
     data['resource']  = self.resources.packet()
     data['skills']    = self.skills.packet()
     data['inventory'] = self.inventory.packet()
 
     return data
 
@@ -128,10 +131,7 @@
         self.receive_damage(None, dmg)
 
     if not self.alive:
       return
 
     self.resources.update()
     self.skills.update()
-
-    if self.diary:
-      self.diary.update(realm)
```

### Comparing `nmmo-1.7.0.1/nmmo/io/action.py` & `nmmo-2.0.0/nmmo/core/action.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # CHECK ME: Should these be fixed as well?
 # pylint: disable=no-method-argument,unused-argument,no-self-argument,no-member
 
 from enum import Enum, auto
 from ordered_set import OrderedSet
+import numpy as np
 
 from nmmo.lib import utils
 from nmmo.lib.utils import staticproperty
 from nmmo.systems.item import Item, Stack
+from nmmo.lib.log import EventCode
 
 class NodeType(Enum):
   #Tree edges
   STATIC = auto()    #Traverses all edges without decisions
   SELECTION = auto() #Picks an edge to follow
 
   #Executable actions
@@ -111,40 +113,46 @@
   priority = 60
   nodeType = NodeType.SELECTION
   def call(realm, entity, direction):
     if direction is None:
       return
 
     assert entity.alive, "Dead entity cannot act"
+    assert realm.map.is_valid_pos(*entity.pos), "Invalid entity position"
 
     r, c  = entity.pos
     ent_id = entity.ent_id
     entity.history.last_pos = (r, c)
     r_delta, c_delta = direction.delta
     r_new, c_new = r+r_delta, c+c_delta
 
-    # CHECK ME: before this agents were allowed to jump into lava and die
-    #   however, when config.IMMORTAL = True was set, lava-jumping agents
-    #   did not die and made all the way to the map edge, causing errors
-    #   e.g., systems/skill.py, line 135: realm.map.tiles[r, c+1] index error
-    # How do we want to handle this?
-    if realm.map.tiles[r_new, c_new].impassible:
+    if not realm.map.is_valid_pos(r_new, c_new) or \
+       realm.map.tiles[r_new, c_new].impassible:
       return
 
     if entity.status.freeze > 0:
       return
 
     entity.row.update(r_new)
     entity.col.update(c_new)
 
     realm.map.tiles[r, c].remove_entity(ent_id)
     realm.map.tiles[r_new, c_new].add_entity(entity)
 
-    # CHECK ME: material.Impassible includes lava, so this line is not reachable
-    if realm.map.tiles[r_new, c_new].lava:
+    # exploration record keeping. moved from entity.py, History.update()
+    dist_from_spawn = utils.linf(entity.spawn_pos, (r_new, c_new))
+    if dist_from_spawn > entity.history.exploration:
+      entity.history.exploration = dist_from_spawn
+      if entity.is_player:
+        realm.event_log.record(EventCode.GO_FARTHEST, entity,
+                               distance=dist_from_spawn)
+
+    # CHECK ME: material.Impassible includes void, so this line is not reachable
+    #   Does this belong to Entity/Player.update()?
+    if realm.map.tiles[r_new, c_new].void:
       entity.receive_damage(None, entity.resources.health.val)
 
   @staticproperty
   def edges():
     return [Direction]
 
   @staticproperty
@@ -155,25 +163,25 @@
     return True
 
 class Direction(Node):
   argType = Fixed
 
   @staticproperty
   def edges():
-    return [North, South, East, West]
+    return [North, South, East, West, Stay]
 
   def args(stim, entity, config):
     return Direction.edges
 
   def deserialize(realm, entity, index):
     return deserialize_fixed_arg(Direction, index)
 
 # a quick helper function
 def deserialize_fixed_arg(arg, index):
-  if isinstance(index, int):
+  if isinstance(index, (int, np.int64)):
     if index < 0:
       return None # so that the action will be discarded
     val = min(index-1, len(arg.edges)-1)
     return arg.edges[val]
 
   # if index is not int, it's probably already deserialized
   if index not in arg.edges:
@@ -188,14 +196,17 @@
 
 class East(Node):
   delta = (0, 1)
 
 class West(Node):
   delta = (0, -1)
 
+class Stay(Node):
+  delta = (0, 0)
+
 
 class Attack(Node):
   priority = 50
   nodeType = NodeType.SELECTION
   @staticproperty
   def n():
     return 3
@@ -248,19 +259,14 @@
       target.history.time_alive < immunity < entity.history.time_alive.val:
       return None
 
     #Check if self targeted
     if entity.ent_id == target.ent_id:
       return None
 
-    #ADDED: POPULATION IMMUNITY
-    if not config.COMBAT_FRIENDLY_FIRE and entity.is_player \
-       and entity.population_id.val == target.population_id.val:
-      return None
-
     #Can't attack out of range
     if utils.linf(entity.pos, target.pos) > style.attack_range(config):
       return None
 
     #Execute attack
     entity.history.attack = {}
     entity.history.attack['target'] = target.ent_id
@@ -270,14 +276,19 @@
 
     from nmmo.systems import combat
     dmg = combat.attack(realm, entity, target, style.skill)
 
     if style.freeze and dmg > 0:
       target.status.freeze.update(config.COMBAT_FREEZE_TIME)
 
+    # record the combat tick for both entities
+    # players and npcs both have latest_combat_tick in EntityState
+    for ent in [entity, target]:
+      ent.latest_combat_tick.update(realm.tick + 1) # because the tick is about to increment
+
     return dmg
 
 class Style(Node):
   argType = Fixed
   @staticproperty
   def edges():
     return [Melee, Range, Mage]
@@ -364,27 +375,30 @@
   def edges():
     return [InventoryItem]
 
   def enabled(config):
     return config.ITEM_SYSTEM_ENABLED
 
   def call(realm, entity, item):
-    if item is None:
+    if item is None or item.owner_id.val != entity.ent_id:
       return
 
     assert entity.alive, "Dead entity cannot act"
     assert entity.is_player, "Npcs cannot use an item"
     assert item.quantity.val > 0, "Item quantity cannot be 0" # indicates item leak
 
     if not realm.config.ITEM_SYSTEM_ENABLED:
       return
 
     if item not in entity.inventory:
       return
 
+    if entity.in_combat: # player cannot use item during combat
+      return
+
     # cannot use listed items or items that have higher level
     if item.listed_price.val > 0 or item.level_gt(entity):
       return
 
     item.use(entity)
 
 class Destroy(Node):
@@ -394,15 +408,15 @@
   def edges():
     return [InventoryItem]
 
   def enabled(config):
     return config.ITEM_SYSTEM_ENABLED
 
   def call(realm, entity, item):
-    if item is None:
+    if item is None or item.owner_id.val != entity.ent_id:
       return
 
     assert entity.alive, "Dead entity cannot act"
     assert entity.is_player, "Npcs cannot destroy an item"
     assert item.quantity.val > 0, "Item quantity cannot be 0" # indicates item leak
 
     if not realm.config.ITEM_SYSTEM_ENABLED:
@@ -410,30 +424,33 @@
 
     if item not in entity.inventory:
       return
 
     if item.equipped.val: # cannot destroy equipped item
       return
 
-    # inventory.remove() also unlists the item, if it has been listed
-    entity.inventory.remove(item)
+    if entity.in_combat: # player cannot destroy item during combat
+      return
+
     item.destroy()
 
+    realm.event_log.record(EventCode.DESTROY_ITEM, entity)
+
 class Give(Node):
   priority = 30
 
   @staticproperty
   def edges():
     return [InventoryItem, Target]
 
   def enabled(config):
     return config.ITEM_SYSTEM_ENABLED
 
   def call(realm, entity, item, target):
-    if item is None or target is None:
+    if item is None or item.owner_id.val != entity.ent_id or target is None:
       return
 
     assert entity.alive, "Dead entity cannot act"
     assert entity.is_player, "Npcs cannot give an item"
     assert item.quantity.val > 0, "Item quantity cannot be 0" # indicates item leak
 
     config = realm.config
@@ -446,32 +463,37 @@
     if item not in entity.inventory:
       return
 
     # cannot give the equipped or listed item
     if item.equipped.val or item.listed_price.val:
       return
 
-    if not (config.ITEM_GIVE_TO_FRIENDLY and
-            entity.population_id == target.population_id and        # the same team
+    if entity.in_combat: # player cannot give item during combat
+      return
+
+    if not (config.ITEM_ALLOW_GIFT and
             entity.ent_id != target.ent_id and                      # but not self
-            utils.linf(entity.pos, target.pos) == 0):               # the same tile
+            target.is_player and
+            entity.pos == target.pos):               # the same tile
       return
 
     if not target.inventory.space:
       # receiver inventory is full - see if it has an ammo stack with the same sig
       if isinstance(item, Stack):
         if not target.inventory.has_stack(item.signature):
           # no ammo stack with the same signature, so cannot give
           return
       else: # no space, and item is not ammo stack, so cannot give
         return
 
     entity.inventory.remove(item)
     target.inventory.receive(item)
 
+    realm.event_log.record(EventCode.GIVE_ITEM, entity)
+
 
 class GiveGold(Node):
   priority = 30
 
   @staticproperty
   def edges():
     # CHECK ME: for now using Price to indicate the gold amount to give
@@ -490,31 +512,36 @@
     config = realm.config
     if not config.EXCHANGE_SYSTEM_ENABLED:
       return
 
     if not (target.is_player and target.alive):
       return
 
-    if not (config.ITEM_GIVE_TO_FRIENDLY and
-            entity.population_id == target.population_id and        # the same team
+    if entity.in_combat: # player cannot give gold during combat
+      return
+
+    if not (config.ITEM_ALLOW_GIFT and
             entity.ent_id != target.ent_id and                      # but not self
-            utils.linf(entity.pos, target.pos) == 0):               # the same tile
+            target.is_player and
+            entity.pos == target.pos):                              # the same tile
       return
 
     if not isinstance(amount, int):
       amount = amount.val
 
     if not (amount > 0 and entity.gold.val > 0): # no gold to give
       return
 
     amount = min(amount, entity.gold.val)
 
     entity.gold.decrement(amount)
     target.gold.increment(amount)
 
+    realm.event_log.record(EventCode.GIVE_GOLD, entity)
+
 
 class MarketItem(Node):
   argType  = None
 
   @classmethod
   def N(cls, config):
     return config.MARKET_N_OBS
@@ -541,15 +568,15 @@
   def edges():
     return [MarketItem]
 
   def enabled(config):
     return config.EXCHANGE_SYSTEM_ENABLED
 
   def call(realm, entity, item):
-    if item is None:
+    if item is None or item.owner_id.val == 0:
       return
 
     assert entity.alive, "Dead entity cannot act"
     assert entity.is_player, "Npcs cannot buy an item"
     assert item.quantity.val > 0, "Item quantity cannot be 0" # indicates item leak
     assert item.equipped.val == 0, 'Listed item must not be equipped'
 
@@ -558,14 +585,17 @@
 
     if entity.gold.val < item.listed_price.val: # not enough money
       return
 
     if entity.ent_id == item.owner_id.val: # cannot buy own item
       return
 
+    if entity.in_combat: # player cannot buy item during combat
+      return
+
     if not entity.inventory.space:
       # buyer inventory is full - see if it has an ammo stack with the same sig
       if isinstance(item, Stack):
         if not entity.inventory.has_stack(item.signature):
           # no ammo stack with the same signature, so cannot give
           return
       else: # no space, and item is not ammo stack, so cannot give
@@ -582,31 +612,30 @@
   def edges():
     return [InventoryItem, Price]
 
   def enabled(config):
     return config.EXCHANGE_SYSTEM_ENABLED
 
   def call(realm, entity, item, price):
-    if item is None or price is None:
+    if item is None or item.owner_id.val != entity.ent_id or price is None:
       return
 
     assert entity.alive, "Dead entity cannot act"
     assert entity.is_player, "Npcs cannot sell an item"
     assert item.quantity.val > 0, "Item quantity cannot be 0" # indicates item leak
 
     if not realm.config.EXCHANGE_SYSTEM_ENABLED:
       return
 
-    # TODO(kywch): Find a better way to check this
-    # Should only occur when item is used on same tick
-    # Otherwise should not be possible
-    #   >> Actions on the same item should be checked at env._validate_actions
     if item not in entity.inventory:
       return
 
+    if entity.in_combat: # player cannot sell item during combat
+      return
+
     # cannot sell the equipped or listed item
     if item.equipped.val or item.listed_price.val:
       return
 
     if not isinstance(price, int):
       price = price.val
```

### Comparing `nmmo-1.7.0.1/nmmo/lib/colors.py` & `nmmo-2.0.0/nmmo/lib/colors.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/lib/material.py` & `nmmo-2.0.0/nmmo/lib/material.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 from nmmo.systems import item, droptable
 
 class Material:
   capacity = 0
   tool = None
   table = None
   index = None
+  respawn = 0
 
   def __init__(self, config):
     pass
 
   def __eq__(self, mtl):
     return self.index == mtl.index
 
   def __equals__(self, mtl):
     return self == mtl
 
   def harvest(self):
     return self.__class__.table
 
-class Lava(Material):
-  tex   = 'lava'
+class Void(Material):
+  tex   = 'void'
   index = 0
 
 class Water(Material):
   tex   = 'water'
   index = 1
 
   table = droptable.Empty()
@@ -37,25 +38,25 @@
   tex   = 'grass'
   index = 2
 
 class Scrub(Material):
   tex   = 'scrub'
   index = 3
 
-class Forest(Material):
-  tex   = 'forest'
+class Foilage(Material):
+  tex   = 'foilage'
   index = 4
 
   deplete = Scrub
   table = droptable.Empty()
 
   def __init__(self, config):
     if config.RESOURCE_SYSTEM_ENABLED:
-      self.capacity = config.RESOURCE_FOREST_CAPACITY
-      self.respawn  = config.RESOURCE_FOREST_RESPAWN
+      self.capacity = config.RESOURCE_FOILAGE_CAPACITY
+      self.respawn  = config.RESOURCE_FOILAGE_RESPAWN
 
 class Stone(Material):
   tex   = 'stone'
   index = 5
 
 class Slag(Material):
   tex   = 'slag'
@@ -68,65 +69,65 @@
   deplete = Slag
   tool    = item.Pickaxe
 
   def __init__(self, config):
     cls = self.__class__
     if cls.table is None:
       cls.table = droptable.Standard()
-      cls.table.add(item.Scrap)
+      cls.table.add(item.Whetstone)
 
       if config.EQUIPMENT_SYSTEM_ENABLED:
         cls.table.add(item.Wand, prob=config.WEAPON_DROP_PROB)
 
     if config.PROFESSION_SYSTEM_ENABLED:
       self.capacity = config.PROFESSION_ORE_CAPACITY
-      self.respawn  = config.PROFESSION_ORE_CAPACITY
+      self.respawn  = config.PROFESSION_ORE_RESPAWN
 
   tool    = item.Pickaxe
   deplete = Slag
 
 class Stump(Material):
   tex   = 'stump'
   index = 8
 
 class Tree(Material):
   tex   = 'tree'
   index = 9
 
   deplete = Stump
-  tool    = item.Chisel
+  tool    = item.Axe
 
   def __init__(self, config):
     cls = self.__class__
     if cls.table is None:
       cls.table = droptable.Standard()
-      cls.table.add(item.Shaving)
+      cls.table.add(item.Arrow)
       if config.EQUIPMENT_SYSTEM_ENABLED:
-        cls.table.add(item.Sword, prob=config.WEAPON_DROP_PROB)
+        cls.table.add(item.Spear, prob=config.WEAPON_DROP_PROB)
 
     if config.PROFESSION_SYSTEM_ENABLED:
       self.capacity = config.PROFESSION_TREE_CAPACITY
       self.respawn  = config.PROFESSION_TREE_RESPAWN
 
 class Fragment(Material):
   tex   = 'fragment'
   index = 10
 
 class Crystal(Material):
   tex   = 'crystal'
   index = 11
 
   deplete = Fragment
-  tool    = item.Arcane
+  tool    = item.Chisel
 
   def __init__(self, config):
     cls = self.__class__
     if cls.table is None:
       cls.table = droptable.Standard()
-      cls.table.add(item.Shard)
+      cls.table.add(item.Runes)
       if config.EQUIPMENT_SYSTEM_ENABLED:
         cls.table.add(item.Bow, prob=config.WEAPON_DROP_PROB)
 
     if config.PROFESSION_SYSTEM_ENABLED:
       self.capacity = config.PROFESSION_CRYSTAL_CAPACITY
       self.respawn  = config.PROFESSION_CRYSTAL_RESPAWN
 
@@ -138,15 +139,15 @@
   tex   = 'herb'
   index = 13
 
   deplete = Weeds
   tool    = item.Gloves
 
   table   = droptable.Standard()
-  table.add(item.Poultice)
+  table.add(item.Potion)
 
   def __init__(self, config):
     if config.PROFESSION_SYSTEM_ENABLED:
       self.capacity = config.PROFESSION_HERB_CAPACITY
       self.respawn  = config.PROFESSION_HERB_RESPAWN
 
 class Ocean(Material):
@@ -183,22 +184,22 @@
     if isinstance(mtl, type):
       return mtl in self.materials
     return mtl in self.indices
 
 class All(metaclass=Meta):
   '''List of all materials'''
   materials = {
-    Lava, Water, Grass, Scrub, Forest,
+    Void, Water, Grass, Scrub, Foilage,
     Stone, Slag, Ore, Stump, Tree,
     Fragment, Crystal, Weeds, Herb, Ocean, Fish}
 
 class Impassible(metaclass=Meta):
   '''Materials that agents cannot walk through'''
-  materials = {Lava, Water, Stone, Ocean, Fish}
+  materials = {Void, Water, Stone, Ocean, Fish}
 
 class Habitable(metaclass=Meta):
   '''Materials that agents cannot walk on'''
-  materials = {Grass, Scrub, Forest, Ore, Slag, Tree, Stump, Crystal, Fragment, Herb, Weeds}
+  materials = {Grass, Scrub, Foilage, Ore, Slag, Tree, Stump, Crystal, Fragment, Herb, Weeds}
 
 class Harvestable(metaclass=Meta):
   '''Materials that agents can harvest'''
-  materials = {Water, Forest, Ore, Tree, Crystal, Herb, Fish}
+  materials = {Water, Foilage, Ore, Tree, Crystal, Herb, Fish}
```

### Comparing `nmmo-1.7.0.1/nmmo/lib/priorityqueue.py` & `nmmo-2.0.0/nmmo/lib/priorityqueue.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/lib/utils.py` & `nmmo-2.0.0/nmmo/lib/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,19 +42,15 @@
       yield name, attr
 
 class NameComparable(type):
   def __hash__(self):
     return hash(self.__name__)
 
   def __eq__(self, other):
-    try:
-      return self.__name__ == other.__name__
-    except:
-        print("Some sphinx bug makes this block doc calls. "
-              "You should not see this in normal NMMO usage")
+    return self.__name__ == other.__name__
 
   def __ne__(self, other):
     return self.__name__ != other.__name__
 
   def __lt__(self, other):
     return self.__name__ < other.__name__
 
@@ -72,15 +68,15 @@
 
 def seed():
   return int(np.random.randint(0, 2**32))
 
 def linf(pos1, pos2):
   # pos could be a single (r,c) or a vector of (r,c)s
   diff = np.abs(np.array(pos1) - np.array(pos2))
-  return np.max(diff, axis=len(diff.shape)-1)  
+  return np.max(diff, axis=len(diff.shape)-1)
 
 #Bounds checker
 def in_bounds(r, c, shape, border=0):
   R, C = shape
   return (
     r > border and
     c > border and
```

### Comparing `nmmo-1.7.0.1/nmmo/resource/crystal.png` & `nmmo-2.0.0/nmmo/resource/crystal.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/fish.png` & `nmmo-2.0.0/nmmo/resource/fish.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/forest.png` & `nmmo-2.0.0/nmmo/resource/foilage.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/fragment.png` & `nmmo-2.0.0/nmmo/resource/fragment.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/grass.png` & `nmmo-2.0.0/nmmo/resource/grass.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/herb.png` & `nmmo-2.0.0/nmmo/resource/herb.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/lava.png` & `nmmo-2.0.0/nmmo/resource/void.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/ocean.png` & `nmmo-2.0.0/nmmo/resource/ocean.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/ore.png` & `nmmo-2.0.0/nmmo/resource/ore.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/scrub.png` & `nmmo-2.0.0/nmmo/resource/scrub.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/slag.png` & `nmmo-2.0.0/nmmo/resource/slag.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/spawn.png` & `nmmo-2.0.0/nmmo/resource/spawn.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/stone.png` & `nmmo-2.0.0/nmmo/resource/stone.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/stump.png` & `nmmo-2.0.0/nmmo/resource/stump.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/tree.png` & `nmmo-2.0.0/nmmo/resource/tree.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/water.png` & `nmmo-2.0.0/nmmo/resource/water.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/resource/weeds.png` & `nmmo-2.0.0/nmmo/resource/weeds.png`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/systems/ai/behavior.py` & `nmmo-2.0.0/nmmo/systems/ai/behavior.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/systems/ai/move.py` & `nmmo-2.0.0/nmmo/systems/ai/move.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # pylint: disable=R0401
 
 import random
 
-from nmmo.io import action
+from nmmo.core import action
 from nmmo.systems.ai import utils
 
 
 def random_direction():
   return random.choice(action.Direction.edges)
 
 def random_safe(tiles, ent):
   r, c  = ent.pos
   cands = []
-  if not tiles[r-1, c].lava:
+  if not tiles[r-1, c].void:
     cands.append(action.North)
-  if not tiles[r+1, c].lava:
+  if not tiles[r+1, c].void:
     cands.append(action.South)
-  if not tiles[r, c-1].lava:
+  if not tiles[r, c-1].void:
     cands.append(action.West)
-  if not tiles[r, c+1].lava:
+  if not tiles[r, c+1].void:
     cands.append(action.East)
 
   return random.choice(cands)
 
 def habitable(tiles, ent):
   r, c  = ent.pos
   cands = []
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/ai/policy.py` & `nmmo-2.0.0/nmmo/systems/ai/policy.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/nmmo/systems/ai/utils.py` & `nmmo-2.0.0/nmmo/systems/ai/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    if lInfty(ent.pos, targ.pos) > rng:
       return False
    return True
 
 
 def validResource(ent, tile, rng):
    return tile is not None and tile.state.tex in (
-      'forest', 'water') and distance(ent, tile) <= rng
+      'foilage', 'water') and distance(ent, tile) <= rng
 
 
 def directionTowards(ent, targ):
    sr, sc = ent.pos
    tr, tc = targ.pos
 
    if abs(sc - tc) > abs(sr - tr):
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/combat.py` & `nmmo-2.0.0/nmmo/systems/combat.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #Various utilities for managing combat, including hit/damage
 
 import numpy as np
 
 from nmmo.systems import skill as Skill
+from nmmo.lib.log import EventCode
 
 def level(skills):
   return max(e.level.val for e in skills.skills)
 
 def damage_multiplier(config, skill, targ):
   skills = [targ.skills.melee, targ.skills.range, targ.skills.mage]
   exp    = [s.exp for s in skills]
@@ -91,16 +92,22 @@
   offense = skill_offense + equipment_offense
   defense = skill_defense + equipment_defense
   damage  = config.COMBAT_DAMAGE_FORMULA(offense, defense, multiplier)
   #damage  = multiplier * (offense - defense)
   damage  = max(int(damage), 0)
 
   if player.is_player:
-    equipment_level_offense = player.equipment.total(lambda e: e.level)
-    equipment_level_defense = target.equipment.total(lambda e: e.level)
+    equipment_level_offense = 0
+    equipment_level_defense = 0
+    if config.EQUIPMENT_SYSTEM_ENABLED:
+      equipment_level_offense = player.equipment.total(lambda e: e.level)
+      equipment_level_defense = target.equipment.total(lambda e: e.level)
+
+    realm.event_log.record(EventCode.SCORE_HIT, player,
+                           combat_style=skill_type, damage=damage)
 
     realm.log_milestone(f'Damage_{skill_name}', damage,
                         f'COMBAT: Inflicted {damage} {skill_name} damage ' +
                         f'(attack equip lvl {equipment_level_offense} vs ' +
                         f'defense equip lvl {equipment_level_defense})',
                         tags={"player_id": player.ent_id})
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/droptable.py` & `nmmo-2.0.0/nmmo/systems/droptable.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 import numpy as np
 
 class Fixed():
-  def __init__(self, item, amount=1):
+  def __init__(self, item):
     self.item = item
-    self.amount = amount
 
   def roll(self, realm, level):
-    return [self.item(realm, level, amount=self.amount)]
+    return [self.item(realm, level)]
 
 class Drop:
-  def __init__(self, item, amount, prob):
+  def __init__(self, item, prob):
     self.item = item
-    self.amount = amount
     self.prob = prob
 
   def roll(self, realm, level):
     if np.random.rand() < self.prob:
-      return self.item(realm, level, quantity=self.amount)
+      return self.item(realm, level)
 
     return None
 
 class Standard:
   def __init__(self):
     self.drops = []
 
-  def add(self, item, quant=1, prob=1.0):
-    self.drops += [Drop(item, quant, prob)]
+  def add(self, item, prob=1.0):
+    self.drops += [Drop(item, prob)]
 
   def roll(self, realm, level):
     ret = []
     for e in self.drops:
       drop = e.roll(realm, level)
       if drop is not None:
         ret += [drop]
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/exchange.py` & `nmmo-2.0.0/nmmo/systems/exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import annotations
 from collections import deque
 import math
 
 from typing import Dict
 
 from nmmo.systems.item import Item, Stack
+from nmmo.lib.log import EventCode
 
 """
 The Exchange class is a simulation of an in-game item exchange.
 It has several methods that allow players to list items for sale,
 buy items, and remove expired listings.
 
 The _list_item() method is used to add a new item to the
@@ -95,14 +96,16 @@
     assert item.quantity.val > 0, f'{item} for sale has quantity {item.quantity.val}'
     assert item.listed_price.val == 0, 'Item is already listed'
     assert item.equipped.val == 0, 'Item has been equiped so cannot be listed'
     assert price > 0, 'Price must be larger than 0'
 
     self._list_item(item, seller, price, tick)
 
+    self._realm.event_log.record(EventCode.LIST_ITEM, seller, item=item, price=price)
+
     self._realm.log_milestone(f'Sell_{item.__class__.__name__}', item.level.val,
       f'EXCHANGE: Offered level {item.level.val} {item.__class__.__name__} for {price} gold',
       tags={"player_id": seller.ent_id})
 
   def buy(self, buyer, item: Item):
     assert item.quantity.val > 0, f'{item} purchase has quantity {item.quantity.val}'
     assert item.equipped.val == 0, 'Listed item must not be equipped'
@@ -126,17 +129,19 @@
 
     self.unlist_item(item)
     listing.seller.inventory.remove(item)
     buyer.inventory.receive(item)
     buyer.gold.decrement(price)
     listing.seller.gold.increment(price)
 
-    # TODO(kywch): fix logs
+    # TODO(kywch): tidy up the logs - milestone, event, etc ...
     #self._realm.log_milestone(f'Buy_{item.__name__}', item.level.val)
     #self._realm.log_milestone('Transaction_Amount', item.listed_price.val)
+    self._realm.event_log.record(EventCode.BUY_ITEM, buyer, item=item, price=price)
+    self._realm.event_log.record(EventCode.EARN_GOLD, listing.seller, amount=price)
 
   @property
   def packet(self):
     packet = {}
     for listing in self._item_listings.values():
       item = listing.item
       key = f'{item.__class__.__name__}_{item.level.val}'
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/inventory.py` & `nmmo-2.0.0/nmmo/systems/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -93,19 +93,18 @@
   def __init__(self, realm, entity):
     config           = realm.config
     self.realm       = realm
     self.entity      = entity
     self.config      = config
 
     self.equipment   = Equipment()
+    self.capacity = 0
 
-    if not config.ITEM_SYSTEM_ENABLED:
-      return
-
-    self.capacity         = config.ITEM_INVENTORY_CAPACITY
+    if config.ITEM_SYSTEM_ENABLED and entity.is_player:
+      self.capacity         = config.ITEM_INVENTORY_CAPACITY
 
     self._item_stacks: Dict[Tuple, Item.Stack] = {}
     self.items: OrderedSet[Item.Item] = OrderedSet([])
 
   @property
   def space(self):
     return self.capacity - len(self.items)
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/item.py` & `nmmo-2.0.0/nmmo/systems/item.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from __future__ import annotations
-from abc import ABC
-import math
 
+import math
+from abc import ABC
 from types import SimpleNamespace
 from typing import Dict
 
-from nmmo.lib.colors import Tier
 from nmmo.datastore.serialized import SerializedState
+from nmmo.lib.colors import Tier
+from nmmo.lib.log import EventCode
 
 # pylint: disable=no-member
 ItemState = SerializedState.subclass("Item", [
   "id",
   "type_id",
   "owner_id",
 
@@ -30,15 +31,15 @@
   # Market
   "listed_price",
 ])
 
 # TODO: These limits should be defined in the config.
 ItemState.Limits = lambda config: {
   "id": (0, math.inf),
-  "type_id": (0, config.ITEM_N + 1),
+  "type_id": (0, (config.ITEM_N + 1) if config.ITEM_SYSTEM_ENABLED else 0),
   "owner_id": (-math.inf, math.inf),
   "level": (0, 99),
   "capacity": (0, 99),
   "quantity": (0, math.inf), # NOTE: Ammunitions can be stacked infinitely
   "melee_attack": (0, 100),
   "range_attack": (0, 100),
   "mage_attack": (0, 100),
@@ -76,42 +77,47 @@
       Item._item_type_id_to_class[item_type.ITEM_TYPE_ID] = item_type
 
   @staticmethod
   def item_class(type_id: int):
     return Item._item_type_id_to_class[type_id]
 
   def __init__(self, realm, level,
-              capacity=0, quantity=1,
+              capacity=0,
               melee_attack=0, range_attack=0, mage_attack=0,
               melee_defense=0, range_defense=0, mage_defense=0,
               health_restore=0, resource_restore=0):
 
     super().__init__(realm.datastore, ItemState.Limits(realm.config))
     self.realm = realm
     self.config = realm.config
 
     Item.register(self.__class__)
 
     self.id.update(self.datastore_record.id)
     self.type_id.update(self.ITEM_TYPE_ID)
     self.level.update(level)
     self.capacity.update(capacity)
-    self.quantity.update(quantity)
+    # every item instance is created individually, i.e., quantity=1
+    self.quantity.update(1)
     self.melee_attack.update(melee_attack)
     self.range_attack.update(range_attack)
     self.mage_attack.update(mage_attack)
     self.melee_defense.update(melee_defense)
     self.range_defense.update(range_defense)
     self.mage_defense.update(mage_defense)
     self.health_restore.update(health_restore)
     self.resource_restore.update(resource_restore)
     realm.items[self.id.val] = self
 
   def destroy(self):
-    del self.realm.items[self.id.val]
+    # NOTE: we may want to track the item lifecycle and
+    #   and see how many high-level items are wasted
+    if self.owner_id.val in self.realm.players:
+      self.realm.players[self.owner_id.val].inventory.remove(self)
+    self.realm.items.pop(self.id.val, None)
     self.datastore_record.delete()
 
   @property
   def packet(self):
     return {'item':             self.__class__.__name__,
             'level':            self.level.val,
             'capacity':         self.capacity.val,
@@ -123,15 +129,15 @@
             'range_defense':    self.range_defense.val,
             'mage_defense':     self.mage_defense.val,
             'health_restore':   self.health_restore.val,
             'resource_restore': self.resource_restore.val,
             }
 
   def _level(self, entity):
-    # this is for armors, ration, and poultice
+    # this is for armors, ration, and potion
     # weapons and tools must override this with specific skills
     return entity.level
 
   def level_gt(self, entity):
     return self.level.val > self._level(entity)
 
   def use(self, entity) -> bool:
@@ -200,15 +206,15 @@
 
     if self.equipped.val:
       self.unequip(self._slot(entity))
     else:
       # always empty the slot first
       self._slot(entity).unequip()
       self.equip(entity, self._slot(entity))
-
+      self.realm.event_log.record(EventCode.EQUIP_ITEM, entity, item=self)
 
 class Armor(Equipment, ABC):
   def __init__(self, realm, level, **kwargs):
     defense = realm.config.EQUIPMENT_ARMOR_BASE_DEFENSE + \
               level*realm.config.EQUIPMENT_ARMOR_LEVEL_DEFENSE
     super().__init__(realm, level,
                      melee_defense=defense,
@@ -235,15 +241,15 @@
     self.attack = (
       realm.config.EQUIPMENT_WEAPON_BASE_DAMAGE +
       level*realm.config.EQUIPMENT_WEAPON_LEVEL_DAMAGE)
 
   def _slot(self, entity):
     return entity.inventory.equipment.held
 
-class Sword(Weapon):
+class Spear(Weapon):
   ITEM_TYPE_ID = 5
 
   def __init__(self, realm, level, **kwargs):
     super().__init__(realm, level, **kwargs)
     self.melee_attack.update(self.attack)
 
   def _level(self, entity):
@@ -288,19 +294,19 @@
   ITEM_TYPE_ID = 9
   def _level(self, entity):
     return entity.skills.herbalism.level.val
 class Pickaxe(Tool):
   ITEM_TYPE_ID = 10
   def _level(self, entity):
     return entity.skills.prospecting.level.val
-class Chisel(Tool):
+class Axe(Tool):
   ITEM_TYPE_ID = 11
   def _level(self, entity):
     return entity.skills.carving.level.val
-class Arcane(Tool):
+class Chisel(Tool):
   ITEM_TYPE_ID = 12
   def _level(self, entity):
     return entity.skills.alchemy.level.val
 
 
 class Ammunition(Equipment, Stack):
   def __init__(self, realm, level, **kwargs):
@@ -321,92 +327,98 @@
     if self.quantity.val == 0:
       entity.inventory.remove(self)
       # delete this empty item instance from the datastore
       self.destroy()
 
     return self.damage
 
-class Scrap(Ammunition):
+class Whetstone(Ammunition):
   ITEM_TYPE_ID = 13
 
   def __init__(self, realm, level, **kwargs):
     super().__init__(realm, level, **kwargs)
     self.melee_attack.update(self.attack)
 
   def _level(self, entity):
     return entity.skills.melee.level.val
 
   @property
   def damage(self):
     return self.melee_attack.val
 
-class Shaving(Ammunition):
+class Arrow(Ammunition):
   ITEM_TYPE_ID = 14
 
   def __init__(self, realm, level, **kwargs):
     super().__init__(realm, level, **kwargs)
     self.range_attack.update(self.attack)
 
   def _level(self, entity):
     return entity.skills.range.level.val
 
   @property
   def damage(self):
     return self.range_attack.val
 
-class Shard(Ammunition):
+class Runes(Ammunition):
   ITEM_TYPE_ID = 15
 
   def __init__(self, realm, level, **kwargs):
     super().__init__(realm, level, **kwargs)
     self.mage_attack.update(self.attack)
 
   def _level(self, entity):
     return entity.skills.mage.level.val
 
   @property
   def damage(self):
     return self.mage_attack.val
 
 
-# NOTE: Each consumable item (ration, poultice) cannot be stacked,
+# NOTE: Each consumable item (ration, potion) cannot be stacked,
 #   so each item takes 1 inventory space
 class Consumable(Item):
   def use(self, entity) -> bool:
     assert self in entity.inventory, "Item is not in entity's inventory"
     assert self.listed_price == 0, "Listed item cannot be used"
     assert self._level(entity) >= self.level.val, "Entity's level is not sufficient to use the item"
 
     self.realm.log_milestone(
       f'Consumed_{self.__class__.__name__}', self.level.val,
       f"PROF: Consumed {self.level.val} {self.__class__.__name__} "
       f"by Entity level {entity.attack_level}",
       tags={"player_id": entity.ent_id})
 
+    self.realm.event_log.record(EventCode.CONSUME_ITEM, entity, item=self)
+
     self._apply_effects(entity)
     entity.inventory.remove(self)
     self.destroy()
     return True
 
 class Ration(Consumable):
   ITEM_TYPE_ID = 16
 
   def __init__(self, realm, level, **kwargs):
-    restore = realm.config.PROFESSION_CONSUMABLE_RESTORE(level)
+    restore = 0
+    if realm.config.PROFESSION_SYSTEM_ENABLED:
+      restore = realm.config.PROFESSION_CONSUMABLE_RESTORE(level)
     super().__init__(realm, level, resource_restore=restore, **kwargs)
 
   def _apply_effects(self, entity):
     entity.resources.food.increment(self.resource_restore.val)
     entity.resources.water.increment(self.resource_restore.val)
 
-class Poultice(Consumable):
+class Potion(Consumable):
   ITEM_TYPE_ID = 17
 
   def __init__(self, realm, level, **kwargs):
-    restore = realm.config.PROFESSION_CONSUMABLE_RESTORE(level)
+    restore = 0
+    if realm.config.PROFESSION_SYSTEM_ENABLED:
+      restore = realm.config.PROFESSION_CONSUMABLE_RESTORE(level)
     super().__init__(realm, level, health_restore=restore, **kwargs)
 
   def _apply_effects(self, entity):
     entity.resources.health.increment(self.health_restore.val)
     entity.poultice_consumed += 1
     entity.poultice_level_consumed = max(
       entity.poultice_level_consumed, self.level.val)
```

### Comparing `nmmo-1.7.0.1/nmmo/systems/skill.py` & `nmmo-2.0.0/nmmo/systems/skill.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import abc
 
 import numpy as np
 from ordered_set import OrderedSet
 
 from nmmo.lib import material
 from nmmo.systems import combat, experience
-
+from nmmo.lib.log import EventCode
 
 ### Infrastructure ###
 class SkillGroup:
   def __init__(self, realm, entity):
     self.config  = realm.config
     self.realm   = realm
     self.entity = entity
@@ -47,23 +47,25 @@
 
     data['exp']   = self.exp
     data['level'] = self.level.val
 
     return data
 
   def add_xp(self, xp):
-    level     = self.experience_calculator.level_at_exp(self.exp)
     self.exp += xp * self.config.PROGRESSION_BASE_XP_SCALE
+    new_level = int(self.experience_calculator.level_at_exp(self.exp))
 
-    level = self.experience_calculator.level_at_exp(self.exp)
-    self.level.update(int(level))
-
-    self.realm.log_milestone(f'Level_{self.__class__.__name__}', int(level),
-      f"PROGRESSION: Reached level {level} {self.__class__.__name__}",
-      tags={"player_id": self.entity.ent_id})
+    if new_level > self.level.val:
+      self.level.update(new_level)
+      self.realm.event_log.record(EventCode.LEVEL_UP, self.entity,
+                                  skill=self, level=new_level)
+
+      self.realm.log_milestone(f'Level_{self.__class__.__name__}', new_level,
+        f"PROGRESSION: Reached level {new_level} {self.__class__.__name__}",
+        tags={"player_id": self.entity.ent_id})
 
   def set_experience_by_level(self, level):
     self.exp = self.experience_calculator.level_at_exp(level)
     self.level.update(int(level))
 
   @property
   def level(self):
@@ -74,24 +76,29 @@
 class CombatSkill(Skill):
   def update(self):
     pass
 
 class NonCombatSkill(Skill):
   def __init__(self, skill_group: SkillGroup):
     super().__init__(skill_group)
-    self._level = Lvl(1)
+    self._level = DummyLevel()
 
   @property
   def level(self):
     return self._level
 
 class HarvestSkill(NonCombatSkill):
   def process_drops(self, matl, drop_table):
+    if not self.config.ITEM_SYSTEM_ENABLED:
+      return
+
     entity = self.entity
 
+    # harvest without tool will only yield level-1 item even with high skill level
+    # for example, fishing level=5 without rod will only yield level-1 ration
     level = 1
     tool  = entity.equipment.held
     if matl.tool is not None and isinstance(tool, matl.tool):
       level = tool.level.val
 
     #TODO: double-check drop table quantity
     for drop in drop_table.roll(self.realm, level):
@@ -100,14 +107,15 @@
       self.realm.log_milestone(f'Gather_{drop.__class__.__name__}',
         level, f"PROFESSION: Gathered level {level} {drop.__class__.__name__} "
         f"(level {self.level.val} {self.__class__.__name__})",
         tags={"player_id": entity.ent_id})
 
       if entity.inventory.space:
         entity.inventory.receive(drop)
+        self.realm.event_log.record(EventCode.HARVEST_ITEM, entity, item=drop)
 
   def harvest(self, matl, deplete=True):
     entity = self.entity
     realm  = self.realm
 
     r, c = entity.pos
     if realm.map.tiles[r, c].state != matl:
@@ -139,21 +147,23 @@
       self.process_drops(matl, drop_table)
 
     return drop_table
 
 class AmmunitionSkill(HarvestSkill):
   def process_drops(self, matl, drop_table):
     super().process_drops(matl, drop_table)
-    self.add_xp(self.config.PROGRESSION_AMMUNITION_XP_SCALE)
+    if self.config.PROGRESSION_SYSTEM_ENABLED:
+      self.add_xp(self.config.PROGRESSION_AMMUNITION_XP_SCALE)
 
 
 class ConsumableSkill(HarvestSkill):
   def process_drops(self, matl, drop_table):
     super().process_drops(matl, drop_table)
-    self.add_xp(self.config.PROGRESSION_CONSUMABLE_XP_SCALE)
+    if self.config.PROGRESSION_SYSTEM_ENABLED:
+      self.add_xp(self.config.PROGRESSION_CONSUMABLE_XP_SCALE)
 
 
 ### Skill groups ###
 class Basic(SkillGroup):
   def __init__(self, realm, entity):
     super().__init__(realm, entity)
 
@@ -200,129 +210,147 @@
   @property
   def combat_level(self):
     return max(self.melee.level,
                 self.range.level,
                 self.mage.level)
 
   def apply_damage(self, style):
-    if not self.config.PROGRESSION_SYSTEM_ENABLED:
-      return
-
-    skill  = self.__dict__[style]
-    skill.add_xp(self.config.PROGRESSION_COMBAT_XP_SCALE)
+    if self.config.PROGRESSION_SYSTEM_ENABLED:
+      skill  = self.__dict__[style]
+      skill.add_xp(self.config.PROGRESSION_COMBAT_XP_SCALE)
 
   def receive_damage(self, dmg):
     pass
 
 class Skills(Basic, Harvest, Combat):
   pass
 
 ### Skills ###
 class Melee(CombatSkill):
+  SKILL_ID = 1
+
   @property
   def level(self):
     return self.entity.melee_level
 
 class Range(CombatSkill):
+  SKILL_ID = 2
+
   @property
   def level(self):
     return self.entity.range_level
 
 class Mage(CombatSkill):
+  SKILL_ID = 3
+
   @property
   def level(self):
     return self.entity.mage_level
 
 Melee.weakness = Mage
 Range.weakness = Melee
 Mage.weakness  = Range
 
 ### Individual Skills ###
 
-class Lvl:
-  def __init__(self, val):
+class DummyLevel:
+  def __init__(self, val=0):
     self.val = val
 
   def update(self, val):
     self.val = val
 
 class Water(HarvestSkill):
   def update(self):
     config = self.config
     if not config.RESOURCE_SYSTEM_ENABLED:
       return
 
+    if config.IMMORTAL:
+      return
+
     depletion = config.RESOURCE_DEPLETION_RATE
     water = self.entity.resources.water
     water.decrement(depletion)
 
-    if self.config.IMMORTAL:
-      return
-
     if not self.harvest_adjacent(material.Water, deplete=False):
       return
 
     restore = np.floor(config.RESOURCE_BASE
                       * config.RESOURCE_HARVEST_RESTORE_FRACTION)
     water.increment(restore)
 
+    self.realm.event_log.record(EventCode.DRINK_WATER, self.entity)
 
-class Food(HarvestSkill):
-  def __init__(self, skill_group):
-    self._level = Lvl(1)
-    super().__init__(skill_group)
 
+class Food(HarvestSkill):
   def update(self):
     config = self.config
     if not config.RESOURCE_SYSTEM_ENABLED:
       return
 
+    if config.IMMORTAL:
+      return
+
     depletion = config.RESOURCE_DEPLETION_RATE
     food = self.entity.resources.food
     food.decrement(depletion)
 
-    if not self.harvest(material.Forest):
+    if not self.harvest(material.Foilage):
       return
 
     restore = np.floor(config.RESOURCE_BASE
                       * config.RESOURCE_HARVEST_RESTORE_FRACTION)
     food.increment(restore)
 
+    self.realm.event_log.record(EventCode.EAT_FOOD, self.entity)
+
+
 class Fishing(ConsumableSkill):
+  SKILL_ID = 4
+
   @property
   def level(self):
     return self.entity.fishing_level
 
   def update(self):
     self.harvest_adjacent(material.Fish)
 
 class Herbalism(ConsumableSkill):
+  SKILL_ID = 5
+
   @property
   def level(self):
     return self.entity.herbalism_level
 
   def update(self):
     self.harvest(material.Herb)
 
 class Prospecting(AmmunitionSkill):
+  SKILL_ID = 6
+
   @property
   def level(self):
     return self.entity.prospecting_level
 
   def update(self):
     self.harvest(material.Ore)
 
 class Carving(AmmunitionSkill):
+  SKILL_ID = 7
+
   @property
   def level(self):
     return self.entity.carving_level
 
   def update(self,):
     self.harvest(material.Tree)
 
 class Alchemy(AmmunitionSkill):
+  SKILL_ID = 8
+
   @property
   def level(self):
     return self.entity.alchemy_level
 
   def update(self):
     self.harvest(material.Crystal)
```

### Comparing `nmmo-1.7.0.1/nmmo/websocket.py` & `nmmo-2.0.0/nmmo/render/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 from twisted.web.server import Site
 from twisted.web.static import File
 
 from autobahn.twisted.websocket import WebSocketServerFactory, \
     WebSocketServerProtocol
 from autobahn.twisted.resource import WebSocketResource
 
+from .render_utils import np_encoder
+
 class GodswordServerProtocol(WebSocketServerProtocol):
     def __init__(self):
         super().__init__()
         print("Created a server")
         self.frame = 0
 
         #"connected" is already used by WSSP
@@ -87,17 +89,18 @@
             packet['size']   = data['size']
             self.sent_environment=True
 
         if 'overlay' in data:
            packet['overlay'] = data['overlay']
            print('SENDING OVERLAY: ', len(packet['overlay']))
 
-        packet = json.dumps(packet).encode('utf8')
+        packet = json.dumps(packet, default=np_encoder).encode('utf8')
         self.sendMessage(packet, False)
 
+
 class WSServerFactory(WebSocketServerFactory):
     def __init__(self, ip, realm):
         super().__init__(ip)
         self.realm = realm
         self.time = time.time()
         self.clients = []
```

### Comparing `nmmo-1.7.0.1/nmmo.egg-info/PKG-INFO` & `nmmo-2.0.0/nmmo.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: nmmo
-Version: 1.7.0.1
+Version: 2.0.0
 Summary: Neural MMO is a platform for multiagent intelligence research inspired by Massively Multiplayer Online (MMO) role-playing games. Documentation hosted at neuralmmo.github.io.
 Home-page: https://github.com/neuralmmo/environment
 Author: Joseph Suarez
 Author-email: jsuarez@mit.edu
 License: MIT
 Keywords: Neural MMO,MMO
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: docs
-Provides-Extra: cleanrl
 Provides-Extra: all
 License-File: LICENSE
 
 UNKNOWN
```

### Comparing `nmmo-1.7.0.1/nmmo.egg-info/SOURCES.txt` & `nmmo-2.0.0/nmmo.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,101 +1,106 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 nmmo/__init__.py
-nmmo/overlay.py
 nmmo/version.py
-nmmo/websocket.py
 nmmo.egg-info/PKG-INFO
 nmmo.egg-info/SOURCES.txt
 nmmo.egg-info/dependency_links.txt
 nmmo.egg-info/requires.txt
 nmmo.egg-info/top_level.txt
 nmmo/core/__init__.py
+nmmo/core/action.py
 nmmo/core/agent.py
 nmmo/core/config.py
 nmmo/core/env.py
 nmmo/core/log_helper.py
 nmmo/core/map.py
 nmmo/core/observation.py
 nmmo/core/realm.py
-nmmo/core/render_helper.py
-nmmo/core/replay.py
-nmmo/core/replay_helper.py
 nmmo/core/terrain.py
 nmmo/core/tile.py
 nmmo/datastore/__init__.py
 nmmo/datastore/datastore.py
 nmmo/datastore/id_allocator.py
 nmmo/datastore/numpy_datastore.py
 nmmo/datastore/serialized.py
 nmmo/entity/__init__.py
 nmmo/entity/entity.py
 nmmo/entity/entity_manager.py
 nmmo/entity/npc.py
 nmmo/entity/player.py
-nmmo/io/__init__.py
-nmmo/io/action.py
 nmmo/lib/__init__.py
 nmmo/lib/colors.py
+nmmo/lib/event_log.py
 nmmo/lib/log.py
 nmmo/lib/material.py
-nmmo/lib/overlay.py
 nmmo/lib/priorityqueue.py
-nmmo/lib/rating.py
 nmmo/lib/spawn.py
-nmmo/lib/task.py
+nmmo/lib/team_helper.py
 nmmo/lib/utils.py
+nmmo/render/__init__.py
+nmmo/render/overlay.py
+nmmo/render/render_client.py
+nmmo/render/render_utils.py
+nmmo/render/replay_helper.py
+nmmo/render/websocket.py
 nmmo/resource/crystal.png
 nmmo/resource/fish.png
-nmmo/resource/forest.png
+nmmo/resource/foilage.png
 nmmo/resource/fragment.png
 nmmo/resource/grass.png
 nmmo/resource/herb.png
-nmmo/resource/lava.png
 nmmo/resource/ocean.png
 nmmo/resource/ore.png
 nmmo/resource/scrub.png
 nmmo/resource/slag.png
 nmmo/resource/spawn.png
 nmmo/resource/stone.png
 nmmo/resource/stump.png
 nmmo/resource/tree.png
+nmmo/resource/void.png
 nmmo/resource/water.png
 nmmo/resource/weeds.png
 nmmo/systems/__init__.py
-nmmo/systems/achievement.py
 nmmo/systems/combat.py
 nmmo/systems/droptable.py
 nmmo/systems/exchange.py
 nmmo/systems/experience.py
 nmmo/systems/inventory.py
 nmmo/systems/item.py
 nmmo/systems/skill.py
 nmmo/systems/ai/__init__.py
 nmmo/systems/ai/behavior.py
 nmmo/systems/ai/move.py
 nmmo/systems/ai/policy.py
 nmmo/systems/ai/utils.py
+nmmo/task/__init__.py
+nmmo/task/base_predicates.py
+nmmo/task/constraint.py
+nmmo/task/game_state.py
+nmmo/task/group.py
+nmmo/task/predicate_api.py
+nmmo/task/task_api.py
 scripted/__init__.py
 scripted/attack.py
 scripted/baselines.py
 scripted/behavior.py
 scripted/move.py
 scripted/utils.py
 tests/__init__.py
 tests/conftest.py
-tests/test_client.py
 tests/test_determinism.py
 tests/test_deterministic_replay.py
+tests/test_eventlog.py
 tests/test_performance.py
 tests/test_pettingzoo.py
 tests/test_rollout.py
-tests/test_task.py
+tests/test_team_spawn.py
 tests/testhelpers.py
 tests/datastore/__init__.py
 tests/datastore/test_datastore.py
 tests/datastore/test_id_allocator.py
 tests/datastore/test_numpy_datastore.py
 tests/entity/__init__.py
 tests/entity/test_entity.py
```

### Comparing `nmmo-1.7.0.1/scripted/attack.py` & `nmmo-2.0.0/scripted/attack.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/scripted/baselines.py` & `nmmo-2.0.0/scripted/baselines.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import random
 
 import nmmo
 from nmmo import material
 from nmmo.systems import skill
 import nmmo.systems.item as item_system
 from nmmo.lib import colors
-from nmmo.io import action
+from nmmo.core import action
 from nmmo.core.observation import Observation
 
 from scripted import attack, move
 
 class Scripted(nmmo.Agent):
   '''Template class for scripted models.
 
@@ -80,17 +80,18 @@
   def target_weak(self):
     '''Target the nearest agent if it is weak'''
     if self.closest is None:
       return False
 
     selfLevel  = self.me.level
     targLevel  = max(self.closest.melee_level, self.closest.range_level, self.closest.mage_level)
-    population = self.closest.population_id
 
-    if population == -1 or targLevel <= selfLevel <= 5 or selfLevel >= targLevel + 3:
+    if self.closest.npc_type == 1 or \
+       targLevel <= selfLevel <= 5 or \
+       selfLevel >= targLevel + 3:
       self.target     = self.closest
       self.targetID   = self.closestID
       self.targetDist = self.closestDist
 
   def scan_agents(self):
     '''Scan the nearby area for agents'''
     self.closest, self.closestDist   = attack.closestTarget(self.config, self.ob)
@@ -133,27 +134,27 @@
     self.best_items: Dict   = {}
     self.item_counts = defaultdict(int)
 
     self.item_levels = {
       item_system.Hat.ITEM_TYPE_ID: self.level,
       item_system.Top.ITEM_TYPE_ID: self.level,
       item_system.Bottom.ITEM_TYPE_ID: self.level,
-      item_system.Sword.ITEM_TYPE_ID: self.me.melee_level,
+      item_system.Spear.ITEM_TYPE_ID: self.me.melee_level,
       item_system.Bow.ITEM_TYPE_ID: self.me.range_level,
       item_system.Wand.ITEM_TYPE_ID: self.me.mage_level,
       item_system.Rod.ITEM_TYPE_ID: self.me.fishing_level,
       item_system.Gloves.ITEM_TYPE_ID: self.me.herbalism_level,
       item_system.Pickaxe.ITEM_TYPE_ID: self.me.prospecting_level,
-      item_system.Chisel.ITEM_TYPE_ID: self.me.carving_level,
-      item_system.Arcane.ITEM_TYPE_ID: self.me.alchemy_level,
-      item_system.Scrap.ITEM_TYPE_ID: self.me.melee_level,
-      item_system.Shaving.ITEM_TYPE_ID: self.me.range_level,
-      item_system.Shard.ITEM_TYPE_ID: self.me.mage_level,
+      item_system.Axe.ITEM_TYPE_ID: self.me.carving_level,
+      item_system.Chisel.ITEM_TYPE_ID: self.me.alchemy_level,
+      item_system.Whetstone.ITEM_TYPE_ID: self.me.melee_level,
+      item_system.Arrow.ITEM_TYPE_ID: self.me.range_level,
+      item_system.Runes.ITEM_TYPE_ID: self.me.mage_level,
       item_system.Ration.ITEM_TYPE_ID: self.level,
-      item_system.Poultice.ITEM_TYPE_ID: self.level
+      item_system.Potion.ITEM_TYPE_ID: self.level
     }
 
     for item_ary in self.ob.inventory.values:
       itm = item_system.ItemState.parse_array(item_ary)
       assert itm.quantity != 0
 
       # Too high level to equip or use
@@ -226,31 +227,31 @@
       # InventoryItem needs where the item is (index) in the inventory
       self.actions[action.Use] = {
         action.InventoryItem: self.ob.inventory.index(itm.id)} # list(self.ob.inventory.ids).index(itm.id)
 
     return True
 
   def consume(self):
-    if self.me.health <= self.health_max // 2 and item_system.Poultice.ITEM_TYPE_ID in self.best_items:
-      itm = self.best_items[item_system.Poultice.ITEM_TYPE_ID]
+    if self.me.health <= self.health_max // 2 and item_system.Potion.ITEM_TYPE_ID in self.best_items:
+      itm = self.best_items[item_system.Potion.ITEM_TYPE_ID]
     elif (self.me.food == 0 or self.me.water == 0) and item_system.Ration.ITEM_TYPE_ID in self.best_items:
       itm = self.best_items[item_system.Ration.ITEM_TYPE_ID]
     else:
       return
 
     if itm.listed_price:
       return
 
     # InventoryItem needs where the item is (index) in the inventory
     self.actions[action.Use] = {
       action.InventoryItem: self.ob.inventory.index(itm.id)} # list(self.ob.inventory.ids).index(itm.id)
 
   def sell(self, keep_k: dict, keep_best: set):
     for itm in self.inventory.values():
-      price = int(max(itm.level, len(action.Price.edges)-1))
+      price = int(max(itm.level, 1))
       assert itm.quantity > 0
 
       if itm.equipped or itm.listed_price:
         continue
 
       if itm.type_id in keep_k:
         owned = self.item_counts[itm.type_id]
@@ -262,15 +263,15 @@
       if itm.type_id in self.best_items and \
         itm.type_id in keep_best and \
         itm.id == self.best_items[itm.type_id].id:
         continue
 
       self.actions[action.Sell] = {
         action.InventoryItem: self.ob.inventory.index(itm.id), # list(self.ob.inventory.ids).index(itm.id)
-        action.Price: action.Price.edges[price] }
+        action.Price: action.Price.edges[price-1] } # Price starts from 1
 
       return itm
 
   def buy(self, buy_k: dict, buy_upgrade: set):
     if len(self.inventory) >= self.config.ITEM_INVENTORY_CAPACITY:
       return
 
@@ -326,27 +327,28 @@
       skill.Herbalism: self.me.herbalism_level,
       skill.Prospecting: self.me.prospecting_level,
       skill.Carving: self.me.carving_level,
       skill.Alchemy: self.me.alchemy_level
     }
 
     # TODO(kywch): need a consistent level variables
-    # level for using armor, rations, and poultice
+    # level for using armor, rations, and potion
     self.level = min(1, max(self.skills.values()))
 
     if self.spawnR is None:
       self.spawnR = self.me.row
     if self.spawnC is None:
       self.spawnC = self.me.col
 
     # When to run from death fog in BR configs
     self.fog_criterion = None
     if self.config.PLAYER_DEATH_FOG is not None:
-      start_running = self.time_alive > self.config.PLAYER_DEATH_FOG - 64
-      run_now = self.time_alive % max(1, int(1 / self.config.PLAYER_DEATH_FOG_SPEED))
+      time_alive = self.me.time_alive
+      start_running = time_alive > self.config.PLAYER_DEATH_FOG - 64
+      run_now = time_alive % max(1, int(1 / self.config.PLAYER_DEATH_FOG_SPEED))
       self.fog_criterion = start_running and run_now
 
 
 class Sleeper(Scripted):
   '''Do Nothing'''
   def __call__(self, obs):
     super().__call__(obs)
@@ -394,15 +396,15 @@
     super().__init__(config, idx)
     self.style  = [action.Melee, action.Range, action.Mage]
 
   @property
   def supplies(self):
     return {
       item_system.Ration.ITEM_TYPE_ID: 2,
-      item_system.Poultice.ITEM_TYPE_ID: 2,
+      item_system.Potion.ITEM_TYPE_ID: 2,
       self.ammo.ITEM_TYPE_ID: 10
     }
 
   @property
   def wishlist(self):
     return {
       item_system.Hat.ITEM_TYPE_ID,
@@ -428,15 +430,15 @@
     super().__init__(config, idx)
     self.resource = [material.Fish, material.Herb, material.Ore, material.Tree, material.Crystal]
 
   @property
   def supplies(self):
     return {
       item_system.Ration.ITEM_TYPE_ID: 1,
-      item_system.Poultice.ITEM_TYPE_ID: 1
+      item_system.Potion.ITEM_TYPE_ID: 1
     }
 
   @property
   def wishlist(self):
     return {
       item_system.Hat.ITEM_TYPE_ID,
       item_system.Top.ITEM_TYPE_ID,
@@ -478,39 +480,39 @@
     self.tool     = item_system.Pickaxe
 
 class Carver(Gather):
   def __init__(self, config, idx):
     super().__init__(config, idx)
     if config.SPECIALIZE:
       self.resource = [material.Tree]
-    self.tool     = item_system.Chisel
+    self.tool     = item_system.Axe
 
 class Alchemist(Gather):
   def __init__(self, config, idx):
     super().__init__(config, idx)
     if config.SPECIALIZE:
       self.resource = [material.Crystal]
-    self.tool     = item_system.Arcane
+    self.tool     = item_system.Chisel
 
 class Melee(Combat):
   def __init__(self, config, idx):
     super().__init__(config, idx)
     if config.SPECIALIZE:
       self.style  = [action.Melee]
-    self.weapon = item_system.Sword
-    self.ammo   = item_system.Scrap
+    self.weapon = item_system.Spear
+    self.ammo   = item_system.Whetstone
 
 class Range(Combat):
   def __init__(self, config, idx):
     super().__init__(config, idx)
     if config.SPECIALIZE:
       self.style  = [action.Range]
     self.weapon = item_system.Bow
-    self.ammo   = item_system.Shaving
+    self.ammo   = item_system.Arrow
 
 class Mage(Combat):
   def __init__(self, config, idx):
     super().__init__(config, idx)
     if config.SPECIALIZE:
       self.style  = [action.Mage]
     self.weapon = item_system.Wand
-    self.ammo   = item_system.Shard
+    self.ammo   = item_system.Runes
```

### Comparing `nmmo-1.7.0.1/scripted/behavior.py` & `nmmo-2.0.0/scripted/behavior.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/scripted/move.py` & `nmmo-2.0.0/scripted/move.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # pylint: disable=all
 
 import numpy as np
 import random
 
 import heapq
 
-from nmmo.io import action
+from nmmo.core import action
 from nmmo.core.observation import Observation
 from nmmo.lib import material
 
 from scripted import utils
 
 def adjacentPos(pos):
    r, c = pos
@@ -41,21 +41,21 @@
 def pathfind(config, ob, actions, rr, cc):
    direction = aStar(config, ob, actions, rr, cc)
    direction = towards(direction)
    actions[action.Move] = {action.Direction: direction}
 
 def meander(config, ob, actions):
    cands = []
-   if ob.tile(-1, 0).material_id in material.Habitable:
+   if ob.tile(-1, 0).material_id in material.Habitable.indices:
       cands.append((-1, 0))
-   if ob.tile(1, 0).material_id in material.Habitable:
+   if ob.tile(1, 0).material_id in material.Habitable.indices:
       cands.append((1, 0))
-   if ob.tile(0, -1).material_id in material.Habitable:
+   if ob.tile(0, -1).material_id in material.Habitable.indices:
       cands.append((0, -1))
-   if ob.tile(0, 1).material_id in material.Habitable:
+   if ob.tile(0, 1).material_id in material.Habitable.indices:
       cands.append((0, 1))
    if not cands:
       return (-1, 0)
 
    direction = random.choices(cands)[0]
    direction = towards(direction)
    actions[action.Move] = {action.Direction: direction}
@@ -108,22 +108,22 @@
 
          if not inSight(*nxt, vision):
             continue
 
          tile     = ob.tile(*nxt)
          matl     = tile.material_id
 
-         if not matl in material.Habitable:
+         if not matl in material.Habitable.indices:
             continue
 
          food, water = reward[cur]
          food  = max(0, food - 1)
          water = max(0, water - 1)
 
-         if matl == material.Forest.index:
+         if matl == material.Foilage.index:
             food = min(food+food_max//2, food_max)
          for pos in adjacentPos(nxt):
             if not inSight(*pos, vision):
                continue
 
             tile = ob.tile(*pos)
             matl = tile.material_id
@@ -207,15 +207,15 @@
             matl     = tile.material_id
 
             if material.Fish in resource and material.Fish.index == matl:
                 found = nxt
                 backtrace[nxt] = cur
                 break
 
-            if not tile.material_id in material.Habitable:
+            if not tile.material_id in material.Habitable.indices:
                 continue
 
             if matl in (e.index for e in resource):
                 found = nxt
                 backtrace[nxt] = cur
                 break
 
@@ -281,19 +281,19 @@
       for nxt in adjacentPos(cur):
          if not inSight(*nxt, vision):
             continue
 
          tile     = ob.tile(*nxt)
          matl     = tile.material_id
 
-         if not matl in material.Habitable:
+         if not matl in material.Habitable.indices:
            continue
 
          #Omitted water from the original implementation. Seems key
-         if matl in material.Impassible:
+         if matl in material.Impassible.indices:
             continue
 
          newCost = cost[cur] + 1
          if nxt not in cost or newCost < cost[nxt]:
             cost[nxt] = newCost
             heuristic = utils.lInfty(goal, nxt)
             priority = newCost + heuristic
```

### Comparing `nmmo-1.7.0.1/scripted/utils.py` & `nmmo-2.0.0/scripted/utils.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/setup.py` & `nmmo-2.0.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,70 +2,67 @@
 
 from setuptools import find_packages, setup
 
 REPO_URL = "https://github.com/neuralmmo/environment"
 
 extra = {
     'docs': [
+        'sphinx==5.0.0',
         'sphinx-rtd-theme==0.5.1',
         'sphinxcontrib-youtube==1.0.1',
-        ],
-    'cleanrl': [
-        'wandb==0.12.9',
-        'supersuit==3.3.5',
-        'tensorboard',
-        'torch',
-        'openskill',
-        ],
-    }
+        'myst-parser==1.0.0',
+        'sphinx-rtd-theme==0.5.1',
+        'sphinx-design==0.4.1',
+        'furo==2023.3.27',
+    ],
+}
 
 extra['all'] = list(set(chain.from_iterable(extra.values())))
- 
+
+with open('nmmo/version.py', encoding="utf-8") as vf:
+  ver = vf.read().split()[-1].strip("'")
+
 setup(
-    name="nmmo",
-    description="Neural MMO is a platform for multiagent intelligence research inspired by "
-    "Massively Multiplayer Online (MMO) role-playing games. Documentation hosted at neuralmmo.github.io.",
-    long_description_content_type="text/markdown",
-    version=open('nmmo/version.py').read().split()[-1].strip("'"),
-    packages=find_packages(),
-    include_package_data=True,
-    install_requires=[
-        'pytest<7',
-        'pytest-pythonpath==0.7.4',
-        'pytest-benchmark==3.4.1',
-        #'openskill==4.0.0',
-        'fire==0.4.0',
-        'setproctitle==1.1.10',
-        'service-identity==21.1.0',
-        'autobahn==19.3.3',
-        'Twisted==19.2.0',
-        'vec-noise==1.1.4',
-        'imageio==2.23.0',
-        'tqdm==4.61.1',
-        'lz4==4.0.0',
-        'h5py==3.7.0',
-        'ordered-set==4.1.0',
-        'pettingzoo==1.19.0',
-        'gym==0.23.0',
-        'pylint==2.16.0',
-        'py==1.11.0',
-        'scipy==1.10.0',
-        'numpy==1.23.3',
-        'numpy-indexed==0.3.7'
-    ],
-    extras_require=extra,
-    python_requires=">=3.7",
-    license="MIT",
-    author="Joseph Suarez",
-    author_email="jsuarez@mit.edu",
-    url=REPO_URL,
-    keywords=["Neural MMO", "MMO"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Intended Audience :: Science/Research",
-        "Intended Audience :: Developers",
-        "Environment :: Console",
-        "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.9",
-    ],
+  name="nmmo",
+  description="Neural MMO is a platform for multiagent intelligence research " + \
+              "inspired by Massively Multiplayer Online (MMO) role-playing games. " + \
+              "Documentation hosted at neuralmmo.github.io.",
+  long_description_content_type="text/markdown",
+  version=ver,
+  packages=find_packages(),
+  include_package_data=True,
+  install_requires=[
+    'numpy==1.23.3',
+    'scipy==1.10.0',
+    'pytest==7.3.0',
+    'pytest-benchmark==3.4.1',
+    'fire==0.4.0',
+    'autobahn==19.3.3',
+    'Twisted==19.2.0',
+    'vec-noise==1.1.4',
+    'imageio==2.23.0',
+    'ordered-set==4.1.0',
+    'pettingzoo==1.19.0',
+    'gym==0.23.0',
+    'pylint==2.16.0',
+    'py==1.11.0',
+    'tqdm<5',
+  ],
+  extras_require=extra,
+  python_requires=">=3.7",
+  license="MIT",
+  author="Joseph Suarez",
+  author_email="jsuarez@mit.edu",
+  url=REPO_URL,
+  keywords=["Neural MMO", "MMO"],
+  classifiers=[
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: Developers",
+    "Environment :: Console",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3.7",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+  ],
 )
-
```

### Comparing `nmmo-1.7.0.1/tests/datastore/test_datastore.py` & `nmmo-2.0.0/tests/datastore/test_datastore.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/tests/datastore/test_id_allocator.py` & `nmmo-2.0.0/tests/datastore/test_id_allocator.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/tests/datastore/test_numpy_datastore.py` & `nmmo-2.0.0/tests/datastore/test_numpy_datastore.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/tests/entity/test_entity.py` & `nmmo-2.0.0/tests/entity/test_entity.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,21 +11,19 @@
     self.datastore.register_object_type("Entity", EntityState.State.num_attributes)
 
 # pylint: disable=no-member
 class TestEntity(unittest.TestCase):
   def test_entity(self):
     realm = MockRealm()
     entity_id = 123
-    population_id = 11
-    entity = Entity(realm, (10,20), entity_id, "name", "color", population_id)
+    entity = Entity(realm, (10,20), entity_id, "name")
 
     self.assertEqual(entity.id.val, entity_id)
     self.assertEqual(entity.row.val, 10)
     self.assertEqual(entity.col.val, 20)
-    self.assertEqual(entity.population_id.val, population_id)
     self.assertEqual(entity.damage.val, 0)
     self.assertEqual(entity.time_alive.val, 0)
     self.assertEqual(entity.freeze.val, 0)
     self.assertEqual(entity.item_level.val, 0)
     self.assertEqual(entity.attacker_id.val, 0)
     self.assertEqual(entity.message.val, 0)
     self.assertEqual(entity.gold.val, 0)
@@ -40,16 +38,15 @@
     self.assertEqual(entity.prospecting_level.val, 0)
     self.assertEqual(entity.carving_level.val, 0)
     self.assertEqual(entity.alchemy_level.val, 0)
 
   def test_query_by_ids(self):
     realm = MockRealm()
     entity_id = 123
-    population_id = 11
-    entity = Entity(realm, (10,20), entity_id, "name", "color", population_id)
+    entity = Entity(realm, (10,20), entity_id, "name")
 
     entities = EntityState.Query.by_ids(realm.datastore, [entity_id])
     self.assertEqual(len(entities), 1)
     self.assertEqual(entities[0][Entity.State.attr_name_to_col["id"]], entity_id)
     self.assertEqual(entities[0][Entity.State.attr_name_to_col["row"]], 10)
     self.assertEqual(entities[0][Entity.State.attr_name_to_col["col"]], 20)
```

### Comparing `nmmo-1.7.0.1/tests/lib/test_serialized.py` & `nmmo-2.0.0/tests/lib/test_serialized.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/tests/test_determinism.py` & `nmmo-2.0.0/tests/test_determinism.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 #from pdb import set_trace as T
 import unittest
 
 import logging
 import random
 from tqdm import tqdm
 
-# pylint: disable=import-error
-from testhelpers import ScriptedAgentTestConfig, ScriptedAgentTestEnv
-from testhelpers import observations_are_equal, actions_are_equal
+from tests.testhelpers import ScriptedAgentTestConfig, ScriptedAgentTestEnv
+from tests.testhelpers import observations_are_equal, actions_are_equal
 
 # 30 seems to be enough to test variety of agent actions
 TEST_HORIZON = 30
 RANDOM_SEED = random.randint(0, 10000)
 
 
 class TestDeterminism(unittest.TestCase):
```

### Comparing `nmmo-1.7.0.1/tests/test_deterministic_replay.py` & `nmmo-2.0.0/tests/test_deterministic_replay.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,16 @@
 import logging
 import random
 from typing import Any, Dict
 
 import numpy as np
 from tqdm import tqdm
 
-# pylint: disable=import-error
-from testhelpers import ScriptedAgentTestConfig, ScriptedAgentTestEnv, observations_are_equal
+from tests.testhelpers import ScriptedAgentTestConfig, ScriptedAgentTestEnv
+from tests.testhelpers import observations_are_equal
 
 import nmmo
 
 TEST_HORIZON = 50
 LOCAL_REPLAY = 'tests/replay_local.pickle'
 
 def load_replay_file(replay_file):
@@ -40,16 +40,16 @@
   return seed, config, map_src, init_obs, init_npcs, med_obs, actions, final_obs, final_npcs
 
 
 def make_actions_picklable(actions: Dict[int, Dict[str, Dict[str, Any]]]):
   for eid in actions:
     for atn, args in actions[eid].items():
       for arg, val in args.items():
-        if arg == nmmo.io.action.Price and not isinstance(val, int):
-          # <class 'nmmo.io.action.Price'>: <class 'nmmo.io.action.Discrete_1'>
+        if arg == nmmo.action.Price and not isinstance(val, int):
+          # <class 'nmmo.action.Price'>: <class 'nmmo.action.Discrete_1'>
           # convert Discrete_1 to 1
           actions[eid][atn][arg] = val.val
   return actions
 
 
 def generate_replay_file(replay_file, test_horizon):
   # generate the new data with a new env
```

### Comparing `nmmo-1.7.0.1/tests/test_performance.py` & `nmmo-2.0.0/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `nmmo-1.7.0.1/tests/testhelpers.py` & `nmmo-2.0.0/tests/testhelpers.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import logging
 import unittest
 
 from copy import deepcopy
+from timeit import timeit
 import numpy as np
 
 import nmmo
 
 from scripted import baselines
 from nmmo.entity.entity import EntityState
-from nmmo.io import action
+from nmmo.core import action
 from nmmo.systems import item as Item
+from nmmo.core.realm import Realm
 
 # this function can be replaced by assertDictEqual
 # but might be still useful for debugging
 def actions_are_equal(source_atn, target_atn, debug=True):
 
   # compare the numbers and player ids
   player_src = list(source_atn.keys())
@@ -108,14 +110,16 @@
 
   LOG_ENV = True
 
   LOG_MILESTONES = True
   LOG_EVENTS = False
   LOG_VERBOSE = False
 
+  PLAYER_DEATH_FOG = 5
+
   SPECIALIZE = True
   PLAYERS = [
     baselines.Fisher, baselines.Herbalist,
     baselines.Prospector,baselines.Carver, baselines.Alchemist,
     baselines.Melee, baselines.Range, baselines.Mage]
 
 
@@ -161,14 +165,36 @@
       # and the env.step() does not give the same results in the deterministic replay.
       for eid, ent in self.realm.players.items():
         ent.agent(self.obs[eid])
 
     return actions
 
 
+def change_spawn_pos(realm: Realm, ent_id: int, new_pos):
+  # check if the position is valid
+  assert realm.map.tiles[new_pos].habitable, "Given pos is not habitable."
+  assert realm.entity(ent_id), "No such entity in the realm"
+
+  entity = realm.entity(ent_id)
+  old_pos = entity.pos
+  realm.map.tiles[old_pos].remove_entity(ent_id)
+
+  # set to new pos
+  entity.row.update(new_pos[0])
+  entity.col.update(new_pos[1])
+  entity.spawn_pos = new_pos
+  realm.map.tiles[new_pos].add_entity(entity)
+
+def provide_item(realm: Realm, ent_id: int,
+                 item: Item.Item, level: int, quantity: int):
+  for _ in range(quantity):
+    realm.players[ent_id].inventory.receive(
+      item(realm, level=level))
+
+
 # pylint: disable=invalid-name,protected-access
 class ScriptedTestTemplate(unittest.TestCase):
 
   @classmethod
   def setUpClass(cls):
     # only use Combat agents
     cls.config = ScriptedAgentTestConfig()
@@ -178,46 +204,27 @@
     cls.config.PLAYER_N = 3
     #cls.config.IMMORTAL = True
 
     # set up agents to test ammo use
     cls.policy = { 1:'Melee', 2:'Range', 3:'Mage' }
     # 1 cannot hit 3, 2 can hit 1, 3 cannot hit 2
     cls.spawn_locs = { 1:(17, 17), 2:(17, 19), 3:(21, 21) }
-    cls.ammo = { 1:Item.Scrap, 2:Item.Shaving, 3:Item.Shard }
+    cls.ammo = { 1:Item.Whetstone, 2:Item.Arrow, 3:Item.Runes }
     cls.ammo_quantity = 2
 
     # items to provide
     cls.init_gold = 5
     cls.item_level = [0, 3] # 0 can be used, 3 cannot be used
     cls.item_sig = {}
 
-  def _change_spawn_pos(self, realm, ent_id, new_pos):
-    # check if the position is valid
-    assert realm.map.tiles[new_pos].habitable, "Given pos is not habitable."
-    assert realm.entity(ent_id), "No such entity in the realm"
-
-    entity = realm.entity(ent_id)
-    old_pos = entity.pos
-    realm.map.tiles[old_pos].remove_entity(ent_id)
-
-    # set to new pos
-    entity.row.update(new_pos[0])
-    entity.col.update(new_pos[1])
-    entity.spawn_pos = new_pos
-    realm.map.tiles[new_pos].add_entity(entity)
-
-  def _provide_item(self, realm, ent_id, item, level, quantity):
-    realm.players[ent_id].inventory.receive(
-      item(realm, level=level, quantity=quantity))
-
   def _make_item_sig(self):
     item_sig = {}
     for ent_id, ammo in self.ammo.items():
       item_sig[ent_id] = []
-      for item in [ammo, Item.Top, Item.Gloves, Item.Ration, Item.Poultice]:
+      for item in [ammo, Item.Top, Item.Gloves, Item.Ration, Item.Potion]:
         for lvl in self.item_level:
           item_sig[ent_id].append((item, lvl))
 
     return item_sig
 
   def _setup_env(self, random_seed, check_assert=True):
     """ set up a new env and perform initial checks """
@@ -229,21 +236,21 @@
       env.realm.players[ent_id].gold.update(self.init_gold)
 
     # provide items that are in item_sig
     self.item_sig = self._make_item_sig()
     for ent_id, items in self.item_sig.items():
       for item_sig in items:
         if item_sig[0] == self.ammo[ent_id]:
-          self._provide_item(env.realm, ent_id, item_sig[0], item_sig[1], self.ammo_quantity)
+          provide_item(env.realm, ent_id, item_sig[0], item_sig[1], self.ammo_quantity)
         else:
-          self._provide_item(env.realm, ent_id, item_sig[0], item_sig[1], 1)
+          provide_item(env.realm, ent_id, item_sig[0], item_sig[1], 1)
 
     # teleport the players, if provided with specific locations
     for ent_id, pos in self.spawn_locs.items():
-      self._change_spawn_pos(env.realm, ent_id, pos)
+      change_spawn_pos(env.realm, ent_id, pos)
 
     env.obs = env._compute_observations()
 
     if check_assert:
       self._check_default_asserts(env)
 
     return env
@@ -321,24 +328,33 @@
       ent_obs = env.obs[ent_id]
 
       if atn in [action.Give, action.GiveGold]:
         # self should be always masked
         self.assertFalse(self._check_ent_mask(ent_obs, atn, ent_id))
 
         # check if the target is masked as expected
-        self.assertEqual( cond['ent_mask'],
-          self._check_ent_mask(ent_obs, atn, cond['tgt_id']) )
+        self.assertEqual(
+          cond['ent_mask'],
+          self._check_ent_mask(ent_obs, atn, cond['tgt_id']),
+          f"ent_id: {ent_id}, atn: {ent_id}, tgt_id: {cond['tgt_id']}"
+        )
 
       if atn in [action.Give]:
-        self.assertEqual( cond['inv_mask'],
-          self._check_inv_mask(ent_obs, atn, cond['item_sig']) )
+        self.assertEqual(
+          cond['inv_mask'],
+          self._check_inv_mask(ent_obs, atn, cond['item_sig']),
+          f"ent_id: {ent_id}, atn: {ent_id}, tgt_id: {cond['item_sig']}"
+        )
 
       if atn in [action.Buy]:
-        self.assertEqual( cond['mkt_mask'],
-          self._check_mkt_mask(ent_obs, cond['item_id']) )
+        self.assertEqual(
+          cond['mkt_mask'],
+          self._check_mkt_mask(ent_obs, cond['item_id']),
+          f"ent_id: {ent_id}, atn: {ent_id}, tgt_id: {cond['item_id']}"
+        )
 
       # append the actions
       if atn == action.Give:
         actions[ent_id] = { action.Give: {
           action.InventoryItem: env.obs[ent_id].inventory.sig(*cond['item_sig']),
           action.Target: cond['tgt_id'] } }
 
@@ -347,7 +363,35 @@
           { action.Target: cond['tgt_id'], action.Price: cond['gold'] } }
 
       elif atn == action.Buy:
         mkt_idx = ent_obs.market.index(cond['item_id'])
         actions[ent_id] = { action.Buy: { action.MarketItem: mkt_idx } }
 
     return actions
+
+# pylint: disable=unnecessary-lambda,bad-builtin
+def profile_env_step(action_target=True, tasks=None, condition=None):
+  config = nmmo.config.Default()
+  config.PLAYERS = [baselines.Sleeper] # the scripted agents doing nothing
+  config.IMMORTAL = True # otherwise the agents will die
+  config.PROVIDE_ACTION_TARGETS = action_target
+  env = nmmo.Env(config)
+  if tasks is None:
+    tasks = []
+  env.reset(seed=0, make_task_fn=lambda: tasks)
+  for _ in range(3):
+    env.step({})
+
+  obs = env._compute_observations()
+
+  test_func = [
+    ('env.step({}):', lambda: env.step({})),
+    ('env.realm.step():', lambda: env.realm.step({})),
+    ('env._compute_observations():', lambda: env._compute_observations()),
+    ('obs.to_gym(), ActionTarget:', lambda: {a: o.to_gym() for a,o in obs.items()}),
+    ('env._compute_rewards():', lambda: env._compute_rewards(obs.keys(), {}))
+  ]
+
+  if condition:
+    print('=== Test condition:', condition, '===')
+  for name, func in test_func:
+    print(' -', name, timeit(func, number=100, globals=globals()))
```

