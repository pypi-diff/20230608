# Comparing `tmp/cerebrium-1.0.4.tar.gz` & `tmp/cerebrium-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cerebrium-1.0.4.tar", max compression
+gzip compressed data, was "cerebrium-1.0.5.tar", max compression
```

## Comparing `cerebrium-1.0.4.tar` & `cerebrium-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    34594 2023-06-06 20:40:18.417607 cerebrium-1.0.4/LICENSE
--rw-r--r--   0        0        0     3193 2023-06-06 20:40:18.417607 cerebrium-1.0.4/README.md
--rw-r--r--   0        0        0      285 2023-06-06 20:44:06.291376 cerebrium-1.0.4/cerebrium/__init__.py
--rwxr-xr-x   0        0        0     8478 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/cli.py
--rw-r--r--   0        0        0    31396 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/conduit.py
--rw-r--r--   0        0        0     4483 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/core.py
--rw-r--r--   0        0        0     2520 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/errors.py
--rw-r--r--   0        0        0    11229 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/flow.py
--rw-r--r--   0        0        0     2807 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/logging/arize.py
--rw-r--r--   0        0        0      705 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/logging/base.py
--rw-r--r--   0        0        0     3855 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/logging/censius.py
--rw-r--r--   0        0        0      911 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/base.py
--rw-r--r--   0        0        0      446 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/hf_pipeline.py
--rw-r--r--   0        0        0      418 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/onnx.py
--rw-r--r--   0        0        0     1116 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/sklearn.py
--rw-r--r--   0        0        0      244 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/spacy.py
--rw-r--r--   0        0        0      342 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/models/torch.py
--rw-r--r--   0        0        0     7124 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/requests.py
--rw-r--r--   0        0        0      465 2023-06-06 20:40:18.417607 cerebrium-1.0.4/cerebrium/utils.py
--rw-r--r--   0        0        0     2340 2023-06-06 20:44:06.287376 cerebrium-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0    34594 2023-06-08 12:44:17.440744 cerebrium-1.0.5/LICENSE
+-rw-r--r--   0        0        0     3193 2023-06-08 12:44:17.440744 cerebrium-1.0.5/README.md
+-rw-r--r--   0        0        0      285 2023-06-08 12:49:17.438397 cerebrium-1.0.5/cerebrium/__init__.py
+-rwxr-xr-x   0        0        0     8478 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/cli.py
+-rw-r--r--   0        0        0    31396 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/conduit.py
+-rw-r--r--   0        0        0     4483 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/core.py
+-rw-r--r--   0        0        0     2520 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/errors.py
+-rw-r--r--   0        0        0    11229 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/flow.py
+-rw-r--r--   0        0        0     2807 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/logging/arize.py
+-rw-r--r--   0        0        0      705 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/logging/base.py
+-rw-r--r--   0        0        0     3855 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/logging/censius.py
+-rw-r--r--   0        0        0      911 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/models/base.py
+-rw-r--r--   0        0        0      446 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/models/hf_pipeline.py
+-rw-r--r--   0        0        0      418 2023-06-08 12:44:17.440744 cerebrium-1.0.5/cerebrium/models/onnx.py
+-rw-r--r--   0        0        0     1116 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/models/sklearn.py
+-rw-r--r--   0        0        0      244 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/models/spacy.py
+-rw-r--r--   0        0        0      342 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/models/torch.py
+-rw-r--r--   0        0        0     7124 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/requests.py
+-rw-r--r--   0        0        0      465 2023-06-08 12:44:17.444744 cerebrium-1.0.5/cerebrium/utils.py
+-rw-r--r--   0        0        0     2340 2023-06-08 12:49:17.434397 cerebrium-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     5282 1970-01-01 00:00:00.000000 cerebrium-1.0.5/PKG-INFO
```

### Comparing `cerebrium-1.0.4/LICENSE` & `cerebrium-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/README.md` & `cerebrium-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/cli.py` & `cerebrium-1.0.5/cerebrium/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 @app.command()
 def deploy(
     name: str = typer.Argument(..., help="Name of the builder deployment."),
     api_key: str = typer.Argument(
         ..., envvar="CEREBRIUM_API_KEY", help="Private API key for the user."
     ),
     hardware: str = typer.Option(
-        "cpu",
+        "GPU",
         help="Hardware to use for the builder deployment. Can be one of 'CPU', 'GPU' or 'A10'.",
     ),
     init_debug: bool = typer.Option(
         False,
         help="Stops the container after initialization.",
     ),
     pre_init_debug: bool = typer.Option(
```

### Comparing `cerebrium-1.0.4/cerebrium/conduit.py` & `cerebrium-1.0.5/cerebrium/conduit.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/core.py` & `cerebrium-1.0.5/cerebrium/core.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/errors.py` & `cerebrium-1.0.5/cerebrium/errors.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/flow.py` & `cerebrium-1.0.5/cerebrium/flow.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/logging/arize.py` & `cerebrium-1.0.5/cerebrium/logging/arize.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/logging/base.py` & `cerebrium-1.0.5/cerebrium/logging/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/logging/censius.py` & `cerebrium-1.0.5/cerebrium/logging/censius.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/models/base.py` & `cerebrium-1.0.5/cerebrium/models/base.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/models/sklearn.py` & `cerebrium-1.0.5/cerebrium/models/sklearn.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/cerebrium/requests.py` & `cerebrium-1.0.5/cerebrium/requests.py`

 * *Files identical despite different names*

### Comparing `cerebrium-1.0.4/pyproject.toml` & `cerebrium-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cerebrium"
-version = "1.0.4"
+version = "1.0.5"
 description = ""
 authors = ["Elijah Roussos <elijah@cerebrium.ai>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 exclude = ["tests/*", "dist/*", "worker/*", "builder/*", "prebuilt/*", "common/*", "examples/*"]
 
 [tool.poetry.urls]
```

### Comparing `cerebrium-1.0.4/PKG-INFO` & `cerebrium-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cerebrium
-Version: 1.0.4
+Version: 1.0.5
 Summary: 
 License: AGPL-3.0-only
 Author: Elijah Roussos
 Author-email: elijah@cerebrium.ai
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
```

