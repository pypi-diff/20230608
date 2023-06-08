# Comparing `tmp/cfg-argparser-1.2.0.post1.tar.gz` & `tmp/cfg-argparser-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfg-argparser-1.2.0.post1.tar", last modified: Wed Jun  7 18:25:11 2023, max compression
+gzip compressed data, was "cfg-argparser-1.2.1.tar", last modified: Thu Jun  8 13:14:39 2023, max compression
```

## Comparing `cfg-argparser-1.2.0.post1.tar` & `cfg-argparser-1.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.526805 cfg-argparser-1.2.0.post1/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.2.0.post1/LICENSE
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1632 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      771 2023-06-07 15:54:57.000000 cfg-argparser-1.2.0.post1/README.md
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      959 2023-06-07 18:24:48.000000 cfg-argparser-1.2.0.post1/pyproject.toml
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-07 18:25:11.526805 cfg-argparser-1.2.0.post1/setup.cfg
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/src/
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/src/cfg_argparser/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/__init__.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/argparse_config.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2882 2023-06-07 05:11:51.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/cfg_dict.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1486 2023-06-07 05:55:21.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/function_config_wrapper.py
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 18:09:29.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser/save_handlers.py
-drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-07 18:25:11.523472 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1632 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/PKG-INFO
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      413 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/SOURCES.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/dependency_links.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/requires.txt
--rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-06-07 18:25:11.000000 cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/top_level.txt
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-08 13:14:39.393631 cfg-argparser-1.2.1/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1071 2023-04-12 20:40:08.000000 cfg-argparser-1.2.1/LICENSE
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1626 2023-06-08 13:14:39.393631 cfg-argparser-1.2.1/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      771 2023-06-08 03:52:10.000000 cfg-argparser-1.2.1/README.md
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      980 2023-06-08 13:14:32.000000 cfg-argparser-1.2.1/pyproject.toml
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       38 2023-06-08 13:14:39.393631 cfg-argparser-1.2.1/setup.cfg
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-08 13:14:39.390297 cfg-argparser-1.2.1/src/
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-08 13:14:39.393631 cfg-argparser-1.2.1/src/cfg_argparser/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      316 2023-06-07 03:20:42.000000 cfg-argparser-1.2.1/src/cfg_argparser/__init__.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     9978 2023-06-07 01:13:05.000000 cfg-argparser-1.2.1/src/cfg_argparser/argparse_config.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2882 2023-06-07 05:11:51.000000 cfg-argparser-1.2.1/src/cfg_argparser/cfg_dict.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     2262 2023-06-08 12:34:52.000000 cfg-argparser-1.2.1/src/cfg_argparser/function_config_wrapper.py
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1391 2023-06-07 18:09:29.000000 cfg-argparser-1.2.1/src/cfg_argparser/save_handlers.py
+drwxr-xr-x   0 xpsyc     (1000) xpsyc     (1000)        0 2023-06-08 13:14:39.393631 cfg-argparser-1.2.1/src/cfg_argparser.egg-info/
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)     1626 2023-06-08 13:14:39.000000 cfg-argparser-1.2.1/src/cfg_argparser.egg-info/PKG-INFO
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)      413 2023-06-08 13:14:39.000000 cfg-argparser-1.2.1/src/cfg_argparser.egg-info/SOURCES.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)        1 2023-06-08 13:14:39.000000 cfg-argparser-1.2.1/src/cfg_argparser.egg-info/dependency_links.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       25 2023-06-08 13:14:39.000000 cfg-argparser-1.2.1/src/cfg_argparser.egg-info/requires.txt
+-rw-r--r--   0 xpsyc     (1000) xpsyc     (1000)       14 2023-06-08 13:14:39.000000 cfg-argparser-1.2.1/src/cfg_argparser.egg-info/top_level.txt
```

### Comparing `cfg-argparser-1.2.0.post1/LICENSE` & `cfg-argparser-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0.post1/PKG-INFO` & `cfg-argparser-1.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.2.0.post1
+Version: 1.2.1
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_argparser 1.2.0
+# cfg_argparser 1.2.1
 
 a config wrapper I made.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-argparser-1.2.0.post1/README.md` & `cfg-argparser-1.2.1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# cfg_argparser 1.2.0
+# cfg_argparser 1.2.1
 
 a config wrapper I made.
 
 ## Installation
 
 ```bash
 # from pypi:
```

