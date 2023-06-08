# Comparing `tmp/cgsubmit-1.0.5.tar.gz` & `tmp/cgsubmit-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cgsubmit-1.0.5.tar", last modified: Wed Jun  7 20:05:48 2023, max compression
+gzip compressed data, was "cgsubmit-1.0.6.tar", last modified: Thu Jun  8 18:54:07 2023, max compression
```

## Comparing `cgsubmit-1.0.5.tar` & `cgsubmit-1.0.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/cgsubmit/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/cgsubmit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/cgsubmit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/cgsubmit/api/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/cgsubmit/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/cgsubmit/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/cgsubmit/games/
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/cgsubmit/games/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/cgsubmit/games/games.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/cgsubmit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-07 20:05:47.000000 cgsubmit-1.0.5/cgsubmit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-07 20:05:47.000000 cgsubmit-1.0.5/cgsubmit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:05:47.000000 cgsubmit-1.0.5/cgsubmit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 20:05:47.000000 cgsubmit-1.0.5/cgsubmit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 20:05:47.000000 cgsubmit-1.0.5/cgsubmit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 20:05:47.999079 cgsubmit-1.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-07 20:05:31.000000 cgsubmit-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2220 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/cgsubmit/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/cgsubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/cgsubmit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/cgsubmit/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/cgsubmit/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/cgsubmit/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/cgsubmit/games/
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/cgsubmit/games/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/cgsubmit/games/games.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/cgsubmit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3298 2023-06-08 18:54:07.000000 cgsubmit-1.0.6/cgsubmit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-06-08 18:54:07.000000 cgsubmit-1.0.6/cgsubmit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:54:07.000000 cgsubmit-1.0.6/cgsubmit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 18:54:07.000000 cgsubmit-1.0.6/cgsubmit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 18:54:07.000000 cgsubmit-1.0.6/cgsubmit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:54:07.325505 cgsubmit-1.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-06-08 18:53:49.000000 cgsubmit-1.0.6/setup.py
```

### Comparing `cgsubmit-1.0.5/LICENSE` & `cgsubmit-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.5/PKG-INFO` & `cgsubmit-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgsubmit-1.0.5/README.md` & `cgsubmit-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.5/cgsubmit/__main__.py` & `cgsubmit-1.0.6/cgsubmit/__main__.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.5/cgsubmit/api/api.py` & `cgsubmit-1.0.6/cgsubmit/api/api.py`

 * *Files identical despite different names*

### Comparing `cgsubmit-1.0.5/cgsubmit/games/games.py` & `cgsubmit-1.0.6/cgsubmit/games/games.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,14 +7,17 @@
     
     def find_pseudo(self, games) -> str:
         player1 = ''
         player2 = ''
 
         i = 0
         while i < len(games):
+            if len(games[i]['players']) <= 1:
+                i = i + 1
+                continue
             if player1 == '':
                 player1 = games[i]['players'][0]['nickname']
                 player2 = games[i]['players'][1]['nickname']
             else:
                 if player1 == games[i]['players'][0]['nickname'] and player2 != games[i]['players'][1]['nickname'] or \
                     player1 == games[i]['players'][1]['nickname'] and player2 != games[i]['players'][0]['nickname']:
                     return player1
```

### Comparing `cgsubmit-1.0.5/cgsubmit.egg-info/PKG-INFO` & `cgsubmit-1.0.6/cgsubmit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cgsubmit
-Version: 1.0.5
+Version: 1.0.6
 Summary: Analyse your submit in codingame competitions.
 Home-page: https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Author: FrequentlyMissedDeadlines
 Author-email: FrequentlyMissedDeadlines+cgsubmit@gmail.com
 Project-URL: Bug Reports, https://github.com/FrequentlyMissedDeadlines/cgsubmit/issues
 Project-URL: Source, https://github.com/FrequentlyMissedDeadlines/cgsubmit
 Classifier: Programming Language :: Python :: 3
```

### Comparing `cgsubmit-1.0.5/setup.py` & `cgsubmit-1.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 README_MD = open(join(dirname(abspath(__file__)), "README.md")).read()
 
 with open('requirements.txt') as f:
     required = f.read().splitlines()
 
 setup(
     name="cgsubmit",
-    version="1.0.5",
+    version="1.0.6",
     packages=find_namespace_packages(include=['cgsubmit', 'cgsubmit.*'], exclude=['*.tests*']),
     description="Analyse your submit in codingame competitions.",
     long_description=README_MD,
     long_description_content_type="text/markdown",
     url="https://github.com/FrequentlyMissedDeadlines/cgsubmit",
     author="FrequentlyMissedDeadlines",
     author_email="FrequentlyMissedDeadlines+cgsubmit@gmail.com",
```

