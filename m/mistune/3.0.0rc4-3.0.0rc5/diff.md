# Comparing `tmp/mistune-3.0.0rc4.tar.gz` & `tmp/mistune-3.0.0rc5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mistune-3.0.0rc4.tar", last modified: Wed Nov 30 08:49:04 2022, max compression
+gzip compressed data, was "mistune-3.0.0rc5.tar", last modified: Wed Mar 22 13:03:09 2023, max compression
```

## Comparing `mistune-3.0.0rc4.tar` & `mistune-3.0.0rc5.tar`

### file list

```diff
@@ -1,54 +1,60 @@
-drwxr-xr-x   0 lepture    (501) staff       (20)        0 2022-11-30 08:49:04.124536 mistune-3.0.0rc4/
--rw-r--r--   0 lepture    (501) staff       (20)     1475 2019-11-21 14:23:44.000000 mistune-3.0.0rc4/LICENSE
--rw-r--r--   0 lepture    (501) staff       (20)       36 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/MANIFEST.in
--rw-r--r--   0 lepture    (501) staff       (20)      562 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/Makefile
--rw-r--r--   0 lepture    (501) staff       (20)     1832 2022-11-30 08:49:04.124892 mistune-3.0.0rc4/PKG-INFO
--rw-r--r--   0 lepture    (501) staff       (20)      434 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/README.rst
-drwxr-xr-x   0 lepture    (501) staff       (20)        0 2022-11-30 08:49:04.072634 mistune-3.0.0rc4/mistune/
--rw-r--r--   0 lepture    (501) staff       (20)     2205 2022-11-30 08:48:34.000000 mistune-3.0.0rc4/mistune/__init__.py
--rw-r--r--   0 lepture    (501) staff       (20)     2858 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/__main__.py
--rw-r--r--   0 lepture    (501) staff       (20)    16028 2022-11-28 14:04:16.000000 mistune-3.0.0rc4/mistune/block_parser.py
--rw-r--r--   0 lepture    (501) staff       (20)     5895 2022-11-27 18:17:08.000000 mistune-3.0.0rc4/mistune/core.py
-drwxr-xr-x   0 lepture    (501) staff       (20)        0 2022-11-30 08:49:04.094745 mistune-3.0.0rc4/mistune/directives/
--rw-r--r--   0 lepture    (501) staff       (20)      810 2022-11-27 17:09:01.000000 mistune-3.0.0rc4/mistune/directives/__init__.py
--rw-r--r--   0 lepture    (501) staff       (20)     3047 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/directives/_base.py
--rw-r--r--   0 lepture    (501) staff       (20)     3565 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/directives/_fenced.py
--rw-r--r--   0 lepture    (501) staff       (20)     1887 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/directives/_rst.py
--rw-r--r--   0 lepture    (501) staff       (20)     1755 2022-11-27 17:50:23.000000 mistune-3.0.0rc4/mistune/directives/admonition.py
--rw-r--r--   0 lepture    (501) staff       (20)     4448 2022-11-27 17:36:30.000000 mistune-3.0.0rc4/mistune/directives/image.py
--rw-r--r--   0 lepture    (501) staff       (20)     1977 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/directives/include.py
--rw-r--r--   0 lepture    (501) staff       (20)     3510 2022-11-27 17:55:28.000000 mistune-3.0.0rc4/mistune/directives/toc.py
--rw-r--r--   0 lepture    (501) staff       (20)     3751 2022-11-28 14:06:08.000000 mistune-3.0.0rc4/mistune/helpers.py
--rw-r--r--   0 lepture    (501) staff       (20)    11986 2022-11-27 16:29:47.000000 mistune-3.0.0rc4/mistune/inline_parser.py
--rw-r--r--   0 lepture    (501) staff       (20)     7108 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/list_parser.py
--rw-r--r--   0 lepture    (501) staff       (20)     3066 2022-11-28 07:05:58.000000 mistune-3.0.0rc4/mistune/markdown.py
-drwxr-xr-x   0 lepture    (501) staff       (20)        0 2022-11-30 08:49:04.115502 mistune-3.0.0rc4/mistune/plugins/
--rw-r--r--   0 lepture    (501) staff       (20)     1253 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/__init__.py
--rw-r--r--   0 lepture    (501) staff       (20)     2902 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/abbr.py
--rw-r--r--   0 lepture    (501) staff       (20)     3459 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/def_list.py
--rw-r--r--   0 lepture    (501) staff       (20)     4432 2022-11-30 08:48:34.000000 mistune-3.0.0rc4/mistune/plugins/footnotes.py
--rw-r--r--   0 lepture    (501) staff       (20)     4562 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/formatting.py
--rw-r--r--   0 lepture    (501) staff       (20)     1682 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/math.py
--rw-r--r--   0 lepture    (501) staff       (20)     2767 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/ruby.py
--rw-r--r--   0 lepture    (501) staff       (20)     1071 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/speedup.py
--rw-r--r--   0 lepture    (501) staff       (20)     2405 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/spoiler.py
--rw-r--r--   0 lepture    (501) staff       (20)     4990 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/table.py
--rw-r--r--   0 lepture    (501) staff       (20)     1681 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/task_lists.py
--rw-r--r--   0 lepture    (501) staff       (20)      524 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/plugins/url.py
-drwxr-xr-x   0 lepture    (501) staff       (20)        0 2022-11-30 08:49:04.123379 mistune-3.0.0rc4/mistune/renderers/
--rw-r--r--   0 lepture    (501) staff       (20)        0 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/renderers/__init__.py
--rw-r--r--   0 lepture    (501) staff       (20)     1648 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/renderers/_list.py
--rw-r--r--   0 lepture    (501) staff       (20)     4569 2022-11-28 14:05:42.000000 mistune-3.0.0rc4/mistune/renderers/html.py
--rw-r--r--   0 lepture    (501) staff       (20)     4685 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/renderers/markdown.py
--rw-r--r--   0 lepture    (501) staff       (20)     5266 2022-11-28 14:07:33.000000 mistune-3.0.0rc4/mistune/renderers/rst.py
--rw-r--r--   0 lepture    (501) staff       (20)     3136 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/toc.py
--rw-r--r--   0 lepture    (501) staff       (20)     1808 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/mistune/util.py
-drwxr-xr-x   0 lepture    (501) staff       (20)        0 2022-11-30 08:49:04.083082 mistune-3.0.0rc4/mistune.egg-info/
--rw-r--r--   0 lepture    (501) staff       (20)     1832 2022-11-30 08:49:04.000000 mistune-3.0.0rc4/mistune.egg-info/PKG-INFO
--rw-r--r--   0 lepture    (501) staff       (20)     1115 2022-11-30 08:49:04.000000 mistune-3.0.0rc4/mistune.egg-info/SOURCES.txt
--rw-r--r--   0 lepture    (501) staff       (20)        1 2022-11-30 08:49:04.000000 mistune-3.0.0rc4/mistune.egg-info/dependency_links.txt
--rw-r--r--   0 lepture    (501) staff       (20)        1 2022-11-30 08:49:03.000000 mistune-3.0.0rc4/mistune.egg-info/not-zip-safe
--rw-r--r--   0 lepture    (501) staff       (20)        8 2022-11-30 08:49:04.000000 mistune-3.0.0rc4/mistune.egg-info/top_level.txt
--rw-r--r--   0 lepture    (501) staff       (20)       92 2022-04-10 05:47:19.000000 mistune-3.0.0rc4/pyproject.toml
--rw-r--r--   0 lepture    (501) staff       (20)     1577 2022-11-30 08:49:04.127496 mistune-3.0.0rc4/setup.cfg
--rw-r--r--   0 lepture    (501) staff       (20)      136 2022-11-25 17:12:06.000000 mistune-3.0.0rc4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.460805 mistune-3.0.0rc5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16017 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/block_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/directives/
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3126 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4354 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/_fenced.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1965 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/_rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1755 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/admonition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3510 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/directives/toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12036 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/inline_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/list_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/abbr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3459 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/def_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/ruby.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/speedup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/spoiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/task_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/plugins/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1667 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4685 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/markdown.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5266 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/renderers/rst.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/toc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1808 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/src/mistune/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.464805 mistune-3.0.0rc5/src/mistune.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-22 13:03:09.000000 mistune-3.0.0rc5/src/mistune.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-22 13:03:09.468805 mistune-3.0.0rc5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2199 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_commonmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2927 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      500 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_renderers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-03-22 13:03:00.000000 mistune-3.0.0rc5/tests/test_syntax.py
```

### Comparing `mistune-3.0.0rc4/LICENSE` & `mistune-3.0.0rc5/LICENSE`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/__init__.py` & `mistune-3.0.0rc5/src/mistune/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,9 +67,9 @@
     'Markdown', 'HTMLRenderer',
     'BlockParser', 'BlockState', 'BaseRenderer',
     'InlineParser', 'InlineState',
     'escape', 'escape_url', 'safe_entity', 'unikey',
     'html', 'create_markdown', 'markdown',
 ]
 
-__version__ = '3.0.0rc4'
+__version__ = '3.0.0rc5'
 __homepage__ = 'https://mistune.lepture.com/'
```

