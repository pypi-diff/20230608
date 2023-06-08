# Comparing `tmp/tortoise_orm_stubs-0.4.4.tar.gz` & `tmp/tortoise_orm_stubs-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tortoise_orm_stubs-0.4.4.tar", max compression
+gzip compressed data, was "tortoise_orm_stubs-1.0.0.tar", max compression
```

## Comparing `tortoise_orm_stubs-0.4.4.tar` & `tortoise_orm_stubs-1.0.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1072 2022-09-22 00:21:21.676040 tortoise_orm_stubs-0.4.4/LICENSE
--rw-r--r--   0        0        0      511 2023-06-07 05:51:08.893037 tortoise_orm_stubs-0.4.4/README.md
--rw-r--r--   0        0        0     1060 2023-06-08 15:37:52.483459 tortoise_orm_stubs-0.4.4/pyproject.toml
--rw-r--r--   0        0        0    13409 2023-06-08 15:37:29.840125 tortoise_orm_stubs-0.4.4/tortoise-stubs/fields/__init__.pyi
--rw-r--r--   0        0        0        8 2022-09-22 19:51:35.803221 tortoise_orm_stubs-0.4.4/tortoise-stubs/py.typed
--rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 tortoise_orm_stubs-0.4.4/setup.py
--rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 tortoise_orm_stubs-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2022-09-22 00:21:21.676040 tortoise_orm_stubs-1.0.0/LICENSE
+-rw-r--r--   0        0        0      511 2023-04-25 17:47:14.750054 tortoise_orm_stubs-1.0.0/README.md
+-rw-r--r--   0        0        0     1060 2023-04-25 13:12:52.836668 tortoise_orm_stubs-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0    13458 2023-04-25 16:51:11.673362 tortoise_orm_stubs-1.0.0/tortoise-stubs/fields/__init__.pyi
+-rw-r--r--   0        0        0        8 2022-09-22 19:51:35.803221 tortoise_orm_stubs-1.0.0/tortoise-stubs/py.typed
+-rw-r--r--   0        0        0     1286 1970-01-01 00:00:00.000000 tortoise_orm_stubs-1.0.0/setup.py
+-rw-r--r--   0        0        0     1273 1970-01-01 00:00:00.000000 tortoise_orm_stubs-1.0.0/PKG-INFO
```

### Comparing `tortoise_orm_stubs-0.4.4/LICENSE` & `tortoise_orm_stubs-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tortoise_orm_stubs-0.4.4/pyproject.toml` & `tortoise_orm_stubs-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tortoise-orm-stubs"
-version = "0.4.4"
+version = "1.0.0"
 description = "Type stubs that make tortoise-orm a lot easier to work with when using type checkers."
 packages = [{ include = "tortoise-stubs" }]
 authors = ["Stanislav Zmiev <szmiev2000@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/Ovsyanka83/tortoise-orm-stubs"
```

### Comparing `tortoise_orm_stubs-0.4.4/tortoise-stubs/fields/__init__.pyi` & `tortoise_orm_stubs-1.0.0/tortoise-stubs/fields/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import datetime
 import decimal
 import typing
 import uuid
-from typing import Any, Callable, Generic, List, Literal, Optional, Type, TypeVar, Union, overload
+from typing import Any, Callable, List, Literal, Optional, Type, Union, overload
 
+import tortoise.fields.base
 import tortoise.validators
-from tortoise.fields.base import NO_ACTION, SET_DEFAULT
-from tortoise.fields.base import Field as _Field
+from tortoise.fields.base import NO_ACTION, SET_DEFAULT, Field
 from tortoise.fields.data import CharEnumType, IntEnumType
 from tortoise.fields.relational import (
     CASCADE,
     RESTRICT,
     SET_NULL,
     BackwardFKRelation,
     BackwardOneToOneRelation,
@@ -59,139 +59,108 @@
     "ManyToManyField",
     "ManyToManyRelation",
     "OneToOneField",
     "OneToOneNullableRelation",
     "OneToOneRelation",
     "ReverseRelation",
 ]
-VALUE = TypeVar("VALUE")
-
-
-class Field(Generic[VALUE], _Field):
-    def __new__(cls, *args: Any, **kwargs: Any) -> "Field[VALUE]":
-        ...
-
-    @overload
-    def __get__(self, instance: None, owner: Type["Model"]) -> "Field[VALUE]":
-        ...
-
-    @overload
-    def __get__(self, instance: "Model", owner: Type["Model"]) -> VALUE:
-        ...
-
-    def __get__(self, instance: Optional["Model"], owner: Type["Model"]) -> "Field[VALUE] | VALUE":
-        ...
-
-    def __set__(self, instance: "Model", value: VALUE) -> None:
-        ...
-
 
 @overload
-def BigIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> Field[int]:
+def BigIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Big integer field. (64-bit signed)
 
     ``pk`` (bool):
         True if field is Primary Key.
     """
 
-
 @overload
-def BigIntField(pk: bool = False, *, null: Literal[True], **kwargs: Any) -> Field[typing.Optional[int]]:
-    ...
-
-
+def BigIntField(
+    pk: bool = False, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[int]]: ...
 @overload
 def BinaryField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[bytes]:
+) -> tortoise.fields.base.Field[bytes]:
     """
     Binary field.
 
     This is for storing ``bytes`` objects.
     Note that filter or queryset-update operations are not supported.
     """
 
-
 @overload
 def BinaryField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[typing.Optional[bytes]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[bytes]]: ...
 @overload
 def BooleanField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[bool]:
+) -> tortoise.fields.base.Field[bool]:
     """
     Boolean field.
     """
 
-
 @overload
 def BooleanField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[typing.Optional[bool]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[bool]]: ...
 @overload
 def CharEnumField(
     enum_type: Type[CharEnumType],
     description: Optional[str] = None,
     max_length: int = 0,
     *,
     null: Literal[False] = False,
     **kwargs: Any,
-) -> Field[CharEnumType]:
+) -> tortoise.fields.base.Field[CharEnumType]:
     """
     Char Enum Field
 
     A field representing a character enumeration.
 
     **Warning**: If ``max_length`` is not specified or equals to zero, the size of represented
     char fields is automatically detected. So if later you update the enum, you need to update your
@@ -206,171 +175,149 @@
         of "name: value" pairs.
     ``max_length``:
         The length of the created CharField. If it is zero it is automatically detected from
         enum_type.
 
     """
 
-
 @overload
 def CharEnumField(
     enum_type: Type[CharEnumType],
     description: Optional[str] = None,
     max_length: int = 0,
     *,
     null: Literal[True],
     **kwargs: Any,
-) -> Field[typing.Optional[CharEnumType]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[CharEnumType]]: ...
 @overload
-def CharField(max_length: int, *, null: Literal[False] = False, **kwargs: Any) -> Field[str]:
+def CharField(max_length: int, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[str]:
     """
     Character field.
 
     You must provide the following:
 
     ``max_length`` (int):
         Maximum length of the field in characters.
     """
 
-
 @overload
-def CharField(max_length: int, *, null: Literal[True], **kwargs: Any) -> Field[typing.Optional[str]]:
-    ...
-
-
+def CharField(
+    max_length: int, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[str]]: ...
 @overload
 def DateField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[datetime.date]:
+) -> tortoise.fields.base.Field[datetime.date]:
     """
     Date field.
     """
 
-
 @overload
 def DateField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[typing.Optional[datetime.date]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[datetime.date]]: ...
 @overload
 def DatetimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[False] = False, **kwargs: Any
-) -> Field[datetime.datetime]:
+) -> tortoise.fields.base.Field[datetime.datetime]:
     """
     Datetime field.
 
     ``auto_now`` and ``auto_now_add`` is exclusive.
     You can opt to set neither or only ONE of them.
 
     ``auto_now`` (bool):
         Always set to ``datetime.utcnow()`` on save.
     ``auto_now_add`` (bool):
         Set to ``datetime.utcnow()`` on first save only.
     """
 
-
 @overload
 def DatetimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[True], **kwargs: Any
-) -> Field[typing.Optional[datetime.datetime]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[datetime.datetime]]: ...
 @overload
 def DecimalField(
     max_digits: int, decimal_places: int, *, null: Literal[False] = False, **kwargs: Any
-) -> Field[decimal.Decimal]:
+) -> tortoise.fields.base.Field[decimal.Decimal]:
     """
     Accurate decimal field.
 
     You must provide the following:
 
     ``max_digits`` (int):
         Max digits of significance of the decimal field.
     ``decimal_places`` (int):
         How many of those significant digits is after the decimal point.
     """
 
-
 @overload
 def DecimalField(
     max_digits: int, decimal_places: int, *, null: Literal[True], **kwargs: Any
-) -> Field[typing.Optional[decimal.Decimal]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[decimal.Decimal]]: ...
 @overload
 def FloatField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[float]:
+) -> tortoise.fields.base.Field[float]:
     """
     Float (double) field.
     """
 
-
 @overload
 def FloatField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[typing.Optional[float]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[float]]: ...
 @overload
 def IntEnumField(
     enum_type: Type[IntEnumType], description: Optional[str] = None, *, null: Literal[False] = False, **kwargs: Any
-) -> Field[IntEnumType]:
+) -> tortoise.fields.base.Field[IntEnumType]:
     """
     Enum Field
 
     A field representing an integer enumeration.
 
     The description of the field is set automatically if not specified to a multiline list of
     "name: value" pairs.
@@ -381,45 +328,39 @@
         The enum class
     ``description``:
         The description of the field. It is set automatically if not specified to a multiline list
         of "name: value" pairs.
 
     """
 
-
 @overload
 def IntEnumField(
     enum_type: Type[IntEnumType], description: Optional[str] = None, *, null: Literal[True], **kwargs: Any
-) -> Field[typing.Optional[IntEnumType]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[IntEnumType]]: ...
 @overload
-def IntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> Field[int]:
+def IntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Integer field. (32-bit signed)
 
     ``pk`` (bool):
         True if field is Primary Key.
     """
 
-
 @overload
-def IntField(pk: bool = False, *, null: Literal[True], **kwargs: Any) -> Field[typing.Optional[int]]:
-    ...
-
-
+def IntField(
+    pk: bool = False, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[int]]: ...
 @overload
 def JSONField(
     encoder: Callable[[Any], str] = ...,
     decoder: Callable[[Union[str, bytes]], Any] = ...,
     *,
     null: Literal[False] = False,
     **kwargs: Any,
-) -> Field[typing.Union[dict, list]]:
+) -> tortoise.fields.base.Field[typing.Union[dict, list]]:
     """
     JSON field.
 
     This field can store dictionaries or lists of any JSON-compliant structure.
 
     You can specify your own custom JSON encoder/decoder, leaving at the default should work well.
     If you have ``python-rapidjson`` installed, we default to using that,
@@ -428,118 +369,98 @@
     ``encoder``:
         The custom JSON encoder.
     ``decoder``:
         The custom JSON decoder.
 
     """
 
