# Comparing `tmp/Orbus-1.0.3.tar.gz` & `tmp/Orbus-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orbus-1.0.3.tar", last modified: Thu Jun  8 02:59:13 2023, max compression
+gzip compressed data, was "Orbus-1.0.4.tar", last modified: Thu Jun  8 03:15:16 2023, max compression
```

## Comparing `Orbus-1.0.3.tar` & `Orbus-1.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:59:13.141567 Orbus-1.0.3/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.3/LICENSE
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      446 2023-06-08 02:59:13.141567 Orbus-1.0.3/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.3/README.md
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 02:59:13.148233 Orbus-1.0.3/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1213 2023-06-08 02:59:06.000000 Orbus-1.0.3/setup.py
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:59:13.134900 Orbus-1.0.3/src/
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 02:59:13.138233 Orbus-1.0.3/src/Orbus.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      446 2023-06-08 02:59:12.000000 Orbus-1.0.3/src/Orbus.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      212 2023-06-08 02:59:13.000000 Orbus-1.0.3/src/Orbus.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 02:59:12.000000 Orbus-1.0.3/src/Orbus.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       56 2023-06-08 02:59:12.000000 Orbus-1.0.3/src/Orbus.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 02:59:12.000000 Orbus-1.0.3/src/Orbus.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       46 2023-06-08 02:51:42.000000 Orbus-1.0.3/src/orbusmaker.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:15:16.602194 Orbus-1.0.4/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.4/LICENSE
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      446 2023-06-08 03:15:16.602194 Orbus-1.0.4/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.4/README.md
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:15:16.602194 Orbus-1.0.4/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      958 2023-06-08 03:14:55.000000 Orbus-1.0.4/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:15:16.602194 Orbus-1.0.4/src/
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:15:16.602194 Orbus-1.0.4/src/Orbus.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      446 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      212 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       56 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 03:15:16.000000 Orbus-1.0.4/src/Orbus.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       35 2023-06-08 03:01:30.000000 Orbus-1.0.4/src/orbusmaker.py
```

### Comparing `Orbus-1.0.3/LICENSE` & `Orbus-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `Orbus-1.0.3/setup.py` & `Orbus-1.0.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,15 @@
-# from setuptools import setup
-
-# setup(
-#     name="mi_libreria",
-#     version="0.5",
-#     py_modules=["mi_libreria"],
-#     entry_points={
-#         "console_scripts": [
-#             "mi_libreria = mi_libreria.__main__:main"
-#         ]
-#     }
-# )
-
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as ld:
     long_description = ld.read()
 
 setuptools.setup(
     name="Orbus",
-    version="1.0.3",
+    version="1.0.4",
     author="Wilovy09",
     author_email="orbuscompany@gmail.com",
     description="An app skeleton creator, using CLI interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OrbusCompany/Orbus",
     project_url={
```

