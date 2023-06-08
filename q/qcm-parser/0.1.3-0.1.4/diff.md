# Comparing `tmp/qcm_parser-0.1.3.tar.gz` & `tmp/qcm_parser-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qcm_parser-0.1.3.tar", last modified: Tue Jun  7 14:44:51 2022, max compression
+gzip compressed data, was "qcm_parser-0.1.4.tar", last modified: Thu Jun  8 07:11:05 2023, max compression
```

## Comparing `qcm_parser-0.1.3.tar` & `qcm_parser-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-06-07 14:44:51.732879 qcm_parser-0.1.3/
--rw-r--r--   0 quentin   (1000) quentin   (1000)    19016 2022-05-13 13:36:51.000000 qcm_parser-0.1.3/LICENSE
--rw-r--r--   0 quentin   (1000) quentin   (1000)     2986 2022-06-07 14:44:51.732879 qcm_parser-0.1.3/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)     2485 2022-06-05 11:11:13.000000 qcm_parser-0.1.3/README.md
--rw-r--r--   0 quentin   (1000) quentin   (1000)       85 2022-06-05 09:47:40.000000 qcm_parser-0.1.3/pyproject.toml
--rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2022-06-07 14:44:51.732879 qcm_parser-0.1.3/setup.cfg
--rw-r--r--   0 quentin   (1000) quentin   (1000)      851 2022-06-07 14:44:40.000000 qcm_parser-0.1.3/setup.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-06-07 14:44:51.729546 qcm_parser-0.1.3/src/
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-06-07 14:44:51.729546 qcm_parser-0.1.3/src/qcm_parser/
--rw-r--r--   0 quentin   (1000) quentin   (1000)        0 2022-06-05 10:11:42.000000 qcm_parser-0.1.3/src/qcm_parser/__init__.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)    10899 2022-06-07 14:44:23.000000 qcm_parser-0.1.3/src/qcm_parser/parser.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)     2448 2022-06-06 19:00:50.000000 qcm_parser-0.1.3/src/qcm_parser/string_parsers.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2022-06-07 14:44:51.732879 qcm_parser-0.1.3/src/qcm_parser.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)     2986 2022-06-07 14:44:51.000000 qcm_parser-0.1.3/src/qcm_parser.egg-info/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      315 2022-06-07 14:44:51.000000 qcm_parser-0.1.3/src/qcm_parser.egg-info/SOURCES.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2022-06-07 14:44:51.000000 qcm_parser-0.1.3/src/qcm_parser.egg-info/dependency_links.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        9 2022-06-07 14:44:51.000000 qcm_parser-0.1.3/src/qcm_parser.egg-info/requires.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       11 2022-06-07 14:44:51.000000 qcm_parser-0.1.3/src/qcm_parser.egg-info/top_level.txt
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    19016 2022-05-13 13:36:51.000000 qcm_parser-0.1.4/LICENSE
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     3028 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     2527 2023-06-08 07:04:59.000000 qcm_parser-0.1.4/README.md
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       85 2022-06-05 09:47:40.000000 qcm_parser-0.1.4/pyproject.toml
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/setup.cfg
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      851 2023-06-08 07:06:05.000000 qcm_parser-0.1.4/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/src/
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/src/qcm_parser/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        0 2022-06-05 10:11:42.000000 qcm_parser-0.1.4/src/qcm_parser/__init__.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    11665 2023-06-08 07:03:33.000000 qcm_parser-0.1.4/src/qcm_parser/parser.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     2448 2022-06-10 15:50:13.000000 qcm_parser-0.1.4/src/qcm_parser/string_parsers.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/src/qcm_parser.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     3028 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      336 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        9 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/requires.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       11 2023-06-08 07:11:05.000000 qcm_parser-0.1.4/src/qcm_parser.egg-info/top_level.txt
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-06-08 07:11:05.018331 qcm_parser-0.1.4/tests/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     3442 2023-06-08 07:00:46.000000 qcm_parser-0.1.4/tests/test_parser.py
```

### Comparing `qcm_parser-0.1.3/LICENSE` & `qcm_parser-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `qcm_parser-0.1.3/PKG-INFO` & `qcm_parser-0.1.4/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcm_parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: A parser of QCM file
 Home-page: https://github.com/qkzk/qcm_parser
 Author: qkzk
 Author-email: qu3nt1n@gmail.com
 Project-URL: Bug Tracker, https://github.com/qkzk/qcm_parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # QCM parser
 
 It's a basic and quite strict QCM (Multiple Choices Questions) parser.
 
-It parses a file .md file into Python objects. 
+It parses a file .md file into Python objects.
 That's all.
 
 There's no rendering, no export. It must be done separetaly.
 
 ## Installation
 
 It requires python>=3.7 and `markdown` package.
@@ -46,108 +46,112 @@
 
 In memory, you `qcm` object is represented as a tree which holds parts.
 
 Those parts holds questions, holding answers.
 
 It is then easy to navigate through it like this :
 
-
 ```
 print(qcm.title)
 for part in qcm.parts:
     print(part.title)
