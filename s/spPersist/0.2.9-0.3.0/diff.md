# Comparing `tmp/spPersist-0.2.9.tar.gz` & `tmp/spPersist-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.2.9.tar", last modified: Thu Jun  8 00:43:10 2023, max compression
+gzip compressed data, was "spPersist-0.3.0.tar", last modified: Thu Jun  8 03:06:26 2023, max compression
```

## Comparing `spPersist-0.2.9.tar` & `spPersist-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:43:10.811502 spPersist-0.2.9/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 23:31:47.000000 spPersist-0.2.9/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:43:10.811502 spPersist-0.2.9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 23:31:47.000000 spPersist-0.2.9/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:43:10.811502 spPersist-0.2.9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 00:42:56.000000 spPersist-0.2.9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:43:10.809502 spPersist-0.2.9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:43:10.810502 spPersist-0.2.9/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:00:39.000000 spPersist-0.2.9/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:30:58.000000 spPersist-0.2.9/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 23:30:58.000000 spPersist-0.2.9/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      634 2023-06-08 00:42:00.000000 spPersist-0.2.9/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 00:00:39.000000 spPersist-0.2.9/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4530 2023-06-08 00:18:56.000000 spPersist-0.2.9/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:43:10.811502 spPersist-0.2.9/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:43:10.000000 spPersist-0.2.9/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 00:43:10.000000 spPersist-0.2.9/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:43:10.000000 spPersist-0.2.9/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 00:43:10.000000 spPersist-0.2.9/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 00:43:10.000000 spPersist-0.2.9/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.326749 spPersist-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 02:50:48.000000 spPersist-0.3.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:06:26.325749 spPersist-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-06-08 02:50:48.000000 spPersist-0.3.0/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 03:06:26.326749 spPersist-0.3.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 03:06:10.000000 spPersist-0.3.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.322749 spPersist-0.3.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.324749 spPersist-0.3.0/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 02:50:15.000000 spPersist-0.3.0/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 03:05:07.000000 spPersist-0.3.0/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 02:50:14.000000 spPersist-0.3.0/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      639 2023-06-08 02:50:14.000000 spPersist-0.3.0/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 02:50:15.000000 spPersist-0.3.0/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4450 2023-06-08 02:50:14.000000 spPersist-0.3.0/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:06:26.325749 spPersist-0.3.0/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 03:06:26.000000 spPersist-0.3.0/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.2.9/LICENSE` & `spPersist-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.9/PKG-INFO` & `spPersist-0.3.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.9
+Version: 0.3.0
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
@@ -16,10 +16,18 @@
 spatial topology. The specific mathematical foundation for the classification is
 the theory of Persistent Homology and its homology barcodes. The package so far
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
-It is intended that the package will also include a pre-processing module, a 
+The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
 named pp, ph and hc.
+
+The persistent homology module contains functions for computing simplicial 
+complexes of point clouds (See data structures in the gudhi package.) and their
+topological measures. It also includes plotting features of the persistence 
+diagram.
+
+The homological classification module computes the number of holes and connected
+components as a dictionary.
```

### Comparing `spPersist-0.2.9/setup.py` & `spPersist-0.3.0/setup.py`

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
-    version="0.2.9",  # Required
+    version="0.3.0",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.2.9/src/spPersist/DTM_filtrations.py` & `spPersist-0.3.0/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.9/src/spPersist/dp.py` & `spPersist-0.3.0/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.9/src/spPersist/hc.py` & `spPersist-0.3.0/src/spPersist/hc.py`

 * *Files 24% similar despite different names*

```diff
@@ -9,14 +9,14 @@
   holes and the values indicate the number of connected
   components or the number of holes of a given dimension.
   '''
 
   hc = {}
   st = ph.compute_simplicial_complex(X,ptype=ptype)
   bn = st.betti_numbers()
-  for i in range(bn):
+  for i in range(len(bn)):
     if i == 0:
       hc['connected components'] = bn[i]
     else:
       hc[str(i)+'-dimensional holes'] = bn[i]
 
   return hc
```

