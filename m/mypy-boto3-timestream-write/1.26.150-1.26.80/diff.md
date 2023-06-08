# Comparing `tmp/mypy-boto3-timestream-write-1.26.150.tar.gz` & `tmp/mypy-boto3-timestream-write-1.26.80.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-timestream-write-1.26.150.tar", last modified: Thu Jun  8 19:32:29 2023, max compression
+gzip compressed data, was "mypy-boto3-timestream-write-1.26.80.tar", last modified: Mon Feb 27 20:35:29 2023, max compression
```

## Comparing `mypy-boto3-timestream-write-1.26.150.tar` & `mypy-boto3-timestream-write-1.26.80.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.743941 mypy-boto3-timestream-write-1.26.150/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-06-08 19:32:29.743941 mypy-boto3-timestream-write-1.26.150/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13178 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.743941 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/
--rw-r--r--   0 runner    (1001) docker     (123)      440 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15356 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    15331 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8684 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)     8682 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    21309 2023-06-08 19:32:19.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    21278 2023-06-08 19:32:19.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.743941 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    14702 2023-06-08 19:32:29.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-06-08 19:32:29.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:32:29.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 19:32:29.000000 mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:29.743941 mypy-boto3-timestream-write-1.26.150/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-06-08 19:32:18.000000 mypy-boto3-timestream-write-1.26.150/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/
+-rw-r--r--   0 runner    (1001) docker     (123)      440 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15263 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15238 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8358 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    20526 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20497 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-27 20:35:19.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    14603 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-02-27 20:35:28.000000 mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-27 20:35:29.120040 mypy-boto3-timestream-write-1.26.80/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2058 2023-02-27 20:35:18.000000 mypy-boto3-timestream-write-1.26.80/setup.py
```

### Comparing `mypy-boto3-timestream-write-1.26.150/LICENSE` & `mypy-boto3-timestream-write-1.26.80/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 Vlad Emelianov
+Copyright (c) 2022 Vlad Emelianov
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `mypy-boto3-timestream-write-1.26.150/PKG-INFO` & `mypy-boto3-timestream-write-1.26.80/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.26.150
-Summary: Type annotations for boto3.TimestreamWrite 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.80
+Summary: Type annotations for boto3.TimestreamWrite 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,16 +281,14 @@
 
 ```python
 from mypy_boto3_timestream_write.literals import (
     BatchLoadDataFormatType,
     BatchLoadStatusType,
     DimensionValueTypeType,
     MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
     TimestreamWriteServiceName,
     ServiceName,
     ResourceServiceName,
@@ -331,15 +329,14 @@
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     CreateBatchLoadTaskResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -353,15 +350,14 @@
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
-    SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
@@ -384,42 +380,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-timestream-write-1.26.150/README.md` & `mypy-boto3-timestream-write-1.26.80/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -249,16 +249,14 @@
 
 ```python
 from mypy_boto3_timestream_write.literals import (
     BatchLoadDataFormatType,
     BatchLoadStatusType,
     DimensionValueTypeType,
     MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
     TimestreamWriteServiceName,
     ServiceName,
     ResourceServiceName,
@@ -299,15 +297,14 @@
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     CreateBatchLoadTaskResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -321,15 +318,14 @@
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
-    SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
@@ -352,42 +348,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/__main__.py` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.TimestreamWrite 1.26.150\nVersion:         1.26.150\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.TimestreamWrite 1.26.80\nVersion:         1.26.80\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write//\nBoto3 docs:    "
         "  https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.150")
+    print("1.26.80")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/client.py` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -132,16 +131,15 @@
     def create_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -288,16 +286,15 @@
 
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/client.pyi` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,14 @@
     ListDatabasesResponseTypeDef,
     ListTablesResponseTypeDef,
     ListTagsForResourceResponseTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     RecordTypeDef,
     ReportConfigurationTypeDef,
     RetentionPropertiesTypeDef,
-    SchemaTypeDef,
     TagTypeDef,
     UpdateDatabaseResponseTypeDef,
     UpdateTableResponseTypeDef,
     WriteRecordsResponseTypeDef,
 )
 
 __all__ = ("TimestreamWriteClient",)
