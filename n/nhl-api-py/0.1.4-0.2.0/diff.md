# Comparing `tmp/nhl_api_py-0.1.4.tar.gz` & `tmp/nhl_api_py-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhl_api_py-0.1.4.tar", max compression
+gzip compressed data, was "nhl_api_py-0.2.0.tar", max compression
```

## Comparing `nhl_api_py-0.1.4.tar` & `nhl_api_py-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
--rw-r--r--   0        0        0     3702 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/README.md
--rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/__init__.py
--rw-r--r--   0        0        0      311 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/__init__.py
--rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/core.py
--rw-r--r--   0        0        0     2045 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/players.py
--rw-r--r--   0        0        0      561 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/schedule.py
--rw-r--r--   0        0        0     1829 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/standings.py
--rw-r--r--   0        0        0     1999 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/api/teams.py
--rw-r--r--   0        0        0      394 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/nhlpy/nhl_client.py
--rw-r--r--   0        0        0     1257 2023-06-03 14:07:42.805624 nhl_api_py-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 nhl_api_py-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     3702 2023-06-08 18:12:39.049268 nhl_api_py-0.2.0/README.md
+-rw-r--r--   0        0        0       34 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/__init__.py
+-rw-r--r--   0        0        0      743 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/core.py
+-rw-r--r--   0        0        0     4171 2023-06-08 18:58:55.919296 nhl_api_py-0.2.0/nhlpy/api/games.py
+-rw-r--r--   0        0        0     2016 2023-06-08 18:14:40.069269 nhl_api_py-0.2.0/nhlpy/api/players.py
+-rw-r--r--   0        0        0      561 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/schedule.py
+-rw-r--r--   0        0        0     1829 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/standings.py
+-rw-r--r--   0        0        0     1999 2023-06-03 14:07:42.805624 nhl_api_py-0.2.0/nhlpy/api/teams.py
+-rw-r--r--   0        0        0      591 2023-06-08 18:20:08.259272 nhl_api_py-0.2.0/nhlpy/nhl_client.py
+-rw-r--r--   0        0        0     1257 2023-06-08 18:59:37.349297 nhl_api_py-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4734 1970-01-01 00:00:00.000000 nhl_api_py-0.2.0/PKG-INFO
```

### Comparing `nhl_api_py-0.1.4/README.md` & `nhl_api_py-0.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
 
-# NHL-py-api
+# NHL-API-PY
 
-NHL-py-api is a Python package that provides a simple wrapper around the 
+NHL-api-py is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
 
 Note: This is very early, I created this to help me with some machine learning
 projects around the NHL and the NHL data sets.  Special thanks to https://github.com/erunion/sport-api-specifications/tree/master/nhl and https://gitlab.com/dword4/nhlapi/-/blob/master/stats-api.md.
 
 ### Example Notebook:
```

### Comparing `nhl_api_py-0.1.4/nhlpy/api/core.py` & `nhl_api_py-0.2.0/nhlpy/api/core.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.4/nhlpy/api/players.py` & `nhl_api_py-0.2.0/nhlpy/api/players.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from typing import Optional
 from nhlpy.api import BaseNHLAPIClient
 
 
 class Players(BaseNHLAPIClient):
     def get_player(self, person_id: str) -> dict:
         """
         Returns a player based on the person_id.
```

### Comparing `nhl_api_py-0.1.4/nhlpy/api/schedule.py` & `nhl_api_py-0.2.0/nhlpy/api/schedule.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.4/nhlpy/api/standings.py` & `nhl_api_py-0.2.0/nhlpy/api/standings.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.4/nhlpy/api/teams.py` & `nhl_api_py-0.2.0/nhlpy/api/teams.py`

 * *Files identical despite different names*

### Comparing `nhl_api_py-0.1.4/pyproject.toml` & `nhl_api_py-0.2.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "nhl-api-py"
-version = "0.1.4"
+version = "0.2.0"
 description = "NHL API Wrapper.  For standings, team stats and outcomes."
 authors = ["Corey Schaf <cschaf@gmail.com>"]
 readme = "README.md"
 packages = [{include = "nhlpy"}]
 license = "GPL-3.0-or-later"
 homepage = "https://github.com/coreyjs/nhl-api-py"
 repository = "https://github.com/coreyjs/nhl-api-py"
```

### Comparing `nhl_api_py-0.1.4/PKG-INFO` & `nhl_api_py-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nhl-api-py
-Version: 0.1.4
+Version: 0.2.0
 Summary: NHL API Wrapper.  For standings, team stats and outcomes.
 Home-page: https://github.com/coreyjs/nhl-api-py
 License: GPL-3.0-or-later
 Keywords: nhl,api,wrapper,hockey,sports
 Author: Corey Schaf
 Author-email: cschaf@gmail.com
 Requires-Python: >=3.10,<4.0
@@ -20,17 +20,17 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: httpx
 Project-URL: Repository, https://github.com/coreyjs/nhl-api-py
 Description-Content-Type: text/markdown
 
 [![PyPI version](https://badge.fury.io/py/nhl-api-py.svg)](https://badge.fury.io/py/nhl-api-py)
 
-# NHL-py-api
+# NHL-API-PY
 
-NHL-py-api is a Python package that provides a simple wrapper around the 
+NHL-api-py is a Python package that provides a simple wrapper around the 
 NHL API, allowing you to easily access and retrieve NHL data in your Python 
 applications.
 
 Note: This is very early, I created this to help me with some machine learning
 projects around the NHL and the NHL data sets.  Special thanks to https://github.com/erunion/sport-api-specifications/tree/master/nhl and https://gitlab.com/dword4/nhlapi/-/blob/master/stats-api.md.
 
 ### Example Notebook:
```

