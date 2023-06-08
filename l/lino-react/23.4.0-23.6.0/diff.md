# Comparing `tmp/lino_react-23.4.0.tar.gz` & `tmp/lino_react-23.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lino_react-23.4.0.tar", last modified: Wed Apr 26 03:16:46 2023, max compression
+gzip compressed data, was "lino_react-23.6.0.tar", last modified: Thu Jun  8 14:51:59 2023, max compression
```

## Comparing `lino_react-23.4.0.tar` & `lino_react-23.6.0.tar`

### file list

```diff
@@ -1,46 +1,52 @@
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.111742 lino_react-23.4.0/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.4.0/COPYING
--rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.4.0/MANIFEST.in
--rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-04-26 03:16:46.111742 lino_react-23.4.0/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.4.0/README.rst
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.4.0/lino_react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3843 2023-03-25 09:38:34.000000 lino_react-23.4.0/lino_react/react/__init__.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/config/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/config/react/
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.4.0/lino_react/react/config/react/linoweb.json
--rw-rw-r--   0 luc       (1000) www-data    (33)     1797 2023-01-07 15:27:20.000000 lino_react-23.4.0/lino_react/react/config/react/main.html
--rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.4.0/lino_react/react/config/react/service-worker.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     3893 2023-04-24 18:09:52.000000 lino_react-23.4.0/lino_react/react/icons.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.4.0/lino_react/react/index.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.4.0/lino_react/react/models.py
--rw-rw-r--   0 luc       (1000) www-data    (33)    29236 2023-04-18 13:23:50.000000 lino_react-23.4.0/lino_react/react/renderer.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react/react/static/
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.107742 lino_react-23.4.0/lino_react/react/static/media/
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/color.6441e63a.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/color.c7a33805.png
--rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.4.0/lino_react/react/static/media/line.567f5738.gif
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.2d2afb27.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.66ee0deb.woff
--rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.c55d94a2.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.df0140f8.ttf
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.dfbfef2d.eot
--rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.e5e0e944.svg
--rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.4.0/lino_react/react/static/media/primeicons.e61f3495.woff
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.107742 lino_react-23.4.0/lino_react/react/static/react/
--rw-rw-r--   0 luc       (1000) www-data    (33)  1776677 2023-04-18 13:23:50.000000 lino_react-23.4.0/lino_react/react/static/react/main.js
--rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.4.0/lino_react/react/static/react/main.js.LICENSE.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.4.0/lino_react/react/views.py
--rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-04-26 03:16:36.000000 lino_react-23.4.0/lino_react/setup_info.py
-drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-04-26 03:16:46.103742 lino_react-23.4.0/lino_react.egg-info/
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/PKG-INFO
--rw-rw-rw-   0 luc       (1000) www-data    (33)     1260 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/SOURCES.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/dependency_links.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.4.0/lino_react.egg-info/not-zip-safe
--rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/requires.txt
--rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-04-26 03:16:46.000000 lino_react-23.4.0/lino_react.egg-info/top_level.txt
--rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-04-26 03:16:46.111742 lino_react-23.4.0/setup.cfg
--rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.4.0/setup.py
--rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.4.0/tasks.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.292652 lino_react-23.6.0/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    34523 2021-04-12 19:37:56.000000 lino_react-23.6.0/COPYING
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      157 2020-04-27 23:26:14.000000 lino_react-23.6.0/MANIFEST.in
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1069 2023-06-08 14:51:59.292652 lino_react-23.6.0/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      178 2021-05-23 18:57:15.000000 lino_react-23.6.0/README.rst
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.284652 lino_react-23.6.0/lino_react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      283 2021-05-23 18:57:15.000000 lino_react-23.6.0/lino_react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3843 2023-03-25 09:38:34.000000 lino_react-23.6.0/lino_react/react/__init__.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/__pycache__/
+-rw-rw-r--   0 luc       (1000) www-data    (33)     2741 2023-05-02 09:01:04.000000 lino_react-23.6.0/lino_react/react/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)     3993 2023-05-02 09:01:06.000000 lino_react-23.6.0/lino_react/react/__pycache__/icons.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)      140 2023-05-02 09:01:04.000000 lino_react-23.6.0/lino_react/react/__pycache__/models.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    18321 2023-06-08 14:51:15.000000 lino_react-23.6.0/lino_react/react/__pycache__/renderer.cpython-310.pyc
+-rw-rw-r--   0 luc       (1000) www-data    (33)    20595 2023-05-02 13:45:04.000000 lino_react-23.6.0/lino_react/react/__pycache__/views.cpython-310.pyc
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.284652 lino_react-23.6.0/lino_react/react/config/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/config/react/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2018-11-27 12:45:09.000000 lino_react-23.6.0/lino_react/react/config/react/linoweb.json
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1797 2023-01-07 15:27:20.000000 lino_react-23.6.0/lino_react/react/config/react/main.html
+-rw-rw-r--   0 luc       (1000) www-data    (33)    16246 2022-11-30 04:23:52.000000 lino_react-23.6.0/lino_react/react/config/react/service-worker.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     3893 2023-04-24 18:09:52.000000 lino_react-23.6.0/lino_react/react/icons.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       36 2018-11-22 22:23:05.000000 lino_react-23.6.0/lino_react/react/index.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        0 2023-03-28 18:53:35.000000 lino_react-23.6.0/lino_react/react/models.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)    29204 2023-06-08 14:51:12.000000 lino_react-23.6.0/lino_react/react/renderer.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.284652 lino_react-23.6.0/lino_react/react/static/
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react/react/static/media/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/color.6441e63a.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    10355 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/color.c7a33805.png
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    13112 2020-09-29 17:55:04.000000 lino_react-23.6.0/lino_react/react/static/media/line.567f5738.gif
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39748 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.2d2afb27.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57384 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39648 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.66ee0deb.woff
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   234640 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.c55d94a2.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    39572 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.df0140f8.ttf
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57560 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.dfbfef2d.eot
+-rw-rw-rw-   0 luc       (1000) www-data    (33)   163568 2021-01-26 04:29:47.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.e5e0e944.svg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)    57460 2021-05-17 15:54:58.000000 lino_react-23.6.0/lino_react/react/static/media/primeicons.e61f3495.woff
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.292652 lino_react-23.6.0/lino_react/react/static/react/
+-rw-rw-r--   0 luc       (1000) www-data    (33)  1776706 2023-04-29 06:53:49.000000 lino_react-23.6.0/lino_react/react/static/react/main.js
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     2437 2021-09-23 03:04:12.000000 lino_react-23.6.0/lino_react/react/static/react/main.js.LICENSE.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)    28705 2023-03-24 10:38:37.000000 lino_react-23.6.0/lino_react/react/views.py
+-rw-rw-r--   0 luc       (1000) www-data    (33)     1431 2023-06-08 14:51:32.000000 lino_react-23.6.0/lino_react/setup_info.py
+drwxrwsr-x   0 luc       (1000) www-data    (33)        0 2023-06-08 14:51:59.288652 lino_react-23.6.0/lino_react.egg-info/
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1069 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/PKG-INFO
+-rw-rw-rw-   0 luc       (1000) www-data    (33)     1522 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/SOURCES.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/dependency_links.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        1 2019-01-08 09:40:17.000000 lino_react-23.6.0/lino_react.egg-info/not-zip-safe
+-rw-rw-rw-   0 luc       (1000) www-data    (33)        5 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/requires.txt
+-rw-rw-rw-   0 luc       (1000) www-data    (33)       11 2023-06-08 14:51:59.000000 lino_react-23.6.0/lino_react.egg-info/top_level.txt
+-rw-rw-r--   0 luc       (1000) www-data    (33)       38 2023-06-08 14:51:59.292652 lino_react-23.6.0/setup.cfg
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      183 2021-04-06 11:15:38.000000 lino_react-23.6.0/setup.py
+-rw-rw-rw-   0 luc       (1000) www-data    (33)      348 2021-05-23 18:57:15.000000 lino_react-23.6.0/tasks.py
```

### Comparing `lino_react-23.4.0/COPYING` & `lino_react-23.6.0/COPYING`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/PKG-INFO` & `lino_react-23.6.0/lino_react.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino_react
-Version: 23.4.0
+Name: lino-react
+Version: 23.6.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.4.0/lino_react/react/__init__.py` & `lino_react-23.6.0/lino_react/react/__init__.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/config/react/main.html` & `lino_react-23.6.0/lino_react/react/config/react/main.html`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/config/react/service-worker.js` & `lino_react-23.6.0/lino_react/react/config/react/service-worker.js`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/icons.py` & `lino_react-23.6.0/lino_react/react/icons.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/renderer.py` & `lino_react-23.6.0/lino_react/react/renderer.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 from pathlib import Path
 from html import escape
 from django.conf import settings
 from django.db import models
 from django.utils.text import format_lazy
 from django.utils import translation
 
-from lino.core import constants as ext_requests
 from lino.core.renderer import add_user_language, JsCacheRenderer
 
 from lino.core.menus import Menu, MenuItem
 from lino.core import constants
 from lino.core import choicelists
 from lino.core.gfks import ContentType
 from lino.modlib.extjs.ext_renderer import ExtRenderer
@@ -232,23 +231,23 @@
         if ar.actor.__name__ == "Main":
             return self.front_end.build_plain_url(*args, **kw)
 
         st = ar.get_status()
         kw.update(st['base_params'])
         add_user_language(kw, ar)
         if ar.offset is not None:
-            kw.setdefault(ext_requests.URL_PARAM_START, ar.offset)
+            kw.setdefault(constants.URL_PARAM_START, ar.offset)
         if ar.limit is not None:
-            kw.setdefault(ext_requests.URL_PARAM_LIMIT, ar.limit)
+            kw.setdefault(constants.URL_PARAM_LIMIT, ar.limit)
         if ar.order_by is not None:
             sc = ar.order_by[0]
             if sc.startswith('-'):
                 sc = sc[1:]
-                kw.setdefault(ext_requests.URL_PARAM_SORTDIR, 'DESC')
-            kw.setdefault(ext_requests.URL_PARAM_SORT, sc)
+                kw.setdefault(constants.URL_PARAM_SORTDIR, 'DESC')
+            kw.setdefault(constants.URL_PARAM_SORT, sc)
         # ~ print '20120901 TODO get_request_url
 
         return self.front_end.build_plain_url(
             ar.actor.app_label, ar.actor.__name__, *args, **kw)
 
     # from extrenderer
     def action_button(self, obj, ar, ba, label=None, **kw):
@@ -521,15 +520,15 @@
         result = []
         hotkeys = []
 
         for ba in actions_list:
             lh = ba.get_layout_handel()
             if (lh or ba.action.window_type):
 
-                action_descriptor = {'an': ba.action.action_name}
+                action_descriptor = { constants.URL_PARAM_ACTION_NAME: ba.action.action_name}
                 if lh:
                     action_descriptor.update(window_layout=lh.layout._formpanel_name)
                 if ba.action.window_type:
                     tbas = []
                     combo_map = dict()
 
                     for a in ba.actor.get_toolbar_actions(
```

