# Comparing `tmp/hctest_record-1.1.tar.gz` & `tmp/hctest_record-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_record-1.1.tar", last modified: Thu Jun  8 09:38:17 2023, max compression
+gzip compressed data, was "dist/hctest_record-1.2.tar", last modified: Thu Jun  8 09:45:18 2023, max compression
```

## Comparing `hctest_record-1.1.tar` & `hctest_record-1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:38:17.082226 hctest_record-1.1/
--rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 09:38:17.081936 hctest_record-1.1/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:38:17.079329 hctest_record-1.1/hc_record/
--rw-r--r--   0 mrding     (501) staff       (20)      106 2023-06-08 09:38:01.000000 hctest_record-1.1/hc_record/__init__.py
--rw-r--r--   0 mrding     (501) staff       (20)     1008 2023-06-08 09:38:01.000000 hctest_record-1.1/hc_record/record.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:38:17.081399 hctest_record-1.1/hctest_record.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      234 2023-06-08 09:38:17.000000 hctest_record-1.1/hctest_record.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)        9 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/requires.txt
--rw-r--r--   0 mrding     (501) staff       (20)       10 2023-06-08 09:38:16.000000 hctest_record-1.1/hctest_record.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-06-08 09:38:17.082318 hctest_record-1.1/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)     1054 2023-06-08 09:37:42.000000 hctest_record-1.1/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:45:18.918952 hctest_record-1.2/
+-rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 09:45:18.918674 hctest_record-1.2/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:45:18.916060 hctest_record-1.2/hc_record/
+-rw-r--r--   0 mrding     (501) staff       (20)      106 2023-06-08 09:38:01.000000 hctest_record-1.2/hc_record/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     3998 2023-06-08 09:44:32.000000 hctest_record-1.2/hc_record/record.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-06-08 09:45:18.918202 hctest_record-1.2/hctest_record.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      423 2023-06-08 09:45:18.000000 hctest_record-1.2/hctest_record.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      234 2023-06-08 09:45:18.000000 hctest_record-1.2/hctest_record.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-06-08 09:45:18.000000 hctest_record-1.2/hctest_record.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        9 2023-06-08 09:45:18.000000 hctest_record-1.2/hctest_record.egg-info/requires.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       10 2023-06-08 09:45:18.000000 hctest_record-1.2/hctest_record.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-06-08 09:45:18.919044 hctest_record-1.2/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)     1054 2023-06-08 09:45:04.000000 hctest_record-1.2/setup.py
```

### Comparing `hctest_record-1.1/setup.py` & `hctest_record-1.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 python3 -m twine upload dist/*
 Could not find 'apksigner.jar' in ["C:\\Users\\wxy\\SDK\\platform-tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\emulator\\apksigner.jar","C:\\Users\\wxy\\SDK\\cmdline-tools\\latest\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\apksigner.jar"]
 """
 from setuptools import setup, find_packages
 
 setup(
     name="hctest_record",
-    version="1.1",
+    version="1.2",
     description="获取用例运行中的数据，并保存起来",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
     package_data={},
     install_requires=[
```

