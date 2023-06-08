# Comparing `tmp/yolo2labelme-0.0.3.tar.gz` & `tmp/yolo2labelme-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yolo2labelme-0.0.3.tar", last modified: Thu Jun  8 17:37:24 2023, max compression
+gzip compressed data, was "yolo2labelme-0.0.4.tar", last modified: Thu Jun  8 17:40:06 2023, max compression
```

## Comparing `yolo2labelme-0.0.3.tar` & `yolo2labelme-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 nithin    (1000) nithin    (1000)        0 2023-06-08 17:37:24.326660 yolo2labelme-0.0.3/
--rw-rw-r--   0 nithin    (1000) nithin    (1000)     1069 2023-06-04 14:00:21.000000 yolo2labelme-0.0.3/LICENSE
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      159 2023-06-08 17:37:24.326660 yolo2labelme-0.0.3/PKG-INFO
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      825 2023-06-08 17:33:33.000000 yolo2labelme-0.0.3/README.md
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      647 2023-06-08 17:36:29.000000 yolo2labelme-0.0.3/pyproject.toml
--rw-rw-r--   0 nithin    (1000) nithin    (1000)       38 2023-06-08 17:37:24.326660 yolo2labelme-0.0.3/setup.cfg
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      231 2023-06-08 17:37:03.000000 yolo2labelme-0.0.3/setup.py
-drwxrwxr-x   0 nithin    (1000) nithin    (1000)        0 2023-06-08 17:37:24.326660 yolo2labelme-0.0.3/yolo2labelme.egg-info/
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      159 2023-06-08 17:37:24.000000 yolo2labelme-0.0.3/yolo2labelme.egg-info/PKG-INFO
--rw-rw-r--   0 nithin    (1000) nithin    (1000)      240 2023-06-08 17:37:24.000000 yolo2labelme-0.0.3/yolo2labelme.egg-info/SOURCES.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)        1 2023-06-08 17:37:24.000000 yolo2labelme-0.0.3/yolo2labelme.egg-info/dependency_links.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)       52 2023-06-08 17:37:24.000000 yolo2labelme-0.0.3/yolo2labelme.egg-info/entry_points.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)       13 2023-06-08 17:37:24.000000 yolo2labelme-0.0.3/yolo2labelme.egg-info/top_level.txt
--rw-rw-r--   0 nithin    (1000) nithin    (1000)     3184 2023-06-08 17:07:33.000000 yolo2labelme-0.0.3/yolo2labelme.py
+drwxrwxr-x   0 nithin    (1000) nithin    (1000)        0 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)     1069 2023-06-04 14:00:21.000000 yolo2labelme-0.0.4/LICENSE
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)     1400 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/PKG-INFO
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)      825 2023-06-08 17:33:33.000000 yolo2labelme-0.0.4/README.md
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)      647 2023-06-08 17:40:00.000000 yolo2labelme-0.0.4/pyproject.toml
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)       38 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/setup.cfg
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)      231 2023-06-08 17:39:52.000000 yolo2labelme-0.0.4/setup.py
+drwxrwxr-x   0 nithin    (1000) nithin    (1000)        0 2023-06-08 17:40:06.007659 yolo2labelme-0.0.4/yolo2labelme.egg-info/
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)     1400 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/PKG-INFO
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)      240 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/SOURCES.txt
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)        1 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/dependency_links.txt
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)       51 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/entry_points.txt
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)       13 2023-06-08 17:40:06.000000 yolo2labelme-0.0.4/yolo2labelme.egg-info/top_level.txt
+-rw-rw-r--   0 nithin    (1000) nithin    (1000)     3184 2023-06-08 17:07:33.000000 yolo2labelme-0.0.4/yolo2labelme.py
```

### Comparing `yolo2labelme-0.0.3/LICENSE` & `yolo2labelme-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `yolo2labelme-0.0.3/README.md` & `yolo2labelme-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `yolo2labelme-0.0.3/pyproject.toml` & `yolo2labelme-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yolo2labelme"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Kadapalla Nithin Kumar", email="kadapallanithin@gmail.com" },
 ]
 description = "Tool to convert yolo format dataset to labelme json format."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `yolo2labelme-0.0.3/yolo2labelme.py` & `yolo2labelme-0.0.4/yolo2labelme.py`

 * *Files identical despite different names*