### Comparing `mistune-3.0.0rc4/mistune/__main__.py` & `mistune-3.0.0rc5/src/mistune/__main__.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/block_parser.py` & `mistune-3.0.0rc5/src/mistune/block_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Optional, List, Tuple, Dict, Any
+from typing import Optional, List, Tuple
 from .util import (
     unikey,
     escape_url,
     expand_tab,
     expand_leading_tab,
 )
 from .core import Parser, BlockState
```

### Comparing `mistune-3.0.0rc4/mistune/core.py` & `mistune-3.0.0rc5/src/mistune/core.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/directives/__init__.py` & `mistune-3.0.0rc5/src/mistune/directives/__init__.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/directives/_base.py` & `mistune-3.0.0rc5/src/mistune/directives/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 import re
 
 
 class DirectiveParser:
-    NAME = 'directive'
+    name = 'directive'
 
     @staticmethod
-    def parse_name(m: re.Match):
+    def parse_type(m: re.Match):
         raise NotImplementedError()
 
     @staticmethod
     def parse_title(m: re.Match):
         raise NotImplementedError()
 
     @staticmethod
     def parse_content(m: re.Match):
         raise NotImplementedError()
 
     @classmethod
     def parse_tokens(cls, block, text, state):
-        if state.depth() >= block.max_nested_level - 1:
+        if state.depth() >= block.max_nested_level - 1 and cls.name in block.rules:
             rules = list(block.rules)
