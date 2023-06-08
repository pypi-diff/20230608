# Comparing `tmp/utilki-0.3.6.tar.gz` & `tmp/utilki-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.3.6.tar", max compression
+gzip compressed data, was "utilki-0.3.7.tar", max compression
```

## Comparing `utilki-0.3.6.tar` & `utilki-0.3.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.6/README.md
--rw-r--r--   0        0        0      525 2023-06-08 13:27:25.500395 utilki-0.3.6/pyproject.toml
--rw-r--r--   0        0        0      104 2023-06-08 13:29:56.115409 utilki-0.3.6/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.6/utilki/cli.py
--rw-r--r--   0        0        0     2653 2023-06-08 13:31:28.820562 utilki-0.3.6/utilki/progress.py
--rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.6/utilki/task_mixin.py
--rw-r--r--   0        0        0     1846 2023-06-08 13:31:38.343447 utilki-0.3.6/setup.py
--rw-r--r--   0        0        0     1608 2023-06-08 13:31:38.343642 utilki-0.3.6/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.7/README.md
+-rw-r--r--   0        0        0      525 2023-06-08 13:35:07.418527 utilki-0.3.7/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-08 13:29:56.115409 utilki-0.3.7/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.7/utilki/cli.py
+-rw-r--r--   0        0        0     2886 2023-06-08 13:34:52.736385 utilki-0.3.7/utilki/progress.py
+-rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.7/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-06-08 13:35:16.296691 utilki-0.3.7/setup.py
+-rw-r--r--   0        0        0     1608 2023-06-08 13:35:16.296922 utilki-0.3.7/PKG-INFO
```

### Comparing `utilki-0.3.6/README.md` & `utilki-0.3.7/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.3.6/pyproject.toml` & `utilki-0.3.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.3.6"
+version = "0.3.7"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.3.6/utilki/cli.py` & `utilki-0.3.7/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.6/utilki/progress.py` & `utilki-0.3.7/utilki/progress.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,17 @@
 from collections.abc import Iterable, Sized
 import logging
 from typing import Optional
 
 
+def set_default_logger_name(name: str):
+    global default_logger_name
+    default_logger_name = name
+
+
 class progress:
     def __init__(
         self,
         iterator: Iterable,
         name: str = "",
         print_idx: bool = False,
         num_steps: int = 10,
@@ -14,14 +19,17 @@
         logger_name: Optional[str] = None,
     ):
         if not isinstance(iterator, Iterable):
             raise ValueError("Passed object is not iterable")
         if not isinstance(iterator, Sized):
             raise ValueError("Passed object does not have a size")
 
+        if logger_name is None:
+            logger_name = default_logger_name
+
         self.logger = logging.getLogger(logger_name)
 
         self.print_idx = print_idx
         self.iterator = iter(iterator)
         self.len = len(iterator)
         self.name = name
         self.num_steps = num_steps
@@ -61,17 +69,19 @@
             self.index += 1
             return next(self.iterator)
 
 
 if __name__ == "__main__":
     import time
 
+    set_default_logger_name("progress")
+
     # setup basic logging format
     logging.basicConfig(
-        format="%(asctime)s %(levelname)s %(message)s",
+        format="%(asctime)s %(levelname)s %(name)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
         level=logging.INFO,
     )
 
     # too lazy rn to make a proper test suite
     for i in progress(range(101), name="test1"):
         time.sleep(0.001)
```

### Comparing `utilki-0.3.6/utilki/task_mixin.py` & `utilki-0.3.7/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.6/setup.py` & `utilki-0.3.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.3.6',
+    'version': '0.3.7',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.3.6/PKG-INFO` & `utilki-0.3.7/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.3.6
+Version: 0.3.7
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

