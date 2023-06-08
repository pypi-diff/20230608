# Comparing `tmp/sekoia_automation_sdk-1.3.0.tar.gz` & `tmp/sekoia_automation_sdk-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sekoia_automation_sdk-1.3.0.tar", max compression
+gzip compressed data, was "sekoia_automation_sdk-1.3.1.tar", max compression
```

## Comparing `sekoia_automation_sdk-1.3.0.tar` & `sekoia_automation_sdk-1.3.1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
--rw-r--r--   0        0        0     1066 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/LICENSE
--rw-r--r--   0        0        0     8422 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/README.md
--rw-r--r--   0        0        0     2114 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/__init__.py
--rw-r--r--   0        0        0    11420 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/action.py
--rw-r--r--   0        0        0     4813 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/cli.py
--rw-r--r--   0        0        0      548 2023-06-06 13:11:35.445782 sekoia_automation_sdk-1.3.0/sekoia_automation/config.py
--rw-r--r--   0        0        0     6955 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/connector/__init__.py
--rw-r--r--   0        0        0     2313 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/connector/workers.py
--rw-r--r--   0        0        0      426 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/constants.py
--rw-r--r--   0        0        0      869 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/exceptions.py
--rw-r--r--   0        0        0      399 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/__init__.py
--rw-r--r--   0        0        0      383 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/base.py
--rw-r--r--   0        0        0     1185 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/prometheus.py
--rw-r--r--   0        0        0    15640 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/module.py
--rw-r--r--   0        0        0        0 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/__init__.py
--rw-r--r--   0        0        0     6605 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/generate.py
--rw-r--r--   0        0        0     2669 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/templates/module.md
--rw-r--r--   0        0        0     7581 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/files_generator.py
--rw-r--r--   0        0        0      144 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/cookiecutter.json
--rw-r--r--   0        0        0      301 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
--rw-r--r--   0        0        0      225 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
--rw-r--r--   0        0        0      417 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
--rw-r--r--   0        0        0      647 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
--rw-r--r--   0        0        0      358 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
--rw-r--r--   0        0        0      368 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
--rw-r--r--   0        0        0      140 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
--rw-r--r--   0        0        0    10011 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/openapi.py
--rwxr-xr-x   0        0        0    14039 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/sync_library.py
--rw-r--r--   0        0        0     6094 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/storage.py
--rw-r--r--   0        0        0    14267 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/trigger.py
--rw-r--r--   0        0        0     1294 2023-06-06 13:11:35.449782 sekoia_automation_sdk-1.3.0/sekoia_automation/utils.py
--rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/LICENSE
+-rw-r--r--   0        0        0     8422 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/README.md
+-rw-r--r--   0        0        0     2114 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/__init__.py
+-rw-r--r--   0        0        0    11420 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/action.py
+-rw-r--r--   0        0        0     4964 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/cli.py
+-rw-r--r--   0        0        0      548 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/config.py
+-rw-r--r--   0        0        0     6955 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/connector/__init__.py
+-rw-r--r--   0        0        0     2313 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/connector/workers.py
+-rw-r--r--   0        0        0      426 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/constants.py
+-rw-r--r--   0        0        0      869 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/exceptions.py
+-rw-r--r--   0        0        0      399 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/__init__.py
+-rw-r--r--   0        0        0      383 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/base.py
+-rw-r--r--   0        0        0     1185 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/prometheus.py
+-rw-r--r--   0        0        0    15640 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/module.py
+-rw-r--r--   0        0        0        0 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/__init__.py
+-rw-r--r--   0        0        0     6605 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/generate.py
+-rw-r--r--   0        0        0     2669 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/templates/module.md
+-rw-r--r--   0        0        0     7581 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/files_generator.py
+-rw-r--r--   0        0        0      144 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/cookiecutter.json
+-rw-r--r--   0        0        0      301 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/Dockerfile
+-rw-r--r--   0        0        0      225 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/main.py
+-rw-r--r--   0        0        0      417 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/manifest.json
+-rw-r--r--   0        0        0      647 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/__init__.py
+-rw-r--r--   0        0        0      358 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/tests/conftest.py
+-rw-r--r--   0        0        0      368 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/__init__.py
+-rw-r--r--   0        0        0      140 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/{{cookiecutter.module_name.lower().replace(" ", "_")}}_modules/models.py
+-rw-r--r--   0        0        0    10011 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/openapi.py
+-rwxr-xr-x   0        0        0    14390 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/sync_library.py
+-rw-r--r--   0        0        0     6094 2023-06-08 14:38:05.977886 sekoia_automation_sdk-1.3.1/sekoia_automation/storage.py
+-rw-r--r--   0        0        0    14267 2023-06-08 14:38:05.981886 sekoia_automation_sdk-1.3.1/sekoia_automation/trigger.py
+-rw-r--r--   0        0        0     1294 2023-06-08 14:38:05.981886 sekoia_automation_sdk-1.3.1/sekoia_automation/utils.py
+-rw-r--r--   0        0        0     9717 1970-01-01 00:00:00.000000 sekoia_automation_sdk-1.3.1/PKG-INFO
```

### Comparing `sekoia_automation_sdk-1.3.0/LICENSE` & `sekoia_automation_sdk-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/README.md` & `sekoia_automation_sdk-1.3.1/README.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/pyproject.toml` & `sekoia_automation_sdk-1.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sekoia-automation-sdk"
 
