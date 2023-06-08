# Comparing `tmp/colorful_terminal-0.0.4.tar.gz` & `tmp/colorful_terminal-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "colorful_terminal-0.0.4.tar", last modified: Sun Jun  4 17:40:48 2023, max compression
+gzip compressed data, was "colorful_terminal-0.0.5.tar", last modified: Thu Jun  8 15:37:19 2023, max compression
```

## Comparing `colorful_terminal-0.0.4.tar` & `colorful_terminal-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-04 17:40:48.503451 colorful_terminal-0.0.4/
--rw-rw-rw-   0        0        0     1091 2023-01-07 18:23:21.000000 colorful_terminal-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     9720 2023-06-04 17:40:48.503451 colorful_terminal-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     8702 2023-01-07 18:23:21.000000 colorful_terminal-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-06-04 17:40:48.495771 colorful_terminal-0.0.4/colorful_terminal/
--rw-rw-rw-   0        0        0      260 2023-06-04 17:39:34.000000 colorful_terminal-0.0.4/colorful_terminal/__init__.py
--rw-rw-rw-   0        0        0    31061 2023-06-04 17:37:21.000000 colorful_terminal-0.0.4/colorful_terminal/definitions.py
-drwxrwxrwx   0        0        0        0 2023-06-04 17:40:48.500908 colorful_terminal-0.0.4/colorful_terminal.egg-info/
--rw-rw-rw-   0        0        0     9720 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-06-04 17:40:48.000000 colorful_terminal-0.0.4/colorful_terminal.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-04 17:40:48.504454 colorful_terminal-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1976 2023-06-04 17:39:43.000000 colorful_terminal-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:37:19.399788 colorful_terminal-0.0.5/
+-rw-rw-rw-   0        0        0     1091 2023-01-07 18:23:21.000000 colorful_terminal-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     9720 2023-06-08 15:37:19.398785 colorful_terminal-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     8702 2023-01-07 18:23:21.000000 colorful_terminal-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 15:37:19.392524 colorful_terminal-0.0.5/colorful_terminal/
+-rw-rw-rw-   0        0        0      260 2023-06-08 15:35:51.000000 colorful_terminal-0.0.5/colorful_terminal/__init__.py
+-rw-rw-rw-   0        0        0    31061 2023-06-04 17:37:21.000000 colorful_terminal-0.0.5/colorful_terminal/definitions.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:37:19.396765 colorful_terminal-0.0.5/colorful_terminal.egg-info/
+-rw-rw-rw-   0        0        0     9720 2023-06-08 15:37:19.000000 colorful_terminal-0.0.5/colorful_terminal.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-06-08 15:37:19.000000 colorful_terminal-0.0.5/colorful_terminal.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:37:19.000000 colorful_terminal-0.0.5/colorful_terminal.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 15:37:19.000000 colorful_terminal-0.0.5/colorful_terminal.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 15:37:19.399788 colorful_terminal-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1976 2023-06-08 15:35:47.000000 colorful_terminal-0.0.5/setup.py
```

### Comparing `colorful_terminal-0.0.4/LICENSE` & `colorful_terminal-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.0.4/PKG-INFO` & `colorful_terminal-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful_terminal
-Version: 0.0.4
+Version: 0.0.5
 Summary: Print with color, style your output and take full control of your terminal.
 Home-page: https://github.com/ICreedenI/colorful_terminal
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python,print,color,colour,colored,coloured,rainbow,terminal,console,colorama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `colorful_terminal-0.0.4/README.md` & `colorful_terminal-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.0.4/colorful_terminal/definitions.py` & `colorful_terminal-0.0.5/colorful_terminal/definitions.py`

 * *Files identical despite different names*

### Comparing `colorful_terminal-0.0.4/colorful_terminal.egg-info/PKG-INFO` & `colorful_terminal-0.0.5/colorful_terminal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: colorful-terminal
-Version: 0.0.4
+Version: 0.0.5
 Summary: Print with color, style your output and take full control of your terminal.
 Home-page: https://github.com/ICreedenI/colorful_terminal
 Author: André Herber
 Author-email: andre.herber.programming@gmail.com
 Keywords: python,print,color,colour,colored,coloured,rainbow,terminal,console,colorama
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
```

### Comparing `colorful_terminal-0.0.4/setup.py` & `colorful_terminal-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = "0.0.4"
+VERSION = "0.0.5"
 DESCRIPTION = (
     "Print with color, style your output and take full control of your terminal."
 )
 
 # Setting up
 setup(
     name="colorful_terminal",
```

