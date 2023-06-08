# Comparing `tmp/tetun_tokenizer-1.1.2.tar.gz` & `tmp/tetun_tokenizer-1.1.3.tar.gz`

## Comparing `tetun_tokenizer-1.1.2.tar` & `tetun_tokenizer-1.1.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/.DS_Store
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/Pipfile
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/Pipfile.lock
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/_token
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/.vscode/settings.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/tetuntokenizer/__init__.py
--rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/tetuntokenizer/tetun_patterns.py
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/tetuntokenizer/tokenizer.py
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/LICENSE
--rw-r--r--   0        0        0     5079 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/README.md
--rw-r--r--   0        0        0      438 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     5457 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/.DS_Store
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/Pipfile
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/Pipfile.lock
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/_token
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/tetuntokenizer/__init__.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/tetuntokenizer/tetun_patterns.py
+-rw-r--r--   0        0        0     3222 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/tetuntokenizer/tokenizer.py
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/LICENSE
+-rw-r--r--   0        0        0     5265 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/README.md
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5721 2020-02-02 00:00:00.000000 tetun_tokenizer-1.1.3/PKG-INFO
```

### Comparing `tetun_tokenizer-1.1.2/.DS_Store` & `tetun_tokenizer-1.1.3/.DS_Store`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.2/Pipfile.lock` & `tetun_tokenizer-1.1.3/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.2/tetuntokenizer/tetun_patterns.py` & `tetun_tokenizer-1.1.3/tetuntokenizer/tetun_patterns.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import re
 
 
-""" This file contains all the regular expressions for the Tetun tokenizer. """
+""" This module contains all the regular expressions for the Tetun tokenizer. """
 
 # E.g.: Ataúru, ne'ebé, ida-ne'ebé, Ofisiál, Ângela, Conceição, Kompañia, etc.
 TETUN_TEXT_PATTERN = r"[A-Za-zÂÁÃâáãÉÊéêÍíÓóÚúÑñÇç]+(?:[-’'][A-Za-zÂÁÃâáãÉÊéêÍíÓóÚúÑñÇç]+)*"
 
 # E.g.: 20.000.000.000,45 or 20,000,000,000.45.
-# E.g.; char ',' or '.' followed digits will be ignored.
+# E.g.; char ',' or '.' at the end of digits will be ignored.
 DIGITS_PATTERN = r"\d+(?:[,.]\d+)*"
 
 # These punctuations and symbols will be tokenized as a token in the Tetun standard tokenizer.
 PUNCTUATIONS_SYMBOLS = '!,./:;?"“”()[\\]^_`{|}#&§©°$€£μ@*+÷%<=>«»~'
 PUNCTUATIONS_SYMBOLS_PATTERN = r"[" + \
     re.escape("".join(PUNCTUATIONS_SYMBOLS)) + "]"
```

### Comparing `tetun_tokenizer-1.1.2/tetuntokenizer/tokenizer.py` & `tetun_tokenizer-1.1.3/tetuntokenizer/tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 """
 import re
 from typing import List
 from . import tetun_patterns
 
 
 class TetunRegexTokenizer:
-    """Tokenizes text using regular expressions."""
+    """ The base tokenizer class. """
 
     def __init__(self, patterns: str, split: bool = False) -> None:
         """
-        :param patterns: a regular expression to match the tokens.
+        :param patterns: regular expression patterns to match the tokens.
         :param split: if True, use re.split() to tokenize text, else use re.findall().            
         """
         self.patterns = patterns
         self.split = split
 
     def tokenize(self, text: str) -> List[str]:
         """ 
@@ -53,15 +53,15 @@
 
     def __init__(self) -> None:
         patterns = f"{tetun_patterns.WHITESPACE_PATTERNS}"
         super().__init__(patterns, split=True)
 
 
 class TetunSentenceTokenizer(TetunRegexTokenizer):
-    """ Tokenize sentence by .?! delimiters. """
+    """ Tokenize text by .?! delimiters. """
 
     def __init__(self) -> None:
         patterns = f"{tetun_patterns.SENTENCE_DELIMITER_PATTERN}"
         super().__init__(patterns, split=True)
 
 
 class TetunBlankLineTokenizer(TetunRegexTokenizer):
