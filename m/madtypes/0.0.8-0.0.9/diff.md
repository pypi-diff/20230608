# Comparing `tmp/madtypes-0.0.8.tar.gz` & `tmp/madtypes-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "madtypes-0.0.8.tar", last modified: Sun Jun  4 13:01:44 2023, max compression
+gzip compressed data, was "madtypes-0.0.9.tar", last modified: Thu Jun  8 08:51:31 2023, max compression
```

## Comparing `madtypes-0.0.8.tar` & `madtypes-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-04 13:01:44.505500 madtypes-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-04 13:01:33.000000 madtypes-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/madtypes/
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-04 13:01:33.000000 madtypes-0.0.8/madtypes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/madtypes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6793 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-04 13:01:44.000000 madtypes-0.0.8/madtypes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-04 13:01:44.505500 madtypes-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-04 13:01:33.000000 madtypes-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-04 13:01:44.505500 madtypes-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5604 2023-06-04 13:01:33.000000 madtypes-0.0.8/tests/test_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-06-04 13:01:33.000000 madtypes-0.0.8/tests/test_json_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:51:31.199551 madtypes-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-06-08 08:51:18.000000 madtypes-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-06-08 08:51:31.199551 madtypes-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-06-08 08:51:18.000000 madtypes-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:51:31.199551 madtypes-0.0.9/madtypes/
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-08 08:51:18.000000 madtypes-0.0.9/madtypes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:51:31.199551 madtypes-0.0.9/madtypes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7648 2023-06-08 08:51:31.000000 madtypes-0.0.9/madtypes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-08 08:51:31.000000 madtypes-0.0.9/madtypes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 08:51:31.000000 madtypes-0.0.9/madtypes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 08:51:31.000000 madtypes-0.0.9/madtypes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 08:51:31.199551 madtypes-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-08 08:51:18.000000 madtypes-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 08:51:31.199551 madtypes-0.0.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-08 08:51:18.000000 madtypes-0.0.9/tests/test_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8668 2023-06-08 08:51:18.000000 madtypes-0.0.9/tests/test_json_schema.py
```

### Comparing `madtypes-0.0.8/PKG-INFO` & `madtypes-0.0.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,61 @@
-Metadata-Version: 2.1
-Name: madtypes
-Version: 0.0.8
-Summary: Python typing that raise TypeError at runtime
-Home-page: https://github.com/6r17/madtypes
-Author: 6r17
-Author-email: patrick.borowy@proton.me
-Keywords: typing,json,json-schema
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-
 # madtypes
