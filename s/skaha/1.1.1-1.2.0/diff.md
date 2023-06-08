# Comparing `tmp/skaha-1.1.1.tar.gz` & `tmp/skaha-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skaha-1.1.1.tar", max compression
+gzip compressed data, was "skaha-1.2.0.tar", max compression
```

## Comparing `skaha-1.1.1.tar` & `skaha-1.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1080 2023-02-01 20:24:58.782787 skaha-1.1.1/LICENSE
--rw-r--r--   0        0        0      710 2023-02-01 20:24:58.786787 skaha-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      657 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/__init__.py
--rw-r--r--   0        0        0     4008 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/client.py
--rw-r--r--   0        0        0     1264 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/context.py
--rw-r--r--   0        0        0      935 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/exceptions.py
--rw-r--r--   0        0        0     1531 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/images.py
--rw-r--r--   0        0        0     3537 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/models.py
--rw-r--r--   0        0        0    10076 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/session.py
--rw-r--r--   0        0        0      917 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/utils/convert.py
--rw-r--r--   0        0        0     1239 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/utils/logs.py
--rw-r--r--   0        0        0     1165 2023-02-01 20:24:58.786787 skaha-1.1.1/skaha/utils/threaded.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 skaha-1.1.1/setup.py
--rw-r--r--   0        0        0      816 1970-01-01 00:00:00.000000 skaha-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-06-08 00:04:18.065427 skaha-1.2.0/LICENSE
+-rw-r--r--   0        0        0      748 2023-06-08 00:04:18.077427 skaha-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0      657 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/__init__.py
+-rw-r--r--   0        0        0     4116 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/client.py
+-rw-r--r--   0        0        0     1284 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/context.py
+-rw-r--r--   0        0        0      935 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/exceptions.py
+-rw-r--r--   0        0        0     1606 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/images.py
+-rw-r--r--   0        0        0     3538 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/models.py
+-rw-r--r--   0        0        0      960 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/overview.py
+-rw-r--r--   0        0        0    10097 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/session.py
+-rw-r--r--   0        0        0      917 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/utils/convert.py
+-rw-r--r--   0        0        0     1239 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/utils/logs.py
+-rw-r--r--   0        0        0     1165 2023-06-08 00:04:18.077427 skaha-1.2.0/skaha/utils/threaded.py
+-rw-r--r--   0        0        0      859 1970-01-01 00:00:00.000000 skaha-1.2.0/PKG-INFO
```

### Comparing `skaha-1.1.1/LICENSE` & `skaha-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `skaha-1.1.1/pyproject.toml` & `skaha-1.2.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 [tool.poetry]
 name = "skaha"
-version = "1.1.1"
+version = "1.2.0"
 description = "Python Client for Skaha Container Platform in CANFAR"
 authors = ["Shiny Brar <charanjotbrar@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 vos = "^3"
 requests = "^2"
 pydantic = "^1"
 toml = "^0.10.2"
 mkdocs-material = {version = "*", optional = true}
 mkdocstrings-python = {version = "*", optional = true}
+defusedxml = "^0.7.1"
 
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "*"
 pre-commit = "*"
 pytest-cov = "*"
 
 [tool.poetry.extras]
 docs = ["mkdocs-material", "mkdocstrings-python"]
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^2.20.0"
+mypy = "^1.3.0"
 
 [build-system]
 requires = ["poetry-core>=1.2.2"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `skaha-1.1.1/skaha/__init__.py` & `skaha-1.2.0/skaha/__init__.py`

 * *Files identical despite different names*

### Comparing `skaha-1.1.1/skaha/client.py` & `skaha-1.2.0/skaha/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 
 
 class SkahaClient(BaseModel):
     """SkahaClient is the base class for all other API clients.
 
     Args:
         server (str): Server URL.
+        version (str): Skaha API version.
         certificate (str): Certificate file.
         timeout (int): Timeout for requests.
 
     Raises:
         InvalidServerURL: If the server URL is invalid.
         InvalidCertificateError: If the client is given an invalid certificate.
 
@@ -44,14 +45,15 @@
                 pass
 
     """
 
     server: AnyHttpUrl = Field(
         default="https://ws-uv.canfar.net/skaha", title="Server URL", type=AnyHttpUrl
     )
+    version: str = Field(default="v0", title="Skaha API Version")
     certificate: FilePath = Field(
         default="{HOME}/.ssl/cadcproxy.pem".format(HOME=environ["HOME"]),
         type=str,
         title="Certificate File",
     )
     timeout: int = Field(default=15, title="Timeout")
     session: Type[Session] = Field(default=Session())
