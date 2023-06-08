# Comparing `tmp/factorio-0.1.0.tar.gz` & `tmp/factorio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "factorio-0.1.0.tar", max compression
+gzip compressed data, was "factorio-0.2.0.tar", max compression
```

## Comparing `factorio-0.1.0.tar` & `factorio-0.2.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     7652 2023-02-24 22:22:14.728991 factorio-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0      610 2023-02-24 22:49:04.339406 factorio-0.1.0/README.rst
--rw-r--r--   0        0        0     2151 2023-02-24 22:49:04.341320 factorio-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-02-24 22:22:14.730638 factorio-0.1.0/src/factorio/__init__.py
--rw-r--r--   0        0        0      510 2023-02-24 22:49:04.337080 factorio-0.1.0/src/factorio/factories.py
--rw-r--r--   0        0        0     1388 2023-02-24 22:49:04.337958 factorio-0.1.0/src/factorio/fields.py
--rw-r--r--   0        0        0     1347 1970-01-01 00:00:00.000000 factorio-0.1.0/setup.py
--rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 factorio-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     7652 2023-03-10 22:07:08.021389 factorio-0.2.0/LICENSE.txt
+-rw-r--r--   0        0        0     1628 2023-04-27 20:50:15.037000 factorio-0.2.0/README.rst
+-rw-r--r--   0        0        0     2621 2023-06-08 15:36:26.218108 factorio-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-10 22:07:08.023760 factorio-0.2.0/src/factorio/__init__.py
+-rw-r--r--   0        0        0      539 2023-04-28 08:43:44.957572 factorio-0.2.0/src/factorio/factories.py
+-rw-r--r--   0        0        0     1667 2023-04-28 08:43:44.957758 factorio-0.2.0/src/factorio/fields.py
+-rw-r--r--   0        0        0        0 2023-03-10 22:07:08.033431 factorio-0.2.0/src/factorio/py.typed
+-rw-r--r--   0        0        0     2533 1970-01-01 00:00:00.000000 factorio-0.2.0/PKG-INFO
```

### Comparing `factorio-0.1.0/LICENSE.txt` & `factorio-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `factorio-0.1.0/pyproject.toml` & `factorio-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,102 +1,147 @@
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-target-version = ["py37", "py38", "py39", "py310", "py311"]
-
-[tool.isort]
-profile = "black"
-known_tests = "tests"
-sections = ["FUTURE", "STDLIB", "THIRDPARTY", "FIRSTPARTY", "TESTS"]
+target-version = ["py38"]
 
 [tool.mypy]
 check_untyped_defs = true
 disallow_any_generics = true
+disallow_incomplete_defs = true
+disallow_subclassing_any = true
+disallow_untyped_calls = true
+disallow_untyped_decorators = true
+disallow_untyped_defs = true
 ignore_missing_imports = true
 no_implicit_reexport = true
 show_error_codes = true
+strict_concatenate = true
+strict_equality = true
 warn_return_any = true
 warn_redundant_casts = true
 warn_unused_ignores = true
 warn_unreachable = true
 warn_unused_configs = true
 
-[tool.flake8]
-exclude = [
-    ".git",
-    "__pycache__",
-    ".venv",
-    ".cache",
+[tool.ruff]
+select = [
+    "A",
+    "ARG",
+    "B",
+    "BLE",
+    "C4",
+    "DTZ",
+    "E",
+    "ERA",
+    "EXE",
+    "F",
+    "FBT",
+    "G",
+    "I",
+    "INP",
+    "ISC",
+    "N",
+    "PGH",
+    "PIE",
+    "PLC",
+    "PLE",
+    "PLW",
+    "PT",
+    "PTH",
+    "RET",
+    "RSE",
+    "RUF",
+    "S",
+    "SIM",
+    "SLF",
+    "T10",
+    "TID",
+    "TRY",
+    "UP",
+    "W",
 ]
-max-line-length = 88
 ignore = [
-    "E203",
     "E501",
-    "W503",
+    "TRY003",
+]
+src = ["src"]
+target-version = "py38"
+
+[tool.ruff.per-file-ignores]
+"tests/**" = [
+    "FBT001",
+    "PT011",
+    "S101",
 ]
-banned-modules = """
-    mock = use unittest.mock
-    pytz = use zoneinfo
-"""
-ban-relative-imports = true
+
+[tool.ruff.flake8-tidy-imports]
+ban-relative-imports = "all"
+
+[tool.ruff.flake8-tidy-imports.banned-api]
+"mock".msg = "Use unittest.mock"
+"pytz".msg = "Use zoneinfo"
+
+[tool.ruff.isort]
+combine-as-imports = true
+forced-separate = ["tests"]
+split-on-trailing-comma = false
 
 [tool.pytest.ini_options]
-addopts = "-vv --cov --cov-report=term-missing:skip-covered"
+addopts = "-vv"
 testpaths = "tests"
 
 [tool.coverage.run]
 source = ["src/"]
+data_file = ".cov_cache/coverage.dat"
+
+[tool.coverage.report]
+show_missing = true
+skip_covered = true
+skip_empty = true
 
 [tool.poetry]
 name = "factorio"
-version = "0.1.0"
+version = "0.2.0"
 description = "A fixtures replacement tool"
 authors = [
     "Stephanos Kuma <stephanos@kuma.ai>",
 ]
 
 license = "LGPL-3.0+"
 readme = "README.rst"
 
+homepage = "https://factorio.readthedocs.io/en/stable/"
 repository = "https://github.com/spapanik/factorio"
+documentation = "https://factorio.readthedocs.io/en/stable/"
 
 keywords = ["tests"]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Operating System :: OS Independent",
 ]
 
 [tool.poetry.dependencies]
 # python version
-python = "^3.7"
+python = "^3.8"
 
 # dependencies
-Faker = "^17.0"
+Faker = "^18.0"
 
 [tool.poetry.group.dev.dependencies]
-ipdb = {version = "^0.13", python = "^3.10"}
-ipython = {version = "^8.9", python = "^3.10"}
-pipdeptree = "^2.3"
+ipdb = {version = "^0.13", python = "^3.9"}
+ipython = {version = "^8.12", python = "^3.9"}
+pipdeptree = "^2.7"
 
 [tool.poetry.group.lint.dependencies]
-black = "^23.1"
-flake8 = "^5.0"
-flake8-bugbear = "^23.1"
-flake8-builtins = "^2.0"
-flake8-comprehensions = "^3.10"
-flake8-eradicate = "^1.4"
-flake8-executable = "^2.1"
-flake8-mutable = "^1.2"
-Flake8-pyproject = "^1.2"
-flake8-tidy-imports = "^4.8"
-isort = {version = "^5.12", python = "^3.10"}
-mypy = "^1.0"
+black = "^23.3"
+mypy = "^1.2"
+ruff = "^0.0"
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.1"
+pytest = "^7.3"
 pytest-cov = "^4.0"
 
 [tool.poetry.group.docs.dependencies]
-sphinx = {version = "^6.1", python = "^3.10"}
-sphinx-rtd-theme = {version = "^1.2", python = "^3.10"}
+sphinx = "^6.2"
+sphinx-rtd-theme = "^1.2"
```

