# Comparing `tmp/schemander-0.0.2.tar.gz` & `tmp/schemander-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schemander-0.0.2.tar", last modified: Fri Jun  2 02:24:55 2023, max compression
+gzip compressed data, was "schemander-0.0.3.tar", last modified: Wed Jun  7 22:23:22 2023, max compression
```

## Comparing `schemander-0.0.2.tar` & `schemander-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:24:55.479877 schemander-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-02 02:24:22.000000 schemander-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-02 02:24:55.479877 schemander-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-02 02:24:22.000000 schemander-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-02 02:24:22.000000 schemander-0.0.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 02:24:55.479877 schemander-0.0.2/schemander.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-02 02:24:55.000000 schemander-0.0.2/schemander.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-02 02:24:55.000000 schemander-0.0.2/schemander.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:24:55.000000 schemander-0.0.2/schemander.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-02 02:24:55.000000 schemander-0.0.2/schemander.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 02:24:55.000000 schemander-0.0.2/schemander.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 02:24:55.479877 schemander-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:22.509270 schemander-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-06-07 22:22:50.000000 schemander-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-07 22:23:22.509270 schemander-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-06-07 22:22:50.000000 schemander-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-07 22:22:50.000000 schemander-0.0.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 22:23:22.509270 schemander-0.0.3/schemander.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-07 22:23:22.000000 schemander-0.0.3/schemander.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    12965 2023-06-07 22:22:50.000000 schemander-0.0.3/schemander.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 22:23:22.509270 schemander-0.0.3/setup.cfg
```

### Comparing `schemander-0.0.2/LICENSE` & `schemander-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `schemander-0.0.2/PKG-INFO` & `schemander-0.0.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.2
+Version: 0.0.3
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `schemander-0.0.2/README.md` & `schemander-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `schemander-0.0.2/pyproject.toml` & `schemander-0.0.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [project]
-version = "0.0.2"
+version = "0.0.3"
 name = "schemander"
 authors = [
     { name="Miguel Alejandro Salgado Zapien", email="ekiim@ekiim.xyz"},
 ]
 description = "A single file schema validator for dictionaries."
 readme="README.md"
 requires-python = ">= 3.11"
@@ -39,17 +39,16 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools]
 license-files = ["LICENSE"]
+py-modules = ["schemander"]
 
-[tool.setuptools.packages.find]
-include = ["schemander"]
 
 [tool.pytest.ini_options]
 addopts = "-q --doctest-modules --cov=schemander --cov-report=term-missing"
 testpaths = ["tests"]
 
 [tool.pytest.plugins]
 cov = {source = "schemander"}
```

### Comparing `schemander-0.0.2/schemander.egg-info/PKG-INFO` & `schemander-0.0.3/schemander.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schemander
-Version: 0.0.2
+Version: 0.0.3
 Summary: A single file schema validator for dictionaries.
 Author-email: Miguel Alejandro Salgado Zapien <ekiim@ekiim.xyz>
 License: GPL-2.0
 Project-URL: Homepage, https://schemander.ekiim.xyz
 Project-URL: Source, https://github.com/ekiim/schemander
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

