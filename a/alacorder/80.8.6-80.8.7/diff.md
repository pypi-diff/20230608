# Comparing `tmp/alacorder-80.8.6.tar.gz` & `tmp/alacorder-80.8.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alacorder-80.8.6.tar", max compression
+gzip compressed data, was "alacorder-80.8.7.tar", max compression
```

## Comparing `alacorder-80.8.6.tar` & `alacorder-80.8.7.tar`

### file list

```diff
@@ -1,9 +1,8 @@
--rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.6/LICENSE
--rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.6/README.md
--rw-r--r--   0        0        0      697 2023-05-30 15:50:27.085894 alacorder-80.8.6/pyproject.toml
--rw-r--r--   0        0        0     6148 2023-05-29 16:04:40.384447 alacorder-80.8.6/src/alacorder/.DS_Store
--rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
--rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.6/src/alacorder/__init__.py
--rw-r--r--   0        0        0   281467 2023-05-30 15:53:52.895017 alacorder-80.8.6/src/alacorder/__main__.py
--rw-r--r--   0        0        0   281467 2023-05-30 15:53:43.101038 alacorder-80.8.6/src/alacorder/alac.py
--rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 alacorder-80.8.6/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-02-07 05:47:31.000000 alacorder-80.8.7/LICENSE
+-rw-r--r--   0        0        0     7315 2023-05-26 22:11:39.116260 alacorder-80.8.7/README.md
+-rw-r--r--   0        0        0      697 2023-06-08 15:29:44.299340 alacorder-80.8.7/pyproject.toml
+-rw-r--r--   0        0        0   234455 2023-05-18 23:58:39.588863 alacorder-80.8.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py
+-rw-r--r--   0        0        0        0 2023-05-02 17:21:37.916960 alacorder-80.8.7/src/alacorder/__init__.py
+-rw-r--r--   0        0        0   281467 2023-06-08 15:28:14.418451 alacorder-80.8.7/src/alacorder/__main__.py
+-rw-r--r--   0        0        0   281467 2023-06-08 15:28:01.542452 alacorder-80.8.7/src/alacorder/alac.py
+-rw-r--r--   0        0        0     8244 1970-01-01 00:00:00.000000 alacorder-80.8.7/PKG-INFO
```

### Comparing `alacorder-80.8.6/LICENSE` & `alacorder-80.8.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.6/README.md` & `alacorder-80.8.7/README.md`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.6/pyproject.toml` & `alacorder-80.8.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alacorder"
-version = "80.8.6"
+version = "80.8.7"
 description = "Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes."
 authors = ["Sam Robson <sbrobson@crimson.ua.edu>"]
 license = "MIT LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `alacorder-80.8.6/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py` & `alacorder-80.8.7/src/alacorder/.ipynb_checkpoints/alac-checkpoint.py`

 * *Files identical despite different names*

### Comparing `alacorder-80.8.6/src/alacorder/__main__.py` & `alacorder-80.8.7/src/alacorder/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
-    polars ^0.18.0, PyMuPDF ^1.21.1,
+    polars ^0.18.1, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.6"
+version = "80.8.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.8.6/src/alacorder/alac.py` & `alacorder-80.8.7/src/alacorder/alac.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 ╔═╗╔╗╔╔═╗╦ ╦╔═╗╔═╗╦  ╔═╗╔═╗╔═╗
 ╚═╗║║║║ ║║║║╠═╝╠═╣║  ╠═╣║  ║╣ 
 ╚═╝╝╚╝╚═╝╚╩╝╩  ╩ ╩╩═╝╩ ╩╚═╝╚═╝
 (c) 2023 Sam Robson ----------
 
 Dependencies: 
     python 3.9+, brotli ^1.0.9, click ^8.1.3,
-    polars ^0.18.0, PyMuPDF ^1.21.1,
+    polars ^0.18.1, PyMuPDF ^1.21.1,
     PySimpleGUI ^4.60.4, selenium ^4.8.3, 
     tqdm ^4.65.0, xlsx2csv ^0.8.1, XlsxWriter ^3.0.9
 Optional dependencies:
     pyarrow required to export summary to .xls, .xlsx,
     Google Chrome required to fetch cases from Alacourt and crawl ADOC
 """
 
 name = "ALACORDER"
 long_version = "snowpalace"
-version = "80.8.6"
+version = "80.8.7"
 
 _autoload_graphical_user_interface = False
 
 import polars as pl
 import os, sys, time, glob, re, math
 import click, fitz, selenium, xlsxwriter
 from tqdm.auto import tqdm
```

### Comparing `alacorder-80.8.6/PKG-INFO` & `alacorder-80.8.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alacorder
-Version: 80.8.6
+Version: 80.8.7
 Summary: Alacorder collects and processes Alacourt case detail PDFs into data tables suitable for research purposes.
 License: MIT
 Author: Sam Robson
 Author-email: sbrobson@crimson.ua.edu
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