### Comparing `factorio-0.1.0/src/factorio/fields.py` & `factorio-0.2.0/src/factorio/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,44 @@
 from __future__ import annotations
 
-from typing import TYPE_CHECKING
+from secrets import choice
+from typing import TYPE_CHECKING, Any, Iterable, NoReturn
 
 from faker import Faker
 
 if TYPE_CHECKING:
     from factorio.factories import Factory
 
 _fake = Faker()
 
 ALIASES = {"int": "pyint"}
 
 
 class AbstractField:
-    def __call__(self):
+    def __call__(self) -> NoReturn:
         raise NotImplementedError("All concrete fields must be callable")
 
 
 class Field(AbstractField):
-    def __init__(self, type_: str, **kwargs):
+    def __init__(self, type_: str, **kwargs: Any):
         self.type = type_
         self.kwargs = kwargs
 
-    def __call__(self):
+    def __call__(self) -> Any:
         return getattr(_fake, ALIASES.get(self.type, self.type))(**self.kwargs)
 
 
+class ChoiceField(AbstractField):
+    def __init__(self, options: Iterable[Any]):
+        self.options = list(options)
+
+    def __call__(self) -> Any:
+        return choice(self.options)
+
+
 class CollectionField(AbstractField):
     def __init__(
         self,
         field: AbstractField,
         container: type,
         min_length: int | None = None,
         max_length: int | None = None,
@@ -39,18 +48,18 @@
         self.container = container
         if length is not None:
             min_length = length
             max_length = length
         self.min_length = min_length
         self.max_length = max_length
 
-    def __call__(self):
+    def __call__(self) -> Any:
         length = _fake.pyint(min_value=self.min_length, max_value=self.max_length)
         return self.container(self.field() for _ in range(length))
 
 
 class FactoryField(AbstractField):
     def __init__(self, factory: type[Factory]):
         self.factory = factory
 
-    def __call__(self):
+    def __call__(self) -> Any:
         return self.factory.build()
```