### Comparing `spPersist-0.2.9/src/spPersist/persistence_statistics.py` & `spPersist-0.3.0/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.9/src/spPersist/ph.py` & `spPersist-0.3.0/src/spPersist/ph.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,64 +1,81 @@
 from . import DTM_filtrations as dtm
 from . import persistence_statistics as ps
 
 import gudhi
 import numpy as np
 import matplotlib.pyplot as plt
 
-def compute_simplicial_complex(X,ptype: str,max_dimension=2,p=1,m=0.1,is_plot=False):
+def compute_Rips_complex(X,DTM=False,max_dimension=2,p=1,m=0.1,is_plot=False):
   '''
-  compute_persistence takes a point cloud X and a ptype indicating whether the
-  type of simplicial complex computed is Rips complex, Alpha complex or DTM filtrations, 
-  and returns the computed simplicial complex of X. If is_plot is true, it also plots
-  its persistence diagram.
+  compute_Rips_complex takes a point cloud X and DTM indicating whether DTM filtrations
+  are used in the computation, and returns the computed simplicial complex of X. 
+  If is_plot is true, it also plots its persistence diagram.
 
   The extra parameter max_dimension can be specified for Rips complex and DTM
   filtrations; and for the case of DTM filtrations, the additional parameters 
   p and m can be specified.
   '''
 
   # create a complex
-  if ptype == 'Rips':
-    st = gudhi.RipsComplex(points=X).create_simplex_tree(max_dimension)
-  elif ptype == 'Alpha':
-    st = gudhi.AlphaComplex(points=X).create_simplex_tree()
-  elif ptype == 'DTM':
+  if DTM:
     st = dtm.DTMFiltration(X, m, p, max_dimension)
   else:
-    raise ValueError('ptype is not one of Rips, Alpha or DTM.')
+    st = gudhi.RipsComplex(points=X).create_simplex_tree(max_dimension)
 
   # compute the persistence
   diagram = st.persistence()                                       
 
   # plot the persistence diagram
   if is_plot:
     gudhi.plot_persistence_diagram(diagram)
-    if ptype == 'Rips':                    
-      title = 'Persistence diagram of the Rips complex'
-    elif ptype == 'Alpha':
-      title = 'Persistence diagram of the Alpha complex'
-    elif ptype == 'DTM':
+    if DTM:
       title = 'Persistence diagram of the DTM-filtration with parameter p ='+str(p)
     else:
-      raise ValueError('ptype is not one of Rips, Alpha or DTM.')
+      title = 'Persistence diagram of the Rips complex'
     plt.title(title);
 
   return st
 
 
-def bottleneck_distance(X, ptype1, ptype2, dim):
+def compute_Alpha_complex(X,DTM=False,max_dimension=3,p=1,m=0.05,is_plot=False):
   '''
-  bottleneck_distance takes a point cloud X and computes
-  the bottleneck distance between persistence diagram of
-  type ptype1 and the one of ptype2 in dimension dim.
+  compute_Alpha_complex takes a point cloud X and DTM indicating whether DTM filtrations
+  are used in the computation, and returns the computed simplicial complex of X. 
+  If is_plot is true, it also plots its persistence diagram.
+
+  The extra parameter max_dimension, p and m can be specified for DTM filtrations.
   '''
 
