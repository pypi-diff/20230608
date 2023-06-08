# Comparing `tmp/quran_downloader-0.0.3.tar.gz` & `tmp/quran_downloader-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quran_downloader-0.0.3.tar", last modified: Thu Jun  8 09:44:28 2023, max compression
+gzip compressed data, was "quran_downloader-0.0.4.tar", last modified: Thu Jun  8 09:54:10 2023, max compression
```

## Comparing `quran_downloader-0.0.3.tar` & `quran_downloader-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:44:28.461549 quran_downloader-0.0.3/
--rw-rw-rw-   0        0        0      546 2023-06-08 09:44:28.460581 quran_downloader-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 09:44:28.449585 quran_downloader-0.0.3/quran-downloader/
--rw-rw-rw-   0        0        0      152 2023-06-08 09:43:56.000000 quran_downloader-0.0.3/quran-downloader/__init__.py
--rw-rw-rw-   0        0        0      239 2023-06-05 18:09:39.000000 quran_downloader-0.0.3/quran-downloader/consts.py
--rw-rw-rw-   0        0        0       64 2023-06-05 18:11:38.000000 quran_downloader-0.0.3/quran-downloader/download.py
--rw-rw-rw-   0        0        0     4652 2023-06-05 18:06:50.000000 quran_downloader-0.0.3/quran-downloader/download_org.py
--rw-rw-rw-   0        0        0     1923 2023-06-08 09:41:35.000000 quran_downloader-0.0.3/quran-downloader/download_verse.py
--rw-rw-rw-   0        0        0     1565 2023-06-08 09:40:28.000000 quran_downloader-0.0.3/quran-downloader/download_word.py
--rw-rw-rw-   0        0        0      342 2023-06-05 18:08:56.000000 quran_downloader-0.0.3/quran-downloader/verse_key_converters.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:44:28.459550 quran_downloader-0.0.3/quran_downloader.egg-info/
--rw-rw-rw-   0        0        0      546 2023-06-08 09:44:28.000000 quran_downloader-0.0.3/quran_downloader.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      396 2023-06-08 09:44:28.000000 quran_downloader-0.0.3/quran_downloader.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:44:28.000000 quran_downloader-0.0.3/quran_downloader.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-08 09:44:28.000000 quran_downloader-0.0.3/quran_downloader.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 09:44:28.461549 quran_downloader-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1110 2023-06-08 09:44:21.000000 quran_downloader-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:54:10.611941 quran_downloader-0.0.4/
+-rw-rw-rw-   0        0        0      546 2023-06-08 09:54:10.610943 quran_downloader-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 09:54:10.590214 quran_downloader-0.0.4/quran_downloader/
+-rw-rw-rw-   0        0        0      152 2023-06-08 09:43:56.000000 quran_downloader-0.0.4/quran_downloader/__init__.py
+-rw-rw-rw-   0        0        0      239 2023-06-05 18:09:39.000000 quran_downloader-0.0.4/quran_downloader/consts.py
+-rw-rw-rw-   0        0        0       64 2023-06-05 18:11:38.000000 quran_downloader-0.0.4/quran_downloader/download.py
+-rw-rw-rw-   0        0        0     4652 2023-06-05 18:06:50.000000 quran_downloader-0.0.4/quran_downloader/download_org.py
+-rw-rw-rw-   0        0        0     1923 2023-06-08 09:41:35.000000 quran_downloader-0.0.4/quran_downloader/download_verse.py
+-rw-rw-rw-   0        0        0     1565 2023-06-08 09:40:28.000000 quran_downloader-0.0.4/quran_downloader/download_word.py
+-rw-rw-rw-   0        0        0      342 2023-06-05 18:08:56.000000 quran_downloader-0.0.4/quran_downloader/verse_key_converters.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:54:10.609945 quran_downloader-0.0.4/quran_downloader.egg-info/
+-rw-rw-rw-   0        0        0      546 2023-06-08 09:54:10.000000 quran_downloader-0.0.4/quran_downloader.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      396 2023-06-08 09:54:10.000000 quran_downloader-0.0.4/quran_downloader.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:54:10.000000 quran_downloader-0.0.4/quran_downloader.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-08 09:54:10.000000 quran_downloader-0.0.4/quran_downloader.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 09:54:10.611941 quran_downloader-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1110 2023-06-08 09:46:35.000000 quran_downloader-0.0.4/setup.py
```

### Comparing `quran_downloader-0.0.3/PKG-INFO` & `quran_downloader-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quran_downloader
-Version: 0.0.3
+Version: 0.0.4
 Summary: download quran verses
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,quran,audio,reciter,verses
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quran_downloader-0.0.3/quran-downloader/download_org.py` & `quran_downloader-0.0.4/quran_downloader/download_org.py`

 * *Files identical despite different names*

### Comparing `quran_downloader-0.0.3/quran-downloader/download_verse.py` & `quran_downloader-0.0.4/quran_downloader/download_verse.py`

 * *Files identical despite different names*

### Comparing `quran_downloader-0.0.3/quran-downloader/download_word.py` & `quran_downloader-0.0.4/quran_downloader/download_word.py`

 * *Files identical despite different names*

### Comparing `quran_downloader-0.0.3/quran_downloader.egg-info/PKG-INFO` & `quran_downloader-0.0.4/quran_downloader.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quran-downloader
-Version: 0.0.3
+Version: 0.0.4
 Summary: download quran verses
 Author: Malik
 Author-email: myemail46926213@gmail.com
 Keywords: python,quran,audio,reciter,verses
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `quran_downloader-0.0.3/setup.py` & `quran_downloader-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # import os
 
 # here = os.path.abspath(os.path.dirname(__file__))
 
 # with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
 #     long_description = "\n" + fh.read()
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'download quran verses'
 LONG_DESCRIPTION = 'download quran verses'
 
 # Setting up
 setup(
     name="quran_downloader",
     version=VERSION,
```

