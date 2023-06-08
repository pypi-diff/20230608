# Comparing `tmp/pytest_ruff-0.0.6.tar.gz` & `tmp/pytest_ruff-0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_ruff-0.0.6.tar", max compression
+gzip compressed data, was "pytest_ruff-0.1.tar", max compression
```

## Comparing `pytest_ruff-0.0.6.tar` & `pytest_ruff-0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1062 2023-04-28 11:42:35.901195 pytest_ruff-0.0.6/LICENSE
--rw-r--r--   0        0        0      542 2023-04-28 11:42:35.901195 pytest_ruff-0.0.6/README.md
--rw-r--r--   0        0        0     1012 2023-04-28 11:43:13.781378 pytest_ruff-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     1999 2023-04-28 11:42:35.901195 pytest_ruff-0.0.6/pytest_ruff.py
--rw-r--r--   0        0        0     1505 1970-01-01 00:00:00.000000 pytest_ruff-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-08 09:25:34.880817 pytest_ruff-0.1/LICENSE
+-rw-r--r--   0        0        0      542 2023-06-08 09:25:34.880817 pytest_ruff-0.1/README.md
+-rw-r--r--   0        0        0     1190 2023-06-08 09:26:11.084066 pytest_ruff-0.1/pyproject.toml
+-rw-r--r--   0        0        0     2436 2023-06-08 09:25:34.880817 pytest_ruff-0.1/pytest_ruff.py
+-rw-r--r--   0        0        0     1463 1970-01-01 00:00:00.000000 pytest_ruff-0.1/PKG-INFO
```

### Comparing `pytest_ruff-0.0.6/LICENSE` & `pytest_ruff-0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.0.6/README.md` & `pytest_ruff-0.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_ruff-0.0.6/pyproject.toml` & `pytest_ruff-0.1/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 [tool.poetry]
 name = "pytest-ruff"
-version = "0.0.6"
+version = "0.1"
 description = "pytest plugin to check ruff requirements."
 authors = ["Iuri de Silvio <iurisilvio@gmail.com>"]
 readme = "README.md"
 classifiers = [ "Development Status :: 4 - Beta", "Intended Audience :: Developers", "Operating System :: OS Independent", "Framework :: Pytest", "Programming Language :: Python :: 3", "Programming Language :: Python :: 3 :: Only", "Topic :: Software Development :: Libraries :: Python Modules"]
 
 [tool.poetry.urls]
-Homepage = "https://github.com/buserbrasil/pytest-ruff"
+Homepage = "https://github.com/businho/pytest-ruff"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry.dependencies]
 python = "^3.7"
-ruff = "*"
+ruff = ">=0.0.242"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.0"
 pytest-mock = "^3.10.0"
+pytest-cov = "^4.1.0"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.pytest.ini_options]
-addopts = "--capture=no"
+addopts = "--capture=no --cov --cov-report term --cov-report xml"
 
 [tool.ruff]
 line-length = 88
 
 [tool.poetry.plugins]
 pytest11 = { ruff = "pytest_ruff" }
+
+[tool.coverage.run]
+branch = true
+
+[tool.coverage.report]
+precision = 2
+show_missing = true
+skip_covered = true
```

### Comparing `pytest_ruff-0.0.6/PKG-INFO` & `pytest_ruff-0.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 Metadata-Version: 2.1
 Name: pytest-ruff
-Version: 0.0.6
+Version: 0.1
 Summary: pytest plugin to check ruff requirements.
 Author: Iuri de Silvio
 Author-email: iurisilvio@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: ruff
-Project-URL: Homepage, https://github.com/buserbrasil/pytest-ruff
+Requires-Dist: ruff (>=0.0.242)
+Project-URL: Homepage, https://github.com/businho/pytest-ruff
 Description-Content-Type: text/markdown
 
 # pytest-ruff
 
 A pytest plugin to run [ruff](https://pypi.org/project/ruff/).
 
 ## Installation
```

