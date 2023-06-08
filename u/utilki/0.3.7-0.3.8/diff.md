# Comparing `tmp/utilki-0.3.7.tar.gz` & `tmp/utilki-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.3.7.tar", max compression
+gzip compressed data, was "utilki-0.3.8.tar", max compression
```

## Comparing `utilki-0.3.7.tar` & `utilki-0.3.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.7/README.md
--rw-r--r--   0        0        0      525 2023-06-08 13:35:07.418527 utilki-0.3.7/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-08 13:29:56.115409 utilki-0.3.7/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.7/utilki/cli.py
--rw-r--r--   0        0        0     2886 2023-06-08 13:34:52.736385 utilki-0.3.7/utilki/progress.py
--rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.7/utilki/task_mixin.py
--rw-r--r--   0        0        0     1846 2023-06-08 13:35:16.296691 utilki-0.3.7/setup.py
--rw-r--r--   0        0        0     1608 2023-06-08 13:35:16.296922 utilki-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.8/README.md
+-rw-r--r--   0        0        0      525 2023-06-08 13:55:01.954820 utilki-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-08 13:47:10.077945 utilki-0.3.8/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.8/utilki/cli.py
+-rw-r--r--   0        0        0     3484 2023-06-08 13:54:38.692311 utilki-0.3.8/utilki/log_utils.py
+-rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.8/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-06-08 13:55:13.954187 utilki-0.3.8/setup.py
+-rw-r--r--   0        0        0     1608 2023-06-08 13:55:13.954373 utilki-0.3.8/PKG-INFO
```

### Comparing `utilki-0.3.7/README.md` & `utilki-0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.3.7/pyproject.toml` & `utilki-0.3.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.3.7"
+version = "0.3.8"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.3.7/utilki/cli.py` & `utilki-0.3.8/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.7/utilki/progress.py` & `utilki-0.3.8/utilki/log_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,35 @@
 from collections.abc import Iterable, Sized
 import logging
-from typing import Optional
+from typing import Callable, Optional
 
 
 def set_default_logger_name(name: str):
-    global default_logger_name
-    default_logger_name = name
+    global _logger_name
+    _logger_name = name
+
+
+def set_use_print(use_print: bool):
+    global _use_print
+    _use_print = use_print
+
+
+def set_callback(callback: Callable):
+    global _callback
+    _callback = callback
+
+
+def log(message: str):
+    global _logger_name
+    global _callback
+    if _use_print:
+        print(f"{message}", flush=True)
+    logging.getLogger(_logger_name).info(message)
+    if _callback:
+        _callback(message)
 
 
 class progress:
     def __init__(
         self,
         iterator: Iterable,
         name: str = "",
@@ -20,15 +40,16 @@
     ):
         if not isinstance(iterator, Iterable):
             raise ValueError("Passed object is not iterable")
         if not isinstance(iterator, Sized):
             raise ValueError("Passed object does not have a size")
 
         if logger_name is None:
-            logger_name = default_logger_name
+            global _logger_name
+            logger_name = _logger_name
 
         self.logger = logging.getLogger(logger_name)
 
         self.print_idx = print_idx
         self.iterator = iter(iterator)
         self.len = len(iterator)
         self.name = name
@@ -94,7 +115,17 @@
         precision=3,
         logger_name="lmao",
     ):
         time.sleep(0.001)
 
     for idx, i in enumerate(progress(["a", "b", "c"], name="test3")):
         time.sleep(0.001)
+
+    def rev(msg):
+        print(msg[::-1])
+        pass
+
+    set_use_print(True)
+    set_default_logger_name("ayy")
+    set_callback(rev)
+    # log("\n\n")
+    log("hello world")
```

### Comparing `utilki-0.3.7/utilki/task_mixin.py` & `utilki-0.3.8/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.7/setup.py` & `utilki-0.3.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.3.7',
+    'version': '0.3.8',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.3.7/PKG-INFO` & `utilki-0.3.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.3.7
+Version: 0.3.8
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

