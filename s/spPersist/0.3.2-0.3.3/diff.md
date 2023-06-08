# Comparing `tmp/spPersist-0.3.2.tar.gz` & `tmp/spPersist-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spPersist-0.3.2.tar", last modified: Thu Jun  8 09:17:06 2023, max compression
+gzip compressed data, was "spPersist-0.3.3.tar", last modified: Thu Jun  8 09:23:38 2023, max compression
```

## Comparing `spPersist-0.3.2.tar` & `spPersist-0.3.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.085866 spPersist-0.3.2/
--rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 09:16:42.000000 spPersist-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1411 2023-06-08 09:17:06.085866 spPersist-0.3.2/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1096 2023-06-08 09:16:42.000000 spPersist-0.3.2/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 09:17:06.085866 spPersist-0.3.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     8113 2023-06-08 09:16:42.000000 spPersist-0.3.2/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.083866 spPersist-0.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.084866 spPersist-0.3.2/src/spPersist/
--rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 09:14:01.000000 spPersist-0.3.2/src/spPersist/DTM_filtrations.py
--rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 09:14:02.000000 spPersist-0.3.2/src/spPersist/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 09:14:02.000000 spPersist-0.3.2/src/spPersist/dp.py
--rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 09:14:01.000000 spPersist-0.3.2/src/spPersist/hc.py
--rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 09:14:02.000000 spPersist-0.3.2/src/spPersist/persistence_statistics.py
--rw-r--r--   0 root         (0) root         (0)     4454 2023-06-08 09:14:01.000000 spPersist-0.3.2/src/spPersist/ph.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:17:06.085866 spPersist-0.3.2/src/spPersist.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1411 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 09:17:06.000000 spPersist-0.3.2/src/spPersist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.186333 spPersist-0.3.3/
+-rw-r--r--   0 root         (0) root         (0)     1091 2023-06-08 09:16:42.000000 spPersist-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 09:23:38.186333 spPersist-0.3.3/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1096 2023-06-08 09:16:42.000000 spPersist-0.3.3/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 09:23:38.187333 spPersist-0.3.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     8111 2023-06-08 09:22:44.000000 spPersist-0.3.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.183333 spPersist-0.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.185333 spPersist-0.3.3/src/spPersist/
+-rw-r--r--   0 root         (0) root         (0)    10798 2023-06-08 09:14:01.000000 spPersist-0.3.3/src/spPersist/DTM_filtrations.py
+-rw-r--r--   0 root         (0) root         (0)       50 2023-06-08 09:14:02.000000 spPersist-0.3.3/src/spPersist/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     9403 2023-06-08 09:14:02.000000 spPersist-0.3.3/src/spPersist/dp.py
+-rw-r--r--   0 root         (0) root         (0)      531 2023-06-08 09:14:01.000000 spPersist-0.3.3/src/spPersist/hc.py
+-rw-r--r--   0 root         (0) root         (0)     3287 2023-06-08 09:14:02.000000 spPersist-0.3.3/src/spPersist/persistence_statistics.py
+-rw-r--r--   0 root         (0) root         (0)     4454 2023-06-08 09:14:01.000000 spPersist-0.3.3/src/spPersist/ph.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:23:38.186333 spPersist-0.3.3/src/spPersist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1332 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      369 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-06-08 09:23:38.000000 spPersist-0.3.3/src/spPersist.egg-info/top_level.txt
```

### Comparing `spPersist-0.3.2/LICENSE` & `spPersist-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/PKG-INFO` & `spPersist-0.3.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.2
+Version: 0.3.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
-Keywords: Spatial transcriptomics,Persistent homology,Single-cell analysis
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
```

### Comparing `spPersist-0.3.2/README.md` & `spPersist-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/setup.py` & `spPersist-0.3.3/setup.py`

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
-    version="0.3.2",  # Required
+    version="0.3.3",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Spatial transcriptomics with Persistent Homology",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
@@ -98,15 +98,15 @@
     # ],
     # This field adds keywords for your project which will appear on the
     # project page. What does your project relate to?
     #
     # Note that this is a list of additional keywords, separated
     # by commas, to be used to assist searching for the distribution in a
     # larger catalog.
-    keywords="Spatial transcriptomics, Persistent homology, Single-cell analysis",  # Optional
+    # keywords="Spatial transcriptomics, Persistent homology, Single-cell analysis",  # Optional
     # When your source code is in a subdirectory under the project root, e.g.
     # `src/`, it is necessary to specify the `package_dir` argument.
     package_dir={"": "src"},  # Optional
     # You can just specify package directories manually here if your project is
     # simple. Or you can use find_packages().
     #
     # Alternatively, if you just want to distribute a single Python file, use
@@ -116,15 +116,15 @@
     #   py_modules=["my_module"],
     #
     packages=find_packages(where="src"),  # Required
     # Specify which Python versions you support. In contrast to the
     # 'Programming Language' classifiers above, 'pip install' will check this
     # and refuse to install the project if the version does not match. See
     # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
-    python_requires=">=3.7, <4",
+    python_requires=">=3.7",
     # This field lists other packages that your project depends on to run.
     # Any package you put here will be installed by pip when your project is
     # installed, so they must be valid existing projects.
     #
     # For an analysis of "install_requires" vs pip's requirements files see:
     # https://packaging.python.org/discussions/install-requires-vs-requirements/
     install_requires=[
```

### Comparing `spPersist-0.3.2/src/spPersist/DTM_filtrations.py` & `spPersist-0.3.3/src/spPersist/DTM_filtrations.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/src/spPersist/dp.py` & `spPersist-0.3.3/src/spPersist/dp.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/src/spPersist/hc.py` & `spPersist-0.3.3/src/spPersist/hc.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/src/spPersist/persistence_statistics.py` & `spPersist-0.3.3/src/spPersist/persistence_statistics.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/src/spPersist/ph.py` & `spPersist-0.3.3/src/spPersist/ph.py`

 * *Files identical despite different names*

### Comparing `spPersist-0.3.2/src/spPersist.egg-info/PKG-INFO` & `spPersist-0.3.3/src/spPersist.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 Metadata-Version: 2.1
 Name: spPersist
-Version: 0.3.2
+Version: 0.3.3
 Summary: Spatial transcriptomics with Persistent Homology
 Author: Lirong Yang
 Author-email: lirong.yang@outlook.com
-Keywords: Spatial transcriptomics,Persistent homology,Single-cell analysis
-Requires-Python: >=3.7, <4
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Spatial transcriptomics with Persistent Homology
 
 This is a package for classifying Spatial transcriptomics data according to its 
 spatial topology. The specific mathematical foundation for the classification is
```

