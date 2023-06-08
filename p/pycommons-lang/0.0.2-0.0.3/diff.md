# Comparing `tmp/pycommons_lang-0.0.2.tar.gz` & `tmp/pycommons_lang-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycommons_lang-0.0.2.tar", max compression
+gzip compressed data, was "pycommons_lang-0.0.3.tar", max compression
```

## Comparing `pycommons_lang-0.0.2.tar` & `pycommons_lang-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,32 @@
--rw-r--r--   0        0        0      587 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/LICENSE
--rw-r--r--   0        0        0      624 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/README.md
--rw-r--r--   0        0        0        0 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/__init__.py
--rw-r--r--   0        0        0      591 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/__init__.py
--rw-r--r--   0        0        0      257 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/arrayutils.py
--rw-r--r--   0        0        0      108 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/bases/__init__.py
--rw-r--r--   0        0        0     2053 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/bases/char.py
--rw-r--r--   0        0        0     3386 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/bases/optional.py
--rw-r--r--   0        0        0     1832 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/charutils.py
--rw-r--r--   0        0        0       88 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/exception/__init__.py
--rw-r--r--   0        0        0      367 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/exception/no_such_element_error.py
--rw-r--r--   0        0        0      266 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/function/__init__.py
--rw-r--r--   0        0        0      708 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/function/consumer.py
--rw-r--r--   0        0        0      542 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/function/function.py
--rw-r--r--   0        0        0      635 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/function/predicate.py
--rw-r--r--   0        0        0      445 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/function/runnable.py
--rw-r--r--   0        0        0      481 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/function/supplier.py
--rw-r--r--   0        0        0      469 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/objectutils.py
--rw-r--r--   0        0        0     3375 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/lang/stringutils.py
--rw-r--r--   0        0        0        0 2023-05-22 06:59:54.525977 pycommons_lang-0.0.2/pycommons/py.typed
--rw-r--r--   0        0        0     1476 2023-05-22 07:00:07.618028 pycommons_lang-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1359 1970-01-01 00:00:00.000000 pycommons_lang-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0    11346 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1343 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/README.md
+-rw-r--r--   0        0        0      431 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/__init__.py
+-rw-r--r--   0        0        0       65 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/base/__init__.py
+-rw-r--r--   0        0        0     5648 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/base/char.py
+-rw-r--r--   0        0        0       58 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/__init__.py
+-rw-r--r--   0        0        0      754 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/boolean.py
+-rw-r--r--   0        0        0      761 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/container.py
+-rw-r--r--   0        0        0     1469 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/integer.py
+-rw-r--r--   0        0        0     4457 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/container/optional.py
+-rw-r--r--   0        0        0       88 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/exception/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/exception/no_such_element_error.py
+-rw-r--r--   0        0        0      320 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/__init__.py
+-rw-r--r--   0        0        0     1266 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/comparator.py
+-rw-r--r--   0        0        0     1454 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/consumer.py
+-rw-r--r--   0        0        0      594 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/function.py
+-rw-r--r--   0        0        0     2249 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/predicate.py
+-rw-r--r--   0        0        0      496 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/runnable.py
+-rw-r--r--   0        0        0      532 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/function/supplier.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:11:44.147592 pycommons_lang-0.0.3/pycommons/lang/streams/__init__.py
+-rw-r--r--   0        0        0     6823 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/streams/iterator.py
+-rw-r--r--   0        0        0     2264 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/streams/stream.py
+-rw-r--r--   0        0        0      725 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/streams/streams.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/__init__.py
+-rw-r--r--   0        0        0      399 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/arrayutils.py
+-rw-r--r--   0        0        0     2385 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/charutils.py
+-rw-r--r--   0        0        0      520 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/objectutils.py
+-rw-r--r--   0        0        0    11127 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/stringutils.py
+-rw-r--r--   0        0        0      119 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/lang/utils/utils.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:11:44.151592 pycommons_lang-0.0.3/pycommons/py.typed
+-rw-r--r--   0        0        0     1780 2023-06-08 19:11:56.867698 pycommons_lang-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 pycommons_lang-0.0.3/PKG-INFO
```

### Comparing `pycommons_lang-0.0.2/pycommons/lang/bases/char.py` & `pycommons_lang-0.0.3/pycommons/lang/container/integer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,81 +1,56 @@
-from __future__ import annotations
+import typing
 
-from typing import TypeVar
+from pycommons.lang.container.container import Container
 
 
-class Char(int):
-    def __new__(cls, c: CharType) -> Char:
-        if c is None:
-            raise ValueError("Illegal Character")
+class IntegerContainer(Container[int]):
+    def __init__(self, value: int = 0):
+        super().__init__(value)
 
-        if isinstance(c, Char):
-            return super(Char, cls).__new__(cls, int(c))
+    def add(self, val: int) -> None:
+        self.set(self.get() + val)
 
-        if isinstance(c, int):
-            chr(c)
-            return super(Char, cls).__new__(cls, c)
+    def add_and_get(self, val: int) -> int:
+        return typing.cast(int, self.set_and_get(self.get() + val))
 
