# Comparing `tmp/arvados_fuse-2.6.3.tar.gz` & `tmp/arvados_fuse-2.6.3rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados_fuse-2.6.3.tar", last modified: Thu Jun  8 21:55:19 2023, max compression
+gzip compressed data, was ".upload_dist/arvados_fuse-2.6.3rc1.tar", last modified: Thu Jun  1 21:38:22 2023, max compression
```

## Comparing `arvados_fuse-2.6.3.tar` & `arvados_fuse-2.6.3rc1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      163 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3082 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2122 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/README.rst
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/agpl-3.0.txt
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28592 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21422 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/command.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2551 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/crunchstat.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4238 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/fresh.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    52126 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/fusedir.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4331 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/fusefile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6742 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_fuse/unmount.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3082 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      487 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      137 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       13 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/arvados_fuse.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      281 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/bin/arv-mount
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-08 21:55:19.000000 arvados_fuse-2.6.3/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1874 2023-06-08 21:55:04.000000 arvados_fuse-2.6.3/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      163 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3085 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2122 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/README.rst
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    34520 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/agpl-3.0.txt
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    28592 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    21422 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/command.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2551 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/crunchstat.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4238 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/fresh.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    52126 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/fusedir.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4331 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/fusefile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6742 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_fuse/unmount.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3085 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      487 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:40.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      140 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       13 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2028 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      281 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/bin/arv-mount
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-06-01 21:38:22.000000 arvados_fuse-2.6.3rc1/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1874 2023-06-01 21:38:09.000000 arvados_fuse-2.6.3rc1/setup.py
```

### Comparing `arvados_fuse-2.6.3/PKG-INFO` & `arvados_fuse-2.6.3rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados_fuse
-Version: 2.6.3
+Version: 2.6.3rc1
 Summary: Arvados FUSE driver
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: GNU Affero General Public License, version 3.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados_fuse-2.6.3/README.rst` & `arvados_fuse-2.6.3rc1/README.rst`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/agpl-3.0.txt` & `arvados_fuse-2.6.3rc1/agpl-3.0.txt`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/__init__.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/command.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/command.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/crunchstat.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/crunchstat.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/fresh.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/fresh.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/fusedir.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/fusedir.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/fusefile.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/fusefile.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse/unmount.py` & `arvados_fuse-2.6.3rc1/arvados_fuse/unmount.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/arvados_fuse.egg-info/PKG-INFO` & `arvados_fuse-2.6.3rc1/arvados_fuse.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-fuse
-Version: 2.6.3
+Version: 2.6.3rc1
 Summary: Arvados FUSE driver
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: GNU Affero General Public License, version 3.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados_fuse-2.6.3/arvados_version.py` & `arvados_fuse-2.6.3rc1/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados_fuse-2.6.3/setup.py` & `arvados_fuse-2.6.3rc1/setup.py`

 * *Files identical despite different names*

