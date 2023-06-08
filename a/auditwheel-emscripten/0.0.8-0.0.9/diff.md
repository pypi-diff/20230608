# Comparing `tmp/auditwheel_emscripten-0.0.8.tar.gz` & `tmp/auditwheel_emscripten-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auditwheel_emscripten-0.0.8.tar", last modified: Mon Nov  7 06:29:23 2022, max compression
+gzip compressed data, was "auditwheel_emscripten-0.0.9.tar", last modified: Tue Dec 20 02:17:42 2022, max compression
```

## Comparing `auditwheel_emscripten-0.0.8.tar` & `auditwheel_emscripten-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     5035 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/README.md
--rw-r--r--   0        0        0      387 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/__init__.py
--rw-r--r--   0        0        0        0 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/cli/__init__.py
--rw-r--r--   0        0        0     3238 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/cli/main.py
--rw-r--r--   0        0        0        0 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/__init__.py
--rw-r--r--   0        0        0     7072 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/diagnostics.py
--rw-r--r--   0        0        0     3316 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/utils.py
--rw-r--r--   0        0        0    17027 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/webassembly.py
--rw-r--r--   0        0        0     1740 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/exports.py
--rw-r--r--   0        0        0     1740 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/imports.py
--rw-r--r--   0        0        0      673 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/lib_utils.py
--rw-r--r--   0        0        0     4935 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/module.py
--rw-r--r--   0        0        0     3486 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/repair.py
--rw-r--r--   0        0        0     1695 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/show.py
--rw-r--r--   0        0        0     2121 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/auditwheel_emscripten/wheel_utils.py
--rw-r--r--   0        0        0      630 2022-11-07 06:29:02.369829 auditwheel_emscripten-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     5509 1970-01-01 00:00:00.000000 auditwheel_emscripten-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     7153 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/README.md
+-rw-r--r--   0        0        0      387 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/cli/__init__.py
+-rw-r--r--   0        0        0     3238 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/cli/main.py
+-rw-r--r--   0        0        0        0 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/__init__.py
+-rw-r--r--   0        0        0     7072 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/diagnostics.py
+-rw-r--r--   0        0        0     3316 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/utils.py
+-rw-r--r--   0        0        0    17027 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/webassembly.py
+-rw-r--r--   0        0        0     1740 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/exports.py
+-rw-r--r--   0        0        0     1740 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/imports.py
+-rw-r--r--   0        0        0      682 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/lib_utils.py
+-rw-r--r--   0        0        0     4935 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/module.py
+-rw-r--r--   0        0        0     3486 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/repair.py
+-rw-r--r--   0        0        0     1695 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/show.py
+-rw-r--r--   0        0        0     2121 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/auditwheel_emscripten/wheel_utils.py
+-rw-r--r--   0        0        0      635 2022-12-20 02:17:25.327754 auditwheel_emscripten-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     7627 1970-01-01 00:00:00.000000 auditwheel_emscripten-0.0.9/PKG-INFO
```

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/cli/main.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/cli/main.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/diagnostics.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/diagnostics.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/utils.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/utils.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/emscripten_tools/webassembly.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/emscripten_tools/webassembly.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/exports.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/exports.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/imports.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/imports.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/lib_utils.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/lib_utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         libdir / "lib" / "wasm32-emscripten" / "pic",
         libdir / "lib" / "wasm32-emscripten",
     ]
 
 
 @cache
 def sharedlib_regex() -> re.Pattern:
-    return re.compile(r"\.so(.\d+)*$")
+    return re.compile(r"(\.so(.\d+)*|\.wasm)$")
 
 
 def get_all_shared_libs_in_dir(directory: str | Path) -> list[Path]:
     directory = Path(directory)
     so_regex = sharedlib_regex()
     return list(
         filter(lambda f: so_regex.search(f.name) is not None, directory.glob("**/*"))
```

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/module.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/module.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/repair.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/repair.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/show.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/show.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/auditwheel_emscripten/wheel_utils.py` & `auditwheel_emscripten-0.0.9/auditwheel_emscripten/wheel_utils.py`

 * *Files identical despite different names*

### Comparing `auditwheel_emscripten-0.0.8/pyproject.toml` & `auditwheel_emscripten-0.0.9/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -23,8 +23,8 @@
 ]
 
 
 [project.urls]
 Home = "https://github.com/ryanking13/auditwheel-emscripten"
 
 [project.entry-points."pyodide.cli"]
-audit = "auditwheel_emscripten.cli.main:app"
+auditwheel = "auditwheel_emscripten.cli.main:app"
```

