# Comparing `tmp/CU_MkDocs_ab6459-0.0.2.tar.gz` & `tmp/CU_MkDocs_ab6459-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CU_MkDocs_ab6459-0.0.2.tar", last modified: Thu Jun  8 09:29:11 2023, max compression
+gzip compressed data, was "CU_MkDocs_ab6459-0.0.3.tar", last modified: Thu Jun  8 09:37:11 2023, max compression
```

## Comparing `CU_MkDocs_ab6459-0.0.2.tar` & `CU_MkDocs_ab6459-0.0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 09:29:11.719010 CU_MkDocs_ab6459-0.0.2/
-drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 09:29:11.719010 CU_MkDocs_ab6459-0.0.2/CU_MkDocs_ab6459.egg-info/
--rw-rw-r--   0 ian       (1000) ian       (1000)      569 2023-06-08 09:29:11.000000 CU_MkDocs_ab6459-0.0.2/CU_MkDocs_ab6459.egg-info/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)      184 2023-06-08 09:29:11.000000 CU_MkDocs_ab6459-0.0.2/CU_MkDocs_ab6459.egg-info/SOURCES.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 09:29:11.000000 CU_MkDocs_ab6459-0.0.2/CU_MkDocs_ab6459.egg-info/dependency_links.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 09:29:11.000000 CU_MkDocs_ab6459-0.0.2/CU_MkDocs_ab6459.egg-info/top_level.txt
--rw-rw-r--   0 ian       (1000) ian       (1000)      569 2023-06-08 09:29:11.719010 CU_MkDocs_ab6459-0.0.2/PKG-INFO
--rw-rw-r--   0 ian       (1000) ian       (1000)        0 2023-06-08 09:11:09.000000 CU_MkDocs_ab6459-0.0.2/README.md
--rw-rw-r--   0 ian       (1000) ian       (1000)      579 2023-06-08 09:29:07.000000 CU_MkDocs_ab6459-0.0.2/pyproject.toml
--rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-06-08 09:29:11.719010 CU_MkDocs_ab6459-0.0.2/setup.cfg
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 09:37:11.494464 CU_MkDocs_ab6459-0.0.3/
+drwxrwxr-x   0 ian       (1000) ian       (1000)        0 2023-06-08 09:37:11.494464 CU_MkDocs_ab6459-0.0.3/CU_MkDocs_ab6459.egg-info/
+-rw-rw-r--   0 ian       (1000) ian       (1000)      569 2023-06-08 09:37:11.000000 CU_MkDocs_ab6459-0.0.3/CU_MkDocs_ab6459.egg-info/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)      184 2023-06-08 09:37:11.000000 CU_MkDocs_ab6459-0.0.3/CU_MkDocs_ab6459.egg-info/SOURCES.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 09:37:11.000000 CU_MkDocs_ab6459-0.0.3/CU_MkDocs_ab6459.egg-info/dependency_links.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)        1 2023-06-08 09:37:11.000000 CU_MkDocs_ab6459-0.0.3/CU_MkDocs_ab6459.egg-info/top_level.txt
+-rw-rw-r--   0 ian       (1000) ian       (1000)      569 2023-06-08 09:37:11.494464 CU_MkDocs_ab6459-0.0.3/PKG-INFO
+-rw-rw-r--   0 ian       (1000) ian       (1000)        0 2023-06-08 09:11:09.000000 CU_MkDocs_ab6459-0.0.3/README.md
+-rw-rw-r--   0 ian       (1000) ian       (1000)      579 2023-06-08 09:35:32.000000 CU_MkDocs_ab6459-0.0.3/pyproject.toml
+-rw-rw-r--   0 ian       (1000) ian       (1000)       38 2023-06-08 09:37:11.494464 CU_MkDocs_ab6459-0.0.3/setup.cfg
```

### Comparing `CU_MkDocs_ab6459-0.0.2/CU_MkDocs_ab6459.egg-info/PKG-INFO` & `CU_MkDocs_ab6459-0.0.3/CU_MkDocs_ab6459.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CU-MkDocs-ab6459
-Version: 0.0.2
+Version: 0.0.3
 Summary: A MkDocs Theme for Coventry University modules delivered by Ian Cornelius.
 Author-email: Ian Cornelius <ab6459@coventry.ac.uk>
 Project-URL: Homepage, https://github.coventry.ac.uk/ab6459/CU_MkDocs_ab6459
 Project-URL: Bug Tracker, https://github.coventry.ac.uk/ab6459/CU_MkDocs_ab6459/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CU_MkDocs_ab6459-0.0.2/PKG-INFO` & `CU_MkDocs_ab6459-0.0.3/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CU_MkDocs_ab6459
-Version: 0.0.2
+Version: 0.0.3
 Summary: A MkDocs Theme for Coventry University modules delivered by Ian Cornelius.
 Author-email: Ian Cornelius <ab6459@coventry.ac.uk>
 Project-URL: Homepage, https://github.coventry.ac.uk/ab6459/CU_MkDocs_ab6459
 Project-URL: Bug Tracker, https://github.coventry.ac.uk/ab6459/CU_MkDocs_ab6459/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `CU_MkDocs_ab6459-0.0.2/pyproject.toml` & `CU_MkDocs_ab6459-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "CU_MkDocs_ab6459"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Ian Cornelius", email="ab6459@coventry.ac.uk" },
 ]
 description = "A MkDocs Theme for Coventry University modules delivered by Ian Cornelius."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

