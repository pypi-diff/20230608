# Comparing `tmp/worddfn-0.1.0rc1.tar.gz` & `tmp/worddfn-0.1.1.tar.gz`

## Comparing `worddfn-0.1.0rc1.tar` & `worddfn-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/worddfn/__init__.py
--rw-r--r--   0        0        0    23198 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/worddfn/__main__.py
--rw-r--r--   0        0        0     3859 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/worddfn/dictionaryAPI.py
--rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/worddfn/setting.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/.gitignore
--rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/LICENSE
--rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/README.md
--rw-r--r--   0        0        0     1025 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/pyproject.toml
--rw-r--r--   0        0        0     9084 2020-02-02 00:00:00.000000 worddfn-0.1.0rc1/PKG-INFO
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/__init__.py
+-rw-r--r--   0        0        0    23239 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/__main__.py
+-rw-r--r--   0        0        0     3861 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/dictionaryAPI.py
+-rw-r--r--   0        0        0     2465 2020-02-02 00:00:00.000000 worddfn-0.1.1/worddfn/setting.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 worddfn-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1077 2020-02-02 00:00:00.000000 worddfn-0.1.1/LICENSE
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 worddfn-0.1.1/README.md
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 worddfn-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7847 2020-02-02 00:00:00.000000 worddfn-0.1.1/PKG-INFO
```

### Comparing `worddfn-0.1.0rc1/worddfn/__main__.py` & `worddfn-0.1.1/worddfn/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
 
                     else:
                         # save data to cache:
                         _cache_data(filePath, ant_result, word, key)
                         # word = _pclp.copy("")
 
     elif word == "":
-        print(f"Using cli argument")
+        print(f"Using cli argument\nrun word -h to view how to run commands")
 
         # Args return from args_handler function.
         words = args_handler()
 
         for k, w in words.items():
             if w != None:
                 key = k
```

### Comparing `worddfn-0.1.0rc1/worddfn/dictionaryAPI.py` & `worddfn-0.1.1/worddfn/dictionaryAPI.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
                     parameters = {
                         "relationshipTypes": "verb-form",
                         "limitPerRelationshipType": limit_relations,
                     }
 
                 # Check to see if the querry is compose of only string.
                 elif val.isalpha():
-                    print(type(val))  # test code
+                    # print(type(val))  # test code
                     word_relations: str = query[0]
 
                     parameters = {
                         "relationshipTypes": word_relations,
                         "limitPerRelationshipType": "5",
                     }
```

### Comparing `worddfn-0.1.0rc1/worddfn/setting.py` & `worddfn-0.1.1/worddfn/setting.py`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.0rc1/LICENSE` & `worddfn-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.0rc1/README.md` & `worddfn-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `worddfn-0.1.0rc1/pyproject.toml` & `worddfn-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 name = "worddfn"
 authors = [
   { name="Shall Mcfield", email="xhall.mc@protonmail.com" },
 ]
 description = "worddfn, lookup word meaning and forms via the wordnik api"
 readme = "README.md"
 requires-python = ">=3.8"
-license = {file = "LICENSE"}
+license = {text = "MIT"}
 classifiers = [
     "Intended Audience :: Information Technology",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python",
     "Operating System :: OS Independent",
     "Topic :: Internet",
     "Development Status :: 4 - Beta",
```

### Comparing `worddfn-0.1.0rc1/PKG-INFO` & `worddfn-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,15 @@
 Metadata-Version: 2.1
 Name: worddfn
-Version: 0.1.0rc1
+Version: 0.1.1
 Summary: worddfn, lookup word meaning and forms via the wordnik api
 Project-URL: Homepage, https://github.com/SirX7/wordDFN
 Project-URL: Bug Tracker, https://github.com/SirX7/wordDFN/issues
 Author-email: Shall Mcfield <xhall.mc@protonmail.com>
-License: MIT License
-        
-        Copyright (c) 2023-present Shall Mcfield
-        
-        Permission is hereby granted, free of charge, to any person obtaining a copy
-        of this software and associated documentation files (the "Software"), to deal
-        in the Software without restriction, including without limitation the rights
-        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-        copies of the Software, and to permit persons to whom the Software is
-        furnished to do so, subject to the following conditions:
-        
-        The above copyright notice and this permission notice shall be included in all
-        copies or substantial portions of the Software.
-        
-        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-        SOFTWARE.
+License: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

