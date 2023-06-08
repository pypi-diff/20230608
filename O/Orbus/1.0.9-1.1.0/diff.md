# Comparing `tmp/Orbus-1.0.9.tar.gz` & `tmp/Orbus-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orbus-1.0.9.tar", last modified: Thu Jun  8 04:11:22 2023, max compression
+gzip compressed data, was "Orbus-1.1.0.tar", last modified: Thu Jun  8 04:31:55 2023, max compression
```

## Comparing `Orbus-1.0.9.tar` & `Orbus-1.1.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 04:11:22.089747 Orbus-1.0.9/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.9/LICENSE
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 04:11:22.089747 Orbus-1.0.9/Orbus.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      868 2023-06-08 04:11:21.000000 Orbus-1.0.9/Orbus.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 04:11:21.000000 Orbus-1.0.9/Orbus.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 04:11:21.000000 Orbus-1.0.9/Orbus.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       61 2023-06-08 04:11:21.000000 Orbus-1.0.9/Orbus.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        6 2023-06-08 04:11:21.000000 Orbus-1.0.9/Orbus.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      868 2023-06-08 04:11:22.089747 Orbus-1.0.9/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      447 2023-06-08 04:09:44.000000 Orbus-1.0.9/README.md
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 04:11:22.089747 Orbus-1.0.9/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      819 2023-06-08 04:10:48.000000 Orbus-1.0.9/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 04:31:55.759524 Orbus-1.1.0/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 04:29:39.000000 Orbus-1.1.0/LICENSE
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 04:31:55.756191 Orbus-1.1.0/Orbus.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      870 2023-06-08 04:31:55.000000 Orbus-1.1.0/Orbus.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 04:31:55.000000 Orbus-1.1.0/Orbus.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 04:31:55.000000 Orbus-1.1.0/Orbus.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       61 2023-06-08 04:31:55.000000 Orbus-1.1.0/Orbus.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        6 2023-06-08 04:31:55.000000 Orbus-1.1.0/Orbus.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      870 2023-06-08 04:31:55.759524 Orbus-1.1.0/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      448 2023-06-08 04:28:45.000000 Orbus-1.1.0/README.md
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 04:31:55.759524 Orbus-1.1.0/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      821 2023-06-08 04:28:24.000000 Orbus-1.1.0/setup.py
```

### Comparing `Orbus-1.0.9/LICENSE` & `Orbus-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Orbus-1.0.9/Orbus.egg-info/PKG-INFO` & `Orbus-1.1.0/Orbus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Orbus
-Version: 1.0.9
+Version: 1.1.0
 Summary: An app skeleton creator, using CLI interface
-Home-page: https://github.com/OrbusCompany/OrbusMaker
+Home-page: https://github.com/Orbus-Company/OrbusMaker
 Author: Wilovy09
 Author-email: orbuscompany@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,11 +32,11 @@
 ```
 
 Esto generara una carpeta donde estemos ubicados.
 
 
 Links:
 - [Pypi](https://pypi.org/project/Orbus/)
-- [Github](https://github.com/OrbusCompany/OrbusMaker)
+- [Github](https://github.com/Orbus-Company/OrbusMaker)
 
 Actualizaciones:
 - [ ] Soporte a STREAMLIT
```

### Comparing `Orbus-1.0.9/PKG-INFO` & `Orbus-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: Orbus
-Version: 1.0.9
+Version: 1.1.0
 Summary: An app skeleton creator, using CLI interface
-Home-page: https://github.com/OrbusCompany/OrbusMaker
+Home-page: https://github.com/Orbus-Company/OrbusMaker
 Author: Wilovy09
 Author-email: orbuscompany@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,11 +32,11 @@
 ```
 
 Esto generara una carpeta donde estemos ubicados.
 
 
 Links:
 - [Pypi](https://pypi.org/project/Orbus/)
-- [Github](https://github.com/OrbusCompany/OrbusMaker)
+- [Github](https://github.com/Orbus-Company/OrbusMaker)
 
 Actualizaciones:
 - [ ] Soporte a STREAMLIT
```

### Comparing `Orbus-1.0.9/setup.py` & `Orbus-1.1.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as ld:
     long_description = ld.read()
 
 setup(
     name="Orbus",
-    version="1.0.9",
+    version="1.1.0",
     author="Wilovy09",
     author_email="orbuscompany@gmail.com",
     description="An app skeleton creator, using CLI interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
-    url="https://github.com/OrbusCompany/OrbusMaker",
+    url="https://github.com/Orbus-Company/OrbusMaker",
     project_url={
-        "Bug Tracker": "https://github.com/OrbusCompany/OrbusMaker/issues",
+        "Bug Tracker": "https://github.com/Orbus-Company/OrbusMaker/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     py_modules=["orbus"],
```

