# Comparing `tmp/utilki-0.3.5.tar.gz` & `tmp/utilki-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "utilki-0.3.5.tar", max compression
+gzip compressed data, was "utilki-0.3.6.tar", max compression
```

## Comparing `utilki-0.3.5.tar` & `utilki-0.3.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.5/README.md
--rw-r--r--   0        0        0      525 2023-06-08 13:24:23.102557 utilki-0.3.5/pyproject.toml
--rw-r--r--   0        0        0       73 2023-04-06 19:12:02.029197 utilki-0.3.5/utilki/__init__.py
--rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.5/utilki/cli.py
--rw-r--r--   0        0        0     2622 2023-06-08 13:24:13.036969 utilki-0.3.5/utilki/progress.py
--rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.5/utilki/task_mixin.py
--rw-r--r--   0        0        0     1846 2023-06-08 13:24:39.933231 utilki-0.3.5/setup.py
--rw-r--r--   0        0        0     1608 2023-06-08 13:24:39.933530 utilki-0.3.5/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-04-07 14:14:58.660919 utilki-0.3.6/README.md
+-rw-r--r--   0        0        0      525 2023-06-08 13:27:25.500395 utilki-0.3.6/pyproject.toml
+-rw-r--r--   0        0        0      104 2023-06-08 13:29:56.115409 utilki-0.3.6/utilki/__init__.py
+-rw-r--r--   0        0        0     2184 2023-04-28 13:17:26.918133 utilki-0.3.6/utilki/cli.py
+-rw-r--r--   0        0        0     2653 2023-06-08 13:31:28.820562 utilki-0.3.6/utilki/progress.py
+-rw-r--r--   0        0        0     7028 2023-06-06 14:34:33.311112 utilki-0.3.6/utilki/task_mixin.py
+-rw-r--r--   0        0        0     1846 2023-06-08 13:31:38.343447 utilki-0.3.6/setup.py
+-rw-r--r--   0        0        0     1608 2023-06-08 13:31:38.343642 utilki-0.3.6/PKG-INFO
```

### Comparing `utilki-0.3.5/README.md` & `utilki-0.3.6/README.md`

 * *Files identical despite different names*

### Comparing `utilki-0.3.5/pyproject.toml` & `utilki-0.3.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "utilki"
-version = "0.3.5"
+version = "0.3.6"
 description = "A collection of useful utilities"
 readme = "README.md"
 authors = ["Khaidar Bikmaev <khaidar@bikmaev.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.7"
 click = "^8.1.3"
```

### Comparing `utilki-0.3.5/utilki/cli.py` & `utilki-0.3.6/utilki/cli.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.5/utilki/progress.py` & `utilki-0.3.6/utilki/progress.py`

 * *Files 7% similar despite different names*

```diff
@@ -41,15 +41,14 @@
                 percent_str = f"{int(percent):d}%"
             self.map[index] = percent_str
 
         self.indices = set(self.map.keys())
         self.index = 0
         self.index_len = len(str(self.len))
         self.percent_len = max([len(p) for p in self.map.values()])
-        self.logger.info(f"{self.index_len=}, {self.percent_len=}")
 
     def __iter__(self):
         return self
 
     def __next__(self):
         if self.index in self.indices:
             msg = f"{self.name} {self.map[self.index]:>{self.percent_len}}"
@@ -70,19 +69,22 @@
     logging.basicConfig(
         format="%(asctime)s %(levelname)s %(message)s",
         datefmt="%Y-%m-%d %H:%M:%S",
         level=logging.INFO,
     )
 
     # too lazy rn to make a proper test suite
-    for i in progress(range(101), name="test"):
+    for i in progress(range(101), name="test1"):
         time.sleep(0.001)
 
     for i in progress(
         range(7),
-        name="test",
+        name="test2",
         print_idx=True,
         num_steps=11,
         precision=3,
         logger_name="lmao",
     ):
         time.sleep(0.001)
+
+    for idx, i in enumerate(progress(["a", "b", "c"], name="test3")):
+        time.sleep(0.001)
```

### Comparing `utilki-0.3.5/utilki/task_mixin.py` & `utilki-0.3.6/utilki/task_mixin.py`

 * *Files identical despite different names*

### Comparing `utilki-0.3.5/setup.py` & `utilki-0.3.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 ['click>=8.1.3,<9.0.0', 'pydantic>=1.10.7,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['utilki = utilki.cli:cli']}
 
 setup_kwargs = {
     'name': 'utilki',
-    'version': '0.3.5',
+    'version': '0.3.6',
     'description': 'A collection of useful utilities',
     'long_description': '# utilki\n\n[![codecov](https://codecov.io/gh/realbikmaev/utilki/branch/main/graph/badge.svg?token=VN0UMT7O9A)](https://codecov.io/gh/realbikmaev/utilki)\n\nutils that are frequently used by me and might be useful for others\n\n## installation\n\n```bash\npip install utilki\n```\n\n## TaskMixin\n\nMixin class that adds `create()` classmethod to dataclass you define as your task params. Useful when you have a lot of container based tasks executed on remote clusters (e.g. Kubernetes, Hashicorp Nomad, etc.). It reads task params from environment variables, parses, and validates them. \n\n```python\nfrom utilki import TaskMixin\n\n@dataclass\nclass Task(TaskMixin):\n    ayy: float = 69.69\n    lmao: str = "420"\n\nos.environ["ayy"] = "42.42"\nos.environ["lmao"] = "69"\n\nt = Task.create()\nprint(f"ayy: {t.ayy}, type: {type(t.ayy)}")\n# ayy: 42.42, type: <class \'float\'>\nprint(f"lmao: {t.lmao}, type: {type(t.lmao)}")\n# lmao: 69, type: <class \'str\'>\n```\n\n## Cli\n\n### Venv\n\n```bash\n$ utilki venv 3.8.10\n$ Enter venv name: new_venv\n$ Created venv `new_venv` with Python version 3.8.10\n```',
     'author': 'Khaidar Bikmaev',
     'author_email': 'khaidar@bikmaev.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': None,
```

### Comparing `utilki-0.3.5/PKG-INFO` & `utilki-0.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: utilki
-Version: 0.3.5
+Version: 0.3.6
 Summary: A collection of useful utilities
 Author: Khaidar Bikmaev
 Author-email: khaidar@bikmaev.com
 Requires-Python: >=3.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
```

