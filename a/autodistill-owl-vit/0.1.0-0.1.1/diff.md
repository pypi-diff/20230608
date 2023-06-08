# Comparing `tmp/autodistill_owl_vit-0.1.0.tar.gz` & `tmp/autodistill_owl_vit-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autodistill_owl_vit-0.1.0.tar", last modified: Wed Jun  7 13:42:03 2023, max compression
+gzip compressed data, was "autodistill_owl_vit-0.1.1.tar", last modified: Thu Jun  8 14:00:34 2023, max compression
```

## Comparing `autodistill_owl_vit-0.1.0.tar` & `autodistill_owl_vit-0.1.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.107805 autodistill_owl_vit-0.1.0/
--rw-r--r--   0 james      (501) staff       (20)    10173 2023-06-07 13:04:07.000000 autodistill_owl_vit-0.1.0/LICENSE
--rw-r--r--   0 james      (501) staff       (20)     2227 2023-06-07 13:42:03.107651 autodistill_owl_vit-0.1.0/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)     1748 2023-06-07 13:40:23.000000 autodistill_owl_vit-0.1.0/README.md
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.105847 autodistill_owl_vit-0.1.0/autodistill_owl_vit/
--rw-r--r--   0 james      (501) staff       (20)       69 2023-06-06 08:41:04.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit/__init__.py
--rw-r--r--   0 james      (501) staff       (20)     1447 2023-06-06 09:25:50.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit/owlvit.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.107119 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/
--rw-r--r--   0 james      (501) staff       (20)     2227 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/PKG-INFO
--rw-r--r--   0 james      (501) staff       (20)      321 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/SOURCES.txt
--rw-r--r--   0 james      (501) staff       (20)        1 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/dependency_links.txt
--rw-r--r--   0 james      (501) staff       (20)       90 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/requires.txt
--rw-r--r--   0 james      (501) staff       (20)       20 2023-06-07 13:42:03.000000 autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/top_level.txt
--rw-r--r--   0 james      (501) staff       (20)       38 2023-06-07 13:42:03.107851 autodistill_owl_vit-0.1.0/setup.cfg
--rw-r--r--   0 james      (501) staff       (20)     1166 2023-06-07 13:41:09.000000 autodistill_owl_vit-0.1.0/setup.py
-drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-07 13:42:03.107301 autodistill_owl_vit-0.1.0/test/
--rw-r--r--   0 james      (501) staff       (20)       91 2023-06-06 08:40:14.000000 autodistill_owl_vit-0.1.0/test/test_hello.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:00:34.103814 autodistill_owl_vit-0.1.1/
+-rw-r--r--   0 james      (501) staff       (20)    10173 2023-06-07 13:04:07.000000 autodistill_owl_vit-0.1.1/LICENSE
+-rw-r--r--   0 james      (501) staff       (20)     2227 2023-06-08 14:00:34.103682 autodistill_owl_vit-0.1.1/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)     1748 2023-06-07 13:40:23.000000 autodistill_owl_vit-0.1.1/README.md
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:00:34.102079 autodistill_owl_vit-0.1.1/autodistill_owl_vit/
+-rw-r--r--   0 james      (501) staff       (20)       69 2023-06-08 14:00:26.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit/__init__.py
+-rw-r--r--   0 james      (501) staff       (20)     1447 2023-06-06 09:25:50.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit/owlvit.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:00:34.103224 autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/
+-rw-r--r--   0 james      (501) staff       (20)     2227 2023-06-08 14:00:34.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/PKG-INFO
+-rw-r--r--   0 james      (501) staff       (20)      321 2023-06-08 14:00:34.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/SOURCES.txt
+-rw-r--r--   0 james      (501) staff       (20)        1 2023-06-08 14:00:34.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/dependency_links.txt
+-rw-r--r--   0 james      (501) staff       (20)       90 2023-06-08 14:00:34.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/requires.txt
+-rw-r--r--   0 james      (501) staff       (20)       20 2023-06-08 14:00:34.000000 autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/top_level.txt
+-rw-r--r--   0 james      (501) staff       (20)       38 2023-06-08 14:00:34.103859 autodistill_owl_vit-0.1.1/setup.cfg
+-rw-r--r--   0 james      (501) staff       (20)     1166 2023-06-07 13:41:09.000000 autodistill_owl_vit-0.1.1/setup.py
+drwxr-xr-x   0 james      (501) staff       (20)        0 2023-06-08 14:00:34.103360 autodistill_owl_vit-0.1.1/test/
+-rw-r--r--   0 james      (501) staff       (20)       91 2023-06-06 08:40:14.000000 autodistill_owl_vit-0.1.1/test/test_hello.py
```

### Comparing `autodistill_owl_vit-0.1.0/LICENSE` & `autodistill_owl_vit-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `autodistill_owl_vit-0.1.0/PKG-INFO` & `autodistill_owl_vit-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill_owl_vit
-Version: 0.1.0
+Version: 0.1.1
 Summary: OWL-ViT module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-owl-vit
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_owl_vit-0.1.0/README.md` & `autodistill_owl_vit-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `autodistill_owl_vit-0.1.0/autodistill_owl_vit/owlvit.py` & `autodistill_owl_vit-0.1.1/autodistill_owl_vit/owlvit.py`

 * *Files identical despite different names*

### Comparing `autodistill_owl_vit-0.1.0/autodistill_owl_vit.egg-info/PKG-INFO` & `autodistill_owl_vit-0.1.1/autodistill_owl_vit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autodistill-owl-vit
-Version: 0.1.0
+Version: 0.1.1
 Summary: OWL-ViT module for use with Autodistill
 Home-page: https://github.com/autodistill/autodistill-owl-vit
 Author: Roboflow
 Author-email: support@roboflow.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `autodistill_owl_vit-0.1.0/setup.py` & `autodistill_owl_vit-0.1.1/setup.py`

 * *Files identical despite different names*

