# Comparing `tmp/kodexa-6.2.25210074074.tar.gz` & `tmp/kodexa-6.2.25211422458.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kodexa-6.2.25210074074.tar", max compression
+gzip compressed data, was "kodexa-6.2.25211422458.tar", max compression
```

## Comparing `kodexa-6.2.25210074074.tar` & `kodexa-6.2.25211422458.tar`

### file list

```diff
@@ -1,41 +1,41 @@
--rw-r--r--   0        0        0    11357 2023-06-08 10:18:48.175210 kodexa-6.2.25210074074/LICENSE
--rw-r--r--   0        0        0     2804 2023-06-08 10:18:48.175210 kodexa-6.2.25210074074/README.md
--rw-r--r--   0        0        0      847 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/__init__.py
--rw-r--r--   0        0        0      171 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/assistant/__init__.py
--rw-r--r--   0        0        0    12530 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/assistant/assistant.py
--rw-r--r--   0        0        0      297 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/connectors/__init__.py
--rw-r--r--   0        0        0     7722 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/connectors/connectors.py
--rw-r--r--   0        0        0      720 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/model/__init__.py
--rw-r--r--   0        0        0      753 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/model/base.py
--rw-r--r--   0        0        0    96316 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/model/model.py
--rw-r--r--   0        0        0   118285 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/model/objects.py
--rw-r--r--   0        0        0    38334 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/model/persistence.py
--rw-r--r--   0        0        0      236 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/pipeline/__init__.py
--rw-r--r--   0        0        0    19763 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/pipeline/pipeline.py
--rw-r--r--   0        0        0      216 2023-06-08 10:18:48.183211 kodexa-6.2.25210074074/kodexa/platform/__init__.py
--rw-r--r--   0        0        0   111822 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/platform/client.py
--rw-r--r--   0        0        0    26888 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/platform/kodexa.py
--rw-r--r--   0        0        0      100 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/__init__.py
--rw-r--r--   0        0        0    13499 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/ast.py
--rw-r--r--   0        0        0     3698 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/core.py
--rw-r--r--   0        0        0     3735 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/lexrules.py
--rw-r--r--   0        0        0     2354 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/lextab.py
--rw-r--r--   0        0        0       60 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/lextab.pyi
--rw-r--r--   0        0        0     7054 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/parserules.py
--rw-r--r--   0        0        0       60 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/parserules.pyi
--rw-r--r--   0        0        0    21267 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/parsetab.py
--rw-r--r--   0        0        0       60 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/selectors/parsetab.pyi
--rw-r--r--   0        0        0        0 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/spatial/__init__.py
--rw-r--r--   0        0        0    18991 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/spatial/azure_models.py
--rw-r--r--   0        0        0     2738 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/spatial/bbox_common.py
--rw-r--r--   0        0        0    34222 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/spatial/table_form_common.py
--rw-r--r--   0        0        0      160 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/steps/__init__.py
--rw-r--r--   0        0        0     9587 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/steps/common.py
--rw-r--r--   0        0        0      159 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/testing/__init__.py
--rw-r--r--   0        0        0      932 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/testing/test_components.py
--rw-r--r--   0        0        0    13596 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/testing/test_utils.py
--rw-r--r--   0        0        0       52 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/training/__init__.py
--rw-r--r--   0        0        0        0 2023-06-08 10:18:48.187211 kodexa-6.2.25210074074/kodexa/training/train_utils.py
--rw-r--r--   0        0        0     1301 2023-06-08 10:19:08.977219 kodexa-6.2.25210074074/pyproject.toml
--rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25210074074/setup.py
--rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25210074074/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 12:52:40.629282 kodexa-6.2.25211422458/LICENSE
+-rw-r--r--   0        0        0     2804 2023-06-08 12:52:40.629282 kodexa-6.2.25211422458/README.md
+-rw-r--r--   0        0        0      847 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/__init__.py
+-rw-r--r--   0        0        0      171 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/assistant/__init__.py
+-rw-r--r--   0        0        0    12530 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/assistant/assistant.py
+-rw-r--r--   0        0        0      297 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/connectors/__init__.py
+-rw-r--r--   0        0        0     7722 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/connectors/connectors.py
+-rw-r--r--   0        0        0      720 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/model/__init__.py
+-rw-r--r--   0        0        0      753 2023-06-08 12:52:40.637282 kodexa-6.2.25211422458/kodexa/model/base.py
+-rw-r--r--   0        0        0    96316 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/model/model.py
+-rw-r--r--   0        0        0   118104 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/model/objects.py
+-rw-r--r--   0        0        0    38334 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/model/persistence.py
+-rw-r--r--   0        0        0      236 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/pipeline/__init__.py
+-rw-r--r--   0        0        0    19763 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/pipeline/pipeline.py
+-rw-r--r--   0        0        0      216 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/platform/__init__.py
+-rw-r--r--   0        0        0   111822 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/platform/client.py
+-rw-r--r--   0        0        0    26888 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/platform/kodexa.py
+-rw-r--r--   0        0        0      100 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/__init__.py
+-rw-r--r--   0        0        0    13499 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/ast.py
+-rw-r--r--   0        0        0     3698 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/core.py
+-rw-r--r--   0        0        0     3735 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/lexrules.py
+-rw-r--r--   0        0        0     2354 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/lextab.py
+-rw-r--r--   0        0        0       60 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/lextab.pyi
+-rw-r--r--   0        0        0     7054 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parserules.py
+-rw-r--r--   0        0        0       60 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parserules.pyi
+-rw-r--r--   0        0        0    21267 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parsetab.py
+-rw-r--r--   0        0        0       60 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/selectors/parsetab.pyi
+-rw-r--r--   0        0        0        0 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/__init__.py
+-rw-r--r--   0        0        0    18991 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/azure_models.py
+-rw-r--r--   0        0        0     2738 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/bbox_common.py
+-rw-r--r--   0        0        0    34222 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/spatial/table_form_common.py
+-rw-r--r--   0        0        0      160 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/steps/__init__.py
+-rw-r--r--   0        0        0     9587 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/steps/common.py
+-rw-r--r--   0        0        0      159 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/testing/__init__.py
+-rw-r--r--   0        0        0      932 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/testing/test_components.py
+-rw-r--r--   0        0        0    13596 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/testing/test_utils.py
+-rw-r--r--   0        0        0       52 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/training/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 12:52:40.641282 kodexa-6.2.25211422458/kodexa/training/train_utils.py
+-rw-r--r--   0        0        0     1301 2023-06-08 12:53:00.681660 kodexa-6.2.25211422458/pyproject.toml
+-rw-r--r--   0        0        0     4103 1970-01-01 00:00:00.000000 kodexa-6.2.25211422458/setup.py
+-rw-r--r--   0        0        0     4158 1970-01-01 00:00:00.000000 kodexa-6.2.25211422458/PKG-INFO
```

### Comparing `kodexa-6.2.25210074074/LICENSE` & `kodexa-6.2.25211422458/LICENSE`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/README.md` & `kodexa-6.2.25211422458/README.md`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/__init__.py` & `kodexa-6.2.25211422458/kodexa/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/assistant/assistant.py` & `kodexa-6.2.25211422458/kodexa/assistant/assistant.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/connectors/connectors.py` & `kodexa-6.2.25211422458/kodexa/connectors/connectors.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/model/__init__.py` & `kodexa-6.2.25211422458/kodexa/model/__init__.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/model/base.py` & `kodexa-6.2.25211422458/kodexa/model/base.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/model/model.py` & `kodexa-6.2.25211422458/kodexa/model/model.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/model/objects.py` & `kodexa-6.2.25211422458/kodexa/model/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -1710,30 +1710,26 @@
 
 
 class MessageFeedback(KodexaBaseModel):
     user_id: Optional[str] = Field(None, alias='userId')
     options: Optional[Dict[str, Any]] = None
 
 
