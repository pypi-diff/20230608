# Comparing `tmp/spPersist-0.3.1.tar.gz` & `tmp/spPersist-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.3.1.tar", last modified: Thu Jun  8 03:20:42 2023, max compression
+gzip compressed data, was "spPersist-0.3.2.tar", last modified: Thu Jun  8 09:17:06 2023, max compression
```

## Comparing `spPersist-0.3.1.tar` & `spPersist-0.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.137033 spPersist-0.3.1/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 02:50:48.000000 spPersist-0.3.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:20:42.137033 spPersist-0.3.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1098 2023-06-08 02:50:48.000000 spPersist-0.3.1/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 03:20:42.137033 spPersist-0.3.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 03:19:53.000000 spPersist-0.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.134033 spPersist-0.3.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.136033 spPersist-0.3.1/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 02:50:15.000000 spPersist-0.3.1/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 03:05:07.000000 spPersist-0.3.1/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 02:50:14.000000 spPersist-0.3.1/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 03:18:30.000000 spPersist-0.3.1/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 02:50:15.000000 spPersist-0.3.1/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-08 03:19:09.000000 spPersist-0.3.1/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 03:20:42.137033 spPersist-0.3.1/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1462 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 03:20:42.000000 spPersist-0.3.1/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.085866 spPersist-0.3.2/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 09:16:42.000000 spPersist-0.3.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-06-08 09:17:06.085866 spPersist-0.3.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-06-08 09:16:42.000000 spPersist-0.3.2/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 09:17:06.085866 spPersist-0.3.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8113 2023-06-08 09:16:42.000000 spPersist-0.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.083866 spPersist-0.3.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.084866 spPersist-0.3.2/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 09:14:01.000000 spPersist-0.3.2/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 09:14:02.000000 spPersist-0.3.2/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 09:14:02.000000 spPersist-0.3.2/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 09:14:01.000000 spPersist-0.3.2/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 09:14:02.000000 spPersist-0.3.2/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-08 09:14:01.000000 spPersist-0.3.2/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.085866 spPersist-0.3.2/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1411 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.3.1/LICENSE` & `spPersist-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.1/PKG-INFO` & `spPersist-0.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.1
+Version: 0.3.2
 Summary: Spatial transcriptomics with Persistent Homology
-Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
-Keywords: spatial transcriptomics,persistent homology,single-cell analysis
+Keywords: Spatial transcriptomics,Persistent homology,Single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Spatial Transcriptomics with Persistent Homology
+# Spatial transcriptomics with Persistent Homology
 
-This is a package for classifying Spatial Transcriptomics data according to its 
+This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and its homology barcodes. The package so far
+the theory of Persistent Homology and persistence diagram. The package so far
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
```

### Comparing `spPersist-0.3.1/README.md` & `spPersist-0.3.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Spatial Transcriptomics with Persistent Homology
+# Spatial transcriptomics with Persistent Homology
 
-This is a package for classifying Spatial Transcriptomics data according to its 
+This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and its homology barcodes. The package so far
+the theory of Persistent Homology and persistence diagram. The package so far
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
```

### Comparing `spPersist-0.3.1/setup.py` & `spPersist-0.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     name="spPersist",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version="0.3.1",  # Required
+    version="0.3.2",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -61,15 +61,15 @@
     # This field corresponds to the "Description-Content-Type" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#description-content-type-optional
     long_description_content_type="text/markdown",  # Optional (see note above)
     # This should be a valid link to your project's main homepage.
     #
     # This field corresponds to the "Home-Page" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#home-page-optional
-    url="https://github.com/pypa/sampleproject",  # Optional
+    # url="https://github.com/pypa/sampleproject",  # Optional
     # This should be your name or the name of the organization which owns the
     # project.
     author="Lirong Yang",  # Optional
     # This should be a valid email address corresponding to the author listed
     # above.
     author_email="lirong.yang@outlook.com",  # Optional
     # Classifiers help users find your project by categorizing it.
@@ -98,15 +98,15 @@
     # ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
-    keywords="spatial transcriptomics, persistent homology, single-cell analysis",  # Optional
+    keywords="Spatial transcriptomics, Persistent homology, Single-cell analysis",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
     package_dir={"": "src"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
```

### Comparing `spPersist-0.3.1/src/spPersist/DTM_filtrations.py` & `spPersist-0.3.2/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.1/src/spPersist/dp.py` & `spPersist-0.3.2/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.1/src/spPersist/hc.py` & `spPersist-0.3.2/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.1/src/spPersist/persistence_statistics.py` & `spPersist-0.3.2/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.1/src/spPersist/ph.py` & `spPersist-0.3.2/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.1/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.3.2/src/spPersist.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.1
+Version: 0.3.2
 Summary: Spatial transcriptomics with Persistent Homology
-Home-page: https://github.com/pypa/sampleproject
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
-Keywords: spatial transcriptomics,persistent homology,single-cell analysis
+Keywords: Spatial transcriptomics,Persistent homology,Single-cell analysis
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# Spatial Transcriptomics with Persistent Homology
+# Spatial transcriptomics with Persistent Homology
 
-This is a package for classifying Spatial Transcriptomics data according to its 
+This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
-the theory of Persistent Homology and its homology barcodes. The package so far
+the theory of Persistent Homology and persistence diagram. The package so far
 contains a data processing module, called dp, allowing users to load either the
 standard datasets from Visium and MERFISH, or published datasets into desired
 annotated data format for the analysis performed in this package. The format is
 compatible with the package Squidpy.
 
 The package also includes a pre-processing module, a 
 persistent homology module and a homological classification module, respectively
```

