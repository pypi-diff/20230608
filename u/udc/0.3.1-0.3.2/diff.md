# Comparing `tmp/udc-0.3.1.tar.gz` & `tmp/udc-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udc-0.3.1.tar", max compression
+gzip compressed data, was "udc-0.3.2.tar", max compression
```

## Comparing `udc-0.3.1.tar` & `udc-0.3.2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.3.1/LICENSE
--rw-r--r--   0        0        0     2767 2023-06-01 22:23:26.719321 udc-0.3.1/README.md
--rw-r--r--   0        0        0      858 2023-06-01 22:23:26.722167 udc-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      232 2023-06-01 02:59:07.594491 udc-0.3.1/udc/__init__.py
--rw-r--r--   0        0        0     1130 2023-06-01 02:59:07.595367 udc-0.3.1/udc/benchling/__init__.py
--rw-r--r--   0        0        0     3211 2023-06-01 22:23:26.724318 udc-0.3.1/udc/benchling/entry.py
--rw-r--r--   0        0        0      693 2023-06-01 02:59:07.596749 udc-0.3.1/udc/benchling/resource.py
--rw-r--r--   0        0        0     2944 2023-06-01 22:23:26.724733 udc-0.3.1/udc/benchling/root.py
--rw-r--r--   0        0        0      357 2023-05-31 06:12:37.912100 udc-0.3.1/udc/benchling/schema.py
--rw-r--r--   0        0        0      353 2023-05-31 06:12:37.911714 udc-0.3.1/udc/benchling/sequence.py
--rw-r--r--   0        0        0      334 2023-06-01 02:59:07.598493 udc-0.3.1/udc/main.py
--rw-r--r--   0        0        0        0 2023-06-01 22:23:26.724816 udc-0.3.1/udc/py.typed
--rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.3.1/udc/quilt/__init__.py
--rw-r--r--   0        0        0      275 2023-05-31 00:13:14.714433 udc-0.3.1/udc/quilt/resource.py
--rw-r--r--   0        0        0      558 2023-06-01 22:23:26.726307 udc-0.3.1/udc/types.py
--rw-r--r--   0        0        0      276 2023-06-01 02:59:07.599906 udc-0.3.1/udc/wrapper.py
--rw-r--r--   0        0        0     3509 1970-01-01 00:00:00.000000 udc-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-12 01:09:39.984612 udc-0.3.2/LICENSE
+-rw-r--r--   0        0        0     3545 2023-06-08 06:45:46.220482 udc-0.3.2/README.md
+-rw-r--r--   0        0        0      933 2023-06-08 06:45:46.224741 udc-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0      505 2023-06-08 06:45:46.228244 udc-0.3.2/udc/__init__.py
+-rw-r--r--   0        0        0     1152 2023-06-08 06:45:46.228630 udc-0.3.2/udc/benchling/__init__.py
+-rw-r--r--   0        0        0     3211 2023-06-01 22:23:26.724318 udc-0.3.2/udc/benchling/entry.py
+-rw-r--r--   0        0        0      855 2023-06-08 06:45:46.228957 udc-0.3.2/udc/benchling/resource.py
+-rw-r--r--   0        0        0     2944 2023-06-01 22:23:26.724733 udc-0.3.2/udc/benchling/root.py
+-rw-r--r--   0        0        0      357 2023-05-31 06:12:37.912100 udc-0.3.2/udc/benchling/schema.py
+-rw-r--r--   0        0        0      353 2023-05-31 06:12:37.911714 udc-0.3.2/udc/benchling/sequence.py
+-rw-r--r--   0        0        0     2727 2023-06-08 06:45:46.229812 udc-0.3.2/udc/cli.yaml
+-rw-r--r--   0        0        0      437 2023-06-08 06:45:46.230516 udc-0.3.2/udc/main.py
+-rw-r--r--   0        0        0        0 2023-06-01 22:23:26.724816 udc-0.3.2/udc/py.typed
+-rw-r--r--   0        0        0       49 2023-05-25 04:58:47.606168 udc-0.3.2/udc/quilt/__init__.py
+-rw-r--r--   0        0        0      125 2023-06-08 06:45:46.231201 udc-0.3.2/udc/quilt/resource.py
+-rw-r--r--   0        0        0      753 2023-06-08 06:45:46.231596 udc-0.3.2/udc/types.py
+-rw-r--r--   0        0        0      292 2023-06-08 06:45:46.232583 udc-0.3.2/udc/wrapper.py
+-rw-r--r--   0        0        0     4280 1970-01-01 00:00:00.000000 udc-0.3.2/PKG-INFO
```

### Comparing `udc-0.3.1/LICENSE` & `udc-0.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `udc-0.3.1/README.md` & `udc-0.3.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,19 @@
 For example:
 
 - `udc list "quilt+s3://quilt-example#package=examples/wellplates"`
 - `udc patch "benchling+https://dtt.benchling.com?name=Update#type=Entry&id=etr_123"`
 
 ## Installation
 
+NOTE: UDC requires Python 3.10 or higher.
+You can check your version with `python3 --version`.
+If you have an older version, you will need to update your environment to a
+[newer version of Python](https://www.pythoncentral.io/how-to-update-python/).
+
 ### Production Package
 
 From PyPi:
 
 <!--pytest.mark.skip-->
 ```bash
 python3 -m pip install udc # OR
