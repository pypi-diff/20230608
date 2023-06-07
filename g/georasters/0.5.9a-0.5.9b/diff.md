# Comparing `tmp/georasters-0.5.9a.tar.gz` & `tmp/georasters-0.5.9b.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/georasters-0.5.9a.tar", last modified: Wed Feb  7 17:30:49 2018, max compression
+gzip compressed data, was "dist/georasters-0.5.9b.tar", last modified: Wed Feb 21 14:43:03 2018, max compression
```

## Comparing `georasters-0.5.9a.tar` & `georasters-0.5.9b.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 bizcocho   (501) staff       (20)        0 2018-02-07 17:30:49.000000 georasters-0.5.9a/
-drwxr-xr-x   0 bizcocho   (501) staff       (20)        0 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters/
--rw-r--r--   0 bizcocho   (501) staff       (20)      824 2017-11-07 00:10:31.000000 georasters-0.5.9a/georasters/__init__.py
--rwxr-xr-x   0 bizcocho   (501) staff       (20)    60179 2018-02-07 17:25:45.000000 georasters-0.5.9a/georasters/georasters.py
-drwxr-xr-x   0 bizcocho   (501) staff       (20)        0 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters.egg-info/
--rw-r--r--   0 bizcocho   (501) staff       (20)        1 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters.egg-info/dependency_links.txt
--rw-r--r--   0 bizcocho   (501) staff       (20)        1 2014-12-02 01:53:06.000000 georasters-0.5.9a/georasters.egg-info/not-zip-safe
--rw-r--r--   0 bizcocho   (501) staff       (20)       47 2016-12-29 00:27:58.000000 georasters-0.5.9a/georasters.egg-info/pbr.json
--rw-r--r--   0 bizcocho   (501) staff       (20)     9111 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters.egg-info/PKG-INFO
--rw-r--r--   0 bizcocho   (501) staff       (20)      105 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters.egg-info/requires.txt
--rw-r--r--   0 bizcocho   (501) staff       (20)      310 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters.egg-info/SOURCES.txt
--rw-r--r--   0 bizcocho   (501) staff       (20)       11 2018-02-07 17:30:49.000000 georasters-0.5.9a/georasters.egg-info/top_level.txt
--rw-r--r--   0 bizcocho   (501) staff       (20)    35147 2016-12-29 00:10:00.000000 georasters-0.5.9a/LICENSE.txt
--rw-r--r--   0 bizcocho   (501) staff       (20)     9111 2018-02-07 17:30:49.000000 georasters-0.5.9a/PKG-INFO
--rw-r--r--   0 bizcocho   (501) staff       (20)     6263 2016-12-26 19:08:47.000000 georasters-0.5.9a/README.rst
--rw-r--r--   0 bizcocho   (501) staff       (20)       59 2018-02-07 17:30:49.000000 georasters-0.5.9a/setup.cfg
--rw-r--r--   0 bizcocho   (501) staff       (20)     2403 2018-02-07 17:30:33.000000 georasters-0.5.9a/setup.py
+drwxr-xr-x   0 bizcocho   (501) staff       (20)        0 2018-02-21 14:43:03.000000 georasters-0.5.9b/
+drwxr-xr-x   0 bizcocho   (501) staff       (20)        0 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters/
+-rw-r--r--   0 bizcocho   (501) staff       (20)      824 2017-11-07 00:10:31.000000 georasters-0.5.9b/georasters/__init__.py
+-rwxr-xr-x   0 bizcocho   (501) staff       (20)    60179 2018-02-07 17:25:45.000000 georasters-0.5.9b/georasters/georasters.py
+drwxr-xr-x   0 bizcocho   (501) staff       (20)        0 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters.egg-info/
+-rw-r--r--   0 bizcocho   (501) staff       (20)        1 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters.egg-info/dependency_links.txt
+-rw-r--r--   0 bizcocho   (501) staff       (20)        1 2014-12-02 01:53:06.000000 georasters-0.5.9b/georasters.egg-info/not-zip-safe
+-rw-r--r--   0 bizcocho   (501) staff       (20)       47 2016-12-29 00:27:58.000000 georasters-0.5.9b/georasters.egg-info/pbr.json
+-rw-r--r--   0 bizcocho   (501) staff       (20)     9111 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters.egg-info/PKG-INFO
+-rw-r--r--   0 bizcocho   (501) staff       (20)      105 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters.egg-info/requires.txt
+-rw-r--r--   0 bizcocho   (501) staff       (20)      310 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters.egg-info/SOURCES.txt
+-rw-r--r--   0 bizcocho   (501) staff       (20)       11 2018-02-21 14:43:03.000000 georasters-0.5.9b/georasters.egg-info/top_level.txt
+-rw-r--r--   0 bizcocho   (501) staff       (20)    35147 2016-12-29 00:10:00.000000 georasters-0.5.9b/LICENSE.txt
+-rw-r--r--   0 bizcocho   (501) staff       (20)     9111 2018-02-21 14:43:03.000000 georasters-0.5.9b/PKG-INFO
+-rw-r--r--   0 bizcocho   (501) staff       (20)     6263 2016-12-26 19:08:47.000000 georasters-0.5.9b/README.rst
+-rw-r--r--   0 bizcocho   (501) staff       (20)       59 2018-02-21 14:43:03.000000 georasters-0.5.9b/setup.cfg
+-rw-r--r--   0 bizcocho   (501) staff       (20)     2403 2018-02-21 14:42:37.000000 georasters-0.5.9b/setup.py
```

### Comparing `georasters-0.5.9a/georasters/__init__.py` & `georasters-0.5.9b/georasters/__init__.py`

 * *Files identical despite different names*

### Comparing `georasters-0.5.9a/georasters/georasters.py` & `georasters-0.5.9b/georasters/georasters.py`

 * *Files identical despite different names*

### Comparing `georasters-0.5.9a/georasters.egg-info/PKG-INFO` & `georasters-0.5.9b/georasters.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: georasters
-Version: 0.5.9a
+Version: 0.5.9b
 Summary: Tools for working with Geographical Information System Rasters
 Home-page: http://github.com/ozak/georasters
 Author: Ömer Özak
 Author-email: omer@omerozak.com
 License: GPLv3
 Description: .. PyPI download statistics are broken, but the new PyPI warehouse makes PyPI
         .. download statistics available through Google BigQuery
