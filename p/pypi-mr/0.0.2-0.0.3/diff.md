# Comparing `tmp/pypi-mr-0.0.2.tar.gz` & `tmp/pypi-mr-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypi-mr-0.0.2.tar", last modified: Thu Jun  8 09:21:13 2023, max compression
+gzip compressed data, was "pypi-mr-0.0.3.tar", last modified: Thu Jun  8 10:10:55 2023, max compression
```

## Comparing `pypi-mr-0.0.2.tar` & `pypi-mr-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:21:13.249050 pypi-mr-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 09:21:13.249050 pypi-mr-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 09:20:58.000000 pypi-mr-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:21:13.249050 pypi-mr-0.0.2/pypi_mr/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 09:20:58.000000 pypi-mr-0.0.2/pypi_mr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-08 09:20:58.000000 pypi-mr-0.0.2/pypi_mr/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-08 09:20:58.000000 pypi-mr-0.0.2/pypi_mr/exists.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 09:20:58.000000 pypi-mr-0.0.2/pypi_mr/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:21:13.249050 pypi-mr-0.0.2/pypi_mr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 09:21:13.000000 pypi-mr-0.0.2/pypi_mr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 09:21:13.000000 pypi-mr-0.0.2/pypi_mr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:21:13.000000 pypi-mr-0.0.2/pypi_mr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 09:21:13.000000 pypi-mr-0.0.2/pypi_mr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 09:21:13.000000 pypi-mr-0.0.2/pypi_mr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-06-08 09:20:58.000000 pypi-mr-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 09:21:13.249050 pypi-mr-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:10:55.215770 pypi-mr-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 10:10:55.215770 pypi-mr-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-08 10:10:37.000000 pypi-mr-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:10:55.215770 pypi-mr-0.0.3/pypi_mr/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 10:10:37.000000 pypi-mr-0.0.3/pypi_mr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-06-08 10:10:37.000000 pypi-mr-0.0.3/pypi_mr/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-08 10:10:37.000000 pypi-mr-0.0.3/pypi_mr/exists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-08 10:10:37.000000 pypi-mr-0.0.3/pypi_mr/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:10:55.215770 pypi-mr-0.0.3/pypi_mr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 10:10:55.000000 pypi-mr-0.0.3/pypi_mr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-06-08 10:10:55.000000 pypi-mr-0.0.3/pypi_mr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:10:55.000000 pypi-mr-0.0.3/pypi_mr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 10:10:55.000000 pypi-mr-0.0.3/pypi_mr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 10:10:55.000000 pypi-mr-0.0.3/pypi_mr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3205 2023-06-08 10:10:37.000000 pypi-mr-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:10:55.215770 pypi-mr-0.0.3/setup.cfg
```

### Comparing `pypi-mr-0.0.2/PKG-INFO` & `pypi-mr-0.0.3/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-mr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Check if package exists on pypi registry using simple API. Clean packages that belongs to closed/merged GitLab MRs
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/pypi-mr
 Project-URL: docs, https://tandav.github.io/pypi-mr/
 Project-URL: issues, https://github.com/tandav/pypi-mr/issues
 Project-URL: release notes, https://github.com/tandav/pypi-mr/releases
 Requires-Python: >=3.9
```

### Comparing `pypi-mr-0.0.2/pypi_mr/cleanup.py` & `pypi-mr-0.0.3/pypi_mr/cleanup.py`

 * *Files identical despite different names*

### Comparing `pypi-mr-0.0.2/pypi_mr/exists.py` & `pypi-mr-0.0.3/pypi_mr/exists.py`

 * *Files identical despite different names*

### Comparing `pypi-mr-0.0.2/pypi_mr.egg-info/PKG-INFO` & `pypi-mr-0.0.3/pypi_mr.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypi-mr
-Version: 0.0.2
+Version: 0.0.3
 Summary: Check if package exists on pypi registry using simple API. Clean packages that belongs to closed/merged GitLab MRs
 Author-email: Alexander Rodionov <tandav@tandav.me>
 Project-URL: source, https://github.com/tandav/pypi-mr
 Project-URL: docs, https://tandav.github.io/pypi-mr/
 Project-URL: issues, https://github.com/tandav/pypi-mr/issues
 Project-URL: release notes, https://github.com/tandav/pypi-mr/releases
 Requires-Python: >=3.9
```

### Comparing `pypi-mr-0.0.2/pyproject.toml` & `pypi-mr-0.0.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [project]
 name = "pypi-mr"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     {name = "Alexander Rodionov", email = "tandav@tandav.me"},
 ]
 description = "Check if package exists on pypi registry using simple API. Clean packages that belongs to closed/merged GitLab MRs"
 readme = "README.md"
 requires-python = ">=3.9"
 dependencies = [
     "requests",
+    "packaging",
 ]
 
 [project.optional-dependencies]
 dev = [
     "bumpver",
     "pre-commit",
     "pytest",
@@ -29,15 +30,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 # ==============================================================================
 
 [bumpver]
-current_version = "v0.0.2"
+current_version = "v0.0.3"
 version_pattern = "vMAJOR.MINOR.PATCH[GITHASH]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
```

