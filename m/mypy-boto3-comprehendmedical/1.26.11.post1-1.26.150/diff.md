# Comparing `tmp/mypy-boto3-comprehendmedical-1.26.11.post1.tar.gz` & `tmp/mypy-boto3-comprehendmedical-1.26.150.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-comprehendmedical-1.26.11.post1.tar", last modified: Wed Nov 16 20:47:45 2022, max compression
+gzip compressed data, was "mypy-boto3-comprehendmedical-1.26.150.tar", last modified: Thu Jun  8 19:32:29 2023, max compression
```

## Comparing `mypy-boto3-comprehendmedical-1.26.11.post1.tar` & `mypy-boto3-comprehendmedical-1.26.150.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:45.434894 mypy-boto3-comprehendmedical-1.26.11.post1/
--rw-r--r--   0 runner    (1001) docker     (122)     1070 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    15815 2022-11-16 20:47:45.434894 mypy-boto3-comprehendmedical-1.26.11.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14332 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:45.430894 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/
--rw-r--r--   0 runner    (1001) docker     (122)      453 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      452 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      960 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    21580 2022-11-16 20:46:52.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/client.py
--rw-r--r--   0 runner    (1001) docker     (122)    21547 2022-11-16 20:46:52.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/client.pyi
--rw-r--r--   0 runner    (1001) docker     (122)    10920 2022-11-16 20:46:52.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/literals.py
--rw-r--r--   0 runner    (1001) docker     (122)    10918 2022-11-16 20:46:52.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)    24865 2022-11-16 20:46:53.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (122)    24850 2022-11-16 20:46:52.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (122)       67 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/version.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2022-11-16 20:47:45.434894 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    15815 2022-11-16 20:47:45.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      785 2022-11-16 20:47:45.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 20:47:45.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2022-11-16 20:47:45.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       25 2022-11-16 20:47:45.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       29 2022-11-16 20:47:45.000000 mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2022-11-16 20:47:45.434894 mypy-boto3-comprehendmedical-1.26.11.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2040 2022-11-16 20:46:51.000000 mypy-boto3-comprehendmedical-1.26.11.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14321 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21580 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21547 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    11568 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11566 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    24890 2023-06-08 19:32:10.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24875 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      785 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 19:32:29.000000 mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:29.727941 mypy-boto3-comprehendmedical-1.26.150/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-06-08 19:32:09.000000 mypy-boto3-comprehendmedical-1.26.150/setup.py
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/LICENSE` & `mypy-boto3-comprehendmedical-1.26.150/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2022 Vlad Emelianov
+Copyright (c) 2023 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/PKG-INFO` & `mypy-boto3-comprehendmedical-1.26.150/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.26.11.post1
-Summary: Type annotations for boto3.ComprehendMedical 1.26.11 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.150
+Summary: Type annotations for boto3.ComprehendMedical 1.26.150 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-comprehendmedical"></a>
 
 # mypy-boto3-comprehendmedical
 
 [![PyPI - mypy-boto3-comprehendmedical](https://img.shields.io/pypi/v/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.26.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,42 +406,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/README.md` & `mypy-boto3-comprehendmedical-1.26.150/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-comprehendmedical"></a>
 
 # mypy-boto3-comprehendmedical
 
 [![PyPI - mypy-boto3-comprehendmedical](https://img.shields.io/pypi/v/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.26.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -374,42 +374,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/__main__.py` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ComprehendMedical 1.26.11\nVersion:        "
-        " 1.26.11.post1\nBuilder version: 7.11.10\nDocs:           "
+        "Type annotations for boto3.ComprehendMedical 1.26.150\nVersion:         1.26.150\nBuilder"
+        " version: 7.14.5\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical//\nBoto3 docs:   "
         "   https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.11.post1")
+    print("1.26.150")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/client.py` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/client.pyi` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/literals.py` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,15 +121,15 @@
     "QUANTITY",
     "SYSTEM_ORGAN_SITE",
     "TIME_EXPRESSION",
     "TIME_TO_DX_NAME",
 ]
 ICD10CMEntityCategoryType = Literal["MEDICAL_CONDITION"]
 ICD10CMEntityTypeType = Literal["DX_NAME", "TIME_EXPRESSION"]
-ICD10CMRelationshipTypeType = Literal["OVERLAP", "SYSTEM_ORGAN_SITE"]
+ICD10CMRelationshipTypeType = Literal["OVERLAP", "QUALITY", "SYSTEM_ORGAN_SITE"]
 ICD10CMTraitNameType = Literal[
     "DIAGNOSIS",
     "HYPOTHETICAL",
     "LOW_CONFIDENCE",
     "NEGATION",
     "PERTAINS_TO_FAMILY",
     "SIGN",
@@ -154,36 +154,38 @@
     "DURATION",
     "EVERY",
     "FOR",
     "FORM",
     "FREQUENCY",
     "NEGATIVE",
     "OVERLAP",
+    "QUALITY",
     "RATE",
     "ROUTE_OR_MODE",
     "STRENGTH",
     "SYSTEM_ORGAN_SITE",
     "TEST_UNIT",
     "TEST_UNITS",
     "TEST_VALUE",
+    "USAGE",
     "WITH_DOSAGE",
 ]
 RxNormAttributeTypeType = Literal[
     "DOSAGE", "DURATION", "FORM", "FREQUENCY", "RATE", "ROUTE_OR_MODE", "STRENGTH"
 ]
 RxNormEntityCategoryType = Literal["MEDICATION"]
 RxNormEntityTypeType = Literal["BRAND_NAME", "GENERIC_NAME"]
-RxNormTraitNameType = Literal["NEGATION"]
+RxNormTraitNameType = Literal["NEGATION", "PAST_HISTORY"]
 SNOMEDCTAttributeTypeType = Literal[
     "ACUITY", "DIRECTION", "QUALITY", "SYSTEM_ORGAN_SITE", "TEST_UNIT", "TEST_VALUE"
 ]
 SNOMEDCTEntityCategoryType = Literal["ANATOMY", "MEDICAL_CONDITION", "TEST_TREATMENT_PROCEDURE"]
 SNOMEDCTEntityTypeType = Literal["DX_NAME", "PROCEDURE_NAME", "TEST_NAME", "TREATMENT_NAME"]
 SNOMEDCTRelationshipTypeType = Literal[
-    "ACUITY", "DIRECTION", "QUALITY", "SYSTEM_ORGAN_SITE", "TEST_UNITS", "TEST_VALUE"
+    "ACUITY", "DIRECTION", "QUALITY", "SYSTEM_ORGAN_SITE", "TEST_UNIT", "TEST_UNITS", "TEST_VALUE"
 ]
 SNOMEDCTTraitNameType = Literal[
     "DIAGNOSIS",
     "FUTURE",
     "HYPOTHETICAL",
     "LOW_CONFIDENCE",
     "NEGATION",
@@ -213,14 +215,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -230,27 +233,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -279,14 +286,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -331,51 +339,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -388,14 +402,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -407,28 +422,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -456,57 +478,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/literals.pyi` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     "QUANTITY",
     "SYSTEM_ORGAN_SITE",
     "TIME_EXPRESSION",
     "TIME_TO_DX_NAME",
 ]
 ICD10CMEntityCategoryType = Literal["MEDICAL_CONDITION"]
 ICD10CMEntityTypeType = Literal["DX_NAME", "TIME_EXPRESSION"]
-ICD10CMRelationshipTypeType = Literal["OVERLAP", "SYSTEM_ORGAN_SITE"]
+ICD10CMRelationshipTypeType = Literal["OVERLAP", "QUALITY", "SYSTEM_ORGAN_SITE"]
 ICD10CMTraitNameType = Literal[
     "DIAGNOSIS",
     "HYPOTHETICAL",
     "LOW_CONFIDENCE",
     "NEGATION",
     "PERTAINS_TO_FAMILY",
     "SIGN",
@@ -152,36 +152,38 @@
     "DURATION",
     "EVERY",
     "FOR",
     "FORM",
     "FREQUENCY",
     "NEGATIVE",
     "OVERLAP",
+    "QUALITY",
     "RATE",
     "ROUTE_OR_MODE",
     "STRENGTH",
     "SYSTEM_ORGAN_SITE",
     "TEST_UNIT",
     "TEST_UNITS",
     "TEST_VALUE",
+    "USAGE",
     "WITH_DOSAGE",
 ]
 RxNormAttributeTypeType = Literal[
     "DOSAGE", "DURATION", "FORM", "FREQUENCY", "RATE", "ROUTE_OR_MODE", "STRENGTH"
 ]
 RxNormEntityCategoryType = Literal["MEDICATION"]
 RxNormEntityTypeType = Literal["BRAND_NAME", "GENERIC_NAME"]
-RxNormTraitNameType = Literal["NEGATION"]
+RxNormTraitNameType = Literal["NEGATION", "PAST_HISTORY"]
 SNOMEDCTAttributeTypeType = Literal[
     "ACUITY", "DIRECTION", "QUALITY", "SYSTEM_ORGAN_SITE", "TEST_UNIT", "TEST_VALUE"
 ]
 SNOMEDCTEntityCategoryType = Literal["ANATOMY", "MEDICAL_CONDITION", "TEST_TREATMENT_PROCEDURE"]
 SNOMEDCTEntityTypeType = Literal["DX_NAME", "PROCEDURE_NAME", "TEST_NAME", "TREATMENT_NAME"]
 SNOMEDCTRelationshipTypeType = Literal[
-    "ACUITY", "DIRECTION", "QUALITY", "SYSTEM_ORGAN_SITE", "TEST_UNITS", "TEST_VALUE"
+    "ACUITY", "DIRECTION", "QUALITY", "SYSTEM_ORGAN_SITE", "TEST_UNIT", "TEST_UNITS", "TEST_VALUE"
 ]
 SNOMEDCTTraitNameType = Literal[
     "DIAGNOSIS",
     "FUTURE",
     "HYPOTHETICAL",
     "LOW_CONFIDENCE",
     "NEGATION",
@@ -211,14 +213,15 @@
     "application-autoscaling",
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
+    "arc-zonal-shift",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "backup",
     "backup-gateway",
     "backupstorage",
@@ -228,27 +231,31 @@
     "budgets",
     "ce",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
+    "chime-sdk-voice",
+    "cleanrooms",
     "cloud9",
     "cloudcontrol",
     "clouddirectory",
     "cloudformation",
     "cloudfront",
     "cloudhsm",
     "cloudhsmv2",
     "cloudsearch",
     "cloudsearchdomain",
     "cloudtrail",
+    "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
+    "codecatalyst",
     "codecommit",
     "codedeploy",
     "codeguru-reviewer",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -277,14 +284,15 @@
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
     "docdb",
+    "docdb-elastic",
     "drs",
     "ds",
     "dynamodb",
     "dynamodbstreams",
     "ebs",
     "ec2",
     "ec2-instance-connect",
@@ -329,51 +337,57 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
+    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
+    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
+    "kendra-ranking",
     "keyspaces",
     "kinesis",
     "kinesis-video-archived-media",
     "kinesis-video-media",
     "kinesis-video-signaling",
+    "kinesis-video-webrtc-storage",
     "kinesisanalytics",
     "kinesisanalyticsv2",
     "kinesisvideo",
     "kms",
     "lakeformation",
     "lambda",
     "lex-models",
     "lex-runtime",
     "lexv2-models",
     "lexv2-runtime",
     "license-manager",
+    "license-manager-linux-subscriptions",
     "license-manager-user-subscriptions",
     "lightsail",
     "location",
     "logs",
     "lookoutequipment",
     "lookoutmetrics",
     "lookoutvision",
@@ -386,14 +400,15 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
+    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -405,28 +420,35 @@
     "mq",
     "mturk",
     "mwaa",
     "neptune",
     "network-firewall",
     "networkmanager",
     "nimble",
+    "oam",
+    "omics",
     "opensearch",
+    "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
+    "osis",
     "outposts",
     "panorama",
+    "payment-cryptography",
+    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
     "pinpoint-sms-voice-v2",
+    "pipes",
     "polly",
     "pricing",
     "privatenetworks",
     "proton",
     "qldb",
     "qldb-session",
     "quicksight",
@@ -454,57 +476,63 @@
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
     "sagemaker-edge",
     "sagemaker-featurestore-runtime",
+    "sagemaker-geospatial",
+    "sagemaker-metrics",
     "sagemaker-runtime",
     "savingsplans",
     "scheduler",
     "schemas",
     "sdb",
     "secretsmanager",
     "securityhub",
+    "securitylake",
     "serverlessrepo",
     "service-quotas",
     "servicecatalog",
     "servicecatalog-appregistry",
     "servicediscovery",
     "ses",
     "sesv2",
     "shield",
     "signer",
+    "simspaceweaver",
     "sms",
     "sms-voice",
     "snow-device-management",
     "snowball",
     "sns",
     "sqs",
     "ssm",
     "ssm-contacts",
     "ssm-incidents",
-    "ssmsap",
+    "ssm-sap",
     "sso",
     "sso-admin",
     "sso-oidc",
     "stepfunctions",
     "storagegateway",
     "sts",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
     "timestream-query",
     "timestream-write",
+    "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
+    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/type_defs.py` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     ICD10CMEntityTypeType,
     ICD10CMRelationshipTypeType,
     ICD10CMTraitNameType,
     JobStatusType,
     RelationshipTypeType,
     RxNormAttributeTypeType,
     RxNormEntityTypeType,
+    RxNormTraitNameType,
     SNOMEDCTAttributeTypeType,
     SNOMEDCTEntityCategoryType,
     SNOMEDCTEntityTypeType,
     SNOMEDCTRelationshipTypeType,
     SNOMEDCTTraitNameType,
 )
 
@@ -304,15 +305,15 @@
     },
     total=False,
 )
 
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
-        "Name": Literal["NEGATION"],
+        "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
 RxNormConceptTypeDef = TypedDict(
     "RxNormConceptTypeDef",
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical/type_defs.pyi` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     ICD10CMEntityTypeType,
     ICD10CMRelationshipTypeType,
     ICD10CMTraitNameType,
     JobStatusType,
     RelationshipTypeType,
     RxNormAttributeTypeType,
     RxNormEntityTypeType,
+    RxNormTraitNameType,
     SNOMEDCTAttributeTypeType,
     SNOMEDCTEntityCategoryType,
     SNOMEDCTEntityTypeType,
     SNOMEDCTRelationshipTypeType,
     SNOMEDCTTraitNameType,
 )
 
@@ -299,15 +300,15 @@
     },
     total=False,
 )
 
 RxNormTraitTypeDef = TypedDict(
     "RxNormTraitTypeDef",
     {
-        "Name": Literal["NEGATION"],
+        "Name": RxNormTraitNameType,
         "Score": float,
     },
     total=False,
 )
 
 RxNormConceptTypeDef = TypedDict(
     "RxNormConceptTypeDef",
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/PKG-INFO` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-comprehendmedical
-Version: 1.26.11.post1
-Summary: Type annotations for boto3.ComprehendMedical 1.26.11 service generated with mypy-boto3-builder 7.11.10
+Version: 1.26.150
+Summary: Type annotations for boto3.ComprehendMedical 1.26.150 service generated with mypy-boto3-builder 7.14.5
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -18,43 +18,44 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <a id="mypy-boto3-comprehendmedical"></a>
 
 # mypy-boto3-comprehendmedical
 
 [![PyPI - mypy-boto3-comprehendmedical](https://img.shields.io/pypi/v/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-comprehendmedical.svg?color=blue)](https://pypi.org/project/mypy-boto3-comprehendmedical)
-[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
+[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-comprehendmedical?color=blue)](https://pypistats.org/packages/mypy-boto3-comprehendmedical)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ComprehendMedical 1.26.11](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
+[boto3.ComprehendMedical 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/comprehendmedical.html#ComprehendMedical)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.11.10](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-comprehendmedical docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/).
 
 See how it helps to find and fix potential bugs:
 
@@ -405,42 +406,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers a drop-in type annotations for you and makes sure that:
+updates. It delivers drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from the documentation (blame `botocore` docs if types
-  are incorrect).
+  annotations extracted from `botocore` schemas.
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
+- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
+  libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.session` calls
-- Auto discovery of types for `session.client` and `session.session` calls
+- Auto discovery of types for `boto3.client` and `boto3.resource` calls
+- Auto discovery of types for `session.client` and `session.resource` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt` & `mypy-boto3-comprehendmedical-1.26.150/mypy_boto3_comprehendmedical.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-comprehendmedical-1.26.11.post1/setup.py` & `mypy-boto3-comprehendmedical-1.26.150/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,54 +1,55 @@
 """
 Setup script for mypy-boto3-comprehendmedical.
 """
-from os.path import abspath, dirname
+from pathlib import Path
 
 from setuptools import setup
 
-LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
+LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-comprehendmedical",
-    version="1.26.11.post1",
+    version="1.26.150",
     packages=["mypy_boto3_comprehendmedical"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ComprehendMedical 1.26.11 service generated with"
-        " mypy-boto3-builder 7.11.10"
+        "Type annotations for boto3.ComprehendMedical 1.26.150 service generated with"
+        " mypy-boto3-builder 7.14.5"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Typing :: Typed",
     ],
     keywords="boto3 comprehendmedical type-annotations boto3-stubs mypy typeshed autocomplete",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
-    package_data={"": ["LICENSE"], "mypy_boto3_comprehendmedical": ["py.typed", "*.pyi"]},
+    package_data={"mypy_boto3_comprehendmedical": ["py.typed", "*.pyi"]},
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_comprehendmedical/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        "typing-extensions>=4.1.0",
+        'typing-extensions>=4.1.0; python_version<"3.9"',
     ],
     zip_safe=False,
 )
```

