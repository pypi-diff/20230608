# Comparing `tmp/un_yaml-0.3.0.tar.gz` & `tmp/un_yaml-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "un_yaml-0.3.0.tar", max compression
+gzip compressed data, was "un_yaml-0.3.1.tar", max compression
```

## Comparing `un_yaml-0.3.0.tar` & `un_yaml-0.3.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.3.0/LICENSE
--rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.3.0/README.md
--rw-r--r--   0        0        0      751 2023-06-05 13:59:26.405560 un_yaml-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      441 2023-06-02 07:14:32.763817 un_yaml-0.3.0/un_yaml/__init__.py
--rw-r--r--   0        0        0      695 2023-06-05 13:59:26.408347 un_yaml-0.3.0/un_yaml/cli.yaml
--rw-r--r--   0        0        0        0 2023-06-02 07:14:32.763900 un_yaml-0.3.0/un_yaml/py.typed
--rw-r--r--   0        0        0     4070 2023-06-05 13:59:26.409191 un_yaml-0.3.0/un_yaml/un_cli.py
--rw-r--r--   0        0        0     1058 2023-06-05 13:59:26.409985 un_yaml-0.3.0/un_yaml/un_conf.py
--rw-r--r--   0        0        0     2180 2023-06-02 07:14:32.765632 un_yaml-0.3.0/un_yaml/un_uri.py
--rw-r--r--   0        0        0     3048 2023-06-05 13:59:26.410872 un_yaml-0.3.0/un_yaml/un_yaml.py
--rw-r--r--   0        0        0      190 2023-06-02 07:14:32.766902 un_yaml-0.3.0/un_yaml/wrapper.py
--rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 un_yaml-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-31 12:54:36.386488 un_yaml-0.3.1/LICENSE
+-rw-r--r--   0        0        0      100 2023-05-31 12:54:36.387406 un_yaml-0.3.1/README.md
+-rw-r--r--   0        0        0      751 2023-06-08 06:13:35.908661 un_yaml-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      202 2023-06-08 06:13:35.911129 un_yaml-0.3.1/un_yaml/__init__.py
+-rw-r--r--   0        0        0     2703 2023-06-08 06:13:35.912052 un_yaml-0.3.1/un_yaml/cli.yaml
+-rw-r--r--   0        0        0        0 2023-06-02 07:14:32.763900 un_yaml-0.3.1/un_yaml/py.typed
+-rw-r--r--   0        0        0     4821 2023-06-08 06:13:35.913072 un_yaml-0.3.1/un_yaml/un_cli.py
+-rw-r--r--   0        0        0     1013 2023-06-08 06:13:35.914001 un_yaml-0.3.1/un_yaml/un_conf.py
+-rw-r--r--   0        0        0     2180 2023-06-02 07:14:32.765632 un_yaml-0.3.1/un_yaml/un_uri.py
+-rw-r--r--   0        0        0     3230 2023-06-08 06:13:35.914781 un_yaml-0.3.1/un_yaml/un_yaml.py
+-rw-r--r--   0        0        0      190 2023-06-02 07:14:32.766902 un_yaml-0.3.1/un_yaml/wrapper.py
+-rw-r--r--   0        0        0      789 1970-01-01 00:00:00.000000 un_yaml-0.3.1/PKG-INFO
```

### Comparing `un_yaml-0.3.0/LICENSE` & `un_yaml-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `un_yaml-0.3.0/pyproject.toml` & `un_yaml-0.3.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "un_yaml"
-version = "0.3.0"
+version = "0.3.1"
 description = "Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 anyio = "^3.7.0"
```

### Comparing `un_yaml-0.3.0/un_yaml/un_cli.py` & `un_yaml-0.3.1/un_yaml/un_cli.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,96 +1,111 @@
 import logging
 from argparse import ArgumentParser, Namespace
 from collections.abc import Sequence
 from pathlib import Path  # NOQA F401
 from sys import stdout
 from typing import Any
 
-
 from .un_conf import UnConf
 from .un_uri import UnUri
-from .un_yaml import UnYaml, __version__
+from .un_yaml import UnYaml
 
 # Harcode most parameters for now
 # TODO: infer them from the YAML file
 
 
 class UnCli(UnYaml):
     """Use UnYaml to create a CLI from a YAML file."""
 
     CLI_YAML = "cli.yaml"