```

### Comparing `skaha-1.1.1/skaha/context.py` & `skaha-1.2.0/skaha/context.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 class Context(SkahaClient):
     """Get available resources from the skaha server."""
 
     @root_validator
     def set_server(cls, values: Dict[str, Any]):
         """Sets the server path after validation."""
-        values["server"] = values["server"] + "/context"
+        values["server"] = f"{values['server']}/{values['version']}/context"
         return values
 
     def resources(self) -> Dict[str, Any]:
         """Get available resources from the skaha server.
 
         Returns:
             A dictionary of available resources.
```

### Comparing `skaha-1.1.1/skaha/exceptions.py` & `skaha-1.2.0/skaha/exceptions.py`

 * *Files identical despite different names*

### Comparing `skaha-1.1.1/skaha/images.py` & `skaha-1.2.0/skaha/images.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 class Images(SkahaClient):
     """Skaha Image Management."""
 
     @root_validator
     def set_server(cls, values: Dict[str, Any]):
         """Sets the server path after validation."""
+        values["server"] = f"{values['server']}/{values['version']}/image"
         values["server"] = values["server"] + "/image"
         return values
 
     def fetch(self, kind: Optional[str] = None) -> List[str]:
         """Get images from Skaha Server.
 
         Args:
```

### Comparing `skaha-1.1.1/skaha/models.py` & `skaha-1.2.0/skaha/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         ...,
         description="Container image to use for the session.",
         example="images.canfar.net/skaha/terminal:1.1.1",
     )
     cores: int = Field(1, description="Number of cores.", ge=1, le=256)
     ram: int = Field(4, description="Amount of RAM (GB).", ge=1, le=512)
     kind: str = Field(..., description="Type of skaha session.", example="headless")
-    gpu: Optional[int] = Field(None, description="Number of GPUs.", ge=1, le=28)
+    gpus: Optional[int] = Field(None, description="Number of GPUs.", ge=1, le=28)
     cmd: Optional[str] = Field(None, description="Command to run.", example="ls")
     args: Optional[str] = Field(
         None, description="Arguments to the command.", example="-la"
     )
     env: Dict[str, Any] = Field(
         ..., description="Environment variables.", example={"TEST": "test"}
     )
```

### Comparing `skaha-1.1.1/skaha/session.py` & `skaha-1.2.0/skaha/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 class Session(SkahaClient):
     """Skaha Session Client."""
 
     @root_validator
     def set_server(cls, values: Dict[str, Any]):
         """Sets the server path after validation."""
-        values["server"] = values["server"] + "/session"
+        values["server"] = f"{values['server']}/{values['version']}/session"
         log.debug(f'Server set to {values["server"]}')
         return values
 
     def fetch(
         self,
         kind: Optional[str] = None,
         status: Optional[str] = None,
@@ -210,15 +210,15 @@
         """
         specification: CreateSpec = CreateSpec(
             name=name,
             image=image,
             cores=cores,
             ram=ram,
             kind=kind,
-            gpu=gpu,
+            gpus=gpu,
             cmd=cmd,
             args=args,
             env=env,
             replicas=replicas,
         )
         data: Dict[str, Any] = specification.dict(exclude_none=True)
         log.info(f"Creating {replicas} session(s) with parameters:")
```

### Comparing `skaha-1.1.1/skaha/utils/convert.py` & `skaha-1.2.0/skaha/utils/convert.py`

 * *Files identical despite different names*

### Comparing `skaha-1.1.1/skaha/utils/logs.py` & `skaha-1.2.0/skaha/utils/logs.py`

 * *Files identical despite different names*

### Comparing `skaha-1.1.1/skaha/utils/threaded.py` & `skaha-1.2.0/skaha/utils/threaded.py`

 * *Files identical despite different names*

### Comparing `skaha-1.1.1/PKG-INFO` & `skaha-1.2.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: skaha
-Version: 1.1.1
+Version: 1.2.0
 Summary: Python Client for Skaha Container Platform in CANFAR
 License: MIT
 Author: Shiny Brar
 Author-email: charanjotbrar@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
+Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: mkdocs-material ; extra == "docs"
 Requires-Dist: mkdocstrings-python ; extra == "docs"
 Requires-Dist: pydantic (>=1,<2)
 Requires-Dist: requests (>=2,<3)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: vos (>=3,<4)
```

