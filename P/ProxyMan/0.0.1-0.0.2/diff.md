# Comparing `tmp/ProxyMan-0.0.1.tar.gz` & `tmp/ProxyMan-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ProxyMan-0.0.1.tar", last modified: Thu Jun  8 15:20:01 2023, max compression
+gzip compressed data, was "ProxyMan-0.0.2.tar", last modified: Thu Jun  8 15:23:58 2023, max compression
```

## Comparing `ProxyMan-0.0.1.tar` & `ProxyMan-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:20:01.029810 ProxyMan-0.0.1/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      546 2023-06-08 15:20:01.029679 ProxyMan-0.0.1/PKG-INFO
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:20:01.028717 ProxyMan-0.0.1/ProxyMan/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      126 2023-06-08 15:19:36.000000 ProxyMan-0.0.1/ProxyMan/__init__.py
--rw-r--r--   0 rawandahmad   (501) staff       (20)     6274 2023-06-08 15:19:36.000000 ProxyMan-0.0.1/ProxyMan/proxyman.py
-drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:20:01.029503 ProxyMan-0.0.1/ProxyMan.egg-info/
--rw-r--r--   0 rawandahmad   (501) staff       (20)      546 2023-06-08 15:20:00.000000 ProxyMan-0.0.1/ProxyMan.egg-info/PKG-INFO
--rw-r--r--   0 rawandahmad   (501) staff       (20)      209 2023-06-08 15:20:01.000000 ProxyMan-0.0.1/ProxyMan.egg-info/SOURCES.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-08 15:20:00.000000 ProxyMan-0.0.1/ProxyMan.egg-info/dependency_links.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        8 2023-06-08 15:20:00.000000 ProxyMan-0.0.1/ProxyMan.egg-info/requires.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-08 15:20:00.000000 ProxyMan-0.0.1/ProxyMan.egg-info/top_level.txt
--rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-08 15:20:01.029860 ProxyMan-0.0.1/setup.cfg
--rw-r--r--   0 rawandahmad   (501) staff       (20)      644 2023-06-08 15:03:25.000000 ProxyMan-0.0.1/setup.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:23:58.074757 ProxyMan-0.0.2/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     3040 2023-06-08 15:23:58.074587 ProxyMan-0.0.2/PKG-INFO
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:23:58.073711 ProxyMan-0.0.2/ProxyMan/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      126 2023-06-08 15:19:36.000000 ProxyMan-0.0.2/ProxyMan/__init__.py
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     6274 2023-06-08 15:19:36.000000 ProxyMan-0.0.2/ProxyMan/proxyman.py
+drwxr-xr-x   0 rawandahmad   (501) staff       (20)        0 2023-06-08 15:23:58.074392 ProxyMan-0.0.2/ProxyMan.egg-info/
+-rw-r--r--   0 rawandahmad   (501) staff       (20)     3040 2023-06-08 15:23:58.000000 ProxyMan-0.0.2/ProxyMan.egg-info/PKG-INFO
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      209 2023-06-08 15:23:58.000000 ProxyMan-0.0.2/ProxyMan.egg-info/SOURCES.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        1 2023-06-08 15:23:58.000000 ProxyMan-0.0.2/ProxyMan.egg-info/dependency_links.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        8 2023-06-08 15:23:58.000000 ProxyMan-0.0.2/ProxyMan.egg-info/requires.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)        9 2023-06-08 15:23:58.000000 ProxyMan-0.0.2/ProxyMan.egg-info/top_level.txt
+-rw-r--r--   0 rawandahmad   (501) staff       (20)       38 2023-06-08 15:23:58.074824 ProxyMan-0.0.2/setup.cfg
+-rw-r--r--   0 rawandahmad   (501) staff       (20)      820 2023-06-08 15:23:54.000000 ProxyMan-0.0.2/setup.py
```

### Comparing `ProxyMan-0.0.1/ProxyMan/proxyman.py` & `ProxyMan-0.0.2/ProxyMan/proxyman.py`

 * *Files identical despite different names*

