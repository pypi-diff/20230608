# Comparing `tmp/tonie_podcast_sync-1.0.1.tar.gz` & `tmp/tonie_podcast_sync-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tonie_podcast_sync-1.0.1.tar", max compression
+gzip compressed data, was "tonie_podcast_sync-1.0.2.tar", max compression
```

## Comparing `tonie_podcast_sync-1.0.1.tar` & `tonie_podcast_sync-1.0.2.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0     1075 2021-04-07 13:07:15.534092 tonie_podcast_sync-1.0.1/LICENSE
--rw-r--r--   0        0        0     2500 2022-11-02 13:03:23.640700 tonie_podcast_sync-1.0.1/README.md
--rw-r--r--   0        0        0     2358 2022-11-01 20:14:50.320861 tonie_podcast_sync-1.0.1/podcast.py
--rw-r--r--   0        0        0      705 2022-11-02 13:07:12.165861 tonie_podcast_sync-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       34 2022-11-02 10:57:56.896161 tonie_podcast_sync-1.0.1/tonie_api/.git
--rw-r--r--   0        0        0     1799 2022-11-02 10:57:56.914079 tonie_podcast_sync-1.0.1/tonie_api/.gitignore
--rw-r--r--   0        0        0     1066 2022-11-02 10:57:56.914373 tonie_podcast_sync-1.0.1/tonie_api/LICENSE
--rw-r--r--   0        0        0      188 2022-11-02 10:57:56.914623 tonie_podcast_sync-1.0.1/tonie_api/README.md
--rw-r--r--   0        0        0     1883 2022-11-02 10:57:56.915018 tonie_podcast_sync-1.0.1/tonie_api/docs/Introduction.rst
--rw-r--r--   0        0        0     1257 2022-11-02 10:57:56.915276 tonie_podcast_sync-1.0.1/tonie_api/docs/api.rst
--rwxr-xr-x   0        0        0     9023 2022-11-02 10:57:56.915593 tonie_podcast_sync-1.0.1/tonie_api/docs/conf.py
--rw-r--r--   0        0        0      210 2022-11-02 10:57:56.915865 tonie_podcast_sync-1.0.1/tonie_api/docs/index.rst
--rwxr-xr-x   0        0        0      503 2022-11-02 10:57:56.916111 tonie_podcast_sync-1.0.1/tonie_api/setup.py
--rwxr-xr-x   0        0        0       25 2022-11-02 10:57:56.916480 tonie_podcast_sync-1.0.1/tonie_api/tonie_api/__init__.py
--rw-r--r--   0        0        0      208 2022-11-02 10:59:43.746185 tonie_podcast_sync-1.0.1/tonie_api/tonie_api/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0    13507 2022-11-02 10:59:43.750528 tonie_podcast_sync-1.0.1/tonie_api/tonie_api/__pycache__/api.cpython-310.pyc
--rwxr-xr-x   0        0        0    14719 2022-11-02 10:57:56.916832 tonie_podcast_sync-1.0.1/tonie_api/tonie_api/api.py
--rw-r--r--   0        0        0      326 2022-11-02 10:59:34.401193 tonie_podcast_sync-1.0.1/tonie_api/tonie_api.egg-info/PKG-INFO
--rw-r--r--   0        0        0      261 2022-11-02 10:59:34.412315 tonie_podcast_sync-1.0.1/tonie_api/tonie_api.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2022-11-02 10:59:34.401903 tonie_podcast_sync-1.0.1/tonie_api/tonie_api.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2022-11-02 10:59:34.401557 tonie_podcast_sync-1.0.1/tonie_api/tonie_api.egg-info/not-zip-safe
--rw-r--r--   0        0        0       27 2022-11-02 10:59:34.402632 tonie_podcast_sync-1.0.1/tonie_api/tonie_api.egg-info/requires.txt
--rw-r--r--   0        0        0       10 2022-11-02 10:59:34.403016 tonie_podcast_sync-1.0.1/tonie_api/tonie_api.egg-info/top_level.txt
--rw-r--r--   0        0        0     7249 2022-11-02 11:10:22.488998 tonie_podcast_sync-1.0.1/toniepodcastsync.py
--rw-r--r--   0        0        0     3567 1970-01-01 00:00:00.000000 tonie_podcast_sync-1.0.1/setup.py
--rw-r--r--   0        0        0     3377 1970-01-01 00:00:00.000000 tonie_podcast_sync-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2021-04-07 13:07:15.000000 tonie_podcast_sync-1.0.2/LICENSE
+-rw-r--r--   0        0        0     2868 2023-01-15 13:03:54.000000 tonie_podcast_sync-1.0.2/README.md
+-rw-r--r--   0        0        0     2358 2022-11-01 20:14:50.000000 tonie_podcast_sync-1.0.2/podcast.py
+-rw-r--r--   0        0        0      719 2023-06-08 10:42:23.487638 tonie_podcast_sync-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/.git
+-rw-r--r--   0        0        0     1799 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/.gitignore
+-rw-r--r--   0        0        0     1066 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/LICENSE
+-rw-r--r--   0        0        0      188 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/README.md
+-rw-r--r--   0        0        0     1883 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/docs/Introduction.rst
+-rw-r--r--   0        0        0     1257 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/docs/api.rst
+-rwxr-xr-x   0        0        0     9023 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/docs/conf.py
+-rw-r--r--   0        0        0      210 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/docs/index.rst
+-rwxr-xr-x   0        0        0      503 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/setup.py
+-rwxr-xr-x   0        0        0       25 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api/__init__.py
+-rw-r--r--   0        0        0      208 2022-11-02 10:59:43.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    13507 2022-11-02 10:59:43.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api/__pycache__/api.cpython-310.pyc
+-rwxr-xr-x   0        0        0    14719 2022-11-02 10:57:56.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api/api.py
+-rw-r--r--   0        0        0      326 2022-11-02 10:59:34.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api.egg-info/PKG-INFO
+-rw-r--r--   0        0        0      261 2022-11-02 10:59:34.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api.egg-info/SOURCES.txt
+-rw-r--r--   0        0        0        1 2022-11-02 10:59:34.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api.egg-info/dependency_links.txt
+-rw-r--r--   0        0        0        1 2022-11-02 10:59:34.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api.egg-info/not-zip-safe
+-rw-r--r--   0        0        0       27 2022-11-02 10:59:34.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api.egg-info/requires.txt
+-rw-r--r--   0        0        0       10 2022-11-02 10:59:34.000000 tonie_podcast_sync-1.0.2/tonie_api/tonie_api.egg-info/top_level.txt
+-rw-r--r--   0        0        0     7249 2022-11-02 11:10:22.000000 tonie_podcast_sync-1.0.2/toniepodcastsync.py
+-rw-r--r--   0        0        0     3782 1970-01-01 00:00:00.000000 tonie_podcast_sync-1.0.2/PKG-INFO
```

### Comparing `tonie_podcast_sync-1.0.1/LICENSE` & `tonie_podcast_sync-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/README.md` & `tonie_podcast_sync-1.0.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -4,15 +4,18 @@
 
 This is a purely private project and has no association with Boxine GmbH.
 
 # Constraints and Limitations
 
 - currently limited to podcasts providing mp3 files
 - tested with the following podcasts:
