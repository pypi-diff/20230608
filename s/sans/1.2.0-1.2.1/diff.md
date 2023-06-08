# Comparing `tmp/sans-1.2.0.tar.gz` & `tmp/sans-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sans-1.2.0.tar", last modified: Sun Jun  4 22:58:05 2023, max compression
+gzip compressed data, was "sans-1.2.1.tar", last modified: Thu Jun  8 04:59:34 2023, max compression
```

## Comparing `sans-1.2.0.tar` & `sans-1.2.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.938731 sans-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.922731 sans-1.2.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.926731 sans-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-04 22:57:54.000000 sans-1.2.0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-04 22:57:54.000000 sans-1.2.0/.github/workflows/pythonpublish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-04 22:57:54.000000 sans-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-04 22:57:54.000000 sans-1.2.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-04 22:57:54.000000 sans-1.2.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-04 22:57:54.000000 sans-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-04 22:58:05.934731 sans-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-04 22:57:54.000000 sans-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.934731 sans-1.2.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-04 22:57:54.000000 sans-1.2.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-04 22:57:54.000000 sans-1.2.0/docs/auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-04 22:57:54.000000 sans-1.2.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-04 22:57:54.000000 sans-1.2.0/docs/errors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-04 22:57:54.000000 sans-1.2.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-04 22:57:54.000000 sans-1.2.0/docs/limiter.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-04 22:57:54.000000 sans-1.2.0/docs/lock.rst
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-04 22:57:54.000000 sans-1.2.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-04 22:57:54.000000 sans-1.2.0/docs/response.rst
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-04 22:57:54.000000 sans-1.2.0/docs/url.rst
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-04 22:57:54.000000 sans-1.2.0/docs/utils.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-04 22:57:54.000000 sans-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-04 22:57:54.000000 sans-1.2.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.934731 sans-1.2.0/sans/
--rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-06-04 22:57:54.000000 sans-1.2.0/sans/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-04 22:57:54.000000 sans-1.2.0/sans/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-06-04 22:57:54.000000 sans-1.2.0/sans/_lock.py
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-04 22:57:54.000000 sans-1.2.0/sans/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-04 22:57:54.000000 sans-1.2.0/sans/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    27979 2023-06-04 22:57:54.000000 sans-1.2.0/sans/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-04 22:57:54.000000 sans-1.2.0/sans/decoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-04 22:57:54.000000 sans-1.2.0/sans/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-06-04 22:57:54.000000 sans-1.2.0/sans/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-04 22:57:54.000000 sans-1.2.0/sans/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-04 22:57:54.000000 sans-1.2.0/sans/response.py
--rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-04 22:57:54.000000 sans-1.2.0/sans/url.py
--rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-04 22:57:54.000000 sans-1.2.0/sans/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 22:58:05.934731 sans-1.2.0/sans.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-04 22:58:05.000000 sans-1.2.0/sans.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 22:58:05.938731 sans-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-04 22:57:54.000000 sans-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:34.710212 sans-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:34.698211 sans-1.2.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:34.702211 sans-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2805 2023-06-08 04:59:22.000000 sans-1.2.1/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-08 04:59:22.000000 sans-1.2.1/.github/workflows/pythonpublish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3101 2023-06-08 04:59:22.000000 sans-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-06-08 04:59:22.000000 sans-1.2.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-08 04:59:22.000000 sans-1.2.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-08 04:59:22.000000 sans-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-08 04:59:34.706212 sans-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-06-08 04:59:22.000000 sans-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:34.706212 sans-1.2.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 04:59:22.000000 sans-1.2.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-08 04:59:22.000000 sans-1.2.1/docs/auth.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6127 2023-06-08 04:59:22.000000 sans-1.2.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-08 04:59:22.000000 sans-1.2.1/docs/errors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-06-08 04:59:22.000000 sans-1.2.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 04:59:22.000000 sans-1.2.1/docs/limiter.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 04:59:22.000000 sans-1.2.1/docs/lock.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-08 04:59:22.000000 sans-1.2.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 04:59:22.000000 sans-1.2.1/docs/response.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 04:59:22.000000 sans-1.2.1/docs/url.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 04:59:22.000000 sans-1.2.1/docs/utils.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-08 04:59:22.000000 sans-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-06-08 04:59:22.000000 sans-1.2.1/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:34.706212 sans-1.2.1/sans/
+-rw-r--r--   0 runner    (1001) docker     (123)     3689 2023-06-08 04:59:22.000000 sans-1.2.1/sans/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6862 2023-06-08 04:59:22.000000 sans-1.2.1/sans/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-08 04:59:22.000000 sans-1.2.1/sans/_lock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-08 04:59:22.000000 sans-1.2.1/sans/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-08 04:59:22.000000 sans-1.2.1/sans/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27979 2023-06-08 04:59:22.000000 sans-1.2.1/sans/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-08 04:59:22.000000 sans-1.2.1/sans/decoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-06-08 04:59:22.000000 sans-1.2.1/sans/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14295 2023-06-08 04:59:22.000000 sans-1.2.1/sans/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:22.000000 sans-1.2.1/sans/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3232 2023-06-08 04:59:22.000000 sans-1.2.1/sans/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-08 04:59:22.000000 sans-1.2.1/sans/url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3641 2023-06-08 04:59:22.000000 sans-1.2.1/sans/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 04:59:34.706212 sans-1.2.1/sans.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6519 2023-06-08 04:59:34.000000 sans-1.2.1/sans.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-06-08 04:59:34.000000 sans-1.2.1/sans.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 04:59:34.000000 sans-1.2.1/sans.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 04:59:34.000000 sans-1.2.1/sans.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 04:59:34.000000 sans-1.2.1/sans.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 04:59:34.000000 sans-1.2.1/sans.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 04:59:34.710212 sans-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-08 04:59:22.000000 sans-1.2.1/setup.py
```

### Comparing `sans-1.2.0/.github/workflows/codeql-analysis.yml` & `sans-1.2.1/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/.github/workflows/pythonpublish.yml` & `sans-1.2.1/.github/workflows/pythonpublish.yml`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/.gitignore` & `sans-1.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/.pre-commit-config.yaml` & `sans-1.2.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/LICENSE` & `sans-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/PKG-INFO` & `sans-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.2.0
+Version: 1.2.1
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sans-1.2.0/README.md` & `sans-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/docs/Makefile` & `sans-1.2.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/docs/conf.py` & `sans-1.2.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/docs/make.bat` & `sans-1.2.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/pyproject.toml` & `sans-1.2.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/__main__.py` & `sans-1.2.1/sans/__main__.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/_lock.py` & `sans-1.2.1/sans/_lock.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,21 +164,14 @@
         return acquire()
 
     def __exit__(self, *_):
         self.release()
 
     @property
     def deferred(self) -> float | None:
-        """
-        Returns when the lock is scheduled to be released in seconds from now,
-        or None if the lock isn't deferred.
-
-        Note that this is only the *schedule* - the value could be
-        0.0 or even negative if the deferring thread falls behind.
-        """
         if self.__deferred:
             return time.monotonic() - self.__deferred.when()
         # return None
 
     _deferred = property(deferred.fget)
 
     @_deferred.setter
```

### Comparing `sans-1.2.0/sans/auth.py` & `sans-1.2.1/sans/auth.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/client.py` & `sans-1.2.1/sans/client.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/client.pyi` & `sans-1.2.1/sans/client.pyi`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/decoder.py` & `sans-1.2.1/sans/decoder.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/errors.py` & `sans-1.2.1/sans/errors.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/limiter.py` & `sans-1.2.1/sans/limiter.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/response.py` & `sans-1.2.1/sans/response.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/url.py` & `sans-1.2.1/sans/url.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans/utils.py` & `sans-1.2.1/sans/utils.py`

 * *Files identical despite different names*

### Comparing `sans-1.2.0/sans.egg-info/PKG-INFO` & `sans-1.2.1/sans.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sans
-Version: 1.2.0
+Version: 1.2.1
 Summary: Synchronous / Asynchronous HTTPX extension for NationStates
 Author: Zephyrkul
 License: MIT License
         
         Copyright (c) 2018 - 2023
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sans-1.2.0/sans.egg-info/SOURCES.txt` & `sans-1.2.1/sans.egg-info/SOURCES.txt`

 * *Files identical despite different names*