+    print(part.text)
     for question in part.questions:
-        print(question.question_title)
+        print(question.title)
         print(question.text)
-        for answer in question.answers:
+        for answer in question.title:
             print(answer.answer)
 ```
 
 ## Modes
 
-There's 2 modes : 
+There's 2 modes :
 
-* for web export (`qcm_part.from_file(filename, mode="web")`), the default one, `mode` named parameter can be ommitted.
-* for pdf export (`qcm_part.from_file(filename, mode="pdf")`).
+- for web export (`qcm_part.from_file(filename, mode="web")`), the default one, `mode` named parameter can be ommitted.
+- for pdf export (`qcm_part.from_file(filename, mode="pdf")`).
 
-The `mode=web` should be used if you want to serve a QCM like I do here.
+The `mode=web` should be used if you want to serve a QCM like I do [here](https://github.com/qkzk/qcm_alchemy)
 
 It replaces `markdown` syntax with `html` syntax using `markdown` module.
 
 The `mode=pdf` can be used to create a randomized QCM in a .md file, then to export it with pandoc.
 
 ## QCM file description
 
 **Files should be utf-8 encoded text files with .md extensions.**
 
 They should respect the [example](./example/example.md) format :
 
 ```markdown
-
 # title
 
 ## part
 
+the text of the part
+
 ### question with multiple choices
 
 optional sub text. Can contains code, latex, whatever
 
 - [x] right answer
 - [ ] wrong answer a
 - [ ] wrong answer b
 
-### question with text allowed 
+### question with text allowed
 
 - [t]
 ```
 
 ## Known limitations
 
 Only a little subset of markdown is supported.
 
 1. A title must be found
 2. title, parts and questions can't have empty string after `#`, `##` or `###` tag
 
-    ```mardown
-    ## valid part
+   ```mardown
+   ## valid part
+
+   ##
+   wrong part
+   ```
 
-    ## 
-    wrong part
-    ```
 3. Code blocks with triple backticks are supported not `~~~`. Those will creates bugs.
 
-    ~~~markdown
-    # title
-    
-    ## part
-
-    ### question
-
-    ```python
-    # comment
-    def f():
-        return 1
-    ```
-    ~~~
-
-    is valid.
-
-    but :
-
-    ```markdown
-    # title
-    
-    ## part
-
-    ### question
-
-    ~~~python
-    # comment
-    def f():
-        return 1
-    ~~~
-    
-    ```
+   ````markdown
+   # title
+
+   ## part
+
+   ### question
+
+   ```python
+   # comment
+   def f():
+       return 1
+   ```
+   ````
+
+   is valid.
+
+   but :
+
+   ````markdown
+   # title
+
+   ## part
+
+   ### question
+
+   ```python
+   # comment
+   def f():
+       return 1
+   ```
+   ````
+
+   ```
 
-    **is not valid.**
+   **is not valid.**
 
-    The `# comment` line will be interpreted as a new title etc.
+   The `# comment` line will be interpreted as a new title etc.
+   ```
```

### Comparing `qcm_parser-0.1.3/README.md` & `qcm_parser-0.1.4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # QCM parser
 
 It's a basic and quite strict QCM (Multiple Choices Questions) parser.
 
-It parses a file .md file into Python objects. 
+It parses a file .md file into Python objects.
 That's all.
 
 There's no rendering, no export. It must be done separetaly.
 
 ## Installation
 
 It requires python>=3.7 and `markdown` package.
@@ -31,108 +31,112 @@
 
 In memory, you `qcm` object is represented as a tree which holds parts.
 
 Those parts holds questions, holding answers.
 
 It is then easy to navigate through it like this :
 
-
 ```
 print(qcm.title)
 for part in qcm.parts:
     print(part.title)
+    print(part.text)
     for question in part.questions:
-        print(question.question_title)
+        print(question.title)
         print(question.text)
-        for answer in question.answers:
+        for answer in question.title:
             print(answer.answer)
 ```
 
 ## Modes
 
-There's 2 modes : 
+There's 2 modes :
 
-* for web export (`qcm_part.from_file(filename, mode="web")`), the default one, `mode` named parameter can be ommitted.
-* for pdf export (`qcm_part.from_file(filename, mode="pdf")`).
+- for web export (`qcm_part.from_file(filename, mode="web")`), the default one, `mode` named parameter can be ommitted.
+- for pdf export (`qcm_part.from_file(filename, mode="pdf")`).
 
