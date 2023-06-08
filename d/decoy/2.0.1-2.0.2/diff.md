# Comparing `tmp/decoy-2.0.1.tar.gz` & `tmp/decoy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "decoy-2.0.1.tar", max compression
+gzip compressed data, was "decoy-2.0.2.tar", max compression
```

## Comparing `decoy-2.0.1.tar` & `decoy-2.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1075 2023-03-21 23:26:27.299118 decoy-2.0.1/LICENSE
--rw-r--r--   0        0        0     5972 2023-03-21 23:26:27.299118 decoy-2.0.1/README.md
--rw-r--r--   0        0        0    11261 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/__init__.py
--rw-r--r--   0        0        0     1511 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/call_handler.py
--rw-r--r--   0        0        0     1286 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/context_managers.py
--rw-r--r--   0        0        0     5829 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/core.py
--rw-r--r--   0        0        0     2893 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/errors.py
--rw-r--r--   0        0        0     9915 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/matchers.py
--rw-r--r--   0        0        0       85 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/mypy/__init__.py
--rw-r--r--   0        0        0     1358 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/mypy/plugin.py
--rw-r--r--   0        0        0        0 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/py.typed
--rw-r--r--   0        0        0      852 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/pytest_plugin.py
--rw-r--r--   0        0        0     7596 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/spy.py
--rw-r--r--   0        0        0     7203 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/spy_core.py
--rw-r--r--   0        0        0     2382 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/spy_events.py
--rw-r--r--   0        0        0     3886 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/spy_log.py
--rw-r--r--   0        0        0     2243 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/stringify.py
--rw-r--r--   0        0        0     1743 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/stub_store.py
--rw-r--r--   0        0        0      403 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/types.py
--rw-r--r--   0        0        0     1638 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/verifier.py
--rw-r--r--   0        0        0     2755 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/warning_checker.py
--rw-r--r--   0        0        0     2985 2023-03-21 23:26:27.299118 decoy-2.0.1/decoy/warnings.py
--rw-r--r--   0        0        0     2360 2023-03-21 23:26:27.303118 decoy-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 decoy-2.0.1/setup.py
--rw-r--r--   0        0        0     7067 1970-01-01 00:00:00.000000 decoy-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-08 15:41:57.075245 decoy-2.0.2/LICENSE
+-rw-r--r--   0        0        0     5972 2023-06-08 15:41:57.075245 decoy-2.0.2/README.md
+-rw-r--r--   0        0        0    11261 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/__init__.py
+-rw-r--r--   0        0        0     1511 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/call_handler.py
+-rw-r--r--   0        0        0     1286 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/context_managers.py
+-rw-r--r--   0        0        0     5829 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/core.py
+-rw-r--r--   0        0        0     2893 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/errors.py
+-rw-r--r--   0        0        0     9895 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/matchers.py
+-rw-r--r--   0        0        0       85 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/mypy/__init__.py
+-rw-r--r--   0        0        0     1358 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/mypy/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-08 15:41:57.075245 decoy-2.0.2/decoy/py.typed
+-rw-r--r--   0        0        0      852 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/pytest_plugin.py
+-rw-r--r--   0        0        0     7596 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/spy.py
+-rw-r--r--   0        0        0     7203 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/spy_core.py
+-rw-r--r--   0        0        0     2382 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/spy_events.py
+-rw-r--r--   0        0        0     3886 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/spy_log.py
+-rw-r--r--   0        0        0     2243 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/stringify.py
+-rw-r--r--   0        0        0     1743 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/stub_store.py
+-rw-r--r--   0        0        0      403 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/types.py
+-rw-r--r--   0        0        0     1638 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/verifier.py
+-rw-r--r--   0        0        0     2756 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/warning_checker.py
+-rw-r--r--   0        0        0     2985 2023-06-08 15:41:57.079241 decoy-2.0.2/decoy/warnings.py
+-rw-r--r--   0        0        0     2374 2023-06-08 15:41:57.079241 decoy-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     6794 1970-01-01 00:00:00.000000 decoy-2.0.2/setup.py
+-rw-r--r--   0        0        0     7067 1970-01-01 00:00:00.000000 decoy-2.0.2/PKG-INFO
```

### Comparing `decoy-2.0.1/LICENSE` & `decoy-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/README.md` & `decoy-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/__init__.py` & `decoy-2.0.2/decoy/__init__.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/call_handler.py` & `decoy-2.0.2/decoy/call_handler.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/context_managers.py` & `decoy-2.0.2/decoy/context_managers.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/core.py` & `decoy-2.0.2/decoy/core.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/errors.py` & `decoy-2.0.2/decoy/errors.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/matchers.py` & `decoy-2.0.2/decoy/matchers.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return matches_type and matches_attrs
 
     def __repr__(self) -> str:
         """Return a string representation of the matcher."""
         if self._attributes is None:
             return f"<IsA {self._match_type.__name__}>"
         else:
