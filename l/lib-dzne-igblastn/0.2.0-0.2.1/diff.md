# Comparing `tmp/lib-dzne-igblastn-0.2.0.tar.gz` & `tmp/lib-dzne-igblastn-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lib-dzne-igblastn-0.2.0.tar", last modified: Thu Jun  8 21:00:06 2023, max compression
+gzip compressed data, was "lib-dzne-igblastn-0.2.1.tar", last modified: Thu Jun  8 21:18:56 2023, max compression
```

## Comparing `lib-dzne-igblastn-0.2.0.tar` & `lib-dzne-igblastn-0.2.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:00:06.719816 lib-dzne-igblastn-0.2.0/
--rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.2.0/LICENSE
--rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-06-08 21:00:06.719816 lib-dzne-igblastn-0.2.0/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:37:39.000000 lib-dzne-igblastn-0.2.0/README.md
--rw-rw-r--   0 base      (1001) base      (1001)      530 2023-06-08 20:57:17.000000 lib-dzne-igblastn-0.2.0/pyproject.toml
--rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-08 21:00:06.719816 lib-dzne-igblastn-0.2.0/setup.cfg
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:00:06.719816 lib-dzne-igblastn-0.2.0/src/
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:00:06.719816 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn/
--rw-rw-r--   0 base      (1001) base      (1001)       84 2023-06-08 20:57:37.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn/__init__.py
--rw-r--r--   0 base      (1001) base      (1001)      886 2023-05-29 13:41:38.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn/_functions.py
--rw-rw-r--   0 base      (1001) base      (1001)     9304 2023-05-29 12:47:17.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn/_parsers.py
-drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:00:06.719816 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/
--rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-06-08 21:00:06.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/PKG-INFO
--rw-rw-r--   0 base      (1001) base      (1001)      370 2023-06-08 21:00:06.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/SOURCES.txt
--rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-08 21:00:06.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/dependency_links.txt
--rw-rw-r--   0 base      (1001) base      (1001)       20 2023-06-08 21:00:06.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/requires.txt
--rw-rw-r--   0 base      (1001) base      (1001)       18 2023-06-08 21:00:06.000000 lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/top_level.txt
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:18:56.013284 lib-dzne-igblastn-0.2.1/
+-rw-r--r--   0 base      (1001) base      (1001)     1066 2023-03-01 20:28:52.000000 lib-dzne-igblastn-0.2.1/LICENSE
+-rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-06-08 21:18:56.013284 lib-dzne-igblastn-0.2.1/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)       20 2023-05-29 10:37:39.000000 lib-dzne-igblastn-0.2.1/README.md
+-rw-rw-r--   0 base      (1001) base      (1001)      562 2023-06-08 21:18:30.000000 lib-dzne-igblastn-0.2.1/pyproject.toml
+-rw-r--r--   0 base      (1001) base      (1001)       38 2023-06-08 21:18:56.013284 lib-dzne-igblastn-0.2.1/setup.cfg
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:18:56.009286 lib-dzne-igblastn-0.2.1/src/
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:18:56.013284 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn/
+-rw-rw-r--   0 base      (1001) base      (1001)       84 2023-06-08 20:57:37.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn/__init__.py
+-rw-r--r--   0 base      (1001) base      (1001)     1018 2023-06-08 21:18:50.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn/_functions.py
+-rw-rw-r--   0 base      (1001) base      (1001)     9304 2023-06-08 21:08:08.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn/_parsers.py
+drwxrwxr-x   0 base      (1001) base      (1001)        0 2023-06-08 21:18:56.013284 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/
+-rw-rw-r--   0 base      (1001) base      (1001)     1474 2023-06-08 21:18:56.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/PKG-INFO
+-rw-rw-r--   0 base      (1001) base      (1001)      370 2023-06-08 21:18:56.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/SOURCES.txt
+-rw-rw-r--   0 base      (1001) base      (1001)        1 2023-06-08 21:18:56.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/dependency_links.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       45 2023-06-08 21:18:56.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/requires.txt
+-rw-rw-r--   0 base      (1001) base      (1001)       18 2023-06-08 21:18:56.000000 lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/top_level.txt
```

### Comparing `lib-dzne-igblastn-0.2.0/LICENSE` & `lib-dzne-igblastn-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lib-dzne-igblastn-0.2.0/PKG-INFO` & `lib-dzne-igblastn-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-igblastn
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libary for using igblastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

### Comparing `lib-dzne-igblastn-0.2.0/pyproject.toml` & `lib-dzne-igblastn-0.2.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lib-dzne-igblastn"
-version = "0.2.0"
+version = "0.2.1"
 description = "Libary for using igblastn. "
 license = { file = "LICENSE" }
 authors = [{ name = "Johannes Horler", email = "johannes.horler@dzne.de" }]
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 keywords = []
 dependencies = [
     'lib-dzne-tsv>=0.1.4',
+    'lib-dzne-filedata>=0.4.4',
 ]
 requires-python = ">=3.11"
```

### Comparing `lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn/_functions.py` & `lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn/_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 
 
 import contextlib as _contextlib
 import os as _os
 import shutil as _shutil
 import tempfile as _tempfile
 
+import lib_dzne_filedata as _fd
+
+import lib_dzne_igblastn._parsers as _prs
+
 
 def get_cline(
     prog,
     *, 
     query, 
     out, 
     auxiliary_data,
@@ -34,12 +38,13 @@
 
 def igdata(IGDATA, *, directory):
     src = _os.path.join(IGDATA, 'internal_data')
     dest = _os.path.join(directory, 'internal_data')
     _shutil.copytree(src, dest)
     _os.environ['IGDATA'] = directory
 
-
+def parse(text):
+    return _prs.Parser.parse_text(text)
```

### Comparing `lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn/_parsers.py` & `lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn/_parsers.py`

 * *Files identical despite different names*

### Comparing `lib-dzne-igblastn-0.2.0/src/lib_dzne_igblastn.egg-info/PKG-INFO` & `lib-dzne-igblastn-0.2.1/src/lib_dzne_igblastn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lib-dzne-igblastn
-Version: 0.2.0
+Version: 0.2.1
 Summary: Libary for using igblastn. 
 Author-email: Johannes Horler <johannes.horler@dzne.de>
 License: Copyright © 2022 Johannes Horler
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the “Software”), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
         
         The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
```