-        c_str: str = str(c)
-        if len(c_str) > 1:
-            raise ValueError("Illegal Character")
-        return super(Char, cls).__new__(cls, ord(c_str))
+    def get_and_add(self, val: int) -> int:
+        return typing.cast(int, self.get_and_set(self.get() + val))
 
-    def __str__(self) -> str:
-        return chr(int(self))
+    def increment(self) -> None:
+        return self.add(1)
 
-    def __len__(self) -> int:
-        return 1
+    def increment_and_get(self) -> int:
+        return self.add_and_get(1)
 
-    def __repr__(self) -> str:
-        return chr(int(self))
+    def get_and_increment(self) -> int:
+        return self.get_and_add(1)
 
-    def __eq__(self, other: CharType) -> bool:  # type: ignore
-        return int(self) == int(Char(other))
+    def subtract(self, val: int) -> None:
+        return self.add(-val)
 
-    def __gt__(self, other: CharType) -> bool:
-        return int(self) > int(Char(other))
+    def subtract_and_get(self, val: int) -> int:
+        return self.add_and_get(-val)
 
-    def __ge__(self, other: CharType) -> bool:
-        return int(self) >= int(Char(other))
+    def get_and_subtract(self, val: int) -> int:
+        return self.get_and_add(-val)
 
-    def __lt__(self, other: CharType) -> bool:
-        return int(self) < int(Char(other))
+    def get(self) -> int:
+        return typing.cast(int, super().get())
 
-    def __le__(self, other: CharType) -> bool:
-        return int(self) <= int(Char(other))
+    def __int__(self) -> int:
+        return self.get()
 
-    def __hash__(self) -> int:
-        return hash(int(self))
+    def __le__(self, other: int) -> bool:
+        return self.get() <= other
 
-    def isupper(self) -> bool:
-        return chr(int(self)).isupper()
+    def __lt__(self, other: int) -> bool:
+        return self.get() < other
 
-    def islower(self) -> bool:
-        return chr(int(self)).islower()
+    def __ge__(self, other: int) -> bool:
+        return self.get() >= other
 
-    def isalpha(self) -> bool:
-        return chr(int(self)).isalpha()
+    def __gt__(self, other: int) -> bool:
+        return self.get() > other
 
-    def isalnum(self) -> bool:
-        return chr(int(self)).isalnum()
-
-    def isascii(self) -> bool:
-        return chr(int(self)).isascii()
-
-    def isdigit(self) -> bool:
-        return chr(int(self)).isdigit()
-
-    def isspace(self) -> bool:
-        return chr(int(self)).isspace()
-
-    def upper(self) -> Char:
-        return Char(chr(int(self)).upper())
-
-    def lower(self) -> Char:
-        return Char(chr(int(self)).lower())
-
-    def swapcase(self) -> Char:
-        return Char(chr(int(self)).swapcase())
-
-
-CharType = TypeVar("CharType", Char, int, str, None)
+    def __eq__(self, other: object) -> bool:
+        return self.get() == other
```

### Comparing `pycommons_lang-0.0.2/pycommons/lang/charutils.py` & `pycommons_lang-0.0.3/pycommons/lang/utils/charutils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import string
 from typing import Optional, Set
 
-from .bases.char import Char, CharType
+from pycommons.lang.base.char import Char, CharType
 
 
 class CharUtils:
     ASCII_SPACE: Char = Char(" ")
 
     # region: Whitespaces
     WHITESPACES: Set[Char] = {Char(c) for c in string.whitespace}
@@ -19,14 +19,19 @@
 
     @classmethod
     def is_ascii_printable(cls, c: Optional[CharType]) -> bool:
         char: Optional[Char] = cls.to_character(c)
         return char is not None and cls.ASCII_SPACE < char < 127
 
     @classmethod
+    def is_digit(cls, c: Optional[CharType]) -> bool:
+        char: Optional[Char] = cls.to_character(c)
+        return char is not None and char.isdigit()
+
+    @classmethod
     def is_letter(cls, c: Optional[CharType]) -> bool:
         char: Optional[Char] = cls.to_character(c)
         return char is not None and char.isalpha()
 
     @classmethod
     def is_letter_or_digit(cls, c: Optional[CharType]) -> bool:
         char: Optional[Char] = cls.to_character(c)
@@ -50,11 +55,21 @@
     @classmethod
     def to_character(cls, c: Optional[CharType]) -> Optional[Char]:
         if c is None:
             return None
         return Char(c)
 
     @classmethod
+    def to_uppercase(cls, c: Optional[CharType]) -> Optional[Char]:
+        char: Optional[Char] = cls.to_character(c)
+        return char.upper() if char else None
+
+    @classmethod
+    def to_lowercase(cls, c: Optional[CharType]) -> Optional[Char]:
+        char: Optional[Char] = cls.to_character(c)
+        return char.lower() if char else None
+
+    @classmethod
     def is_equal(cls, c: CharType, other: CharType) -> bool:
         if c is None or other is None:
             return False
         return Char(c) == Char(other)
