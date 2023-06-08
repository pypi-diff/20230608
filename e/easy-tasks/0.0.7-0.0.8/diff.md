# Comparing `tmp/easy_tasks-0.0.7.tar.gz` & `tmp/easy_tasks-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_tasks-0.0.7.tar", last modified: Sat Jan  7 17:58:38 2023, max compression
+gzip compressed data, was "easy_tasks-0.0.8.tar", last modified: Thu Jun  8 16:01:58 2023, max compression
```

## Comparing `easy_tasks-0.0.7.tar` & `easy_tasks-0.0.8.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-01-07 17:58:38.042375 easy_tasks-0.0.7/
--rw-rw-rw-   0        0        0     1095 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/LICENSE
--rw-rw-rw-   0        0        0      137 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2755 2023-01-07 17:58:38.042375 easy_tasks-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     2040 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-01-07 17:58:38.044375 easy_tasks-0.0.7/easy_tasks/
--rw-rw-rw-   0        0        0      607 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/easy_tasks/__init__.py
--rw-rw-rw-   0        0        0      518 2023-01-07 17:58:38.044375 easy_tasks-0.0.7/easy_tasks/_version.py
--rw-rw-rw-   0        0        0      542 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/easy_tasks/closest_furthest_value.py
--rw-rw-rw-   0        0        0     2223 2023-01-07 16:48:18.000000 easy_tasks-0.0.7/easy_tasks/dublicates.py
--rw-rw-rw-   0        0        0      735 2022-07-27 22:28:07.000000 easy_tasks-0.0.7/easy_tasks/help_with_json.py
--rw-rw-rw-   0        0        0      618 2023-01-07 17:20:37.000000 easy_tasks-0.0.7/easy_tasks/help_with_pickle.py
--rw-rw-rw-   0        0        0     3614 2023-01-07 16:53:43.000000 easy_tasks-0.0.7/easy_tasks/percentage.py
--rw-rw-rw-   0        0        0      338 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/easy_tasks/sorter.py
--rw-rw-rw-   0        0        0     1437 2023-01-07 16:48:45.000000 easy_tasks-0.0.7/easy_tasks/string_transformation.py
--rw-rw-rw-   0        0        0      235 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/easy_tasks/unpack.py
-drwxrwxrwx   0        0        0        0 2023-01-07 17:58:38.041375 easy_tasks-0.0.7/easy_tasks.egg-info/
--rw-rw-rw-   0        0        0     2755 2023-01-07 17:58:37.000000 easy_tasks-0.0.7/easy_tasks.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      522 2023-01-07 17:58:37.000000 easy_tasks-0.0.7/easy_tasks.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-07 17:58:37.000000 easy_tasks-0.0.7/easy_tasks.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2023-01-07 17:58:37.000000 easy_tasks-0.0.7/easy_tasks.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-01-07 17:58:37.000000 easy_tasks-0.0.7/easy_tasks.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      210 2023-01-07 17:58:38.043375 easy_tasks-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0     1886 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/setup.py
--rw-rw-rw-   0        0        0    85451 2023-01-07 16:40:31.000000 easy_tasks-0.0.7/versioneer.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:01:58.388882 easy_tasks-0.0.8/
+-rw-rw-rw-   0        0        0     1095 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/LICENSE
+-rw-rw-rw-   0        0        0       82 2023-01-17 17:17:39.000000 easy_tasks-0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0     3118 2023-06-08 16:01:58.387879 easy_tasks-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2402 2023-02-14 21:25:45.000000 easy_tasks-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 16:01:58.379875 easy_tasks-0.0.8/easy_tasks/
+-rw-rw-rw-   0        0        0      742 2023-06-08 16:00:31.000000 easy_tasks-0.0.8/easy_tasks/__init__.py
+-rw-rw-rw-   0        0        0      542 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/closest_furthest_value.py
+-rw-rw-rw-   0        0        0     2223 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/dublicates.py
+-rw-rw-rw-   0        0        0      735 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/help_with_json.py
+-rw-rw-rw-   0        0        0      618 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/help_with_pickle.py
+-rw-rw-rw-   0        0        0     3627 2023-01-17 17:22:26.000000 easy_tasks-0.0.8/easy_tasks/list_printer.py
+-rw-rw-rw-   0        0        0     3614 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/percentage.py
+-rw-rw-rw-   0        0        0      338 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/sorter.py
+-rw-rw-rw-   0        0        0     1437 2023-01-07 18:12:34.000000 easy_tasks-0.0.8/easy_tasks/string_transformation.py
+-rw-rw-rw-   0        0        0      654 2023-05-16 22:05:16.000000 easy_tasks-0.0.8/easy_tasks/unpack.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:01:58.386876 easy_tasks-0.0.8/easy_tasks.egg-info/
+-rw-rw-rw-   0        0        0     3118 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-08 16:01:58.000000 easy_tasks-0.0.8/easy_tasks.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:01:58.388882 easy_tasks-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1809 2023-06-08 16:00:23.000000 easy_tasks-0.0.8/setup.py
```

### Comparing `easy_tasks-0.0.7/LICENSE` & `easy_tasks-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/PKG-INFO` & `easy_tasks-0.0.8/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,76 +1,59 @@
-Metadata-Version: 2.1
-Name: easy_tasks
-Version: 0.0.7
-Summary: Normal python class tasks like sorting, closet/furthest value, dublicates, ...
-Author: André Herber
-Author-email: andre.herber.programming@gmail.com
-Keywords: python
-Classifier: Development Status :: 1 - Planning
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-
-# easy_taks
-
-To not get annoyed by simple recurring tasks I created this small library.  
-
-## Content
-- Installation
-- Usage  
-
-## Installation
-- `pip install easy-tasks`
-
-## Usage
-- `furthest_value_in_list`  
-  Function returning the closest number of a list to a given value
-
-- `closest_value_in_list`  
-  Function returning the closest number of a list to a given value
-
-- `furthest_value_in_dict`  
-  Function returning the closest number of a dicts values to a given value
-
-- `closest_value_in_dict`  
-  Function returning the closest number of a dicts values to a given value
-
-- `find_dublicates`  
-  Function returning a list of Dubs objects which have the properties: *value*, *number_of_dublicates* and *indices*
-
-- `remove_dublicates`  
-  Function returning a copy of the given list in which only the first occurrence of every value remains
-
-- `get_percentage_as_fitted_string`  
-  Function returning the calculated percentage from the inout count and total fittet to the string lenght of 100.00 %  
-  args:
-  - count: current counting value
-  - total: total value 
-  - round_to: rounding digits, default: 2
-  - with_percentage_symbol: boolean, adds ' %' if True
-
-- `progress_printer`  
-  Call this funciton in a loop with index+1 as count to monitor your progress.  
-  Will automatically switch to a new line when 100 % is reached.
-  Remember to call print once if you break since the cursor will not move to the next line till 100 % are reached.
-
-- `main_and_sub_progress_printer`  
-  Basically the progress_printer with one susbprocess. 
-
-- `upper_case_first_letter_of_word`  
-  Function returning a string in which the word begins with an upper case letter.
-
-- `upper_case_first_letter_of_words`  
-  Function returning a string in which every word begins with an upper case letter.
-
-- `unpack_list`  
-  Dissolve inner lists and tuples of nested list and tuples.
-
-
-## Links
-[GitHub](https://github.com/ICreedenI/easy_tasks) | [PyPI](https://pypi.org/project/easy-tasks/)
+# easy_taks
+
+To not get annoyed by simple recurring tasks I created this small library.  
+
+## Content
+- Installation
+- Usage  
+
+## Installation
+- `pip install easy-tasks`
+- You will need to install to_precision from github to use all the percentage stuff. For this visit https://github.com/BebeSparkelSparkel/to-precision, go to the latest release, which might be https://github.com/BebeSparkelSparkel/to-precision/releases/tag/0.0.1, and download the .tar.gz. With `pip install <path to .tar.gz>` you can finish your installation.
+
+## Usage
+- `furthest_value_in_list`  
+  Function returning the closest number of a list to a given value
+
+- `closest_value_in_list`  
+  Function returning the closest number of a list to a given value
+
+- `furthest_value_in_dict`  
+  Function returning the closest number of a dicts values to a given value
+
+- `closest_value_in_dict`  
+  Function returning the closest number of a dicts values to a given value
+
+- `find_dublicates`  
+  Function returning a list of Dubs objects which have the properties: *value*, *number_of_dublicates* and *indices*
+
+- `remove_dublicates`  
+  Function returning a copy of the given list in which only the first occurrence of every value remains
+
+- `get_percentage_as_fitted_string`  
+  Function returning the calculated percentage from the inout count and total fittet to the string lenght of 100.00 %  
+  args:
+  - count: current counting value
+  - total: total value 
+  - round_to: rounding digits, default: 2
+  - with_percentage_symbol: boolean, adds ' %' if True
+
+- `progress_printer`  
+  Call this funciton in a loop with index+1 as count to monitor your progress.  
+  Will automatically switch to a new line when 100 % is reached.
+  Remember to call print once if you break since the cursor will not move to the next line till 100 % are reached.
+
+- `main_and_sub_progress_printer`  
+  Basically the progress_printer with one susbprocess. 
+
+- `upper_case_first_letter_of_word`  
+  Function returning a string in which the word begins with an upper case letter.
+
+- `upper_case_first_letter_of_words`  
+  Function returning a string in which every word begins with an upper case letter.
+
+- `unpack_list`  
+  Dissolve inner lists and tuples of nested list and tuples.
+
+
+## Links
+[GitHub](https://github.com/ICreedenI/easy_tasks) | [PyPI](https://pypi.org/project/easy-tasks/)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `easy_tasks-0.0.7/README.md` & `easy_tasks-0.0.8/easy_tasks.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,58 +1,77 @@
-# easy_taks
-
-To not get annoyed by simple recurring tasks I created this small library.  
-
-## Content
-- Installation
-- Usage  
-
-## Installation
-- `pip install easy-tasks`
-
-## Usage
-- `furthest_value_in_list`  
-  Function returning the closest number of a list to a given value
-
-- `closest_value_in_list`  
-  Function returning the closest number of a list to a given value
-
-- `furthest_value_in_dict`  
-  Function returning the closest number of a dicts values to a given value
-
-- `closest_value_in_dict`  
-  Function returning the closest number of a dicts values to a given value
-
-- `find_dublicates`  
-  Function returning a list of Dubs objects which have the properties: *value*, *number_of_dublicates* and *indices*
-
-- `remove_dublicates`  
-  Function returning a copy of the given list in which only the first occurrence of every value remains
-
-- `get_percentage_as_fitted_string`  
-  Function returning the calculated percentage from the inout count and total fittet to the string lenght of 100.00 %  
-  args:
-  - count: current counting value
-  - total: total value 
-  - round_to: rounding digits, default: 2
-  - with_percentage_symbol: boolean, adds ' %' if True
-
-- `progress_printer`  
-  Call this funciton in a loop with index+1 as count to monitor your progress.  
-  Will automatically switch to a new line when 100 % is reached.
-  Remember to call print once if you break since the cursor will not move to the next line till 100 % are reached.
-
-- `main_and_sub_progress_printer`  
-  Basically the progress_printer with one susbprocess. 
-
-- `upper_case_first_letter_of_word`  
-  Function returning a string in which the word begins with an upper case letter.
-
-- `upper_case_first_letter_of_words`  
-  Function returning a string in which every word begins with an upper case letter.
-
-- `unpack_list`  
-  Dissolve inner lists and tuples of nested list and tuples.
-
-
-## Links
-[GitHub](https://github.com/ICreedenI/easy_tasks) | [PyPI](https://pypi.org/project/easy-tasks/)
+Metadata-Version: 2.1
+Name: easy-tasks
+Version: 0.0.8
+Summary: Normal python class tasks like sorting, closet/furthest value, dublicates, ...
+Author: André Herber
+Author-email: andre.herber.programming@gmail.com
+Keywords: python
+Classifier: Development Status :: 1 - Planning
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+
+# easy_taks
+
+To not get annoyed by simple recurring tasks I created this small library.  
+
+## Content
+- Installation
+- Usage  
+
+## Installation
+- `pip install easy-tasks`
+- You will need to install to_precision from github to use all the percentage stuff. For this visit https://github.com/BebeSparkelSparkel/to-precision, go to the latest release, which might be https://github.com/BebeSparkelSparkel/to-precision/releases/tag/0.0.1, and download the .tar.gz. With `pip install <path to .tar.gz>` you can finish your installation.
+
+## Usage
+- `furthest_value_in_list`  
+  Function returning the closest number of a list to a given value
+
+- `closest_value_in_list`  
+  Function returning the closest number of a list to a given value
+
+- `furthest_value_in_dict`  
+  Function returning the closest number of a dicts values to a given value
+
+- `closest_value_in_dict`  
+  Function returning the closest number of a dicts values to a given value
+
+- `find_dublicates`  
+  Function returning a list of Dubs objects which have the properties: *value*, *number_of_dublicates* and *indices*
+
+- `remove_dublicates`  
+  Function returning a copy of the given list in which only the first occurrence of every value remains
+
+- `get_percentage_as_fitted_string`  
+  Function returning the calculated percentage from the inout count and total fittet to the string lenght of 100.00 %  
+  args:
+  - count: current counting value
+  - total: total value 
+  - round_to: rounding digits, default: 2
+  - with_percentage_symbol: boolean, adds ' %' if True
+
+- `progress_printer`  
+  Call this funciton in a loop with index+1 as count to monitor your progress.  
+  Will automatically switch to a new line when 100 % is reached.
+  Remember to call print once if you break since the cursor will not move to the next line till 100 % are reached.
+
+- `main_and_sub_progress_printer`  
+  Basically the progress_printer with one susbprocess. 
+
+- `upper_case_first_letter_of_word`  
+  Function returning a string in which the word begins with an upper case letter.
+
+- `upper_case_first_letter_of_words`  
+  Function returning a string in which every word begins with an upper case letter.
+
+- `unpack_list`  
+  Dissolve inner lists and tuples of nested list and tuples.
+
+
+## Links
+[GitHub](https://github.com/ICreedenI/easy_tasks) | [PyPI](https://pypi.org/project/easy-tasks/)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `easy_tasks-0.0.7/easy_tasks/__init__.py` & `easy_tasks-0.0.8/easy_tasks/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,12 +12,14 @@
 )
 from .sorter import sorted_dict
 from .string_transformation import (
     upper_case_first_letter_of_word,
     upper_case_first_letter_of_words,
 )
 from .unpack import unpack_list
+from .list_printer import pretty_print_list, pretty_print_nested_list
 
+from .help_with_pickle import pickle_pack, pickle_unpack
+from .help_with_json import dump_as_json, get_from_json
 
-from . import _version
 
-__version__ = _version.get_versions()["version"]
+__version__ = "0.0.8"
```

### Comparing `easy_tasks-0.0.7/easy_tasks/closest_furthest_value.py` & `easy_tasks-0.0.8/easy_tasks/closest_furthest_value.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/easy_tasks/dublicates.py` & `easy_tasks-0.0.8/easy_tasks/dublicates.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/easy_tasks/help_with_json.py` & `easy_tasks-0.0.8/easy_tasks/help_with_json.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/easy_tasks/help_with_pickle.py` & `easy_tasks-0.0.8/easy_tasks/help_with_pickle.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/easy_tasks/percentage.py` & `easy_tasks-0.0.8/easy_tasks/percentage.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/easy_tasks/string_transformation.py` & `easy_tasks-0.0.8/easy_tasks/string_transformation.py`

 * *Files identical despite different names*

### Comparing `easy_tasks-0.0.7/easy_tasks.egg-info/PKG-INFO` & `easy_tasks-0.0.8/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: easy-tasks
-Version: 0.0.7
+Name: easy_tasks
+Version: 0.0.8
 Summary: Normal python class tasks like sorting, closet/furthest value, dublicates, ...
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -22,14 +22,15 @@
 
 ## Content
 - Installation
 - Usage  
 
 ## Installation
 - `pip install easy-tasks`
+- You will need to install to_precision from github to use all the percentage stuff. For this visit https://github.com/BebeSparkelSparkel/to-precision, go to the latest release, which might be https://github.com/BebeSparkelSparkel/to-precision/releases/tag/0.0.1, and download the .tar.gz. With `pip install <path to .tar.gz>` you can finish your installation.
 
 ## Usage
 - `furthest_value_in_list`  
   Function returning the closest number of a list to a given value
 
 - `closest_value_in_list`  
   Function returning the closest number of a list to a given value
```

### Comparing `easy_tasks-0.0.7/setup.py` & `easy_tasks-0.0.8/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 # twine upload dist/*
 # twine upload --skip-existing dist/*
 # twine upload --verbose --skip-existing dist/*
 # twine upload --verbose dist/*
 
 from setuptools import setup, find_packages
-import versioneer
 import codecs
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
@@ -27,16 +26,15 @@
 DESCRIPTION = (
     "Normal python class tasks like sorting, closet/furthest value, dublicates, ..."
 )
 
 # Setting up
 setup(
     name="easy_tasks",
-    version=versioneer.get_version(),
-    cmdclass=versioneer.get_cmdclass(),
+    version="0.0.8",
     author="André Herber",
     author_email="andre.herber.programming@gmail.com",
     # url="https://github.com/ICreedenI/xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
```

