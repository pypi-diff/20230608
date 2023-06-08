# Comparing `tmp/mfconv-0.2.1.tar.gz` & `tmp/mfconv-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mfconv-0.2.1.tar", last modified: Wed Jun  7 23:46:18 2023, max compression
+gzip compressed data, was "mfconv-0.2.2.tar", last modified: Thu Jun  8 15:12:09 2023, max compression
```

## Comparing `mfconv-0.2.1.tar` & `mfconv-0.2.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 23:46:18.057639 mfconv-0.2.1/
--rw-rw-rw-   0        0        0     1080 2023-04-21 17:04:38.000000 mfconv-0.2.1/LICENSE.txt
--rw-rw-rw-   0        0        0     1092 2023-06-07 23:46:18.057639 mfconv-0.2.1/PKG-INFO
--rw-rw-rw-   0        0        0      354 2023-04-21 17:04:38.000000 mfconv-0.2.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 23:46:18.045710 mfconv-0.2.1/mfconv/
--rw-rw-rw-   0        0        0      181 2023-06-07 23:44:58.000000 mfconv-0.2.1/mfconv/__init__.py
--rw-rw-rw-   0        0        0       55 2023-06-07 23:14:01.000000 mfconv-0.2.1/mfconv/__main__.py
--rw-rw-rw-   0        0        0     7243 2023-06-07 21:33:38.000000 mfconv-0.2.1/mfconv/plotter.py
-drwxrwxrwx   0        0        0        0 2023-06-07 23:46:18.057639 mfconv-0.2.1/mfconv.egg-info/
--rw-rw-rw-   0        0        0     1092 2023-06-07 23:46:17.000000 mfconv-0.2.1/mfconv.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2023-06-07 23:46:17.000000 mfconv-0.2.1/mfconv.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 23:46:17.000000 mfconv-0.2.1/mfconv.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-06-07 23:46:17.000000 mfconv-0.2.1/mfconv.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        0 2023-04-21 17:04:38.000000 mfconv-0.2.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 23:46:18.057639 mfconv-0.2.1/setup.cfg
--rw-rw-rw-   0        0        0     1554 2023-06-07 23:22:43.000000 mfconv-0.2.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:12:09.617985 mfconv-0.2.2/
+-rw-rw-rw-   0        0        0     1080 2023-04-21 17:04:38.000000 mfconv-0.2.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     1115 2023-06-08 15:12:09.616985 mfconv-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0      354 2023-04-21 17:04:38.000000 mfconv-0.2.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 15:12:09.611985 mfconv-0.2.2/mfconv/
+-rw-rw-rw-   0        0        0      283 2023-06-08 15:11:59.000000 mfconv-0.2.2/mfconv/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-06-07 23:14:01.000000 mfconv-0.2.2/mfconv/__main__.py
+-rw-rw-rw-   0        0        0     7243 2023-06-07 21:33:38.000000 mfconv-0.2.2/mfconv/plotter.py
+drwxrwxrwx   0        0        0        0 2023-06-08 15:12:09.615985 mfconv-0.2.2/mfconv.egg-info/
+-rw-rw-rw-   0        0        0     1115 2023-06-08 15:12:09.000000 mfconv-0.2.2/mfconv.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2023-06-08 15:12:09.000000 mfconv-0.2.2/mfconv.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 15:12:09.000000 mfconv-0.2.2/mfconv.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 15:12:09.000000 mfconv-0.2.2/mfconv.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        0 2023-04-21 17:04:38.000000 mfconv-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 15:12:09.617985 mfconv-0.2.2/setup.cfg
+-rw-rw-rw-   0        0        0     1554 2023-06-07 23:22:43.000000 mfconv-0.2.2/setup.py
```

### Comparing `mfconv-0.2.1/LICENSE.txt` & `mfconv-0.2.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mfconv-0.2.1/PKG-INFO` & `mfconv-0.2.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mfconv
-Version: 0.2.1
+Version: 0.2.2
 Summary: a python package to plot modflow convergence while you run a model
 Home-page: https://github.com/gmezacuadra/mfconv
 Author: Gustavo Meza-Cuadra
 Author-email: gmeza-cuadra@flosolutions.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,7 +35,9 @@
 
 TODO - fill this in later
 
 Contribute
 ----------
 
 If you'd like to contribute to mfconv, check out https://github.com/gmezacuadra/mfconv
+
+
```

### Comparing `mfconv-0.2.1/mfconv/plotter.py` & `mfconv-0.2.2/mfconv/plotter.py`

 * *Files identical despite different names*

### Comparing `mfconv-0.2.1/mfconv.egg-info/PKG-INFO` & `mfconv-0.2.2/mfconv.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: mfconv
-Version: 0.2.1
+Version: 0.2.2
 Summary: a python package to plot modflow convergence while you run a model
 Home-page: https://github.com/gmezacuadra/mfconv
 Author: Gustavo Meza-Cuadra
 Author-email: gmeza-cuadra@flosolutions.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -34,7 +35,9 @@
 
 TODO - fill this in later
 
 Contribute
 ----------
 
 If you'd like to contribute to mfconv, check out https://github.com/gmezacuadra/mfconv
+
+
```

### Comparing `mfconv-0.2.1/setup.py` & `mfconv-0.2.2/setup.py`

 * *Files identical despite different names*

