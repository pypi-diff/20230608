# Comparing `tmp/pdm-multirun-0.2.0.tar.gz` & `tmp/pdm_multirun-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm-multirun-0.2.0.tar", last modified: Mon Dec  5 14:26:14 2022, max compression
+gzip compressed data, was "pdm_multirun-0.3.0.tar", last modified: Thu Jun  8 14:08:15 2023, max compression
```

## Comparing `pdm-multirun-0.2.0.tar` & `pdm_multirun-0.3.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0 pawamoy   (1000) users      (985)      754 2022-12-05 09:16:51.461043 pdm-multirun-0.2.0/LICENSE
--rw-r--r--   0 pawamoy   (1000) users      (985)     2352 2022-12-05 14:20:24.874608 pdm-multirun-0.2.0/README.md
--rw-r--r--   0 pawamoy   (1000) users      (985)     3127 2022-12-05 09:18:16.971937 pdm-multirun-0.2.0/pyproject.toml
--rw-r--r--   0 pawamoy   (1000) users      (985)      187 2022-12-05 09:16:51.374379 pdm-multirun-0.2.0/src/pdm_multirun/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)     2644 2022-12-05 14:15:43.833878 pdm-multirun-0.2.0/src/pdm_multirun/plugin.py
--rw-r--r--   0 pawamoy   (1000) users      (985)        0 2022-12-05 09:16:51.367713 pdm-multirun-0.2.0/src/pdm_multirun/py.typed
--rw-r--r--   0 pawamoy   (1000) users      (985)      165 2022-12-05 09:16:51.361046 pdm-multirun-0.2.0/tests/__init__.py
--rw-r--r--   0 pawamoy   (1000) users      (985)       47 2022-12-05 09:16:51.361046 pdm-multirun-0.2.0/tests/conftest.py
--rw-r--r--   0 pawamoy   (1000) users      (985)      144 2022-12-05 09:32:03.277935 pdm-multirun-0.2.0/tests/test_plugin.py
--rw-------   0 pawamoy   (1000) users      (985)     3821 2022-12-05 14:26:14.648032 pdm-multirun-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-06-08 13:02:32.508182 pdm_multirun-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2353 2023-06-08 13:02:35.261493 pdm_multirun-0.3.0/README.md
+-rw-r--r--   0        0        0     2535 2023-06-08 14:08:15.587166 pdm_multirun-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      150 2023-06-08 13:02:32.381516 pdm_multirun-0.3.0/src/pdm_multirun/__init__.py
+-rw-r--r--   0        0        0     3208 2023-06-08 14:07:21.166026 pdm_multirun-0.3.0/src/pdm_multirun/plugin.py
+-rw-r--r--   0        0        0        0 2023-06-08 13:02:32.378183 pdm_multirun-0.3.0/src/pdm_multirun/py.typed
+-rw-r--r--   0        0        0      165 2023-06-08 13:02:32.371516 pdm_multirun-0.3.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-06-08 13:02:32.368183 pdm_multirun-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      155 2023-06-08 13:53:36.229321 pdm_multirun-0.3.0/tests/test_plugin.py
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 pdm_multirun-0.3.0/PKG-INFO
```

### Comparing `pdm-multirun-0.2.0/LICENSE` & `pdm_multirun-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm-multirun-0.2.0/README.md` & `pdm_multirun-0.3.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -66,11 +66,11 @@
 if MULTIRUN:
     py = f"{sys.version_info[0]}.{sys.version_info[1]}"  # 3.8, 3.9, etc.
     ...  # use `py` string accordingly
 ```
 
 ---
 
-PDM Multirun successively run the `pdm use` then `pdm run` internal actions.
+PDM Multirun successively runs the `pdm use` then `pdm run` internal actions.
 If the command fails on a Python version, PDM Multirun stops there.
 It any case, PDM Multirun will restore the Python version
 saved in `.pdm.toml` (through the `pdm use` command) before exiting.
```

### Comparing `pdm-multirun-0.2.0/src/pdm_multirun/plugin.py` & `pdm_multirun-0.3.0/src/pdm_multirun/plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,70 +1,88 @@
 """PDM Multirun plugin."""
 
 from __future__ import annotations
 
-import argparse
 import os
+from typing import TYPE_CHECKING
 
 from pdm import termui
 from pdm.cli import actions
 from pdm.cli.commands.run import Command as RunCommand
 from pdm.cli.commands.run import Project
 from pdm.cli.hooks import HookManager
 
+if TYPE_CHECKING:
+    import argparse
+
+    from pdm.core import Core
+
 PYTHON_VERSIONS = os.getenv("PDM_MULTIRUN_VERSIONS", "").split()
