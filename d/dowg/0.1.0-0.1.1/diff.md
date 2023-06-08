# Comparing `tmp/dowg-0.1.0.tar.gz` & `tmp/dowg-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dowg-0.1.0.tar", last modified: Thu Jun  8 15:23:39 2023, max compression
+gzip compressed data, was "dowg-0.1.1.tar", last modified: Thu Jun  8 16:10:12 2023, max compression
```

## Comparing `dowg-0.1.0.tar` & `dowg-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 15:23:39.014460 dowg-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      805 2023-06-08 15:23:39.014460 dowg-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.1.0/README.md
--rw-rw-rw-   0        0        0      552 2023-06-08 15:23:26.000000 dowg-0.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 15:23:39.014460 dowg-0.1.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 15:23:38.995460 dowg-0.1.0/src/
-drwxrwxrwx   0        0        0        0 2023-06-08 15:23:39.002462 dowg-0.1.0/src/dowg/
--rw-rw-rw-   0        0        0     2036 2023-06-08 15:14:14.000000 dowg-0.1.0/src/dowg/CoordinateDoWG.py
--rw-rw-rw-   0        0        0     1913 2023-06-08 15:14:11.000000 dowg-0.1.0/src/dowg/ScalarDoWG.py
--rw-rw-rw-   0        0        0        0 2023-06-08 15:18:11.000000 dowg-0.1.0/src/dowg/__init__.py
--rw-rw-rw-   0        0        0      844 2023-06-08 15:06:06.000000 dowg-0.1.0/src/dowg/clip.py
-drwxrwxrwx   0        0        0        0 2023-06-08 15:23:39.013466 dowg-0.1.0/src/dowg.egg-info/
--rw-rw-rw-   0        0        0      805 2023-06-08 15:23:38.000000 dowg-0.1.0/src/dowg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      248 2023-06-08 15:23:38.000000 dowg-0.1.0/src/dowg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 15:23:38.000000 dowg-0.1.0/src/dowg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2023-06-08 15:23:38.000000 dowg-0.1.0/src/dowg.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.553344 dowg-0.1.1/
+-rw-rw-rw-   0        0        0     1090 2023-06-08 13:29:34.000000 dowg-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      805 2023-06-08 16:10:12.553344 dowg-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0      341 2023-06-08 15:21:40.000000 dowg-0.1.1/README.md
+-rw-rw-rw-   0        0        0      552 2023-06-08 16:10:00.000000 dowg-0.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 16:10:12.553344 dowg-0.1.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.536346 dowg-0.1.1/src/
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.543344 dowg-0.1.1/src/dowg/
+-rw-rw-rw-   0        0        0     2037 2023-06-08 16:09:08.000000 dowg-0.1.1/src/dowg/CoordinateDoWG.py
+-rw-rw-rw-   0        0        0     1914 2023-06-08 16:09:01.000000 dowg-0.1.1/src/dowg/ScalarDoWG.py
+-rw-rw-rw-   0        0        0        0 2023-06-08 15:18:11.000000 dowg-0.1.1/src/dowg/__init__.py
+-rw-rw-rw-   0        0        0      844 2023-06-08 15:06:06.000000 dowg-0.1.1/src/dowg/clip.py
+drwxrwxrwx   0        0        0        0 2023-06-08 16:10:12.552345 dowg-0.1.1/src/dowg.egg-info/
+-rw-rw-rw-   0        0        0      805 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      248 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2023-06-08 16:10:12.000000 dowg-0.1.1/src/dowg.egg-info/top_level.txt
```

### Comparing `dowg-0.1.0/LICENSE` & `dowg-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dowg-0.1.0/PKG-INFO` & `dowg-0.1.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.1.0
+Version: 0.1.1
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `dowg-0.1.0/pyproject.toml` & `dowg-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dowg"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Patrick Shanahan", email="patrick.e.shanahan@gmail.com" },
 ]
 description = "DoWG parameter-free adaptive optimizer"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `dowg-0.1.0/src/dowg/CoordinateDoWG.py` & `dowg-0.1.1/src/dowg/CoordinateDoWG.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from clip import clip_gradient
+from .clip import clip_gradient
 
 
 class CoordinateDoWG(torch.optim.Optimizer):
     """Implements CDoWG-- a coordinate-wise version of DoWG.
 
         Args:
             params (iterable): iterable of parameters to optimize or dicts defining
```

### Comparing `dowg-0.1.0/src/dowg/ScalarDoWG.py` & `dowg-0.1.1/src/dowg/ScalarDoWG.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import torch
 
-from clip import clip_gradient
+from .clip import clip_gradient
 
 
 class ScalarDoWG(torch.optim.Optimizer):
     def __init__(self, params, epsilon=1e-4, clip=0.5, *args, **kwargs):
         defaults = dict(r_epsilon=epsilon, lr=1, clip=clip)
         self.epsilon = epsilon
         super(ScalarDoWG, self).__init__(params, defaults)
```

### Comparing `dowg-0.1.0/src/dowg/clip.py` & `dowg-0.1.1/src/dowg/clip.py`

 * *Files identical despite different names*

### Comparing `dowg-0.1.0/src/dowg.egg-info/PKG-INFO` & `dowg-0.1.1/src/dowg.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dowg
-Version: 0.1.0
+Version: 0.1.1
 Summary: DoWG parameter-free adaptive optimizer
 Author-email: Patrick Shanahan <patrick.e.shanahan@gmail.com>
 Project-URL: Homepage, https://github.com/AMorporkian/dowg
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

