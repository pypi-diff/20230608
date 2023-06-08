# Comparing `tmp/nextguild-1.1.6.tar.gz` & `tmp/nextguild-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nextguild-1.1.6.tar", last modified: Wed Jun  7 18:22:04 2023, max compression
+gzip compressed data, was "nextguild-1.1.7.tar", last modified: Thu Jun  8 18:03:44 2023, max compression
```

## Comparing `nextguild-1.1.6.tar` & `nextguild-1.1.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:22:04.789006 nextguild-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 18:21:54.000000 nextguild-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-07 18:22:04.789006 nextguild-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-07 18:21:54.000000 nextguild-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:22:04.789006 nextguild-1.1.6/nextguild/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/channel.py
--rw-r--r--   0 runner    (1001) docker     (123)    41009 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/embed.py
--rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     2097 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-07 18:21:54.000000 nextguild-1.1.6/nextguild/reaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 18:22:04.789006 nextguild-1.1.6/nextguild.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-07 18:22:04.000000 nextguild-1.1.6/nextguild.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-07 18:22:04.000000 nextguild-1.1.6/nextguild.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 18:22:04.000000 nextguild-1.1.6/nextguild.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 18:22:04.000000 nextguild-1.1.6/nextguild.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-07 18:21:54.000000 nextguild-1.1.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 18:22:04.789006 nextguild-1.1.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:03:44.568209 nextguild-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 18:03:31.000000 nextguild-1.1.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-08 18:03:44.568209 nextguild-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-08 18:03:31.000000 nextguild-1.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:03:44.568209 nextguild-1.1.7/nextguild/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41069 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/embed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42840 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-06-08 18:03:31.000000 nextguild-1.1.7/nextguild/reaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:03:44.568209 nextguild-1.1.7/nextguild.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3158 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:03:44.000000 nextguild-1.1.7/nextguild.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-08 18:03:31.000000 nextguild-1.1.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:03:44.568209 nextguild-1.1.7/setup.cfg
```

### Comparing `nextguild-1.1.6/LICENSE` & `nextguild-1.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.6/PKG-INFO` & `nextguild-1.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.6
+Version: 1.1.7
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.6/README.md` & `nextguild-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.6/nextguild/channel.py` & `nextguild-1.1.7/nextguild/channel.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.6/nextguild/client.py` & `nextguild-1.1.7/nextguild/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,14 +190,16 @@
             group_id: str = None,
             category_id: int = None,
             is_public: bool = False,
             parent_id: str = None,
             message_id: str = None
     ):
         data = {'name': name, 'type': channel_type}
+        if topic:
+            data.update({'topic': topic})
         if category_id:
             data.update({'categoryId': category_id})
         if group_id:
             data.update({'groupId': group_id})
         if server_id:
             data.update({'serverId': server_id})
         if parent_id:
```

### Comparing `nextguild-1.1.6/nextguild/embed.py` & `nextguild-1.1.7/nextguild/embed.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.6/nextguild/events.py` & `nextguild-1.1.7/nextguild/events.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.6/nextguild/message.py` & `nextguild-1.1.7/nextguild/message.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         ))
         # If message is not a response it's empty
         self.reply_message_ids: list[str] = message.get('replyMessageIds', [])
         self.is_private: bool = message.get('isPrivate', False)
         self.is_silent: bool = message.get('isSilent', False)
         # If message has no mentions it's empty
         # TODO Model "mentions" attribute
-        self.mentions = [mention['id'] for mention in message.get('mentions', {}).get('users', [])]
+        self.mentions = message.get('mentions', {})
         self.created_at: str = message.get('createdAt')
         self.author_id: str = message.get('createdBy')
         self.webhook_id: str = message.get('createdByWebhookId')
         self.updated_at: str = message.get('updatedAt')
 
     async def reply(self):  # TODO "reply" method
         pass
```

### Comparing `nextguild-1.1.6/nextguild/reaction.py` & `nextguild-1.1.7/nextguild/reaction.py`

 * *Files identical despite different names*

### Comparing `nextguild-1.1.6/nextguild.egg-info/PKG-INFO` & `nextguild-1.1.7/nextguild.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nextguild
-Version: 1.1.6
+Version: 1.1.7
 Summary: Interactions with the Guilded API made simpler
 Author-email: Arjun Sharda <sharda.aj17@gmail.com>, Erik Thorsell <contact@erikthorsell.com>
 License: MIT License
         
         Copyright (c) 2023 Arjun Sharda
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `nextguild-1.1.6/pyproject.toml` & `nextguild-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "requests", "asyncio", "websockets"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nextguild"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
     { name="Arjun Sharda", email="sharda.aj17@gmail.com" },
     { name="Erik Thorsell", email="contact@erikthorsell.com" },
 ]
 description = "Interactions with the Guilded API made simpler"
 readme = "README.md"
 license = { file="LICENSE" }
```

