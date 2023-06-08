# Comparing `tmp/reliably-cli-0.5.9.tar.gz` & `tmp/reliably_cli-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reliably-cli-0.5.9.tar", last modified: Thu Mar 16 15:51:23 2023, max compression
+gzip compressed data, was "reliably_cli-0.6.0.tar", last modified: Thu Jun  8 08:54:42 2023, max compression
```

## Comparing `reliably-cli-0.5.9.tar` & `reliably_cli-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2023-03-16 15:50:55.186972 reliably-cli-0.5.9/LICENSE
--rw-r--r--   0        0        0     1472 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/README.md
--rw-r--r--   0        0        0     2404 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/pyproject.toml
--rw-r--r--   0        0        0      114 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/__init__.py
--rw-r--r--   0        0        0      881 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/__main__.py
--rw-r--r--   0        0        0      166 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/__version__.py
--rw-r--r--   0        0        0     1221 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/agent/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/agent/cli.py
--rw-r--r--   0        0        0     2770 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/agent/plan/__init__.py
--rw-r--r--   0        0        0     1352 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/agent/plan/providers/__init__.py
--rw-r--r--   0        0        0     3493 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/agent/plan/providers/github.py
--rw-r--r--   0        0        0     1215 2023-03-16 15:50:55.190972 reliably-cli-0.5.9/reliably_cli/client.py
--rw-r--r--   0        0        0     1087 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/config/__init__.py
--rw-r--r--   0        0        0     3552 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/config/cli.py
--rw-r--r--   0        0        0     2403 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/config/types.py
--rw-r--r--   0        0        0      546 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/format.py
--rw-r--r--   0        0        0      126 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/log.py
--rw-r--r--   0        0        0        0 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/services/__init__.py
--rw-r--r--   0        0        0      211 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/services/cli.py
--rw-r--r--   0        0        0     2388 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/services/org.py
--rw-r--r--   0        0        0     5851 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/services/plan.py
--rw-r--r--   0        0        0     1777 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/reliably_cli/types.py
--rw-r--r--   0        0        0      662 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/tests/conftest.py
--rw-r--r--   0        0        0      581 2023-03-16 15:50:55.194972 reliably-cli-0.5.9/tests/test_cli.py
--rw-r--r--   0        0        0     1751 1970-01-01 00:00:00.000000 reliably-cli-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-08 08:54:24.435650 reliably_cli-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1467 2023-06-08 08:54:24.435650 reliably_cli-0.6.0/README.md
+-rw-r--r--   0        0        0     3015 2023-06-08 08:54:42.675957 reliably_cli-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      114 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/__init__.py
+-rw-r--r--   0        0        0      881 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/__main__.py
+-rw-r--r--   0        0        0      166 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/__version__.py
+-rw-r--r--   0        0        0     1221 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/agent/__init__.py
+-rw-r--r--   0        0        0     1545 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/agent/cli.py
+-rw-r--r--   0        0        0     2770 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/agent/plan/__init__.py
+-rw-r--r--   0        0        0     1352 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/agent/plan/providers/__init__.py
+-rw-r--r--   0        0        0     3493 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/agent/plan/providers/github.py
+-rw-r--r--   0        0        0     1215 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/client.py
+-rw-r--r--   0        0        0     1087 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/config/__init__.py
+-rw-r--r--   0        0        0     3552 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/config/cli.py
+-rw-r--r--   0        0        0     2403 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/config/types.py
+-rw-r--r--   0        0        0      566 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/format.py
+-rw-r--r--   0        0        0      126 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/log.py
+-rw-r--r--   0        0        0        0 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/services/__init__.py
+-rw-r--r--   0        0        0      211 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/services/cli.py
+-rw-r--r--   0        0        0     2388 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/services/org.py
+-rw-r--r--   0        0        0    10148 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/services/plan.py
+-rw-r--r--   0        0        0     2068 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/reliably_cli/types.py
+-rw-r--r--   0        0        0      662 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      581 2023-06-08 08:54:24.439650 reliably_cli-0.6.0/tests/test_cli.py
+-rw-r--r--   0        0        0     3562 1970-01-01 00:00:00.000000 reliably_cli-0.6.0/PKG-INFO
```

### Comparing `reliably-cli-0.5.9/LICENSE` & `reliably_cli-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/README.md` & `reliably_cli-0.6.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 
 <h4 align="center">Reliably CLI | Optimise your operations</h4>
 
 <p align="center">
    <a href="https://github.com/reliablyhq/cli/releases">
    <img alt="Release" src="https://img.shields.io/pypi/v/reliably-cli.svg">
    <a href="https://pypi.org/project/reliably-cli/">
-   <img alt="Supported Python" src="https://img.shields.io/pypi/pyversions/chaostoolkit-reliably.svg">
+   <img alt="Supported Python" src="https://img.shields.io/pypi/pyversions/reliably-cli.svg">
    <a href="https://goreportcard.com/report/github.com/reliablyhq/cli">
    <a href="#">
    <img alt="Build" src="https://github.com/reliablyhq/cli/actions/workflows/cli-check.yaml/badge.svg">
    <a href="https://github.com/reliablyhq/cli/issues">
    <img alt="GitHub issues" src="https://img.shields.io/github/issues/reliablyhq/cli?style=flat-square&logo=github&logoColor=white">
    <a href="https://github.com/reliablyhq/cli/blob/master/LICENSE.md">
    <img alt="License" src="https://img.shields.io/github/license/reliablyhq/cli">
 </p>
 
 <p align="center">
   <a href="#installation">Installation</a> •
-  <a href="https://reliably.com/docs/">Documentation</a> •
+  <a href="https://reliably.com/docs/cli/">Documentation</a> •
   <a href="https://github.com/reliablyhq/cli/blob/main/CHANGELOG.md">Changes</a>
 </p>
 
 ---
 
 The Reliably CLI is your interface to the Reliably services.
