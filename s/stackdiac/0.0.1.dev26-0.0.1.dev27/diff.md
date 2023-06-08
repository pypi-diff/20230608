# Comparing `tmp/stackdiac-0.0.1.dev26.tar.gz` & `tmp/stackdiac-0.0.1.dev27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stackdiac-0.0.1.dev26.tar", max compression
+gzip compressed data, was "stackdiac-0.0.1.dev27.tar", max compression
```

## Comparing `stackdiac-0.0.1.dev26.tar` & `stackdiac-0.0.1.dev27.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1066 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/LICENSE
--rw-r--r--   0        0        0     1415 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/README.md
--rw-r--r--   0        0        0      592 2023-06-06 23:58:58.401808 stackdiac-0.0.1.dev26/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/__init__.py
--rw-r--r--   0        0        0       23 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/api/__init__.py
--rw-r--r--   0        0        0     1179 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/api/server.py
--rw-r--r--   0        0        0     1800 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/__init__.py
--rw-r--r--   0        0        0      729 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/build.py
--rw-r--r--   0        0        0     1594 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/create.py
--rw-r--r--   0        0        0      464 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/cli/ui.py
--rw-r--r--   0        0        0      381 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/__init__.py
--rw-r--r--   0        0        0     1145 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/backend.py
--rw-r--r--   0        0        0     2582 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/binary.py
--rw-r--r--   0        0        0    12716 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/cluster.py
--rw-r--r--   0        0        0     2769 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/config.py
--rw-r--r--   0        0        0     2325 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/operation.py
--rw-r--r--   0        0        0      161 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/provider.py
--rw-r--r--   0        0        0     5276 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/repo.py
--rw-r--r--   0        0        0      411 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/secret.py
--rw-r--r--   0        0        0     1716 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/spec.py
--rw-r--r--   0        0        0    12726 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/models/stack.py
--rw-r--r--   0        0        0      108 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/__init__.py
--rw-r--r--   0        0        0      193 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/filters.py
--rw-r--r--   0        0        0      297 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/sdmod.py
--rw-r--r--   0        0        0    11387 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/stackd/stackd.py
--rw-r--r--   0        0        0   164360 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/ui/4753c5ba57962b4d7bf8.woff
--rw-r--r--   0        0        0   121340 2023-06-06 23:58:41.881348 stackdiac-0.0.1.dev26/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
--rw-r--r--   0        0        0  2216438 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js
--rw-r--r--   0        0        0     3087 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js.LICENSE.txt
--rw-r--r--   0        0        0      415 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/ui/index.html
--rw-r--r--   0        0        0        0 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/views/__init__.py
--rw-r--r--   0        0        0      780 2023-06-06 23:58:41.897349 stackdiac-0.0.1.dev26/stackdiac/views/module.py
--rw-r--r--   0        0        0     2327 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev26/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-06-08 13:29:56.996106 stackdiac-0.0.1.dev27/LICENSE
+-rw-r--r--   0        0        0     1415 2023-06-08 13:29:56.996106 stackdiac-0.0.1.dev27/README.md
+-rw-r--r--   0        0        0      616 2023-06-08 13:30:17.488548 stackdiac-0.0.1.dev27/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/__init__.py
+-rw-r--r--   0        0        0       23 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/api/__init__.py
+-rw-r--r--   0        0        0     1179 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/api/server.py
+-rw-r--r--   0        0        0     1800 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/__init__.py
+-rw-r--r--   0        0        0      729 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/build.py
+-rw-r--r--   0        0        0     1594 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/create.py
+-rw-r--r--   0        0        0      464 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/cli/ui.py
+-rw-r--r--   0        0        0      381 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/__init__.py
+-rw-r--r--   0        0        0     1145 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/backend.py
+-rw-r--r--   0        0        0     2582 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/binary.py
+-rw-r--r--   0        0        0    12716 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/cluster.py
+-rw-r--r--   0        0        0     2769 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/config.py
+-rw-r--r--   0        0        0     2325 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/operation.py
+-rw-r--r--   0        0        0      161 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/provider.py
+-rw-r--r--   0        0        0     5276 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/repo.py
+-rw-r--r--   0        0        0      411 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/secret.py
+-rw-r--r--   0        0        0     1716 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/spec.py
+-rw-r--r--   0        0        0    12809 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/models/stack.py
+-rw-r--r--   0        0        0      108 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/__init__.py
+-rw-r--r--   0        0        0      193 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/filters.py
+-rw-r--r--   0        0        0      297 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/sdmod.py
+-rw-r--r--   0        0        0    11901 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/stackd/stackd.py
+-rw-r--r--   0        0        0   164360 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/ui/4753c5ba57962b4d7bf8.woff
+-rw-r--r--   0        0        0   121340 2023-06-08 13:29:57.000106 stackdiac-0.0.1.dev27/stackdiac/ui/6d63d0501e5ed7b79dab.woff2
+-rw-r--r--   0        0        0  2216438 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js
+-rw-r--r--   0        0        0     3087 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js.LICENSE.txt
+-rw-r--r--   0        0        0      415 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/ui/index.html
+-rw-r--r--   0        0        0        0 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/views/__init__.py
+-rw-r--r--   0        0        0      780 2023-06-08 13:29:57.016106 stackdiac-0.0.1.dev27/stackdiac/views/module.py
+-rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 stackdiac-0.0.1.dev27/PKG-INFO
```

### Comparing `stackdiac-0.0.1.dev26/LICENSE` & `stackdiac-0.0.1.dev27/LICENSE`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/README.md` & `stackdiac-0.0.1.dev27/README.md`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/pyproject.toml` & `stackdiac-0.0.1.dev27/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stackdiac"
-version = "0.0.1-dev26"
+version = "0.0.1-dev27"
 description = ""
 authors = ["sysr9 <38893296+sysr9@users.noreply.github.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
@@ -16,14 +16,15 @@
 requests = "^2.28.2"
 jinja2 = "^3.1.2"
 deepmerge = "^1.1.0"
 fastapi = "^0.95.0"
 uvicorn = "^0.21.1"
 mergedeep = "^1.3.4"
 hvac = "^1.1.0"
+pyyaml-include = "^1.3"
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
```

### Comparing `stackdiac-0.0.1.dev26/stackdiac/api/server.py` & `stackdiac-0.0.1.dev27/stackdiac/api/server.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/cli/__init__.py` & `stackdiac-0.0.1.dev27/stackdiac/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/cli/build.py` & `stackdiac-0.0.1.dev27/stackdiac/cli/build.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/cli/create.py` & `stackdiac-0.0.1.dev27/stackdiac/cli/create.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/backend.py` & `stackdiac-0.0.1.dev27/stackdiac/models/backend.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/binary.py` & `stackdiac-0.0.1.dev27/stackdiac/models/binary.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/cluster.py` & `stackdiac-0.0.1.dev27/stackdiac/models/cluster.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/config.py` & `stackdiac-0.0.1.dev27/stackdiac/models/config.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/operation.py` & `stackdiac-0.0.1.dev27/stackdiac/models/operation.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/repo.py` & `stackdiac-0.0.1.dev27/stackdiac/models/repo.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/spec.py` & `stackdiac-0.0.1.dev27/stackdiac/models/spec.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/models/stack.py` & `stackdiac-0.0.1.dev27/stackdiac/models/stack.py`

 * *Files 6% similar despite different names*

```diff
@@ -49,38 +49,32 @@
 class ModuleSecret(BaseModel):
     name: str | None = None
     secret_type: str | None = None
     secret_schema: dict | None = None
     required: bool = False
     status: ModuleSecretStatus = ModuleSecretStatus.UNKNOWN
 
-    def build(self, cluster, cluster_stack, stack, sd, module, status, **kwargs):
-        logger.info(f"building secret {self.name} for {module.name}")
+    def build(self, cluster, cluster_stack, stack, sd, module, status, **kwargs):       
 
         if self.secret_schema is None and self.secret_type is not None:
             # extracting schema from stack.schema.components.schemas
             self.secret_schema = stack.stack_schema['components']['schemas'][self.secret_type]
             self.status = status
 
 class ModuleSchemas(BaseModel):
     secrets: dict[str, ModuleSecret] = {}
     vars: str | None = None
 
     schemas: dict[str, Any] = {}
 
-    def build(self, cluster, cluster_stack, stack, sd, module, **kwargs):
-        logger.info(f"building schemas for {module.name}")
-
+    def build(self, cluster, cluster_stack, stack, sd, module, **kwargs):        
         if self.vars:
             self.schemas["vars"] = stack.stack_schema['components']['schemas'][self.vars]
 
-        # if self.secrets:
-        #     for name, secret in self.secrets.items():
-        #         secret.build(cluster, cluster_stack, stack, sd, module, status, **kwargs)
-        #         self.schemas[name] = SpecModel.parse_obj(secret.secret_schema)
+  
 
 class Module(BaseModel):
     name: str | None = None
     source: str | None = None
     src: str | None = None
     vars: dict[str, Any] = {}
     module_vars: dict[str, Any] = {}
@@ -310,14 +304,22 @@
             status = ModuleSecretStatus.EXISTS if s.name in vault_module_secrets else ModuleSecretStatus.NOT_EXISTS
             s.build(cluster, cluster_stack, stack, sd, module=self, status=status, **kwargs)
         
         # building schemas
 
         if self.schemas:
             self.schemas.build(cluster, cluster_stack, stack, sd, module=self, **kwargs)
+
+        if not self.module_vars and self.schemas and self.schemas.vars:
+            logger.info("copying built vars to module vars")
+            for v in self.schemas.schemas["vars"]["properties"].keys():                
+                _v = self.built_vars.get(v, self.schemas.schemas["vars"]["properties"][v].get("default", None))
+                logger.info(f"copying {v}={_v}")
+                if _v:
+                    self.module_vars[v] = _v
         
         ctx = dict(module=self, cluster=cluster, stackd=sd, vars=_vars, 
             inputs=list(self.build_deps(stack=stack, cluster=cluster, module=self, deps=self.inputs, sd=sd, **kwargs)),
             module_deps=[ d.abspath for d in list(self.build_deps(stack=stack, cluster=cluster, module=self, 
                 deps=self.deps, sd=sd, **kwargs)) ],
             vars_list=list(get_vars_list()),
             tf_backend=bk.build(sd, stack, self, cluster, cluster_stack, **kwargs),
```

### Comparing `stackdiac-0.0.1.dev26/stackdiac/stackd/stackd.py` & `stackdiac-0.0.1.dev27/stackdiac/stackd/stackd.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,19 @@
 import json
 import logging, yaml, os
 from jinja2 import Environment, FileSystemLoader
 import time
 from urllib.parse import parse_qs, urlparse
 
 from pydantic import parse_obj_as, BaseModel
-from typing import Any
+from typing import Any, Optional, Pattern, Sequence, Tuple
 import subprocess
 from deepmerge import always_merger
-
+from yamlinclude import YamlIncludeConstructor
+from yamlinclude.readers import Reader
 
 from stackdiac import models
 from stackdiac.models.provider import Provider
 from ..models import spec
 
 import hvac
 
@@ -49,14 +50,45 @@
     pass
 
 class StackdModel(BaseModel):
     conf: models.ConfigModel | None = None
     root: str = os.environ.get("STACKD_ROOT", ".")
     clusters: dict[str, models.ClusterModel] = {}    
     providers: dict[str, models.Provider] = {}
+
+
+class RepoYamlIncludeConstructor(YamlIncludeConstructor):
+    def __init__(self, sd, *args, **kwargs):
+        self.sd = sd
+        super().__init__(*args, **kwargs)
+
+    def get_fragment(self, data, fragment):
+        # fragment is a path to a dict key, e.g. "/components/schemas/Resources" from openapi spec
+        # it is parsed and element is fetched from data then returned
+        fragments = [ f for f in fragment.split("/") if f ]
+        if len(fragments) == 1:
+            return data[fragments[0]]
+        else:
+            return self.get_fragment(data[fragments[0]], "/".join(fragments[1:]))
+        
+
+    def load(
+            self,
+            loader,
+            pathname: str,
+            *args, **kwargs):
+        
+        path, fragment = self.sd.resolve_path(pathname, with_fragment=True)
+        
+        data = super().load(loader, path, *args, **kwargs)
+        if fragment:
+            return self.get_fragment(data, fragment)
+        
+        return data
+
     
 class Stackd(StackdModel):
     conf: models.Config | None = None
     counters: StackdCounters = StackdCounters()
     vault: hvac.Client | None = None
 
     class Config:
@@ -77,39 +109,14 @@
         else:
             logger.debug("don't forget to run configure()")
 
     @property
     def builddir(self):
         return os.path.join(self.root, "build")
 
-    def parse_tunnel(self, tunnel_qs: str) -> str:
-        
-        spec = dict(
-            ssh = {},
-            remote = {},
-            local = {},
-        )
-
-        qs = parse_qs(tunnel_qs)
-
-        spec["ssh"]["username"], server_hostport = qs["server"][0].split("@")
-        spec["ssh"]["host"], spec["ssh"]["port"] = server_hostport.split(":")
-        spec["ssh"]["port"] = int(spec["ssh"]["port"])
-
-        spec["remote"]["host"], spec["remote"]["port"] = qs["remote"][0].split(":")
-        spec["remote"]["port"] = int(spec["remote"]["port"])
-
-        local_endpoint, spec["local"]["port"] = qs["local"][0].split(":")
-        spec["local"]["port"] = int(spec["local"]["port"])
-        spec["local"]["service"], spec["local"]["namespace"] = local_endpoint.split(".")
-
-        
-        logger.info(f"parsing tunnel {qs} {spec}")
-        return json.dumps(spec)
-
     def tpl_readfile_func(self, jinja_env):
         def func(path: str) -> str:
             return jinja_env.get_template(path).render(stackd=self)            
         return func
   
 
     def configure(self):
@@ -119,15 +126,15 @@
         os.chdir(self.root)
         logger.debug(f"{self} chdir to {self.root}")
 
         self.conf = spec.Spec(path=self.config_file,
                 merge_from=models.get_initial_config(name="unconfigured", domain="example.com", 
                                                         vault_address="http://127.0.0.1:9090").dict()
                                             ).parse_obj_as(config.Config)
-
+        RepoYamlIncludeConstructor(sd=self).add_to_loader_class(loader_class=yaml.SafeLoader, base_dir=self.root, sd=self)
         try:
             self.vault = hvac.Client(url=self.conf.vars['vault_address'],
                                     token=os.environ['TF_VAR_vault_token'])
         except KeyError:
             logger.error(f"{self} vault not configured. set TF_VAR_vault_token")
             raise ProcessException("vault not configured. set TF_VAR_vault_token")
         else:
@@ -257,25 +264,28 @@
             path = os.path.join(repo.repo_dir, parsed_src.path.lstrip("/"))           
         else:
             path = os.path.join(repo.repo_dir, parsed_src.path.lstrip("/"), "stack.yaml")
         
         return path
 
 
-    def resolve_path(self, src):
+    def resolve_path(self, src, with_fragment=False):
         """
         Resolve a module path to a local path
         repo can be specified as scheme: prefix
         """
         parsed_src = urlparse(src)
         if not parsed_src.scheme:
-            parsed_src = urlparse(f"root:{src}") # add root repo
-       
+            parsed_src = urlparse(f"root:{src}") # add root repo       
+        
         repo = self.conf.repos[parsed_src.scheme]
-        return os.path.join(repo.repo_dir, parsed_src.path)
+        if with_fragment:
+            return os.path.join(repo.repo_dir, parsed_src.path), parsed_src.fragment
+        else:
+            return os.path.join(repo.repo_dir, parsed_src.path)
     
     resolve_module_path = resolve_path
 
     def terragrunt(self, target, terragrunt_options:list[str], **kwargs):
         env = dict(
             TERRAGRUNT_WORKING_DIR=target,
             TERRAGRUNT_TFPATH=self.conf.binaries.terraform.abspath,
```

### Comparing `stackdiac-0.0.1.dev26/stackdiac/ui/4753c5ba57962b4d7bf8.woff` & `stackdiac-0.0.1.dev27/stackdiac/ui/4753c5ba57962b4d7bf8.woff`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/ui/6d63d0501e5ed7b79dab.woff2` & `stackdiac-0.0.1.dev27/stackdiac/ui/6d63d0501e5ed7b79dab.woff2`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js` & `stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/ui/bundle.js.LICENSE.txt` & `stackdiac-0.0.1.dev27/stackdiac/ui/bundle.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/stackdiac/views/module.py` & `stackdiac-0.0.1.dev27/stackdiac/views/module.py`

 * *Files identical despite different names*

### Comparing `stackdiac-0.0.1.dev26/PKG-INFO` & `stackdiac-0.0.1.dev27/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stackdiac
-Version: 0.0.1.dev26
+Version: 0.0.1.dev27
 Summary: 
 License: MIT
 Author: sysr9
 Author-email: 38893296+sysr9@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -16,14 +16,15 @@
 Requires-Dist: fastapi (>=0.95.0,<0.96.0)
 Requires-Dist: gitpython (>=3.1.31,<4.0.0)
 Requires-Dist: hvac (>=1.1.0,<2.0.0)
 Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: mergedeep (>=1.3.4,<2.0.0)
 Requires-Dist: pydantic (>=1.10.6,<2.0.0)
 Requires-Dist: pyyaml (>=6.0,<7.0)
+Requires-Dist: pyyaml-include (>=1.3,<2.0)
 Requires-Dist: requests (>=2.28.2,<3.0.0)
 Requires-Dist: uvicorn (>=0.21.1,<0.22.0)
 Description-Content-Type: text/markdown
 
 # Stackd IAC
 
 IAC stack
```