@@ -124,16 +123,15 @@
     def create_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
     ) -> CreateTableResponseTypeDef:
         """
         Adds a new table to an existing database in your account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.create_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#create_table)
         """
@@ -264,16 +262,15 @@
         """
     def update_table(
         self,
         *,
         DatabaseName: str,
         TableName: str,
         RetentionProperties: RetentionPropertiesTypeDef = ...,
-        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...,
-        Schema: SchemaTypeDef = ...
+        MagneticStoreWriteProperties: MagneticStoreWritePropertiesTypeDef = ...
     ) -> UpdateTableResponseTypeDef:
         """
         Modifies the retention duration of the memory store and magnetic store for your
         Timestream table.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite.Client.update_table)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/client/#update_table)
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/literals.py` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,41 +14,35 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
-
 __all__ = (
     "BatchLoadDataFormatType",
     "BatchLoadStatusType",
     "DimensionValueTypeType",
     "MeasureValueTypeType",
-    "PartitionKeyEnforcementLevelType",
-    "PartitionKeyTypeType",
     "S3EncryptionOptionType",
     "ScalarMeasureValueTypeType",
     "TableStatusType",
     "TimeUnitType",
     "TimestreamWriteServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
-
 BatchLoadDataFormatType = Literal["CSV"]
 BatchLoadStatusType = Literal[
     "CREATED", "FAILED", "IN_PROGRESS", "PENDING_RESUME", "PROGRESS_STOPPED", "SUCCEEDED"
 ]
 DimensionValueTypeType = Literal["VARCHAR"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "TIMESTAMP", "VARCHAR"]
-PartitionKeyEnforcementLevelType = Literal["OPTIONAL", "REQUIRED"]
-PartitionKeyTypeType = Literal["DIMENSION", "MEASURE"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
 TableStatusType = Literal["ACTIVE", "DELETING", "RESTORING"]
 TimeUnitType = Literal["MICROSECONDS", "MILLISECONDS", "NANOSECONDS", "SECONDS"]
 TimestreamWriteServiceName = Literal["timestream-write"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -213,15 +207,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -257,15 +250,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -284,19 +276,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -381,15 +370,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/literals.pyi` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/literals.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,39 +14,37 @@
 import sys
 
 if sys.version_info >= (3, 9):
     from typing import Literal
 else:
     from typing_extensions import Literal
 
+
 __all__ = (
     "BatchLoadDataFormatType",
     "BatchLoadStatusType",
     "DimensionValueTypeType",
     "MeasureValueTypeType",
-    "PartitionKeyEnforcementLevelType",
-    "PartitionKeyTypeType",
     "S3EncryptionOptionType",
     "ScalarMeasureValueTypeType",
     "TableStatusType",
     "TimeUnitType",
     "TimestreamWriteServiceName",
     "ServiceName",
     "ResourceServiceName",
     "RegionName",
 )
 
+
 BatchLoadDataFormatType = Literal["CSV"]
 BatchLoadStatusType = Literal[
     "CREATED", "FAILED", "IN_PROGRESS", "PENDING_RESUME", "PROGRESS_STOPPED", "SUCCEEDED"
 ]
 DimensionValueTypeType = Literal["VARCHAR"]
 MeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "MULTI", "TIMESTAMP", "VARCHAR"]