-            rules.remove(cls.NAME)
+            rules.remove(cls.name)
         else:
             rules = block.rules
         child = state.child_state(text)
         block.parse(child, rules)
         return child.tokens
 
     @staticmethod
@@ -44,25 +44,25 @@
             options.append((k, v))
         return options
 
 
 class BaseDirective:
     parser = DirectiveParser
     directive_pattern = None
-    register_before = None
 
     def __init__(self, plugins):
         self._methods = {}
         self.__plugins = plugins
 
     def register(self, name, fn):
         self._methods[name] = fn
 
-    def parse_method(self, name, block, m, state):
-        method = self._methods.get(name)
+    def parse_method(self, block, m, state):
+        _type = self.parser.parse_type(m)
+        method = self._methods.get(_type)
         if method:
             try:
                 token = method(block, m, state)
             except ValueError as e:
                 token = {'type': 'block_error', 'raw': str(e)}
         else:
             text = m.group(0)
@@ -77,35 +77,37 @@
         else:
             state.append_token(token)
         return token
 
     def parse_directive(self, block, m, state):
         raise NotImplementedError()
 
-    def __call__(self, md):
+    def register_block_parser(self, md, before=None):
         md.block.register(
-            self.parser.NAME,
+            self.parser.name,
             self.directive_pattern,
             self.parse_directive,
-            before=self.register_before,
+            before=before,
         )
+
+    def __call__(self, md):
         for plugin in self.__plugins:
             plugin.parser = self.parser
             plugin(self, md)
 
 
 class DirectivePlugin:
     def __init__(self):
         self.parser = None
 
     def parse_options(self, m: re.Match):
         return self.parser.parse_options(m)
 