```

### Comparing `tetun_tokenizer-1.1.2/LICENSE` & `tetun_tokenizer-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tetun_tokenizer-1.1.2/README.md` & `tetun_tokenizer-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ### Tetun Tokenizer
 
-Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built along with this package as follows:
+Tetun tokenizer is a Python package used to tokenize an input text into tokens. There are several tokenization techniques we built along with this package as follows:
 1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
 2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
-3. `TetunSentenceTokenizer()`: tokenize the input text by `.?!` delimiters.
+3. `TetunSentenceTokenizer()`: tokenize the input text by period (.), question mark (?) and exclamation mark (!) delimiters.
 4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
 5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
 6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
 
 ### Installation
 
 To install Tetun tokenizer, run the following command in your console:
@@ -25,15 +25,15 @@
 It also supports `conda` and `pipenv` or similar commands.
 
 
 ### Usage
 
 To use Tetun tokenizer, `from` the `tokenizer` module on the `tetuntokenizer` package, `import` a tokenizer class. Instantiate the imported class and then call a `tokenize` function as follows:
 
-1. Using  `TetunStandardTokenizer()` to tokenize a given text.
+1. Using  `TetunStandardTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunStandardTokenizer
 
 tetun_tokenizer = TetunStandardTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -43,15 +43,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", '.', "Ha'u", 'iha', '$', '0.25', 'atu', 'fó', 'ba', 'ita', '.']
 ```
 
-2. Using `TetunWhiteSpaceTokenizer()` to tokenize a given text.
+2. Using `TetunWhiteSpaceTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWhiteSpaceTokenizer
 
 tetun_tokenizer = TetunWhiteSpaceTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -61,15 +61,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak.", "Ha'u", 'iha', '$0.25', 'atu', 'fó', 'ba', 'ita.']
 ```
 
