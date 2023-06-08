# Comparing `tmp/iguala-0.5.1.tar.gz` & `tmp/iguala-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iguala-0.5.1.tar", last modified: Tue May 16 19:31:01 2023, max compression
+gzip compressed data, was "iguala-0.5.2.tar", last modified: Thu Jun  8 14:34:44 2023, max compression
```

## Comparing `iguala-0.5.1.tar` & `iguala-0.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:31:01.942409 iguala-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-05-16 19:30:50.000000 iguala-0.5.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-16 19:30:50.000000 iguala-0.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-16 19:30:50.000000 iguala-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-05-16 19:31:01.942409 iguala-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-05-16 19:30:50.000000 iguala-0.5.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:31:01.942409 iguala-0.5.1/iguala/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    19148 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/matchers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-05-16 19:30:50.000000 iguala-0.5.1/iguala/paths.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-16 19:31:01.942409 iguala-0.5.1/iguala.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-16 19:31:01.000000 iguala-0.5.1/iguala.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-16 19:31:01.942409 iguala-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-16 19:30:50.000000 iguala-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:34:44.016916 iguala-0.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-08 14:34:31.000000 iguala-0.5.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-06-08 14:34:31.000000 iguala-0.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-08 14:34:31.000000 iguala-0.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-06-08 14:34:44.012916 iguala-0.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    28431 2023-06-08 14:34:31.000000 iguala-0.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:34:44.012916 iguala-0.5.2/iguala/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-06-08 14:34:31.000000 iguala-0.5.2/iguala/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-06-08 14:34:31.000000 iguala-0.5.2/iguala/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19238 2023-06-08 14:34:31.000000 iguala-0.5.2/iguala/matchers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3678 2023-06-08 14:34:31.000000 iguala-0.5.2/iguala/paths.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:34:44.012916 iguala-0.5.2/iguala.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    29356 2023-06-08 14:34:43.000000 iguala-0.5.2/iguala.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 14:34:43.000000 iguala-0.5.2/iguala.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:34:43.000000 iguala-0.5.2/iguala.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 14:34:43.000000 iguala-0.5.2/iguala.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:34:44.016916 iguala-0.5.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-06-08 14:34:31.000000 iguala-0.5.2/setup.py
```

### Comparing `iguala-0.5.1/CHANGELOG.md` & `iguala-0.5.2/CHANGELOG.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # CHANGELOG
 
+## 0.5.2
+
+### Fixes
+
+* Fix issue in the regex matcher where `None` was actually used as target for the regex.
+
+
 ## 0.5.1
 
 ### Fixes
 
 * Fix issue in the dict matcher, the path were badly interpreted.
```

### Comparing `iguala-0.5.1/LICENSE` & `iguala-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `iguala-0.5.1/PKG-INFO` & `iguala-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguala
-Version: 0.5.1
+Version: 0.5.2
 Summary: Non-linear pattern matching for Python's objects, or rexep-like for objects
 Home-page: https://github.com/aranega/iguala
 Author: Vincent Aranega
 Author-email: vincent.aranega@gmail.com
 License: BSD 3-Clause
 Keywords: pattern matching matcher regexp graph query term rewriting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iguala-0.5.1/README.md` & `iguala-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `iguala-0.5.1/iguala/helpers.py` & `iguala-0.5.2/iguala/helpers.py`

 * *Files identical despite different names*

### Comparing `iguala-0.5.1/iguala/matchers.py` & `iguala-0.5.2/iguala/matchers.py`

 * *Files 0% similar despite different names*

```diff
@@ -322,14 +322,17 @@
         self.label = label
 
     def __rshift__(self, label):
         self.label = label
         return self
 
     def match_context(self, obj, context):
+        if obj is None:
+            context.is_match = False
+            return [context]
         result = self.regexp.match(obj)
         context.is_match = result is not None
         if self.label:
             context[self.label] = result
         return [context]
```

### Comparing `iguala-0.5.1/iguala/paths.py` & `iguala-0.5.2/iguala/paths.py`

 * *Files identical despite different names*

### Comparing `iguala-0.5.1/iguala.egg-info/PKG-INFO` & `iguala-0.5.2/iguala.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iguala
-Version: 0.5.1
+Version: 0.5.2
 Summary: Non-linear pattern matching for Python's objects, or rexep-like for objects
 Home-page: https://github.com/aranega/iguala
 Author: Vincent Aranega
 Author-email: vincent.aranega@gmail.com
 License: BSD 3-Clause
 Keywords: pattern matching matcher regexp graph query term rewriting
 Classifier: Development Status :: 4 - Beta
```

### Comparing `iguala-0.5.1/setup.py` & `iguala-0.5.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 if version < (3, 7):
     sys.exit('Sorry, Python < 3.7 is not supported')
 
 packages = ['iguala']
 
 setup(
     name='iguala',
-    version='0.5.1',
+    version='0.5.2',
     description=("Non-linear pattern matching for Python's objects, or rexep-like for objects"),
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     keywords='pattern matching matcher regexp graph query term rewriting',
     url='https://github.com/aranega/iguala',
     author='Vincent Aranega',
     author_email='vincent.aranega@gmail.com',
```

