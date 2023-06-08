# Comparing `tmp/pygef-0.8.1.tar.gz` & `tmp/pygef-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygef-0.8.1.tar", last modified: Fri Jun  2 08:16:52 2023, max compression
+gzip compressed data, was "pygef-0.8.2.tar", last modified: Thu Jun  8 18:52:27 2023, max compression
```

## Comparing `pygef-0.8.1.tar` & `pygef-0.8.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-02 08:16:42.000000 pygef-0.8.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-02 08:16:52.963508 pygef-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12967 2023-06-02 08:16:42.000000 pygef-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-02 08:16:42.000000 pygef-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 08:16:52.963508 pygef-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-02 08:16:42.000000 pygef-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/bore.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef/broxml/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/parse_bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/parse_cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8203 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/resolvers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/broxml/xml_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef/gef/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9298 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/gef.py
--rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/parse_bore.py
--rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/parse_cpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/gef/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/plotting.py
--rw-r--r--   0 runner    (1001) docker     (123)     7394 2023-06-02 08:16:42.000000 pygef-0.8.1/src/pygef/shim.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 08:16:52.963508 pygef-0.8.1/src/pygef.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-02 08:16:52.000000 pygef-0.8.1/src/pygef.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:27.640504 pygef-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-06-08 18:52:19.000000 pygef-0.8.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-06-08 18:52:27.640504 pygef-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-08 18:52:19.000000 pygef-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1691 2023-06-08 18:52:19.000000 pygef-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:52:27.640504 pygef-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 18:52:19.000000 pygef-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:27.636504 pygef-0.8.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:27.640504 pygef-0.8.2/src/pygef/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5012 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/bore.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:27.640504 pygef-0.8.2/src/pygef/broxml/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/broxml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7413 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/broxml/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5065 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/broxml/parse_bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8449 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/broxml/parse_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8247 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/broxml/resolvers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/broxml/xml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9310 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:27.640504 pygef-0.8.2/src/pygef/gef/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/gef/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9298 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/gef/gef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11027 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/gef/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/gef/parse_bore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7504 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/gef/parse_cpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15924 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/gef/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9793 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/plotting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7364 2023-06-08 18:52:19.000000 pygef-0.8.2/src/pygef/shim.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:52:27.640504 pygef-0.8.2/src/pygef.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14475 2023-06-08 18:52:27.000000 pygef-0.8.2/src/pygef.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-08 18:52:27.000000 pygef-0.8.2/src/pygef.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:52:27.000000 pygef-0.8.2/src/pygef.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-08 18:52:27.000000 pygef-0.8.2/src/pygef.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 18:52:27.000000 pygef-0.8.2/src/pygef.egg-info/top_level.txt
```

### Comparing `pygef-0.8.1/LICENSE.txt` & `pygef-0.8.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/PKG-INFO` & `pygef-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygef
-Version: 0.8.1
+Version: 0.8.2
 Summary: Parse soil measurument data.
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -32,15 +32,15 @@
 License-File: LICENSE.txt
 
 # PYGEF
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPi Version](https://img.shields.io/pypi/v/pygef.svg)](https://pypi.org/project/pygef)
 [![GitHub stars](https://img.shields.io/github/stars/ritchie46/pygef.svg?logo=github&label=Stars&logoColor=white)](https://github.com/ritchie46/pygef)
-[![Coverage Status](https://coveralls.io/repos/github/ritchie46/pygef/badge.svg?branch=master)](https://coveralls.io/github/ritchie46/pygef?branch=code-coverage)
+[![Coverage Status](https://coveralls.io/repos/github/cemsbv/pygef/badge.svg?branch=master)](https://coveralls.io/github/cemsbv/pygef?branch=master)
 
 Simple parser for \*.gef files. These are ASCII based files used for soil properties measurements.
 Compatible with Python 3.9.
 
 Recently added the parsing of xml boreholes file, the xml parsing is still in a preliminary phase,
 not all the files are supported. If you find a file that doesn't work with pygef, please make an issue about it or PR :)
```

### Comparing `pygef-0.8.1/README.md` & `pygef-0.8.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # PYGEF
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPi Version](https://img.shields.io/pypi/v/pygef.svg)](https://pypi.org/project/pygef)
 [![GitHub stars](https://img.shields.io/github/stars/ritchie46/pygef.svg?logo=github&label=Stars&logoColor=white)](https://github.com/ritchie46/pygef)
-[![Coverage Status](https://coveralls.io/repos/github/ritchie46/pygef/badge.svg?branch=master)](https://coveralls.io/github/ritchie46/pygef?branch=code-coverage)
+[![Coverage Status](https://coveralls.io/repos/github/cemsbv/pygef/badge.svg?branch=master)](https://coveralls.io/github/cemsbv/pygef?branch=master)
 
 Simple parser for \*.gef files. These are ASCII based files used for soil properties measurements.
 Compatible with Python 3.9.
 
 Recently added the parsing of xml boreholes file, the xml parsing is still in a preliminary phase,
 not all the files are supported. If you find a file that doesn't work with pygef, please make an issue about it or PR :)
```

### Comparing `pygef-0.8.1/pyproject.toml` & `pygef-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pygef"
-version = "0.8.1"
+version = "0.8.2"
 description = "Parse soil measurument data."
 dependencies = [
-    "polars[pyarrow]>=0.16.3,<0.19",
+    "polars[pyarrow]>0.16.14,<0.19",
     "matplotlib>=3.6,<4.0",
     "lxml>=4.9.1,<5.0",
     "gef-file-to-map>=0.1,<0.2",
 ]
 requires-python = ">=3.9"
 license = { file = "LICENSE.txt" }
 readme = "README.md"
```

### Comparing `pygef-0.8.1/src/pygef/bore.py` & `pygef-0.8.2/src/pygef/bore.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/broxml/mapping.py` & `pygef-0.8.2/src/pygef/broxml/mapping.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/broxml/parse_bore.py` & `pygef-0.8.2/src/pygef/broxml/parse_bore.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/broxml/parse_cpt.py` & `pygef-0.8.2/src/pygef/broxml/parse_cpt.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/broxml/resolvers.py` & `pygef-0.8.2/src/pygef/broxml/resolvers.py`

 * *Files 1% similar despite different names*

```diff
@@ -191,14 +191,15 @@
     # we strip the data because there is leading and trailing whitespace.
     data = el.find(f"{prefix}/cptcommon:values", namespaces=namespaces).text.strip()
     return pl.read_csv(
         data.encode(),
         new_columns=columns,
         columns=selection,
         has_header=False,
+        dtypes=[pl.Float64] * len(columns),
         separator=delimiter,
         eol_char=new_line_char,
         ignore_errors=True,
         null_values="-999999",
     ).drop_nulls("coneResistance")
```

### Comparing `pygef-0.8.1/src/pygef/broxml/xml_parser.py` & `pygef-0.8.2/src/pygef/broxml/xml_parser.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/common.py` & `pygef-0.8.2/src/pygef/common.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/cpt.py` & `pygef-0.8.2/src/pygef/cpt.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/exceptions.py` & `pygef-0.8.2/src/pygef/exceptions.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/gef/gef.py` & `pygef-0.8.2/src/pygef/gef/gef.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/gef/mapping.py` & `pygef-0.8.2/src/pygef/gef/mapping.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/gef/parse_bore.py` & `pygef-0.8.2/src/pygef/gef/parse_bore.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/gef/parse_cpt.py` & `pygef-0.8.2/src/pygef/gef/parse_cpt.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/gef/utils.py` & `pygef-0.8.2/src/pygef/gef/utils.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/plotting.py` & `pygef-0.8.2/src/pygef/plotting.py`

 * *Files identical despite different names*

### Comparing `pygef-0.8.1/src/pygef/shim.py` & `pygef-0.8.2/src/pygef/shim.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 from __future__ import annotations
 
 import io
 import os
 from pathlib import Path
-from typing import Any
-
-from typing_extensions import Literal
+from typing import Any, Literal
 
 from pygef.bore import BoreData
 from pygef.broxml.parse_bore import read_bore as read_bore_xml
 from pygef.broxml.parse_cpt import read_cpt as read_cpt_xml
 from pygef.common import Location, VerticalDatumClass
 from pygef.cpt import CPTData, QualityClass
 from pygef.gef.parse_bore import _GefBore
```

### Comparing `pygef-0.8.1/src/pygef.egg-info/PKG-INFO` & `pygef-0.8.2/src/pygef.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygef
-Version: 0.8.1
+Version: 0.8.2
 Summary: Parse soil measurument data.
 License: MIT License
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -32,15 +32,15 @@
 License-File: LICENSE.txt
 
 # PYGEF
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![PyPi Version](https://img.shields.io/pypi/v/pygef.svg)](https://pypi.org/project/pygef)
 [![GitHub stars](https://img.shields.io/github/stars/ritchie46/pygef.svg?logo=github&label=Stars&logoColor=white)](https://github.com/ritchie46/pygef)
-[![Coverage Status](https://coveralls.io/repos/github/ritchie46/pygef/badge.svg?branch=master)](https://coveralls.io/github/ritchie46/pygef?branch=code-coverage)
+[![Coverage Status](https://coveralls.io/repos/github/cemsbv/pygef/badge.svg?branch=master)](https://coveralls.io/github/cemsbv/pygef?branch=master)
 
 Simple parser for \*.gef files. These are ASCII based files used for soil properties measurements.
 Compatible with Python 3.9.
 
 Recently added the parsing of xml boreholes file, the xml parsing is still in a preliminary phase,
 not all the files are supported. If you find a file that doesn't work with pygef, please make an issue about it or PR :)
```

### Comparing `pygef-0.8.1/src/pygef.egg-info/SOURCES.txt` & `pygef-0.8.2/src/pygef.egg-info/SOURCES.txt`

 * *Files identical despite different names*

