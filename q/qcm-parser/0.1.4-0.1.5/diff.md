# Comparing `tmp/qcm_parser-0.1.4.tar.gz` & `tmp/qcm_parser-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcm_parser-0.1.4.tar", last modified: Thu Jun  8 07:11:05 2023, max compression
+gzip compressed data, was "qcm_parser-0.1.5.tar", last modified: Thu Jun  8 18:55:10 2023, max compression
```

## Comparing `qcm_parser-0.1.4.tar` & `qcm_parser-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/
--rw-r--r--   0 quentin   (1000) quentin   (1000)    19016 2022-05-13 13:36:51.000000 qcm_parser-0.1.4/LICENSE
--rw-r--r--   0 quentin   (1000) quentin   (1000)     3028 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)     2527 2023-06-08 07:04:59.000000 qcm_parser-0.1.4/README.md
--rw-r--r--   0 quentin   (1000) quentin   (1000)       85 2022-06-05 09:47:40.000000 qcm_parser-0.1.4/pyproject.toml
--rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/setup.cfg
--rw-r--r--   0 quentin   (1000) quentin   (1000)      851 2023-06-08 07:06:05.000000 qcm_parser-0.1.4/setup.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/src/
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/src/qcm_parser/
--rw-r--r--   0 quentin   (1000) quentin   (1000)        0 2022-06-05 10:11:42.000000 qcm_parser-0.1.4/src/qcm_parser/__init__.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)    11665 2023-06-08 07:03:33.000000 qcm_parser-0.1.4/src/qcm_parser/parser.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)     2448 2022-06-10 15:50:13.000000 qcm_parser-0.1.4/src/qcm_parser/string_parsers.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/src/qcm_parser.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     3028 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      336 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/SOURCES.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/dependency_links.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        9 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/requires.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       11 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/top_level.txt
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/tests/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     3442 2023-06-08 07:00:46.000000 qcm_parser-0.1.4/tests/test_parser.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 18:55:10.939486 qcm_parser-0.1.5/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    19016 2022-05-13 13:36:51.000000 qcm_parser-0.1.5/LICENSE
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     3028 2023-06-08 18:55:10.939486 qcm_parser-0.1.5/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     2527 2023-06-08 18:45:09.000000 qcm_parser-0.1.5/README.md
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       85 2022-06-05 09:47:40.000000 qcm_parser-0.1.5/pyproject.toml
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-06-08 18:55:10.939486 qcm_parser-0.1.5/setup.cfg
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      851 2023-06-08 18:49:40.000000 qcm_parser-0.1.5/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 18:55:10.936153 qcm_parser-0.1.5/src/
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 18:55:10.939486 qcm_parser-0.1.5/src/qcm_parser/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        0 2022-06-05 10:11:42.000000 qcm_parser-0.1.5/src/qcm_parser/__init__.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    11666 2023-06-08 18:49:20.000000 qcm_parser-0.1.5/src/qcm_parser/parser.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     2448 2022-06-10 15:50:13.000000 qcm_parser-0.1.5/src/qcm_parser/string_parsers.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 18:55:10.939486 qcm_parser-0.1.5/src/qcm_parser.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     3028 2023-06-08 18:55:10.000000 qcm_parser-0.1.5/src/qcm_parser.egg-info/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      336 2023-06-08 18:55:10.000000 qcm_parser-0.1.5/src/qcm_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-06-08 18:55:10.000000 qcm_parser-0.1.5/src/qcm_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        9 2023-06-08 18:55:10.000000 qcm_parser-0.1.5/src/qcm_parser.egg-info/requires.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       11 2023-06-08 18:55:10.000000 qcm_parser-0.1.5/src/qcm_parser.egg-info/top_level.txt
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 18:55:10.939486 qcm_parser-0.1.5/tests/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     3448 2023-06-08 18:52:14.000000 qcm_parser-0.1.5/tests/test_parser.py
```

### Comparing `qcm_parser-0.1.4/LICENSE` & `qcm_parser-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qcm_parser-0.1.4/PKG-INFO` & `qcm_parser-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcm_parser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A parser of QCM file
 Home-page: https://github.com/qkzk/qcm_parser
 Author: qkzk
 Author-email: qu3nt1n@gmail.com
 Project-URL: Bug Tracker, https://github.com/qkzk/qcm_parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `qcm_parser-0.1.4/README.md` & `qcm_parser-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `qcm_parser-0.1.4/setup.py` & `qcm_parser-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qcm_parser",
