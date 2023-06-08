# Comparing `tmp/Orbus-1.0.7.tar.gz` & `tmp/Orbus-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Orbus-1.0.7.tar", last modified: Thu Jun  8 03:37:25 2023, max compression
+gzip compressed data, was "Orbus-1.0.8.tar", last modified: Thu Jun  8 03:40:30 2023, max compression
```

## Comparing `Orbus-1.0.7.tar` & `Orbus-1.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:37:24.992971 Orbus-1.0.7/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.7/LICENSE
-drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:37:24.986304 Orbus-1.0.7/Orbus.egg-info/
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:37:24.000000 Orbus-1.0.7/Orbus.egg-info/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 03:37:24.000000 Orbus-1.0.7/Orbus.egg-info/SOURCES.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:37:24.000000 Orbus-1.0.7/Orbus.egg-info/dependency_links.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       61 2023-06-08 03:37:24.000000 Orbus-1.0.7/Orbus.egg-info/entry_points.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       11 2023-06-08 03:37:24.000000 Orbus-1.0.7/Orbus.egg-info/top_level.txt
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:37:24.989637 Orbus-1.0.7/PKG-INFO
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.7/README.md
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:37:24.992971 Orbus-1.0.7/setup.cfg
--rw-r--r--   0 wilovy    (1000) wilovy    (1000)      814 2023-06-08 03:34:21.000000 Orbus-1.0.7/setup.py
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:40:30.433185 Orbus-1.0.8/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)     1069 2023-06-08 02:54:32.000000 Orbus-1.0.8/LICENSE
+drwxr-xr-x   0 wilovy    (1000) wilovy    (1000)        0 2023-06-08 03:40:30.433185 Orbus-1.0.8/Orbus.egg-info/
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:40:30.000000 Orbus-1.0.8/Orbus.egg-info/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      174 2023-06-08 03:40:30.000000 Orbus-1.0.8/Orbus.egg-info/SOURCES.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        1 2023-06-08 03:40:30.000000 Orbus-1.0.8/Orbus.egg-info/dependency_links.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       61 2023-06-08 03:40:30.000000 Orbus-1.0.8/Orbus.egg-info/entry_points.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        6 2023-06-08 03:40:30.000000 Orbus-1.0.8/Orbus.egg-info/top_level.txt
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      423 2023-06-08 03:40:30.433185 Orbus-1.0.8/PKG-INFO
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)        8 2023-06-08 02:53:32.000000 Orbus-1.0.8/README.md
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)       38 2023-06-08 03:40:30.433185 Orbus-1.0.8/setup.cfg
+-rw-r--r--   0 wilovy    (1000) wilovy    (1000)      809 2023-06-08 03:40:16.000000 Orbus-1.0.8/setup.py
```

### Comparing `Orbus-1.0.7/LICENSE` & `Orbus-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `Orbus-1.0.7/setup.py` & `Orbus-1.0.8/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 
 with open("README.md", "r", encoding="utf-8") as ld:
     long_description = ld.read()
 
 setup(
     name="Orbus",
-    version="1.0.7",
+    version="1.0.8",
     author="Wilovy09",
     author_email="orbuscompany@gmail.com",
     description="An app skeleton creator, using CLI interface",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OrbusCompany/Orbus",
     project_url={
         "Bug Tracker": "https://github.com/OrbusCompany/Orbus/issues",
     },
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    py_modules=["orbusmaker"],
+    py_modules=["orbus"],
     entry_points={"console_scripts": ["create-flet-app = orbusmaker.__main__:FLET"]},
 )
```

