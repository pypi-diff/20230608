# Comparing `tmp/flachtex-0.3.8.tar.gz` & `tmp/flachtex-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flachtex-0.3.8.tar", last modified: Thu Oct  6 09:38:03 2022, max compression
+gzip compressed data, was "flachtex-0.3.9.tar", last modified: Thu Oct 27 16:47:43 2022, max compression
```

## Comparing `flachtex-0.3.8.tar` & `flachtex-0.3.9.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:38:03.860965 flachtex-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-06 09:37:56.000000 flachtex-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-10-06 09:38:03.860965 flachtex-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7828 2022-10-06 09:37:56.000000 flachtex-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:38:03.860965 flachtex-0.3.8/flachtex/
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/command_finder.py
--rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/command_substitution.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/comments.py
--rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/cycle_prevention.py
--rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/filefinder.py
--rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/preprocessor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:38:03.860965 flachtex-0.3.8/flachtex/rules/
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/rules/import_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/rules/skip_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/rules/substitution_rules.py
--rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/traceable_string.py
--rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-10-06 09:37:56.000000 flachtex-0.3.8/flachtex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-06 09:38:03.860965 flachtex-0.3.8/flachtex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8311 2022-10-06 09:38:03.000000 flachtex-0.3.8/flachtex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      591 2022-10-06 09:38:03.000000 flachtex-0.3.8/flachtex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 09:38:03.000000 flachtex-0.3.8/flachtex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-06 09:38:03.000000 flachtex-0.3.8/flachtex.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-06 09:38:03.000000 flachtex-0.3.8/flachtex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-06 09:38:03.000000 flachtex-0.3.8/flachtex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-06 09:38:03.860965 flachtex-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-06 09:37:56.000000 flachtex-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:47:43.848813 flachtex-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-10-27 16:47:36.000000 flachtex-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     8406 2022-10-27 16:47:43.848813 flachtex-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7923 2022-10-27 16:47:36.000000 flachtex-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:47:43.848813 flachtex-0.3.9/flachtex/
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2452 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9624 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/command_finder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4958 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/command_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/comments.py
+-rw-r--r--   0 runner    (1001) docker     (121)      611 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/cycle_prevention.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3512 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/filefinder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3185 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/preprocessor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:47:43.848813 flachtex-0.3.9/flachtex/rules/
+-rw-r--r--   0 runner    (1001) docker     (121)      427 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/rules/import_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2782 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/rules/skip_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4287 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/rules/substitution_rules.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5459 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/traceable_string.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1453 2022-10-27 16:47:36.000000 flachtex-0.3.9/flachtex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-27 16:47:43.848813 flachtex-0.3.9/flachtex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8406 2022-10-27 16:47:43.000000 flachtex-0.3.9/flachtex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      606 2022-10-27 16:47:43.000000 flachtex-0.3.9/flachtex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 16:47:43.000000 flachtex-0.3.9/flachtex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-10-27 16:47:43.000000 flachtex-0.3.9/flachtex.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-27 16:47:43.000000 flachtex-0.3.9/flachtex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-10-27 16:47:43.000000 flachtex-0.3.9/flachtex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       81 2022-10-27 16:47:36.000000 flachtex-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-27 16:47:43.848813 flachtex-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      858 2022-10-27 16:47:36.000000 flachtex-0.3.9/setup.py
```

### Comparing `flachtex-0.3.8/LICENSE` & `flachtex-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/PKG-INFO` & `flachtex-0.3.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flachtex
-Version: 0.3.8
+Version: 0.3.9
 Summary: A traceable LaTeX flattener.
 Home-page: https://github.com/d-krupke/flachtex
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: LaTeX flatten
 Platform: UNKNOWN
@@ -248,14 +248,15 @@
 The primary reason I added this functionality to this tool (and not some higher level
 tool)
 is that I also saw that some people define their own \input/\include commands, which
 could not be imported easily without this feature.
 
 ## Changelog
 
+* **0.3.9**: PEP compliance which may have created problems in environments without setuptools
 * **0.3.8**: Substituting newcommands is no longer enabled by default.
 * **0.3.7**: Versions got slightly mixed up. Should be fixed now.
 * **0.3.6** bugfix: Using  findall instead of finditer.
 * **0.3.4** Dealing with `\xspace` in command substitution.
 * **0.3.3**
   * `FileFinder` now has a default and allows to set a new root.
   * Command substitution for commands without parameters made more accurate.
