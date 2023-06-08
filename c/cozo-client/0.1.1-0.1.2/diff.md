# Comparing `tmp/cozo_client-0.1.1.tar.gz` & `tmp/cozo_client-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cozo_client-0.1.1.tar", last modified: Wed May 31 08:51:04 2023, max compression
+gzip compressed data, was "cozo_client-0.1.2.tar", last modified: Thu Jun  8 17:46:32 2023, max compression
```

## Comparing `cozo_client-0.1.1.tar` & `cozo_client-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-31 08:51:04.006130 cozo_client-0.1.1/
--rw-r--r--   0 zh217      (501) staff       (20)     3098 2023-05-30 06:46:54.000000 cozo_client-0.1.1/.gitignore
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-05-31 08:51:04.005982 cozo_client-0.1.1/PKG-INFO
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-31 08:51:04.005055 cozo_client-0.1.1/cozo_client/
--rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.1/cozo_client/__init__.py
--rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.1/cozo_client/_builder.py
--rw-r--r--   0 zh217      (501) staff       (20)    22427 2023-05-31 08:19:07.000000 cozo_client-0.1.1/cozo_client/_client.py
-drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-05-31 08:51:04.005782 cozo_client-0.1.1/cozo_client.egg-info/
--rw-r--r--   0 zh217      (501) staff       (20)      304 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/PKG-INFO
--rw-r--r--   0 zh217      (501) staff       (20)      296 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/SOURCES.txt
--rw-r--r--   0 zh217      (501) staff       (20)        1 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/dependency_links.txt
--rw-r--r--   0 zh217      (501) staff       (20)       41 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/requires.txt
--rw-r--r--   0 zh217      (501) staff       (20)       12 2023-05-31 08:51:03.000000 cozo_client-0.1.1/cozo_client.egg-info/top_level.txt
--rw-r--r--   0 zh217      (501) staff       (20)      535 2023-05-31 08:08:04.000000 cozo_client-0.1.1/pyproject.toml
--rw-r--r--   0 zh217      (501) staff       (20)       40 2023-05-31 08:07:55.000000 cozo_client-0.1.1/requirements.txt
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-31 08:51:04.006177 cozo_client-0.1.1/setup.cfg
--rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.1/setup.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-08 17:46:32.233044 cozo_client-0.1.2/
+-rw-r--r--   0 zh217      (501) staff       (20)     3098 2023-05-30 06:46:54.000000 cozo_client-0.1.2/.gitignore
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-08 17:46:32.232909 cozo_client-0.1.2/PKG-INFO
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-08 17:46:32.231938 cozo_client-0.1.2/cozo_client/
+-rw-r--r--   0 zh217      (501) staff       (20)      464 2023-05-30 06:34:19.000000 cozo_client-0.1.2/cozo_client/__init__.py
+-rw-r--r--   0 zh217      (501) staff       (20)     7424 2023-05-30 06:27:28.000000 cozo_client-0.1.2/cozo_client/_builder.py
+-rw-r--r--   0 zh217      (501) staff       (20)    22686 2023-06-08 14:39:52.000000 cozo_client-0.1.2/cozo_client/_client.py
+drwxr-xr-x   0 zh217      (501) staff       (20)        0 2023-06-08 17:46:32.232748 cozo_client-0.1.2/cozo_client.egg-info/
+-rw-r--r--   0 zh217      (501) staff       (20)      304 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/PKG-INFO
+-rw-r--r--   0 zh217      (501) staff       (20)      296 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/SOURCES.txt
+-rw-r--r--   0 zh217      (501) staff       (20)        1 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/dependency_links.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       41 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/requires.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       12 2023-06-08 17:46:32.000000 cozo_client-0.1.2/cozo_client.egg-info/top_level.txt
+-rw-r--r--   0 zh217      (501) staff       (20)      535 2023-06-08 17:45:52.000000 cozo_client-0.1.2/pyproject.toml
+-rw-r--r--   0 zh217      (501) staff       (20)       40 2023-05-31 08:07:55.000000 cozo_client-0.1.2/requirements.txt
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-06-08 17:46:32.233086 cozo_client-0.1.2/setup.cfg
+-rw-r--r--   0 zh217      (501) staff       (20)       38 2023-05-20 12:04:30.000000 cozo_client-0.1.2/setup.py
```

### Comparing `cozo_client-0.1.1/.gitignore` & `cozo_client-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `cozo_client-0.1.1/cozo_client/_builder.py` & `cozo_client-0.1.2/cozo_client/_builder.py`

 * *Files identical despite different names*

### Comparing `cozo_client-0.1.1/cozo_client/_client.py` & `cozo_client-0.1.2/cozo_client/_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import hashlib
+import re
 from enum import Enum
 import logging
 import html
 import json
 from typing import Any, Generator, Union, Callable
 
 import requests
@@ -485,16 +486,25 @@
     def _embedded_request(self, script, params=None, immutable=False):
         try:
             res = self.embedded.run_script(script, params or {}, immutable)
         except Exception as e:
             raise QueryException(e.args[0])
         return CozoResponse(**res)
 
-    def run(self, script: str | InputProgram, params: dict[str, Any] | None = None, immutable=False) -> CozoResponse:
+    def run(self,
+            script: str | InputProgram,
+            params: dict[str, Any] | None = None,
+            replace: dict[str, str] | None = None,
+            immutable=False
+            ) -> CozoResponse:
         script = str(script)
+        if replace:
+            for k, v in replace.items():
+                r = r'\$\$' + k + r'\$\$'
+                script = re.sub(r, v, script)
         if self.is_remote:
             return self._client_request(script, params, immutable)
         else:
             return self._embedded_request(script, params, immutable)
 
     def export_relations(self, relations) -> dict[str, CozoResponse]:
         if not self.is_remote:
```

### Comparing `cozo_client-0.1.1/pyproject.toml` & `cozo_client-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,8 +17,8 @@
 ]
 dependencies = [
     "cozo-embedded",
     "requests",
     "pydantic",
     "openpyxl"
 ]
-version = "0.1.1"
+version = "0.1.2"
```