### Comparing `lino_react-23.4.0/lino_react/react/static/media/color.6441e63a.png` & `lino_react-23.6.0/lino_react/react/static/media/color.6441e63a.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/color.c7a33805.png` & `lino_react-23.6.0/lino_react/react/static/media/color.c7a33805.png`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/line.567f5738.gif` & `lino_react-23.6.0/lino_react/react/static/media/line.567f5738.gif`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.2d2afb27.eot` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.2d2afb27.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.3a0d4a58.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.66ee0deb.woff` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.66ee0deb.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.c55d94a2.svg` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.c55d94a2.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.df0140f8.ttf` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.df0140f8.ttf`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.dfbfef2d.eot` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.dfbfef2d.eot`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.e5e0e944.svg` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.e5e0e944.svg`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/media/primeicons.e61f3495.woff` & `lino_react-23.6.0/lino_react/react/static/media/primeicons.e61f3495.woff`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/static/react/main.js` & `lino_react-23.6.0/lino_react/react/static/react/main.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -5451,24 +5451,26 @@
                                         router: t
                                     }))
                                 }
                             }))), !this.state.loading && this.data.detail_window && a.createElement(l.AW, {
                                 path: this.state.static_page ? "".concat(this.props.router.match.path) : "".concat(this.props.router.match.path, "/:pk"),
                                 render: function(t) {
                                     var n;
-                                    return n = "/" === t.location.pathname && window.App.state.user_settings.dashboard_layout ? window.App.state.site_data.choicelists["system.DashboardLayouts"].find((function(e) {
+                                    n = "/" === t.location.pathname && window.App.state.user_settings.dashboard_layout ? window.App.state.site_data.choicelists["system.DashboardLayouts"].find((function(e) {
                                         return e.value === window.App.state.user_settings.dashboard_layout
-                                    })).window_layout : e.props.actorData.window_layout, a.createElement(Ee.Z, {
+                                    })).window_layout : e.props.actorData.window_layout;
+                                    var o = e.props.mt;
+                                    return [void 0, null].includes(o) && (o = e.props.actorData.content_type), a.createElement(Ee.Z, {
                                         actorData: e.props.actorData,
                                         actorId: e.props.actorId,
                                         data: e.data.data,
                                         disabled_fields: e.data.disabled_fields,
                                         editing_mode: !e.data.data.disable_editing && e.data.editing_mode,
                                         mk: e.props.mk,
-                                        mt: e.props.actorData.content_type,
+                                        mt: o,
                                         packId: e.props.packId,
                                         parent: e,
                                         parent_pv: e.data.pv,
                                         pk: e.data.id,
                                         reload_timestamp: e.data.reload_timestamp,
                                         router: t,
                                         task: e.data.task,
@@ -14626,15 +14628,15 @@
                             return o.createElement(o.Fragment, null, o.createElement(f.ZP, {
                                 actorData: this.props.actorData,
                                 actorId: "".concat(this.props.packId, ".").concat(this.props.actorId),
                                 data: this.data.data,
                                 disabled_fields: this.state.disabled_fields,
                                 editing_mode: !this.data.data.disable_editing && this.state.editing_mode,
                                 mk: this.props.mk,
-                                mt: this.props.actorData.content_type,
+                                mt: this.props.mt,
                                 router: this.props.router,
                                 reload_timestamp: this.state.reload_timestamp,
                                 rp: this.rp || p()(this),
                                 parent_pv: this.state.pv,
                                 pk: this.props.pk,
                                 save: this.save,
                                 title: this.state.title,
```

### Comparing `lino_react-23.4.0/lino_react/react/static/react/main.js.LICENSE.txt` & `lino_react-23.6.0/lino_react/react/static/react/main.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/react/views.py` & `lino_react-23.6.0/lino_react/react/views.py`

 * *Files identical despite different names*

### Comparing `lino_react-23.4.0/lino_react/setup_info.py` & `lino_react-23.6.0/lino_react/setup_info.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: UTF-8 -*-
 # Copyright 2015-2023 Rumma & Ko Ltd
 # License: GNU Affero General Public License v3 (see file COPYING for details)
 
 SETUP_INFO = dict(
     name='lino_react',
-    version='23.4.0',
+    version='23.6.0',
     install_requires=['lino'],
     tests_require=[],
     test_suite='tests',
     description="The React front end for Lino",
     license_files=['COPYING'],
     include_package_data=False,
     zip_safe=False,
```

### Comparing `lino_react-23.4.0/lino_react.egg-info/PKG-INFO` & `lino_react-23.6.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: lino-react
-Version: 23.4.0
+Name: lino_react
+Version: 23.6.0
 Summary: The React front end for Lino
 Home-page: https://gitlab.com/lino-framework/react
 Author: Rumma & Ko Ltd
 Author-email: info@lino-framework.org
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier:   Programming Language :: Python
```

### Comparing `lino_react-23.4.0/lino_react.egg-info/SOURCES.txt` & `lino_react-23.6.0/lino_react.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 lino_react.egg-info/top_level.txt
 lino_react/react/__init__.py
 lino_react/react/icons.py
 lino_react/react/index.js
 lino_react/react/models.py
 lino_react/react/renderer.py
 lino_react/react/views.py
+lino_react/react/__pycache__/__init__.cpython-310.pyc
+lino_react/react/__pycache__/icons.cpython-310.pyc
+lino_react/react/__pycache__/models.cpython-310.pyc
+lino_react/react/__pycache__/renderer.cpython-310.pyc
+lino_react/react/__pycache__/views.cpython-310.pyc
 lino_react/react/config/react/linoweb.json
 lino_react/react/config/react/main.html
 lino_react/react/config/react/service-worker.js
 lino_react/react/static/media/color.6441e63a.png
 lino_react/react/static/media/color.c7a33805.png
 lino_react/react/static/media/line.567f5738.gif
 lino_react/react/static/media/primeicons.2d2afb27.eot
```