```

### Comparing `georasters-0.5.9a/LICENSE.txt` & `georasters-0.5.9b/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `georasters-0.5.9a/PKG-INFO` & `georasters-0.5.9b/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: georasters
-Version: 0.5.9a
+Version: 0.5.9b
 Summary: Tools for working with Geographical Information System Rasters
 Home-page: http://github.com/ozak/georasters
 Author: Ömer Özak
 Author-email: omer@omerozak.com
 License: GPLv3
 Description: .. PyPI download statistics are broken, but the new PyPI warehouse makes PyPI
         .. download statistics available through Google BigQuery
```

### Comparing `georasters-0.5.9a/README.rst` & `georasters-0.5.9b/README.rst`

 * *Files identical despite different names*

### Comparing `georasters-0.5.9a/setup.py` & `georasters-0.5.9b/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
     def run_tests(self):
         import pytest
         errno = pytest.main(self.test_args)
         sys.exit(errno)
 
 setup(name='georasters',
-      version='0.5.9a',
+      version='0.5.9b',
       description='Tools for working with Geographical Information System Rasters',
       url='http://github.com/ozak/georasters',
       keywords="gis geospatial geographic raster vector zonal statistics spatial analysis",
       author='Ömer Özak',
       author_email='omer@omerozak.com',
       license='GPLv3',
       #package_dir={'': 'src'},
```