-    CMD = "commands"
     ARG_KEYS = (
         "dest,metavar,type,default,required,choices,action,nargs,const,help".split(",")
     )
+    K_ARG = "argument"
+    K_CMD = "command"
+    K_OPT = "option"
     K_VER = "version"
+    K_VRB = "verbose"
+    K_GLOB = "global"
 
     @staticmethod
-    def ARG_KWS(arg: dict):
+    def VALID_KEYS(arg: dict):
         kwargs = {k: v for k, v in arg.items() if k in UnCli.ARG_KEYS}
-        kwargs["type"] = eval(kwargs["type"]) if "type" in kwargs else str
+        if "type" in kwargs:
+            kwargs["type"] = eval(kwargs["type"])
         return kwargs
 
-    def __init__(self, pkg: str, file=CLI_YAML, dir=".") -> None:
+    def __init__(self, pkg: str, version: str, file=CLI_YAML, dir=".") -> None:
         yaml_data = UnYaml.LoadYaml(file, pkg)
         super().__init__(yaml_data)
-        if UnCli.CMD not in self.data:
-            raise ValueError(f"'{UnCli.CMD}' not in file '{file}':\n{self.data}")
-        self.cmds = self.get(UnCli.CMD)
+        if UnCli.K_CMD not in self.data:
+            raise ValueError(f"'{UnCli.K_CMD}' not in file '{file}':\n{self.data}")
+        self.version = version
+        self.cmds = self.get(UnCli.K_CMD)
         self.doc = self.get_handler("doc")()
         self.path = Path(dir) / UnCli.DEFAULT
         self.conf = UnConf(self.path, doc=type(self.doc).__name__)
 
     def parse_version(self, parser: ArgumentParser) -> None:
         doc_name = self.info("doc")
         parser.add_argument(
-            "-v",
+            "-V",
             f"--{UnCli.K_VER}",
             action="store_const",
-            const=f"{doc_name} {__version__}",
+            const=f"{doc_name} {self.version}",
             help="Show version and exit.",
         )
 
     def make_parser(self) -> ArgumentParser:
-        parser = ArgumentParser(self.get("doc"))
+        parser = ArgumentParser(self.info("doc"))
         self.parse_version(parser)
-        subparsers = parser.add_subparsers(dest="command")
+        subparsers = parser.add_subparsers(dest=UnCli.K_CMD)
         for cmd, opts in self.cmds.items():
             if cmd[0] != "_":
                 subparser = subparsers.add_parser(cmd, help=opts["help"])
-                args = opts.get("arguments")
-                for arg in args or []:
-                    subparser.add_argument(arg["name"], **UnCli.ARG_KWS(arg))
+                for arg in opts.get(UnCli.K_ARG, []):
+                    subparser.add_argument(arg["name"], **UnCli.VALID_KEYS(arg))
+                for opt in opts.get(UnCli.K_OPT, []):
+                    subparser.add_argument(
+                        opt["short"], opt["name"], **UnCli.VALID_KEYS(opt)
+                    )
+                globs = self.get(UnCli.K_GLOB) or {}
+                for gopts in globs.values():
+                    subparser.add_argument(gopts["name"], **UnCli.VALID_KEYS(gopts))
         return parser
 
     async def run(self, argv: Sequence[str] | None, out=stdout):
-        args: Any = self.parse(argv)
+        args = self.parse(argv)
         if not args:
             return False
         if hasattr(args, UnCli.K_VER) and args.version:
             print(args.version, file=out)
             return False
+        if hasattr(args, UnCli.K_VRB) and args.verbose:
+            logging.basicConfig()
+            logging.getLogger().setLevel(logging.DEBUG)
         return await self.execute(args, out)
 
     def parse(self, argv: Sequence[str] | None) -> Namespace | None:
         parser = self.make_parser()
         args = parser.parse_args(argv)
+        logging.debug(f"UnCli.parse.args: {args}")
         if args.command is None and not args.version:
             parser.print_help()
             return None
         return args
 
     def get_resource(self, uri: UnUri) -> Any:
         handler = self.get_handler(uri.tool())
-        logging.debug(f"handler: {handler}")
+        logging.debug(f"get_resource.handler: {handler}")
         return handler(uri.attrs)
 
     def log_resource(self, argv: dict):
         args = argv.copy()
