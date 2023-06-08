# Comparing `tmp/encoo-1.0.1.tar.gz` & `tmp/encoo-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoo-1.0.1.tar", last modified: Thu Apr  6 06:39:55 2023, max compression
+gzip compressed data, was "encoo-2023.6.8.tar", last modified: Thu Jun  8 02:19:56 2023, max compression
```

## Comparing `encoo-1.0.1.tar` & `encoo-2023.6.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-06 06:39:55.523434 encoo-1.0.1/
--rw-rw-rw-   0        0        0       52 2023-04-06 06:39:55.521368 encoo-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-06 06:39:55.502914 encoo-1.0.1/encoo/
--rw-rw-rw-   0        0        0       21 2023-03-12 06:33:22.000000 encoo-1.0.1/encoo/__init__.py
--rw-rw-rw-   0        0        0     1672 2023-03-31 06:16:15.000000 encoo-1.0.1/encoo/config.py
--rw-rw-rw-   0        0        0     1659 2023-04-04 09:57:56.000000 encoo-1.0.1/encoo/eml.py
--rw-rw-rw-   0        0        0     1283 2023-03-29 10:16:12.000000 encoo-1.0.1/encoo/logger.py
--rw-rw-rw-   0        0        0      969 2023-03-13 08:42:33.000000 encoo-1.0.1/encoo/util.py
-drwxrwxrwx   0        0        0        0 2023-04-06 06:39:55.518066 encoo-1.0.1/encoo.egg-info/
--rw-rw-rw-   0        0        0       52 2023-04-06 06:39:55.000000 encoo-1.0.1/encoo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      229 2023-04-06 06:39:55.000000 encoo-1.0.1/encoo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-06 06:39:55.000000 encoo-1.0.1/encoo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       84 2023-04-06 06:39:55.000000 encoo-1.0.1/encoo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-06 06:39:55.000000 encoo-1.0.1/encoo.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-06 06:39:55.523434 encoo-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      449 2023-04-06 06:39:38.000000 encoo-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:19:56.552573 encoo-2023.6.8/
+-rw-rw-rw-   0        0        0       55 2023-06-08 02:19:56.550640 encoo-2023.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 02:19:56.524576 encoo-2023.6.8/encoo/
+-rw-rw-rw-   0        0        0       21 2023-03-12 06:33:22.000000 encoo-2023.6.8/encoo/__init__.py
+-rw-rw-rw-   0        0        0     1672 2023-03-31 06:16:15.000000 encoo-2023.6.8/encoo/config.py
+-rw-rw-rw-   0        0        0     1659 2023-04-04 09:57:56.000000 encoo-2023.6.8/encoo/eml.py
+-rw-rw-rw-   0        0        0     1283 2023-03-29 10:16:12.000000 encoo-2023.6.8/encoo/logger.py
+-rw-rw-rw-   0        0        0      969 2023-03-13 08:42:33.000000 encoo-2023.6.8/encoo/util.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:19:56.544574 encoo-2023.6.8/encoo.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-06-08 02:19:56.000000 encoo-2023.6.8/encoo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      229 2023-06-08 02:19:56.000000 encoo-2023.6.8/encoo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:19:56.000000 encoo-2023.6.8/encoo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       84 2023-06-08 02:19:56.000000 encoo-2023.6.8/encoo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 02:19:56.000000 encoo-2023.6.8/encoo.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:19:56.554612 encoo-2023.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      452 2023-06-08 02:19:43.000000 encoo-2023.6.8/setup.py
```

### Comparing `encoo-1.0.1/encoo/config.py` & `encoo-2023.6.8/encoo/config.py`

 * *Files identical despite different names*

### Comparing `encoo-1.0.1/encoo/eml.py` & `encoo-2023.6.8/encoo/eml.py`

 * *Files identical despite different names*

### Comparing `encoo-1.0.1/encoo/logger.py` & `encoo-2023.6.8/encoo/logger.py`

 * *Files identical despite different names*

### Comparing `encoo-1.0.1/encoo/util.py` & `encoo-2023.6.8/encoo/util.py`

 * *Files identical despite different names*

