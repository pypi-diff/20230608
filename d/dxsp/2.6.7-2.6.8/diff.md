# Comparing `tmp/dxsp-2.6.7.tar.gz` & `tmp/dxsp-2.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dxsp-2.6.7.tar", max compression
+gzip compressed data, was "dxsp-2.6.8.tar", max compression
```

## Comparing `dxsp-2.6.7.tar` & `dxsp-2.6.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-06-05 19:17:11.526409 dxsp-2.6.7/LICENSE
--rw-r--r--   0        0        0     2348 2023-06-05 19:17:11.526409 dxsp-2.6.7/README.md
--rw-r--r--   0        0        0       86 2023-06-05 19:17:12.306439 dxsp-2.6.7/dxsp/__init__.py
--rw-r--r--   0        0        0      387 2023-06-05 19:17:11.526409 dxsp-2.6.7/dxsp/config.py
--rw-r--r--   0        0        0     3679 2023-06-05 19:17:11.526409 dxsp-2.6.7/dxsp/default_settings.toml
--rw-r--r--   0        0        0    18964 2023-06-05 19:17:11.526409 dxsp-2.6.7/dxsp/main.py
--rw-r--r--   0        0        0     1542 2023-06-05 19:17:12.306439 dxsp-2.6.7/pyproject.toml
--rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-08 15:15:07.664281 dxsp-2.6.8/LICENSE
+-rw-r--r--   0        0        0     2348 2023-06-08 15:15:07.664281 dxsp-2.6.8/README.md
+-rw-r--r--   0        0        0       86 2023-06-08 15:15:28.893762 dxsp-2.6.8/dxsp/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-08 15:15:07.664281 dxsp-2.6.8/dxsp/config.py
+-rw-r--r--   0        0        0     3679 2023-06-08 15:15:07.664281 dxsp-2.6.8/dxsp/default_settings.toml
+-rw-r--r--   0        0        0    18964 2023-06-08 15:15:07.664281 dxsp-2.6.8/dxsp/main.py
+-rw-r--r--   0        0        0     1542 2023-06-08 15:15:28.893762 dxsp-2.6.8/pyproject.toml
+-rw-r--r--   0        0        0     3138 1970-01-01 00:00:00.000000 dxsp-2.6.8/PKG-INFO
```

### Comparing `dxsp-2.6.7/LICENSE` & `dxsp-2.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.7/README.md` & `dxsp-2.6.8/README.md`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.7/dxsp/default_settings.toml` & `dxsp-2.6.8/dxsp/default_settings.toml`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.7/dxsp/main.py` & `dxsp-2.6.8/dxsp/main.py`

 * *Files identical despite different names*

### Comparing `dxsp-2.6.7/pyproject.toml` & `dxsp-2.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dxsp"
-version = "2.6.7"
+version = "2.6.8"
 description = "DXSP (DeX SwaP), A defi swap helper package. Swap made easy."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [
     {include = "dxsp"}
 ]
```

### Comparing `dxsp-2.6.7/PKG-INFO` & `dxsp-2.6.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dxsp
-Version: 2.6.7
+Version: 2.6.8
 Summary: DXSP (DeX SwaP), A defi swap helper package. Swap made easy.
 License: MIT
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