```

### Comparing `flachtex-0.3.8/README.md` & `flachtex-0.3.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -231,14 +231,15 @@
 The primary reason I added this functionality to this tool (and not some higher level
 tool)
 is that I also saw that some people define their own \input/\include commands, which
 could not be imported easily without this feature.
 
 ## Changelog
 
+* **0.3.9**: PEP compliance which may have created problems in environments without setuptools
 * **0.3.8**: Substituting newcommands is no longer enabled by default.
 * **0.3.7**: Versions got slightly mixed up. Should be fixed now.
 * **0.3.6** bugfix: Using  findall instead of finditer.
 * **0.3.4** Dealing with `\xspace` in command substitution.
 * **0.3.3**
   * `FileFinder` now has a default and allows to set a new root.
   * Command substitution for commands without parameters made more accurate.
```

### Comparing `flachtex-0.3.8/flachtex/__main__.py` & `flachtex-0.3.9/flachtex/__main__.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/command_finder.py` & `flachtex-0.3.9/flachtex/command_finder.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/command_substitution.py` & `flachtex-0.3.9/flachtex/command_substitution.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/comments.py` & `flachtex-0.3.9/flachtex/comments.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/cycle_prevention.py` & `flachtex-0.3.9/flachtex/cycle_prevention.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/filefinder.py` & `flachtex-0.3.9/flachtex/filefinder.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/preprocessor.py` & `flachtex-0.3.9/flachtex/preprocessor.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/rules/import_rules.py` & `flachtex-0.3.9/flachtex/rules/import_rules.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/rules/skip_rules.py` & `flachtex-0.3.9/flachtex/rules/skip_rules.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/rules/substitution_rules.py` & `flachtex-0.3.9/flachtex/rules/substitution_rules.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/traceable_string.py` & `flachtex-0.3.9/flachtex/traceable_string.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex/utils.py` & `flachtex-0.3.9/flachtex/utils.py`

 * *Files identical despite different names*

### Comparing `flachtex-0.3.8/flachtex.egg-info/PKG-INFO` & `flachtex-0.3.9/flachtex.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flachtex
-Version: 0.3.8
+Version: 0.3.9
 Summary: A traceable LaTeX flattener.
 Home-page: https://github.com/d-krupke/flachtex
 Author: Dominik Krupke
 Author-email: krupke@ibr.cs.tu-bs.de
 License: MIT
 Keywords: LaTeX flatten
 Platform: UNKNOWN
@@ -248,14 +248,15 @@
 The primary reason I added this functionality to this tool (and not some higher level
 tool)
 is that I also saw that some people define their own \input/\include commands, which
 could not be imported easily without this feature.
 
 ## Changelog
 
+* **0.3.9**: PEP compliance which may have created problems in environments without setuptools
 * **0.3.8**: Substituting newcommands is no longer enabled by default.
 * **0.3.7**: Versions got slightly mixed up. Should be fixed now.
 * **0.3.6** bugfix: Using  findall instead of finditer.
 * **0.3.4** Dealing with `\xspace` in command substitution.
 * **0.3.3**
   * `FileFinder` now has a default and allows to set a new root.
   * Command substitution for commands without parameters made more accurate.
```

### Comparing `flachtex-0.3.8/flachtex.egg-info/SOURCES.txt` & `flachtex-0.3.9/flachtex.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 LICENSE
 README.md
+pyproject.toml
 setup.py
 flachtex/__init__.py
 flachtex/__main__.py
 flachtex/command_finder.py
 flachtex/command_substitution.py
 flachtex/comments.py
 flachtex/cycle_prevention.py
```

### Comparing `flachtex-0.3.8/setup.py` & `flachtex-0.3.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 def readme():
     with open("README.md") as f:
         return f.read()
 
 
 setup(
     name="flachtex",
-    version="0.3.8",
+    version="0.3.9",
     description="A traceable LaTeX flattener.",
     long_description=readme(),
     long_description_content_type="text/markdown",
     classifiers=[
         "Development Status :: 4 - Beta",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python :: 3",
```