-3. Using `TetunSentenceTokenizer()` to tokenize a given text.
+3. Using `TetunSentenceTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSentenceTokenizer
 
 tetun_tokenizer = TetunSentenceTokenizer()
 
 text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ga? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
@@ -79,15 +79,15 @@
 
 The output will be:
 
 ```
 ["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ga?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
 ```
 
-4. Using `TetunBlankLineTokenizer()` to tokenize a given text.
+4. Using `TetunBlankLineTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
 
 tetun_tokenizer = TetunBlankLineTokenizer()
 
 text = """
@@ -118,15 +118,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', '0.25', 'atu', 'fó', 'ba', 'ita']
 ```
 
-6. Using `TetunWordTokenizer()` to tokenize a given text.
+6. Using `TetunWordTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWordTokenizer
 
 tetun_tokenizer = TetunWordTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -136,15 +136,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', 'atu', 'fó', 'ba', 'ita']
 ```
 
-To print the resulting output to the console, with each element on a new line, you can use `for` loop or simply use `join()` as follows:
+To print the resulting output in the console, with each element on a new line, you can use `for` loop or simply use `join()` as follows:
 
 ```
 print('\n'.join(output))
 ```
 
 The output will be:
 
@@ -196,8 +196,10 @@
 dezenvolve
 ha'u-nia
 lian
 tetun 
 ...
 ```
 
-There are a few more ways to read file contents that you can use to achieve the same output.
+There are a few more ways to read file contents that you can use to achieve the same output.
+
+For the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-tokenizer) for this project.
```

### Comparing `tetun_tokenizer-1.1.2/PKG-INFO` & `tetun_tokenizer-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: tetun_tokenizer
-Version: 1.1.2
+Version: 1.1.3
 Summary: Tetun tokenizer
+Project-URL: repository, https://github.com/borulilitimornews/tetun-tokenizer
 Author-email: Gabriel de Jesus <gabriel.dejesus@timornews.tl>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ### Tetun Tokenizer
 
-Tetun tokenizer is a Python package for tokenizing an input text into tokens. There are several tokenization techniques we built along with this package as follows:
+Tetun tokenizer is a Python package used to tokenize an input text into tokens. There are several tokenization techniques we built along with this package as follows:
 1. `TetunStandardTokenizer()`: tokenize the input text by `word`, `punctuations`, and `special characters`.
 2. `TetunWhiteSpaceTokenizer()`: tokenize the input text by `whitespace` delimiter.
-3. `TetunSentenceTokenizer()`: tokenize the input text by `.?!` delimiters.
+3. `TetunSentenceTokenizer()`: tokenize the input text by period (.), question mark (?) and exclamation mark (!) delimiters.
 4. `TetunBlankLineTokenizer()`: tokenize the input text by `blank lines` delimiter.
 5. `TetunSimpleTokenizer()`: tokenize the input text by extracting `only string and number` and ignore punctuations and special characters.
 6. `TetunWordTokenizer()`: tokenize the input text by extracting `only string` and ignore numbers, punctuations, and special characters.
 
 ### Installation
 
 To install Tetun tokenizer, run the following command in your console:
@@ -37,15 +38,15 @@
 It also supports `conda` and `pipenv` or similar commands.
 
 
 ### Usage
 
 To use Tetun tokenizer, `from` the `tokenizer` module on the `tetuntokenizer` package, `import` a tokenizer class. Instantiate the imported class and then call a `tokenize` function as follows:
 
-1. Using  `TetunStandardTokenizer()` to tokenize a given text.
+1. Using  `TetunStandardTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunStandardTokenizer
 
 tetun_tokenizer = TetunStandardTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -55,15 +56,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", '.', "Ha'u", 'iha', '$', '0.25', 'atu', 'fó', 'ba', 'ita', '.']
 ```
 
-2. Using `TetunWhiteSpaceTokenizer()` to tokenize a given text.
+2. Using `TetunWhiteSpaceTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWhiteSpaceTokenizer
 
 tetun_tokenizer = TetunWhiteSpaceTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -73,15 +74,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak.", "Ha'u", 'iha', '$0.25', 'atu', 'fó', 'ba', 'ita.']
 ```
 
-3. Using `TetunSentenceTokenizer()` to tokenize a given text.
+3. Using `TetunSentenceTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunSentenceTokenizer
 
 tetun_tokenizer = TetunSentenceTokenizer()
 
 text = "Ha'u ema-ida ne'ebé baibain de'it. Tebes ga? Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!"
@@ -91,15 +92,15 @@
 
 The output will be:
 
 ```
 ["Ha'u ema-ida ne'ebé baibain de'it.", 'Tebes ga?', 'Ita-nia maluk Dr. ka Ph.D sira hosi U.S.A mós dehan!']
 ```
 
-4. Using `TetunBlankLineTokenizer()` to tokenize a given text.
+4. Using `TetunBlankLineTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunBlankLineTokenizer
 
 tetun_tokenizer = TetunBlankLineTokenizer()
 
 text = """
@@ -130,15 +131,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', '0.25', 'atu', 'fó', 'ba', 'ita']
 ```
 
-6. Using `TetunWordTokenizer()` to tokenize a given text.
+6. Using `TetunWordTokenizer()` to tokenize the input text.
 
 ```python
 from tetuntokenizer.tokenizer import TetunWordTokenizer
 
 tetun_tokenizer = TetunWordTokenizer()
 
 text = "Ha'u mak ita-nia maluk di'ak. Ha'u iha $0.25 atu fó ba ita."
@@ -148,15 +149,15 @@
 
 The output will be:
 
 ```
 ["Ha'u", 'mak', 'ita-nia', 'maluk', "di'ak", "Ha'u", 'iha', 'atu', 'fó', 'ba', 'ita']
 ```
 
-To print the resulting output to the console, with each element on a new line, you can use `for` loop or simply use `join()` as follows:
+To print the resulting output in the console, with each element on a new line, you can use `for` loop or simply use `join()` as follows:
 
 ```
 print('\n'.join(output))
 ```
 
 The output will be:
 
@@ -208,8 +209,10 @@
 dezenvolve
 ha'u-nia
 lian
 tetun 
 ...
 ```
 
-There are a few more ways to read file contents that you can use to achieve the same output.
+There are a few more ways to read file contents that you can use to achieve the same output.
+
+For the source code, visit the [GitHub repository](https://github.com/borulilitimornews/tetun-tokenizer) for this project.
```