-    def parse_name(self, m: re.Match):
-        return self.parser.parse_name(m)
+    def parse_type(self, m: re.Match):
+        return self.parser.parse_type(m)
 
     def parse_title(self, m: re.Match):
         return self.parser.parse_title(m)
 
     def parse_content(self, m: re.Match):
         return self.parser.parse_content(m)
```

### Comparing `mistune-3.0.0rc4/mistune/directives/_fenced.py` & `mistune-3.0.0rc5/src/mistune/directives/_fenced.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import re
 from ._base import DirectiveParser, BaseDirective
 
 __all__ = ['FencedDirective']
 
 
+_type_re = re.compile(r'^ *\{[a-zA-Z0-9_-]+\}')
 _directive_re = re.compile(
-    r'\{(?P<name>[a-zA-Z0-9_-]+)\} *(?P<title>[^\n]*)(?:\n|$)'
+    r'\{(?P<type>[a-zA-Z0-9_-]+)\} *(?P<title>[^\n]*)(?:\n|$)'
     r'(?P<options>(?:\:[a-zA-Z0-9_-]+\: *[^\n]*\n+)*)'
     r'\n*(?P<text>(?:[^\n]*\n+)*)'
 )
 
 
 class FencedParser(DirectiveParser):
-    NAME = 'fenced_directive'
+    name = 'fenced_directive'
 
     @staticmethod
-    def parse_name(m: re.Match):
-        return m.group('name')
+    def parse_type(m: re.Match):
+        return m.group('type')
 
     @staticmethod
     def parse_title(m: re.Match):
         return m.group('title')
 
     @staticmethod
     def parse_content(m: re.Match):
@@ -29,15 +30,15 @@
 
 class FencedDirective(BaseDirective):
     """A **fenced** style of directive looks like a fenced code block, it is
     inspired by markdown-it-docutils. The syntax looks like:
 
     .. code-block:: text
 
-        ```{directive-name} title
+        ```{directive-type} title
         :option-key: option value
         :option-key: option value
 
         content text here
         ```
 
     To use ``FencedDirective``, developers can add it into plugin list in
@@ -79,42 +80,63 @@
         ::::
 
     :param plugins: list of directive plugins
     :param markers: characters to determine the fence, default is backtick
                     and curly-bracket
     """
     parser = FencedParser
-    register_before = 'fenced_code'
 
     def __init__(self, plugins, markers='`~'):
         super(FencedDirective, self).__init__(plugins)
+        self.markers = markers
         _marker_pattern = '|'.join(re.escape(c) for c in markers)
         self.directive_pattern = (
             r'^(?P<fenced_directive_mark>(?:' + _marker_pattern + r'){3,})'
             r'\{[a-zA-Z0-9_-]+\}'
         )
 
-    def parse_directive(self, block, m, state):
-        marker = m.group('fenced_directive_mark')
+    def _process_directive(self, block, marker, start, state):
         mlen = len(marker)
+        cursor_start = start + len(marker)
+
         _end_pattern = (
             r'^ {0,3}' + marker[0] + '{' + str(mlen) + r',}'
             r'[ \t]*(?:\n|$)'
         )
         _end_re = re.compile(_end_pattern, re.M)
-        cursor_start = m.start() + mlen
 
         _end_m = _end_re.search(state.src, cursor_start)
         if _end_m:
             text = state.src[cursor_start:_end_m.start()]
             end_pos = _end_m.end()
         else:
             text = state.src[cursor_start:]
             end_pos = state.cursor_max
 
-        _new_m = _directive_re.match(text)
-        if not _new_m:
+        m = _directive_re.match(text)
+        if not m:
             return
 
-        name = _new_m.group('name')
-        self.parse_method(name, block, _new_m, state)
+        self.parse_method(block, m, state)
         return end_pos
