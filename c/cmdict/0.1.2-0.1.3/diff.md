# Comparing `tmp/cmdict-0.1.2.tar.gz` & `tmp/cmdict-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmdict-0.1.2.tar", last modified: Thu Jan 14 04:15:35 2021, max compression
+gzip compressed data, was "cmdict-0.1.3.tar", max compression
```

## Comparing `cmdict-0.1.2.tar` & `cmdict-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1065 2020-07-04 22:22:18.955788 cmdict-0.1.2/LICENSE
--rw-r--r--   0        0        0      926 2021-01-14 04:15:22.026620 cmdict-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       82 2020-07-21 00:28:59.617883 cmdict-0.1.2/src/cmdict/__init__.py
--rw-r--r--   0        0        0     2558 2021-01-14 04:00:05.920493 cmdict-0.1.2/src/cmdict/ecdict_connector.py
--rw-r--r--   0        0        0     1356 2021-01-14 04:15:22.026981 cmdict-0.1.2/src/cmdict/history.py
--rw-r--r--   0        0        0     4362 2021-01-14 04:00:05.920790 cmdict-0.1.2/src/cmdict/pdf_tools.py
--rw-r--r--   0        0        0     5882 2021-01-14 04:15:22.027448 cmdict-0.1.2/src/cmdict/run_script.py
--rw-r--r--   0        0        0      463 2020-07-25 22:15:56.621399 cmdict-0.1.2/src/cmdict/txt_tools.py
--rw-r--r--   0        0        0      384 2020-07-25 22:15:56.621685 cmdict-0.1.2/src/cmdict/utils.py
--rw-r--r--   0        0        0      996 2021-01-14 04:15:35.632278 cmdict-0.1.2/setup.py
--rw-r--r--   0        0        0      745 2021-01-14 04:15:35.632604 cmdict-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-06-08 14:28:05.993779 cmdict-0.1.3/LICENSE
+-rw-r--r--   0        0        0     2717 2023-06-08 14:28:05.993779 cmdict-0.1.3/README.md
+-rw-r--r--   0        0        0     1209 2023-06-08 14:28:05.993779 cmdict-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0       82 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/__init__.py
+-rw-r--r--   0        0        0     2558 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/ecdict_connector.py
+-rw-r--r--   0        0        0     1356 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/history.py
+-rw-r--r--   0        0        0     4551 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/pdf_tools.py
+-rw-r--r--   0        0        0     6129 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/run_script.py
+-rw-r--r--   0        0        0      463 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/txt_tools.py
+-rw-r--r--   0        0        0      384 2023-06-08 14:28:05.993779 cmdict-0.1.3/src/cmdict/utils.py
+-rw-r--r--   0        0        0     3674 1970-01-01 00:00:00.000000 cmdict-0.1.3/PKG-INFO
```

### Comparing `cmdict-0.1.2/LICENSE` & `cmdict-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.2/src/cmdict/ecdict_connector.py` & `cmdict-0.1.3/src/cmdict/ecdict_connector.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.2/src/cmdict/history.py` & `cmdict-0.1.3/src/cmdict/history.py`

 * *Files identical despite different names*

### Comparing `cmdict-0.1.2/src/cmdict/pdf_tools.py` & `cmdict-0.1.3/src/cmdict/pdf_tools.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 """Functions to handle highlights in PDF files."""
-import fitz
+from fitz import Document
 
 from cmdict.ecdict_connector import ECDICTConnector
 from cmdict.utils import remove_punctuation
 
+PDF_FEATURES: bool
+"""If the features for PDF are enabled."""
+try:
+    import fitz
+except ImportError:
+    PDF_FEATURES = False
+else:
+    PDF_FEATURES = True
 
-# Mac OS Preview supported colors
 PREVIEW_COLORS = {
     "yellow": [250, 205, 90],
     "green": [124, 200, 104],
     "blue": [105, 176, 241],
     "pink": [251, 92, 137],
     "purple": [200, 133, 218],
 }
+"""Colors supported by MacOS Preview by default."""
 
 PDF_ANNOT_HIGHLIGHT = 8
 
 
 def extract_words(file_path, color):
     """Extract highlighted words with specified color in a PDF file.
 
@@ -46,25 +54,25 @@
 
         for word in _fix_hyphen_broken(word_list):
             res.add(remove_punctuation(word))
 
     return res
 
 
-def _iterate_all_word_blocks(document):
+def _iterate_all_word_blocks(document: Document):
     """Iterate word blocks in order from the document.
 
     Args:
-        document (fitz.Document): the document.
+        document: the PDF document.
 
     Yields:
         tuple: word block.
     """
     for page in document:
-        for wb in sorted(page.getText("words"), key=lambda w: (w[1], w[0])):
+        for wb in sorted(page.get_text("words"), key=lambda w: (w[1], w[0])):
             yield wb
 
 
 def _iterate_filtered_annotations(document, color):
     """Iterate Annotations that are highlighted by target color.
 
     Args:
```

### Comparing `cmdict-0.1.2/src/cmdict/run_script.py` & `cmdict-0.1.3/src/cmdict/run_script.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-"""Functions for seaching in command line."""
+"""Functions for searching in command line."""
 import os
 import pathlib
 import zipfile
 
 import click
 from colorama import Fore, Style
 from colorama import init as _init_colorama
 import requests
 from tqdm import tqdm
 import yaml
 
 from cmdict.ecdict_connector import ECDICTConnector
-from cmdict.pdf_tools import extract_words
+from cmdict.pdf_tools import extract_words, PDF_FEATURES
 from cmdict.txt_tools import scan_words
 
 DB_URL = "https://github.com/skywind3000/ECDICT/releases/download/1.0.28/ecdict-sqlite-28.zip"  # noqa: E501
 DB_VALID_SIZE = (851288064, 17408)  # (full size, test size)
 
 _init_colorama(autoreset=True)
 
@@ -126,15 +126,22 @@
 def extract(pdf_path, color, save):
     """Extract highlighted words with specified color in a PDF file.
 
     Args:
         pdf_path (str): path to the PDF file.
         color (str): three numbers ranging between 0 and 1.
         save (bool): if extracted words will be saved in yaml file.
+
+    Raises:
+        ImportError: when the features for PDF are not enabled, most
+            likely because ``PyMuPDF`` is not installed.
     """
+    if not PDF_FEATURES:
+        raise ImportError("The features for PDF are not enabled.")
+
     if _valid_db_exists():
         db_engine = ECDICTConnector()
         words = extract_words(pdf_path, color)
 
         if save:
             with open(_db_dir + "/.extraction.yaml", "w") as f:
                 yaml.safe_dump(list(words), f)
```

