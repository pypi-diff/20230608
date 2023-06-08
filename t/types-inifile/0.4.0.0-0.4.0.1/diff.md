# Comparing `tmp/types-inifile-0.4.0.0.tar.gz` & `tmp/types-inifile-0.4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-inifile-0.4.0.0.tar", last modified: Wed Jun  7 06:18:44 2023, max compression
+gzip compressed data, was "types-inifile-0.4.0.1.tar", last modified: Thu Jun  8 01:37:27 2023, max compression
```

## Comparing `types-inifile-0.4.0.0.tar` & `types-inifile-0.4.0.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:44.606323 types-inifile-0.4.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-07 06:18:43.000000 types-inifile-0.4.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 06:18:43.000000 types-inifile-0.4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-07 06:18:44.606323 types-inifile-0.4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:44.606323 types-inifile-0.4.0.0/inifile-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-07 06:18:43.000000 types-inifile-0.4.0.0/inifile-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     4466 2023-06-07 06:18:43.000000 types-inifile-0.4.0.0/inifile-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 06:18:44.606323 types-inifile-0.4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-07 06:18:43.000000 types-inifile-0.4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 06:18:44.606323 types-inifile-0.4.0.0/types_inifile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-07 06:18:44.000000 types-inifile-0.4.0.0/types_inifile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 06:18:44.000000 types-inifile-0.4.0.0/types_inifile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 06:18:44.000000 types-inifile-0.4.0.0/types_inifile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 06:18:44.000000 types-inifile-0.4.0.0/types_inifile.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:37:27.887733 types-inifile-0.4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-08 01:37:26.000000 types-inifile-0.4.0.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 01:37:26.000000 types-inifile-0.4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-08 01:37:27.887733 types-inifile-0.4.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:37:27.883733 types-inifile-0.4.0.1/inifile-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 01:37:26.000000 types-inifile-0.4.0.1/inifile-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-06-08 01:37:26.000000 types-inifile-0.4.0.1/inifile-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:37:27.887733 types-inifile-0.4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-08 01:37:26.000000 types-inifile-0.4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:37:27.887733 types-inifile-0.4.0.1/types_inifile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-06-08 01:37:27.000000 types-inifile-0.4.0.1/types_inifile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-08 01:37:27.000000 types-inifile-0.4.0.1/types_inifile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:37:27.000000 types-inifile-0.4.0.1/types_inifile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 01:37:27.000000 types-inifile-0.4.0.1/types_inifile.egg-info/top_level.txt
```

### Comparing `types-inifile-0.4.0.0/PKG-INFO` & `types-inifile-0.4.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-inifile
-Version: 0.4.0.0
+Version: 0.4.0.1
 Summary: Typing stubs for inifile
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/inifile.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `inifile`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/inifile. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `89a22f99120600ab77df27ec93e1ed1fe00185f7`.
+This package was generated from typeshed commit `4849ddd74a2036ea29dd309d29c2466febc310f1`.
```

### Comparing `types-inifile-0.4.0.0/inifile-stubs/__init__.pyi` & `types-inifile-0.4.0.1/inifile-stubs/__init__.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from _typeshed import StrOrBytesPath, StrPath, SupportsKeysAndGetItem
+from _typeshed import StrPath, SupportsKeysAndGetItem
 from collections.abc import Container, Iterable, Iterator, Mapping, MutableMapping, Sequence
 from typing import TypeVar, overload
 from typing_extensions import Literal, TypeAlias
 from uuid import UUID
 
 _T = TypeVar("_T")
 
@@ -12,33 +12,41 @@
     | tuple[Literal["SECTION"], str, tuple[str, ...]]
     | tuple[Literal["KV"], str, tuple[str, str, str]]
 )
 
 def get_app_dir(app_name: str, roaming: bool = ..., force_posix: bool = ...) -> str: ...
 
 class Dialect:
