# Comparing `tmp/mysmallutils-2.0.7.tar.gz` & `tmp/mysmallutils-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysmallutils-2.0.7.tar", last modified: Sat Jun  3 12:55:30 2023, max compression
+gzip compressed data, was "mysmallutils-2.0.8.tar", last modified: Thu Jun  8 14:20:22 2023, max compression
```

## Comparing `mysmallutils-2.0.7.tar` & `mysmallutils-2.0.8.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-03 12:55:30.182975 mysmallutils-2.0.7/
--rw-rw-rw-   0        0        0    59645 2023-06-03 12:55:30.181975 mysmallutils-2.0.7/PKG-INFO
--rw-rw-rw-   0        0        0    59163 2023-06-03 12:54:04.000000 mysmallutils-2.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-03 12:55:30.096162 mysmallutils-2.0.7/mysmallutils.egg-info/
--rw-rw-rw-   0        0        0    59645 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-03 12:55:29.000000 mysmallutils-2.0.7/mysmallutils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-03 12:55:30.178658 mysmallutils-2.0.7/mysutils/
--rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/__init__.py
--rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.7/mysutils/collections.py
--rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/command.py
--rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/config.py
--rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/fastapi.py
--rw-rw-rw-   0        0        0    26268 2023-06-03 12:41:08.000000 mysmallutils-2.0.7/mysutils/file.py
--rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/logging.py
--rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/method.py
--rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/misc.py
--rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/request.py
--rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/service.py
--rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.7/mysutils/tar.py
--rw-rw-rw-   0        0        0    10988 2023-06-03 12:53:32.000000 mysmallutils-2.0.7/mysutils/text.py
--rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.7/mysutils/tmp.py
--rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/unittest.py
--rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.7/mysutils/web.py
--rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.7/mysutils/yaml.py
--rw-rw-rw-   0        0        0       42 2023-06-03 12:55:30.183969 mysmallutils-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1711 2023-05-24 14:01:37.000000 mysmallutils-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 14:20:22.704259 mysmallutils-2.0.8/
+-rw-rw-rw-   0        0        0    60363 2023-06-08 14:20:22.704259 mysmallutils-2.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0    59881 2023-06-08 14:18:49.000000 mysmallutils-2.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 14:20:22.540732 mysmallutils-2.0.8/mysmallutils.egg-info/
+-rw-rw-rw-   0        0        0    60363 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 14:20:22.701259 mysmallutils-2.0.8/mysutils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/__init__.py
+-rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.8/mysutils/collections.py
+-rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/command.py
+-rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/config.py
+-rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/fastapi.py
+-rw-rw-rw-   0        0        0    26268 2023-06-03 12:41:08.000000 mysmallutils-2.0.8/mysutils/file.py
+-rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/logging.py
+-rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/method.py
+-rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/misc.py
+-rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/request.py
+-rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/service.py
+-rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.8/mysutils/tar.py
+-rw-rw-rw-   0        0        0    11276 2023-06-08 12:19:58.000000 mysmallutils-2.0.8/mysutils/text.py
+-rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.8/mysutils/tmp.py
+-rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/unittest.py
+-rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/web.py
+-rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.8/mysutils/yaml.py
+-rw-rw-rw-   0        0        0       42 2023-06-08 14:20:22.704259 mysmallutils-2.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1711 2023-06-03 12:59:04.000000 mysmallutils-2.0.8/setup.py
```

### Comparing `mysmallutils-2.0.7/PKG-INFO` & `mysmallutils-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.7
+Version: 2.0.8
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -34,14 +34,16 @@
   * [Find URLs](#find-urls)
   * [Get URLs](#get-urls)
   * [Remove URLs](#remove-urls)
   * [Replace URLs](#replace-urls)
   * [Check URLs in a text](#check-urls-in-a-text)
   * [Clean text](#clean-text)
   * [Text markup](#text-markup)
+  * [Hash a text](#hash-a-text)
+  * [Is float](#is-float)
 * [File access, load and save files](#file-access-load-and-save-files)
   * [Open files](#open-files)
   * [Read file](#read-file)
   * [Write in a file](#write-in-a-file)
   * [Load and save json files](#load-and-save-json-files)
   * [Load and save pickle files](#load-and-save-pickle-files)
   * [Load and save Yaml files](#load-and-save-yaml-files)
@@ -797,23 +799,43 @@
       markup('text', AnsiCodes.UNDERLINE, 
              color(255, 255, 20), 
              bg_color(60, 60, 60),
              un_color(80, 80, 255)) + 'with effects.')
 ```
 **Important note:** All these font variants, styles and color do not work in all the consoles/terminals.
 
-## Hash a text
+## Hash a text<a id="hash-a-text" name="hash-a-text"></a>
 
-An very easy way to hash a text.
+A very easy way to hash a text.
 
 ```python
 from mysutils.text import hash_text
 
-# Print the SHA256 hash of that text
+# Print the SHA256 hash of that text in utf-8
 print(hash_text('This is a text'))
+
+# Print the SHA256 hash of that text in iso8859-1
+print(hash_text('This is a text', encoding='iso8859-1'))
+```
+
+## Is float<a id="is-float" name="is-float"></a>
+
+Check when a string is a float valid number or not.
+
+```python
+from mysutils.text import is_float
+
+print(is_float('1.23'))  # Print True
+print(is_float('3.14159'))  # Print True
+print(is_float('1.23e6'))  # Print True
+print(is_float('3.45e-2'))  # Print True
+print(is_float(Fraction(22, 7)))  # Print True
+print(is_float('123'))  # Print True
+print(is_float('1,234'))  # Print  False
+print(is_float('a1234'))  # Print False
 ```
 
 # File access, load and save files<a id="file-access-load-and-save-files" name="file-access-load-and-save-files"></a>
 With these functions you can open files, create json and pickle files, and execute external commands very easily.
 Moreover, only changing the file extension you can store the information in a compressed file with gzip.
 
 ## Open files<a id="open-files" name="open-files"></a>
```

### Comparing `mysmallutils-2.0.7/README.md` & `mysmallutils-2.0.8/mysmallutils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,21 @@
+Metadata-Version: 2.1
+Name: mysmallutils
+Version: 2.0.8
+Summary: Small Python utils to do life easier.
+Home-page: https://github.com/jmgomezsoriano/mysmallutils
+Author: José Manuel Gómez Soriano
+Author-email: jmgomez.soriano@gmail.com
+License: LGPL2
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.10,<4
+Description-Content-Type: text/markdown
+
 # MySmallUtils
 Small Python utils to do life easier.
 
 This includes tools to execute external commands, compress files,
 manage configuration files, open different types of files (JSON, YAML and Pickle) compressed or not,
 configure logging, obtain metrics, download files, etc.
 
@@ -20,14 +34,16 @@
   * [Find URLs](#find-urls)
   * [Get URLs](#get-urls)
   * [Remove URLs](#remove-urls)
   * [Replace URLs](#replace-urls)
   * [Check URLs in a text](#check-urls-in-a-text)
   * [Clean text](#clean-text)
   * [Text markup](#text-markup)
+  * [Hash a text](#hash-a-text)
+  * [Is float](#is-float)
 * [File access, load and save files](#file-access-load-and-save-files)
   * [Open files](#open-files)
   * [Read file](#read-file)
   * [Write in a file](#write-in-a-file)
   * [Load and save json files](#load-and-save-json-files)
   * [Load and save pickle files](#load-and-save-pickle-files)
   * [Load and save Yaml files](#load-and-save-yaml-files)
@@ -783,23 +799,43 @@
       markup('text', AnsiCodes.UNDERLINE, 
              color(255, 255, 20), 
              bg_color(60, 60, 60),
              un_color(80, 80, 255)) + 'with effects.')
 ```
 **Important note:** All these font variants, styles and color do not work in all the consoles/terminals.
 
-## Hash a text
+## Hash a text<a id="hash-a-text" name="hash-a-text"></a>
 
-An very easy way to hash a text.
+A very easy way to hash a text.
 
 ```python
 from mysutils.text import hash_text
 
-# Print the SHA256 hash of that text
+# Print the SHA256 hash of that text in utf-8
 print(hash_text('This is a text'))
+
+# Print the SHA256 hash of that text in iso8859-1
+print(hash_text('This is a text', encoding='iso8859-1'))
+```
+
+## Is float<a id="is-float" name="is-float"></a>
+
+Check when a string is a float valid number or not.
+
+```python
+from mysutils.text import is_float
+
+print(is_float('1.23'))  # Print True
+print(is_float('3.14159'))  # Print True
+print(is_float('1.23e6'))  # Print True
+print(is_float('3.45e-2'))  # Print True
+print(is_float(Fraction(22, 7)))  # Print True
+print(is_float('123'))  # Print True
+print(is_float('1,234'))  # Print  False
+print(is_float('a1234'))  # Print False
 ```
 
 # File access, load and save files<a id="file-access-load-and-save-files" name="file-access-load-and-save-files"></a>
 With these functions you can open files, create json and pickle files, and execute external commands very easily.
 Moreover, only changing the file extension you can store the information in a compressed file with gzip.
 
 ## Open files<a id="open-files" name="open-files"></a>
@@ -1781,8 +1817,8 @@
 
 # You can do
 conditional(my_func, a > b, 1, 'apple', c='Lucas')
 ```
 
 # How to collaborate
 
-I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
+I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mysmallutils-2.0.7/mysmallutils.egg-info/PKG-INFO` & `mysmallutils-2.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: mysmallutils
-Version: 2.0.7
-Summary: Small Python utils to do life easier.
-Home-page: https://github.com/jmgomezsoriano/mysmallutils
-Author: José Manuel Gómez Soriano
-Author-email: jmgomez.soriano@gmail.com
-License: LGPL2
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10,<4
-Description-Content-Type: text/markdown
-
 # MySmallUtils
 Small Python utils to do life easier.
 
 This includes tools to execute external commands, compress files,
 manage configuration files, open different types of files (JSON, YAML and Pickle) compressed or not,
 configure logging, obtain metrics, download files, etc.
 
@@ -34,14 +20,16 @@
   * [Find URLs](#find-urls)
   * [Get URLs](#get-urls)
   * [Remove URLs](#remove-urls)
   * [Replace URLs](#replace-urls)
   * [Check URLs in a text](#check-urls-in-a-text)
   * [Clean text](#clean-text)
   * [Text markup](#text-markup)
+  * [Hash a text](#hash-a-text)
+  * [Is float](#is-float)
 * [File access, load and save files](#file-access-load-and-save-files)
   * [Open files](#open-files)
   * [Read file](#read-file)
   * [Write in a file](#write-in-a-file)
   * [Load and save json files](#load-and-save-json-files)
   * [Load and save pickle files](#load-and-save-pickle-files)
   * [Load and save Yaml files](#load-and-save-yaml-files)
@@ -797,23 +785,43 @@
       markup('text', AnsiCodes.UNDERLINE, 
              color(255, 255, 20), 
              bg_color(60, 60, 60),
              un_color(80, 80, 255)) + 'with effects.')
 ```
 **Important note:** All these font variants, styles and color do not work in all the consoles/terminals.
 
-## Hash a text
+## Hash a text<a id="hash-a-text" name="hash-a-text"></a>
 
-An very easy way to hash a text.
+A very easy way to hash a text.
 
 ```python
 from mysutils.text import hash_text
 
-# Print the SHA256 hash of that text
+# Print the SHA256 hash of that text in utf-8
 print(hash_text('This is a text'))
+
+# Print the SHA256 hash of that text in iso8859-1
+print(hash_text('This is a text', encoding='iso8859-1'))
+```
+
+## Is float<a id="is-float" name="is-float"></a>
+
+Check when a string is a float valid number or not.
+
+```python
+from mysutils.text import is_float
+
+print(is_float('1.23'))  # Print True
+print(is_float('3.14159'))  # Print True
+print(is_float('1.23e6'))  # Print True
+print(is_float('3.45e-2'))  # Print True
+print(is_float(Fraction(22, 7)))  # Print True
+print(is_float('123'))  # Print True
+print(is_float('1,234'))  # Print  False
+print(is_float('a1234'))  # Print False
 ```
 
 # File access, load and save files<a id="file-access-load-and-save-files" name="file-access-load-and-save-files"></a>
 With these functions you can open files, create json and pickle files, and execute external commands very easily.
 Moreover, only changing the file extension you can store the information in a compressed file with gzip.
 
 ## Open files<a id="open-files" name="open-files"></a>
@@ -1795,8 +1803,8 @@
 
 # You can do
 conditional(my_func, a > b, 1, 'apple', c='Lucas')
 ```
 
 # How to collaborate
 
-I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
+I you want to collaborate with this project, please, <a href="mailto:jmgomez.soriano@gmail.com">contact with me</a>.
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `mysmallutils-2.0.7/mysutils/collections.py` & `mysmallutils-2.0.8/mysutils/collections.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/command.py` & `mysmallutils-2.0.8/mysutils/command.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/config.py` & `mysmallutils-2.0.8/mysutils/config.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/fastapi.py` & `mysmallutils-2.0.8/mysutils/fastapi.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/file.py` & `mysmallutils-2.0.8/mysutils/file.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/logging.py` & `mysmallutils-2.0.8/mysutils/logging.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/method.py` & `mysmallutils-2.0.8/mysutils/method.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/request.py` & `mysmallutils-2.0.8/mysutils/request.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/service.py` & `mysmallutils-2.0.8/mysutils/service.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/tar.py` & `mysmallutils-2.0.8/mysutils/tar.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/text.py` & `mysmallutils-2.0.8/mysutils/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,7 +281,19 @@
 def hash_text(text: str, encoding='utf-8') -> str:
     """ Hash the text with SHA256.
     :param text: The text to hash.
     :param encoding: The encoding to convert to bytes.
     :return: A SHA256 hash that represents that text.
     """
     return sha256(text.encode(encoding)).hexdigest()
+
+
+def is_float(value: str) -> bool:
+    """ Check if a value is a float.
+    :param value: The value to evaluate.
+    :return: True if the value is a float, False otherwise.
+    """
+    try:
+        float(value)
+        return True
+    except ValueError:
+        return False
```

### Comparing `mysmallutils-2.0.7/mysutils/tmp.py` & `mysmallutils-2.0.8/mysutils/tmp.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/unittest.py` & `mysmallutils-2.0.8/mysutils/unittest.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/web.py` & `mysmallutils-2.0.8/mysutils/web.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/mysutils/yaml.py` & `mysmallutils-2.0.8/mysutils/yaml.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.7/setup.py` & `mysmallutils-2.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 setuptools.setup(
     cmdclass={
         'clean': CleanCommand,
         'prepublish': PrepublishCommand,
     },
     name='mysmallutils',
-    version='2.0.7',
+    version='2.0.8',
     url='https://github.com/jmgomezsoriano/mysmallutils',
     license='LGPL2',
     author='José Manuel Gómez Soriano',
     author_email='jmgomez.soriano@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Small Python utils to do life easier.',
```