-The `mode=web` should be used if you want to serve a QCM like I do here.
+The `mode=web` should be used if you want to serve a QCM like I do [here](https://github.com/qkzk/qcm_alchemy)
 
 It replaces `markdown` syntax with `html` syntax using `markdown` module.
 
 The `mode=pdf` can be used to create a randomized QCM in a .md file, then to export it with pandoc.
 
 ## QCM file description
 
 **Files should be utf-8 encoded text files with .md extensions.**
 
 They should respect the [example](./example/example.md) format :
 
 ```markdown
-
 # title
 
 ## part
 
+the text of the part
+
 ### question with multiple choices
 
 optional sub text. Can contains code, latex, whatever
 
 - [x] right answer
 - [ ] wrong answer a
 - [ ] wrong answer b
 
-### question with text allowed 
+### question with text allowed
 
 - [t]
 ```
 
 ## Known limitations
 
 Only a little subset of markdown is supported.
 
 1. A title must be found
 2. title, parts and questions can't have empty string after `#`, `##` or `###` tag
 
-    ```mardown
-    ## valid part
+   ```mardown
+   ## valid part
+
+   ##
+   wrong part
+   ```
 
-    ## 
-    wrong part
-    ```
 3. Code blocks with triple backticks are supported not `~~~`. Those will creates bugs.
 
-    ~~~markdown
-    # title
-    
-    ## part
-
-    ### question
-
-    ```python
-    # comment
-    def f():
-        return 1
-    ```
-    ~~~
-
-    is valid.
-
-    but :
-
-    ```markdown
-    # title
-    
-    ## part
-
-    ### question
-
-    ~~~python
-    # comment
-    def f():
-        return 1
-    ~~~
-    
-    ```
+   ````markdown
+   # title
+
+   ## part
+
+   ### question
+
+   ```python
+   # comment
+   def f():
+       return 1
+   ```
+   ````
+
+   is valid.
+
+   but :
+
+   ````markdown
+   # title
+
+   ## part
+
+   ### question
+
+   ```python
+   # comment
+   def f():
+       return 1
+   ```
+   ````
+
+   ```
 
-    **is not valid.**
+   **is not valid.**
 
-    The `# comment` line will be interpreted as a new title etc.
+   The `# comment` line will be interpreted as a new title etc.
+   ```
```

### Comparing `qcm_parser-0.1.3/setup.py` & `qcm_parser-0.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="qcm_parser",
-    version="0.1.3",
+    version="0.1.4",
     author="qkzk",
     author_email="qu3nt1n@gmail.com",
     description="A parser of QCM file",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/qkzk/qcm_parser",
     project_urls={
```

### Comparing `qcm_parser-0.1.3/src/qcm_parser/parser.py` & `qcm_parser-0.1.4/src/qcm_parser/parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 title: QCM parser
 author: qkzk
-date: 2021/06/28
+date: 2023/06/08
 """
 from typing import List, Tuple, Type
 
-from .string_parsers import StringParsers, WebParsers, PDFParsers
+from string_parsers import StringParsers, WebParsers, PDFParsers
 
 
 class ParseQCMError(Exception):
     """Exception raised when parsing went wrong."""
 
 
 class ParseQCM:
@@ -140,40 +140,64 @@
 
 class QCM_Part:
     """Holds a part of the QCM"""
 
     def __init__(self, lines: list, parsers: Type[StringParsers]):
         self._lines = lines
         self._parsers = parsers
-        self._start_questions, self._title = self._read_title()
+        self._start_text, self._title = self._read_title()
+        self._text, self._start_questions = self._read_text()
         self._questions_lines = self._read_questions()
         self._questions = [
             self._read_question(start, end) for start, end in self._questions_lines
         ]
 
     @property
     def title(self) -> str:
         """Part title"""
         return self._title
 
     @property
+    def text(self) -> str:
+        """Question sub text"""
+        return self._text
+
+    @property
     def questions(self) -> List["QCM_Question"]:
         """Questions in this part"""
         return self._questions
 
     def __repr__(self):
         return "".join(self._lines)
 
     def _read_title(self) -> tuple:
         """Read the title of the part and returns its position and content"""
         for index, line in enumerate(self._lines):
             if line.startswith("## "):
                 return index + 1, self._parsers.line(line[3:])
         raise QCM_PartError(f"No title found for this part : {self}")
 
+    def _read_text(self) -> Tuple[str, int]:
+        """
+        Read the 'text' of the question, the lines below the title and
+        before the answer.
+        """
+        for index, line in enumerate(
+            self._lines[self._start_text :], start=self._start_text
+        ):
+            if line.startswith("###"):
+                end = index
+                return (
+                    self._parsers.bloc(
+                        self._lines[self._start_text : end],
+                    ),
+                    end,
+                )
+        raise QCM_PartError(f"No text found for question {self}")
+
     def _read_questions(self) -> list:
         """Returns a list of line indexes questions"""
         questions = []
         is_code_block = False
         for index, line in enumerate(
             self._lines[self._start_questions :], start=self._start_questions
         ):
```

### Comparing `qcm_parser-0.1.3/src/qcm_parser/string_parsers.py` & `qcm_parser-0.1.4/src/qcm_parser/string_parsers.py`

 * *Files identical despite different names*

### Comparing `qcm_parser-0.1.3/src/qcm_parser.egg-info/PKG-INFO` & `qcm_parser-0.1.4/src/qcm_parser.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qcm-parser
-Version: 0.1.3
+Version: 0.1.4
 Summary: A parser of QCM file
 Home-page: https://github.com/qkzk/qcm_parser
 Author: qkzk
 Author-email: qu3nt1n@gmail.com
 Project-URL: Bug Tracker, https://github.com/qkzk/qcm_parser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # QCM parser
 
 It's a basic and quite strict QCM (Multiple Choices Questions) parser.
 
-It parses a file .md file into Python objects. 
+It parses a file .md file into Python objects.
 That's all.
 
 There's no rendering, no export. It must be done separetaly.
 
 ## Installation
 
 It requires python>=3.7 and `markdown` package.
@@ -46,108 +46,112 @@
 
 In memory, you `qcm` object is represented as a tree which holds parts.
 
 Those parts holds questions, holding answers.
 
 It is then easy to navigate through it like this :
 
-
 ```
 print(qcm.title)
 for part in qcm.parts:
     print(part.title)
+    print(part.text)
     for question in part.questions:
-        print(question.question_title)
+        print(question.title)
         print(question.text)
-        for answer in question.answers:
+        for answer in question.title:
             print(answer.answer)
 ```
 
 ## Modes
 
-There's 2 modes : 
+There's 2 modes :
 
-* for web export (`qcm_part.from_file(filename, mode="web")`), the default one, `mode` named parameter can be ommitted.
-* for pdf export (`qcm_part.from_file(filename, mode="pdf")`).
+- for web export (`qcm_part.from_file(filename, mode="web")`), the default one, `mode` named parameter can be ommitted.
+- for pdf export (`qcm_part.from_file(filename, mode="pdf")`).
 
-The `mode=web` should be used if you want to serve a QCM like I do here.
+The `mode=web` should be used if you want to serve a QCM like I do [here](https://github.com/qkzk/qcm_alchemy)
 
 It replaces `markdown` syntax with `html` syntax using `markdown` module.
 
 The `mode=pdf` can be used to create a randomized QCM in a .md file, then to export it with pandoc.
 
 ## QCM file description
 
 **Files should be utf-8 encoded text files with .md extensions.**
 
 They should respect the [example](./example/example.md) format :
 
 ```markdown
-
 # title
 
 ## part
 
+the text of the part
+
 ### question with multiple choices
 
 optional sub text. Can contains code, latex, whatever
 
 - [x] right answer
 - [ ] wrong answer a
 - [ ] wrong answer b
 
-### question with text allowed 
+### question with text allowed
 
 - [t]
 ```
 
 ## Known limitations
 
 Only a little subset of markdown is supported.
 
 1. A title must be found
 2. title, parts and questions can't have empty string after `#`, `##` or `###` tag
 
-    ```mardown
-    ## valid part
+   ```mardown
+   ## valid part
+
+   ##
+   wrong part
+   ```
 
-    ## 
-    wrong part
-    ```
 3. Code blocks with triple backticks are supported not `~~~`. Those will creates bugs.
 
-    ~~~markdown
-    # title
-    
-    ## part
-
-    ### question
-
-    ```python
-    # comment
-    def f():
-        return 1
-    ```
-    ~~~
-
-    is valid.
-
-    but :
-
-    ```markdown
-    # title
-    
-    ## part
-
-    ### question
-
-    ~~~python
-    # comment
-    def f():
-        return 1
-    ~~~
-    
-    ```
+   ````markdown
+   # title
+
+   ## part
+
+   ### question
+
+   ```python
+   # comment
+   def f():
+       return 1
+   ```
+   ````
+
+   is valid.
+
+   but :
+
+   ````markdown
+   # title
+
+   ## part
+
+   ### question
+
+   ```python
+   # comment
+   def f():
+       return 1
+   ```
+   ````
+
+   ```
 
-    **is not valid.**
+   **is not valid.**
 
-    The `# comment` line will be interpreted as a new title etc.
+   The `# comment` line will be interpreted as a new title etc.
+   ```
```