-  st1 = compute_simplicial_complex(X, ptype=ptype1)
-  st2 = compute_simplicial_complex(X, ptype=ptype2)
+  # create a complex
+  if DTM:
+    st = dtm.AlphaDTMFiltration(X, m, p, max_dimension)
+  else:
+    st = gudhi.AlphaComplex(points=X).create_simplex_tree()
+
+  # compute the persistence
+  diagram = st.persistence()                                       
+
+  # plot the persistence diagram
+  if is_plot:
+    gudhi.plot_persistence_diagram(diagram)
+    if DTM:
+      title = 'Persistence diagram of the Alpha-DTM-filtration with parameter p ='+str(p)
+    else:
+      title = 'Persistence diagram of the Alpha complex'
+    plt.title(title);
+
+  return st
+
+
+def bottleneck_distance(st1, st2, dim):
+  '''
+  bottleneck_distance takes SimplexTree st1 and st2 and computes
+  the bottleneck distance of their persistence diagram in dimension dim.
+  '''
   
   diag1 = st1.persistence_intervals_in_dimension(dim)
   diag2 = st2.persistence_intervals_in_dimension(dim)
 
   distance = gudhi.bottleneck_distance(diag1, diag2)
 
   message = "Bottleneck distance approximation = " + '%.2f' % gudhi.bottleneck_distance(diag1, diag2, 0.1)
@@ -83,63 +100,56 @@
   band is considered 'topological signal'.
 
   The desired confidence level can be specified using
   the parameter level.
   '''
 
   hatc = ps.hausd_interval(data=X, level=level)
-  st = compute_simplicial_complex(X,ptype)
   if ptype == 'Rips':
+    st = compute_Rips_complex(X)
     diagram = st.persistence()
   elif ptype == 'Alpha':
+    st = compute_Alpha_complex(X)
     st_list = st.get_filtration()
     for splx in st_list:
       st.assign_filtration(splx[0],filtration= np.sqrt(splx[1])) 
     diagram = st.persistence()
   else:
     raise ValueError('ptype is not either Rips or Alpha.')
   
   gudhi.plot_persistence_diagram(diagram,band=2*hatc);
 
 
-def connected_components(X, ptype: str):
+def connected_components(st):
   '''
-  connected_components takes a point cloud X and ptype
-  indicating the type of persistence computed, and
+  connected_components takes a SimplexTree st and
   return the number of connected components of X.
   '''
 
-  st = compute_simplicial_complex(X, ptype=ptype)
   return st.betti_numbers()[0]
 
 
-def one_dimensional_holes(X, ptype: str):
+def one_dimensional_holes(st):
   '''
-  one_dimensional_holes takes a point cloud X and ptype 
-  indicating the type of persistence computed, and
+  one_dimensional_holes takes a SimplexTree st and
   return the number of one dimensional holes of X.
   '''
 
-  st = compute_simplicial_complex(X, ptype=ptype)
   return st.betti_numbers()[1]
 
 
-def two_dimensional_holes(X, ptype: str):
+def two_dimensional_holes(st):
   '''
-  one_dimensional_holes takes a point cloud X and ptype 
-  indicating the type of persistence computed, and
+  one_dimensional_holes takes a SimplexTree st and
   return the number of one dimensional holes of X.
   '''
 
-  st = compute_simplicial_complex(X, ptype=ptype)
   return st.betti_numbers()[2]
 
 
-def holes(X, ptype: str, dim: int):
+def holes(st, dim: int):
   '''
-  holes takes a point cloud X and ptype indicating 
-  the type of persistence computed, and return the 
-  number of holes of X in dimension dim.
+  holes takes a SimplexTree st and return 
+  the number of holes of X in dimension dim.
   '''
 
-  st = compute_simplicial_complex(X, ptype=ptype)
   return st.betti_numbers()[dim]
```

### Comparing `spPersist-0.2.9/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.3.0/src/spPersist.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.9
+Version: 0.3.0
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
@@ -16,10 +16,18 @@
 spatial topology. The specific mathematical foundation for the classification is
 the theory of Persistent Homology and its homology barcodes. The package so far
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
-It is intended that the package will also include a pre-processing module, a 
+The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
 named pp, ph and hc.
+
+The persistent homology module contains functions for computing simplicial 
+complexes of point clouds (See data structures in the gudhi package.) and their
+topological measures. It also includes plotting features of the persistence 
+diagram.
+
+The homological classification module computes the number of holes and connected
+components as a dictionary.
```

