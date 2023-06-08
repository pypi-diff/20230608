# Comparing `tmp/hctest_record-1.0.tar.gz` & `tmp/hctest_record-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_record-1.0.tar", last modified: Thu Jun  8 05:57:36 2023, max compression
+gzip compressed data, was "dist/hctest_record-1.1.tar", last modified: Thu Jun  8 09:38:17 2023, max compression
```

## Comparing `hctest_record-1.0.tar` & `hctest_record-1.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 05:57:36.761886 hctest_record-1.0/
--rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 05:57:36.761262 hctest_record-1.0/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 05:57:36.757398 hctest_record-1.0/hc_record/
--rw-r--r--   0 mrding     (501) staff       (20)      106 2023-06-08 05:55:00.000000 hctest_record-1.0/hc_record/__init__.py
--rw-r--r--   0 mrding     (501) staff       (20)     1008 2023-06-07 14:07:01.000000 hctest_record-1.0/hc_record/record.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 05:57:36.760349 hctest_record-1.0/hctest_record.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 05:57:36.000000 hctest_record-1.0/hctest_record.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      198 2023-06-08 05:57:36.000000 hctest_record-1.0/hctest_record.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-06-08 05:57:36.000000 hctest_record-1.0/hctest_record.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)       10 2023-06-08 05:57:36.000000 hctest_record-1.0/hctest_record.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-06-08 05:57:36.762121 hctest_record-1.0/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)     1035 2023-06-08 05:57:06.000000 hctest_record-1.0/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:38:17.082226 hctest_record-1.1/
+-rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 09:38:17.081936 hctest_record-1.1/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:38:17.079329 hctest_record-1.1/hc_record/
+-rw-r--r--   0 mrding     (501) staff       (20)      106 2023-06-08 09:38:01.000000 hctest_record-1.1/hc_record/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     1008 2023-06-08 09:38:01.000000 hctest_record-1.1/hc_record/record.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:38:17.081399 hctest_record-1.1/hctest_record.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      234 2023-06-08 09:38:17.000000 hctest_record-1.1/hctest_record.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        9 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/requires.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       10 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-06-08 09:38:17.082318 hctest_record-1.1/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)     1054 2023-06-08 09:37:42.000000 hctest_record-1.1/setup.py
```

### Comparing `hctest_record-1.0/hc_record/record.py` & `hctest_record-1.1/hc_record/record.py`

 * *Files identical despite different names*

### Comparing `hctest_record-1.0/setup.py` & `hctest_record-1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,22 +6,23 @@
 python3 -m twine upload dist/*
 Could not find 'apksigner.jar' in ["C:\\Users\\wxy\\SDK\\platform-tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\emulator\\apksigner.jar","C:\\Users\\wxy\\SDK\\cmdline-tools\\latest\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\apksigner.jar"]
 """
 from setuptools import setup, find_packages
 
 setup(
     name="hctest_record",
-    version="1.0",
+    version="1.1",
     description="获取用例运行中的数据，并保存起来",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
     package_data={},
     install_requires=[
+        "requests"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
```