-PartitionKeyEnforcementLevelType = Literal["OPTIONAL", "REQUIRED"]
-PartitionKeyTypeType = Literal["DIMENSION", "MEASURE"]
 S3EncryptionOptionType = Literal["SSE_KMS", "SSE_S3"]
 ScalarMeasureValueTypeType = Literal["BIGINT", "BOOLEAN", "DOUBLE", "TIMESTAMP", "VARCHAR"]
 TableStatusType = Literal["ACTIVE", "DELETING", "RESTORING"]
 TimeUnitType = Literal["MICROSECONDS", "MILLISECONDS", "NANOSECONDS", "SECONDS"]
 TimestreamWriteServiceName = Literal["timestream-write"]
 ServiceName = Literal[
     "accessanalyzer",
@@ -211,15 +209,14 @@
     "iotfleetwise",
     "iotsecuretunneling",
     "iotsitewise",
     "iotthingsgraph",
     "iottwinmaker",
     "iotwireless",
     "ivs",
-    "ivs-realtime",
     "ivschat",
     "kafka",
     "kafkaconnect",
     "kendra",
     "kendra-ranking",
     "keyspaces",
     "kinesis",
@@ -255,15 +252,14 @@
     "marketplace-entitlement",
     "marketplacecommerceanalytics",
     "mediaconnect",
     "mediaconvert",
     "medialive",
     "mediapackage",
     "mediapackage-vod",
-    "mediapackagev2",
     "mediastore",
     "mediastore-data",
     "mediatailor",
     "memorydb",
     "meteringmarketplace",
     "mgh",
     "mgn",
@@ -282,19 +278,16 @@
     "oam",
     "omics",
     "opensearch",
     "opensearchserverless",
     "opsworks",
     "opsworkscm",
     "organizations",
-    "osis",
     "outposts",
     "panorama",
-    "payment-cryptography",
-    "payment-cryptography-data",
     "personalize",
     "personalize-events",
     "personalize-runtime",
     "pi",
     "pinpoint",
     "pinpoint-email",
     "pinpoint-sms-voice",
@@ -379,15 +372,14 @@
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "voice-id",
-    "vpc-lattice",
     "waf",
     "waf-regional",
     "wafv2",
     "wellarchitected",
     "wisdom",
     "workdocs",
     "worklink",
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/type_defs.py` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
 )
 
 if sys.version_info >= (3, 9):
@@ -31,15 +29,14 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
-
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
@@ -57,15 +54,14 @@
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
-    "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
     "ReportS3ConfigurationTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "CreateBatchLoadTaskResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -79,15 +75,14 @@
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
-    "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
@@ -209,21 +204,19 @@
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
-
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
-
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -276,19 +269,17 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
-
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
-
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -352,41 +343,19 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
-
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-
-_RequiredPartitionKeyTypeDef = TypedDict(
-    "_RequiredPartitionKeyTypeDef",
-    {
-        "Type": PartitionKeyTypeType,
-    },
-)
-_OptionalPartitionKeyTypeDef = TypedDict(
-    "_OptionalPartitionKeyTypeDef",
-    {
-        "Name": str,
-        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
-    },
-    total=False,
-)
-
-
-class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
-    pass
-
-
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
     },
@@ -405,21 +374,19 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
-
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
-
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
@@ -474,21 +441,19 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
-
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
-
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -545,21 +510,19 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
-
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
-
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -600,50 +563,38 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
-
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
-
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
-
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-
-SchemaTypeDef = TypedDict(
-    "SchemaTypeDef",
-    {
-        "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
-    },
-    total=False,
-)
-
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -666,21 +617,19 @@
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
-
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
-
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -689,21 +638,19 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
-
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
-
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -714,56 +661,50 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
-
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
-
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
 _OptionalCreateTableRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
-
 TableTypeDef = TypedDict(
     "TableTypeDef",
     {
         "Arn": str,
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -772,26 +713,23 @@
     },
 )
 _OptionalUpdateTableRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
-
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
-
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
@@ -865,22 +803,20 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
-
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
-
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write/type_defs.pyi` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write/type_defs.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,16 +14,14 @@
 import sys
 from datetime import datetime
 from typing import Dict, List, Sequence
 
 from .literals import (
     BatchLoadStatusType,
     MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
 )
 
 if sys.version_info >= (3, 9):
@@ -31,14 +29,15 @@
 else:
     from typing_extensions import Literal
 if sys.version_info >= (3, 9):
     from typing import TypedDict
 else:
     from typing_extensions import TypedDict
 
+
 __all__ = (
     "BatchLoadProgressReportTypeDef",
     "BatchLoadTaskTypeDef",
     "ResponseMetadataTypeDef",
     "TagTypeDef",
     "DatabaseTypeDef",
     "RetentionPropertiesTypeDef",
@@ -56,15 +55,14 @@
     "ListBatchLoadTasksRequestRequestTypeDef",
     "ListDatabasesRequestRequestTypeDef",
     "ListTablesRequestRequestTypeDef",
     "ListTagsForResourceRequestRequestTypeDef",
     "S3ConfigurationTypeDef",
     "MeasureValueTypeDef",
     "MultiMeasureAttributeMappingTypeDef",
-    "PartitionKeyTypeDef",
     "RecordsIngestedTypeDef",
     "ReportS3ConfigurationTypeDef",
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateDatabaseRequestRequestTypeDef",
     "CreateBatchLoadTaskResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
@@ -78,15 +76,14 @@
     "UpdateDatabaseResponseTypeDef",
     "DataSourceConfigurationTypeDef",
     "DescribeEndpointsResponseTypeDef",
     "MagneticStoreRejectedDataLocationTypeDef",
     "RecordTypeDef",
     "MixedMeasureMappingTypeDef",
     "MultiMeasureMappingsTypeDef",
-    "SchemaTypeDef",
     "WriteRecordsResponseTypeDef",
     "ReportConfigurationTypeDef",
     "MagneticStoreWritePropertiesTypeDef",
     "WriteRecordsRequestRequestTypeDef",
     "DataModelTypeDef",
     "CreateTableRequestRequestTypeDef",
     "TableTypeDef",
@@ -208,19 +205,21 @@
     "_OptionalDataSourceS3ConfigurationTypeDef",
     {
         "ObjectKeyPrefix": str,
     },
     total=False,
 )
 
+
 class DataSourceS3ConfigurationTypeDef(
     _RequiredDataSourceS3ConfigurationTypeDef, _OptionalDataSourceS3ConfigurationTypeDef
 ):
     pass
 
+
 DeleteDatabaseRequestRequestTypeDef = TypedDict(
     "DeleteDatabaseRequestRequestTypeDef",
     {
         "DatabaseName": str,
     },
 )
 
@@ -273,17 +272,19 @@
     "_OptionalDimensionTypeDef",
     {
         "DimensionValueType": Literal["VARCHAR"],
     },
     total=False,
 )
 
