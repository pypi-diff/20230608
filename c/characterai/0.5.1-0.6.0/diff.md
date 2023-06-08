# Comparing `tmp/characterai-0.5.1.tar.gz` & `tmp/characterai-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\characterai-0.5.1.tar", last modified: Fri May 26 09:36:12 2023, max compression
+gzip compressed data, was "dist\characterai-0.6.0.tar", last modified: Thu Jun  8 11:59:15 2023, max compression
```

## Comparing `characterai-0.5.1.tar` & `characterai-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-26 09:36:12.047120 characterai-0.5.1/
--rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.5.1/LICENSE
--rw-rw-rw-   0        0        0     1873 2023-05-26 09:36:12.046120 characterai-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0     1481 2023-05-01 15:25:41.000000 characterai-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-26 09:36:11.986474 characterai-0.5.1/characterai/
--rw-rw-rw-   0        0        0       90 2023-05-05 18:13:37.000000 characterai-0.5.1/characterai/__init__.py
--rw-rw-rw-   0        0        0     9061 2023-05-26 09:30:05.000000 characterai-0.5.1/characterai/characterai.py
--rw-rw-rw-   0        0        0      126 2023-05-16 17:53:10.000000 characterai-0.5.1/characterai/errors.py
--rw-rw-rw-   0        0        0     9455 2023-05-26 09:29:05.000000 characterai-0.5.1/characterai/pyasynccai.py
-drwxrwxrwx   0        0        0        0 2023-05-26 09:36:12.044122 characterai-0.5.1/characterai.egg-info/
--rw-rw-rw-   0        0        0     1873 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      299 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       19 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-05-26 09:36:11.000000 characterai-0.5.1/characterai.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-26 09:36:12.048122 characterai-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      622 2023-05-26 09:28:56.000000 characterai-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:59:15.681496 characterai-0.6.0/
+-rw-rw-rw-   0        0        0     1082 2023-04-28 16:51:34.000000 characterai-0.6.0/LICENSE
+-rw-rw-rw-   0        0        0     1696 2023-06-08 11:59:15.679492 characterai-0.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1304 2023-06-08 11:51:59.000000 characterai-0.6.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:59:15.614490 characterai-0.6.0/characterai/
+-rw-rw-rw-   0        0        0       90 2023-06-08 11:33:02.000000 characterai-0.6.0/characterai/__init__.py
+-rw-rw-rw-   0        0        0    15262 2023-06-08 11:33:12.000000 characterai-0.6.0/characterai/characterai.py
+-rw-rw-rw-   0        0        0      257 2023-06-08 11:33:21.000000 characterai-0.6.0/characterai/errors.py
+-rw-rw-rw-   0        0        0    15781 2023-06-08 11:32:46.000000 characterai-0.6.0/characterai/pyasynccai.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:59:15.674493 characterai-0.6.0/characterai.egg-info/
+-rw-rw-rw-   0        0        0     1696 2023-06-08 11:59:15.000000 characterai-0.6.0/characterai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      299 2023-06-08 11:59:15.000000 characterai-0.6.0/characterai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:59:15.000000 characterai-0.6.0/characterai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       19 2023-06-08 11:59:15.000000 characterai-0.6.0/characterai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-08 11:59:15.000000 characterai-0.6.0/characterai.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:59:15.682493 characterai-0.6.0/setup.cfg
+-rw-rw-rw-   0        0        0      622 2023-06-08 11:33:52.000000 characterai-0.6.0/setup.py
```

### Comparing `characterai-0.5.1/LICENSE` & `characterai-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `characterai-0.5.1/setup.py` & `characterai-0.6.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', encoding='utf8') as f:
     long_description = f.read()
 
 setup(
     name='characterai',
-    version='0.5.1',
+    version='0.6.0',
     author='kramcat',
     description='An unofficial API for character.ai for Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/kramcat/characterai',
     packages=find_packages(),
     install_requires=["playwright>=1.32.1"],
```

