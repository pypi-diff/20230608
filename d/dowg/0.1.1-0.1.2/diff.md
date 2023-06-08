# Comparing `tmp/dowg-0.1.1.tar.gz` & `tmp/dowg-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowg-0.1.1.tar", last modified: Thu Jun  8 16:10:12 2023, max compression
+gzip compressed data, was "dowg-0.1.2.tar", last modified: Thu Jun  8 16:19:58 2023, max compression
```

## Comparing `dowg-0.1.1.tar` & `dowg-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.553344 dowg-0.1.1/
--rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.1.1/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-08 16:10:12.553344 dowg-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.1.1/README.md
--rw-rw-rw-   0        0        0      552 2023-06-08 16:10:00.000000 dowg-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 16:10:12.553344 dowg-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.536346 dowg-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.543344 dowg-0.1.1/src/dowg/
--rw-rw-rw-   0        0        0     2037 2023-06-08 16:09:08.000000 dowg-0.1.1/src/dowg/CoordinateDoWG.py
--rw-rw-rw-   0        0        0     1914 2023-06-08 16:09:01.000000 dowg-0.1.1/src/dowg/ScalarDoWG.py
--rw-rw-rw-   0        0        0        0 2023-06-08 15:18:11.000000 dowg-0.1.1/src/dowg/__init__.py
--rw-rw-rw-   0        0        0      844 2023-06-08 15:06:06.000000 dowg-0.1.1/src/dowg/clip.py
-drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.552345 dowg-0.1.1/src/dowg.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.261800 dowg-0.1.2/
+-rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-08 16:19:58.260800 dowg-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.1.2/README.md
+-rw-rw-rw-   0        0        0      552 2023-06-08 16:19:35.000000 dowg-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:19:58.261800 dowg-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.243799 dowg-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.250798 dowg-0.1.2/src/dowg/
+-rw-rw-rw-   0        0        0     2037 2023-06-08 16:09:08.000000 dowg-0.1.2/src/dowg/CoordinateDoWG.py
+-rw-rw-rw-   0        0        0     1914 2023-06-08 16:09:01.000000 dowg-0.1.2/src/dowg/ScalarDoWG.py
+-rw-rw-rw-   0        0        0      172 2023-06-08 16:18:17.000000 dowg-0.1.2/src/dowg/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-06-08 15:06:06.000000 dowg-0.1.2/src/dowg/clip.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:19:58.259800 dowg-0.1.2/src/dowg.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-08 16:19:58.000000 dowg-0.1.2/src/dowg.egg-info/top_level.txt
```

### Comparing `dowg-0.1.1/LICENSE` & `dowg-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dowg-0.1.1/PKG-INFO` & `dowg-0.1.2/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.1.1
+Version: 0.1.2
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dowg-0.1.1/pyproject.toml` & `dowg-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dowg"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Patrick Shanahan", email="patrick.e.shanahan@gmail.com" },
 ]
 description = "DoWG parameter-free adaptive optimizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dowg-0.1.1/src/dowg/CoordinateDoWG.py` & `dowg-0.1.2/src/dowg/CoordinateDoWG.py`

 * *Files identical despite different names*

### Comparing `dowg-0.1.1/src/dowg/ScalarDoWG.py` & `dowg-0.1.2/src/dowg/ScalarDoWG.py`

 * *Files identical despite different names*

### Comparing `dowg-0.1.1/src/dowg/clip.py` & `dowg-0.1.2/src/dowg/clip.py`

 * *Files identical despite different names*

### Comparing `dowg-0.1.1/src/dowg.egg-info/PKG-INFO` & `dowg-0.1.2/src/dowg.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.1.1
+Version: 0.1.2
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