+
 class DimensionTypeDef(_RequiredDimensionTypeDef, _OptionalDimensionTypeDef):
     pass
 
+
 ListBatchLoadTasksRequestRequestTypeDef = TypedDict(
     "ListBatchLoadTasksRequestRequestTypeDef",
     {
         "NextToken": str,
         "MaxResults": int,
         "TaskStatus": BatchLoadStatusType,
     },
@@ -347,36 +348,20 @@
     {
         "TargetMultiMeasureAttributeName": str,
         "MeasureValueType": ScalarMeasureValueTypeType,
     },
     total=False,
 )
 
+
 class MultiMeasureAttributeMappingTypeDef(
     _RequiredMultiMeasureAttributeMappingTypeDef, _OptionalMultiMeasureAttributeMappingTypeDef
 ):
     pass
 
-_RequiredPartitionKeyTypeDef = TypedDict(
-    "_RequiredPartitionKeyTypeDef",
-    {
-        "Type": PartitionKeyTypeType,
-    },
-)
-_OptionalPartitionKeyTypeDef = TypedDict(
-    "_OptionalPartitionKeyTypeDef",
-    {
-        "Name": str,
-        "EnforcementInRecord": PartitionKeyEnforcementLevelType,
-    },
-    total=False,
-)
-
-class PartitionKeyTypeDef(_RequiredPartitionKeyTypeDef, _OptionalPartitionKeyTypeDef):
-    pass
 
 RecordsIngestedTypeDef = TypedDict(
     "RecordsIngestedTypeDef",
     {
         "Total": int,
         "MemoryStore": int,
         "MagneticStore": int,
@@ -396,19 +381,21 @@
         "ObjectKeyPrefix": str,
         "EncryptionOption": S3EncryptionOptionType,
         "KmsKeyId": str,
     },
     total=False,
 )
 
+
 class ReportS3ConfigurationTypeDef(
     _RequiredReportS3ConfigurationTypeDef, _OptionalReportS3ConfigurationTypeDef
 ):
     pass
 
+
 ResumeBatchLoadTaskRequestRequestTypeDef = TypedDict(
     "ResumeBatchLoadTaskRequestRequestTypeDef",
     {
         "TaskId": str,
     },
 )
 
@@ -463,19 +450,21 @@
     {
         "KmsKeyId": str,
         "Tags": Sequence[TagTypeDef],
     },
     total=False,
 )
 