-    version="0.1.4",
+    version="0.1.5",
     author="qkzk",
     author_email="qu3nt1n@gmail.com",
     description="A parser of QCM file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/qkzk/qcm_parser",
     project_urls={
```

### Comparing `qcm_parser-0.1.4/src/qcm_parser/parser.py` & `qcm_parser-0.1.5/src/qcm_parser/parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 title: QCM parser
 author: qkzk
 date: 2023/06/08
 """
 from typing import List, Tuple, Type
 
-from string_parsers import StringParsers, WebParsers, PDFParsers
+from .string_parsers import StringParsers, WebParsers, PDFParsers
 
 
 class ParseQCMError(Exception):
     """Exception raised when parsing went wrong."""
 
 
 class ParseQCM:
```

### Comparing `qcm_parser-0.1.4/src/qcm_parser/string_parsers.py` & `qcm_parser-0.1.5/src/qcm_parser/string_parsers.py`

 * *Files identical despite different names*

### Comparing `qcm_parser-0.1.4/src/qcm_parser.egg-info/PKG-INFO` & `qcm_parser-0.1.5/src/qcm_parser.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcm-parser
-Version: 0.1.4
+Version: 0.1.5
 Summary: A parser of QCM file
 Home-page: https://github.com/qkzk/qcm_parser
 Author: qkzk
 Author-email: qu3nt1n@gmail.com
 Project-URL: Bug Tracker, https://github.com/qkzk/qcm_parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `qcm_parser-0.1.4/tests/test_parser.py` & `qcm_parser-0.1.5/tests/test_parser.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import os.path
 
-# os.sys.path.append(os.path.dirname("../src/qcm_parser/"))
-from parserz import ParseQCM, ParseQCMError
+os.sys.path.append(os.path.dirname("../src/qcm_parser/"))
+from parser import ParseQCM, ParseQCMError
 
 
 def test_parser_web():
     expected_string = """## Un exemple avec une image
 
 texte de la partie
 
@@ -51,15 +51,15 @@
 
 ### Un exemple avec une zone de texte
 
 Écrire un sonnet.
 
 - [t]
 """
-    qcm = ParseQCM.from_file("example.md", mode="web")
+    qcm = ParseQCM.from_file("../example.md", mode="web")
     assert repr(qcm) == expected_string, "Parsing example failed"
 
     assert qcm.title == "Exemple de QCM", "wrong title"
 
     assert qcm.parts[0].title == "Un exemple avec une image", "wrong part title"
     assert qcm.parts[0].questions[0].title == "Qui est-ce ?", "wrong question title"
     assert (
@@ -84,15 +84,15 @@
     answers = qcm.parts[0].questions[0].answers
     assert answers[0].is_valid, "answer should be valid"
     assert answers[0].title == "Jacques Chirac", "didn't parse right correctly"
     assert answers[1].title == "Raymond Barre", "didn't parse wrong answer correctly"
 
 
 def test_parser_pdf():
-    qcm = ParseQCM.from_file("example.md", mode="pdf")
+    qcm = ParseQCM.from_file("../example.md", mode="pdf")
 
     assert qcm.title == """Exemple de QCM""", "wrong title"
     assert qcm.parts[0].title == "Un exemple avec une image\n", "wrong part title"
     assert qcm.parts[1].questions[0].title == "Calculer $2^3$\n", "wrong question title"
     assert qcm.parts[1].questions[0].answers[0].is_valid, "this answer should be valid"
     assert qcm.parts[1].questions[0].answers[0].title == " 8\n", "wrong question text"
     assert (
@@ -104,15 +104,15 @@
   s += i
 ```
 
 """
     ), "wrong question text"
 
     try:
-        qcm = ParseQCM.from_file("example.md", mode="thing")
+        qcm = ParseQCM.from_file("../example.md", mode="thing")
         raise AssertionError("Should have crashed, from unknown mode")
     except ParseQCMError:
         pass
 
 
 def test_all():
     test_parser_web()
```

