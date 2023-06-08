# Comparing `tmp/spPersist-0.3.0.tar.gz` & `tmp/spPersist-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.3.0.tar", last modified: Thu Jun  8 03:06:26 2023, max compression
+gzip compressed data, was "spPersist-0.3.1.tar", last modified: Thu Jun  8 03:20:42 2023, max compression
```

## Comparing `spPersist-0.3.0.tar` & `spPersist-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.326749 spPersist-0.3.0/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 02:50:48.000000 spPersist-0.3.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:06:26.325749 spPersist-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1098 2023-06-08 02:50:48.000000 spPersist-0.3.0/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 03:06:26.326749 spPersist-0.3.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 03:06:10.000000 spPersist-0.3.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.322749 spPersist-0.3.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.324749 spPersist-0.3.0/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 02:50:15.000000 spPersist-0.3.0/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 03:05:07.000000 spPersist-0.3.0/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 02:50:14.000000 spPersist-0.3.0/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      639 2023-06-08 02:50:14.000000 spPersist-0.3.0/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 02:50:15.000000 spPersist-0.3.0/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4450 2023-06-08 02:50:14.000000 spPersist-0.3.0/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.325749 spPersist-0.3.0/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.137033 spPersist-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 02:50:48.000000 spPersist-0.3.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:20:42.137033 spPersist-0.3.1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-06-08 02:50:48.000000 spPersist-0.3.1/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 03:20:42.137033 spPersist-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 03:19:53.000000 spPersist-0.3.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.134033 spPersist-0.3.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.136033 spPersist-0.3.1/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 02:50:15.000000 spPersist-0.3.1/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 03:05:07.000000 spPersist-0.3.1/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 02:50:14.000000 spPersist-0.3.1/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 03:18:30.000000 spPersist-0.3.1/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 02:50:15.000000 spPersist-0.3.1/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-08 03:19:09.000000 spPersist-0.3.1/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.137033 spPersist-0.3.1/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.3.0/LICENSE` & `spPersist-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.0/PKG-INFO` & `spPersist-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.0
+Version: 0.3.1
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `spPersist-0.3.0/README.md` & `spPersist-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.0/setup.py` & `spPersist-0.3.1/setup.py`

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
-    version="0.3.0",  # Required
+    version="0.3.1",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.3.0/src/spPersist/DTM_filtrations.py` & `spPersist-0.3.1/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.0/src/spPersist/dp.py` & `spPersist-0.3.1/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.0/src/spPersist/hc.py` & `spPersist-0.3.1/src/spPersist/hc.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from . import ph
 
-def homological_classification(X, ptype:str):
+def homological_classification(st):
   '''
-  homological_classification takes a point cloud X
-  and ptype indicating the persistence computed,
-  and return a dictionary of homologies of X where
+  homological_classification takes a SimplexTree st,
+  and return a dictionary of homologies of st where
   the keys indicate connected components or n-dimensional
   holes and the values indicate the number of connected
   components or the number of holes of a given dimension.
   '''
 
   hc = {}
-  st = ph.compute_simplicial_complex(X,ptype=ptype)
   bn = st.betti_numbers()
   for i in range(len(bn)):
     if i == 0:
       hc['connected components'] = bn[i]
     else:
       hc[str(i)+'-dimensional holes'] = bn[i]
```

### Comparing `spPersist-0.3.0/src/spPersist/persistence_statistics.py` & `spPersist-0.3.1/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.0/src/spPersist/ph.py` & `spPersist-0.3.1/src/spPersist/ph.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,38 +118,38 @@
   
   gudhi.plot_persistence_diagram(diagram,band=2*hatc);
 
 
 def connected_components(st):
   '''
   connected_components takes a SimplexTree st and
-  return the number of connected components of X.
+  return the number of connected components of st.
   '''
 
   return st.betti_numbers()[0]
 
 
 def one_dimensional_holes(st):
   '''
   one_dimensional_holes takes a SimplexTree st and
-  return the number of one dimensional holes of X.
+  return the number of one dimensional holes of st.
   '''
 
   return st.betti_numbers()[1]
 
 
 def two_dimensional_holes(st):
   '''
   one_dimensional_holes takes a SimplexTree st and
-  return the number of one dimensional holes of X.
+  return the number of one dimensional holes of st.
   '''
 
   return st.betti_numbers()[2]
 
 
 def holes(st, dim: int):
   '''
   holes takes a SimplexTree st and return 
-  the number of holes of X in dimension dim.
+  the number of holes of st in dimension dim.
   '''
 
   return st.betti_numbers()[dim]
```

### Comparing `spPersist-0.3.0/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.3.1/src/spPersist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.0
+Version: 0.3.1
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

