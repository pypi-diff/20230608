# Comparing `tmp/yplib-0.0.1.tar.gz` & `tmp/yplib-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\yplib-0.0.1.tar", last modified: Thu Jun  8 01:52:02 2023, max compression
+gzip compressed data, was "dist\yplib-0.0.2.tar", last modified: Thu Jun  8 02:36:38 2023, max compression
```

## Comparing `yplib-0.0.1.tar` & `yplib-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 01:52:02.761144 yplib-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      567 2023-06-08 01:52:02.761144 yplib-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-08 01:52:02.761144 yplib-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      561 2023-06-08 01:40:04.000000 yplib-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:52:02.758382 yplib-0.0.1/yplib/
--rw-rw-rw-   0        0        0       14 2023-06-08 01:39:55.000000 yplib-0.0.1/yplib/__init__.py
--rw-rw-rw-   0        0        0       43 2023-06-08 00:54:48.000000 yplib-0.0.1/yplib/example.py
-drwxrwxrwx   0        0        0        0 2023-06-08 01:52:02.760407 yplib-0.0.1/yplib.egg-info/
--rw-rw-rw-   0        0        0      567 2023-06-08 01:52:02.000000 yplib-0.0.1/yplib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2023-06-08 01:52:02.000000 yplib-0.0.1/yplib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 01:52:02.000000 yplib-0.0.1/yplib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 01:52:02.000000 yplib-0.0.1/yplib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 02:36:38.559502 yplib-0.0.2/
+-rw-rw-rw-   0        0        0     1091 2023-06-08 01:05:18.000000 yplib-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      567 2023-06-08 02:36:38.559502 yplib-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      178 2023-06-08 01:05:32.000000 yplib-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:36:38.559502 yplib-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      561 2023-06-08 02:36:29.000000 yplib-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:36:38.556679 yplib-0.0.2/yplib/
+-rw-rw-rw-   0        0        0      709 2023-06-08 02:34:39.000000 yplib-0.0.2/yplib/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-06-08 00:54:48.000000 yplib-0.0.2/yplib/example.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:36:38.558887 yplib-0.0.2/yplib.egg-info/
+-rw-rw-rw-   0        0        0      567 2023-06-08 02:36:38.000000 yplib-0.0.2/yplib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2023-06-08 02:36:38.000000 yplib-0.0.2/yplib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:36:38.000000 yplib-0.0.2/yplib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 02:36:38.000000 yplib-0.0.2/yplib.egg-info/top_level.txt
```

### Comparing `yplib-0.0.1/LICENSE` & `yplib-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `yplib-0.0.1/PKG-INFO` & `yplib-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.0.1
+Version: 0.0.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yplib-0.0.1/setup.py` & `yplib-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
   long_description = fh.read()
 
 setuptools.setup(
   name="yplib",
-  version="0.0.1",
+  version="0.0.2",
   author="yangpu",
   author_email="wantwaterfish@gmail.com",
   description="util",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/pypa/sampleproject",
   packages=setuptools.find_packages(),
```

### Comparing `yplib-0.0.1/yplib.egg-info/PKG-INFO` & `yplib-0.0.2/yplib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yplib
-Version: 0.0.1
+Version: 0.0.2
 Summary: util
 Home-page: https://github.com/pypa/sampleproject
 Author: yangpu
 Author-email: wantwaterfish@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

