# Comparing `tmp/poetry_python_version-0.0.4.tar.gz` & `tmp/poetry_python_version-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "poetry_python_version-0.0.4.tar", max compression
+gzip compressed data, was "poetry_python_version-0.0.5.tar", max compression
```

## Comparing `poetry_python_version-0.0.4.tar` & `poetry_python_version-0.0.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1055 2023-06-08 14:37:00.044013 poetry_python_version-0.0.4/LICENSE
--rw-r--r--   0        0        0     1138 2023-06-08 14:37:00.044013 poetry_python_version-0.0.4/README.md
--rw-r--r--   0        0        0     1466 2023-06-08 14:37:00.044013 poetry_python_version-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      170 2023-06-08 14:37:00.044013 poetry_python_version-0.0.4/src/poetry_python_version/__init__.py
--rw-r--r--   0        0        0     1223 2023-06-08 14:37:00.044013 poetry_python_version-0.0.4/src/poetry_python_version/plugins.py
--rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 poetry_python_version-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1055 2023-06-08 14:53:36.119554 poetry_python_version-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1138 2023-06-08 14:53:36.119554 poetry_python_version-0.0.5/README.md
+-rw-r--r--   0        0        0     1466 2023-06-08 14:53:36.119554 poetry_python_version-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      170 2023-06-08 14:53:36.119554 poetry_python_version-0.0.5/src/poetry_python_version/__init__.py
+-rw-r--r--   0        0        0     1223 2023-06-08 14:53:36.119554 poetry_python_version-0.0.5/src/poetry_python_version/plugins.py
+-rw-r--r--   0        0        0     2160 1970-01-01 00:00:00.000000 poetry_python_version-0.0.5/PKG-INFO
```

### Comparing `poetry_python_version-0.0.4/LICENSE` & `poetry_python_version-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `poetry_python_version-0.0.4/README.md` & `poetry_python_version-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `poetry_python_version-0.0.4/pyproject.toml` & `poetry_python_version-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "poetry-python-version"
-version = "0.0.4"
+version = "0.0.5"
 authors = ["Jiri Kuncar <jiri.kuncar@gmail.com>"]
 description = "Poetry plugin to read Python version from .python-version file"
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/jirikuncar/poetry-python-version"
 repository = "https://github.com/jirikuncar/poetry-python-version"
 packages = [{include = "poetry_python_version", from = "src"}]
```

### Comparing `poetry_python_version-0.0.4/src/poetry_python_version/plugins.py` & `poetry_python_version-0.0.5/src/poetry_python_version/plugins.py`

 * *Files identical despite different names*

### Comparing `poetry_python_version-0.0.4/PKG-INFO` & `poetry_python_version-0.0.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: poetry-python-version
-Version: 0.0.4
+Version: 0.0.5
 Summary: Poetry plugin to read Python version from .python-version file
 Home-page: https://github.com/jirikuncar/poetry-python-version
 License: MIT
 Author: Jiri Kuncar
 Author-email: jiri.kuncar@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 2
```

