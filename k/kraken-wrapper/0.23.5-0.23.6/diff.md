# Comparing `tmp/kraken_wrapper-0.23.5.tar.gz` & `tmp/kraken_wrapper-0.23.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kraken_wrapper-0.23.5.tar", max compression
+gzip compressed data, was "kraken_wrapper-0.23.6.tar", max compression
```

## Comparing `kraken_wrapper-0.23.5.tar` & `kraken_wrapper-0.23.6.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      988 2023-06-05 10:39:56.886168 kraken_wrapper-0.23.5/LICENSE
--rw-r--r--   0        0        0      433 2023-06-05 10:39:56.886275 kraken_wrapper-0.23.5/README.md
--rw-r--r--   0        0        0     2084 2023-06-08 12:50:40.456290 kraken_wrapper-0.23.5/pyproject.toml
--rw-r--r--   0        0        0      134 2023-06-08 12:50:40.456570 kraken_wrapper-0.23.5/src/kraken/wrapper/__init__.py
--rw-r--r--   0        0        0     3637 2023-06-05 10:39:56.887091 kraken_wrapper-0.23.5/src/kraken/wrapper/_buildend_venv.py
--rw-r--r--   0        0        0     3374 2023-06-05 10:39:56.887216 kraken_wrapper-0.23.5/src/kraken/wrapper/_buildenv.py
--rw-r--r--   0        0        0     5311 2023-06-05 10:39:56.887336 kraken_wrapper-0.23.5/src/kraken/wrapper/_buildenv_manager.py
--rw-r--r--   0        0        0     3674 2023-06-05 10:39:56.887462 kraken_wrapper-0.23.5/src/kraken/wrapper/_buildenv_pex.py
--rw-r--r--   0        0        0     3175 2023-06-05 10:39:56.887587 kraken_wrapper-0.23.5/src/kraken/wrapper/_config.py
--rw-r--r--   0        0        0     4605 2023-06-05 10:39:56.887725 kraken_wrapper-0.23.5/src/kraken/wrapper/_lockfile.py
--rw-r--r--   0        0        0     3564 2023-06-05 10:39:56.887849 kraken_wrapper-0.23.5/src/kraken/wrapper/_option_sets.py
--rw-r--r--   0        0        0     4222 2023-06-05 10:39:56.887977 kraken_wrapper-0.23.5/src/kraken/wrapper/_pex.py
--rw-r--r--   0        0        0    15754 2023-06-05 10:39:56.888145 kraken_wrapper-0.23.5/src/kraken/wrapper/main.py
--rw-r--r--   0        0        0        0 2023-06-05 10:39:56.888214 kraken_wrapper-0.23.5/src/kraken/wrapper/py.typed
--rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 kraken_wrapper-0.23.5/PKG-INFO
+-rw-r--r--   0        0        0      988 2023-06-05 10:39:56.886168 kraken_wrapper-0.23.6/LICENSE
+-rw-r--r--   0        0        0      433 2023-06-05 10:39:56.886275 kraken_wrapper-0.23.6/README.md
+-rw-r--r--   0        0        0     2084 2023-06-08 14:34:11.182387 kraken_wrapper-0.23.6/pyproject.toml
+-rw-r--r--   0        0        0      134 2023-06-08 14:34:11.182520 kraken_wrapper-0.23.6/src/kraken/wrapper/__init__.py
+-rw-r--r--   0        0        0     3637 2023-06-05 10:39:56.887091 kraken_wrapper-0.23.6/src/kraken/wrapper/_buildend_venv.py
+-rw-r--r--   0        0        0     3374 2023-06-05 10:39:56.887216 kraken_wrapper-0.23.6/src/kraken/wrapper/_buildenv.py
+-rw-r--r--   0        0        0     5311 2023-06-05 10:39:56.887336 kraken_wrapper-0.23.6/src/kraken/wrapper/_buildenv_manager.py
+-rw-r--r--   0        0        0     3674 2023-06-05 10:39:56.887462 kraken_wrapper-0.23.6/src/kraken/wrapper/_buildenv_pex.py
+-rw-r--r--   0        0        0     3175 2023-06-05 10:39:56.887587 kraken_wrapper-0.23.6/src/kraken/wrapper/_config.py
+-rw-r--r--   0        0        0     4605 2023-06-05 10:39:56.887725 kraken_wrapper-0.23.6/src/kraken/wrapper/_lockfile.py
+-rw-r--r--   0        0        0     3564 2023-06-05 10:39:56.887849 kraken_wrapper-0.23.6/src/kraken/wrapper/_option_sets.py
+-rw-r--r--   0        0        0     4222 2023-06-05 10:39:56.887977 kraken_wrapper-0.23.6/src/kraken/wrapper/_pex.py
+-rw-r--r--   0        0        0    15754 2023-06-05 10:39:56.888145 kraken_wrapper-0.23.6/src/kraken/wrapper/main.py
+-rw-r--r--   0        0        0        0 2023-06-05 10:39:56.888214 kraken_wrapper-0.23.6/src/kraken/wrapper/py.typed
+-rw-r--r--   0        0        0     1428 1970-01-01 00:00:00.000000 kraken_wrapper-0.23.6/PKG-INFO
```

### Comparing `kraken_wrapper-0.23.5/LICENSE` & `kraken_wrapper-0.23.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/pyproject.toml` & `kraken_wrapper-0.23.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "kraken-wrapper"
-version = "0.23.5"
+version = "0.23.6"
 description = ""
 authors = ["Unknown <me@unknown.org>"]
 license = "MIT"
 readme = "README.md"
 packages = [{ include = "kraken/wrapper", from = "src" }]
 classifiers = []
 keywords = []