+
 class CreateDatabaseRequestRequestTypeDef(
     _RequiredCreateDatabaseRequestRequestTypeDef, _OptionalCreateDatabaseRequestRequestTypeDef
 ):
     pass
 
+
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -532,19 +521,21 @@
     "_OptionalDataSourceConfigurationTypeDef",
     {
         "CsvConfiguration": CsvConfigurationTypeDef,
     },
     total=False,
 )
 
+
 class DataSourceConfigurationTypeDef(
     _RequiredDataSourceConfigurationTypeDef, _OptionalDataSourceConfigurationTypeDef
 ):
     pass
 
+
 DescribeEndpointsResponseTypeDef = TypedDict(
     "DescribeEndpointsResponseTypeDef",
     {
         "Endpoints": List[EndpointTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -585,45 +576,41 @@
         "SourceColumn": str,
         "TargetMeasureName": str,
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
     total=False,
 )
 
+
 class MixedMeasureMappingTypeDef(
     _RequiredMixedMeasureMappingTypeDef, _OptionalMixedMeasureMappingTypeDef
 ):
     pass
 
+
 _RequiredMultiMeasureMappingsTypeDef = TypedDict(
     "_RequiredMultiMeasureMappingsTypeDef",
     {
         "MultiMeasureAttributeMappings": Sequence[MultiMeasureAttributeMappingTypeDef],
     },
 )
 _OptionalMultiMeasureMappingsTypeDef = TypedDict(
     "_OptionalMultiMeasureMappingsTypeDef",
     {
         "TargetMultiMeasureName": str,
     },
     total=False,
 )
 
+
 class MultiMeasureMappingsTypeDef(
     _RequiredMultiMeasureMappingsTypeDef, _OptionalMultiMeasureMappingsTypeDef
 ):
     pass
 
-SchemaTypeDef = TypedDict(
-    "SchemaTypeDef",
-    {
-        "CompositePartitionKey": Sequence[PartitionKeyTypeDef],
-    },
-    total=False,
-)
 
 WriteRecordsResponseTypeDef = TypedDict(
     "WriteRecordsResponseTypeDef",
     {
         "RecordsIngested": RecordsIngestedTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -647,19 +634,21 @@
     "_OptionalMagneticStoreWritePropertiesTypeDef",
     {
         "MagneticStoreRejectedDataLocation": MagneticStoreRejectedDataLocationTypeDef,
     },
     total=False,
 )
 
+
 class MagneticStoreWritePropertiesTypeDef(
     _RequiredMagneticStoreWritePropertiesTypeDef, _OptionalMagneticStoreWritePropertiesTypeDef
 ):
     pass
 
+
 _RequiredWriteRecordsRequestRequestTypeDef = TypedDict(
     "_RequiredWriteRecordsRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
         "Records": Sequence[RecordTypeDef],
     },
@@ -668,19 +657,21 @@
     "_OptionalWriteRecordsRequestRequestTypeDef",
     {
         "CommonAttributes": RecordTypeDef,
     },
     total=False,
 )
 
+
 class WriteRecordsRequestRequestTypeDef(
     _RequiredWriteRecordsRequestRequestTypeDef, _OptionalWriteRecordsRequestRequestTypeDef
 ):
     pass
 
+
 _RequiredDataModelTypeDef = TypedDict(
     "_RequiredDataModelTypeDef",
     {
         "DimensionMappings": Sequence[DimensionMappingTypeDef],
     },
 )
 _OptionalDataModelTypeDef = TypedDict(
@@ -691,52 +682,54 @@
         "MultiMeasureMappings": MultiMeasureMappingsTypeDef,
         "MixedMeasureMappings": Sequence[MixedMeasureMappingTypeDef],
         "MeasureNameColumn": str,
     },
     total=False,
 )
 
+
 class DataModelTypeDef(_RequiredDataModelTypeDef, _OptionalDataModelTypeDef):
     pass
 
+
 _RequiredCreateTableRequestRequestTypeDef = TypedDict(
     "_RequiredCreateTableRequestRequestTypeDef",
     {
         "DatabaseName": str,
         "TableName": str,
     },
 )
 _OptionalCreateTableRequestRequestTypeDef = TypedDict(
     "_OptionalCreateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "Tags": Sequence[TagTypeDef],
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class CreateTableRequestRequestTypeDef(
     _RequiredCreateTableRequestRequestTypeDef, _OptionalCreateTableRequestRequestTypeDef
 ):
     pass
 
+
 TableTypeDef = TypedDict(
     "TableTypeDef",
     {
         "Arn": str,
         "TableName": str,
         "DatabaseName": str,
         "TableStatus": TableStatusType,
         "RetentionProperties": RetentionPropertiesTypeDef,
         "CreationTime": datetime,
         "LastUpdatedTime": datetime,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
 _RequiredUpdateTableRequestRequestTypeDef = TypedDict(
     "_RequiredUpdateTableRequestRequestTypeDef",
     {
@@ -745,24 +738,25 @@
     },
 )
 _OptionalUpdateTableRequestRequestTypeDef = TypedDict(
     "_OptionalUpdateTableRequestRequestTypeDef",
     {
         "RetentionProperties": RetentionPropertiesTypeDef,
         "MagneticStoreWriteProperties": MagneticStoreWritePropertiesTypeDef,
-        "Schema": SchemaTypeDef,
     },
     total=False,
 )
 
+
 class UpdateTableRequestRequestTypeDef(
     _RequiredUpdateTableRequestRequestTypeDef, _OptionalUpdateTableRequestRequestTypeDef
 ):
     pass
 
+
 DataModelConfigurationTypeDef = TypedDict(
     "DataModelConfigurationTypeDef",
     {
         "DataModel": DataModelTypeDef,
         "DataModelS3Configuration": DataModelS3ConfigurationTypeDef,
     },
     total=False,
@@ -836,20 +830,22 @@
         "ClientToken": str,
         "DataModelConfiguration": DataModelConfigurationTypeDef,
         "RecordVersion": int,
     },
     total=False,
 )
 
+
 class CreateBatchLoadTaskRequestRequestTypeDef(
     _RequiredCreateBatchLoadTaskRequestRequestTypeDef,
     _OptionalCreateBatchLoadTaskRequestRequestTypeDef,
 ):
     pass
 
+
 DescribeBatchLoadTaskResponseTypeDef = TypedDict(
     "DescribeBatchLoadTaskResponseTypeDef",
     {
         "BatchLoadTaskDescription": BatchLoadTaskDescriptionTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/PKG-INFO` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-timestream-write
-Version: 1.26.150
-Summary: Type annotations for boto3.TimestreamWrite 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.80
+Summary: Type annotations for boto3.TimestreamWrite 1.26.80 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-timestream-write"></a>
 
 # mypy-boto3-timestream-write
 
 [![PyPI - mypy-boto3-timestream-write](https://img.shields.io/pypi/v/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-timestream-write.svg?color=blue)](https://pypi.org/project/mypy-boto3-timestream-write)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-timestream-write?color=blue)](https://pypistats.org/packages/mypy-boto3-timestream-write)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.TimestreamWrite 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
+[boto3.TimestreamWrite 1.26.80](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/timestream-write.html#TimestreamWrite)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.14.5](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.12.4](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-timestream-write docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/).
 
 See how it helps to find and fix potential bugs:
 
@@ -281,16 +281,14 @@
 
 ```python
 from mypy_boto3_timestream_write.literals import (
     BatchLoadDataFormatType,
     BatchLoadStatusType,
     DimensionValueTypeType,
     MeasureValueTypeType,
-    PartitionKeyEnforcementLevelType,
-    PartitionKeyTypeType,
     S3EncryptionOptionType,
     ScalarMeasureValueTypeType,
     TableStatusType,
     TimeUnitType,
     TimestreamWriteServiceName,
     ServiceName,
     ResourceServiceName,
@@ -331,15 +329,14 @@
     ListBatchLoadTasksRequestRequestTypeDef,
     ListDatabasesRequestRequestTypeDef,
     ListTablesRequestRequestTypeDef,
     ListTagsForResourceRequestRequestTypeDef,
     S3ConfigurationTypeDef,
     MeasureValueTypeDef,
     MultiMeasureAttributeMappingTypeDef,
-    PartitionKeyTypeDef,
     RecordsIngestedTypeDef,
     ReportS3ConfigurationTypeDef,
     ResumeBatchLoadTaskRequestRequestTypeDef,
     UntagResourceRequestRequestTypeDef,
     UpdateDatabaseRequestRequestTypeDef,
     CreateBatchLoadTaskResponseTypeDef,
     EmptyResponseMetadataTypeDef,
@@ -353,15 +350,14 @@
     UpdateDatabaseResponseTypeDef,
     DataSourceConfigurationTypeDef,
     DescribeEndpointsResponseTypeDef,
     MagneticStoreRejectedDataLocationTypeDef,
     RecordTypeDef,
     MixedMeasureMappingTypeDef,
     MultiMeasureMappingsTypeDef,
-    SchemaTypeDef,
     WriteRecordsResponseTypeDef,
     ReportConfigurationTypeDef,
     MagneticStoreWritePropertiesTypeDef,
     WriteRecordsRequestRequestTypeDef,
     DataModelTypeDef,
     CreateTableRequestRequestTypeDef,
     TableTypeDef,
@@ -384,42 +380,42 @@
 <a id="how-it-works"></a>
 
 ## How it works
 
 Fully automated
 [mypy-boto3-builder](https://github.com/youtype/mypy_boto3_builder) carefully
 generates type annotations for each service, patiently waiting for `boto3`
-updates. It delivers drop-in type annotations for you and makes sure that:
+updates. It delivers a drop-in type annotations for you and makes sure that:
 
 - All available `boto3` services are covered.
 - Each public class and method of every `boto3` service gets valid type
-  annotations extracted from `botocore` schemas.
+  annotations extracted from the documentation (blame `botocore` docs if types
+  are incorrect).
 - Type annotations include up-to-date documentation.
 - Link to documentation is provided for every method.
 - Code is processed by [black](https://github.com/psf/black) and
   [isort](https://github.com/PyCQA/isort) for readability.
 
 <a id="what's-new"></a>
 
 ## What's new
 
 <a id="implemented-features"></a>
 
 ### Implemented features
 
-- Fully type annotated `boto3`, `botocore`, `aiobotocore` and `aioboto3`
-  libraries
+- Fully type annotated `boto3`, `botocore` and `aiobotocore` libraries
 - `mypy`, `pyright`, `VSCode`, `PyCharm`, `Sublime Text` and `Emacs`
   compatibility
 - `Client`, `ServiceResource`, `Resource`, `Waiter` `Paginator` type
   annotations for each service
 - Generated `TypeDefs` for each service
 - Generated `Literals` for each service
-- Auto discovery of types for `boto3.client` and `boto3.resource` calls
-- Auto discovery of types for `session.client` and `session.resource` calls
+- Auto discovery of types for `boto3.client` and `boto3.session` calls
+- Auto discovery of types for `session.client` and `session.session` calls
 - Auto discovery of types for `client.get_waiter` and `client.get_paginator`
   calls
 - Auto discovery of types for `ServiceResource` and `Resource` collections
 - Auto discovery of types for `aiobotocore.Session.create_client` calls
 
 <a id="latest-changes"></a>
```

### Comparing `mypy-boto3-timestream-write-1.26.150/mypy_boto3_timestream_write.egg-info/SOURCES.txt` & `mypy-boto3-timestream-write-1.26.80/mypy_boto3_timestream_write.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-timestream-write-1.26.150/setup.py` & `mypy-boto3-timestream-write-1.26.80/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-timestream-write.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-timestream-write",
-    version="1.26.150",
+    version="1.26.80",
     packages=["mypy_boto3_timestream_write"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.TimestreamWrite 1.26.150 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.TimestreamWrite 1.26.80 service generated with"
+        " mypy-boto3-builder 7.12.4"
     ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
@@ -45,11 +45,11 @@
     python_requires=">=3.7",
     project_urls={
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_timestream_write/",
         "Source": "https://github.com/youtype/mypy_boto3_builder",
         "Tracker": "https://github.com/youtype/mypy_boto3_builder/issues",
     },
     install_requires=[
-        'typing-extensions>=4.1.0; python_version<"3.9"',
+        "typing-extensions>=4.1.0",
     ],
     zip_safe=False,
 )
```