-
 @overload
 def JSONField(
     encoder: Callable[[Any], str] = ...,
     decoder: Callable[[Union[str, bytes]], Any] = ...,
     *,
     null: Literal[True],
     **kwargs: Any,
-) -> Field[typing.Union[dict, list, None]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Union[dict, list, None]]: ...
 @overload
-def SmallIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> Field[int]:
+def SmallIntField(pk: bool = False, *, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[int]:
     """
     Small integer field. (16-bit signed)
 
     ``pk`` (bool):
         True if field is Primary Key.
     """
 
-
 @overload
-def SmallIntField(pk: bool = False, *, null: Literal[True], **kwargs: Any) -> Field[typing.Optional[int]]:
-    ...
-
-
+def SmallIntField(
+    pk: bool = False, *, null: Literal[True], **kwargs: Any
+) -> tortoise.fields.base.Field[typing.Optional[int]]: ...
 @overload
 def TextField(
     pk: bool = False, unique: bool = False, index: bool = False, *, null: Literal[False] = False, **kwargs: Any
-) -> Field[str]:
+) -> tortoise.fields.base.Field[str]:
     """
     Large Text field.
     """
 
-
 @overload
 def TextField(
     pk: bool = False, unique: bool = False, index: bool = False, *, null: Literal[True], **kwargs: Any
-) -> Field[typing.Optional[str]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[str]]: ...
 @overload
 def TimeDeltaField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[False] = False,
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[datetime.timedelta]:
+) -> tortoise.fields.base.Field[datetime.timedelta]:
     """
     A field for storing time differences.
     """
 