+
+    def parse_directive(self, block, m, state):
+        marker = m.group('fenced_directive_mark')
+        return self._process_directive(block, marker, m.start(), state)
+
+    def parse_fenced_code(self, block, m, state):
+        info = m.group('fenced_3')
+        if not info or not _type_re.match(info):
+            return block.parse_fenced_code(m, state)
+
+        if state.depth() >= block.max_nested_level:
+            return block.parse_fenced_code(m, state)
+
+        marker = m.group('fenced_2')
+        return self._process_directive(block, marker, m.start(), state)
+
+    def __call__(self, md):
+        super(FencedDirective, self).__call__(md)
+        if self.markers == '`~':
+            md.block.register('fenced_code', None, self.parse_fenced_code)
+        else:
+            self.register_block_parser(md, 'fenced_code')
```

### Comparing `mistune-3.0.0rc4/mistune/directives/_rst.py` & `mistune-3.0.0rc5/src/mistune/directives/_rst.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 import re
 from ._base import DirectiveParser, BaseDirective
 
 __all__ = ['RSTDirective']
 
 
 _directive_re = re.compile(
-    r'\.\.( +)(?P<name>[a-zA-Z0-9_-]+)\:\: *(?P<title>[^\n]*)(?:\n|$)'
+    r'\.\.( +)(?P<type>[a-zA-Z0-9_-]+)\:\: *(?P<title>[^\n]*)(?:\n|$)'
     r'(?P<options>(?:  \1 {0,3}\:[a-zA-Z0-9_-]+\: *[^\n]*\n+)*)'
     r'\n*(?P<text>(?:  \1 {0,3}[^\n]*\n+)*)'
 )
 
 
 class RSTParser(DirectiveParser):
-    NAME = 'rst_directive'
+    name = 'rst_directive'
 
     @staticmethod
-    def parse_name(m: re.Match):
-        return m.group('name')
+    def parse_type(m: re.Match):
+        return m.group('type')
 
     @staticmethod
     def parse_title(m: re.Match):
         return m.group('title')
 
     @staticmethod
     def parse_content(m: re.Match):
