# Comparing `tmp/mypy-boto3-servicecatalog-1.26.150.tar.gz` & `tmp/mypy-boto3-servicecatalog-1.26.79.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-servicecatalog-1.26.150.tar", last modified: Thu Jun  8 19:32:29 2023, max compression
+gzip compressed data, was "mypy-boto3-servicecatalog-1.26.79.tar", last modified: Fri Feb 24 21:22:49 2023, max compression
```

## Comparing `mypy-boto3-servicecatalog-1.26.150.tar` & `mypy-boto3-servicecatalog-1.26.79.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.735941 mypy-boto3-servicecatalog-1.26.150/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    27673 2023-06-08 19:32:29.735941 mypy-boto3-servicecatalog-1.26.150/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    26156 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.735941 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/
--rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      938 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    76162 2023-06-08 19:32:15.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    76049 2023-06-08 19:32:15.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/client.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14717 2023-06-08 19:32:15.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/literals.py
--rw-r--r--   0 runner    (1001) docker     (123)    14715 2023-06-08 19:32:15.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-06-08 19:32:15.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/paginator.py
--rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-06-08 19:32:15.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)   102689 2023-06-08 19:32:18.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (123)   102544 2023-06-08 19:32:16.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:32:29.735941 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    27673 2023-06-08 19:32:29.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-06-08 19:32:29.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:32:29.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:32:29.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 19:32:29.000000 mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:32:29.735941 mypy-boto3-servicecatalog-1.26.150/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-08 19:32:14.000000 mypy-boto3-servicecatalog-1.26.150/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.737199 mypy-boto3-servicecatalog-1.26.79/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    27349 2023-02-24 21:22:49.733199 mypy-boto3-servicecatalog-1.26.79/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    25834 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.729198 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/
+-rw-r--r--   0 runner    (1001) docker     (123)     4570 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      935 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73597 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73487 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14280 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14278 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    21847 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21828 2023-02-24 21:22:34.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    99234 2023-02-24 21:22:38.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99095 2023-02-24 21:22:36.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-24 21:22:49.733199 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    27349 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      813 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-02-24 21:22:49.000000 mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-24 21:22:49.737199 mypy-boto3-servicecatalog-1.26.79/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2045 2023-02-24 21:22:33.000000 mypy-boto3-servicecatalog-1.26.79/setup.py
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/LICENSE` & `mypy-boto3-servicecatalog-1.26.79/LICENSE`

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

### Comparing `mypy-boto3-servicecatalog-1.26.150/PKG-INFO` & `mypy-boto3-servicecatalog-1.26.79/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.26.150
-Summary: Type annotations for boto3.ServiceCatalog 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.79
+Summary: Type annotations for boto3.ServiceCatalog 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-servicecatalog"></a>
 
 # mypy-boto3-servicecatalog
 
 [![PyPI - mypy-boto3-servicecatalog](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,15 +362,14 @@
 from mypy_boto3_servicecatalog.literals import (
     AccessLevelFilterKeyType,
     AccessStatusType,
     ChangeActionType,
     CopyOptionType,
     CopyProductStatusType,
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     EvaluationTypeType,
     LastSyncStatusType,
     ListAcceptedPortfolioSharesPaginatorName,
     ListConstraintsForPortfolioPaginatorName,
     ListLaunchPathsPaginatorName,
     ListOrganizationPortfolioAccessPaginatorName,
     ListPortfoliosForProductPaginatorName,
@@ -496,15 +495,14 @@
     DescribeServiceActionInputRequestTypeDef,
     DescribeTagOptionInputRequestTypeDef,
     DisassociateBudgetFromResourceInputRequestTypeDef,
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
-    UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
     PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
@@ -525,15 +523,14 @@
     ResourceDetailTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
-    NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
@@ -581,14 +578,15 @@
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
     ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
+    DescribeProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
     ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
@@ -597,17 +595,15 @@
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
     DescribeProductViewOutputTypeDef,
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
-    NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
-    EngineWorkflowResourceIdentifierTypeDef,
     ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
     ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
@@ -637,19 +633,17 @@
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
     SearchProvisionedProductsOutputTypeDef,
     ListProvisioningArtifactsForServiceActionOutputTypeDef,
-    NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
     CreateServiceActionOutputTypeDef,
     DescribeServiceActionOutputTypeDef,
     UpdateServiceActionOutputTypeDef,
-    DescribeProvisioningArtifactOutputTypeDef,
     DescribeProvisioningParametersOutputTypeDef,
     DescribeRecordOutputTypeDef,
     ExecuteProvisionedProductPlanOutputTypeDef,
     ExecuteProvisionedProductServiceActionOutputTypeDef,
     ImportAsProvisionedProductOutputTypeDef,
     ListRecordHistoryOutputTypeDef,
     ProvisionProductOutputTypeDef,
@@ -675,42 +669,42 @@
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

### Comparing `mypy-boto3-servicecatalog-1.26.150/README.md` & `mypy-boto3-servicecatalog-1.26.79/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 <a id="mypy-boto3-servicecatalog"></a>
 
 # mypy-boto3-servicecatalog
 
 [![PyPI - mypy-boto3-servicecatalog](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -330,15 +330,14 @@
 from mypy_boto3_servicecatalog.literals import (
     AccessLevelFilterKeyType,
     AccessStatusType,
     ChangeActionType,
     CopyOptionType,
     CopyProductStatusType,
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     EvaluationTypeType,
     LastSyncStatusType,
     ListAcceptedPortfolioSharesPaginatorName,
     ListConstraintsForPortfolioPaginatorName,
     ListLaunchPathsPaginatorName,
     ListOrganizationPortfolioAccessPaginatorName,
     ListPortfoliosForProductPaginatorName,
@@ -464,15 +463,14 @@
     DescribeServiceActionInputRequestTypeDef,
     DescribeTagOptionInputRequestTypeDef,
     DisassociateBudgetFromResourceInputRequestTypeDef,
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
-    UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
     PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
@@ -493,15 +491,14 @@
     ResourceDetailTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
-    NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
@@ -549,14 +546,15 @@
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
     ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
+    DescribeProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
     ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
@@ -565,17 +563,15 @@
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
     DescribeProductViewOutputTypeDef,
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
-    NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
-    EngineWorkflowResourceIdentifierTypeDef,
     ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
     ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
@@ -605,19 +601,17 @@
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
     SearchProvisionedProductsOutputTypeDef,
     ListProvisioningArtifactsForServiceActionOutputTypeDef,
-    NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
     CreateServiceActionOutputTypeDef,
     DescribeServiceActionOutputTypeDef,
     UpdateServiceActionOutputTypeDef,
-    DescribeProvisioningArtifactOutputTypeDef,
     DescribeProvisioningParametersOutputTypeDef,
     DescribeRecordOutputTypeDef,
     ExecuteProvisionedProductPlanOutputTypeDef,
     ExecuteProvisionedProductServiceActionOutputTypeDef,
     ImportAsProvisionedProductOutputTypeDef,
     ListRecordHistoryOutputTypeDef,
     ProvisionProductOutputTypeDef,
@@ -643,42 +637,42 @@
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

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/__init__.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/__init__.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/__main__.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,28 +5,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ServiceCatalog 1.26.150\nVersion:         1.26.150\nBuilder"
-        " version: 7.14.5\nDocs:           "
+        "Type annotations for boto3.ServiceCatalog 1.26.79\nVersion:         1.26.79\nBuilder"
+        " version: 7.12.4\nDocs:           "
         " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog//\nBoto3 docs:     "
         " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog\nOther"
         " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
         " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.26.150")
+    print("1.26.79")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/client.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     OrganizationNodeTypeType,
     PortfolioShareTypeType,
     PrincipalTypeType,
     ProductTypeType,
     ProductViewFilterByType,
     ProductViewSortByType,
     PropertyKeyType,
@@ -76,15 +75,14 @@
     DescribeProvisionedProductPlanOutputTypeDef,
     DescribeProvisioningArtifactOutputTypeDef,
     DescribeProvisioningParametersOutputTypeDef,
     DescribeRecordOutputTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     DescribeServiceActionOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
-    EngineWorkflowResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanOutputTypeDef,
     ExecuteProvisionedProductServiceActionOutputTypeDef,
     GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     ImportAsProvisionedProductOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
@@ -107,15 +105,14 @@
     ListTagOptionsFiltersTypeDef,
     ListTagOptionsOutputTypeDef,
     OrganizationNodeTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     ProvisionProductOutputTypeDef,
-    RecordOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     SearchProductsOutputTypeDef,
     SearchProvisionedProductsOutputTypeDef,
     ServiceActionAssociationTypeDef,
     SourceConnectionTypeDef,
     TagTypeDef,
@@ -649,16 +646,15 @@
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisioningArtifactId: str = ...,
         ProductId: str = ...,
         ProvisioningArtifactName: str = ...,
         ProductName: str = ...,
-        Verbose: bool = ...,
-        IncludeProvisioningArtifactParameters: bool = ...
+        Verbose: bool = ...
     ) -> DescribeProvisioningArtifactOutputTypeDef:
         """
         Gets information about the specified provisioning artifact (also known as a
         version) for the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_provisioning_artifact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#describe_provisioning_artifact)
@@ -855,15 +851,15 @@
         ProvisionedProductId: str = ...,
         ProvisionedProductName: str = ...,
         OutputKeys: Sequence[str] = ...,
         PageSize: int = ...,
         PageToken: str = ...
     ) -> GetProvisionedProductOutputsOutputTypeDef:
         """
-        This API takes either a `ProvisonedProductId` or a `ProvisionedProductName`,
+        This API takes either a `ProvisonedProductId` or a `ProvisionedProductName` ,
         along with a list of one or more output keys, and responds with the key/value
         pairs of those outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.get_provisioned_product_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#get_provisioned_product_outputs)
         """
 
@@ -1009,16 +1005,16 @@
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
         PageToken: str = ...
     ) -> ListPrincipalsForPortfolioOutputTypeDef:
         """
-        Lists all `PrincipalARN`s and corresponding `PrincipalType`s associated with the
-        specified portfolio.
+        Lists all `PrincipalARN` s and corresponding `PrincipalType` s associated with
+        the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_principals_for_portfolio)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#list_principals_for_portfolio)
         """
 
     def list_provisioned_product_plans(
         self,
@@ -1148,65 +1144,14 @@
         """
         Lists the specified TagOptions or all TagOptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_tag_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#list_tag_options)
         """
 
-    def notify_provision_product_engine_workflow_result(
-        self,
-        *,
-        WorkflowToken: str,
-        RecordId: str,
-        Status: EngineWorkflowStatusType,
-        IdempotencyToken: str,
-        FailureReason: str = ...,
-        ResourceIdentifier: EngineWorkflowResourceIdentifierTypeDef = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
-    ) -> Dict[str, Any]:
-        """
-        Notifies the result of the provisioning engine execution.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_provision_product_engine_workflow_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#notify_provision_product_engine_workflow_result)
-        """
-
-    def notify_terminate_provisioned_product_engine_workflow_result(
-        self,
-        *,
-        WorkflowToken: str,
-        RecordId: str,
-        Status: EngineWorkflowStatusType,
-        IdempotencyToken: str,
-        FailureReason: str = ...
-    ) -> Dict[str, Any]:
-        """
-        Notifies the result of the terminate engine execution.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_terminate_provisioned_product_engine_workflow_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#notify_terminate_provisioned_product_engine_workflow_result)
-        """
-
-    def notify_update_provisioned_product_engine_workflow_result(
-        self,
-        *,
-        WorkflowToken: str,
-        RecordId: str,
-        Status: EngineWorkflowStatusType,
-        IdempotencyToken: str,
-        FailureReason: str = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
-    ) -> Dict[str, Any]:
-        """
-        Notifies the result of the update engine execution.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_update_provisioned_product_engine_workflow_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#notify_update_provisioned_product_engine_workflow_result)
-        """
-
     def provision_product(
         self,
         *,
         ProvisionedProductName: str,
         ProvisionToken: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/client.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 import sys
 from typing import Any, Dict, Mapping, Sequence, Type, overload
 
 from botocore.client import BaseClient, ClientMeta
 
 from .literals import (
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     OrganizationNodeTypeType,
     PortfolioShareTypeType,
     PrincipalTypeType,
     ProductTypeType,
     ProductViewFilterByType,
     ProductViewSortByType,
     PropertyKeyType,
@@ -76,15 +75,14 @@
     DescribeProvisionedProductPlanOutputTypeDef,
     DescribeProvisioningArtifactOutputTypeDef,
     DescribeProvisioningParametersOutputTypeDef,
     DescribeRecordOutputTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
     DescribeServiceActionOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
-    EngineWorkflowResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanOutputTypeDef,
     ExecuteProvisionedProductServiceActionOutputTypeDef,
     GetAWSOrganizationsAccessStatusOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
     ImportAsProvisionedProductOutputTypeDef,
     ListAcceptedPortfolioSharesOutputTypeDef,
     ListBudgetsForResourceOutputTypeDef,
@@ -107,15 +105,14 @@
     ListTagOptionsFiltersTypeDef,
     ListTagOptionsOutputTypeDef,
     OrganizationNodeTypeDef,
     ProvisioningArtifactPropertiesTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     ProvisionProductOutputTypeDef,
-    RecordOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     SearchProductsAsAdminOutputTypeDef,
     SearchProductsOutputTypeDef,
     SearchProvisionedProductsOutputTypeDef,
     ServiceActionAssociationTypeDef,
     SourceConnectionTypeDef,
     TagTypeDef,
@@ -607,16 +604,15 @@
         self,
         *,
         AcceptLanguage: str = ...,
         ProvisioningArtifactId: str = ...,
         ProductId: str = ...,
         ProvisioningArtifactName: str = ...,
         ProductName: str = ...,
-        Verbose: bool = ...,
-        IncludeProvisioningArtifactParameters: bool = ...
+        Verbose: bool = ...
     ) -> DescribeProvisioningArtifactOutputTypeDef:
         """
         Gets information about the specified provisioning artifact (also known as a
         version) for the specified product.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.describe_provisioning_artifact)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#describe_provisioning_artifact)
@@ -796,15 +792,15 @@
         ProvisionedProductId: str = ...,
         ProvisionedProductName: str = ...,
         OutputKeys: Sequence[str] = ...,
         PageSize: int = ...,
         PageToken: str = ...
     ) -> GetProvisionedProductOutputsOutputTypeDef:
         """
-        This API takes either a `ProvisonedProductId` or a `ProvisionedProductName`,
+        This API takes either a `ProvisonedProductId` or a `ProvisionedProductName` ,
         along with a list of one or more output keys, and responds with the key/value
         pairs of those outputs.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.get_provisioned_product_outputs)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#get_provisioned_product_outputs)
         """
     def import_as_provisioned_product(
@@ -940,16 +936,16 @@
         *,
         PortfolioId: str,
         AcceptLanguage: str = ...,
         PageSize: int = ...,
         PageToken: str = ...
     ) -> ListPrincipalsForPortfolioOutputTypeDef:
         """
-        Lists all `PrincipalARN`s and corresponding `PrincipalType`s associated with the
-        specified portfolio.
+        Lists all `PrincipalARN` s and corresponding `PrincipalType` s associated with
+        the specified portfolio.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_principals_for_portfolio)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#list_principals_for_portfolio)
         """
     def list_provisioned_product_plans(
         self,
         *,
@@ -1069,62 +1065,14 @@
     ) -> ListTagOptionsOutputTypeDef:
         """
         Lists the specified TagOptions or all TagOptions.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.list_tag_options)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#list_tag_options)
         """
-    def notify_provision_product_engine_workflow_result(
-        self,
-        *,
-        WorkflowToken: str,
-        RecordId: str,
-        Status: EngineWorkflowStatusType,
-        IdempotencyToken: str,
-        FailureReason: str = ...,
-        ResourceIdentifier: EngineWorkflowResourceIdentifierTypeDef = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
-    ) -> Dict[str, Any]:
-        """
-        Notifies the result of the provisioning engine execution.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_provision_product_engine_workflow_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#notify_provision_product_engine_workflow_result)
-        """
-    def notify_terminate_provisioned_product_engine_workflow_result(
-        self,
-        *,
-        WorkflowToken: str,
-        RecordId: str,
-        Status: EngineWorkflowStatusType,
-        IdempotencyToken: str,
-        FailureReason: str = ...
-    ) -> Dict[str, Any]:
-        """
-        Notifies the result of the terminate engine execution.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_terminate_provisioned_product_engine_workflow_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#notify_terminate_provisioned_product_engine_workflow_result)
-        """
-    def notify_update_provisioned_product_engine_workflow_result(
-        self,
-        *,
-        WorkflowToken: str,
-        RecordId: str,
-        Status: EngineWorkflowStatusType,
-        IdempotencyToken: str,
-        FailureReason: str = ...,
-        Outputs: Sequence[RecordOutputTypeDef] = ...
-    ) -> Dict[str, Any]:
-        """
-        Notifies the result of the update engine execution.
-
-        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog.Client.notify_update_provisioned_product_engine_workflow_result)
-        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/client/#notify_update_provisioned_product_engine_workflow_result)
-        """
     def provision_product(
         self,
         *,
         ProvisionedProductName: str,
         ProvisionToken: str,
         AcceptLanguage: str = ...,
         ProductId: str = ...,
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/literals.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 __all__ = (
     "AccessLevelFilterKeyType",
     "AccessStatusType",
     "ChangeActionType",
     "CopyOptionType",
     "CopyProductStatusType",
     "DescribePortfolioShareTypeType",
-    "EngineWorkflowStatusType",
     "EvaluationTypeType",
     "LastSyncStatusType",
     "ListAcceptedPortfolioSharesPaginatorName",
     "ListConstraintsForPortfolioPaginatorName",
     "ListLaunchPathsPaginatorName",
     "ListOrganizationPortfolioAccessPaginatorName",
     "ListPortfoliosForProductPaginatorName",
@@ -85,15 +84,14 @@
 AccessStatusType = Literal["DISABLED", "ENABLED", "UNDER_CHANGE"]
 ChangeActionType = Literal["ADD", "MODIFY", "REMOVE"]
 CopyOptionType = Literal["CopyTags"]
 CopyProductStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 DescribePortfolioShareTypeType = Literal[
     "ACCOUNT", "ORGANIZATION", "ORGANIZATIONAL_UNIT", "ORGANIZATION_MEMBER_ACCOUNT"
 ]
-EngineWorkflowStatusType = Literal["FAILED", "SUCCEEDED"]
 EvaluationTypeType = Literal["DYNAMIC", "STATIC"]
 LastSyncStatusType = Literal["FAILED", "SUCCEEDED"]
 ListAcceptedPortfolioSharesPaginatorName = Literal["list_accepted_portfolio_shares"]
 ListConstraintsForPortfolioPaginatorName = Literal["list_constraints_for_portfolio"]
 ListLaunchPathsPaginatorName = Literal["list_launch_paths"]
 ListOrganizationPortfolioAccessPaginatorName = Literal["list_organization_portfolio_access"]
 ListPortfoliosForProductPaginatorName = Literal["list_portfolios_for_product"]
@@ -110,15 +108,15 @@
 ]
 ListServiceActionsPaginatorName = Literal["list_service_actions"]
 ListTagOptionsPaginatorName = Literal["list_tag_options"]
 OrganizationNodeTypeType = Literal["ACCOUNT", "ORGANIZATION", "ORGANIZATIONAL_UNIT"]
 PortfolioShareTypeType = Literal["AWS_ORGANIZATIONS", "AWS_SERVICECATALOG", "IMPORTED"]
 PrincipalTypeType = Literal["IAM", "IAM_PATTERN"]
 ProductSourceType = Literal["ACCOUNT"]
-ProductTypeType = Literal["CLOUD_FORMATION_TEMPLATE", "MARKETPLACE", "TERRAFORM_OPEN_SOURCE"]
+ProductTypeType = Literal["CLOUD_FORMATION_TEMPLATE", "MARKETPLACE"]
 ProductViewFilterByType = Literal["FullTextSearch", "Owner", "ProductType", "SourceProductId"]
 ProductViewSortByType = Literal["CreationDate", "Title", "VersionCount"]
 PropertyKeyType = Literal["LAUNCH_ROLE", "OWNER"]
 ProvisionedProductPlanStatusType = Literal[
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_SUCCESS",
@@ -130,31 +128,26 @@
 ProvisionedProductStatusType = Literal[
     "AVAILABLE", "ERROR", "PLAN_IN_PROGRESS", "TAINTED", "UNDER_CHANGE"
 ]
 ProvisionedProductViewFilterByType = Literal["SearchQuery"]
 ProvisioningArtifactGuidanceType = Literal["DEFAULT", "DEPRECATED"]
 ProvisioningArtifactPropertyNameType = Literal["Id"]
 ProvisioningArtifactTypeType = Literal[
-    "CLOUD_FORMATION_TEMPLATE", "MARKETPLACE_AMI", "MARKETPLACE_CAR", "TERRAFORM_OPEN_SOURCE"
+    "CLOUD_FORMATION_TEMPLATE", "MARKETPLACE_AMI", "MARKETPLACE_CAR"
 ]
 RecordStatusType = Literal["CREATED", "FAILED", "IN_PROGRESS", "IN_PROGRESS_IN_ERROR", "SUCCEEDED"]
 ReplacementType = Literal["CONDITIONAL", "FALSE", "TRUE"]
 RequiresRecreationType = Literal["ALWAYS", "CONDITIONALLY", "NEVER"]
 ResourceAttributeType = Literal[
     "CREATIONPOLICY", "DELETIONPOLICY", "METADATA", "PROPERTIES", "TAGS", "UPDATEPOLICY"
 ]
 ScanProvisionedProductsPaginatorName = Literal["scan_provisioned_products"]
 SearchProductsAsAdminPaginatorName = Literal["search_products_as_admin"]
 ServiceActionAssociationErrorCodeType = Literal[
-    "DUPLICATE_RESOURCE",
-    "INTERNAL_FAILURE",
-    "INVALID_PARAMETER",
-    "LIMIT_EXCEEDED",
-    "RESOURCE_NOT_FOUND",
-    "THROTTLING",
+    "DUPLICATE_RESOURCE", "INTERNAL_FAILURE", "LIMIT_EXCEEDED", "RESOURCE_NOT_FOUND", "THROTTLING"
 ]
 ServiceActionDefinitionKeyType = Literal["AssumeRole", "Name", "Parameters", "Version"]
 ServiceActionDefinitionTypeType = Literal["SSM_AUTOMATION"]
 ShareStatusType = Literal[
     "COMPLETED", "COMPLETED_WITH_ERRORS", "ERROR", "IN_PROGRESS", "NOT_STARTED"
 ]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
@@ -307,15 +300,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -326,15 +318,14 @@
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
@@ -370,15 +361,14 @@
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
@@ -397,19 +387,16 @@
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
@@ -494,15 +481,14 @@
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
@@ -545,29 +531,24 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/literals.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/literals.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 __all__ = (
     "AccessLevelFilterKeyType",
     "AccessStatusType",
     "ChangeActionType",
     "CopyOptionType",
     "CopyProductStatusType",
     "DescribePortfolioShareTypeType",
-    "EngineWorkflowStatusType",
     "EvaluationTypeType",
     "LastSyncStatusType",
     "ListAcceptedPortfolioSharesPaginatorName",
     "ListConstraintsForPortfolioPaginatorName",
     "ListLaunchPathsPaginatorName",
     "ListOrganizationPortfolioAccessPaginatorName",
     "ListPortfoliosForProductPaginatorName",
@@ -83,15 +82,14 @@
 AccessStatusType = Literal["DISABLED", "ENABLED", "UNDER_CHANGE"]
 ChangeActionType = Literal["ADD", "MODIFY", "REMOVE"]
 CopyOptionType = Literal["CopyTags"]
 CopyProductStatusType = Literal["FAILED", "IN_PROGRESS", "SUCCEEDED"]
 DescribePortfolioShareTypeType = Literal[
     "ACCOUNT", "ORGANIZATION", "ORGANIZATIONAL_UNIT", "ORGANIZATION_MEMBER_ACCOUNT"
 ]
-EngineWorkflowStatusType = Literal["FAILED", "SUCCEEDED"]
 EvaluationTypeType = Literal["DYNAMIC", "STATIC"]
 LastSyncStatusType = Literal["FAILED", "SUCCEEDED"]
 ListAcceptedPortfolioSharesPaginatorName = Literal["list_accepted_portfolio_shares"]
 ListConstraintsForPortfolioPaginatorName = Literal["list_constraints_for_portfolio"]
 ListLaunchPathsPaginatorName = Literal["list_launch_paths"]
 ListOrganizationPortfolioAccessPaginatorName = Literal["list_organization_portfolio_access"]
 ListPortfoliosForProductPaginatorName = Literal["list_portfolios_for_product"]
@@ -108,15 +106,15 @@
 ]
 ListServiceActionsPaginatorName = Literal["list_service_actions"]
 ListTagOptionsPaginatorName = Literal["list_tag_options"]
 OrganizationNodeTypeType = Literal["ACCOUNT", "ORGANIZATION", "ORGANIZATIONAL_UNIT"]
 PortfolioShareTypeType = Literal["AWS_ORGANIZATIONS", "AWS_SERVICECATALOG", "IMPORTED"]
 PrincipalTypeType = Literal["IAM", "IAM_PATTERN"]
 ProductSourceType = Literal["ACCOUNT"]
-ProductTypeType = Literal["CLOUD_FORMATION_TEMPLATE", "MARKETPLACE", "TERRAFORM_OPEN_SOURCE"]
+ProductTypeType = Literal["CLOUD_FORMATION_TEMPLATE", "MARKETPLACE"]
 ProductViewFilterByType = Literal["FullTextSearch", "Owner", "ProductType", "SourceProductId"]
 ProductViewSortByType = Literal["CreationDate", "Title", "VersionCount"]
 PropertyKeyType = Literal["LAUNCH_ROLE", "OWNER"]
 ProvisionedProductPlanStatusType = Literal[
     "CREATE_FAILED",
     "CREATE_IN_PROGRESS",
     "CREATE_SUCCESS",
@@ -128,31 +126,26 @@
 ProvisionedProductStatusType = Literal[
     "AVAILABLE", "ERROR", "PLAN_IN_PROGRESS", "TAINTED", "UNDER_CHANGE"
 ]
 ProvisionedProductViewFilterByType = Literal["SearchQuery"]
 ProvisioningArtifactGuidanceType = Literal["DEFAULT", "DEPRECATED"]
 ProvisioningArtifactPropertyNameType = Literal["Id"]
 ProvisioningArtifactTypeType = Literal[
-    "CLOUD_FORMATION_TEMPLATE", "MARKETPLACE_AMI", "MARKETPLACE_CAR", "TERRAFORM_OPEN_SOURCE"
+    "CLOUD_FORMATION_TEMPLATE", "MARKETPLACE_AMI", "MARKETPLACE_CAR"
 ]
 RecordStatusType = Literal["CREATED", "FAILED", "IN_PROGRESS", "IN_PROGRESS_IN_ERROR", "SUCCEEDED"]
 ReplacementType = Literal["CONDITIONAL", "FALSE", "TRUE"]
 RequiresRecreationType = Literal["ALWAYS", "CONDITIONALLY", "NEVER"]
 ResourceAttributeType = Literal[
     "CREATIONPOLICY", "DELETIONPOLICY", "METADATA", "PROPERTIES", "TAGS", "UPDATEPOLICY"
 ]
 ScanProvisionedProductsPaginatorName = Literal["scan_provisioned_products"]
 SearchProductsAsAdminPaginatorName = Literal["search_products_as_admin"]
 ServiceActionAssociationErrorCodeType = Literal[
-    "DUPLICATE_RESOURCE",
-    "INTERNAL_FAILURE",
-    "INVALID_PARAMETER",
-    "LIMIT_EXCEEDED",
-    "RESOURCE_NOT_FOUND",
-    "THROTTLING",
+    "DUPLICATE_RESOURCE", "INTERNAL_FAILURE", "LIMIT_EXCEEDED", "RESOURCE_NOT_FOUND", "THROTTLING"
 ]
 ServiceActionDefinitionKeyType = Literal["AssumeRole", "Name", "Parameters", "Version"]
 ServiceActionDefinitionTypeType = Literal["SSM_AUTOMATION"]
 ShareStatusType = Literal[
     "COMPLETED", "COMPLETED_WITH_ERRORS", "ERROR", "IN_PROGRESS", "NOT_STARTED"
 ]
 SortOrderType = Literal["ASCENDING", "DESCENDING"]
@@ -305,15 +298,14 @@
     "honeycode",
     "iam",
     "identitystore",
     "imagebuilder",
     "importexport",
     "inspector",
     "inspector2",
-    "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
     "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
@@ -324,15 +316,14 @@
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
@@ -368,15 +359,14 @@
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
@@ -395,19 +385,16 @@
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
@@ -492,15 +479,14 @@
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
@@ -543,29 +529,24 @@
 RegionName = Literal[
     "af-south-1",
     "ap-east-1",
     "ap-northeast-1",
     "ap-northeast-2",
     "ap-northeast-3",
     "ap-south-1",
-    "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
-    "ap-southeast-4",
     "ca-central-1",
     "eu-central-1",
-    "eu-central-2",
     "eu-north-1",
     "eu-south-1",
-    "eu-south-2",
     "eu-west-1",
     "eu-west-2",
     "eu-west-3",
-    "me-central-1",
     "me-south-1",
     "sa-east-1",
     "us-east-1",
     "us-east-2",
     "us-west-1",
     "us-west-2",
 ]
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/paginator.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/paginator.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/type_defs.py` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from .literals import (
     AccessLevelFilterKeyType,
     AccessStatusType,
     ChangeActionType,
     CopyProductStatusType,
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     EvaluationTypeType,
     LastSyncStatusType,
     OrganizationNodeTypeType,
     PortfolioShareTypeType,
     PrincipalTypeType,
     ProductTypeType,
     ProductViewFilterByType,
@@ -121,15 +120,14 @@
     "DescribeServiceActionInputRequestTypeDef",
     "DescribeTagOptionInputRequestTypeDef",
     "DisassociateBudgetFromResourceInputRequestTypeDef",
     "DisassociatePrincipalFromPortfolioInputRequestTypeDef",
     "DisassociateProductFromPortfolioInputRequestTypeDef",
     "DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
-    "UniqueTagResourceIdentifierTypeDef",
     "ExecuteProvisionedProductPlanInputRequestTypeDef",
     "ExecuteProvisionedProductServiceActionInputRequestTypeDef",
     "GetProvisionedProductOutputsInputRequestTypeDef",
     "ImportAsProvisionedProductInputRequestTypeDef",
     "LastSyncTypeDef",
     "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
@@ -150,15 +148,14 @@
     "ResourceDetailTypeDef",
     "ListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     "ServiceActionSummaryTypeDef",
     "ListServiceActionsInputRequestTypeDef",
     "ListStackInstancesForProvisionedProductInputRequestTypeDef",
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
-    "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
@@ -206,14 +203,15 @@
     "UpdatePortfolioOutputTypeDef",
     "CreatePortfolioShareInputRequestTypeDef",
     "DeletePortfolioShareInputRequestTypeDef",
     "ListOrganizationPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareInputRequestTypeDef",
     "CreateProvisioningArtifactInputRequestTypeDef",
     "CreateProvisioningArtifactOutputTypeDef",
+    "DescribeProvisioningArtifactOutputTypeDef",
     "ListProvisioningArtifactsOutputTypeDef",
     "UpdateProvisioningArtifactOutputTypeDef",
     "CreateProvisionedProductPlanInputRequestTypeDef",
     "ProvisionedProductPlanDetailsTypeDef",
     "CreateTagOptionOutputTypeDef",
     "DescribePortfolioOutputTypeDef",
     "DescribeTagOptionOutputTypeDef",
@@ -222,17 +220,15 @@
     "DescribePortfolioSharesOutputTypeDef",
     "DescribeProductOutputTypeDef",
     "DescribeProductViewOutputTypeDef",
     "ProvisioningArtifactViewTypeDef",
     "DescribeProvisionedProductOutputTypeDef",
     "ScanProvisionedProductsOutputTypeDef",
     "GetProvisionedProductOutputsOutputTypeDef",
-    "NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "DescribeServiceActionExecutionParametersOutputTypeDef",
-    "EngineWorkflowResourceIdentifierTypeDef",
     "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
     "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
     "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
     "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
     "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
     "ListPortfoliosInputListPortfoliosPaginateTypeDef",
     "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
@@ -262,19 +258,17 @@
     "ShareDetailsTypeDef",
     "UpdateProvisionedProductInputRequestTypeDef",
     "SourceConnectionDetailTypeDef",
     "SourceConnectionTypeDef",
     "ListLaunchPathsOutputTypeDef",
     "SearchProvisionedProductsOutputTypeDef",
     "ListProvisioningArtifactsForServiceActionOutputTypeDef",
-    "NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
     "CreateServiceActionOutputTypeDef",
     "DescribeServiceActionOutputTypeDef",
     "UpdateServiceActionOutputTypeDef",
-    "DescribeProvisioningArtifactOutputTypeDef",
     "DescribeProvisioningParametersOutputTypeDef",
     "DescribeRecordOutputTypeDef",
     "ExecuteProvisionedProductPlanOutputTypeDef",
     "ExecuteProvisionedProductServiceActionOutputTypeDef",
     "ImportAsProvisionedProductOutputTypeDef",
     "ListRecordHistoryOutputTypeDef",
     "ProvisionProductOutputTypeDef",
@@ -1053,15 +1047,14 @@
     {
         "AcceptLanguage": str,
         "ProvisioningArtifactId": str,
         "ProductId": str,
         "ProvisioningArtifactName": str,
         "ProductName": str,
         "Verbose": bool,
-        "IncludeProvisioningArtifactParameters": bool,
     },
     total=False,
 )
 
 DescribeProvisioningParametersInputRequestTypeDef = TypedDict(
     "DescribeProvisioningParametersInputRequestTypeDef",
     {
@@ -1290,23 +1283,14 @@
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagOptionId": str,
     },
 )
 
-UniqueTagResourceIdentifierTypeDef = TypedDict(
-    "UniqueTagResourceIdentifierTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredExecuteProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredExecuteProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanId": str,
         "IdempotencyToken": str,
     },
 )
@@ -1801,39 +1785,14 @@
         "Key": str,
         "Value": str,
         "Active": bool,
     },
     total=False,
 )
 
-_RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "WorkflowToken": str,
-        "RecordId": str,
-        "Status": EngineWorkflowStatusType,
-        "IdempotencyToken": str,
-    },
-)
-_OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "FailureReason": str,
-    },
-    total=False,
-)
-
-
-class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
-    _RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    _OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-):
-    pass
-
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
         "AllowedPattern": str,
         "ConstraintDescription": str,
         "MaxLength": str,
@@ -2608,14 +2567,24 @@
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeProvisioningArtifactOutputTypeDef = TypedDict(
+    "DescribeProvisioningArtifactOutputTypeDef",
+    {
+        "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
+        "Info": Dict[str, str],
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListProvisioningArtifactsOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsOutputTypeDef",
     {
         "ProvisioningArtifactDetails": List[ProvisioningArtifactDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2789,56 +2758,22 @@
     {
         "Outputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "WorkflowToken": str,
-        "RecordId": str,
-        "Status": EngineWorkflowStatusType,
-        "IdempotencyToken": str,
-    },
-)
-_OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "FailureReason": str,
-        "Outputs": Sequence[RecordOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
-    _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    _OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-):
-    pass
-
-
 DescribeServiceActionExecutionParametersOutputTypeDef = TypedDict(
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     {
         "ServiceActionParameters": List[ExecutionParameterTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EngineWorkflowResourceIdentifierTypeDef = TypedDict(
-    "EngineWorkflowResourceIdentifierTypeDef",
-    {
-        "UniqueTag": UniqueTagResourceIdentifierTypeDef,
-    },
-    total=False,
-)
-
 ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
     {
         "AcceptLanguage": str,
         "PortfolioShareType": PortfolioShareTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3371,41 +3306,14 @@
     {
         "ProvisioningArtifactViews": List[ProvisioningArtifactViewTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "WorkflowToken": str,
-        "RecordId": str,
-        "Status": EngineWorkflowStatusType,
-        "IdempotencyToken": str,
-    },
-)
-_OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "FailureReason": str,
-        "ResourceIdentifier": EngineWorkflowResourceIdentifierTypeDef,
-        "Outputs": Sequence[RecordOutputTypeDef],
-    },
-    total=False,
-)
-
-
-class NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef(
-    _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
-    _OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
-):
-    pass
-
-
 CreateServiceActionOutputTypeDef = TypedDict(
     "CreateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3422,25 +3330,14 @@
     "UpdateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeProvisioningArtifactOutputTypeDef = TypedDict(
-    "DescribeProvisioningArtifactOutputTypeDef",
-    {
-        "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
-        "Info": Dict[str, str],
-        "Status": StatusType,
-        "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeProvisioningParametersOutputTypeDef = TypedDict(
     "DescribeProvisioningParametersOutputTypeDef",
     {
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "UsageInstructions": List[UsageInstructionTypeDef],
         "TagOptions": List[TagOptionSummaryTypeDef],
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog/type_defs.pyi` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog/type_defs.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,14 @@
 
 from .literals import (
     AccessLevelFilterKeyType,
     AccessStatusType,
     ChangeActionType,
     CopyProductStatusType,
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     EvaluationTypeType,
     LastSyncStatusType,
     OrganizationNodeTypeType,
     PortfolioShareTypeType,
     PrincipalTypeType,
     ProductTypeType,
     ProductViewFilterByType,
@@ -120,15 +119,14 @@
     "DescribeServiceActionInputRequestTypeDef",
     "DescribeTagOptionInputRequestTypeDef",
     "DisassociateBudgetFromResourceInputRequestTypeDef",
     "DisassociatePrincipalFromPortfolioInputRequestTypeDef",
     "DisassociateProductFromPortfolioInputRequestTypeDef",
     "DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef",
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
-    "UniqueTagResourceIdentifierTypeDef",
     "ExecuteProvisionedProductPlanInputRequestTypeDef",
     "ExecuteProvisionedProductServiceActionInputRequestTypeDef",
     "GetProvisionedProductOutputsInputRequestTypeDef",
     "ImportAsProvisionedProductInputRequestTypeDef",
     "LastSyncTypeDef",
     "PaginatorConfigTypeDef",
     "ListAcceptedPortfolioSharesInputRequestTypeDef",
@@ -149,15 +147,14 @@
     "ResourceDetailTypeDef",
     "ListServiceActionsForProvisioningArtifactInputRequestTypeDef",
     "ServiceActionSummaryTypeDef",
     "ListServiceActionsInputRequestTypeDef",
     "ListStackInstancesForProvisionedProductInputRequestTypeDef",
     "StackInstanceTypeDef",
     "ListTagOptionsFiltersTypeDef",
-    "NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "ParameterConstraintsTypeDef",
     "ProductViewAggregationValueTypeDef",
     "ProvisioningParameterTypeDef",
     "ProvisioningPreferencesTypeDef",
     "RecordErrorTypeDef",
     "RecordTagTypeDef",
     "RejectPortfolioShareInputRequestTypeDef",
@@ -205,14 +202,15 @@
     "UpdatePortfolioOutputTypeDef",
     "CreatePortfolioShareInputRequestTypeDef",
     "DeletePortfolioShareInputRequestTypeDef",
     "ListOrganizationPortfolioAccessOutputTypeDef",
     "UpdatePortfolioShareInputRequestTypeDef",
     "CreateProvisioningArtifactInputRequestTypeDef",
     "CreateProvisioningArtifactOutputTypeDef",
+    "DescribeProvisioningArtifactOutputTypeDef",
     "ListProvisioningArtifactsOutputTypeDef",
     "UpdateProvisioningArtifactOutputTypeDef",
     "CreateProvisionedProductPlanInputRequestTypeDef",
     "ProvisionedProductPlanDetailsTypeDef",
     "CreateTagOptionOutputTypeDef",
     "DescribePortfolioOutputTypeDef",
     "DescribeTagOptionOutputTypeDef",
@@ -221,17 +219,15 @@
     "DescribePortfolioSharesOutputTypeDef",
     "DescribeProductOutputTypeDef",
     "DescribeProductViewOutputTypeDef",
     "ProvisioningArtifactViewTypeDef",
     "DescribeProvisionedProductOutputTypeDef",
     "ScanProvisionedProductsOutputTypeDef",
     "GetProvisionedProductOutputsOutputTypeDef",
-    "NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
     "DescribeServiceActionExecutionParametersOutputTypeDef",
-    "EngineWorkflowResourceIdentifierTypeDef",
     "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
     "ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef",
     "ListLaunchPathsInputListLaunchPathsPaginateTypeDef",
     "ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef",
     "ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef",
     "ListPortfoliosInputListPortfoliosPaginateTypeDef",
     "ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef",
@@ -261,19 +257,17 @@
     "ShareDetailsTypeDef",
     "UpdateProvisionedProductInputRequestTypeDef",
     "SourceConnectionDetailTypeDef",
     "SourceConnectionTypeDef",
     "ListLaunchPathsOutputTypeDef",
     "SearchProvisionedProductsOutputTypeDef",
     "ListProvisioningArtifactsForServiceActionOutputTypeDef",
-    "NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
     "CreateServiceActionOutputTypeDef",
     "DescribeServiceActionOutputTypeDef",
     "UpdateServiceActionOutputTypeDef",
-    "DescribeProvisioningArtifactOutputTypeDef",
     "DescribeProvisioningParametersOutputTypeDef",
     "DescribeRecordOutputTypeDef",
     "ExecuteProvisionedProductPlanOutputTypeDef",
     "ExecuteProvisionedProductServiceActionOutputTypeDef",
     "ImportAsProvisionedProductOutputTypeDef",
     "ListRecordHistoryOutputTypeDef",
     "ProvisionProductOutputTypeDef",
@@ -1014,15 +1008,14 @@
     {
         "AcceptLanguage": str,
         "ProvisioningArtifactId": str,
         "ProductId": str,
         "ProvisioningArtifactName": str,
         "ProductName": str,
         "Verbose": bool,
-        "IncludeProvisioningArtifactParameters": bool,
     },
     total=False,
 )
 
 DescribeProvisioningParametersInputRequestTypeDef = TypedDict(
     "DescribeProvisioningParametersInputRequestTypeDef",
     {
@@ -1239,23 +1232,14 @@
     "DisassociateTagOptionFromResourceInputRequestTypeDef",
     {
         "ResourceId": str,
         "TagOptionId": str,
     },
 )
 
-UniqueTagResourceIdentifierTypeDef = TypedDict(
-    "UniqueTagResourceIdentifierTypeDef",
-    {
-        "Key": str,
-        "Value": str,
-    },
-    total=False,
-)
-
 _RequiredExecuteProvisionedProductPlanInputRequestTypeDef = TypedDict(
     "_RequiredExecuteProvisionedProductPlanInputRequestTypeDef",
     {
         "PlanId": str,
         "IdempotencyToken": str,
     },
 )
@@ -1720,37 +1704,14 @@
         "Key": str,
         "Value": str,
         "Active": bool,
     },
     total=False,
 )
 
-_RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "WorkflowToken": str,
-        "RecordId": str,
-        "Status": EngineWorkflowStatusType,
-        "IdempotencyToken": str,
-    },
-)
-_OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "FailureReason": str,
-    },
-    total=False,
-)
-
-class NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
-    _RequiredNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    _OptionalNotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-):
-    pass
-
 ParameterConstraintsTypeDef = TypedDict(
     "ParameterConstraintsTypeDef",
     {
         "AllowedValues": List[str],
         "AllowedPattern": str,
         "ConstraintDescription": str,
         "MaxLength": str,
@@ -2495,14 +2456,24 @@
         "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
         "Info": Dict[str, str],
         "Status": StatusType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
+DescribeProvisioningArtifactOutputTypeDef = TypedDict(
+    "DescribeProvisioningArtifactOutputTypeDef",
+    {
+        "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
+        "Info": Dict[str, str],
+        "Status": StatusType,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+
 ListProvisioningArtifactsOutputTypeDef = TypedDict(
     "ListProvisioningArtifactsOutputTypeDef",
     {
         "ProvisioningArtifactDetails": List[ProvisioningArtifactDetailTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
@@ -2674,54 +2645,22 @@
     {
         "Outputs": List[RecordOutputTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "WorkflowToken": str,
-        "RecordId": str,
-        "Status": EngineWorkflowStatusType,
-        "IdempotencyToken": str,
-    },
-)
-_OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "FailureReason": str,
-        "Outputs": Sequence[RecordOutputTypeDef],
-    },
-    total=False,
-)
-
-class NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef(
-    _RequiredNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-    _OptionalNotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
-):
-    pass
-
 DescribeServiceActionExecutionParametersOutputTypeDef = TypedDict(
     "DescribeServiceActionExecutionParametersOutputTypeDef",
     {
         "ServiceActionParameters": List[ExecutionParameterTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-EngineWorkflowResourceIdentifierTypeDef = TypedDict(
-    "EngineWorkflowResourceIdentifierTypeDef",
-    {
-        "UniqueTag": UniqueTagResourceIdentifierTypeDef,
-    },
-    total=False,
-)
-
 ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef = TypedDict(
     "ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef",
     {
         "AcceptLanguage": str,
         "PortfolioShareType": PortfolioShareTypeType,
         "PaginationConfig": PaginatorConfigTypeDef,
     },
@@ -3232,39 +3171,14 @@
     {
         "ProvisioningArtifactViews": List[ProvisioningArtifactViewTypeDef],
         "NextPageToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "WorkflowToken": str,
-        "RecordId": str,
-        "Status": EngineWorkflowStatusType,
-        "IdempotencyToken": str,
-    },
-)
-_OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef = TypedDict(
-    "_OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef",
-    {
-        "FailureReason": str,
-        "ResourceIdentifier": EngineWorkflowResourceIdentifierTypeDef,
-        "Outputs": Sequence[RecordOutputTypeDef],
-    },
-    total=False,
-)
-
-class NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef(
-    _RequiredNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
-    _OptionalNotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
-):
-    pass
-
 CreateServiceActionOutputTypeDef = TypedDict(
     "CreateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
@@ -3281,25 +3195,14 @@
     "UpdateServiceActionOutputTypeDef",
     {
         "ServiceActionDetail": ServiceActionDetailTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 
-DescribeProvisioningArtifactOutputTypeDef = TypedDict(
-    "DescribeProvisioningArtifactOutputTypeDef",
-    {
-        "ProvisioningArtifactDetail": ProvisioningArtifactDetailTypeDef,
-        "Info": Dict[str, str],
-        "Status": StatusType,
-        "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-
 DescribeProvisioningParametersOutputTypeDef = TypedDict(
     "DescribeProvisioningParametersOutputTypeDef",
     {
         "ProvisioningArtifactParameters": List[ProvisioningArtifactParameterTypeDef],
         "ConstraintSummaries": List[ConstraintSummaryTypeDef],
         "UsageInstructions": List[UsageInstructionTypeDef],
         "TagOptions": List[TagOptionSummaryTypeDef],
```

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/PKG-INFO` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-servicecatalog
-Version: 1.26.150
-Summary: Type annotations for boto3.ServiceCatalog 1.26.150 service generated with mypy-boto3-builder 7.14.5
+Version: 1.26.79
+Summary: Type annotations for boto3.ServiceCatalog 1.26.79 service generated with mypy-boto3-builder 7.12.4
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -32,30 +32,30 @@
 
 <a id="mypy-boto3-servicecatalog"></a>
 
 # mypy-boto3-servicecatalog
 
 [![PyPI - mypy-boto3-servicecatalog](https://img.shields.io/pypi/v/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-servicecatalog.svg?color=blue)](https://pypi.org/project/mypy-boto3-servicecatalog)
-[![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/)
+[![Docs](https://img.shields.io/readthedocs/mypy-boto3-builder.svg?color=blue)](https://mypy-boto3-builder.readthedocs.io/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/mypy-boto3-servicecatalog?color=blue)](https://pypistats.org/packages/mypy-boto3-servicecatalog)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ServiceCatalog 1.26.150](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
+[boto3.ServiceCatalog 1.26.79](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/servicecatalog.html#ServiceCatalog)
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
 [mypy-boto3-servicecatalog docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/).
 
 See how it helps to find and fix potential bugs:
 
@@ -362,15 +362,14 @@
 from mypy_boto3_servicecatalog.literals import (
     AccessLevelFilterKeyType,
     AccessStatusType,
     ChangeActionType,
     CopyOptionType,
     CopyProductStatusType,
     DescribePortfolioShareTypeType,
-    EngineWorkflowStatusType,
     EvaluationTypeType,
     LastSyncStatusType,
     ListAcceptedPortfolioSharesPaginatorName,
     ListConstraintsForPortfolioPaginatorName,
     ListLaunchPathsPaginatorName,
     ListOrganizationPortfolioAccessPaginatorName,
     ListPortfoliosForProductPaginatorName,
@@ -496,15 +495,14 @@
     DescribeServiceActionInputRequestTypeDef,
     DescribeTagOptionInputRequestTypeDef,
     DisassociateBudgetFromResourceInputRequestTypeDef,
     DisassociatePrincipalFromPortfolioInputRequestTypeDef,
     DisassociateProductFromPortfolioInputRequestTypeDef,
     DisassociateServiceActionFromProvisioningArtifactInputRequestTypeDef,
     DisassociateTagOptionFromResourceInputRequestTypeDef,
-    UniqueTagResourceIdentifierTypeDef,
     ExecuteProvisionedProductPlanInputRequestTypeDef,
     ExecuteProvisionedProductServiceActionInputRequestTypeDef,
     GetProvisionedProductOutputsInputRequestTypeDef,
     ImportAsProvisionedProductInputRequestTypeDef,
     LastSyncTypeDef,
     PaginatorConfigTypeDef,
     ListAcceptedPortfolioSharesInputRequestTypeDef,
@@ -525,15 +523,14 @@
     ResourceDetailTypeDef,
     ListServiceActionsForProvisioningArtifactInputRequestTypeDef,
     ServiceActionSummaryTypeDef,
     ListServiceActionsInputRequestTypeDef,
     ListStackInstancesForProvisionedProductInputRequestTypeDef,
     StackInstanceTypeDef,
     ListTagOptionsFiltersTypeDef,
-    NotifyTerminateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     ParameterConstraintsTypeDef,
     ProductViewAggregationValueTypeDef,
     ProvisioningParameterTypeDef,
     ProvisioningPreferencesTypeDef,
     RecordErrorTypeDef,
     RecordTagTypeDef,
     RejectPortfolioShareInputRequestTypeDef,
@@ -581,14 +578,15 @@
     UpdatePortfolioOutputTypeDef,
     CreatePortfolioShareInputRequestTypeDef,
     DeletePortfolioShareInputRequestTypeDef,
     ListOrganizationPortfolioAccessOutputTypeDef,
     UpdatePortfolioShareInputRequestTypeDef,
     CreateProvisioningArtifactInputRequestTypeDef,
     CreateProvisioningArtifactOutputTypeDef,
+    DescribeProvisioningArtifactOutputTypeDef,
     ListProvisioningArtifactsOutputTypeDef,
     UpdateProvisioningArtifactOutputTypeDef,
     CreateProvisionedProductPlanInputRequestTypeDef,
     ProvisionedProductPlanDetailsTypeDef,
     CreateTagOptionOutputTypeDef,
     DescribePortfolioOutputTypeDef,
     DescribeTagOptionOutputTypeDef,
@@ -597,17 +595,15 @@
     DescribePortfolioSharesOutputTypeDef,
     DescribeProductOutputTypeDef,
     DescribeProductViewOutputTypeDef,
     ProvisioningArtifactViewTypeDef,
     DescribeProvisionedProductOutputTypeDef,
     ScanProvisionedProductsOutputTypeDef,
     GetProvisionedProductOutputsOutputTypeDef,
-    NotifyUpdateProvisionedProductEngineWorkflowResultInputRequestTypeDef,
     DescribeServiceActionExecutionParametersOutputTypeDef,
-    EngineWorkflowResourceIdentifierTypeDef,
     ListAcceptedPortfolioSharesInputListAcceptedPortfolioSharesPaginateTypeDef,
     ListConstraintsForPortfolioInputListConstraintsForPortfolioPaginateTypeDef,
     ListLaunchPathsInputListLaunchPathsPaginateTypeDef,
     ListOrganizationPortfolioAccessInputListOrganizationPortfolioAccessPaginateTypeDef,
     ListPortfoliosForProductInputListPortfoliosForProductPaginateTypeDef,
     ListPortfoliosInputListPortfoliosPaginateTypeDef,
     ListPrincipalsForPortfolioInputListPrincipalsForPortfolioPaginateTypeDef,
@@ -637,19 +633,17 @@
     ShareDetailsTypeDef,
     UpdateProvisionedProductInputRequestTypeDef,
     SourceConnectionDetailTypeDef,
     SourceConnectionTypeDef,
     ListLaunchPathsOutputTypeDef,
     SearchProvisionedProductsOutputTypeDef,
     ListProvisioningArtifactsForServiceActionOutputTypeDef,
-    NotifyProvisionProductEngineWorkflowResultInputRequestTypeDef,
     CreateServiceActionOutputTypeDef,
     DescribeServiceActionOutputTypeDef,
     UpdateServiceActionOutputTypeDef,
-    DescribeProvisioningArtifactOutputTypeDef,
     DescribeProvisioningParametersOutputTypeDef,
     DescribeRecordOutputTypeDef,
     ExecuteProvisionedProductPlanOutputTypeDef,
     ExecuteProvisionedProductServiceActionOutputTypeDef,
     ImportAsProvisionedProductOutputTypeDef,
     ListRecordHistoryOutputTypeDef,
     ProvisionProductOutputTypeDef,
@@ -675,42 +669,42 @@
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

### Comparing `mypy-boto3-servicecatalog-1.26.150/mypy_boto3_servicecatalog.egg-info/SOURCES.txt` & `mypy-boto3-servicecatalog-1.26.79/mypy_boto3_servicecatalog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-servicecatalog-1.26.150/setup.py` & `mypy-boto3-servicecatalog-1.26.79/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 """
 Setup script for mypy-boto3-servicecatalog.
 """
-from pathlib import Path
+from os.path import abspath, dirname
 
 from setuptools import setup
 
-LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
+LONG_DESCRIPTION = open(dirname(abspath(__file__)) + "/README.md", "r").read()
 
 
 setup(
     name="mypy-boto3-servicecatalog",
-    version="1.26.150",
+    version="1.26.79",
     packages=["mypy_boto3_servicecatalog"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
     description=(
-        "Type annotations for boto3.ServiceCatalog 1.26.150 service generated with"
-        " mypy-boto3-builder 7.14.5"
+        "Type annotations for boto3.ServiceCatalog 1.26.79 service generated with"
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
         "Documentation": "https://youtype.github.io/boto3_stubs_docs/mypy_boto3_servicecatalog/",
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

