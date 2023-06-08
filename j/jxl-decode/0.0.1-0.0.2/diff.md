# Comparing `tmp/jxl_decode-0.0.1.tar.gz` & `tmp/jxl_decode-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jxl_decode-0.0.1.tar", last modified: Thu Jun  8 18:44:17 2023, max compression
+gzip compressed data, was "jxl_decode-0.0.2.tar", last modified: Thu Jun  8 19:32:34 2023, max compression
```

## Comparing `jxl_decode-0.0.1.tar` & `jxl_decode-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-06-08 18:44:17.723787 jxl_decode-0.0.1/
--rw-r--r--   0 james     (1000) james     (1000)     1111 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/LICENCE.md
--rw-r--r--   0 james     (1000) james     (1000)     2530 2023-06-08 18:44:17.723787 jxl_decode-0.0.1/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)     1913 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/README.md
--rw-r--r--   0 james     (1000) james     (1000)      734 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/pyproject.toml
--rw-r--r--   0 james     (1000) james     (1000)       38 2023-06-08 18:44:17.723787 jxl_decode-0.0.1/setup.cfg
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-06-08 18:44:17.722787 jxl_decode-0.0.1/src/
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-06-08 18:44:17.723787 jxl_decode-0.0.1/src/jxl_decode/
--rw-r--r--   0 james     (1000) james     (1000)      152 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/__init__.py
--rw-r--r--   0 james     (1000) james     (1000)       94 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/__main__.py
--rw-r--r--   0 james     (1000) james     (1000)     1299 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/common.py
--rw-r--r--   0 james     (1000) james     (1000)      296 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/decode_jpg.py
--rw-r--r--   0 james     (1000) james     (1000)     4684 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/decode_jxl.py
--rw-r--r--   0 james     (1000) james     (1000)     2052 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/decode_ppm.py
--rw-r--r--   0 james     (1000) james     (1000)      234 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/encode_png.py
--rw-r--r--   0 james     (1000) james     (1000)     2442 2023-06-08 18:38:21.000000 jxl_decode-0.0.1/src/jxl_decode/main.py
-drwxr-xr-x   0 james     (1000) james     (1000)        0 2023-06-08 18:44:17.723787 jxl_decode-0.0.1/src/jxl_decode.egg-info/
--rw-r--r--   0 james     (1000) james     (1000)     2530 2023-06-08 18:44:17.000000 jxl_decode-0.0.1/src/jxl_decode.egg-info/PKG-INFO
--rw-r--r--   0 james     (1000) james     (1000)      405 2023-06-08 18:44:17.000000 jxl_decode-0.0.1/src/jxl_decode.egg-info/SOURCES.txt
--rw-r--r--   0 james     (1000) james     (1000)        1 2023-06-08 18:44:17.000000 jxl_decode-0.0.1/src/jxl_decode.egg-info/dependency_links.txt
--rw-r--r--   0 james     (1000) james     (1000)       11 2023-06-08 18:44:17.000000 jxl_decode-0.0.1/src/jxl_decode.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:34.985247 jxl_decode-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/LICENCE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-08 19:32:34.985247 jxl_decode-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:34.985247 jxl_decode-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:34.981247 jxl_decode-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:34.985247 jxl_decode-0.0.2/src/jxl_decode/
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/decode_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/decode_jxl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/decode_ppm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/encode_png.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-06-08 19:32:21.000000 jxl_decode-0.0.2/src/jxl_decode/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:34.985247 jxl_decode-0.0.2/src/jxl_decode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-08 19:32:34.000000 jxl_decode-0.0.2/src/jxl_decode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-08 19:32:34.000000 jxl_decode-0.0.2/src/jxl_decode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:34.000000 jxl_decode-0.0.2/src/jxl_decode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-08 19:32:34.000000 jxl_decode-0.0.2/src/jxl_decode.egg-info/top_level.txt
```

### Comparing `jxl_decode-0.0.1/LICENCE.md` & `jxl_decode-0.0.2/LICENCE.md`

 * *Files identical despite different names*

### Comparing `jxl_decode-0.0.1/PKG-INFO` & `jxl_decode-0.0.2/src/jxl_decode.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jxl_decode
-Version: 0.0.1
+Name: jxl-decode
+Version: 0.0.2
 Summary: A pure python JPEG XL decoder.
 Author-email: James Frost <git@frost.cx>
 Project-URL: Homepage, https://github.com/Fraetor/jxl_decode
 Project-URL: Bug Tracker, https://github.com/Fraetor/jxl_decode/issues
 Keywords: JPEG XL,jxl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,28 @@
 
 # jxl_decode
 
 A pure python JPEG XL decoder. It is currently *very* incomplete.
 
 ## Installation
 