@@ -18,15 +18,15 @@
 Documentation = "https://kraken-build.github.io/kraken-build/"
 Homepage = "https://kraken-build.github.io/kraken-build/"
 Repository = "https://github.com/kraken-build/kraken-build/"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
 keyring = "^23.8.2"
-kraken-common = "^0.23.5"
+kraken-common = "^0.23.6"
 pex = "^2.1.103"
 setuptools = ">=33.0.0"  # For pkg_resources
 termcolor = "^1.1.0"
 
 [tool.poetry.dev-dependencies]
 black = "*"
 flake8 = "*"
```

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_buildend_venv.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_buildend_venv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_buildenv.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_buildenv.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_buildenv_manager.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_buildenv_manager.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_buildenv_pex.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_buildenv_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_config.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_config.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_lockfile.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_lockfile.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_option_sets.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_option_sets.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/_pex.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/_pex.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/src/kraken/wrapper/main.py` & `kraken_wrapper-0.23.6/src/kraken/wrapper/main.py`

 * *Files identical despite different names*

### Comparing `kraken_wrapper-0.23.5/PKG-INFO` & `kraken_wrapper-0.23.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: kraken-wrapper
-Version: 0.23.5
+Version: 0.23.6
 Summary: 
 License: MIT
 Author: Unknown
 Author-email: me@unknown.org
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: keyring (>=23.8.2,<24.0.0)
-Requires-Dist: kraken-common (>=0.23.5,<0.24.0)
+Requires-Dist: kraken-common (>=0.23.6,<0.24.0)
 Requires-Dist: pex (>=2.1.103,<3.0.0)
 Requires-Dist: setuptools (>=33.0.0)
 Requires-Dist: termcolor (>=1.1.0,<2.0.0)
 Project-URL: Bug Tracker, https://github.com/kraken-build/kraken-build/issues
 Project-URL: Documentation, https://kraken-build.github.io/kraken-build/
 Project-URL: Homepage, https://kraken-build.github.io/kraken-build/
 Project-URL: Repository, https://github.com/kraken-build/kraken-build/
```