-    - [WDR: Gute Nacht mit der Maus](https://www.wdrmaus.de/hoeren/gute_nacht_mit_der_maus.php5)
+    - WDR [Maus Podcasts](https://www.wdrmaus.de/hoeren/MausLive/Podcasts/podcasts.php5), e.g. 
+        - [Gute Nacht mit der Maus](https://kinder.wdr.de/radio/diemaus/audio/gute-nacht-mit-der-maus/diemaus-gute-nacht-104.podcast)
+        - [Maus zum Hören - 60 Minuten](https://kinder.wdr.de/radio/diemaus/audio/diemaus-60/diemaus-60-106.podcast)
+        - [Maus Zoom - Kindernachrichten](https://kinder.wdr.de/radio/diemaus/audio/maus-zoom/maus-zoom-106.podcast)
     - [Bayern 2: Pumuckl - Der Hörspiel-Klassiker](https://www.br.de/mediathek/podcast/pumuckl/830)
     - [Checker Tobi Podcast](https://www.br.de/mediathek/podcast/checkpod-der-podcast-mit-checker-tobi/859)
     - [Anna und die wilden Tiere - der Podcast](https://www.br.de/mediathek/podcast/anna-und-die-wilden-tiere/858)
 - ... but in general, it should hopefully work with all podcasts out there
 
 # Usage
```

### Comparing `tonie_podcast_sync-1.0.1/podcast.py` & `tonie_podcast_sync-1.0.2/podcast.py`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/pyproject.toml` & `tonie_podcast_sync-1.0.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tonie-podcast-sync"
-version = "1.0.1"
+version = "1.0.2"
 description = "allows synching podcast episodes to creative tonies"
 authors = ["Alexander Hartmann <16985220+alexhartm@users.noreply.github.com>"]
 repository = "https://github.com/alexhartm/tonie-podcast-sync"
 readme = "README.md"
 license = "MIT"
 keywords = ["toniebox", "podcast"]
 packages = [
@@ -17,11 +17,12 @@
 [tool.poetry.dependencies]
 python = "^3.9.2"
 wget = "^3.2"
 requests = "^2.25.1"
 requests-oauthlib = "^1.3.0"
 beautifulsoup4 = "^4.10.0"
 config-with-yaml = "^0.1.0"
+lxml="^4.9.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/.gitignore` & `tonie_podcast_sync-1.0.2/tonie_api/.gitignore`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/LICENSE` & `tonie_podcast_sync-1.0.2/tonie_api/LICENSE`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/docs/Introduction.rst` & `tonie_podcast_sync-1.0.2/tonie_api/docs/Introduction.rst`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/docs/api.rst` & `tonie_podcast_sync-1.0.2/tonie_api/docs/api.rst`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/docs/conf.py` & `tonie_podcast_sync-1.0.2/tonie_api/docs/conf.py`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/tonie_api/__pycache__/api.cpython-310.pyc` & `tonie_podcast_sync-1.0.2/tonie_api/tonie_api/__pycache__/api.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/tonie_api/tonie_api/api.py` & `tonie_podcast_sync-1.0.2/tonie_api/tonie_api/api.py`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/toniepodcastsync.py` & `tonie_podcast_sync-1.0.2/toniepodcastsync.py`

 * *Files identical despite different names*

### Comparing `tonie_podcast_sync-1.0.1/setup.py` & `tonie_podcast_sync-1.0.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,85 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
-
-packages = \
-['tonie_api', 'tonie_api.docs', 'tonie_api.tonie_api']
-
-package_data = \
-{'': ['*'], 'tonie_api': ['tonie_api.egg-info/*']}
-
-modules = \
-['toniepodcastsync', 'podcast']
-install_requires = \
-['beautifulsoup4>=4.10.0,<5.0.0',
- 'config-with-yaml>=0.1.0,<0.2.0',
- 'requests-oauthlib>=1.3.0,<2.0.0',
- 'requests>=2.25.1,<3.0.0',
- 'wget>=3.2,<4.0']
-
-setup_kwargs = {
-    'name': 'tonie-podcast-sync',
-    'version': '1.0.1',
-    'description': 'allows synching podcast episodes to creative tonies',
-    'long_description': '# tonie-podcast-sync\n\ntonie-podcast-sync allows synching podcast episodes to [creative tonies](https://tonies.com).\n\nThis is a purely private project and has no association with Boxine GmbH.\n\n# Constraints and Limitations\n\n- currently limited to podcasts providing mp3 files\n- tested with the following podcasts:\n    - [WDR: Gute Nacht mit der Maus](https://www.wdrmaus.de/hoeren/gute_nacht_mit_der_maus.php5)\n    - [Bayern 2: Pumuckl - Der Hörspiel-Klassiker](https://www.br.de/mediathek/podcast/pumuckl/830)\n    - [Checker Tobi Podcast](https://www.br.de/mediathek/podcast/checkpod-der-podcast-mit-checker-tobi/859)\n    - [Anna und die wilden Tiere - der Podcast](https://www.br.de/mediathek/podcast/anna-und-die-wilden-tiere/858)\n- ... but in general, it should hopefully work with all podcasts out there\n\n# Usage\n\ntonie-podcast-sync is available as [a pip package on pypi](https://pypi.org/project/tonie-podcast-sync). Install via\n\n`pip install tonie-podcast-sync`\n\nThen, use it as shown in the following example code:\n\n```python\nfrom toniepodcastsync import ToniePodcastSync, Podcast\n\n# create two Podcast objects, providing the feed URL to each\npumuckl = Podcast("https://feeds.br.de/pumuckl/feed.xml")\nmaus = Podcast("https://kinder.wdr.de/radio/diemaus/audio/gute-nacht-mit-der-maus/diemaus-gute-nacht-104.podcast")\n\n# create instance of ToniePodcastSync\ntps = ToniePodcastSync("<toniecloud-username>", "<toniecloud-password>")\n\n# for an overview of your creative tonies and their IDs\ntps.printToniesOverview()\n\n# define creative tonies based on their ID\ngreenTonie = "<your-tonieID>"\norangeTonie = "<your-tonieID>"\n\n# Fetch new podcast episodes and copy them to greenTonie.\n# The tonie will be filled with as much episodes as fit (90 min max).\n# Episode are ordered with newest first.\ntps.syncPodcast2Tonie(pumuckl, greenTonie)\n\n# Kid\'s should fall asleep, so let\'s limit the podcast \n# episodes on this tonie to 60 minutes in total.\n# Use the optional parameter for this:\ntps.syncPodcast2Tonie(maus, orangeTonie, 60)  \n```\n\nFor the tonie to fetch new content from tonie-cloud, you have to press one ear for 3s (until the "ping" sound) with no tonie on the box (refer also to TonieBox manual).\n\n\n# builds upon work of / kudos to\n- moritj29\'s awesome [tonie_api](https://github.com/moritzj29/tonie_api)\n- [Tobias Raabe](https://tobiasraabe.github.io/blog/how-to-download-files-with-python.html)\n- [Matthew Wimberly](https://codeburst.io/building-an-rss-feed-scraper-with-python-73715ca06e1f)',
-    'author': 'Alexander Hartmann',
-    'author_email': '16985220+alexhartm@users.noreply.github.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/alexhartm/tonie-podcast-sync',
-    'packages': packages,
-    'package_data': package_data,
-    'py_modules': modules,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9.2,<4.0.0',
-}
-
-
-setup(**setup_kwargs)
+Metadata-Version: 2.1
+Name: tonie-podcast-sync
+Version: 1.0.2
+Summary: allows synching podcast episodes to creative tonies
+Home-page: https://github.com/alexhartm/tonie-podcast-sync
+License: MIT
+Keywords: toniebox,podcast
+Author: Alexander Hartmann
+Author-email: 16985220+alexhartm@users.noreply.github.com
+Requires-Python: >=3.9.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: beautifulsoup4 (>=4.10.0,<5.0.0)
+Requires-Dist: config-with-yaml (>=0.1.0,<0.2.0)
+Requires-Dist: lxml (>=4.9.2,<5.0.0)
+Requires-Dist: requests (>=2.25.1,<3.0.0)
+Requires-Dist: requests-oauthlib (>=1.3.0,<2.0.0)
+Requires-Dist: wget (>=3.2,<4.0)
+Project-URL: Repository, https://github.com/alexhartm/tonie-podcast-sync
+Description-Content-Type: text/markdown
+
+# tonie-podcast-sync
+
+tonie-podcast-sync allows synching podcast episodes to [creative tonies](https://tonies.com).
+
+This is a purely private project and has no association with Boxine GmbH.
+
+# Constraints and Limitations
+
+- currently limited to podcasts providing mp3 files
+- tested with the following podcasts:
+    - WDR [Maus Podcasts](https://www.wdrmaus.de/hoeren/MausLive/Podcasts/podcasts.php5), e.g. 
+        - [Gute Nacht mit der Maus](https://kinder.wdr.de/radio/diemaus/audio/gute-nacht-mit-der-maus/diemaus-gute-nacht-104.podcast)
+        - [Maus zum Hören - 60 Minuten](https://kinder.wdr.de/radio/diemaus/audio/diemaus-60/diemaus-60-106.podcast)
+        - [Maus Zoom - Kindernachrichten](https://kinder.wdr.de/radio/diemaus/audio/maus-zoom/maus-zoom-106.podcast)
+    - [Bayern 2: Pumuckl - Der Hörspiel-Klassiker](https://www.br.de/mediathek/podcast/pumuckl/830)
+    - [Checker Tobi Podcast](https://www.br.de/mediathek/podcast/checkpod-der-podcast-mit-checker-tobi/859)
+    - [Anna und die wilden Tiere - der Podcast](https://www.br.de/mediathek/podcast/anna-und-die-wilden-tiere/858)
+- ... but in general, it should hopefully work with all podcasts out there
+
+# Usage
+
+tonie-podcast-sync is available as [a pip package on pypi](https://pypi.org/project/tonie-podcast-sync). Install via
+
+`pip install tonie-podcast-sync`
+
+Then, use it as shown in the following example code:
+
+```python
+from toniepodcastsync import ToniePodcastSync, Podcast
+
+# create two Podcast objects, providing the feed URL to each
+pumuckl = Podcast("https://feeds.br.de/pumuckl/feed.xml")
+maus = Podcast("https://kinder.wdr.de/radio/diemaus/audio/gute-nacht-mit-der-maus/diemaus-gute-nacht-104.podcast")
+
+# create instance of ToniePodcastSync
+tps = ToniePodcastSync("<toniecloud-username>", "<toniecloud-password>")
+
+# for an overview of your creative tonies and their IDs
+tps.printToniesOverview()
+
+# define creative tonies based on their ID
+greenTonie = "<your-tonieID>"
+orangeTonie = "<your-tonieID>"
+
+# Fetch new podcast episodes and copy them to greenTonie.
+# The tonie will be filled with as much episodes as fit (90 min max).
+# Episode are ordered with newest first.
+tps.syncPodcast2Tonie(pumuckl, greenTonie)
+
+# Kid's should fall asleep, so let's limit the podcast 
+# episodes on this tonie to 60 minutes in total.
+# Use the optional parameter for this:
+tps.syncPodcast2Tonie(maus, orangeTonie, 60)  
+```
+
+For the tonie to fetch new content from tonie-cloud, you have to press one ear for 3s (until the "ping" sound) with no tonie on the box (refer also to TonieBox manual).
+
+
+# builds upon work of / kudos to
+- moritj29's awesome [tonie_api](https://github.com/moritzj29/tonie_api)
+- [Tobias Raabe](https://tobiasraabe.github.io/blog/how-to-download-files-with-python.html)
+- [Matthew Wimberly](https://codeburst.io/building-an-rss-feed-scraper-with-python-73715ca06e1f)
```