-
 @overload
 def TimeDeltaField(
     source_field: Optional[str] = None,
     generated: bool = False,
     pk: bool = False,
     *,
     null: Literal[True],
     default: Any = None,
     unique: bool = False,
     index: bool = False,
     description: Optional[str] = None,
     model: "Optional[Model]" = None,
     validators: Optional[List[Union[tortoise.validators.Validator, Callable]]] = None,
     **kwargs: Any,
-) -> Field[typing.Optional[datetime.timedelta]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[datetime.timedelta]]: ...
 @overload
 def TimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[False] = False, **kwargs: Any
-) -> Field[datetime.time]:
+) -> tortoise.fields.base.Field[datetime.time]:
     """
     Time field.
     """
 
-
 @overload
 def TimeField(
     auto_now: bool = False, auto_now_add: bool = False, *, null: Literal[True], **kwargs: Any
-) -> Field[typing.Optional[datetime.time]]:
-    ...
-
-
+) -> tortoise.fields.base.Field[typing.Optional[datetime.time]]: ...
 @overload
-def UUIDField(*, null: Literal[False] = False, **kwargs: Any) -> Field[uuid.UUID]:
+def UUIDField(*, null: Literal[False] = False, **kwargs: Any) -> tortoise.fields.base.Field[uuid.UUID]:
     """
     UUID Field
 
     This field can store uuid value.
 
     If used as a primary key, it will auto-generate a UUID4 by default.
     """
 
