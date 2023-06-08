# Comparing `tmp/wkw-1.1.8.tar.gz` & `tmp/wkw-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/wkw-1.1.8.tar", last modified: Thu Nov  5 10:20:08 2020, max compression
+gzip compressed data, was "dist/wkw-1.1.9.tar", last modified: Thu Nov  5 12:00:09 2020, max compression
```

## Comparing `wkw-1.1.8.tar` & `wkw-1.1.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:20:08.000000 wkw-1.1.8/
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw.egg-info/
--rw-r--r--   0 root         (0) root         (0)        1 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      249 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       11 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)      338 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)       10 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      249 2020-11-05 10:20:08.000000 wkw-1.1.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      186 2020-11-05 10:16:57.000000 wkw-1.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)       61 2020-11-05 10:16:57.000000 wkw-1.1.8/.gitignore
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:20:08.000000 wkw-1.1.8/tests/
--rw-r--r--   0 root         (0) root         (0)        0 2020-11-05 10:16:57.000000 wkw-1.1.8/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12377 2020-11-05 10:16:57.000000 wkw-1.1.8/tests/test_wkw.py
--rw-r--r--   0 root         (0) root         (0)      457 2020-11-05 10:16:57.000000 wkw-1.1.8/Dockerfile
--rw-r--r--   0 root         (0) root         (0)     2033 2020-11-05 10:16:57.000000 wkw-1.1.8/setup.py
--rw-r--r--   0 root         (0) root         (0)      928 2020-11-05 10:16:57.000000 wkw-1.1.8/Build-on-Windows.md
--rw-r--r--   0 root         (0) root         (0)       11 2020-11-05 10:16:57.000000 wkw-1.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)     1389 2020-11-05 10:16:57.000000 wkw-1.1.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw/
--rw-r--r--   0 root         (0) root         (0)       80 2020-11-05 10:16:57.000000 wkw-1.1.8/wkw/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7955 2020-11-05 10:16:57.000000 wkw-1.1.8/wkw/wkw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 10:20:08.000000 wkw-1.1.8/wkw/lib/
--rw-r--r--   0 root         (0) root         (0)      764 2020-11-05 10:19:05.000000 wkw-1.1.8/wkw/lib/wkw.h
--rwxr-xr-x   0 root         (0) root         (0)   211920 2020-11-05 10:19:05.000000 wkw-1.1.8/wkw/lib/liblz4.so.1
--rwxr-xr-x   0 root         (0) root         (0)  3238744 2020-11-05 10:19:05.000000 wkw-1.1.8/wkw/lib/libwkw.so
--rw-r--r--   0 root         (0) root         (0)       38 2020-11-05 10:20:08.000000 wkw-1.1.8/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 12:00:09.000000 wkw-1.1.9/
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw.egg-info/
+-rw-r--r--   0 root         (0) root         (0)        1 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       11 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      338 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      249 2020-11-05 12:00:09.000000 wkw-1.1.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      186 2020-11-05 11:56:54.000000 wkw-1.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)       61 2020-11-05 11:56:54.000000 wkw-1.1.9/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 12:00:09.000000 wkw-1.1.9/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2020-11-05 11:56:54.000000 wkw-1.1.9/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12377 2020-11-05 11:56:54.000000 wkw-1.1.9/tests/test_wkw.py
+-rw-r--r--   0 root         (0) root         (0)      457 2020-11-05 11:56:54.000000 wkw-1.1.9/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)     2033 2020-11-05 11:56:54.000000 wkw-1.1.9/setup.py
+-rw-r--r--   0 root         (0) root         (0)      928 2020-11-05 11:56:54.000000 wkw-1.1.9/Build-on-Windows.md
+-rw-r--r--   0 root         (0) root         (0)       11 2020-11-05 11:56:54.000000 wkw-1.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)     1389 2020-11-05 11:56:54.000000 wkw-1.1.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw/
+-rw-r--r--   0 root         (0) root         (0)       80 2020-11-05 11:56:54.000000 wkw-1.1.9/wkw/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7955 2020-11-05 11:56:54.000000 wkw-1.1.9/wkw/wkw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2020-11-05 12:00:09.000000 wkw-1.1.9/wkw/lib/
+-rw-r--r--   0 root         (0) root         (0)      764 2020-11-05 11:59:05.000000 wkw-1.1.9/wkw/lib/wkw.h
+-rwxr-xr-x   0 root         (0) root         (0)   211920 2020-11-05 11:59:05.000000 wkw-1.1.9/wkw/lib/liblz4.so.1
+-rwxr-xr-x   0 root         (0) root         (0)  3238744 2020-11-05 11:59:05.000000 wkw-1.1.9/wkw/lib/libwkw.so
+-rw-r--r--   0 root         (0) root         (0)       38 2020-11-05 12:00:09.000000 wkw-1.1.9/setup.cfg
```

### Comparing `wkw-1.1.8/tests/test_wkw.py` & `wkw-1.1.9/tests/test_wkw.py`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/setup.py` & `wkw-1.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/Build-on-Windows.md` & `wkw-1.1.9/Build-on-Windows.md`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/README.md` & `wkw-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/wkw/wkw.py` & `wkw-1.1.9/wkw/wkw.py`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/wkw/lib/wkw.h` & `wkw-1.1.9/wkw/lib/wkw.h`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/wkw/lib/liblz4.so.1` & `wkw-1.1.9/wkw/lib/liblz4.so.1`

 * *Files identical despite different names*

### Comparing `wkw-1.1.8/wkw/lib/libwkw.so` & `wkw-1.1.9/wkw/lib/libwkw.so`

 * *Files identical despite different names*