-        args.pop(UnCli.K_VER, None)
+        args[UnCli.K_VER] = self.version
         uri = args.pop(UnUri.ARG_URI)
         tool = uri.tool()
         opts = {str(uri): args}
         logging.debug(f"tool[{tool}] {opts}")
         self.conf.put(tool, opts)
         self.conf.save()
 
@@ -107,14 +122,15 @@
         cmd = args.command
         if cmd not in self.cmds:
             logging.error(f"Unknown command: {cmd}\n{args}")
             exit(1)
 
         argv = vars(args)
         self.resource(argv)
+        logging.debug(f"UnCli.execute.argv: {argv}")
 
         results = await self.doc.execute(cmd, argv)
         return self.echo(results, out)
 
     def echo(self, results: list, out=stdout):
         """Print result of calling a method."""
         [print(f'"{item}"', file=out) for item in results]
```

### Comparing `un_yaml-0.3.0/un_yaml/un_conf.py` & `un_yaml-0.3.1/un_yaml/un_conf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 import logging
 from pathlib import Path  # NOQA F401
 from typing import Any
 
-from yaml import safe_dump, safe_load
+from yaml import safe_dump
 
-from .un_yaml import __version__
 from .un_yaml import UnYaml
 
 
 class UnConf(UnYaml):
     """Editable subclass of UnYaml."""
 
     @staticmethod
     def SaveYaml(path: Path, yaml_data: dict):
         with path.open("w") as outfile:
             safe_dump(yaml_data, outfile)
 
-
     def __init__(self, path: Path, **defaults) -> None:
         yaml_data = UnConf.ReadYaml(path.resolve(), defaults)
         super().__init__(yaml_data)
         self.path = path.resolve()
 
     def save(self):
         UnConf.SaveYaml(self.path, self.data)
```

### Comparing `un_yaml-0.3.0/un_yaml/un_uri.py` & `un_yaml-0.3.1/un_yaml/un_uri.py`

 * *Files identical despite different names*

### Comparing `un_yaml-0.3.0/un_yaml/un_yaml.py` & `un_yaml-0.3.1/un_yaml/un_yaml.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 from importlib import import_module, resources
 from importlib.metadata import version
-from typing import Any, Callable
 from pathlib import Path
+from typing import Any, Callable
 
 from yaml import safe_load
 
 __version__: str = version("un_yaml")
 
+
 class UnYaml:
     KEY = "_yaml"
+    K_HANDLER = "handler"
     SEP = "/"
     PREFIX = "#/"
     REF = "$ref"
     REF_ERROR = f"Value for Key {REF} does not start with {PREFIX}"
+    VAL_ERROR = f"Value for Key {REF} not deferencable"
+
     DEFAULT = "data.yaml"
     DEFAULT_INFO = {
         "_version": __version__,
         "app": "data-yaml",
         "app_version": "0.0.1",
         "doc": __name__,
         "doc_version": "0.0.1",
@@ -67,14 +71,16 @@
         return item
 
     def _expand(self, item):
         ref = item[UnYaml.REF]
         if not ref.startswith(UnYaml.PREFIX):
             raise ValueError(f"cannot expand {ref}: {UnYaml.REF_ERROR}")
         value = self.get(ref[2:])
+        if not value:
+            raise ValueError(f"cannot get {ref}: {UnYaml.VAL_ERROR}")
         for key in item:
             if key != UnYaml.REF:
                 value[key] = item[key]
         return self.expand(value)
 
     def _get(self, result, key: str):
         if not result:
@@ -88,14 +94,14 @@
         for key in keylist.split(UnYaml.SEP):
             item = self._get(result, key)
             result = self.expand(item)
 
         return result
 
     def get_handler(self, key: str) -> Callable:
-        handlers = self.info("handlers")
+        handlers = self.info(UnYaml.K_HANDLER)
         handler = handlers.get(key)
         if not handler:
             raise ValueError(f"UnYaml.get_handler: no handler for {key}")
 
         module = import_module(handler["module"])
         return getattr(module, handler["method"])
```

### Comparing `un_yaml-0.3.0/PKG-INFO` & `un_yaml-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: un-yaml
-Version: 0.3.0
+Version: 0.3.1
 Summary: Universal YAML: replace repetitive code with your own Domain-Specific un-Language (DSuL)
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