-
 @overload
-def UUIDField(*, null: Literal[True], **kwargs: Any) -> Field[typing.Optional[uuid.UUID]]:
-    ...
+def UUIDField(*, null: Literal[True], **kwargs: Any) -> tortoise.fields.base.Field[typing.Optional[uuid.UUID]]: ...
```

### Comparing `tortoise_orm_stubs-0.4.4/setup.py` & `tortoise_orm_stubs-1.0.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*'], 'tortoise-stubs': ['fields/*']}
 
 install_requires = \
 ['tortoise-orm']
 
 setup_kwargs = {
     'name': 'tortoise-orm-stubs',
-    'version': '0.4.4',
+    'version': '1.0.0',
     'description': 'Type stubs that make tortoise-orm a lot easier to work with when using type checkers.',
     'long_description': "# tortoise-orm-stubs\n\nType stubs that make **tortoise-orm** a bit easier to work with when using type checkers.\n\nSpecifically, data fields' types automatically reflect the value of null argument (i.e. become optional if you set null=True)\n\n## Installation\n\n`pip install tortoise-orm-stubs`\n\n## Disclaimer\n\nPreviously **tortoise-orm-stubs** provided a lot more value but now the majority of its functionality has become a part of **tortoise-orm**. Hopefully, it will become completely unnecessary in the future.\n",
     'author': 'Stanislav Zmiev',
     'author_email': 'szmiev2000@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/Ovsyanka83/tortoise-orm-stubs',
```

### Comparing `tortoise_orm_stubs-0.4.4/PKG-INFO` & `tortoise_orm_stubs-1.0.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tortoise-orm-stubs
-Version: 0.4.4
+Version: 1.0.0
 Summary: Type stubs that make tortoise-orm a lot easier to work with when using type checkers.
 Home-page: https://github.com/Ovsyanka83/tortoise-orm-stubs
 License: MIT
 Author: Stanislav Zmiev
 Author-email: szmiev2000@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