-- 💢 Python `Type` that raise TypeError at runtime
+- 💢 `MadType` is a Python metaclass that does type-validation at run-time.
 - 🌐 Generate [Json-Schema](https://json-schema.org/)
 - 📖 [Type hints cheat sheet](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html)
+- 💪 [32 tests](https://github.com/6r17/madtypes/blob/madmeta/tests/test_integrity.py) for the features and usage of MadType class
+- 💪 [18 tests](https://github.com/6r17/madtypes/blob/madmeta/tests/test_json_schema.py) for the features and usage of json-schema function
+
+- **[PEP589](https://peps.python.org/pep-0589/) does not perform type-checking.**
+> TypedDict type definitions could plausibly used to perform runtime type checking of dictionaries. For example, they could be used to validate that a JSON object conforms to the schema specified by a TypedDict type. This PEP doesn’t include such functionality, since the focus of this proposal is static type checking only, and other existing types do not support this, as discussed in Class-based syntax. Such functionality can be provided by a third-party library using the [typing_inspect](https://github.com/ilevkivskyi/typing_inspect) third-party module, for example.
+
 
 
 ```python
 
-def test_simple_dict_incorrect_setattr(): # Python default typing 🤯 DOES NOT RAISE ERROR 🤯
-    class Simple(dict):
+from typing import TypedDict
+from madtypes import MadType
+
+def test_simple_dict_incorrect_setattr(): # 🤯 DOES NOT RAISE ERROR 🤯
+    class Simple(TypedDict):
         name: str
 
     Simple(name=2)
-    a = Simple()
-    a.simple = 5
+    a: Simple = { "name": 2 }
 
 
 class Person(dict, metaclass=MadType): # 💢 MadType does !
     name: str
 
 
 def test_mad_dict_type_error_with_incorrect_creation():
     with pytest.raises(TypeError):
         Person(name=2)
 
 
 
 ```
-- 💪 [32 tests](https://github.com/6r17/madtypes/blob/madmeta/tests/test_integrity.py) proving the features and usage of MadType class
+
+
+|     [![Benchmark](https://github.com/6r17/madtypes/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/6r17/madtypes/actions/workflows/benchmark.yaml)               | Min   | Max   | Mean   | Min (+)        | Max (+)        | Mean (+)       |
+|----------------------------:|-------|-------|--------|----------------|----------------|----------------|
+| Correct instantiation      | 0.000 | 0.000 | 0.000  | 0.000 (18.1x) | 0.000 (23.8x) | 0.000 (17.3x) |
+| Incorrect instantiation    | 0.000 | 0.000 | 0.000  | 0.000 (2.6x) | 0.000 (3.7x) | 0.000 (2.9x) |
+
+
+- :warning: MadType instanciation is much slower than pure Python.
+- :warning: Manually adding type-check inside a class is more effective than using MadType
+
+
+**MadType is appropriate to apply when** :
+- The described data is a business related element
+- You are using MadType to assert valid data
+- You are debugging
+- The instantiation occurs rarely
+- The schema has to be communicated with the team
  
 - ### json-schema
 
 ```python
 
 def test_object_json_schema():
     class Item(dict, metaclass=MadType):
@@ -54,27 +64,29 @@
     assert json_schema(Item) == {
         "type": "object",
         "properties": {"name": {"type": "string"}},
         "required": ["name"],
     }
 ```
 
-- 💪 [18](https://github.com/6r17/madtypes/blob/madmeta/tests/test_json_schema.py) tests proving the features and usage of json-schema function.
 
-- ### 🔥 MadType attributes
+
+- ### Further customization
 It is possible to use the `MadType` metaclass customize primitives as well.
 
 ```python
 class SomeStringAttribute(str, metaclass=MadType):
    pass
 
 SomeDescriptedAttribute(2) # raise type error
 ```
 
-It is possible to use this to further describe a field.
+- ### Field description
+
+It is possible to use this to describe a field.
 
 ```python
 class SomeDescriptedAttribute(str, metaclass=MadType):
     annotation = str
     description = "Some description"
 ```
 
@@ -205,15 +217,15 @@
     FooBar(foo="foo", bar="bar")
     with pytest.raises(TypeError):
         FooBar()
 ```
 
 - ### Dynamicly remove a field
 
-Fields can be removed
+Fields can be removed.
 
 ```python
 
 
 def test_fields_can_be_removed():
     @subtract_fields("name")
     class Foo(dict, metaclass=MadType):
@@ -227,18 +239,7 @@
 [![pypi](https://img.shields.io/pypi/v/madtypes)](https://pypi.org/project/madtypes/)
 ![python: >3.10](https://img.shields.io/badge/python-%3E3.10-informational)
 ### Installation
 
 ```bash
 pip3 install madtypes
 ```
-
-- ### Context
-`madtypes` is a Python3.9+ library that provides enhanced data type checking capabilities. It offers features beyond the scope of [PEP 589](https://peps.python.org/pep-0589/) and is built toward an industrial use-case that require reliability.
-
-- The library introduces a Schema class that allows you to define classes with strict type enforcement. By inheriting from Schema, you can specify the expected data structure and enforce type correctness at runtime. If an incorrect type is assigned to an attribute, madtypes raises a TypeError.
-
-- Schema class and it's attributes inherit from `dict`. Attributes are considered values of the dictionnary.
-
-- It renders natively to `JSON`, facilitating data serialization and interchange.
-
-- The library also includes a `json_schema()` function that generates JSON-Schema representations based on class definitions.
```

### Comparing `madtypes-0.0.8/madtypes/__init__.py` & `madtypes-0.0.9/madtypes/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,28 @@
     ) in getattr(annotation, "__args__", ())
 
 
 def remove_optional(typing_annotation):
     return get_args(typing_annotation)[0]
 
 
-def type_check(value, annotation):
+def type_check(value, annotation, prev_optional: bool = False):
     origin = get_origin(annotation)
     args = get_args(annotation)
 
+    if prev_optional and value is None:
+        return True
     if origin is None:
         # Non-generic type
         return isinstance(value, annotation)
     elif origin is list or origin is set or origin is Union:
         # typing.Union cannot be used by is_instance
         if is_optional_type(annotation):
             inner_annotation = args[0]
-            return type_check(value, inner_annotation)
+            return type_check(value, inner_annotation, prev_optional=True)
         elif isinstance(value, origin):
             if args:
                 # Parametrized list annotation
                 inner_annotation = args[0]
                 return all(
                     type_check(item, inner_annotation) for item in value
                 )
@@ -110,14 +112,18 @@
     def typecheck_primitive_initialization(method):
         """Decorator for string.__init__"""
 
         def wrapper(self, *values, **key_values):
             if method != DOES_NOTHING:
                 method(*values, **key_values)
             else:
+                if _type_ == list:
+                    self.extend(*values)
+                elif _type_ == set:
+                    self.update(*values)
                 if (
                     (_type_ == str or _type_ == bytes)
                     and getattr(self, "pattern", False)
                     and (
                         not values[0]
                         or not re.fullmatch(
                             getattr(self, "pattern"), values[0]
@@ -126,35 +132,38 @@
                 ):
                     if len(values) != 0:
                         raise TypeError(
                             f"{values[0]} did not match {self.pattern}"
                         )
 
                 annotation = self.annotation if self.annotation else _type_
-                if len(values) == 0:
+                if len(values) == 0 or values[0] == None:
                     if is_optional_type(annotation):
                         _type_.__init__(None)
                     else:
                         raise TypeError(
-                            "Value mandatory for annotation {annotation}"
+                            f"Value mandatory for annotation {annotation}"
                         )
                 elif not type_check(values[0], annotation):
                     raise TypeError(
-                        "Value `{values[0]}` is not compatible with `{annotation}`"
+                        f"Value `{values[0]}` is not compatible with `{annotation}`"
                     )
 
         return wrapper
 
     return typecheck_primitive_initialization
 
 
 def __getattr__(self, name):
     if name in self:
         return self[name]
-    return super(self.__class__).__getattribute__(name)
+    try:
+        return super(self.__class__).__getattribute__(name)
+    except AttributeError:
+        return None
 
 
 def __setattr__(self, name, value):
     if not type_check(value, self.__annotations__[name]):
         raise TypeError(
             f"value `{value}` does not fit {self.__annotations__[name]} for key {name}"
         )
```

### Comparing `madtypes-0.0.8/madtypes.egg-info/PKG-INFO` & `madtypes-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,77 @@
 Metadata-Version: 2.1
 Name: madtypes
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python typing that raise TypeError at runtime
 Home-page: https://github.com/6r17/madtypes
 Author: 6r17
 Author-email: patrick.borowy@proton.me
 Keywords: typing,json,json-schema
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 # madtypes
-- 💢 Python `Type` that raise TypeError at runtime
+- 💢 `MadType` is a Python metaclass that does type-validation at run-time.
 - 🌐 Generate [Json-Schema](https://json-schema.org/)
 - 📖 [Type hints cheat sheet](https://mypy.readthedocs.io/en/stable/cheat_sheet_py3.html)
+- 💪 [32 tests](https://github.com/6r17/madtypes/blob/madmeta/tests/test_integrity.py) for the features and usage of MadType class
+- 💪 [18 tests](https://github.com/6r17/madtypes/blob/madmeta/tests/test_json_schema.py) for the features and usage of json-schema function
+
+- **[PEP589](https://peps.python.org/pep-0589/) does not perform type-checking.**
+> TypedDict type definitions could plausibly used to perform runtime type checking of dictionaries. For example, they could be used to validate that a JSON object conforms to the schema specified by a TypedDict type. This PEP doesn’t include such functionality, since the focus of this proposal is static type checking only, and other existing types do not support this, as discussed in Class-based syntax. Such functionality can be provided by a third-party library using the [typing_inspect](https://github.com/ilevkivskyi/typing_inspect) third-party module, for example.
+
 
 
 ```python
 
-def test_simple_dict_incorrect_setattr(): # Python default typing 🤯 DOES NOT RAISE ERROR 🤯
-    class Simple(dict):
+from typing import TypedDict
+from madtypes import MadType
+
+def test_simple_dict_incorrect_setattr(): # 🤯 DOES NOT RAISE ERROR 🤯
+    class Simple(TypedDict):
         name: str
 
     Simple(name=2)
-    a = Simple()
-    a.simple = 5
+    a: Simple = { "name": 2 }
 
 
 class Person(dict, metaclass=MadType): # 💢 MadType does !
     name: str
 
 
 def test_mad_dict_type_error_with_incorrect_creation():
     with pytest.raises(TypeError):
         Person(name=2)
 
 
 
 ```
-- 💪 [32 tests](https://github.com/6r17/madtypes/blob/madmeta/tests/test_integrity.py) proving the features and usage of MadType class
+
+
+|     [![Benchmark](https://github.com/6r17/madtypes/actions/workflows/benchmark.yaml/badge.svg)](https://github.com/6r17/madtypes/actions/workflows/benchmark.yaml)               | Min   | Max   | Mean   | Min (+)        | Max (+)        | Mean (+)       |
+|----------------------------:|-------|-------|--------|----------------|----------------|----------------|
+| Correct instantiation      | 0.000 | 0.000 | 0.000  | 0.000 (18.1x) | 0.000 (23.8x) | 0.000 (17.3x) |
+| Incorrect instantiation    | 0.000 | 0.000 | 0.000  | 0.000 (2.6x) | 0.000 (3.7x) | 0.000 (2.9x) |
+
+
+- :warning: MadType instanciation is much slower than pure Python.
+- :warning: Manually adding type-check inside a class is more effective than using MadType
+
+
+**MadType is appropriate to apply when** :
+- The described data is a business related element
+- You are using MadType to assert valid data
+- You are debugging
+- The instantiation occurs rarely
+- The schema has to be communicated with the team
  
 - ### json-schema
 
 ```python
 
 def test_object_json_schema():
     class Item(dict, metaclass=MadType):
@@ -54,27 +80,29 @@
     assert json_schema(Item) == {
         "type": "object",
         "properties": {"name": {"type": "string"}},
         "required": ["name"],
     }
 ```
 
-- 💪 [18](https://github.com/6r17/madtypes/blob/madmeta/tests/test_json_schema.py) tests proving the features and usage of json-schema function.
 
-- ### 🔥 MadType attributes
+
+- ### Further customization
 It is possible to use the `MadType` metaclass customize primitives as well.
 
 ```python
 class SomeStringAttribute(str, metaclass=MadType):
    pass
 
 SomeDescriptedAttribute(2) # raise type error
 ```
 
-It is possible to use this to further describe a field.
+- ### Field description
+
+It is possible to use this to describe a field.
 
 ```python
 class SomeDescriptedAttribute(str, metaclass=MadType):
     annotation = str
     description = "Some description"
 ```
 
@@ -205,15 +233,15 @@
     FooBar(foo="foo", bar="bar")
     with pytest.raises(TypeError):
         FooBar()
 ```
 
 - ### Dynamicly remove a field
 
-Fields can be removed
+Fields can be removed.
 
 ```python
 
 
 def test_fields_can_be_removed():
     @subtract_fields("name")
     class Foo(dict, metaclass=MadType):
@@ -227,18 +255,7 @@
 [![pypi](https://img.shields.io/pypi/v/madtypes)](https://pypi.org/project/madtypes/)
 ![python: >3.10](https://img.shields.io/badge/python-%3E3.10-informational)
 ### Installation
 
 ```bash
 pip3 install madtypes
 ```
-
-- ### Context
-`madtypes` is a Python3.9+ library that provides enhanced data type checking capabilities. It offers features beyond the scope of [PEP 589](https://peps.python.org/pep-0589/) and is built toward an industrial use-case that require reliability.
-
-- The library introduces a Schema class that allows you to define classes with strict type enforcement. By inheriting from Schema, you can specify the expected data structure and enforce type correctness at runtime. If an incorrect type is assigned to an attribute, madtypes raises a TypeError.
-
-- Schema class and it's attributes inherit from `dict`. Attributes are considered values of the dictionnary.
-
-- It renders natively to `JSON`, facilitating data serialization and interchange.
-
-- The library also includes a `json_schema()` function that generates JSON-Schema representations based on class definitions.
```

### Comparing `madtypes-0.0.8/setup.py` & `madtypes-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="madtypes",
-    version="0.0.8",
+    version="0.0.9",
     author="6r17",
     author_email="patrick.borowy@proton.me",
     description="Python typing that raise TypeError at runtime",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/6r17/madtypes",
     packages=find_packages(include=["madtypes"]),
```

### Comparing `madtypes-0.0.8/tests/test_integrity.py` & `madtypes-0.0.9/tests/test_integrity.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import json
 import pytest
 from typing import Optional
 from madtypes import MadType, subtract_fields
 from enum import Enum
+from typing import TypedDict
 
 
 def test_simple_dict_incorrect_setattr():
-    class Simple(dict):
+    class Simple(TypedDict):
         name: str
 
     Simple(name=2)
-    a = Simple()
-    a.simple = 5
+    a: Simple = {"name": 2}
 
 
 class Person(dict, metaclass=MadType):
     name: str
 
 
 def test_mad_dict_type_error_with_incorrect_creation():
@@ -69,14 +69,15 @@
 
 
 def test_mad_dict_is_ok_with_optional_type():
     Opt()
     opt = Opt(name="foo")
     assert opt["name"] == "foo"
     assert opt.name == "foo"
+    Opt(name=None)
 
 
 def test_mad_dict_type_error__with_erronous_optional_type():
     with pytest.raises(TypeError):
         Opt(name=2)
 
 
@@ -110,34 +111,48 @@
         annotation = Optional[_type_]
 
     SomeType()
 
 
 @pytest.mark.parametrize(
     "value",
-    [(str, "correct"), (int, 2), (float, 2.4), (bytes, b"hello")],
-    ids=["string", "int", "float", "bytes"],
+    [
+        (str, "correct"),
+        (int, 2),
+        (float, 2.4),
+        (bytes, b"hello"),
+        (list, [1]),
+        (set, {1}),
+    ],
+    ids=["string", "int", "float", "bytes", "list", "set"],
 )
 def test_correct_mad_primitive(value):
     _type_, correct = value
 
     class SomeType(_type_, metaclass=MadType):
         annotation = _type_
         description = f"{_type_}"
 
-    SomeType(correct)
+    assert SomeType(correct) == correct
 
     with pytest.raises(TypeError):
         SomeType()
 
 
 @pytest.mark.parametrize(
     "value",
-    [(str, 2), (int, "2"), (float, "2"), (bytes, "incorrect")],
-    ids=["string", "int", "float", "bytes"],
+    [
+        (str, 2),
+        (int, "2"),
+        (float, "2"),
+        (bytes, "incorrect"),
+        (list, "incorrect"),
+        (set, "incorrect"),
+    ],
+    ids=["string", "int", "float", "bytes", "list", "set"],
 )
 def test_incorrect_mad_primitive(value):
     _type_, incorrect = value
 
     class SomeType(_type_, metaclass=MadType):
         annotation = _type_
         description = f"{_type_}"
```

### Comparing `madtypes-0.0.8/tests/test_json_schema.py` & `madtypes-0.0.9/tests/test_json_schema.py`

 * *Files identical despite different names*

