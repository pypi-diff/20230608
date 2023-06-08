# Comparing `tmp/pikanetwork.py-1.0.0.tar.gz` & `tmp/pikanetwork.py-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pikanetwork.py-1.0.0.tar", last modified: Wed Jun  7 13:27:52 2023, max compression
+gzip compressed data, was "pikanetwork.py-1.0.1.tar", last modified: Thu Jun  8 08:40:41 2023, max compression
```

## Comparing `pikanetwork.py-1.0.0.tar` & `pikanetwork.py-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 13:27:52.158774 pikanetwork.py-1.0.0/
--rw-rw-rw-   0        0        0     1070 2023-06-07 11:42:00.000000 pikanetwork.py-1.0.0/LICENSE
--rw-rw-rw-   0        0        0       24 2023-06-07 13:25:41.000000 pikanetwork.py-1.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2464 2023-06-07 13:27:52.156773 pikanetwork.py-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1531 2023-06-07 11:49:13.000000 pikanetwork.py-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 13:27:52.145415 pikanetwork.py-1.0.0/pikanetwork/
--rw-rw-rw-   0        0        0      311 2023-06-07 13:27:49.000000 pikanetwork.py-1.0.0/pikanetwork/__init__.py
--rw-rw-rw-   0        0        0     1162 2023-06-07 11:49:13.000000 pikanetwork.py-1.0.0/pikanetwork/api.py
--rw-rw-rw-   0        0        0     2481 2023-06-07 11:27:56.000000 pikanetwork.py-1.0.0/pikanetwork/builders.py
--rw-rw-rw-   0        0        0     1747 2023-06-07 10:59:44.000000 pikanetwork.py-1.0.0/pikanetwork/models.py
-drwxrwxrwx   0        0        0        0 2023-06-07 13:27:52.154775 pikanetwork.py-1.0.0/pikanetwork.py.egg-info/
--rw-rw-rw-   0        0        0     2464 2023-06-07 13:27:52.000000 pikanetwork.py-1.0.0/pikanetwork.py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      333 2023-06-07 13:27:52.000000 pikanetwork.py-1.0.0/pikanetwork.py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 13:27:52.000000 pikanetwork.py-1.0.0/pikanetwork.py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 13:27:52.000000 pikanetwork.py-1.0.0/pikanetwork.py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-07 13:27:52.000000 pikanetwork.py-1.0.0/pikanetwork.py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        8 2023-06-07 12:54:25.000000 pikanetwork.py-1.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 13:27:52.158774 pikanetwork.py-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     2182 2023-06-07 12:58:41.000000 pikanetwork.py-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:40:41.347729 pikanetwork.py-1.0.1/
+-rw-rw-rw-   0        0        0     1070 2023-06-07 11:42:00.000000 pikanetwork.py-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0       24 2023-06-07 13:25:41.000000 pikanetwork.py-1.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3899 2023-06-08 08:40:41.346726 pikanetwork.py-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2966 2023-06-08 08:36:17.000000 pikanetwork.py-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 08:40:41.333095 pikanetwork.py-1.0.1/pikanetwork/
+-rw-rw-rw-   0        0        0      313 2023-06-08 08:37:00.000000 pikanetwork.py-1.0.1/pikanetwork/__init__.py
+-rw-rw-rw-   0        0        0     1087 2023-06-08 08:26:33.000000 pikanetwork.py-1.0.1/pikanetwork/api.py
+-rw-rw-rw-   0        0        0     2548 2023-06-08 08:22:02.000000 pikanetwork.py-1.0.1/pikanetwork/builders.py
+-rw-rw-rw-   0        0        0      189 2023-06-08 08:25:43.000000 pikanetwork.py-1.0.1/pikanetwork/exceptions.py
+-rw-rw-rw-   0        0        0     3481 2023-06-08 08:17:32.000000 pikanetwork.py-1.0.1/pikanetwork/models.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:40:41.343727 pikanetwork.py-1.0.1/pikanetwork.py.egg-info/
+-rw-rw-rw-   0        0        0     3899 2023-06-08 08:40:41.000000 pikanetwork.py-1.0.1/pikanetwork.py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      359 2023-06-08 08:40:41.000000 pikanetwork.py-1.0.1/pikanetwork.py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 08:40:41.000000 pikanetwork.py-1.0.1/pikanetwork.py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 08:40:41.000000 pikanetwork.py-1.0.1/pikanetwork.py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 08:40:41.000000 pikanetwork.py-1.0.1/pikanetwork.py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 08:26:33.000000 pikanetwork.py-1.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 08:40:41.348728 pikanetwork.py-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     2182 2023-06-07 12:58:41.000000 pikanetwork.py-1.0.1/setup.py
```

### Comparing `pikanetwork.py-1.0.0/LICENSE` & `pikanetwork.py-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pikanetwork.py-1.0.0/pikanetwork/builders.py` & `pikanetwork.py-1.0.1/pikanetwork/builders.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from pikanetwork.models import *
 
 
-def build_player(player_data: dict):
+async def build_player(player_data: dict) -> Player:
 
     ranks = []
 
     friends = []
 
     for rank in player_data["ranks"]:
         ranks.append(GameRank(
@@ -27,29 +27,29 @@
     if player_data["clan"] is None:
         clan = None
     else:
         clan_data = player_data["clan"]
 
         members = []
 
-        for index in clan_data["members"]:
-            member_data = clan_data["members"][index]["user"]
+        for member_raw_data in clan_data["members"]:
+            member_data = member_raw_data["user"]
             member = ClanMember(
                 username=member_data["username"],
                 last_seen=member_data["lastSeen"],
                 online=member_data["online"],
-                join_date=clan_data["members"][index]["joinDate"]
+                join_date=member_raw_data["joinDate"]
             )
             members.append(member)
 
         clan = Clan(
             name=clan_data["name"],
             tag=clan_data["tag"],
             current_trophies=clan_data["currentTrophies"],
-            creation_time=clan_data["CreationTime"],
+            creation_time=clan_data["creationTime"],
             members=members,
             owner=ClanOwner(
                 username=clan_data["owner"]["username"],
                 last_seen=clan_data["owner"]["lastSeen"],
                 online=clan_data["owner"]["online"]
             ),
             level=clan_data["leveling"]["level"],
@@ -72,7 +72,10 @@
             percentage=player_data["rank"]["percentage"],
             rank_display=player_data["rank"]["rankDisplay"]
         ),
         friends=friends
     )
 
     return player
+
+async def build_player_leaderboard(leaderboard_data):
+    pass
```

### Comparing `pikanetwork.py-1.0.0/setup.py` & `pikanetwork.py-1.0.1/setup.py`

 * *Files identical despite different names*