@@ -34,15 +34,15 @@
 class RSTDirective(BaseDirective):
     """A RST style of directive syntax is inspired by reStructuredText.
     The syntax is very powerful that you can define a lot of custom
     features on your own. The syntax looks like:
 
     .. code-block:: text
 
-        .. directive-name:: directive value
+        .. directive-type:: directive value
            :option-key: option value
            :option-key: option value
 
            content text here
 
     To use ``RSTDirective``, developers can add it into plugin list in
     the :class:`Markdown` instance:
@@ -61,10 +61,13 @@
     directive_pattern = r'^\.\. +[a-zA-Z0-9_-]+\:\:'
 
     def parse_directive(self, block, m, state):
         m = _directive_re.match(state.src, state.cursor)
         if not m:
             return
 
-        name = m.group('name')
-        self.parse_method(name, block, m, state)
+        self.parse_method(block, m, state)
         return m.end()
+
+    def __call__(self, md):
+        super(RSTDirective, self).__call__(md)
+        self.register_block_parser(md)
```

### Comparing `mistune-3.0.0rc4/mistune/directives/admonition.py` & `mistune-3.0.0rc5/src/mistune/directives/admonition.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 class Admonition(DirectivePlugin):
     SUPPORTED_NAMES = {
         "attention", "caution", "danger", "error", "hint",
         "important", "note", "tip", "warning",
     }
 
     def parse(self, block, m, state):
-        name = self.parse_name(m)
+        name = self.parse_type(m)
         attrs = {'name': name}
         options = dict(self.parse_options(m))
         if 'class' in options:
             attrs['class'] = options['class']
 
         title = self.parse_title(m)
         if not title:
```

### Comparing `mistune-3.0.0rc4/mistune/directives/image.py` & `mistune-3.0.0rc5/src/mistune/directives/image.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/directives/include.py` & `mistune-3.0.0rc5/src/mistune/directives/include.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/directives/toc.py` & `mistune-3.0.0rc5/src/mistune/directives/toc.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/helpers.py` & `mistune-3.0.0rc5/src/mistune/helpers.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/inline_parser.py` & `mistune-3.0.0rc5/src/mistune/inline_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -163,15 +163,18 @@
                     end_pos = pos2
                     if label2:
                         label = label2
 
         if label is None:
             return
 
-        ref_links = state.env['ref_links']
+        ref_links = state.env.get('ref_links')
+        if not ref_links:
+            return
+
         key = unikey(label)
         env = ref_links.get(key)
         if env:
             attrs = {'url': env['url'], 'title': env.get('title')}
             token = self.__parse_link_token(is_image, text, attrs, state)
             token['ref'] = key
             token['label'] = label
```

### Comparing `mistune-3.0.0rc4/mistune/list_parser.py` & `mistune-3.0.0rc5/src/mistune/list_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     ordered = len(marker) > 1
     depth = state.depth()
     token = {
         'type': 'list',
         'children': [],
         'tight': True,
         'bullet': marker[-1],
-        'depth': depth,
         'attrs': {
+            'depth': depth,
             'ordered': ordered,
         },
     }
     if ordered:
         start = int(marker[:-1])
         if start != 1:
             # Example 304
```

### Comparing `mistune-3.0.0rc4/mistune/markdown.py` & `mistune-3.0.0rc5/src/mistune/markdown.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/__init__.py` & `mistune-3.0.0rc5/src/mistune/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/abbr.py` & `mistune-3.0.0rc5/src/mistune/plugins/abbr.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/def_list.py` & `mistune-3.0.0rc5/src/mistune/plugins/def_list.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/footnotes.py` & `mistune-3.0.0rc5/src/mistune/plugins/footnotes.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/formatting.py` & `mistune-3.0.0rc5/src/mistune/plugins/formatting.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/math.py` & `mistune-3.0.0rc5/src/mistune/plugins/math.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 __all__ = ['math', 'math_in_quote', 'math_in_list']
 
-BLOCK_MATH_PATTERN = r'^ {0,3}\$\$[ \t]*\n(?P<math_text>.+?)\n\$\$[ \t]*$'
+BLOCK_MATH_PATTERN = r'^ {0,3}\$\$[ \t]*\n(?P<math_text>[\s\S]+?)\n\$\$[ \t]*$'
 INLINE_MATH_PATTERN = r'\$(?!\s)(?P<math_text>.+?)(?!\s)\$'
 
 
 def parse_block_math(block, m, state):
     text = m.group('math_text')
     state.append_token({'type': 'block_math', 'raw': text})
     return m.end() + 1
```

### Comparing `mistune-3.0.0rc4/mistune/plugins/ruby.py` & `mistune-3.0.0rc5/src/mistune/plugins/ruby.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/speedup.py` & `mistune-3.0.0rc5/src/mistune/plugins/speedup.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/spoiler.py` & `mistune-3.0.0rc5/src/mistune/plugins/spoiler.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/table.py` & `mistune-3.0.0rc5/src/mistune/plugins/table.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/task_lists.py` & `mistune-3.0.0rc5/src/mistune/plugins/task_lists.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/plugins/url.py` & `mistune-3.0.0rc5/src/mistune/plugins/url.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/renderers/_list.py` & `mistune-3.0.0rc5/src/mistune/renderers/_list.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         if tok['type'] == 'list':
             tok['parent'] = parent
         elif tok['type'] == 'blank_line':
             continue
         text += renderer.render_token(tok, state)
 
     lines = text.splitlines()
-    text = lines[0] + '\n'
+    text = (lines[0] if lines else '') + '\n'
     prefix = ' ' * len(leading)
     for line in lines[1:]:
         if line:
             text += prefix + line + '\n'
         else:
             text += '\n'
     return leading + text
```

### Comparing `mistune-3.0.0rc4/mistune/renderers/html.py` & `mistune-3.0.0rc5/src/mistune/renderers/html.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/renderers/markdown.py` & `mistune-3.0.0rc5/src/mistune/renderers/markdown.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/renderers/rst.py` & `mistune-3.0.0rc5/src/mistune/renderers/rst.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/toc.py` & `mistune-3.0.0rc5/src/mistune/toc.py`

 * *Files identical despite different names*

### Comparing `mistune-3.0.0rc4/mistune/util.py` & `mistune-3.0.0rc5/src/mistune/util.py`

 * *Files identical despite different names*