```

### Comparing `reliably-cli-0.5.9/pyproject.toml` & `reliably_cli-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -3,32 +3,49 @@
 description = "Reliably CLI"
 dynamic = []
 authors = [
     { name = "Sylvain Hellegouarch", email = "sylvain@reliably.com" },
 ]
 requires-python = ">=3.10"
 readme = "README.md"
+classifiers = [
+    "License :: OSI Approved :: Apache Software License",
+    "Development Status :: 4 - Beta",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: System :: Monitoring",
+    "Topic :: Utilities",
+]
 dependencies = [
     "httpx[http2]>=0.23.0",
     "pydantic[dotenv]>=1.10.2",
     "typer>=0.6.1",
     "anyio[trio]>=3.6.2",
     "tomli>=1.1.0; python_version < \"3.11\"",
     "ruamel.yaml>=0.17.21",
     "rich>=13.3.1",
     "chaostoolkit-addons>=0.4.0",
     "chaostoolkit>=1.15.0",
     "chaostoolkit-lib>=1.33.1",
     "chaostoolkit-reliably>=0.22.0",
+    "orjson>=3.8.10",
 ]
-version = "0.5.9"
+version = "0.6.0"
 
 [project.license]
 text = "Apache-2.0"
 
+[project.urls]
+Homepage = "https://reliably.com/"
+Repository = "https://github.com/reliablyhq/cli"
+Documentation = "https://reliably.com/docs/cli/"
+Changelog = "https://github.com/reliablyhq/cli/blob/main/CHANGELOG.md"
+
 [project.scripts]
 reliably = "reliably_cli.__main__:cli"
 
 [project.optional-dependencies]
 bin-builder = [
     "pyoxidizer>=0.22.0",
 ]
@@ -38,21 +55,22 @@
     "chaostoolkit-google-cloud-platform>=0.8.2",
     "chaostoolkit-prometheus>=0.5.0",
     "chaostoolkit-opentracing>=0.9.1",
     "chaostoolkit-dynatrace>=0.2.0",
     "chaostoolkit-grafana>=0.2.0",
     "chaostoolkit-slack>=0.5.7",
     "chaostoolkit-datadog>=0.1.1",
+    "jsonpath2>=0.4.5",
 ]
 
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
 
 [tool.ruff]
 line-length = 80
 
 [tool.black]
 color = true
 line-length = 80
```

### Comparing `reliably-cli-0.5.9/reliably_cli/__main__.py` & `reliably_cli-0.6.0/reliably_cli/__main__.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/agent/__init__.py` & `reliably_cli-0.6.0/reliably_cli/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/agent/cli.py` & `reliably_cli-0.6.0/reliably_cli/agent/cli.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/agent/plan/__init__.py` & `reliably_cli-0.6.0/reliably_cli/agent/plan/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/agent/plan/providers/__init__.py` & `reliably_cli-0.6.0/reliably_cli/agent/plan/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/agent/plan/providers/github.py` & `reliably_cli-0.6.0/reliably_cli/agent/plan/providers/github.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/client.py` & `reliably_cli-0.6.0/reliably_cli/client.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/config/__init__.py` & `reliably_cli-0.6.0/reliably_cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/config/cli.py` & `reliably_cli-0.6.0/reliably_cli/config/cli.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/config/types.py` & `reliably_cli-0.6.0/reliably_cli/config/types.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/format.py` & `reliably_cli-0.6.0/reliably_cli/format.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
-import json
 
+import orjson
 from ruamel.yaml import YAML
 
 from .types import BaseSchema, FormatOption
 
 __all__ = ["format_as"]
 
 
@@ -14,11 +14,11 @@
     match fmt.value:
         case "json":
             return entity.json(indent=2)
         case "yaml":
             with io.StringIO() as s:
                 yaml = YAML()
                 yaml.default_flow_style = False
-                yaml.dump(json.loads(entity.json()), s)
+                yaml.dump(orjson.loads(entity.json().encode("utf-8")), s)
                 return s.getvalue()
 
     return None
```

### Comparing `reliably-cli-0.5.9/reliably_cli/services/org.py` & `reliably_cli-0.6.0/reliably_cli/services/org.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/reliably_cli/types.py` & `reliably_cli-0.6.0/reliably_cli/types.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,34 @@
-import json
 from datetime import datetime
 from enum import Enum
 from typing import Any, Dict, List, Literal
 
+import orjson
 from pydantic import UUID4, BaseModel
 
 __all__ = ["Plan", "FormatOption", "Organization"]
 
 
+def _json_dumps(*args, **kwargs) -> str:  # type: ignore[no-untyped-def]
+    return orjson.dumps(*args, **kwargs).decode("utf-8")
+
+
+def _json_loads(obj: str, *args, **kwargs) -> Any:  # type: ignore[no-untyped-def]  # noqa
+    return orjson.loads(obj.encode("utf-8"), *args, **kwargs)
+
+
 class FormatOption(Enum):
     json = "json"
     yaml = "yaml"
 
 
 class BaseSchema(BaseModel):
     class Config:
-        json_loads = json.loads
-        json_dumps = json.dumps
+        json_loads = _json_loads
+        json_dumps = _json_dumps
 
 
 class PlanReliablyEnvironment(BaseSchema):
     provider: Literal["reliably_cloud"] = "reliably_cloud"
     id: UUID4
```

### Comparing `reliably-cli-0.5.9/tests/conftest.py` & `reliably_cli-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `reliably-cli-0.5.9/tests/test_cli.py` & `reliably_cli-0.6.0/tests/test_cli.py`

 * *Files identical despite different names*