### Comparing `cfg-argparser-1.2.0.post1/pyproject.toml` & `cfg-argparser-1.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools", "toml"]
+requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cfg-argparser"
-version = "1.2.0-1"
+version = "1.2.1"
 authors = [{ name = "Zeptofine", email = "zeptofine@gmail.com" }]
 description = "A package designed to simplify configurable defaults from argparse."
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
@@ -25,7 +25,10 @@
 [project.urls]
 "Homepage" = "https://github.com/zeptofine/cfg-argparser"
 "Bug Tracker" = "https://github.com/zeptofine/cfg-argparser/issues"
 
 
 [project.optional-dependencies]
 typer = ['typer[all]']
+
+[tool.ruff]
+line-length = 120
```

### Comparing `cfg-argparser-1.2.0.post1/src/cfg_argparser/argparse_config.py` & `cfg-argparser-1.2.1/src/cfg_argparser/argparse_config.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0.post1/src/cfg_argparser/cfg_dict.py` & `cfg-argparser-1.2.1/src/cfg_argparser/cfg_dict.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0.post1/src/cfg_argparser/function_config_wrapper.py` & `cfg-argparser-1.2.1/src/cfg_argparser/function_config_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,59 @@
 """A function that can be decorated or wrapped around a file"""
 import functools
 import inspect
 from typing import Callable
-
+import types
 from .cfg_dict import CfgDict
 
 
+def copy_func(f, name=None):
+    """
+    return a function with same code, globals, defaults, closure, and
+    name (or provide a new name)
+    """
+    fn = types.FunctionType(f.__code__, f.__globals__, name or f.__name__, f.__defaults__, f.__closure__)
+    # in case f was given attrs (note this dict is a shallow copy):
+    fn.__dict__.update(f.__dict__)
+    fn.__annotations__ = f.__annotations__
+    fn.__doc__ = f.__doc__
+    return fn
+
+
 def wrap_config(cfg_dict: CfgDict) -> Callable[..., Callable]:
     """Wraps a function with a CfgDict file to make an easy config configuration"""
 
     def _wrapper(func: Callable) -> Callable:
         # get parameters and defaults
+
         parameters: dict[str, inspect.Parameter] = dict(inspect.signature(func).parameters)
         save_after = False
         for name, param in parameters.items():
             if name not in cfg_dict:
                 if cfg_dict.is_json_serializable(param.default):
                     save_after = True
                     cfg_dict[name] = param.default
         if save_after:
             cfg_dict.save()
+        new_defaults = dict(zip(parameters.keys(), map(lambda x: x.default, parameters.values())))
+        new_defaults.update({k: v for k, v in cfg_dict.items() if k in new_defaults})
+
+        func = copy_func(func)
 
         @functools.wraps(func)
         def _wrap(*args, **kwargs):
             new_defaults = dict(zip(parameters.keys(), map(lambda x: x.default, parameters.values())))
             new_defaults.update({k: v for k, v in cfg_dict.items() if k in new_defaults})
             new_defaults.update(kwargs)
 
             # convert args to kwargs
             default_lst = list(enumerate(new_defaults.items()))
             for idx, arg in enumerate(args):
                 default_lst[idx] = (default_lst[idx][0], (default_lst[idx][1][0], arg))
             new_defaults = dict(map(lambda arg: arg[1], default_lst))
-            return func(**new_defaults)
+            return func(**new_defaults)  # type: ignore
+
+        _wrap.__wrapped__.__defaults__ = tuple(new_defaults.values())  # type: ignore
 
         return _wrap
 
     return _wrapper
```

### Comparing `cfg-argparser-1.2.0.post1/src/cfg_argparser/save_handlers.py` & `cfg-argparser-1.2.1/src/cfg_argparser/save_handlers.py`

 * *Files identical despite different names*

### Comparing `cfg-argparser-1.2.0.post1/src/cfg_argparser.egg-info/PKG-INFO` & `cfg-argparser-1.2.1/src/cfg_argparser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfg-argparser
-Version: 1.2.0.post1
+Version: 1.2.1
 Summary: A package designed to simplify configurable defaults from argparse.
 Author-email: Zeptofine <zeptofine@gmail.com>
 Project-URL: Homepage, https://github.com/zeptofine/cfg-argparser
 Project-URL: Bug Tracker, https://github.com/zeptofine/cfg-argparser/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 Provides-Extra: typer
 License-File: LICENSE
 
-# cfg_argparser 1.2.0
+# cfg_argparser 1.2.1
 
 a config wrapper I made.
 
 ## Installation
 
 ```bash
 # from pypi:
```

