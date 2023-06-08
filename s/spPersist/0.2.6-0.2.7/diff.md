# Comparing `tmp/spPersist-0.2.6.tar.gz` & `tmp/spPersist-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.2.6.tar", last modified: Thu Jun  8 00:03:48 2023, max compression
+gzip compressed data, was "spPersist-0.2.7.tar", last modified: Thu Jun  8 00:07:46 2023, max compression
```

## Comparing `spPersist-0.2.6.tar` & `spPersist-0.2.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:03:48.008565 spPersist-0.2.6/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 23:31:47.000000 spPersist-0.2.6/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:03:48.008565 spPersist-0.2.6/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 23:31:47.000000 spPersist-0.2.6/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:03:48.008565 spPersist-0.2.6/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 00:03:29.000000 spPersist-0.2.6/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:03:48.005565 spPersist-0.2.6/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:03:48.007565 spPersist-0.2.6/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:00:39.000000 spPersist-0.2.6/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:30:58.000000 spPersist-0.2.6/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 23:30:58.000000 spPersist-0.2.6/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 00:00:39.000000 spPersist-0.2.6/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     3973 2023-06-08 00:01:56.000000 spPersist-0.2.6/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:03:48.008565 spPersist-0.2.6/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:03:47.000000 spPersist-0.2.6/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 00:03:48.000000 spPersist-0.2.6/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:03:47.000000 spPersist-0.2.6/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 00:03:48.000000 spPersist-0.2.6/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 00:03:48.000000 spPersist-0.2.6/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.740551 spPersist-0.2.7/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 23:31:47.000000 spPersist-0.2.7/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:07:46.740551 spPersist-0.2.7/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 23:31:47.000000 spPersist-0.2.7/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:07:46.740551 spPersist-0.2.7/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 00:07:32.000000 spPersist-0.2.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.737551 spPersist-0.2.7/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.739551 spPersist-0.2.7/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:00:39.000000 spPersist-0.2.7/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:30:58.000000 spPersist-0.2.7/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 23:30:58.000000 spPersist-0.2.7/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 00:00:39.000000 spPersist-0.2.7/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     3954 2023-06-08 00:07:10.000000 spPersist-0.2.7/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.739551 spPersist-0.2.7/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.2.6/LICENSE` & `spPersist-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.6/PKG-INFO` & `spPersist-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.6
+Version: 0.2.7
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `spPersist-0.2.6/README.md` & `spPersist-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.6/setup.py` & `spPersist-0.2.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.2.6",  # Required
+    version="0.2.7",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.2.6/src/spPersist/DTM_filtrations.py` & `spPersist-0.2.7/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.6/src/spPersist/dp.py` & `spPersist-0.2.7/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.6/src/spPersist/persistence_statistics.py` & `spPersist-0.2.7/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.6/src/spPersist/ph.py` & `spPersist-0.2.7/src/spPersist/ph.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from . import DTM_filtrations
-from DTM_filtrations import *
+from . import DTM_filtrations as dtm
 from . import persistence_statistics as ps
 
 import gudhi
 import numpy as np
 import matplotlib.pyplot as plt
 
 def compute_simplicial_complex(X,ptype: str,max_dimension=2,p=1,m=0.1,is_plot=False):
@@ -20,15 +19,15 @@
 
   # create a complex
   if ptype == 'Rips':
     st = gudhi.RipsComplex(points=X).create_simplex_tree(max_dimension)
   elif ptype == 'Alpha':
     st = gudhi.AlphaComplex(points=X).create_simplex_tree()
   elif ptype == 'DTM':
-    st = DTMFiltration(X, m, p, max_dimension)
+    st = dtm.DTMFiltration(X, m, p, max_dimension)
   else:
     raise ValueError('ptype is not one of Rips, Alpha or DTM.')
 
   # compute the persistence
   diagram = st.persistence()                                       
 
   # plot the persistence diagram
```

### Comparing `spPersist-0.2.6/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.2.7/src/spPersist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.6
+Version: 0.2.7
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

