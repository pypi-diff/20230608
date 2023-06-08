# Comparing `tmp/spPersist-0.2.7.tar.gz` & `tmp/spPersist-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.2.7.tar", last modified: Thu Jun  8 00:07:46 2023, max compression
+gzip compressed data, was "spPersist-0.2.8.tar", last modified: Thu Jun  8 00:19:51 2023, max compression
```

## Comparing `spPersist-0.2.7.tar` & `spPersist-0.2.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.740551 spPersist-0.2.7/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 23:31:47.000000 spPersist-0.2.7/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:07:46.740551 spPersist-0.2.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 23:31:47.000000 spPersist-0.2.7/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:07:46.740551 spPersist-0.2.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 00:07:32.000000 spPersist-0.2.7/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.737551 spPersist-0.2.7/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.739551 spPersist-0.2.7/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:00:39.000000 spPersist-0.2.7/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:30:58.000000 spPersist-0.2.7/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 23:30:58.000000 spPersist-0.2.7/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 00:00:39.000000 spPersist-0.2.7/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     3954 2023-06-08 00:07:10.000000 spPersist-0.2.7/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:07:46.739551 spPersist-0.2.7/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 00:07:46.000000 spPersist-0.2.7/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:51.344529 spPersist-0.2.8/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-07 23:31:47.000000 spPersist-0.2.8/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:19:51.343529 spPersist-0.2.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      761 2023-06-07 23:31:47.000000 spPersist-0.2.8/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 00:19:51.344529 spPersist-0.2.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 00:19:24.000000 spPersist-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:51.341529 spPersist-0.2.8/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:51.342529 spPersist-0.2.8/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 00:00:39.000000 spPersist-0.2.8/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-07 23:30:58.000000 spPersist-0.2.8/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-07 23:30:58.000000 spPersist-0.2.8/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 00:00:39.000000 spPersist-0.2.8/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4530 2023-06-08 00:18:56.000000 spPersist-0.2.8/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 00:19:51.343529 spPersist-0.2.8/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1133 2023-06-08 00:19:51.000000 spPersist-0.2.8/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      349 2023-06-08 00:19:51.000000 spPersist-0.2.8/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 00:19:51.000000 spPersist-0.2.8/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 00:19:51.000000 spPersist-0.2.8/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 00:19:51.000000 spPersist-0.2.8/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.2.7/LICENSE` & `spPersist-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.7/PKG-INFO` & `spPersist-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.7
+Version: 0.2.8
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `spPersist-0.2.7/README.md` & `spPersist-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.7/setup.py` & `spPersist-0.2.8/setup.py`

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
-    version="0.2.7",  # Required
+    version="0.2.8",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `spPersist-0.2.7/src/spPersist/DTM_filtrations.py` & `spPersist-0.2.8/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.7/src/spPersist/dp.py` & `spPersist-0.2.8/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.7/src/spPersist/persistence_statistics.py` & `spPersist-0.2.8/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.2.7/src/spPersist/ph.py` & `spPersist-0.2.8/src/spPersist/ph.py`

 * *Files 7% similar despite different names*

```diff
@@ -116,8 +116,30 @@
   '''
   one_dimensional_holes takes a point cloud X and ptype 
   indicating the type of persistence computed, and
   return the number of one dimensional holes of X.
   '''
 
   st = compute_simplicial_complex(X, ptype=ptype)
-  return st.betti_numbers()[1]
+  return st.betti_numbers()[1]
+
+
+def two_dimensional_holes(X, ptype: str):
+  '''
+  one_dimensional_holes takes a point cloud X and ptype 
+  indicating the type of persistence computed, and
+  return the number of one dimensional holes of X.
+  '''
+
+  st = compute_simplicial_complex(X, ptype=ptype)
+  return st.betti_numbers()[2]
+
+
+def holes(X, ptype: str, dim: int):
+  '''
+  holes takes a point cloud X and ptype indicating 
+  the type of persistence computed, and return the 
+  number of holes of X in dimension dim.
+  '''
+
+  st = compute_simplicial_complex(X, ptype=ptype)
+  return st.betti_numbers()[dim]
```

### Comparing `spPersist-0.2.7/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.2.8/src/spPersist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.2.7
+Version: 0.2.8
 Summary: Spatial transcriptomics with Persistent Homology
 Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
 Keywords: spatial transcriptomics,persistent homology,single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

