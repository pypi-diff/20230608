# Comparing `tmp/duckduckgo_search-3.8.1.tar.gz` & `tmp/duckduckgo_search-3.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duckduckgo_search-3.8.1.tar", last modified: Sat Jun  3 07:39:55 2023, max compression
+gzip compressed data, was "duckduckgo_search-3.8.2.tar", last modified: Thu Jun  8 08:22:30 2023, max compression
```

## Comparing `duckduckgo_search-3.8.1.tar` & `duckduckgo_search-3.8.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)    14025 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.760635 duckduckgo_search-3.8.1/duckduckgo_search/
--rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16380 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    31788 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/duckduckgo_search.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/duckduckgo_search/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15140 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-03 07:39:55.000000 duckduckgo_search-3.8.1/duckduckgo_search.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 07:39:55.764635 duckduckgo_search-3.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-03 07:39:41.000000 duckduckgo_search-3.8.1/tests/test_duckduckgo_search.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1063 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14271 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/duckduckgo_search/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      607 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      138 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16474 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31995 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/duckduckgo_search.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       22 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/duckduckgo_search/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15386 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 08:22:30.000000 duckduckgo_search-3.8.2/duckduckgo_search.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:22:30.439219 duckduckgo_search-3.8.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4633 2023-06-08 08:22:15.000000 duckduckgo_search-3.8.2/tests/test_duckduckgo_search.py
```

### Comparing `duckduckgo_search-3.8.1/LICENSE.md` & `duckduckgo_search-3.8.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.1/PKG-INFO` & `duckduckgo_search-3.8.2/duckduckgo_search.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo_search
-Version: 3.8.1
+Name: duckduckgo-search
+Version: 3.8.2
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -68,14 +68,16 @@
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
 # find and download any xls files from a specific site
 ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
