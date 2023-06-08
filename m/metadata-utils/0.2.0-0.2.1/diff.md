# Comparing `tmp/metadata_utils-0.2.0.tar.gz` & `tmp/metadata_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metadata_utils-0.2.0.tar", last modified: Wed Apr 19 16:45:05 2023, max compression
+gzip compressed data, was "metadata_utils-0.2.1.tar", last modified: Thu Jun  8 19:22:16 2023, max compression
```

## Comparing `metadata_utils-0.2.0.tar` & `metadata_utils-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.836947 metadata_utils-0.2.0/
--rw-r--r--   0 jvanasco   (501) admin       (80)      368 2023-04-19 16:18:53.000000 metadata_utils-0.2.0/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1105 2013-10-22 19:00:17.000000 metadata_utils-0.2.0/LICENSE
--rw-r--r--   0 jvanasco   (501) admin       (80)      179 2021-03-26 16:10:32.000000 metadata_utils-0.2.0/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     1236 2023-04-19 16:45:05.837327 metadata_utils-0.2.0/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)      400 2020-10-20 21:33:43.000000 metadata_utils-0.2.0/README.md
--rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-04-19 15:50:34.000000 metadata_utils-0.2.0/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)       69 2023-04-19 16:45:05.838847 metadata_utils-0.2.0/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1847 2023-04-19 16:44:40.000000 metadata_utils-0.2.0/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.808022 metadata_utils-0.2.0/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.820179 metadata_utils-0.2.0/src/metadata_utils/
--rw-r--r--   0 jvanasco   (501) admin       (80)      957 2023-04-19 15:55:35.000000 metadata_utils-0.2.0/src/metadata_utils/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.833011 metadata_utils-0.2.0/src/metadata_utils.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1236 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)      401 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-26 16:10:54.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)       18 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       15 2023-04-19 16:45:05.000000 metadata_utils-0.2.0/src/metadata_utils.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-04-19 16:45:05.836148 metadata_utils-0.2.0/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:10:41.000000 metadata_utils-0.2.0/tests/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     1675 2023-04-19 16:35:27.000000 metadata_utils-0.2.0/tests/test_core.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-04-19 16:17:53.000000 metadata_utils-0.2.0/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:22:16.458462 metadata_utils-0.2.1/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      397 2023-06-08 19:21:48.000000 metadata_utils-0.2.1/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1105 2013-10-22 19:00:17.000000 metadata_utils-0.2.1/LICENSE
+-rw-r--r--   0 jvanasco   (501) admin       (80)      179 2021-03-26 16:10:32.000000 metadata_utils-0.2.1/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1236 2023-06-08 19:22:16.458803 metadata_utils-0.2.1/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      400 2020-10-20 21:33:43.000000 metadata_utils-0.2.1/README.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-08 19:15:44.000000 metadata_utils-0.2.1/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      247 2023-06-08 19:22:16.460144 metadata_utils-0.2.1/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1860 2023-06-08 19:15:44.000000 metadata_utils-0.2.1/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:22:16.417555 metadata_utils-0.2.1/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:22:16.431405 metadata_utils-0.2.1/src/metadata_utils/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      985 2023-06-08 19:21:48.000000 metadata_utils-0.2.1/src/metadata_utils/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:15:44.000000 metadata_utils-0.2.1/src/metadata_utils/py.typed
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:22:16.453035 metadata_utils-0.2.1/src/metadata_utils.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1236 2023-06-08 19:22:16.000000 metadata_utils-0.2.1/src/metadata_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      429 2023-06-08 19:22:16.000000 metadata_utils-0.2.1/src/metadata_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-08 19:22:16.000000 metadata_utils-0.2.1/src/metadata_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-08 19:11:15.000000 metadata_utils-0.2.1/src/metadata_utils.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       23 2023-06-08 19:22:16.000000 metadata_utils-0.2.1/src/metadata_utils.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       15 2023-06-08 19:22:16.000000 metadata_utils-0.2.1/src/metadata_utils.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-08 19:22:16.457176 metadata_utils-0.2.1/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2021-03-26 16:10:41.000000 metadata_utils-0.2.1/tests/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1693 2023-06-08 19:15:44.000000 metadata_utils-0.2.1/tests/test_core.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-04-19 16:48:46.000000 metadata_utils-0.2.1/tox.ini
```

### Comparing `metadata_utils-0.2.0/LICENSE` & `metadata_utils-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `metadata_utils-0.2.0/PKG-INFO` & `metadata_utils-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata_utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lightweight Metadata Support
 Home-page: https://github.com/jvanasco/metadata_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Keywords: web
 Classifier: Intended Audience :: Developers
```

### Comparing `metadata_utils-0.2.0/setup.py` & `metadata_utils-0.2.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 """metadata_utils installation script.
 """
 import os
 import re
-from setuptools import setup
+
 from setuptools import find_packages
+from setuptools import setup
 
 HERE = os.path.abspath(os.path.dirname(__file__))
 
 long_description = description = "Lightweight Metadata Support"
 with open(os.path.join(HERE, "README.md")) as fp:
     long_description = fp.read()
 
 # store version in the init.py
 with open(os.path.join(HERE, "src", "metadata_utils", "__init__.py")) as v_file:
     VERSION = re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
 
 requires = []
 tests_require = [
+    "mypy",
     "pytest",
 ]
 testing_extras = tests_require + []
 
 setup(
     name="metadata_utils",
     description="Lightweight Metadata Support",
```

### Comparing `metadata_utils-0.2.0/src/metadata_utils/__init__.py` & `metadata_utils-0.2.1/src/metadata_utils/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # stdlib
 import unicodedata
-from xml.sax.saxutils import escape, unescape
+from xml.sax.saxutils import escape
+from xml.sax.saxutils import unescape
 
-__VERSION__ = "0.2.0"
+__VERSION__ = "0.2.1"
 
 
 # ==============================================================================
 
 
 # https://wiki.python.org/moin/EscapingHtml
 # escape() and unescape() takes care of "&" , "<" and ">"
```

### Comparing `metadata_utils-0.2.0/src/metadata_utils.egg-info/PKG-INFO` & `metadata_utils-0.2.1/src/metadata_utils.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metadata-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Lightweight Metadata Support
 Home-page: https://github.com/jvanasco/metadata_utils
 Author: Jonathan Vanasco
 Author-email: jonathan@findmeon.com
 License: MIT
 Keywords: web
 Classifier: Intended Audience :: Developers
```

### Comparing `metadata_utils-0.2.0/tests/test_core.py` & `metadata_utils-0.2.1/tests/test_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
+# stdlib
 import unittest
+
+# local
 import metadata_utils
 
 
 # ==============================================================================
 
 
 class TestEscaping(unittest.TestCase):
```