-PYTHON_VERSIONS = PYTHON_VERSIONS or [f"python3.{minor}" for minor in range(7, 12)]  # noqa: WPS432
+PYTHON_VERSIONS = PYTHON_VERSIONS or [f"python3.{minor}" for minor in range(7, 12)]
 
 
 def _interpreters(versions: str) -> list[str]:
     return [f"python{version.strip()}" for version in versions.split(",")]
 
 
 class MultirunCommand(RunCommand):
     """Run a command under multiple Python versions."""
 
     def add_arguments(self, parser: argparse.ArgumentParser) -> None:  # noqa: D102
         super().add_arguments(parser)
         parser.add_argument(
+            "-f",
+            "--fail-fast",
+            help="Exit as soon as an interpreter cannot be found or used",
+            action="store_true",
+            default=False,
+        )
+        parser.add_argument(
             "-i",
             "--interpreters",
             "--versions",
             help="Comma-separated list of Python versions to run the command with",
             type=_interpreters,
         )
 
     def handle(self, project: Project, options: argparse.Namespace) -> None:  # noqa: D102
         os.environ["PDM_MULTIRUN"] = "1"
         old_python = str(project.environment.interpreter.path)
         project.core.ui.echo(f"Current interpreter: {old_python}", verbosity=termui.Verbosity.DETAIL)
         for python_version in options.interpreters or PYTHON_VERSIONS:
-            self._use(project, options, python_version)
+            try:
+                self._use(project, options, python_version)
+            except Exception:  # noqa: BLE001
+                if options.fail_fast:
+                    raise
+                project.core.ui.echo(f"Skipped interpreter: {python_version}", verbosity=termui.Verbosity.DETAIL)
+                continue
             try:
                 super().handle(project, options)
             except SystemExit as exit:
                 if exit.code:
                     self._use(project, options, old_python)
                     raise
         project.core.ui.echo(f"Restoring interpreter: {old_python}", verbosity=termui.Verbosity.DETAIL)
         self._use(project, options, old_python)
         os.environ.pop("PDM_MULTIRUN", None)
 
     def _use(self, project: Project, options: argparse.Namespace, python: str) -> None:
         old_echo = project.core.ui.echo
         if not options.verbose:
-            project.core.ui.echo = lambda *args, **kwargs: None  # type: ignore[assignment]
+            project.core.ui.echo = lambda *args, **kwargs: None  # type: ignore[method-assign]
         # unset cached environment
         project.environment = None  # type: ignore[assignment]
-        try:  # noqa: WPS501
+        try:
             actions.do_use(
                 project,
                 python=python,
                 first=True,
                 ignore_remembered=False,
                 hooks=HookManager(project, skip=options.skip),
             )
         finally:
-            project.core.ui.echo = old_echo  # type: ignore[assignment]
+            project.core.ui.echo = old_echo  # type: ignore[method-assign]
 
 
-def multirun(core):  # noqa: D103
+def multirun(core: Core) -> None:  # noqa: D103
     core.register_command(MultirunCommand, "multirun")
```

### Comparing `pdm-multirun-0.2.0/PKG-INFO` & `pdm_multirun-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 Metadata-Version: 2.1
 Name: pdm-multirun
-Version: 0.2.0
+Version: 0.3.0
 Summary: A PDM plugin to run a command on multiple Python versions.
+Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
-Author-email: Timothée Mazzucotelli <pawamoy@pm.me>
-Requires-Python: >=3.7
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
+Project-URL: Homepage, https://pawamoy.github.io/pdm-multirun
+Project-URL: Documentation, https://pawamoy.github.io/pdm-multirun
 Project-URL: Changelog, https://pawamoy.github.io/pdm-multirun/changelog
+Project-URL: Repository, https://github.com/pawamoy/pdm-multirun
+Project-URL: Issues, https://github.com/pawamoy/pdm-multirun/issues
 Project-URL: Discussions, https://github.com/pawamoy/pdm-multirun/discussions
-Project-URL: Documentation, https://pawamoy.github.io/pdm-multirun
-Project-URL: Funding, https://github.com/sponsors/pawamoy
 Project-URL: Gitter, https://gitter.im/pdm-multirun/community
-Project-URL: Homepage, https://pawamoy.github.io/pdm-multirun
-Project-URL: Issues, https://github.com/pawamoy/pdm-multirun/issues
-Project-URL: Repository, https://github.com/pawamoy/pdm-multirun
+Project-URL: Funding, https://github.com/sponsors/pawamoy
+Requires-Python: >=3.7
+Requires-Dist: pdm>=2
 Description-Content-Type: text/markdown
 
 # PDM Multirun
 
 [![ci](https://github.com/pawamoy/pdm-multirun/workflows/ci/badge.svg)](https://github.com/pawamoy/pdm-multirun/actions?query=workflow%3Aci)
 [![documentation](https://img.shields.io/badge/docs-mkdocs%20material-blue.svg?style=flat)](https://pawamoy.github.io/pdm-multirun/)
 [![pypi version](https://img.shields.io/pypi/v/pdm-multirun.svg)](https://pypi.org/project/pdm-multirun/)
@@ -98,12 +98,11 @@
 if MULTIRUN:
     py = f"{sys.version_info[0]}.{sys.version_info[1]}"  # 3.8, 3.9, etc.
     ...  # use `py` string accordingly
 ```
 
 ---
 
-PDM Multirun successively run the `pdm use` then `pdm run` internal actions.
+PDM Multirun successively runs the `pdm use` then `pdm run` internal actions.
 If the command fails on a Python version, PDM Multirun stops there.
 It any case, PDM Multirun will restore the Python version
 saved in `.pdm.toml` (through the `pdm use` command) before exiting.
-
```