-class MessageMetadata(KodexaBaseModel):
-    sender_id: Optional[str] = Field(None, alias='senderId')
-    sender_type: Optional[str] = Field(None, alias='senderType')
-
-
 class Message(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the message')
     uuid: Optional[str] = None
     created_on: Optional[datetime] = Field(None, alias='createdOn')
     updated_on: Optional[datetime] = Field(None, alias='updatedOn')
     channel: Optional[Channel] = None
     message_blocks: Optional[MessageBlock] = Field(None, alias='messageBlock')
     message_type: Optional[str] = Field(None, alias='messageType')
     content: Optional[str] = None
     message_feedback: Optional[MessageFeedback] = Field(None, alias='messageFeedback')
-    message_metadata: Optional[MessageMetadata] = Field(None, alias='messageMetadata')
+    assistant: Optional[Assistant] = None
+    user: Optional[User] = None
 
 
 class DataAttribute(KodexaBaseModel):
     id: Optional[str] = Field(None, description='The ID of the object')
     uuid: Optional[str] = None
     created_on: Optional[datetime] = Field(None, alias='createdOn')
     updated_on: Optional[datetime] = Field(None, alias='updatedOn')
```

### Comparing `kodexa-6.2.25210074074/kodexa/model/persistence.py` & `kodexa-6.2.25211422458/kodexa/model/persistence.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/pipeline/pipeline.py` & `kodexa-6.2.25211422458/kodexa/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/platform/client.py` & `kodexa-6.2.25211422458/kodexa/platform/client.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/platform/kodexa.py` & `kodexa-6.2.25211422458/kodexa/platform/kodexa.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/selectors/ast.py` & `kodexa-6.2.25211422458/kodexa/selectors/ast.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/selectors/core.py` & `kodexa-6.2.25211422458/kodexa/selectors/core.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/selectors/lexrules.py` & `kodexa-6.2.25211422458/kodexa/selectors/lexrules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/selectors/lextab.py` & `kodexa-6.2.25211422458/kodexa/selectors/lextab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/selectors/parserules.py` & `kodexa-6.2.25211422458/kodexa/selectors/parserules.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/selectors/parsetab.py` & `kodexa-6.2.25211422458/kodexa/selectors/parsetab.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/spatial/azure_models.py` & `kodexa-6.2.25211422458/kodexa/spatial/azure_models.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/spatial/bbox_common.py` & `kodexa-6.2.25211422458/kodexa/spatial/bbox_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/spatial/table_form_common.py` & `kodexa-6.2.25211422458/kodexa/spatial/table_form_common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/steps/common.py` & `kodexa-6.2.25211422458/kodexa/steps/common.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/testing/test_components.py` & `kodexa-6.2.25211422458/kodexa/testing/test_components.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/kodexa/testing/test_utils.py` & `kodexa-6.2.25211422458/kodexa/testing/test_utils.py`

 * *Files identical despite different names*

### Comparing `kodexa-6.2.25210074074/pyproject.toml` & `kodexa-6.2.25211422458/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kodexa"
-version = "6.2.25210074074"
+version = "6.2.25211422458"
 description = "Python SDK for the Kodexa Platform"
 authors = ["Austin Redenbaugh <austin@kodexa.com>", "Philip Dodds <philip@kodexa.com>", "Romar Cablao <rcablao@kodexa.com>", "Amadea Paula Dodds <amadeapaula@kodexa.com>"]
 readme = "README.md"
 
 packages = [
     { include = "kodexa" }
 ]
```

### Comparing `kodexa-6.2.25210074074/setup.py` & `kodexa-6.2.25211422458/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
  'pyyaml>=6.0,<7.0',
  'requests>=2.28.1,<3.0.0',
  'simpleeval==0.9.12',
  'urllib3>=1.26.14,<2.0.0']
 
 setup_kwargs = {
     'name': 'kodexa',
-    'version': '6.2.25210074074',
+    'version': '6.2.25211422458',
     'description': 'Python SDK for the Kodexa Platform',
     'long_description': '# Kodexa\n\n[![Build and Package with Poetry](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml/badge.svg?branch=main)](https://github.com/kodexa-ai/kodexa/actions/workflows/main.yml)\n\n![img.png](https://docs.kodexa.com/img.png)\n\nKodexa is a platform for building intelligent document processing pipelines. It is a set of tools and services that\nallow you to build a pipeline that can take a document, extract the content, and then process it to extract the\ninformation you need.\n\nIt is built on a set of core principles:\n\n* **Document Centric** - Kodexa is built around the idea of a document. A document is a collection of content\n  nodes that are connected together. This is a powerful model that allows you to build pipelines that can\n  extract content from a wide range of sources.\n\n* **Pipeline Oriented** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that\n  can be executed on a document. This allows you to build a pipeline that can extract content from a wide range\n  of sources.\n\n* **Extensible** - Kodexa is built around the idea of a pipeline. A pipeline is a series of steps that can be executed\n  on a document. This allows you to build a pipeline that can extract content from a wide range of sources.\n\n* **Label Driven** - Kodexa focuses on the idea of labels. Labels are a way to identify content within a document\n  and then use that content to drive the processing of the document.\n\n# Python SDK\n\nThis repository contains the Python SDK for Kodexa. The SDK is the primary way to interact with Kodexa. It allows you to\ndefine actions, models, and pipelines that can be executed on Kodexa. It also includes a complete SDK client for\nworking with a Kodexa platform instance.\n\n## Documentation & Examples\n\nDocumentation is available at the [Kodexa Documentation Portal](https://docs.kodexa.com)\n\n## Current Development\n\n[//]: # (Replace it with the diagrams and descriptions for build releases)\n**BUILD VERSION FLOW**\n![build-version-flow.png](docs%2Fbuild-version-flow.png)\nBuild version will differ based on the branches that are published to pypi.\n\n**GITHUB PROCESS**\n![github-process.png](docs%2Fgithub-process.png)\nChanges that contain bugs, features, and fixes should first be pushed to the test branch. \nOnce these changes are thoroughly tested, they can be submitted as a pull request to the main branch. The pull request should be reviewed and approved by an appropriate person before the changes can be merged.\n\n## Set-up\n\nWe use poetry to manage our dependencies, so you can install them with:\n\n    poetry install\n\nYou can then run the tests with:\n\n    poetry run pytest\n\n# Contributing\n\nWe welcome contributions to the Kodexa platform. Please see our [contributing guide](CONTRIBUTING.md) for more details.\n\n# License\n\nApache 2.0\n\n',
     'author': 'Austin Redenbaugh',
     'author_email': 'austin@kodexa.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `kodexa-6.2.25210074074/PKG-INFO` & `kodexa-6.2.25211422458/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kodexa
-Version: 6.2.25210074074
+Version: 6.2.25211422458
 Summary: Python SDK for the Kodexa Platform
 Author: Austin Redenbaugh
 Author-email: austin@kodexa.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

