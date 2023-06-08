# Comparing `tmp/poetry_python_version-0.0.2.tar.gz` & `tmp/poetry_python_version-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_python_version-0.0.2.tar", max compression
+gzip compressed data, was "poetry_python_version-0.0.3.tar", max compression
```

## Comparing `poetry_python_version-0.0.2.tar` & `poetry_python_version-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1055 2023-06-08 12:55:38.354863 poetry_python_version-0.0.2/LICENSE
--rw-r--r--   0        0        0        0 2023-06-08 11:10:06.901265 poetry_python_version-0.0.2/README.md
--rw-r--r--   0        0        0     1482 2023-06-08 13:22:28.211958 poetry_python_version-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      170 2023-06-08 13:01:40.363685 poetry_python_version-0.0.2/src/poetry_python_version/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-08 13:29:20.830896 poetry_python_version-0.0.2/src/poetry_python_version/plugins.py
--rw-r--r--   0        0        0      802 1970-01-01 00:00:00.000000 poetry_python_version-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-08 14:26:32.456048 poetry_python_version-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1138 2023-06-08 14:26:32.456048 poetry_python_version-0.0.3/README.md
+-rw-r--r--   0        0        0     1482 2023-06-08 14:26:32.456048 poetry_python_version-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-06-08 14:26:32.456048 poetry_python_version-0.0.3/src/poetry_python_version/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-08 14:26:32.456048 poetry_python_version-0.0.3/src/poetry_python_version/plugins.py
+-rw-r--r--   0        0        0     1940 1970-01-01 00:00:00.000000 poetry_python_version-0.0.3/PKG-INFO
```

### Comparing `poetry_python_version-0.0.2/LICENSE` & `poetry_python_version-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_python_version-0.0.2/pyproject.toml` & `poetry_python_version-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-python-version"
-version = "0.0.2"
+version = "0.0.3"
 authors = ["Jiri Kuncar <jiri.kuncar@gmail.com>"]
 description = "Poetry plugin to read Python version from .python-version file"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jirikuncar/poetry-python-version"
 repository = "https://github.com/jirikuncar/poetry-python-version"
 packages = [{include = "poetry_python_version", from = "src"}]
```

### Comparing `poetry_python_version-0.0.2/src/poetry_python_version/plugins.py` & `poetry_python_version-0.0.3/src/poetry_python_version/plugins.py`

 * *Files identical despite different names*