@@ -28,15 +33,15 @@
 which udc
 ```
 
 ## Development Branch
 
 <!--pytest.mark.skip-->
 ```bash
-python3 -m pip install https://github.com/data-yaml/udc@main
+python3 -m pip install git+https://github.com/data-yaml/udc.git@main
 ```
 
 ## Cloned
 
 When cloned from [GitHub](https://github.com/data-yaml/udc):
 
 ```bash
@@ -94,14 +99,40 @@
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
 "quilt+s3://quilt-example#package=akarve/amazon-reviews:latest"
 ```
 
+### Get a package into a specific directory
+
+You can also use `put` (replace) and `patch` (merge) if you have write access.
+
+```bash
+udc get "quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2" --dir /tmp/wellplates
+```
+
+Checking the download directory:
+
+```bash
+ls /tmp/wellplates
+```
+
+Should reveal the following output:
+<!--pytest-codeblocks:expected-output-->
+```bash
+README.md
+autoplate_H1N1.csv
+data_products.ipynb
+neutralisation-altair.json
+neutralisation.json
+quilt_summarize.json
+render.html
+```
+
 ## Development
 
 ### Testing
 
 <!--pytest.mark.skip-->
 ```bash
 make test
```

### Comparing `udc-0.3.1/pyproject.toml` & `udc-0.3.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,37 @@
 [tool.poetry]
 name = "udc"
-version = "0.3.1"
+version = "0.3.2"
 description = "The Universal Data Client command-line tool"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
 trio = "^0.22.0"
 asyncclick = "^8.1.3.4"
 quilt3 = "^5.3.1"
 urllib3 = "<2"
 typing-extensions = "^4.5.0"
-quiltplus = ">=0.9.0"
-# quiltplus = {git = "https://github.com/quiltdata/quiltplus.git", rev = "42-resourceattrs-to-align-with-udc"}
+quiltplus = ">=0.9.3"
+# quiltplus = {git = "https://github.com/quiltdata/quiltplus.git", rev = "main"}
 benchling-sdk = "^1.6.1"
-un-yaml = "^0.1.2"
+un-yaml = ">=0.3.1"
+# un-yaml = {git = "https://github.com/data-yaml/un-yaml.git", rev = "main"}
 
 [tool.poetry.group.dev.dependencies]
 pytest-coverage = "^0.0"
 pytest-watcher = "^0.2.6"
 pytest-asyncio = "^0.21.0"
 pytest-trio = "^0.8.0"
 pytest-codeblocks = "^0.16.1"
 ipykernel = "^6.23.1"
 mypy = "^1.3.0"
+types-tzlocal = "^5.0.1.0"
 
 [tool.poetry.scripts]
 udc = "udc.main:main"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `udc-0.3.1/udc/benchling/__init__.py` & `udc-0.3.2/udc/benchling/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from .entry import BenchlingEntry, BenchlingEntryList  # NOQA F401
-from .resource import RESOURCE_MAP, BenchlingResource  # NOQA F401
+from .resource import RESOURCE_MAP, BenchlingResource, BenchlingResourceURI  # NOQA F401
 from .root import BenchlingById, BenchlingRoot  # NOQA F401
 from .schema import BenchlingSchema, BenchlingSchemaList  # NOQA F401
 from .sequence import BenchlingSequence, BenchlingSequenceList  # NOQA F401
 
 RESOURCES = [
     "aa_sequences",
     "api",
```

### Comparing `udc-0.3.1/udc/benchling/entry.py` & `udc-0.3.2/udc/benchling/entry.py`

 * *Files identical despite different names*

### Comparing `udc-0.3.1/udc/benchling/resource.py` & `udc-0.3.2/udc/benchling/resource.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,25 @@
 from .entry import BenchlingEntry, BenchlingEntryList
 from .root import BenchlingRoot
 from .schema import BenchlingSchema, BenchlingSchemaList
 from .sequence import BenchlingSequence, BenchlingSequenceList