+jxl_decode can be installed from [PyPI](https://pypi.org/project/jxl-decode/).
+
+```sh
+pip install jxl_decode
+```
+
 I am aiming to make this decoder as portable as possible. As such it will
 ideally have minimal dependencies outside of the standard library. I may use a
 dependency for PNG output, if I don't write one myself.
 
 ### Requirements
 
-- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work with some older versions)
+- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work
+  with some older versions)
 
 ### Development Requirements
 
 - [PyTest](https://docs.pytest.org/)
 
 ## Usage
```

### Comparing `jxl_decode-0.0.1/README.md` & `jxl_decode-0.0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 # jxl_decode
 
 A pure python JPEG XL decoder. It is currently *very* incomplete.
 
 ## Installation
 
+jxl_decode can be installed from [PyPI](https://pypi.org/project/jxl-decode/).
+
+```sh
+pip install jxl_decode
+```
+
 I am aiming to make this decoder as portable as possible. As such it will
 ideally have minimal dependencies outside of the standard library. I may use a
 dependency for PNG output, if I don't write one myself.
 
 ### Requirements
 
-- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work with some older versions)
+- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work
+  with some older versions)
 
 ### Development Requirements
 
 - [PyTest](https://docs.pytest.org/)
 
 ## Usage
```

### Comparing `jxl_decode-0.0.1/pyproject.toml` & `jxl_decode-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "jxl_decode"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="James Frost", email="git@frost.cx" },
 ]
 description = "A pure python JPEG XL decoder."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = ["JPEG XL", "jxl"]
```

### Comparing `jxl_decode-0.0.1/src/jxl_decode/common.py` & `jxl_decode-0.0.2/src/jxl_decode/common.py`

 * *Files identical despite different names*

### Comparing `jxl_decode-0.0.1/src/jxl_decode/decode_jxl.py` & `jxl_decode-0.0.2/src/jxl_decode/decode_jxl.py`

 * *Files identical despite different names*

### Comparing `jxl_decode-0.0.1/src/jxl_decode/decode_ppm.py` & `jxl_decode-0.0.2/src/jxl_decode/decode_ppm.py`

 * *Files identical despite different names*

### Comparing `jxl_decode-0.0.1/src/jxl_decode/main.py` & `jxl_decode-0.0.2/src/jxl_decode/main.py`

 * *Files identical despite different names*

### Comparing `jxl_decode-0.0.1/src/jxl_decode.egg-info/PKG-INFO` & `jxl_decode-0.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: jxl-decode
-Version: 0.0.1
+Name: jxl_decode
+Version: 0.0.2
 Summary: A pure python JPEG XL decoder.
 Author-email: James Frost <git@frost.cx>
 Project-URL: Homepage, https://github.com/Fraetor/jxl_decode
 Project-URL: Bug Tracker, https://github.com/Fraetor/jxl_decode/issues
 Keywords: JPEG XL,jxl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -17,21 +17,28 @@
 
 # jxl_decode
 
 A pure python JPEG XL decoder. It is currently *very* incomplete.
 
 ## Installation
 
+jxl_decode can be installed from [PyPI](https://pypi.org/project/jxl-decode/).
+
+```sh
+pip install jxl_decode
+```
+
 I am aiming to make this decoder as portable as possible. As such it will
 ideally have minimal dependencies outside of the standard library. I may use a
 dependency for PNG output, if I don't write one myself.
 
 ### Requirements
 
-- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work with some older versions)
+- Recent [Python 3](https://www.python.org/) (developed with 3.11, but may work
+  with some older versions)
 
 ### Development Requirements
 
 - [PyTest](https://docs.pytest.org/)
 
 ## Usage
```