-version = "1.3.0"
+version = "1.3.1"
 description = "SDK to create SEKOIA.IO playbook modules"
 license = "MIT"
 readme = "README.md"
 authors = ["SEKOIA.IO"]
 packages = [
     { include = "sekoia_automation" },
 ]
```

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/action.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/action.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/cli.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/cli.py`

 * *Files 8% similar despite different names*

```diff
@@ -135,23 +135,31 @@
     OpenApiToModule(
         modules_path=modules_path, swagger_file=swagger, use_tags=tags
     ).run()
 
 
 @app.command(name="synchronize-library")
 def sync_library(
-    playbook_url=typer.Argument(..., help="URL of the Playbook API"),
-    api_key=typer.Argument(..., help="Secret key to connect to the Playbook API"),
-    modules_path: Path = typer.Argument(".", help="Path to the playbook modules"),
+    playbook_url=typer.Argument(
+        ..., envvar="PLAYBOOK_URL", help="URL of the Playbook API"
+    ),
+    api_key=typer.Argument(
+        ..., envvar="PLAYBOOK_API_KEY", help="Secret key to connect to the Playbook API"
+    ),
+    modules_path: Path = typer.Option(".", help="Path to the playbook modules"),
     module: str = typer.Option("", help="Module to deploy. Default to all modules"),
     check_image_on_registry: bool = typer.Option(
         False, help="Whether to check registry for existing image"
     ),
-    registry_pat: str = typer.Option("", help="Docker registry personal access token"),
-    registry_user: str = typer.Option("", help="Docker registry username"),
+    registry_pat: str = typer.Option(
+        "", envvar="REGISTRY_PAT", help="Docker registry personal access token"
+    ),
+    registry_user: str = typer.Option(
+        "", envvar="REGISTRY_USER", help="Docker registry username"
+    ),
 ):
     """
     Synchronize the module library to Sekoia.io
     """
     SyncLibrary(
         playbook_url,
         api_key,
```

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/config.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/config.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/connector/__init__.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/connector/workers.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/connector/workers.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/exceptions.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/exceptions.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/metrics/prometheus.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/metrics/prometheus.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/module.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/module.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/generate.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/generate.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/documentation/templates/module.md` & `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/documentation/templates/module.md`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/files_generator.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/files_generator.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml` & `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/new_module/template/{{cookiecutter.module_dir}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/openapi.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/openapi.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/scripts/sync_library.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/scripts/sync_library.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
 import requests
 import typer
 from requests.auth import HTTPBasicAuth
 from rich import print
 
 
 class SyncLibrary:
+    DOCKER_PREFIX = "automation-module-"
+
     def __init__(
         self,
         playbook_url: str,
         api_key: str,
         modules_path: Path,
         registry_pat: str | None = None,
         registry_user: str | None = None,
@@ -226,18 +228,18 @@
         Args:
             manifests (list): List of dict representing the objects to be checked
             module (dict): Data dict of the parent module
 
         Returns:
             list: Modified version of the manifests received as parameter
         """
-        if "docker" in module and "version" in module:
-            for manifest in manifests:
-                if "docker" not in manifest or manifest["docker"] == module["docker"]:
-                    manifest["docker"] = f"{module['docker']}:{module['version']}"
+        module_docker_name = self._get_module_docker_name(module)
+        for manifest in manifests:
+            if "docker" not in manifest or manifest["docker"] == module_docker_name:
+                manifest["docker"] = f"{module_docker_name}:{module['version']}"
 
         return manifests
 
     def get_module_logo(self, module_path: Path) -> str | None:
         """Checks if a logo exists for a given module and returns its path
 
         Args:
@@ -335,15 +337,15 @@
         """
         manifest_path = module_path / "manifest.json"
 
         with manifest_path.open() as fd:
             module_info = json.load(fd)
 
         if self.registry_check and not self.check_image_on_registry(
-            module_info["docker"], module_info["version"]
+            self._get_module_docker_name(module_info), module_info["version"]
         ):
             print(
                 f"[bold red][!] Image {module_info['docker']}:{module_info['version']} "
                 f"not available on registry"
             )
             raise typer.Exit(code=1)
 
@@ -414,7 +416,14 @@
             self.load(
                 library_path=library_path,
             )
         else:
             self.load_module(
                 module_path=self.modules_path.joinpath(self.module).absolute(),
             )
+
+    def _get_module_docker_name(self, manifest: dict) -> str:
+        if docker := manifest.get("docker"):
+            return docker
+        if slug := manifest.get("slug"):
+            return f"{self.DOCKER_PREFIX}{slug}"
+        raise ValueError("Impossible to generate image name")
```

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/storage.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/storage.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/trigger.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/trigger.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/sekoia_automation/utils.py` & `sekoia_automation_sdk-1.3.1/sekoia_automation/utils.py`

 * *Files identical despite different names*

### Comparing `sekoia_automation_sdk-1.3.0/PKG-INFO` & `sekoia_automation_sdk-1.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sekoia-automation-sdk
-Version: 1.3.0
+Version: 1.3.1
 Summary: SDK to create SEKOIA.IO playbook modules
 Home-page: https://sekoia.io/
 License: MIT
 Keywords: SDK,SEKOIA.IO,automation,playbook
 Author: SEKOIA.IO
 Requires-Python: >=3.10,<3.12
 Classifier: Intended Audience :: Developers
```