-            return f"<IsA {self._match_type.__name__} {repr(self._attributes)}>"
+            return f"<IsA {self._match_type.__name__} {self._attributes!r}>"
 
 
 def IsA(match_type: type, attributes: Optional[Mapping[str, Any]] = None) -> Any:
     """Match anything that satisfies the passed in type.
 
     Arguments:
         match_type: Type to match.
@@ -122,15 +122,15 @@
 
     def __eq__(self, target: object) -> bool:
         """Return true if target is not self._reject_value."""
         return target != self._reject_value
 
     def __repr__(self) -> str:
         """Return a string representation of the matcher."""
-        return f"<IsNot {repr(self._reject_value)}>"
+        return f"<IsNot {self._reject_value!r}>"
 
 
 def IsNot(value: object) -> Any:
     """Match anything that isn't the passed in value.
 
     Arguments:
         value: Value to check against.
@@ -160,15 +160,15 @@
                     hasattr(target, attr_name) and getattr(target, attr_name) == value
                 )
 
         return is_match
 
     def __repr__(self) -> str:
         """Return a string representation of the matcher."""
-        return f"<HasAttributes {repr(self._attributes)}>"
+        return f"<HasAttributes {self._attributes!r}>"
 
 
 def HasAttributes(attributes: Mapping[str, Any]) -> Any:
     """Match anything with the passed in attributes.
 
     Arguments:
         attributes: Attribute values to check.
@@ -203,15 +203,15 @@
                 except TypeError:
                     is_match = False
 
         return is_match
 
     def __repr__(self) -> str:
         """Return a string representation of the matcher."""
-        return f"<DictMatching {repr(self._values)}>"
+        return f"<DictMatching {self._values!r}>"
 
 
 def DictMatching(values: Mapping[str, Any]) -> Any:
     """Match any dictionary with the passed in keys / values.
 
     Arguments:
         values: Keys and values to check.
@@ -234,15 +234,15 @@
 
     def __eq__(self, target: object) -> bool:
         """Return true if target is not self._reject_value."""
         return isinstance(target, str) and self._pattern.search(target) is not None
 
     def __repr__(self) -> str:
         """Return a string representation of the matcher."""
