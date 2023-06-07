# Comparing `tmp/redoubt_agent-0.1.97.tar.gz` & `tmp/redoubt_agent-0.1.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redoubt_agent-0.1.97.tar", last modified: Mon Jun  5 18:58:13 2023, max compression
+gzip compressed data, was "redoubt_agent-0.1.98.tar", last modified: Wed Jun  7 22:17:02 2023, max compression
```

## Comparing `redoubt_agent-0.1.97.tar` & `redoubt_agent-0.1.98.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:58:13.073222 redoubt_agent-0.1.97/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-05 18:58:03.000000 redoubt_agent-0.1.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 18:58:13.073222 redoubt_agent-0.1.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-05 18:58:03.000000 redoubt_agent-0.1.97/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-05 18:58:03.000000 redoubt_agent-0.1.97/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:58:13.069222 redoubt_agent-0.1.97/redoubt_agent/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-05 18:58:03.000000 redoubt_agent-0.1.97/redoubt_agent/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-05 18:58:03.000000 redoubt_agent-0.1.97/redoubt_agent/redoubt_sdk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 18:58:13.073222 redoubt_agent-0.1.97/redoubt_agent.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-05 18:58:13.000000 redoubt_agent-0.1.97/redoubt_agent.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-05 18:58:13.000000 redoubt_agent-0.1.97/redoubt_agent.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:58:13.000000 redoubt_agent-0.1.97/redoubt_agent.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 18:58:12.000000 redoubt_agent-0.1.97/redoubt_agent.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-05 18:58:13.000000 redoubt_agent-0.1.97/redoubt_agent.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 18:58:13.000000 redoubt_agent-0.1.97/redoubt_agent.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-05 18:58:13.073222 redoubt_agent-0.1.97/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-05 18:58:03.000000 redoubt_agent-0.1.97/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:17:02.919442 redoubt_agent-0.1.98/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-07 22:16:52.000000 redoubt_agent-0.1.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-07 22:17:02.919442 redoubt_agent-0.1.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-06-07 22:16:52.000000 redoubt_agent-0.1.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-07 22:16:52.000000 redoubt_agent-0.1.98/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:17:02.919442 redoubt_agent-0.1.98/redoubt_agent/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-07 22:16:52.000000 redoubt_agent-0.1.98/redoubt_agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-07 22:16:52.000000 redoubt_agent-0.1.98/redoubt_agent/redoubt_sdk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:17:02.919442 redoubt_agent-0.1.98/redoubt_agent.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-06-07 22:17:02.000000 redoubt_agent-0.1.98/redoubt_agent.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-07 22:17:02.000000 redoubt_agent-0.1.98/redoubt_agent.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:17:02.000000 redoubt_agent-0.1.98/redoubt_agent.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:17:02.000000 redoubt_agent-0.1.98/redoubt_agent.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-07 22:17:02.000000 redoubt_agent-0.1.98/redoubt_agent.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 22:17:02.000000 redoubt_agent-0.1.98/redoubt_agent.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-06-07 22:17:02.919442 redoubt_agent-0.1.98/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-07 22:16:52.000000 redoubt_agent-0.1.98/setup.py
```

### Comparing `redoubt_agent-0.1.97/LICENSE` & `redoubt_agent-0.1.98/LICENSE`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.97/PKG-INFO` & `redoubt_agent-0.1.98/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redoubt_agent
-Version: 0.1.97
+Version: 0.1.98
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
```

### Comparing `redoubt_agent-0.1.97/README.md` & `redoubt_agent-0.1.98/README.md`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.97/redoubt_agent/redoubt_sdk.py` & `redoubt_agent-0.1.98/redoubt_agent/redoubt_sdk.py`

 * *Files identical despite different names*

### Comparing `redoubt_agent-0.1.97/redoubt_agent.egg-info/PKG-INFO` & `redoubt_agent-0.1.98/redoubt_agent.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redoubt-agent
-Version: 0.1.97
+Version: 0.1.98
 Summary: re:doubt Bot Python SDK
 Home-page: https://www.redoubt.online/
 Author: maksymds
 Author-email: redoubt@devnull.ae
 License: Apache 2.0
 Project-URL: Github, https://github.com/re-doubt/redoubt-bot-python-sdk
 Project-URL: Documentation, https://docs.redoubt.online/
```

### Comparing `redoubt_agent-0.1.97/setup.cfg` & `redoubt_agent-0.1.98/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = redoubt_agent
-version = 0.1.97
+version = 0.1.98
 description = re:doubt Bot Python SDK
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://www.redoubt.online/
 keywords = TON, redoubt, sdk
 license = Apache 2.0
 classifiers =
```

