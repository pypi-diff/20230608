# Comparing `tmp/python-eigen-ingenuity-0.4.8.tar.gz` & `tmp/python-eigen-ingenuity-0.4.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-eigen-ingenuity-0.4.8.tar", last modified: Wed Jun  7 12:12:42 2023, max compression
+gzip compressed data, was "python-eigen-ingenuity-0.4.8.1.tar", last modified: Thu Jun  8 08:35:19 2023, max compression
```

## Comparing `python-eigen-ingenuity-0.4.8.tar` & `python-eigen-ingenuity-0.4.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.729014 python-eigen-ingenuity-0.4.8/
--rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/LICENSE
--rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.8/MANIFEST.in
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-07 12:12:42.728734 python-eigen-ingenuity-0.4.8/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/README.md
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.727292 python-eigen-ingenuity-0.4.8/eigeningenuity/
--rw-r--r--   0 berhic     (501) staff       (20)     1205 2023-05-23 15:38:30.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/assetmodel.py
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.727647 python-eigen-ingenuity-0.4.8/eigeningenuity/core/
--rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/core/__init__.py
--rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/core/debug.py
--rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/elastic.py
--rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/events.py
--rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/historian.py
--rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/smartdash.py
--rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/sql.py
--rw-r--r--   0 berhic     (501) staff       (20)    15067 2023-06-07 12:09:52.000000 python-eigen-ingenuity-0.4.8/eigeningenuity/util.py
--rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8/pyproject.toml
-drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-07 12:12:42.728508 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/
--rw-r--r--   0 berhic     (501) staff       (20)    11663 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/PKG-INFO
--rw-r--r--   0 berhic     (501) staff       (20)      551 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/SOURCES.txt
--rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/dependency_links.txt
--rw-r--r--   0 berhic     (501) staff       (20)       24 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/requires.txt
--rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-07 12:12:42.000000 python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/top_level.txt
--rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-07 12:12:42.729074 python-eigen-ingenuity-0.4.8/setup.cfg
--rw-r--r--   0 berhic     (501) staff       (20)      689 2023-06-07 12:12:34.000000 python-eigen-ingenuity-0.4.8/setup.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 08:35:19.324661 python-eigen-ingenuity-0.4.8.1/
+-rw-r--r--   0 berhic     (501) staff       (20)      578 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.1/LICENSE
+-rw-r--r--   0 berhic     (501) staff       (20)       70 2022-11-30 15:55:19.000000 python-eigen-ingenuity-0.4.8.1/MANIFEST.in
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-06-08 08:35:19.324417 python-eigen-ingenuity-0.4.8.1/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)    11343 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.1/README.md
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 08:35:19.323028 python-eigen-ingenuity-0.4.8.1/eigeningenuity/
+-rw-r--r--   0 berhic     (501) staff       (20)     1205 2023-05-23 15:38:30.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)    16232 2023-05-18 14:59:11.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/assetmodel.py
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 08:35:19.323365 python-eigen-ingenuity-0.4.8.1/eigeningenuity/core/
+-rw-r--r--   0 berhic     (501) staff       (20)     7741 2023-05-23 15:25:59.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/core/__init__.py
+-rw-r--r--   0 berhic     (501) staff       (20)     1146 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/core/debug.py
+-rw-r--r--   0 berhic     (501) staff       (20)     6250 2023-05-17 13:22:24.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/elastic.py
+-rw-r--r--   0 berhic     (501) staff       (20)     3054 2023-05-17 13:22:33.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/events.py
+-rw-r--r--   0 berhic     (501) staff       (20)    36274 2023-05-24 08:12:38.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/historian.py
+-rw-r--r--   0 berhic     (501) staff       (20)     2843 2023-05-17 13:22:46.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/smartdash.py
+-rw-r--r--   0 berhic     (501) staff       (20)     4081 2023-05-17 13:22:51.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/sql.py
+-rw-r--r--   0 berhic     (501) staff       (20)    15067 2023-06-08 08:34:28.000000 python-eigen-ingenuity-0.4.8.1/eigeningenuity/util.py
+-rw-r--r--   0 berhic     (501) staff       (20)       92 2022-08-16 09:33:43.000000 python-eigen-ingenuity-0.4.8.1/pyproject.toml
+drwxr-xr-x   0 berhic     (501) staff       (20)        0 2023-06-08 08:35:19.324176 python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/
+-rw-r--r--   0 berhic     (501) staff       (20)    11665 2023-06-08 08:35:19.000000 python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/PKG-INFO
+-rw-r--r--   0 berhic     (501) staff       (20)      551 2023-06-08 08:35:19.000000 python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/SOURCES.txt
+-rw-r--r--   0 berhic     (501) staff       (20)        1 2023-06-08 08:35:19.000000 python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/dependency_links.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       24 2023-06-08 08:35:19.000000 python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/requires.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       15 2023-06-08 08:35:19.000000 python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/top_level.txt
+-rw-r--r--   0 berhic     (501) staff       (20)       38 2023-06-08 08:35:19.324724 python-eigen-ingenuity-0.4.8.1/setup.cfg
+-rw-r--r--   0 berhic     (501) staff       (20)      691 2023-06-08 08:35:00.000000 python-eigen-ingenuity-0.4.8.1/setup.py
```

### Comparing `python-eigen-ingenuity-0.4.8/LICENSE` & `python-eigen-ingenuity-0.4.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/PKG-INFO` & `python-eigen-ingenuity-0.4.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.8
+Version: 0.4.8.1
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.8/README.md` & `python-eigen-ingenuity-0.4.8.1/README.md`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/__init__.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/assetmodel.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/assetmodel.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/core/__init__.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/core/__init__.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/core/debug.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/core/debug.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/elastic.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/elastic.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/events.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/events.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/historian.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/historian.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/smartdash.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/smartdash.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/sql.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/sql.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/eigeningenuity/util.py` & `python-eigen-ingenuity-0.4.8.1/eigeningenuity/util.py`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/PKG-INFO` & `python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-eigen-ingenuity
-Version: 0.4.8
+Version: 0.4.8.1
 Summary: A python library used to query data from the Eigen Ingenuity system
 Home-page: https://www.eigen.co/
 Author: Murray Callander
 Author-email: info@eigen.co
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `python-eigen-ingenuity-0.4.8/python_eigen_ingenuity.egg-info/SOURCES.txt` & `python-eigen-ingenuity-0.4.8.1/python_eigen_ingenuity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-eigen-ingenuity-0.4.8/setup.py` & `python-eigen-ingenuity-0.4.8.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 README = (HERE / "README.md").read_text()
 
 pkgname = 'python-eigen-ingenuity'
 
 # Invoke setup
 setup(
     name=pkgname,
-    version='0.4.8',
+    version='0.4.8.1',
     author='Murray Callander',
     author_email='info@eigen.co',
     url='https://www.eigen.co/',
     description="A python library used to query data from the Eigen Ingenuity system",
     long_description=README,
     long_description_content_type="text/markdown",
     packages=find_packages("."),
```

