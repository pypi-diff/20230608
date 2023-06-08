# Comparing `tmp/pymemuc-0.3.4.tar.gz` & `tmp/pymemuc-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymemuc-0.3.4.tar", max compression
+gzip compressed data, was "pymemuc-0.3.5.tar", max compression
```

## Comparing `pymemuc-0.3.4.tar` & `pymemuc-0.3.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1057 2023-06-06 18:09:50.890067 pymemuc-0.3.4/LICENSE
--rw-r--r--   0        0        0     1586 2023-06-06 18:09:50.890067 pymemuc-0.3.4/README.md
--rw-r--r--   0        0        0      386 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/__init__.py
--rw-r--r--   0        0        0    22761 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_command.py
--rw-r--r--   0        0        0      465 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_constants.py
--rw-r--r--   0        0        0     4984 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_control.py
--rw-r--r--   0        0        0     1214 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_decorators.py
--rw-r--r--   0        0        0    13670 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_manage.py
--rw-r--r--   0        0        0     4096 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/_memuc.py
--rw-r--r--   0        0        0      891 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/exceptions.py
--rw-r--r--   0        0        0     2899 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/pymemuc.py
--rw-r--r--   0        0        0      379 2023-06-06 18:09:50.894067 pymemuc-0.3.4/pymemuc/vminfo.py
--rw-r--r--   0        0        0     1665 2023-06-06 18:10:10.714555 pymemuc-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-06-08 18:30:14.192958 pymemuc-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1586 2023-06-08 18:30:14.192958 pymemuc-0.3.5/README.md
+-rw-r--r--   0        0        0      386 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/__init__.py
+-rw-r--r--   0        0        0    22761 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_command.py
+-rw-r--r--   0        0        0      465 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_constants.py
+-rw-r--r--   0        0        0     4984 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_control.py
+-rw-r--r--   0        0        0     1214 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_decorators.py
+-rw-r--r--   0        0        0    13670 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_manage.py
+-rw-r--r--   0        0        0     4134 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/_memuc.py
+-rw-r--r--   0        0        0      891 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/exceptions.py
+-rw-r--r--   0        0        0     2899 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/pymemuc.py
+-rw-r--r--   0        0        0      379 2023-06-08 18:30:14.196958 pymemuc-0.3.5/pymemuc/vminfo.py
+-rw-r--r--   0        0        0     1665 2023-06-08 18:30:40.189348 pymemuc-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2394 1970-01-01 00:00:00.000000 pymemuc-0.3.5/PKG-INFO
```

### Comparing `pymemuc-0.3.4/LICENSE` & `pymemuc-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/README.md` & `pymemuc-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pymemuc/_command.py` & `pymemuc-0.3.5/pymemuc/_command.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pymemuc/_control.py` & `pymemuc-0.3.5/pymemuc/_control.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pymemuc/_decorators.py` & `pymemuc-0.3.5/pymemuc/_decorators.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pymemuc/_manage.py` & `pymemuc-0.3.5/pymemuc/_manage.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pymemuc/_memuc.py` & `pymemuc-0.3.5/pymemuc/_memuc.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 """This module contains functions for directly interacting with memuc.exe."""
 from contextlib import suppress
 from os.path import join, normpath
-from subprocess import PIPE, STDOUT, CalledProcessError, Popen, TimeoutExpired
+from subprocess import PIPE, CalledProcessError, Popen, TimeoutExpired
 from typing import TYPE_CHECKING, Tuple
 
 from ._constants import WIN32, WINREG_EN
 from .exceptions import PyMemucError, PyMemucException, PyMemucTimeoutExpired
 
 if WINREG_EN:
     # pylint: disable=import-error
     from winreg import HKEY_LOCAL_MACHINE, ConnectRegistry, OpenKey, QueryValueEx
 
 ST_INFO = None
 if WIN32:
     from subprocess import (
         REALTIME_PRIORITY_CLASS,
         STARTF_USESHOWWINDOW,
+        STARTF_USESTDHANDLES,
         STARTUPINFO,
         SW_HIDE,
     )
 
     ST_INFO = STARTUPINFO()
-    ST_INFO.dwFlags |= STARTF_USESHOWWINDOW
-    ST_INFO.dwFlags |= REALTIME_PRIORITY_CLASS
+    ST_INFO.dwFlags |= (
+        STARTF_USESHOWWINDOW | STARTF_USESTDHANDLES | REALTIME_PRIORITY_CLASS
+    )
     ST_INFO.wShowWindow = SW_HIDE
 
 
 if TYPE_CHECKING:
     from pymemuc import PyMemuc
 
 
@@ -78,15 +80,15 @@
     self.logger.debug("pymemuc._memuc.memuc_run:")
     self.logger.debug(f"\tCommand: \"{' '.join(args)}\"")
     try:
         with Popen(
             args,
             shell=False,
             stdout=PIPE,
-            stderr=STDOUT,
+            stderr=PIPE,
             startupinfo=ST_INFO,
             close_fds=True,
             universal_newlines=True,
         ) as process:
             try:
                 result, _ = process.communicate(timeout=timeout)
             except TimeoutExpired as err:
```

### Comparing `pymemuc-0.3.4/pymemuc/exceptions.py` & `pymemuc-0.3.5/pymemuc/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pymemuc/pymemuc.py` & `pymemuc-0.3.5/pymemuc/pymemuc.py`

 * *Files identical despite different names*

### Comparing `pymemuc-0.3.4/pyproject.toml` & `pymemuc-0.3.5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "pymemuc"
-version = "v0.3.4"
+version = "v0.3.5"
 description = "A Memuc.exe wrapper for Python"
 readme = "README.md"
 authors = ["Martin Miglio <code@martinmiglio.dev>"]
 license = "MIT"
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `pymemuc-0.3.4/PKG-INFO` & `pymemuc-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymemuc
-Version: 0.3.4
+Version: 0.3.5
 Summary: A Memuc.exe wrapper for Python
 Home-page: https://github.com/martinmiglio/pymemuc
 License: MIT
 Keywords: memu,memuc,wrapper,api
 Author: Martin Miglio
 Author-email: code@martinmiglio.dev
 Requires-Python: >=3.9,<4.0
```

