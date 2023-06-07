# Comparing `tmp/static-frame-pyodide-0.1.5.tar.gz` & `tmp/static-frame-pyodide-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "static-frame-pyodide-0.1.5.tar", last modified: Mon Jun  5 00:17:26 2023, max compression
+gzip compressed data, was "static-frame-pyodide-0.1.6.tar", last modified: Wed Jun  7 23:01:40 2023, max compression
```

## Comparing `static-frame-pyodide-0.1.5.tar` & `static-frame-pyodide-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-05 00:17:26.803172 static-frame-pyodide-0.1.5/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.5/LICENSE
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-05 00:17:26.803172 static-frame-pyodide-0.1.5/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.5/README.md
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.5/pyproject.toml
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-05 00:17:26.803172 static-frame-pyodide-0.1.5/setup.cfg
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-05 00:17:26.799172 static-frame-pyodide-0.1.5/static_frame_pyodide/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)     1259 2023-06-05 00:16:07.000000 static-frame-pyodide-0.1.5/static_frame_pyodide/__init__.py
-drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-05 00:17:26.803172 static-frame-pyodide-0.1.5/static_frame_pyodide.egg-info/
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-05 00:17:26.000000 static-frame-pyodide-0.1.5/static_frame_pyodide.egg-info/PKG-INFO
--rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-05 00:17:26.000000 static-frame-pyodide-0.1.5/static_frame_pyodide.egg-info/SOURCES.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-05 00:17:26.000000 static-frame-pyodide-0.1.5/static_frame_pyodide.egg-info/dependency_links.txt
--rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-05 00:17:26.000000 static-frame-pyodide-0.1.5/static_frame_pyodide.egg-info/top_level.txt
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-07 23:01:40.633834 static-frame-pyodide-0.1.6/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1069 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.6/LICENSE
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-07 23:01:40.633834 static-frame-pyodide-0.1.6/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      114 2023-06-02 14:53:38.000000 static-frame-pyodide-0.1.6/README.md
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     1191 2023-06-02 23:47:09.000000 static-frame-pyodide-0.1.6/pyproject.toml
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       38 2023-06-07 23:01:40.633834 static-frame-pyodide-0.1.6/setup.cfg
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-07 23:01:40.629834 static-frame-pyodide-0.1.6/static_frame_pyodide/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)     2383 2023-06-07 22:59:44.000000 static-frame-pyodide-0.1.6/static_frame_pyodide/__init__.py
+drwxrwxr-x   0 ariza     (1000) ariza     (1000)        0 2023-06-07 23:01:40.629834 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      987 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/PKG-INFO
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)      241 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/SOURCES.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)        1 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/dependency_links.txt
+-rw-rw-r--   0 ariza     (1000) ariza     (1000)       21 2023-06-07 23:01:40.000000 static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/top_level.txt
```

### Comparing `static-frame-pyodide-0.1.5/LICENSE` & `static-frame-pyodide-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.5/PKG-INFO` & `static-frame-pyodide-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.5
+Version: 0.1.6
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

### Comparing `static-frame-pyodide-0.1.5/pyproject.toml` & `static-frame-pyodide-0.1.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `static-frame-pyodide-0.1.5/static_frame_pyodide.egg-info/PKG-INFO` & `static-frame-pyodide-0.1.6/static_frame_pyodide.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: static-frame-pyodide
-Version: 0.1.5
+Version: 0.1.6
 Summary: StaticFrame packaged for use in Pyodide, PyScript, and WebAssembly/Emscripten environments
 Author: Christopher Ariza
 License: MIT
 Keywords: immutable,array,numpy,data structures
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
```