+# get last day's news and save it to a csv file
+ddgs news -k "hubble telescope" -t d -m 50 -o csv
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
@@ -199,15 +201,15 @@
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     backend: str = "api",
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
@@ -244,15 +246,15 @@
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
 ```python
-def answers(keywords: str) -> Generator[dict, None, None]:
+def answers(keywords: str) -> Iterator[Dict[str, Optional[str]]]::
     """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
 
     Yields:
         dict with instant answers results.
@@ -279,15 +281,15 @@
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     size: Optional[str] = None,
     color: Optional[str] = None,
     type_image: Optional[str] = None,
     layout: Optional[str] = None,
     license_image: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: Day, Week, Month, Year. Defaults to None.
@@ -336,15 +338,15 @@
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     resolution: Optional[str] = None,
     duration: Optional[str] = None,
     license_videos: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -382,15 +384,15 @@
 
 ```python
 def news(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -429,15 +431,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -470,15 +472,15 @@
 
 ```python
 def translate(
     self,
     keywords: str,
     from_: Optional[str] = None,
     to: str = "en",
-) -> Optional[dict]:
+) -> Optional[Dict[str, Optional[str]]]:
     """DuckDuckGo translate
 
     Args:
         keywords: string or a list of strings to translate
         from_: translate from (defaults automatically). Defaults to None.
         to: what language to translate. Defaults to "en".
 
@@ -501,15 +503,15 @@
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
 def suggestions(
     keywords,
     region: str = "wt-wt",
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
     Yields:
```

### Comparing `duckduckgo_search-3.8.1/README.md` & `duckduckgo_search-3.8.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,16 @@
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
 # find and download any xls files from a specific site
 ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
+# get last day's news and save it to a csv file
+ddgs news -k "hubble telescope" -t d -m 50 -o csv
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
@@ -174,15 +176,15 @@
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     backend: str = "api",
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
@@ -219,15 +221,15 @@
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
 ```python
-def answers(keywords: str) -> Generator[dict, None, None]:
+def answers(keywords: str) -> Iterator[Dict[str, Optional[str]]]::
     """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
 
     Yields:
         dict with instant answers results.
@@ -254,15 +256,15 @@
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     size: Optional[str] = None,
     color: Optional[str] = None,
     type_image: Optional[str] = None,
     layout: Optional[str] = None,
     license_image: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: Day, Week, Month, Year. Defaults to None.
@@ -311,15 +313,15 @@
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     resolution: Optional[str] = None,
     duration: Optional[str] = None,
     license_videos: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -357,15 +359,15 @@
 
 ```python
 def news(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -404,15 +406,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -445,15 +447,15 @@
 
 ```python
 def translate(
     self,
     keywords: str,
     from_: Optional[str] = None,
     to: str = "en",
-) -> Optional[dict]:
+) -> Optional[Dict[str, Optional[str]]]:
     """DuckDuckGo translate
 
     Args:
         keywords: string or a list of strings to translate
         from_: translate from (defaults automatically). Defaults to None.
         to: what language to translate. Defaults to "en".
 
@@ -476,15 +478,15 @@
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
 def suggestions(
     keywords,
     region: str = "wt-wt",
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
     Yields:
```

### Comparing `duckduckgo_search-3.8.1/duckduckgo_search/__init__.py` & `duckduckgo_search-3.8.2/duckduckgo_search/__init__.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.1/duckduckgo_search/cli.py` & `duckduckgo_search-3.8.2/duckduckgo_search/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import json
 import logging
 import os
 from datetime import datetime
 from random import choice
 from urllib.parse import unquote
 
+import aiofiles
 import click
 import httpx
 
 from .duckduckgo_search import DDGS, USERAGENTS
 from .version import __version__
 
 logger = logging.getLogger(__name__)
@@ -46,15 +47,15 @@
             writer.writeheader()
             writer.writerows(data)
 
 
 def print_data(data):
     if data:
         for i, e in enumerate(data, start=1):
-            click.secho(f"{i}. {'-' * 78}", bg="black", fg="white")
+            click.secho(f"{i}.\t    {'=' * 78}", bg="black", fg="white")
             for j, (k, v) in enumerate(e.items(), start=1):
                 if v:
                     width = (
                         300
                         if k
                         in (
                             "content",
@@ -94,20 +95,22 @@
     return keywords
 
 
 async def download_file(url, dir_path, filename, sem):
     headers = {"User-Agent": choice(USERAGENTS)}
     try:
         async with sem:
-            async with httpx.AsyncClient() as client:
-                async with client.stream("GET", url, headers=headers) as resp:
+            async with httpx.AsyncClient(headers=headers) as client:
+                async with client.stream("GET", url) as resp:
                     if resp.status_code == 200:
-                        with open(os.path.join(dir_path, filename), "wb") as file:
+                        async with aiofiles.open(
+                            os.path.join(dir_path, filename), "wb"
+                        ) as file:
                             async for chunk in resp.aiter_bytes():
-                                file.write(chunk)
+                                await file.write(chunk)
                 logger.info(f"File downloaded {url}")
     except Exception as ex:
         logger.debug(f"download_file url={url} {type(ex).__name__} {ex}")
 
 
 async def _download_results(keywords, results, images=False):
     if images:
```

### Comparing `duckduckgo_search-3.8.1/duckduckgo_search/compat.py` & `duckduckgo_search-3.8.2/duckduckgo_search/compat.py`

 * *Files identical despite different names*

### Comparing `duckduckgo_search-3.8.1/duckduckgo_search/duckduckgo_search.py` & `duckduckgo_search-3.8.2/duckduckgo_search/duckduckgo_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from dataclasses import dataclass
 from datetime import datetime
 from decimal import Decimal
 from html import unescape
 from itertools import cycle
 from random import choice
 from time import sleep
-from typing import Deque, Dict, Iterator, Optional, Set, Union
+from typing import Deque, Dict, Iterator, Optional, Set, Tuple
 from urllib.parse import unquote
 
 import httpx
 from lxml import html
 
 logger = logging.getLogger(__name__)
 
@@ -36,42 +36,42 @@
     longitude: Optional[str] = None
     url: Optional[str] = None
     desc: Optional[str] = None
     phone: Optional[str] = None
     image: Optional[str] = None
     source: Optional[str] = None
     links: Optional[str] = None
-    hours: Optional[Dict] = None
+    hours: Optional[Dict[str, str]] = None
 
 
 class DDGS:
     """DuckDuckgo_search class to get search results from duckduckgo.com"""
 
     def __init__(
         self,
-        headers: Optional[Dict[str, str]] = None,
-        proxies: Optional[Union[Dict, str]] = None,
-        timeout: int = 10,
+        headers=None,
+        proxies=None,
+        timeout=10,
     ) -> None:
         if headers is None:
             headers = {
                 "User-Agent": choice(USERAGENTS),
                 "Referer": "https://duckduckgo.com/",
             }
         self._client = httpx.Client(
             headers=headers,
             proxies=proxies,
             timeout=timeout,
             http2=True,
         )
 
-    def __enter__(self):
+    def __enter__(self) -> "DDGS":
         return self
 
-    def __exit__(self, exc_type, exc_val, exc_tb):
+    def __exit__(self, exc_type, exc_val, exc_tb) -> None:
         self._client.close()
 
     def _get_url(
         self, method: str, url: str, **kwargs
     ) -> Optional[httpx._models.Response]:
         for i in range(3):
             try:
@@ -115,24 +115,26 @@
         """strip HTML tags"""
         if raw_html:
             return unescape(re.sub(REGEX_STRIP_TAGS, "", raw_html))
         return ""
 
     def _normalize_url(self, url: str) -> str:
         """unquote url and replace spaces with '+'"""
-        return unquote(url).replace(" ", "+")
+        if url:
+            return unquote(url).replace(" ", "+")
+        return ""
 
     def text(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         backend: str = "api",
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
@@ -153,15 +155,15 @@
 
     def _text_api(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
@@ -170,15 +172,14 @@
             dict with search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         assert vqd, "error in getting vqd"
-        sleep(0.75)
 
         payload = {
             "q": keywords,  #
             "kl": region,
             "l": region,
             "s": 0,
             "df": timelimit,
@@ -222,26 +223,26 @@
                     cache.add(href)
                     body = self._normalize(row["a"])
                     if body:
                         result_exists = True
                         yield {
                             "title": self._normalize(row["t"]),
                             "href": self._normalize_url(href),
-                            "body": self._normalize(body),
+                            "body": body,
                         }
             if result_exists is False:
                 break
 
     def _text_html(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m, y. Defaults to None.
@@ -301,15 +302,15 @@
             sleep(0.75)
 
     def _text_lite(
         self,
         keywords: str,
         region: str = "wt-wt",
         timelimit: Optional[str] = None,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             timelimit: d, w, m, y. Defaults to None.
 
@@ -372,15 +373,15 @@
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         size: Optional[str] = None,
         color: Optional[str] = None,
         type_image: Optional[str] = None,
         layout: Optional[str] = None,
         license_image: Optional[str] = None,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: Day, Week, Month, Year. Defaults to None.
@@ -399,15 +400,14 @@
             dict with image search results.
 
         """
         assert keywords, "keywords is mandatory"
 
         vqd = self._get_vqd(keywords)
         assert vqd, "error in getting vqd"
-        sleep(0.75)
 
         safesearch_base = {"on": 1, "moderate": 1, "off": -1}
         timelimit = f"time:{timelimit}" if timelimit else ""
         size = f"size:{size}" if size else ""
         color = f"color:{color}" if color else ""
         type_image = f"type:{type_image}" if type_image else ""
         layout = f"layout:{layout}" if layout else ""
@@ -461,15 +461,15 @@
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
         resolution: Optional[str] = None,
         duration: Optional[str] = None,
         license_videos: Optional[str] = None,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
@@ -528,15 +528,15 @@
 
     def news(
         self,
         keywords: str,
         region: str = "wt-wt",
         safesearch: str = "moderate",
         timelimit: Optional[str] = None,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
             safesearch: on, moderate, off. Defaults to "moderate".
             timelimit: d, w, m. Defaults to None.
@@ -596,15 +596,15 @@
                 payload["s"] = next.split("s=")[-1].split("&")[0]
             if not result_exists or not next:
                 break
 
     def answers(
         self,
         keywords: str,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
 
         Yields:
             dict with instant answers results.
@@ -670,15 +670,15 @@
                             "url": subrow["FirstURL"],
                         }
 
     def suggestions(
         self,
         keywords: str,
         region: str = "wt-wt",
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query.
             region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
         Yields:
@@ -710,15 +710,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -787,15 +787,15 @@
         lat_t += Decimal(radius) * Decimal(0.008983)
         lat_b -= Decimal(radius) * Decimal(0.008983)
         lon_l -= Decimal(radius) * Decimal(0.008983)
         lon_r += Decimal(radius) * Decimal(0.008983)
         logging.debug(f"bbox coordinates\n{lat_t} {lon_l}\n{lat_b} {lon_r}")
 
         # сreate a queue of search squares (bboxes)
-        work_bboxes: Deque = deque()
+        work_bboxes: Deque[Tuple[Decimal, Decimal, Decimal, Decimal]] = deque()
         work_bboxes.append((lat_t, lon_l, lat_b, lon_r))
 
         # bbox iterate
         cache = set()
         stop_find = False
         while work_bboxes and not stop_find:
             lat_t, lon_l, lat_b, lon_r = work_bboxes.pop()
@@ -855,15 +855,15 @@
                 work_bboxes.extendleft([bbox1, bbox2, bbox3, bbox4])
 
     def translate(
         self,
         keywords: str,
         from_: Optional[str] = None,
         to: str = "en",
-    ) -> Optional[dict]:
+    ) -> Optional[Dict[str, Optional[str]]]:
         """DuckDuckGo translate
 
         Args:
             keywords: string or a list of strings to translate
             from_: translate from (defaults automatically). Defaults to None.
             to: what language to translate. Defaults to "en".
```

### Comparing `duckduckgo_search-3.8.1/duckduckgo_search.egg-info/PKG-INFO` & `duckduckgo_search-3.8.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: duckduckgo-search
-Version: 3.8.1
+Name: duckduckgo_search
+Version: 3.8.2
 Summary: Search for words, documents, images, news, maps and text translation using the DuckDuckGo.com search engine.
 Author: deedy5
 License: MIT License
 Project-URL: Homepage, https://github.com/deedy5/duckduckgo_search
 Keywords: python,duckduckgo
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
@@ -68,14 +68,16 @@
 ddgs text -k 'sanctions filetype:xls site:gov.ua' -m 50 -d
 # find and download any xls files from a specific site
 ddgs text -k 'filetype:xls site:mos.ru' -m 50 -d
 # find and download images
 ddgs images -k "yuri kuklachev cat theatre" -m 500 -s off -d
 # get latest news
 ddgs news -k "ukraine war" -s off -t d -m 10
+# get last day's news and save it to a csv file
+ddgs news -k "hubble telescope" -t d -m 50 -o csv
 ```
 [Go To TOP](#TOP)
 
 ## Duckduckgo search operators
 
 | Keywords example |	Result|
 | ---     | ---   |
@@ -199,15 +201,15 @@
 ```python
 def text(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     backend: str = "api",
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo text search generator. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m, y. Defaults to None.
@@ -244,15 +246,15 @@
 
 
 [Go To TOP](#TOP)
 
 ## 2. answers() - instant answers by duckduckgo.com
 
 ```python
-def answers(keywords: str) -> Generator[dict, None, None]:
+def answers(keywords: str) -> Iterator[Dict[str, Optional[str]]]::
     """DuckDuckGo instant answers. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
 
     Yields:
         dict with instant answers results.
@@ -279,15 +281,15 @@
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     size: Optional[str] = None,
     color: Optional[str] = None,
     type_image: Optional[str] = None,
     layout: Optional[str] = None,
     license_image: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo images search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: Day, Week, Month, Year. Defaults to None.
@@ -336,15 +338,15 @@
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
     resolution: Optional[str] = None,
     duration: Optional[str] = None,
     license_videos: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo videos search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -382,15 +384,15 @@
 
 ```python
 def news(
     keywords: str,
     region: str = "wt-wt",
     safesearch: str = "moderate",
     timelimit: Optional[str] = None,
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo news search. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
         safesearch: on, moderate, off. Defaults to "moderate".
         timelimit: d, w, m. Defaults to None.
@@ -429,15 +431,15 @@
         county: Optional[str] = None,
         state: Optional[str] = None,
         country: Optional[str] = None,
         postalcode: Optional[str] = None,
         latitude: Optional[str] = None,
         longitude: Optional[str] = None,
         radius: int = 0,
-    ) -> Iterator[dict]:
+    ) -> Iterator[Dict[str, Optional[str]]]:
         """DuckDuckGo maps search. Query params: https://duckduckgo.com/params
 
         Args:
             keywords: keywords for query
             place: if set, the other parameters are not used. Defaults to None.
             street: house number/street. Defaults to None.
             city: city of search. Defaults to None.
@@ -470,15 +472,15 @@
 
 ```python
 def translate(
     self,
     keywords: str,
     from_: Optional[str] = None,
     to: str = "en",
-) -> Optional[dict]:
+) -> Optional[Dict[str, Optional[str]]]:
     """DuckDuckGo translate
 
     Args:
         keywords: string or a list of strings to translate
         from_: translate from (defaults automatically). Defaults to None.
         to: what language to translate. Defaults to "en".
 
@@ -501,15 +503,15 @@
 
 ## 8. suggestions() - suggestions by duckduckgo.com
 
 ```python
 def suggestions(
     keywords,
     region: str = "wt-wt",
-) -> Iterator[dict]:
+) -> Iterator[Dict[str, Optional[str]]]:
     """DuckDuckGo suggestions. Query params: https://duckduckgo.com/params
 
     Args:
         keywords: keywords for query.
         region: wt-wt, us-en, uk-en, ru-ru, etc. Defaults to "wt-wt".
 
     Yields:
```

### Comparing `duckduckgo_search-3.8.1/pyproject.toml` & `duckduckgo_search-3.8.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Topic :: Internet :: WWW/HTTP :: Indexing/Search",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dependencies = [
+    "aiofiles>=23.1.0",
     "click>=8.1.3",
     "lxml>=4.9.2",
     "httpx[http2,socks,brotli]>=0.24.1",
 ]
 dynamic = ["version"]
 
 [project.urls]  # Optional
```

### Comparing `duckduckgo_search-3.8.1/tests/test_duckduckgo_search.py` & `duckduckgo_search-3.8.2/tests/test_duckduckgo_search.py`

 * *Files identical despite different names*

