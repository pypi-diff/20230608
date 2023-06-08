# Comparing `tmp/terraply-0.0.1.tar.gz` & `tmp/terraply-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terraply-0.0.1.tar", last modified: Thu Jun  1 02:24:54 2023, max compression
+gzip compressed data, was "terraply-0.0.2.tar", last modified: Thu Jun  8 18:53:12 2023, max compression
```

## Comparing `terraply-0.0.1.tar` & `terraply-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 joshuaadkins   (501) staff       (20)        0 2023-06-01 02:24:54.965335 terraply-0.0.1/
--rw-r--r--   0 joshuaadkins   (501) staff       (20)     1062 2023-05-31 22:58:13.000000 terraply-0.0.1/LICENSE
--rw-r--r--   0 joshuaadkins   (501) staff       (20)      784 2023-06-01 02:24:54.965214 terraply-0.0.1/PKG-INFO
--rw-r--r--   0 joshuaadkins   (501) staff       (20)      383 2023-05-31 23:09:25.000000 terraply-0.0.1/README.md
--rw-r--r--   0 joshuaadkins   (501) staff       (20)      534 2023-05-31 23:28:10.000000 terraply-0.0.1/pyproject.toml
--rw-r--r--   0 joshuaadkins   (501) staff       (20)       38 2023-06-01 02:24:54.965372 terraply-0.0.1/setup.cfg
-drwxr-xr-x   0 joshuaadkins   (501) staff       (20)        0 2023-06-01 02:24:54.964423 terraply-0.0.1/terraply/
--rw-r--r--   0 joshuaadkins   (501) staff       (20)       49 2023-05-31 23:27:56.000000 terraply-0.0.1/terraply/__init__.py
--rw-r--r--   0 joshuaadkins   (501) staff       (20)     3202 2023-06-01 02:19:48.000000 terraply-0.0.1/terraply/terraply.py
-drwxr-xr-x   0 joshuaadkins   (501) staff       (20)        0 2023-06-01 02:24:54.965077 terraply-0.0.1/terraply.egg-info/
--rw-r--r--   0 joshuaadkins   (501) staff       (20)      784 2023-06-01 02:24:54.000000 terraply-0.0.1/terraply.egg-info/PKG-INFO
--rw-r--r--   0 joshuaadkins   (501) staff       (20)      237 2023-06-01 02:24:54.000000 terraply-0.0.1/terraply.egg-info/SOURCES.txt
--rw-r--r--   0 joshuaadkins   (501) staff       (20)        1 2023-06-01 02:24:54.000000 terraply-0.0.1/terraply.egg-info/dependency_links.txt
--rw-r--r--   0 joshuaadkins   (501) staff       (20)       43 2023-06-01 02:24:54.000000 terraply-0.0.1/terraply.egg-info/entry_points.txt
--rw-r--r--   0 joshuaadkins   (501) staff       (20)        9 2023-06-01 02:24:54.000000 terraply-0.0.1/terraply.egg-info/top_level.txt
+drwxr-xr-x   0 joshuaadkins   (501) staff       (20)        0 2023-06-08 18:53:12.291583 terraply-0.0.2/
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)     1062 2023-05-31 22:58:13.000000 terraply-0.0.2/LICENSE
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)      784 2023-06-08 18:53:12.291433 terraply-0.0.2/PKG-INFO
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)      383 2023-05-31 23:09:25.000000 terraply-0.0.2/README.md
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)      534 2023-06-08 18:52:19.000000 terraply-0.0.2/pyproject.toml
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)       38 2023-06-08 18:53:12.291622 terraply-0.0.2/setup.cfg
+drwxr-xr-x   0 joshuaadkins   (501) staff       (20)        0 2023-06-08 18:53:12.290465 terraply-0.0.2/terraply/
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)       49 2023-05-31 23:27:56.000000 terraply-0.0.2/terraply/__init__.py
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)     4680 2023-06-08 18:52:03.000000 terraply-0.0.2/terraply/terraply.py
+drwxr-xr-x   0 joshuaadkins   (501) staff       (20)        0 2023-06-08 18:53:12.291178 terraply-0.0.2/terraply.egg-info/
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)      784 2023-06-08 18:53:12.000000 terraply-0.0.2/terraply.egg-info/PKG-INFO
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)      237 2023-06-08 18:53:12.000000 terraply-0.0.2/terraply.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)        1 2023-06-08 18:53:12.000000 terraply-0.0.2/terraply.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)       43 2023-06-08 18:53:12.000000 terraply-0.0.2/terraply.egg-info/entry_points.txt
+-rw-r--r--   0 joshuaadkins   (501) staff       (20)        9 2023-06-08 18:53:12.000000 terraply-0.0.2/terraply.egg-info/top_level.txt
```

### Comparing `terraply-0.0.1/LICENSE` & `terraply-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `terraply-0.0.1/PKG-INFO` & `terraply-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraply
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wrapper to expand and exclude targets in terraform.
 Author-email: Joshua Adkins <josh@nline.io>
 Project-URL: Homepage, https://github.com/nline/terraply
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `terraply-0.0.1/pyproject.toml` & `terraply-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 terraply = "terraply:main"
 
 [project]
 name = "terraply"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Joshua Adkins", email="josh@nline.io" },
 ]
 description = "A wrapper to expand and exclude targets in terraform."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `terraply-0.0.1/terraply.egg-info/PKG-INFO` & `terraply-0.0.2/terraply.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terraply
-Version: 0.0.1
+Version: 0.0.2
 Summary: A wrapper to expand and exclude targets in terraform.
 Author-email: Joshua Adkins <josh@nline.io>
 Project-URL: Homepage, https://github.com/nline/terraply
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

