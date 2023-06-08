# Comparing `tmp/pysaltcorn-0.2.0.tar.gz` & `tmp/pysaltcorn-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pysaltcorn-0.2.0.tar", max compression
+gzip compressed data, was "pysaltcorn-0.3.0.tar", max compression
```

## Comparing `pysaltcorn-0.2.0.tar` & `pysaltcorn-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      858 2023-02-28 13:42:14.594312 pysaltcorn-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     5621 2023-02-28 13:44:00.617553 pysaltcorn-0.2.0/pysaltcorn/__init__.py
--rw-r--r--   0        0        0        0 2022-11-28 14:00:07.341449 pysaltcorn-0.2.0/pysaltcorn/py.typed
--rw-r--r--   0        0        0      624 2023-02-28 13:50:59.525473 pysaltcorn-0.2.0/setup.py
--rw-r--r--   0        0        0      384 2023-02-28 13:50:59.525626 pysaltcorn-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      757 2023-06-08 12:28:19.116406 pysaltcorn-0.3.0/README.md
+-rw-r--r--   0        0        0      905 2023-06-08 12:39:17.940594 pysaltcorn-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0    19182 2023-06-08 12:34:53.732452 pysaltcorn-0.3.0/pysaltcorn/__init__.py
+-rw-r--r--   0        0        0        0 2022-11-28 14:00:07.341449 pysaltcorn-0.3.0/pysaltcorn/py.typed
+-rw-r--r--   0        0        0      620 2023-06-06 14:39:05.380571 pysaltcorn-0.3.0/pysaltcorn/support.py
+-rw-r--r--   0        0        0     1446 2023-06-08 12:39:39.957601 pysaltcorn-0.3.0/setup.py
+-rw-r--r--   0        0        0     1183 2023-06-08 12:39:39.957746 pysaltcorn-0.3.0/PKG-INFO
```

### Comparing `pysaltcorn-0.2.0/pyproject.toml` & `pysaltcorn-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 [tool.poetry]
 name = "pysaltcorn"
-version = "0.2.0"
+version = "0.3.0"
 description = "Python library for Saltcorn API"
 authors = ["Michael Dubner <pywebmail@list.ru>"]
 license = "MIT"
+readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.1"
 
 [tool.poetry.dev-dependencies]
 flake8 = "^6.0.0"
 twine = "^4.0.1"
 mypy = "^0.991"
 types-requests = "^2.28.11"
 bumpver = "^2022.1119"
 black = "^23.1.0"
 isort = "^5.12.0"
+types-Werkzeug = "^1.0.9"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.bumpver]
-current_version = "0.2.0"
+current_version = "0.3.0"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

