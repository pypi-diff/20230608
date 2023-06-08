# Comparing `tmp/jquants_derivatives-0.1.0a1.tar.gz` & `tmp/jquants_derivatives-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jquants_derivatives-0.1.0a1.tar", max compression
+gzip compressed data, was "jquants_derivatives-0.1.0a2.tar", max compression
```

## Comparing `jquants_derivatives-0.1.0a1.tar` & `jquants_derivatives-0.1.0a2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       22 2023-06-06 13:53:32.816616 jquants_derivatives-0.1.0a1/README.md
--rw-r--r--   0        0        0      124 2023-06-06 14:36:12.452162 jquants_derivatives-0.1.0a1/jquants_derivatives/__init__.py
--rw-r--r--   0        0        0     1870 2023-06-06 15:52:55.552479 jquants_derivatives-0.1.0a1/jquants_derivatives/client.py
--rw-r--r--   0        0        0     1290 2023-06-05 23:18:08.508412 jquants_derivatives-0.1.0a1/jquants_derivatives/database.py
--rw-r--r--   0        0        0     5337 2023-06-06 15:43:26.519073 jquants_derivatives-0.1.0a1/jquants_derivatives/derivatievs.py
--rw-r--r--   0        0        0     1302 2023-06-06 15:08:31.605466 jquants_derivatives-0.1.0a1/jquants_derivatives/models.py
--rw-r--r--   0        0        0      514 2023-06-06 14:46:30.172595 jquants_derivatives-0.1.0a1/pyproject.toml
--rw-r--r--   0        0        0      654 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a1/setup.py
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a1/PKG-INFO
+-rw-r--r--   0        0        0     8758 2023-06-08 05:22:56.205337 jquants_derivatives-0.1.0a2/README.md
+-rw-r--r--   0        0        0      124 2023-06-06 14:36:12.452162 jquants_derivatives-0.1.0a2/jquants_derivatives/__init__.py
+-rw-r--r--   0        0        0     1870 2023-06-06 15:52:55.552479 jquants_derivatives-0.1.0a2/jquants_derivatives/client.py
+-rw-r--r--   0        0        0     1290 2023-06-05 23:18:08.508412 jquants_derivatives-0.1.0a2/jquants_derivatives/database.py
+-rw-r--r--   0        0        0     5337 2023-06-06 15:43:26.519073 jquants_derivatives-0.1.0a2/jquants_derivatives/derivatievs.py
+-rw-r--r--   0        0        0     1302 2023-06-06 15:08:31.605466 jquants_derivatives-0.1.0a2/jquants_derivatives/models.py
+-rw-r--r--   0        0        0      656 2023-06-08 05:27:40.458941 jquants_derivatives-0.1.0a2/pyproject.toml
+-rw-r--r--   0        0        0     9716 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a2/setup.py
+-rw-r--r--   0        0        0     9258 1970-01-01 00:00:00.000000 jquants_derivatives-0.1.0a2/PKG-INFO
```

### Comparing `jquants_derivatives-0.1.0a1/jquants_derivatives/client.py` & `jquants_derivatives-0.1.0a2/jquants_derivatives/client.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a1/jquants_derivatives/database.py` & `jquants_derivatives-0.1.0a2/jquants_derivatives/database.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a1/jquants_derivatives/derivatievs.py` & `jquants_derivatives-0.1.0a2/jquants_derivatives/derivatievs.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a1/jquants_derivatives/models.py` & `jquants_derivatives-0.1.0a2/jquants_derivatives/models.py`

 * *Files identical despite different names*

### Comparing `jquants_derivatives-0.1.0a1/pyproject.toml` & `jquants_derivatives-0.1.0a2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "jquants-derivatives"
-version = "0.1.0-alpha1"
-description = ""
+version = "0.1.0-alpha2"
+description = "J-Quants API Client Derivatives Library"
 authors = ["driller"]
 readme = "README.md"
 packages = [{include = "jquants_derivatives"}]
+homepage = "https://github.com/drillan/jquants-derivatives"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 jquants-api-client = "^1.2.0"
 plotly = "^5.14.1"
 
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.1"
+tabulate = "^0.9.0"
+ipython-sql = "^0.5.0"
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.3.1"
 python-dotenv = "^1.0.0"
 mypy = "^1.3.0"
```