-    ns_sep: str
-    kv_sep: str
-    quotes: Sequence[str]
-    true: Sequence[str]
-    false: Sequence[str]
-    comments: Container[str]
-    allow_escaping: bool
-    linesep: str | None
     def __init__(
         self,
         ns_sep: str = ...,
         kv_sep: str = ...,
         quotes: Sequence[str] = ...,
         true: Sequence[str] = ...,
         false: Sequence[str] = ...,
         comments: Container[str] = ...,
         allow_escaping: bool = ...,
         linesep: str | None = ...,
     ) -> None: ...
+    @property
+    def ns_sep(self) -> str: ...
+    @property
+    def kv_sep(self) -> str: ...
+    @property
+    def quotes(self) -> Sequence[str]: ...
+    @property
+    def true(self) -> Sequence[str]: ...
+    @property
+    def false(self) -> Sequence[str]: ...
+    @property
+    def comments(self) -> Container[str]: ...
+    @property
+    def allow_escaping(self) -> bool: ...
+    @property
+    def linesep(self) -> str | None: ...
     def get_actual_linesep(self) -> str: ...
     def get_strippable_lineseps(self) -> str: ...
     def kv_serialize(self, key, val: str | None) -> str | None: ...
     def escape(self, value: str, quote: str | None = ...) -> str: ...
     def unescape(self, value: str) -> str: ...
     def to_string(self, value: bool | float | str) -> str: ...
     def dict_from_iterable(self, iterable: Iterable[str]) -> MutableMapping[str, str]: ...
@@ -48,14 +56,16 @@
     ) -> list[_Token]: ...
 
 default_dialect: Dialect
 
 class IniData(MutableMapping[str, str]):
     def __init__(self, mapping: Mapping[str, str] | None = ..., dialect: Dialect | None = ...) -> None: ...
     @property
+    def dialect(self) -> Dialect: ...
+    @property
     def is_dirty(self) -> bool: ...
     def get_updated_lines(self, line_iter: Iterable[_Token] | None = ...) -> list[_Token]: ...
     def discard(self) -> None: ...
     def rollover(self) -> None: ...
     def to_dict(self) -> dict[str, str]: ...
     def __len__(self) -> int: ...
     @overload
@@ -95,15 +105,21 @@
     def values(self) -> Iterator[str]: ...  # type: ignore[override]
     def section_as_dict(self, section: str) -> dict[str, str]: ...
     def __getitem__(self, name: str) -> str: ...
     def __setitem__(self, name: str, value: str) -> None: ...
     def __delitem__(self, name: str) -> None: ...
 
 class IniFile(IniData):
-    def __init__(self, filename: StrOrBytesPath | int, encoding: str | None = ..., dialect: Dialect | None = ...) -> None: ...
+    def __init__(self, filename: StrPath, encoding: str | None = ..., dialect: Dialect | None = ...) -> None: ...
+    @property
+    def filename(self) -> str: ...
+    @property
+    def encoding(self) -> str | None: ...
+    @property
+    def is_new(self) -> bool: ...
     def save(self, create_folder: bool = ...) -> None: ...
 
 class AppIniFile(IniFile):
     def __init__(
         self,
         app_name: str,
         filename: StrPath,
```

### Comparing `types-inifile-0.4.0.0/setup.py` & `types-inifile-0.4.0.1/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `inifile`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/inifile. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `89a22f99120600ab77df27ec93e1ed1fe00185f7`.
+This package was generated from typeshed commit `4849ddd74a2036ea29dd309d29c2466febc310f1`.
 '''.lstrip()
 
 setup(name=name,
-      version="0.4.0.0",
+      version="0.4.0.1",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/inifile.md",
```

### Comparing `types-inifile-0.4.0.0/types_inifile.egg-info/PKG-INFO` & `types-inifile-0.4.0.1/types_inifile.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-inifile
-Version: 0.4.0.0
+Version: 0.4.0.1
 Summary: Typing stubs for inifile
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/inifile.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -22,8 +22,8 @@
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `inifile`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/inifile. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `89a22f99120600ab77df27ec93e1ed1fe00185f7`.
+This package was generated from typeshed commit `4849ddd74a2036ea29dd309d29c2466febc310f1`.
```