-        return f"<StringMatching {repr(self._pattern.pattern)}>"
+        return f"<StringMatching {self._pattern.pattern!r}>"
 
 
 def StringMatching(match: str) -> str:
     """Match any string matching the passed in pattern.
 
     Arguments:
         match: Pattern to check against; will be compiled into an re.Pattern.
```

### Comparing `decoy-2.0.1/decoy/mypy/plugin.py` & `decoy-2.0.2/decoy/mypy/plugin.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/pytest_plugin.py` & `decoy-2.0.2/decoy/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/spy.py` & `decoy-2.0.2/decoy/spy.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/spy_core.py` & `decoy-2.0.2/decoy/spy_core.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/spy_events.py` & `decoy-2.0.2/decoy/spy_events.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,20 +79,20 @@
         and rehearsal.payload.ignore_extra_args
     ):
         call = event.payload
         rehearsed_call = rehearsal.payload
 
         try:
             args_match = all(
-                call.args[i] == value for i, value in enumerate(rehearsed_call.args)
+                value == call.args[i] for i, value in enumerate(rehearsed_call.args)
             )
             kwargs_match = all(
-                call.kwargs[key] == value
+                value == call.kwargs[key]
                 for key, value in rehearsed_call.kwargs.items()
             )
 
             return args_match and kwargs_match
 
         except (IndexError, KeyError):
             return False
 
-    return event.payload == rehearsal.payload
+    return rehearsal.payload == event.payload
```

### Comparing `decoy-2.0.1/decoy/spy_log.py` & `decoy-2.0.2/decoy/spy_log.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/stringify.py` & `decoy-2.0.2/decoy/stringify.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/stub_store.py` & `decoy-2.0.2/decoy/stub_store.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/verifier.py` & `decoy-2.0.2/decoy/verifier.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/decoy/warning_checker.py` & `decoy-2.0.2/decoy/warning_checker.py`

 * *Files 1% similar despite different names*

```diff
@@ -67,10 +67,11 @@
     when_rehearsals = [c for c in all_calls if isinstance(c, WhenRehearsal)]
     verify_rehearsals = [c for c in all_calls if isinstance(c, VerifyRehearsal)]
 
     for vr in verify_rehearsals:
         if any(wr for wr in when_rehearsals if wr == vr):
             _warn(RedundantVerifyWarning(rehearsal=vr))
 
+
 def _warn(warning: DecoyWarning) -> None:
     """Trigger a warning, at the stack level of whatever called `Decoy.reset`."""
     warn(warning, stacklevel=6)
```

### Comparing `decoy-2.0.1/decoy/warnings.py` & `decoy-2.0.2/decoy/warnings.py`

 * *Files identical despite different names*

### Comparing `decoy-2.0.1/pyproject.toml` & `decoy-2.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "decoy"
-version = "2.0.1"
+version = "2.0.2"
 description = "Opinionated mocking library for Python"
 authors = ["Mike Cousins <mike@cousins.io>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mcous/decoy"
 homepage = "https://mike.cousins.io/decoy/"
 documentation = "https://mike.cousins.io/decoy/"
@@ -25,29 +25,29 @@
 python = "^3.7"
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
 coverage = { extras = ["toml"], version = "^7.1.0" }
 mkdocs = "^1.4.2"
 mkdocs-material = "^9.0.13"
-mkdocstrings = { extras = ["python"], version = "^0.20.0" }
+mkdocstrings = { extras = ["python"], version = ">=0.20,<0.23" }
 mypy = "^1.0.1"
-poethepoet = "^0.18.1"
+poethepoet = ">=0.18.1,<0.20.0"
 pytest = "^7.0.1"
-pytest-asyncio = "^0.20.3"
+pytest-asyncio = ">=0.20.3,<0.22.0"
 pytest-mypy-plugins = "^1.10.1"
 pytest-xdist = "^3.0.2"
-ruff = ">=0.0.247,<0.0.258"
+ruff = ">=0.0.247,<0.0.271"
 
 [tool.poe.tasks]
 all = [ "check", "lint", "format-check", "test-once", "coverage", "docs-build", "build" ]
 check = "mypy"
 lint = "ruff check ."
 format = "black ."
-format-check = { ref = "format --check" }
+format-check = "black . --check"
 test = "pytest -f"
 test-once = "coverage run --branch --source=decoy -m pytest --mypy-same-process"
 coverage = "coverage report"
 coverage-xml = "coverage xml"
 docs = "mkdocs serve"
 docs-build = "mkdocs build"
 build = "poetry build"
```

### Comparing `decoy-2.0.1/setup.py` & `decoy-2.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'pytest11': ['decoy = decoy.pytest_plugin']}
 
 setup_kwargs = {
     'name': 'decoy',
-    'version': '2.0.1',
+    'version': '2.0.2',
     'description': 'Opinionated mocking library for Python',
     'long_description': '<div align="center">\n    <img alt="Decoy logo" src="https://mike.cousins.io/decoy/img/decoy.png" width="256px">\n    <h1 class="decoy-title">Decoy</h1>\n    <p>Opinionated mocking library for Python</p>\n    <p>\n        <a title="CI Status" href="https://github.com/mcous/decoy/actions">\n        <img src="https://img.shields.io/github/actions/workflow/status/mcous/decoy/ci.yml?branch=main&style=flat-square"></a>\n        <a title="Code Coverage" href="https://app.codecov.io/gh/mcous/decoy/"><img src="https://img.shields.io/codecov/c/github/mcous/decoy?style=flat-square"></a>\n        <a title="License" href="https://github.com/mcous/decoy/blob/main/LICENSE"><img src="https://img.shields.io/github/license/mcous/decoy?style=flat-square"></a>\n        <a title="PyPI Version"href="https://pypi.org/project/decoy/"><img src="https://img.shields.io/pypi/v/decoy?style=flat-square"></a>\n        <a title="Supported Python Versions" href="https://pypi.org/project/decoy/"><img src="https://img.shields.io/pypi/pyversions/decoy?style=flat-square"></a>\n    </p>\n    <p>\n        <a href="https://mike.cousins.io/decoy/" class="decoy-hidden">Usage guide and documentation</a>\n    </p>\n</div>\n\nDecoy is a mocking library designed for **effective and productive test-driven development** in Python. If you want to use tests to guide the structure of your code, Decoy might be for you!\n\nDecoy mocks are **async/await** and **type-checking** friendly. Decoy is heavily inspired by (and/or stolen from) the excellent [testdouble.js][] and [Mockito][] projects. The Decoy API is powerful, easy to read, and strives to help you make good decisions about your code.\n\n## Install\n\n```bash\n# pip\npip install decoy\n\n# poetry\npoetry add --dev decoy\n\n# pipenv\npipenv install --dev decoy\n```\n\n## Setup\n\n### Pytest setup\n\nDecoy ships with its own [pytest][] plugin, so once Decoy is installed, you\'re ready to start using it via its pytest fixture, called `decoy`.\n\n```python\n# test_my_thing.py\nfrom decoy import Decoy\n\ndef test_my_thing_works(decoy: Decoy) -> None:\n    ...\n```\n\n### Mypy setup\n\nBy default, Decoy is compatible with Python [typing][] and type-checkers like [mypy][]. However, stubbing functions that return `None` can trigger a [type checking error](https://mypy.readthedocs.io/en/stable/error_code_list.html#check-that-called-function-returns-a-value-func-returns-value) during correct usage of the Decoy API. To suppress these errors, add Decoy\'s plugin to your mypy configuration.\n\n```ini\n# mypy.ini\nplugins = decoy.mypy\n```\n\n### Other testing libraries\n\nDecoy works well with [pytest][], but if you use another testing library or framework, you can still use Decoy! You just need to do two things:\n\n1. Create a new instance of [`Decoy()`](https://mike.cousins.io/decoy/api/#decoy.Decoy) before each test\n2. Call [`decoy.reset()`](https://mike.cousins.io/decoy/api/#decoy.Decoy.reset) after each test\n\nFor example, using the built-in [unittest][] framework, you would use the `setUp` fixture method to do `self.decoy = Decoy()` and the `tearDown` method to call `self.decoy.reset()`. For a working example, see [`tests/test_unittest.py`](https://github.com/mcous/decoy/blob/main/tests/test_unittest.py).\n\n## Basic Usage\n\nThis basic example assumes you are using [pytest][]. For more detailed documentation, see Decoy\'s [usage guide][] and [API reference][].\n\nDecoy will add a `decoy` fixture to pytest that provides its mock creation API.\n\n```python\nfrom decoy import Decoy\n\ndef test_something(decoy: Decoy) -> None:\n    ...\n```\n\n!!! note\n\n    Importing the `Decoy` interface for type annotations is recommended, but optional. If your project does not use type annotations, you can simply write:\n\n    ```python\n    def test_something(decoy):\n        ...\n    ```\n\n### Create a mock\n\nUse `decoy.mock` to create a mock based on some specification. From there, inject the mock into your test subject.\n\n```python\ndef test_add_todo(decoy: Decoy) -> None:\n    todo_store = decoy.mock(cls=TodoStore)\n    subject = TodoAPI(store=todo_store)\n    ...\n```\n\nSee [creating mocks][] for more details.\n\n### Stub a behavior\n\nUse `decoy.when` to configure your mock\'s behaviors. For example, you can set the mock to return a certain value when called in a certain way using `then_return`:\n\n```python\ndef test_add_todo(decoy: Decoy) -> None:\n    """Adding a todo should create a TodoItem in the TodoStore."""\n    todo_store = decoy.mock(cls=TodoStore)\n    subject = TodoAPI(store=todo_store)\n\n    decoy.when(\n        todo_store.add(name="Write a test for adding a todo")\n    ).then_return(\n        TodoItem(id="abc123", name="Write a test for adding a todo")\n    )\n\n    result = subject.add("Write a test for adding a todo")\n    assert result == TodoItem(id="abc123", name="Write a test for adding a todo")\n```\n\nSee [stubbing with when][] for more details.\n\n### Verify a call\n\nUse `decoy.verify` to assert that a mock was called in a certain way. This is best used with dependencies that are being used for their side-effects and don\'t return a useful value.\n\n```python\ndef test_remove_todo(decoy: Decoy) -> None:\n    """Removing a todo should remove the item from the TodoStore."""\n    todo_store = decoy.mock(cls=TodoStore)\n    subject = TodoAPI(store=todo_store)\n\n    subject.remove("abc123")\n\n    decoy.verify(todo_store.remove(id="abc123"), times=1)\n```\n\nSee [spying with verify][] for more details.\n\n[testdouble.js]: https://github.com/testdouble/testdouble.js\n[mockito]: https://site.mockito.org/\n[pytest]: https://docs.pytest.org/\n[unittest]: https://docs.python.org/3/library/unittest.html\n[typing]: https://docs.python.org/3/library/typing.html\n[mypy]: https://mypy.readthedocs.io/\n[api reference]: https://mike.cousins.io/decoy/api/\n[usage guide]: https://mike.cousins.io/decoy/usage/create/\n[creating mocks]: https://mike.cousins.io/decoy/usage/create/\n[stubbing with when]: https://mike.cousins.io/decoy/usage/when/\n[spying with verify]: https://mike.cousins.io/decoy/usage/verify/\n',
     'author': 'Mike Cousins',
     'author_email': 'mike@cousins.io',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://mike.cousins.io/decoy/',
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['decoy',
 'decoy.mypy'] package_data = \ {'': ['*']} entry_points = \ {'pytest11':
 ['decoy = decoy.pytest_plugin']} setup_kwargs = { 'name': 'decoy', 'version':
-'2.0.1', 'description': 'Opinionated mocking library for Python',
+'2.0.2', 'description': 'Opinionated mocking library for Python',
 'long_description': '
                                \n [Decoy logo]\n
                               ****** Decoy ******
                                       \n
                     Opinionated mocking library for Python
                                       \n
    \n \n_[https://img.shields.io/github/actions/workflow/status/mcous/decoy/
```

### Comparing `decoy-2.0.1/PKG-INFO` & `decoy-2.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: decoy
-Version: 2.0.1
+Version: 2.0.2
 Summary: Opinionated mocking library for Python
 Home-page: https://mike.cousins.io/decoy/
 License: MIT
 Author: Mike Cousins
 Author-email: mike@cousins.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

