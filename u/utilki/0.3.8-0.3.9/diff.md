# Comparing `tmp/utilki-0.3.8.tar.gz` & `tmp/utilki-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.3.8.tar", max compression
+gzip compressed data, was "utilki-0.3.9.tar", max compression
```

## Comparing `utilki-0.3.8.tar` & `utilki-0.3.9.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.8/README.md
--rw-r--r--   0        0        0      525 2023-06-08 13:55:01.954820 utilki-0.3.8/pyproject.toml
--rw-r--r--   0        0        0      150 2023-06-08 13:47:10.077945 utilki-0.3.8/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.8/utilki/cli.py
--rw-r--r--   0        0        0     3484 2023-06-08 13:54:38.692311 utilki-0.3.8/utilki/log_utils.py
--rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.8/utilki/task_mixin.py
--rw-r--r--   0        0        0     1846 2023-06-08 13:55:13.954187 utilki-0.3.8/setup.py
--rw-r--r--   0        0        0     1608 2023-06-08 13:55:13.954373 utilki-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.9/README.md
+-rw-r--r--   0        0        0      525 2023-06-08 14:09:32.883608 utilki-0.3.9/pyproject.toml
+-rw-r--r--   0        0        0      189 2023-06-08 14:09:19.007700 utilki-0.3.9/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.9/utilki/cli.py
+-rw-r--r--   0        0        0     3484 2023-06-08 13:54:38.692311 utilki-0.3.9/utilki/log_utils.py
+-rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.9/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-06-08 14:09:34.362990 utilki-0.3.9/setup.py
+-rw-r--r--   0        0        0     1608 2023-06-08 14:09:34.363186 utilki-0.3.9/PKG-INFO
```

### Comparing `utilki-0.3.8/README.md` & `utilki-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.3.8/pyproject.toml` & `utilki-0.3.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.3.8"
+version = "0.3.9"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.3.8/utilki/cli.py` & `utilki-0.3.9/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.8/utilki/log_utils.py` & `utilki-0.3.9/utilki/log_utils.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.8/utilki/task_mixin.py` & `utilki-0.3.9/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.8/setup.py` & `utilki-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.3.8',
+    'version': '0.3.9',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.3.8/PKG-INFO` & `utilki-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.3.8
+Version: 0.3.9
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

