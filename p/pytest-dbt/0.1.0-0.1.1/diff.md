# Comparing `tmp/pytest_dbt-0.1.0.tar.gz` & `tmp/pytest_dbt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_dbt-0.1.0.tar", max compression
+gzip compressed data, was "pytest_dbt-0.1.1.tar", max compression
```

## Comparing `pytest_dbt-0.1.0.tar` & `pytest_dbt-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1062 2023-05-31 09:50:43.761839 pytest_dbt-0.1.0/LICENSE
--rw-r--r--   0        0        0     2177 2023-05-31 09:50:43.761839 pytest_dbt-0.1.0/README.md
--rw-r--r--   0        0        0     1571 2023-05-31 09:50:43.765839 pytest_dbt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-31 09:50:43.765839 pytest_dbt-0.1.0/pytest_dbt/__init__.py
--rw-r--r--   0        0        0     1024 2023-05-31 09:50:43.765839 pytest_dbt-0.1.0/pytest_dbt/dbt_context.py
--rw-r--r--   0        0        0     3589 2023-05-31 09:50:43.765839 pytest_dbt-0.1.0/pytest_dbt/pytest_dbt.py
--rw-r--r--   0        0        0     3535 1970-01-01 00:00:00.000000 pytest_dbt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2023-06-08 00:19:42.035284 pytest_dbt-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4415 2023-06-08 00:19:42.035284 pytest_dbt-0.1.1/README.md
+-rw-r--r--   0        0        0     1444 2023-06-08 00:19:42.039284 pytest_dbt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 00:19:42.039284 pytest_dbt-0.1.1/pytest_dbt/__init__.py
+-rw-r--r--   0        0        0     1040 2023-06-08 00:19:42.039284 pytest_dbt-0.1.1/pytest_dbt/dbt_context.py
+-rw-r--r--   0        0        0     5136 2023-06-08 00:19:42.039284 pytest_dbt-0.1.1/pytest_dbt/pytest_dbt.py
+-rw-r--r--   0        0        0     2526 2023-06-08 00:19:42.039284 pytest_dbt-0.1.1/pytest_dbt/sql_exec.py
+-rw-r--r--   0        0        0     5632 1970-01-01 00:00:00.000000 pytest_dbt-0.1.1/PKG-INFO
```

### Comparing `pytest_dbt-0.1.0/LICENSE` & `pytest_dbt-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_dbt-0.1.0/pyproject.toml` & `pytest_dbt-0.1.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-dbt"
-version = "0.1.0"
+version = "0.1.1"
 description = "Unit test dbt models with standard python tooling"
 authors = ["Anup Kalburgi <anupkalburgi@gmail.com>"]
 readme = "README.md"
 license = "MPL-2.0"
 packages = [{include = "pytest_dbt"}]
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
@@ -16,16 +16,14 @@
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS :: MacOS X",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
-  "Programming Language :: Python :: Implementation :: CPython",
-  "Programming Language :: Python :: Implementation :: PyPy",
   "Topic :: Software Development :: Quality Assurance",
   "Topic :: Software Development :: Testing",
   "Topic :: Utilities",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `pytest_dbt-0.1.0/pytest_dbt/dbt_context.py` & `pytest_dbt-0.1.1/pytest_dbt/dbt_context.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,21 +5,21 @@
 
 class DbtContextSingleton:
     _instance = None
     _dbt_manifest_file_path = ""
 
     @staticmethod
     def getInstance():
-        """ Static access method. """
+        """Static access method."""
         if DbtContextSingleton._instance is None:
             DbtContextSingleton()
         return DbtContextSingleton._instance
 
     def __init__(self):
-        """ Virtually private constructor. """
+        """Virtually private constructor."""
         if DbtContextSingleton._instance is not None:
             raise Exception("This class is a singleton!")
         else:
             DbtContextSingleton._instance = self
 
     @property
     def dbt_manifest_file_path(self):
@@ -33,8 +33,9 @@
 @dataclass(frozen=True)
 class DBTModelDetails:
     name: str
     alias: str
     original_file_path: str
     compiled_path: str
     upstream_models: Set[str]
-    compiled_code: str
+    udfs: Set[str]
+    compiled_code: str
```