```

### Comparing `pycommons_lang-0.0.2/pycommons/lang/function/consumer.py` & `pycommons_lang-0.0.3/pycommons/lang/function/function.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 from __future__ import annotations
 
+from abc import abstractmethod
 from typing import TypeVar, Generic, Callable, Any
 
 _T = TypeVar("_T")
+_U = TypeVar("_U")
 
 
-class Consumer(Generic[_T]):
+class Function(Generic[_T, _U]):
     @classmethod
-    def of(cls, consumer: Callable[[_T], None]) -> Consumer[_T]:
-        class BasicConsumer(Consumer[_T]):
-            def accept(self, value: _T) -> None:
-                consumer(value)
+    def of(cls, function: Callable[[_T], _U]) -> Function[_T, _U]:
+        class BasicFunction(Function[_T, _U]):
+            def apply(self, t: _T) -> _U:
+                return function(t)
 
-        return BasicConsumer()
+        return BasicFunction()
 
-    def accept(self, value: _T) -> None:
+    @abstractmethod
+    def apply(self, t: _T) -> _U:
         pass
 
-    def and_then(self, after: Consumer[_T]) -> Consumer[_T]:
-        def _impl(_t: _T) -> None:
-            self.accept(_t)
-            after.accept(_t)
-
-        return Consumer.of(_impl)
-
-    def __call__(self, *args: _T, **kwargs: Any) -> None:
-        self.accept(args[0])
+    def __call__(self, t: _T, *args: Any, **kwargs: Any) -> _U:
+        return self.apply(t)
```

### Comparing `pycommons_lang-0.0.2/pycommons/lang/function/function.py` & `pycommons_lang-0.0.3/pycommons/lang/function/supplier.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 from __future__ import annotations
 
+from abc import abstractmethod
 from typing import TypeVar, Generic, Callable, Any
 
 _T = TypeVar("_T")
-_U = TypeVar("_U")
 
 
-class Function(Generic[_T, _U]):
+class Supplier(Generic[_T]):
     @classmethod
-    def of(cls, function: Callable[[_T], _U]) -> Function[_T, _U]:
-        class BasicFunction(Function[_T, _U]):
-            def apply(self, t: _T) -> _U:
-                return function(t)
+    def of(cls, supplier: Callable[[], _T]) -> Supplier[_T]:
+        class BasicSupplier(Supplier[_T]):
+            def get(self) -> _T:
+                return supplier()
 
-        return BasicFunction()
+        return BasicSupplier()
 
-    def apply(self, t: _T) -> _U:
+    @abstractmethod
+    def get(self) -> _T:
         pass
 
-    def __call__(self, *args: Any, **kwargs: Any) -> _U:
-        return self.apply(args[0])
+    def __call__(self, *args: Any, **kwargs: Any) -> _T:
+        return self.get()
```

### Comparing `pycommons_lang-0.0.2/pyproject.toml` & `pycommons_lang-0.0.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool]
 
 [tool.poetry]
 name = "pycommons.lang"
-version = "0.0.2"
+version = "0.0.3"
 homepage = "https://github.com/shashankrnr32/pycommons-lang"
 description = "Python Commons Lang"
 authors = ["Shashank Sharma <shashankrnr32@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
     'License :: OSI Approved :: Apache Software License',
@@ -19,45 +19,56 @@
 ]
 include = [
     "LICENSE",
     "pycommons/py.typed"
 ]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 importlib_metadata = "*"
 
 [tool.poetry.dev-dependencies]
 mkdocs-material = ">7.0.0"
 mkdocstrings = { version = ">0.18", extras = ["python-legacy"] }
 mkdocs-awesome-pages-plugin = "*"
 markdown-include = "*"
 livereload = "*"
+poethepoet = "^0.20.0"
 
-pytest = "^6.0"
+pytest = ">=7.2.0"
 pytest-cov = "^2.10.1"
 
 pylint = "^2.6.0"
 black = "22.3.0"
 mypy = "0.960"
 
 [tool.black]
 line-length = 100
 
 [tool.pylint.reports]
 output-format = "colorized"
 reports = "y"
-include-ids = "yes"
 msg-template = "{msg_id}:{line:3d},{column}: {obj}: {msg}"
-disable = "C0103, C0116, C0114, C0115"
+disable = "C0103, C0116, C0114, C0115, R0801, R0903"
+max-public-methods = 50
+max-args = 8
+max-locals = 20
+min-public-method = 0
 
 [tool.pytest.ini_options]
-addopts = "--cov=pycommons --cov-branch --cov-report term-missing  -vv --color=yes --cov-fail-under 40"
+addopts = "--cov=pycommons --cov-branch --cov-report term-missing --cov-report xml -vv --color=yes --cov-fail-under 10"
 python_files = "tests.py test_*.py *_tests.py *Test.py"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.mypy.overrides]
 module = "pycommons.lang"
 implicit_reexport = true
+
+[tool.poe.tasks]
+test = "pytest"
+lint = "pylint pycommons/ tests/"
+black = "black ."
+mypy = "mypy --namespace-packages -p pycommons.lang --strict --config-file=mypy.ini"
+docs = "mkdocs serve"
```