+from un_yaml import UnUri
 
 RESOURCE_MAP = {
     "entries": [BenchlingEntryList, BenchlingEntry],
     "dna_sequences": [BenchlingSequenceList, BenchlingSequence],
     "schemas": [BenchlingSchemaList, BenchlingSchema],
 }
 
 
-def BenchlingResource(attrs: dict):
+def BenchlingResource(attrs: dict) -> BenchlingRoot:
     root = BenchlingRoot(attrs)
     type = root.type
     klasses = RESOURCE_MAP.get(type)
     if not klasses:
         raise ValueError(f"Unknown resource type[{type}]: {attrs}")
     klass = klasses[0] if not root.id else klasses[1]
     return klass(attrs)
+
+def BenchlingResourceURI(uri: str) -> BenchlingRoot:
+    attrs = UnUri(uri).attrs
+    return BenchlingResource(attrs)
```

### Comparing `udc-0.3.1/udc/benchling/root.py` & `udc-0.3.2/udc/benchling/root.py`

 * *Files identical despite different names*

### Comparing `udc-0.3.1/udc/types.py` & `udc-0.3.2/udc/types.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,11 +14,17 @@
 class Getable(Protocol):
     async def get(self, argv: dict = {}) -> ResultList:
         """Get contents of URI into path"""
         return []
 
 
 @runtime_checkable
+class Patchable(Protocol):
+    async def patch(self, argv: dict = {}) -> ResultList:
+        """Patch (merge/update) contents of path into URI."""
+        return []
+
+@runtime_checkable
 class Putable(Protocol):
     async def put(self, argv: dict = {}) -> ResultList:
-        """Put contents of path into URI."""
+        """Put (replace) contents of path into URI."""
         return []
```

### Comparing `udc-0.3.1/PKG-INFO` & `udc-0.3.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: udc
-Version: 0.3.1
+Version: 0.3.2
 Summary: The Universal Data Client command-line tool
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: anyio (>=3.7.0,<4.0.0)
 Requires-Dist: asyncclick (>=8.1.3.4,<9.0.0.0)
 Requires-Dist: benchling-sdk (>=1.6.1,<2.0.0)
 Requires-Dist: quilt3 (>=5.3.1,<6.0.0)
-Requires-Dist: quiltplus (>=0.9.0)
+Requires-Dist: quiltplus (>=0.9.3)
 Requires-Dist: trio (>=0.22.0,<0.23.0)
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
-Requires-Dist: un-yaml (>=0.1.2,<0.2.0)
+Requires-Dist: un-yaml (>=0.3.1)
 Requires-Dist: urllib3 (<2)
 Description-Content-Type: text/markdown
 
 # UDC
 
 ## The Universal Data Client
 
@@ -34,14 +34,19 @@
 For example:
 
 - `udc list "quilt+s3://quilt-example#package=examples/wellplates"`
 - `udc patch "benchling+https://dtt.benchling.com?name=Update#type=Entry&id=etr_123"`
 
 ## Installation
 
+NOTE: UDC requires Python 3.10 or higher.
+You can check your version with `python3 --version`.
+If you have an older version, you will need to update your environment to a
+[newer version of Python](https://www.pythoncentral.io/how-to-update-python/).
+
 ### Production Package
 
 From PyPi:
 
 <!--pytest.mark.skip-->
 ```bash
 python3 -m pip install udc # OR
@@ -49,15 +54,15 @@
 which udc
 ```
 
 ## Development Branch
 
 <!--pytest.mark.skip-->
 ```bash
-python3 -m pip install https://github.com/data-yaml/udc@main
+python3 -m pip install git+https://github.com/data-yaml/udc.git@main
 ```
 
 ## Cloned
 
 When cloned from [GitHub](https://github.com/data-yaml/udc):
 
 ```bash
@@ -115,14 +120,40 @@
 
 e.g.,
 <!--pytest-codeblocks:expected-output-->
 ```bash
 "quilt+s3://quilt-example#package=akarve/amazon-reviews:latest"
 ```
 
+### Get a package into a specific directory
+
+You can also use `put` (replace) and `patch` (merge) if you have write access.
+
+```bash
+udc get "quilt+s3://quilt-example#package=examples/wellplates@6782cf98a2" --dir /tmp/wellplates
+```
+
+Checking the download directory:
+
+```bash
+ls /tmp/wellplates
+```
+
+Should reveal the following output:
+<!--pytest-codeblocks:expected-output-->
+```bash
+README.md
+autoplate_H1N1.csv
+data_products.ipynb
+neutralisation-altair.json
+neutralisation.json
+quilt_summarize.json
+render.html
+```
+
 ## Development
 
 ### Testing
 
 <!--pytest.mark.skip-->
 ```bash
 make test
```

