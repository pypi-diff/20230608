# Comparing `tmp/coveo-stew-3.0a4.tar.gz` & `tmp/coveo-stew-3.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coveo-stew-3.0a4.tar", max compression
+gzip compressed data, was "coveo-stew-3.0a5.tar", max compression
```

## Comparing `coveo-stew-3.0a4.tar` & `coveo-stew-3.0a5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0    11357 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/LICENSE
--rw-r--r--   0        0        0      561 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/LICENSE.md
--rw-r--r--   0        0        0    14175 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/README.md
--rw-r--r--   0        0        0        0 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/__init__.py
--rw-r--r--   0        0        0       99 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/__main__.py
--rw-r--r--   0        0        0        0 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/__init__.py
--rw-r--r--   0        0        0     4106 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/any_runner.py
--rw-r--r--   0        0        0     1573 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/black_runner.py
--rw-r--r--   0        0        0     5278 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/config.py
--rw-r--r--   0        0        0     3554 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/mypy_runner.py
--rw-r--r--   0        0        0      622 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/poetry_runners.py
--rw-r--r--   0        0        0     1409 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/pytest_runner.py
--rw-r--r--   0        0        0      357 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/reporting.py
--rw-r--r--   0        0        0    10789 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/runner.py
--rw-r--r--   0        0        0     2312 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/ci/stew_runners.py
--rw-r--r--   0        0        0    13078 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/commands.py
--rw-r--r--   0        0        0     2623 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/discovery.py
--rw-r--r--   0        0        0     4303 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/environment.py
--rw-r--r--   0        0        0      559 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/exceptions.py
--rw-r--r--   0        0        0        0 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/metadata/__init__.py
--rw-r--r--   0        0        0     2949 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/metadata/poetry_api.py
--rw-r--r--   0        0        0      367 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/metadata/python_api.py
--rw-r--r--   0        0        0      647 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/metadata/stew_api.py
--rw-r--r--   0        0        0     6744 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/offline_publish.py
--rw-r--r--   0        0        0      700 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/package_resources/mypy.ini
--rw-r--r--   0        0        0        0 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/py.typed
--rw-r--r--   0        0        0     4180 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/pydev.py
--rw-r--r--   0        0        0    13582 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/stew.py
--rw-r--r--   0        0        0      686 2022-06-13 13:44:18.676890 coveo-stew-3.0a4/coveo_stew/utils.py
--rw-r--r--   0        0        0     1178 2022-06-13 13:44:36.573897 coveo-stew-3.0a4/pyproject.toml
--rw-r--r--   0        0        0    15588 2022-06-13 13:44:38.185922 coveo-stew-3.0a4/setup.py
--rw-r--r--   0        0        0    15029 2022-06-13 13:44:38.187201 coveo-stew-3.0a4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/LICENSE
+-rw-r--r--   0        0        0      561 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/LICENSE.md
+-rw-r--r--   0        0        0    14280 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/README.md
+-rw-r--r--   0        0        0        0 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/__init__.py
+-rw-r--r--   0        0        0       99 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/__main__.py
+-rw-r--r--   0        0        0        0 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/__init__.py
+-rw-r--r--   0        0        0     4106 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/any_runner.py
+-rw-r--r--   0        0        0     1573 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/black_runner.py
+-rw-r--r--   0        0        0     5595 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/config.py
+-rw-r--r--   0        0        0     3554 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/mypy_runner.py
+-rw-r--r--   0        0        0      622 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/poetry_runners.py
+-rw-r--r--   0        0        0     1409 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/pytest_runner.py
+-rw-r--r--   0        0        0      357 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/reporting.py
+-rw-r--r--   0        0        0    10813 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/runner.py
+-rw-r--r--   0        0        0     2312 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/ci/stew_runners.py
+-rw-r--r--   0        0        0    13171 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/commands.py
+-rw-r--r--   0        0        0     2623 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/discovery.py
+-rw-r--r--   0        0        0     4303 2022-07-04 19:43:51.865620 coveo-stew-3.0a5/coveo_stew/environment.py
+-rw-r--r--   0        0        0      559 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/exceptions.py
+-rw-r--r--   0        0        0        0 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/metadata/__init__.py
+-rw-r--r--   0        0        0     2949 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/metadata/poetry_api.py
+-rw-r--r--   0        0        0      367 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/metadata/python_api.py
+-rw-r--r--   0        0        0      647 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/metadata/stew_api.py
+-rw-r--r--   0        0        0     6744 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/offline_publish.py
+-rw-r--r--   0        0        0      700 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/package_resources/mypy.ini
+-rw-r--r--   0        0        0        0 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/py.typed
+-rw-r--r--   0        0        0     4180 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/pydev.py
+-rw-r--r--   0        0        0    13472 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/stew.py
+-rw-r--r--   0        0        0      686 2022-07-04 19:43:51.869620 coveo-stew-3.0a5/coveo_stew/utils.py
+-rw-r--r--   0        0        0     1178 2022-07-04 19:44:06.041689 coveo-stew-3.0a5/pyproject.toml
+-rw-r--r--   0        0        0    15694 2022-07-04 19:44:07.163281 coveo-stew-3.0a5/setup.py
+-rw-r--r--   0        0        0    15134 2022-07-04 19:44:07.164300 coveo-stew-3.0a5/PKG-INFO
```

### Comparing `coveo-stew-3.0a4/LICENSE` & `coveo-stew-3.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/LICENSE.md` & `coveo-stew-3.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/README.md` & `coveo-stew-3.0a5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -101,14 +101,15 @@
 - poetry check
 - stew check-outdated
 
 Options:
 
 - `--fix` will reformat the code if `black` fails. Additional fix routines may be added in the future.
 - `--check <runner>` will launch only that runner. This option can be repeated.
+- `--skip <runner>` will skip that runner. Takes precedence over `--check`. This option can be repeated.
 - `--quick` skips running `poetry install --remove-untracked` before running the checks.
 
 The configuration for this feature is explained in more details in the [runners](#runners-stew-ci) section.
 
 ## `stew build`
 
 Store the project and its **locked dependencies** to disk, so it can be installed without contacting a `pypi` server.
```

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/any_runner.py` & `coveo-stew-3.0a5/coveo_stew/ci/any_runner.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/black_runner.py` & `coveo-stew-3.0a5/coveo_stew/ci/black_runner.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/config.py` & `coveo-stew-3.0a5/coveo_stew/ci/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
+from itertools import cycle
 from typing import (
     Any,
     Dict,
     Generator,
     Iterator,
     List,
     Optional,
     Tuple,
     Type,
     TypeVar,
     Union,
 )
 
 from coveo_functools.casing import flexfactory
-from coveo_styles.styles import ExitWithFailure
+from coveo_styles.styles import ExitWithFailure, echo
 
 from coveo_stew.ci.any_runner import AnyRunner
 from coveo_stew.ci.black_runner import BlackRunner
 from coveo_stew.ci.mypy_runner import MypyRunner
 from coveo_stew.ci.poetry_runners import PoetryCheckRunner
 from coveo_stew.ci.pytest_runner import PytestRunner
 from coveo_stew.ci.runner import CIPlan, ContinuousIntegrationRunner, RunnerStatus
@@ -94,39 +95,44 @@
         )
 
     def get_runner(self, runner_name: str) -> Optional[ContinuousIntegrationRunner]:
         """Obtain a runner by name."""
         return self._runners.get(runner_name)
 
     def _generate_ci_plans(
-        self, checks: Optional[List[str]], parallel: bool = True
+        self, checks: Optional[List[str]], skips: Optional[List[str]], parallel: bool = True
     ) -> Generator[CIPlan, None, None]:
         """Generates one test plan per environment."""
         checks = [check.lower() for check in checks] if checks else []
+        skips = [skip.lower() for skip in skips] if skips else []
+
+        emojis = cycle(("see_no_evil", "hear_no_evil", "speak_no_evil"))
 
         for environment in self._pyproject.virtual_environments(create_default_if_missing=True):
             runners = []
             for runner in self.runners:
-                if checks and runner.name.lower() not in checks:
+                if (checks and runner.name.lower() not in checks) or runner.name.lower() in skips:
+                    echo.noise(f"{runner.name} will be skipped.", emoji=next(emojis))
                     continue
                 runners.append(runner)
 
             yield CIPlan(environment, runners, parallel)
 
     async def launch_continuous_integration(
-        self, auto_fix: bool, checks: Optional[List[str]], quick: bool, parallel: bool
+        self,
+        auto_fix: bool,
+        checks: Optional[List[str]],
+        skips: Optional[List[str]],
+        quick: bool,
+        parallel: bool,
     ) -> bool:
         if self.disabled:
             return True
 
-        ci_plans = list(
-            self._generate_ci_plans(
-                checks=[check.lower() for check in checks or []], parallel=parallel
-            )
-        )
+        ci_plans = list(self._generate_ci_plans(checks=checks, skips=skips, parallel=parallel))
         for plan in ci_plans:
             if not quick:
                 self._pyproject.install(environment=plan.environment, remove_untracked=True)
             await plan.orchestrate(auto_fix)
 
         allowed_statuses: Tuple[RunnerStatus, ...] = (
             (RunnerStatus.Success, RunnerStatus.NotRan) if checks else (RunnerStatus.Success,)
```

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/mypy_runner.py` & `coveo-stew-3.0a5/coveo_stew/ci/mypy_runner.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/poetry_runners.py` & `coveo-stew-3.0a5/coveo_stew/ci/poetry_runners.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/pytest_runner.py` & `coveo-stew-3.0a5/coveo_stew/ci/pytest_runner.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/runner.py` & `coveo-stew-3.0a5/coveo_stew/ci/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import asyncio
 from abc import abstractmethod
-from collections.abc import Coroutine
 from dataclasses import dataclass
 from enum import Enum, auto
 from functools import cached_property
 from pathlib import Path
-from typing import Callable, Iterable, List, Optional, Sequence, Tuple
+from typing import Callable, Coroutine, Iterable, List, Optional, Sequence, Tuple
 
 from coveo_styles.styles import ExitWithFailure, echo
 from coveo_systools.subprocess import DetailedCalledProcessError
 from junit_xml import TestCase
 
 from coveo_stew.ci.reporting import generate_report
 from coveo_stew.environment import PythonEnvironment
@@ -223,20 +222,22 @@
 
     async def run_and_report(
         self, auto_fix: bool = False, feedback: bool = True, parallel: bool = True
     ) -> None:
         """Launch the runners and report the results to the user."""
         self.exceptions.clear()
 
-        if auto_fix:
-            parallel = False  # can't run autofix routines in parallel, and crashing is bad UX
+        if auto_fix and parallel:
+            raise AssertionError(
+                "Some dev made a mistake; parallel and autofix are mutually exclusive!"
+            )
 
         if parallel:
             for next_result in asyncio.as_completed(
-                [runner.launch(self.environment, auto_fix=auto_fix) for runner in self.checks]
+                [runner.launch(self.environment, auto_fix=False) for runner in self.checks]
             ):
                 self._report(await next_result, feedback=feedback)
         else:
             for runner in self.checks:
                 self._report(
                     await runner.launch(self.environment, auto_fix=auto_fix), feedback=feedback
                 )
```

### Comparing `coveo-stew-3.0a4/coveo_stew/ci/stew_runners.py` & `coveo-stew-3.0a5/coveo_stew/ci/stew_runners.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/commands.py` & `coveo-stew-3.0a5/coveo_stew/commands.py`

 * *Files 0% similar despite different names*

```diff
@@ -301,39 +301,41 @@
 
 
 @stew.command()
 @click.argument("project_name", default=None, required=False)
 @click.option("--exact-match/--no-exact-match", default=False)
 @click.option("--fix/--no-fix", default=False)
 @click.option("--check", multiple=True, default=None)
+@click.option("--skip", multiple=True, default=None)
 @click.option("--verbose", is_flag=True, default=False)
 @click.option(
     "--quick",
     is_flag=True,
     default=False,
     help="Do not call 'poetry install --remove-untracked' before testing.",
 )
 @click.option("--parallel/--sequential", default=True)
 def ci(
     project_name: str = None,
     exact_match: bool = False,
     fix: bool = False,
     check: List[str] = None,
+    skip: List[str] = None,
     verbose: bool = False,
     quick: bool = False,
     parallel: bool = True,
 ) -> None:
     failures = []
     try:
         for project in discover_pyprojects(
             query=project_name, exact_match=exact_match, verbose=verbose
         ):
             echo.step(project.package.name, pad_after=False)
             if not project.launch_continuous_integration(
-                auto_fix=fix, checks=check, quick=quick, parallel=parallel
+                auto_fix=fix, checks=check, skips=skip, quick=quick, parallel=parallel
             ):
                 failures.append(project)
     except PythonProjectNotFound as exception:
         raise ExitWithFailure from exception
 
     if failures:
         raise ExitWithFailure(failures=failures) from CheckFailed(
```

### Comparing `coveo-stew-3.0a4/coveo_stew/discovery.py` & `coveo-stew-3.0a5/coveo_stew/discovery.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/environment.py` & `coveo-stew-3.0a5/coveo_stew/environment.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/exceptions.py` & `coveo-stew-3.0a5/coveo_stew/exceptions.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/metadata/poetry_api.py` & `coveo-stew-3.0a5/coveo_stew/metadata/poetry_api.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/metadata/stew_api.py` & `coveo-stew-3.0a5/coveo_stew/metadata/stew_api.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/offline_publish.py` & `coveo-stew-3.0a5/coveo_stew/offline_publish.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/package_resources/mypy.ini` & `coveo-stew-3.0a5/coveo_stew/package_resources/mypy.ini`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/pydev.py` & `coveo-stew-3.0a5/coveo_stew/pydev.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/coveo_stew/stew.py` & `coveo-stew-3.0a5/coveo_stew/stew.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,30 +2,35 @@
 
 import asyncio
 import os
 import re
 import shutil
 import sys
 from contextlib import contextmanager
+from functools import cached_property
 from pathlib import Path
 from shutil import rmtree
-from typing import Any, Dict, Generator, Iterator, List, Optional
+from typing import Any, Final, Generator, Iterator, List, Optional, Pattern, Tuple
 
 from coveo_functools.casing import flexfactory
 from coveo_itertools.lookups import dict_lookup
 from coveo_systools.filesystem import CannotFindRepoRoot, find_repo_root
-from coveo_systools.subprocess import DetailedCalledProcessError, check_run
+from coveo_systools.subprocess import check_run
 
 from coveo_stew.environment import PythonEnvironment, PythonTool, find_python_tool
 from coveo_stew.exceptions import NotAPoetryProject, StewException
 from coveo_stew.metadata.poetry_api import PoetryAPI
 from coveo_stew.metadata.python_api import PythonFile
 from coveo_stew.metadata.stew_api import StewPackage
 from coveo_stew.utils import load_toml_from_path
 
+ENVIRONMENT_PATH_PATTERN: Final[Pattern] = re.compile(
+    r"^(?P<path>.+?)(?: (?P<activated>\(Activated\)))?$"
+)
+
 
 class PythonProject:
     """Access the information within a pyproject.toml file and operate on them."""
 
     def __init__(self, project_path: Path, *, verbose: bool = False) -> None:
         self.verbose = verbose
         self.project_path: Path = (
@@ -67,15 +72,29 @@
 
         try:
             repo_root: Optional[Path] = find_repo_root(self.project_path)
         except CannotFindRepoRoot:
             repo_root = None
 
         self.repo_root: Optional[Path] = repo_root
-        self._cached_environments: Optional[Dict[Path, PythonEnvironment]] = None
+
+    @cached_property
+    def _virtual_environments_cache(self) -> List[PythonEnvironment]:
+        cache: List[PythonEnvironment] = []
+
+        for path, activated in self._get_virtual_environment_paths():
+            environment = PythonEnvironment(path)
+            cache.append(environment)
+            environment.activated = activated
+
+        if cache and not any(environment.activated for environment in cache):
+            self.poetry_run("env", "use", cache[0].python_executable)
+            cache[0].activated = True
+
+        return cache
 
     def relative_path(self, path: Path) -> Path:
         """returns the relative path of a path vs the project folder."""
         return path.relative_to(self.project_path)
 
     def lock_is_outdated(self) -> bool:
         """True if the toml file has pending changes that were not applied to poetry.lock"""
@@ -103,75 +122,54 @@
         Note: cached for performance, could theoretically become out-of-sync with reality, either due to a bug,
         or because someone called `poetry env use` while we were working :shrug:
 
         To prevent out of sync:
             - Use the context manager `self._activate_poetry_environment`
             - or use the `environment` argument of `self.poetry_run`
         """
+        if not self._virtual_environments_cache:
+            return None
+
         return next(
-            (environment for environment in self.virtual_environments() if environment.activated),
-            None,
+            environment for environment in self._virtual_environments_cache if environment.activated
         )
 
     def virtual_environments(
         self, *, create_default_if_missing: bool = False
     ) -> Iterator[PythonEnvironment]:
         """The project's virtual environments. These are cached for performance.
 
         create_default_if_missing: When no environments are found, install the environment using what poetry
             would use by default.
         """
-        reevaluate = self._cached_environments is None or all(
-            (
-                # we already have a cache
-                self._cached_environments is not None,
-                # but it's empty
-                not self._cached_environments,
-                # and we are supposed to create one
-                create_default_if_missing,
-            )
-        )
+        if not self._virtual_environments_cache and create_default_if_missing:
+            self._create_default_poetry_install()
 
-        if reevaluate:
-            self._refresh_virtual_environment_cache()
-            if not self._cached_environments and create_default_if_missing:
-                self.install()
-                self._refresh_virtual_environment_cache()
-
-        yield from self._cached_environments.values()
-
-    def _refresh_virtual_environment_cache(self) -> None:
-        if self._cached_environments is None:
-            self._cached_environments = {}
-
-        for path in self._get_virtual_environment_paths():
-            if path not in self._cached_environments:
-                self._cached_environments[path] = PythonEnvironment(path)
+        yield from self._virtual_environments_cache
 
-        # reprocess all environments to set the activated_environment one correctly
-        try:
-            activated_environment: Optional[PythonEnvironment] = PythonEnvironment(
-                self.poetry_run("env", "info", "--path", capture_output=True, breakout_of_venv=True)
-            )
-        except DetailedCalledProcessError as exception:
-            if exception.returncode != 1:
-                raise
-            activated_environment = None
-
-        for environment in self._cached_environments.values():
-            environment.activated = (
-                (environment == activated_environment) if activated_environment else False
-            )
+    def _create_default_poetry_install(self) -> PythonEnvironment:
+        """To be used only when no environments exist. Creates a default one by calling "poetry install"."""
+        self.poetry_run("install")
+        del self._virtual_environments_cache  # force cache refresh
+        activated_environment = self.activated_environment()
+        activated_environment.installed = True
+        activated_environment.cleaned = True
+        return activated_environment
 
-    def _get_virtual_environment_paths(self) -> Iterator[Path]:
+    def _get_virtual_environment_paths(self) -> Iterator[Tuple[Path, bool]]:
+        """Returns tuples of (path, activated)"""
         for str_path in self.poetry_run(
             "env", "list", "--full-path", capture_output=True, breakout_of_venv=True
         ).split("\n"):
-            if str_path.strip():
-                yield Path(str_path.replace("(Activated)", "").strip())
+            if (stripped := str_path.strip()) and (
+                match := re.fullmatch(ENVIRONMENT_PATH_PATTERN, stripped)
+            ):
+                yield Path(match.groupdict()["path"].strip()), bool(
+                    match.groupdict().get("activated")
+                )
 
     def current_environment_belongs_to_project(self) -> bool:
         """True if we're running from one of the project's virtual envs.
         Typically False; serves the rare cases where stew is installed inside the environment.
         """
         current_executable = Path(sys.executable)
         return any(
@@ -226,53 +224,55 @@
         """Generates the content of a `requirements.txt` file based on the lock."""
         return self.poetry_run("export", capture_output=True)
 
     def launch_continuous_integration(
         self,
         auto_fix: bool = False,
         checks: Optional[List[str]] = None,
+        skips: Optional[List[str]] = None,
         quick: bool = False,
         parallel: bool = True,
     ) -> bool:
         """Launch all continuous integration runners on the project."""
         return asyncio.run(
             self.ci.launch_continuous_integration(
-                auto_fix=auto_fix, checks=checks, quick=quick, parallel=parallel
+                auto_fix=auto_fix, checks=checks, skips=skips, quick=quick, parallel=parallel
             )
         )
 
     def install(
         self,
         *,
         environment: PythonEnvironment = None,
         remove_untracked: bool = False,
         quiet: bool = False,
     ) -> None:
         """
         Performs a 'poetry install --remove-untracked' on the project. If an environment is provided, target it.
         """
         target_environment = environment or self.activated_environment()
-        if target_environment and target_environment.installed:
+        if not target_environment:
+            self._create_default_poetry_install()
+            return
+
+        if target_environment.installed:
             # this environment was already installed
             if not (remove_untracked and not target_environment.cleaned):
                 # return unless we are cleaning a non-cleaned environment
                 return
 
         command = ["install"]
         if remove_untracked:
             command.append("--remove-untracked")
         if quiet and not self.verbose:
             command.append("--quiet")
 
         self.poetry_run(*command, environment=target_environment)
-
-        self._refresh_virtual_environment_cache()
-        affected_environment = target_environment or self.activated_environment()
-        affected_environment.installed = True
-        affected_environment.cleaned |= remove_untracked
+        target_environment.installed = True
+        target_environment.cleaned |= remove_untracked
 
     def remove_egg_info(self) -> bool:
         """Removes the egg-info (editable project hook) from the folder. Returns True if we removed it."""
         if self.egg_path.exists():
             rmtree(str(self.egg_path))
             return True
         return False
```

### Comparing `coveo-stew-3.0a4/coveo_stew/utils.py` & `coveo-stew-3.0a5/coveo_stew/utils.py`

 * *Files identical despite different names*

### Comparing `coveo-stew-3.0a4/pyproject.toml` & `coveo-stew-3.0a5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "coveo-stew"
-version = "3.0a4"
+version = "3.0a5"
 description = "Opinionated python packaging and development utilities"
 license = "Apache-2.0"
 readme = "README.md"
 repository = "https://github.com/coveo/stew"
 authors = ["Jonathan Piché <tools@coveo.com>"]
 
 packages = [
@@ -21,15 +21,15 @@
 coveo-styles = "^2.0.0"
 junit-xml = "*"
 toml = "*"
 tomlkit = "*"
 
 
 [tool.poetry.dev-dependencies]
-black = "22.3"
+black = "22.6"
 coveo-testing = "^2.0.0"
 flake8 = "*"
 isort = "*"
 mypy = "0.950"  # required for 3.10 support
 pytest = "*"
 types-setuptools = "*"
 types-toml = "*"
```

### Comparing `coveo-stew-3.0a4/setup.py` & `coveo-stew-3.0a5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,17 +18,17 @@
  'tomlkit']
 
 entry_points = \
 {'console_scripts': ['stew = coveo_stew.commands:stew']}
 
 setup_kwargs = {
     'name': 'coveo-stew',
-    'version': '3.0a4',
+    'version': '3.0a5',
     'description': 'Opinionated python packaging and development utilities',
-    'long_description': '# coveo-stew\n\ncoveo-stew delivers a complete Continuous Integration (CI) and Continuous Delivery (CD) solution\nusing [poetry](https://python-poetry.org) as its backend.\n\n\n# Features\n\n## CI tools\n- Config-free pytest, mypy and black runners\n- Add your own linters and tools\n- JUnit report generation\n- GitHub Action that runs all your CI tools\n\nSimilar to: tox\n\n## CD tools\n- GitHub Action for Continuous Delivery (CD) (publish to pypi)\n- Automated "patch" version bumps (requires a `pypi` server)\n- Can download locked dependencies into a folder, for offline distribution\n\nSimilar to: poetry, flit, pbr, setuptools\n\n## Multiple projects\n- Support for several isolated poetry projects in one GitHub repository\n- Support for local path references\n- A "one ring to rule them all" virtual environment that includes all subprojects within the repository\n- Batch operations\n- Note: Single projects are also supported! 😅\n\nSimilar to: nothing! it\'s unique! 😎 \n\n\n# Prerequisites\n\n*Changed in 3.0*: `poetry` is no longer provided out-of-the-box.\n\nYou need [poetry](https://python-poetry.org/) installed on your system, and it must be available through the `PATH`.\n\nThe `3.0` version of `coveo-stew` is designed to work with `poetry >= 1.1.13`.\n\nWhile it is compatible with older versions, old poetry issues \nsuch as [this](https://github.com/python-poetry/poetry/issues/3189) \nand [this](https://github.com/python-poetry/poetry/issues/3254) \nwill cause `stew` to misbehave.\n\nIf you need to work with an older version of poetry, \nconsider using `coveo-stew < 3.0` which had workarounds implemented around these issues.\n\n\n# Installation\n\nJust like poetry, `stew` is a CLI tool that you install in your system.\n\nIt is recommended to install using [pipx](https://github.com/pipxproject/pipx) in order to isolate this into a nice little space:\n\n```\npip install pipx --user\npipx install coveo-stew\n```\n\nIf you don\'t use pipx, make sure to isolate the installation into a virtual environment.\n\n\n# Repository Structure\n\nPlease read these guides in order to learn how to organize your repository for maximum compatibility:\n\n- [For a single library](README_SINGLE_LIBRARY.md)\n- [For multiple libraries](README_MULTIPLE_LIBRARIES.md)\n\n\n# Commands\n\n## General command usage\n\nUnless a project name is specified, most commands will operate on all projects in a git repository based on the current working folder:\n\n- `stew <command>`\n    - Perform a command on all projects\n- `stew <command> --help`\n    - Obtain help about a particular command\n- `stew <command> <project-name>`\n    - Perform the command on all projects with `<project-name>` in their name (partial match)\n- `stew <command> <project-name> --exact-match`\n    - Disable partial project name matching\n\nThe main commands are explained below.\n\n\n## `stew ci`\n\nThe main show; it runs all CI tools on one or multiple projects.\n\nErrors will show in the console, and junit xml reports will be generated inside the `.ci` folder.\n\nWithout configuration, this command will run the following checks:\n\n- mypy (using opinionated, strict rules)\n  - Note: `mypy` is not provided with `coveo-stew`. See [builtin-runners](#builtin-runners) for info.\n- poetry check\n- stew check-outdated\n\nOptions:\n\n- `--fix` will reformat the code if `black` fails. Additional fix routines may be added in the future.\n- `--check <runner>` will launch only that runner. This option can be repeated.\n- `--quick` skips running `poetry install --remove-untracked` before running the checks.\n\nThe configuration for this feature is explained in more details in the [runners](#runners-stew-ci) section.\n\n## `stew build`\n\nStore the project and its **locked dependencies** to disk, so it can be installed without contacting a `pypi` server.\n\nOptimally used to create truly repeatable builds and workflows (e.g.: containerized images, cloud storage, etc).\n\nThe folder can later be installed offline with `pip install --no-index --find-links <folder> <project-name>`.\n\n\nOptions:\n\n- `--directory` specifies where the wheels should be downloaded.\n- `--python` may be used to target a different python. It\'s important to use the same python version, architecture and OS than the target system.\n\n**Make sure your target `<folder>` is clean**: Keep in mind that `pip` will still use the `pyproject.toml` constraints when installing, not `poetry.lock`. \nThe locked version system works when the locked version is the only thing that `pip` can find in the `<folder>`.\n\n\n## `stew check-outdated` and `stew fix-outdated` \n\nChecks for out-of-date files or automatically update them.\n\nSummary of actions:\n- `poetry lock` if `pyproject.toml` changed but not the `poetry.lock`\n- `stew pull-dev-requirements` if a pydev project\'s dev-requirements are out of sync\n\n\n## `stew bump`\n\nCalls `poetry lock` on all projects.\n\n\n## `stew refresh`\n\nCalls `poetry install` on all projects.\n\n\n## `stew fresh-eggs`\n\nClears the `.egg-info` folder from your projects. Usually followed by a `poetry install` or a `stew refresh`.\n\nUse this if you change a `[tool.poetry.scripts]` section, else the changes will not be honored.\n\n\n## `stew locate <project>`\n\nReturns the path to a project:\n\n```\n$ stew locate coveo-stew\n/home/jonapich/code/stew/coveo-stew\n```\n\n# Configuration\n\nConfiguration is done through each `pyproject.toml` file; default values are shown:\n\n```\n[tool.stew.ci]\nmypy = true\npytest = false\nblack = false\npoetry-check = true\ncheck-outdated = true\noffline-build = false\n```\n\nYou don\'t have to include the `[tool.stew.ci]` section at all if these defaults suit you!\n\n\n# Runners (stew ci)\n\n*Changed in coveo-stew 3.0*: mypy and black are no longer provided out-of-the-box.\n\nIn order to use a builtin or custom runner, you must have it installed. These locations are supported:\n\n- Recommended: The runner is in the project\'s virtual environment (most likely as a dev dependency in `pyproject.toml`)\n- Alternative: The runner is installed in your system and available through the PATH\n\nWe strongly suggest pinning them to your\n`pyproject.toml` file in the `[tool.poetry.dev-dependencies]` section.\n\nThis way, mypy won\'t surprise you with new failures when they release new versions! 😎\n\nNote: You can override and customize most runners by [rewriting them as custom runners.](#custom-runners)\n\n\n## Builtin Runners\n\n### mypy\n\nA strict mypy configuration is provided. \n\nYou can provide your own mypy configuration, but you\'ll have to specify the `set-config` option: \n\n```\n[tool.stew.ci]\n\n# disable stew\'s strict mypy config (i.e.: let mypy find its config)\nmypy = { set-config = False } \n\n# use a specific config (path relative to `pyproject.toml`\'s folder)\nmypy = { set-config = "mypy.ini" }\n```\n\nSee https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml\n\n### pytest\n\nPytest is configured to run with `--doctest-modules --tb=short --durations=5` as well as JUnit report generation.\n\nSome additional options are available:\n\n```\n[tool.stew.ci]\n\n# configure the markers to test (i.e.: `-m`)\npytest = { marker-expression = \'not docker_tests\' }\n\n# disable the doctests\npytest = { doctest-modules = False }\n```\n\n\n### black\n\nBlack supports the `pyproject.toml` file natively:\n\n```\n[tool.black]\nline-length = 100\n```\n\nRef: [black documentation](https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file)\n\n\n### poetry-check\n\nRuns `poetry check` on each project.\n\n\n### check-outdated\n\nRuns `stew check-outdated`.\n\nNote: This runner cannot be overridden, but it can be disabled.\n\n\n### offline-build\n\nRuns `stew build` to a temporary folder and ensures that pip is able to reinstall everything from there.\n\nNote: This runner cannot be overridden, but it can be disabled.\n\n\n## Custom Runners\n\nYou can add your own runners to `stew ci`. \nYou can also redefine a builtin runner completely.\n\nIn this example, we create runners for flake8, bandit and isort. We also redefine the pytest runner:\n\n\n```\n[tool.stew.ci.custom-runners]\nflake8 = true\nbandit = { check-args = ["--quiet", "--recursive", "."] }\n\n# some may prefer this toml syntax:\n[tool.stew.ci.custom-runners.isort]\ncheck-args = ["--check", ".", "--profile black"]\nautofix-args = [".", "--profile black"]\n\n[tool.stew.ci.custom-runners.pytest] \ncheck-args = ["--tb=long", "--junitxml=.ci/pytest-results.xml"]\n```\n\nWhen a builtin runner such as pytest is redefined as a custom runner, you must provide all the arguments.\nIn this case, not passing `--junitxml` would mean that we lose the report that used to be in the `.ci/` directory. \n\n\n### Options\n\nThe following options are supported for custom runners:\n\n- name: You can specify the module name if it differs from the name of the tool.\n  - Important: Runners are called through `python -m <name>`, not through the shell! \n- check-args: The arguments to invoke the check.\n- autofix-args: The arguments to invoke the autofix. Provide the empty string "" in order to run without arguments.\n- check-failed-exit-codes: A list of ints denoting the exit codes to consider "failed" (anything else will be "error"). 0 is always a success. default is `[1]`.\n- create-generic-report: Whether to create a generic pass/fail JUnit report for this check.\n- working-directory: The default is "project" which corresponds to the project\'s `pyproject.toml` file. You can change it to "repository" in order to run from the root.\n\nThe `args` and `check-args` can be:\n\n- A string\n  - Such as a single argument "--check"\n  - Such as a path "."\n  - Such as an option "--profile black"\n  - But NOT as a combo of the above: "--check . --profile black" will most likely not work.\n\n- A list of string:\n  - Any combination of the "string" rules explained above.\n\n\n# FAQ, Tips and Tricks\n\n## constraints vs locks - where do they apply?\n\nWhen you call `poetry install`, you end up installing packages based on the `poetry.lock` file.\nThe resulting packages will always be the same, no matter what.\nThis is the dev scenario.\n\nWhen you call `pip install`, you are installing packages based on the constraints placed in a `pyproject.toml` or a `setup.py` file.\nUnless the constraints are hard pinned versions, the resulting packages are not guaranteed and will depend on the point in time when the installation is performed, among other factors.\nThis is the shared library scenario.\n\nWhen you use poetry, you cover the two scenarios above.\n\nThe third scenario is the private business use case: you want to freeze your dependencies in time so that everything from the developer to the CI servers to the production system is identical.\nEssentially, you want `poetry install` without the dev requirements.\n\nThis functionality is provided out of the box by `stew build`, which creates a pip-installable package from the lock file that you can then stash in a private storage of your choice or pass around your deployments.\n\n\n## How to provision a business production system / how to freeze your project for "offline" distribution\n\nYou can keep `poetry` and `stew` off your production environment by creating a frozen archive of your application or library from your CI servers (docker used as example):\n\n- Use the `stew build` tool which:\n    - performs a `poetry build` on your project\n    - calls `pip download` based on the content of the lock file\n    - Moves the artifacts to the `.wheels` folder of your repo\n- Recommended: Use the `--python` switch when calling `stew build` to specify which python executable to use! Make sure to use a python interpreter that matches the os/arch/bits of the system you want to provision.\n\nThe content in `.wheels` can then be zipped and moved around. A typical scenario is to push it into a Docker Container:\n\n- Include the `.wheels` folder into your Docker build context\n- In your Dockerfile:\n    - ADD the `.wheels` folder\n    - Manage the `pip` version! Either update it to latest, or pin it to something.\n    - Prepare a python environment\n        - Use `python -m venv <location>` to create a virtual environment natively.\n        - Note the executable location... typically (`location/bin/python` or `location/Scripts/python.exe`)\n    - Install your application into the python environment you just created:\n        - Use `<venv-python-executable> -m pip install <your-package> --no-index --find-links <wheels-folder-location>`\n    - You may delete the `.wheels` folder if you want. Consider keeping a copy of the lock file within the docker image, for reference.\n\nTo make sure you use the python interpreter that matches the os/arch/bits of the system you want to provision, you can run `stew build` directly when building the container image.\nIn order to do so without packaging `stew` in production, you can use [multi-stage builds](https://docs.docker.com/develop/develop-images/multistage-build/).\n\n## How to hook your IDE with the virtual environment\n\nIf your IDE supports poetry, it should detect and use the `pyproject.toml` file.\n\nTo set it up manually:\n\n1. Call `poetry install` from the location of the `pyproject.toml` file\n1. Obtain the location of the virtual environment (i.e.: `poetry env list --full-path`)\n1. Configure your IDE to use the python interpreter from that location\n\nYour IDE should proceed to analyze the environment and will pick up all imports automatically, \nregardless of your PYTHONPATH or your working directory.\nSince the local source is editable, any change to the source code will be reflected on the next interpreter run.\n\nIf you use the multiple-projects approach, you should hook your IDE to the `pydev` environment. See [this documentation](./README_MULTIPLE_LIBRARIES.md) for more information.\n\n\n## Using the virtual environment without activating it\n\nUsing the correct interpreter is all you need to do. \nThere is no activation script or environment variables to set up: the interpreter executable inside the virtual environment folder is a fully bootstrapped and isolated environment.\n\n- A python dockerfile may call `<venv-python-exec>` directly in the dockerfile\'s CMD\n- A service that spawns other processes should receive the path to the `<venv-python-exec>`\n\n[Use the `-m` switch](https://docs.python.org/3/using/cmdline.html#cmdoption-m) in order to launch your app!\n',
+    'long_description': '# coveo-stew\n\ncoveo-stew delivers a complete Continuous Integration (CI) and Continuous Delivery (CD) solution\nusing [poetry](https://python-poetry.org) as its backend.\n\n\n# Features\n\n## CI tools\n- Config-free pytest, mypy and black runners\n- Add your own linters and tools\n- JUnit report generation\n- GitHub Action that runs all your CI tools\n\nSimilar to: tox\n\n## CD tools\n- GitHub Action for Continuous Delivery (CD) (publish to pypi)\n- Automated "patch" version bumps (requires a `pypi` server)\n- Can download locked dependencies into a folder, for offline distribution\n\nSimilar to: poetry, flit, pbr, setuptools\n\n## Multiple projects\n- Support for several isolated poetry projects in one GitHub repository\n- Support for local path references\n- A "one ring to rule them all" virtual environment that includes all subprojects within the repository\n- Batch operations\n- Note: Single projects are also supported! 😅\n\nSimilar to: nothing! it\'s unique! 😎 \n\n\n# Prerequisites\n\n*Changed in 3.0*: `poetry` is no longer provided out-of-the-box.\n\nYou need [poetry](https://python-poetry.org/) installed on your system, and it must be available through the `PATH`.\n\nThe `3.0` version of `coveo-stew` is designed to work with `poetry >= 1.1.13`.\n\nWhile it is compatible with older versions, old poetry issues \nsuch as [this](https://github.com/python-poetry/poetry/issues/3189) \nand [this](https://github.com/python-poetry/poetry/issues/3254) \nwill cause `stew` to misbehave.\n\nIf you need to work with an older version of poetry, \nconsider using `coveo-stew < 3.0` which had workarounds implemented around these issues.\n\n\n# Installation\n\nJust like poetry, `stew` is a CLI tool that you install in your system.\n\nIt is recommended to install using [pipx](https://github.com/pipxproject/pipx) in order to isolate this into a nice little space:\n\n```\npip install pipx --user\npipx install coveo-stew\n```\n\nIf you don\'t use pipx, make sure to isolate the installation into a virtual environment.\n\n\n# Repository Structure\n\nPlease read these guides in order to learn how to organize your repository for maximum compatibility:\n\n- [For a single library](README_SINGLE_LIBRARY.md)\n- [For multiple libraries](README_MULTIPLE_LIBRARIES.md)\n\n\n# Commands\n\n## General command usage\n\nUnless a project name is specified, most commands will operate on all projects in a git repository based on the current working folder:\n\n- `stew <command>`\n    - Perform a command on all projects\n- `stew <command> --help`\n    - Obtain help about a particular command\n- `stew <command> <project-name>`\n    - Perform the command on all projects with `<project-name>` in their name (partial match)\n- `stew <command> <project-name> --exact-match`\n    - Disable partial project name matching\n\nThe main commands are explained below.\n\n\n## `stew ci`\n\nThe main show; it runs all CI tools on one or multiple projects.\n\nErrors will show in the console, and junit xml reports will be generated inside the `.ci` folder.\n\nWithout configuration, this command will run the following checks:\n\n- mypy (using opinionated, strict rules)\n  - Note: `mypy` is not provided with `coveo-stew`. See [builtin-runners](#builtin-runners) for info.\n- poetry check\n- stew check-outdated\n\nOptions:\n\n- `--fix` will reformat the code if `black` fails. Additional fix routines may be added in the future.\n- `--check <runner>` will launch only that runner. This option can be repeated.\n- `--skip <runner>` will skip that runner. Takes precedence over `--check`. This option can be repeated.\n- `--quick` skips running `poetry install --remove-untracked` before running the checks.\n\nThe configuration for this feature is explained in more details in the [runners](#runners-stew-ci) section.\n\n## `stew build`\n\nStore the project and its **locked dependencies** to disk, so it can be installed without contacting a `pypi` server.\n\nOptimally used to create truly repeatable builds and workflows (e.g.: containerized images, cloud storage, etc).\n\nThe folder can later be installed offline with `pip install --no-index --find-links <folder> <project-name>`.\n\n\nOptions:\n\n- `--directory` specifies where the wheels should be downloaded.\n- `--python` may be used to target a different python. It\'s important to use the same python version, architecture and OS than the target system.\n\n**Make sure your target `<folder>` is clean**: Keep in mind that `pip` will still use the `pyproject.toml` constraints when installing, not `poetry.lock`. \nThe locked version system works when the locked version is the only thing that `pip` can find in the `<folder>`.\n\n\n## `stew check-outdated` and `stew fix-outdated` \n\nChecks for out-of-date files or automatically update them.\n\nSummary of actions:\n- `poetry lock` if `pyproject.toml` changed but not the `poetry.lock`\n- `stew pull-dev-requirements` if a pydev project\'s dev-requirements are out of sync\n\n\n## `stew bump`\n\nCalls `poetry lock` on all projects.\n\n\n## `stew refresh`\n\nCalls `poetry install` on all projects.\n\n\n## `stew fresh-eggs`\n\nClears the `.egg-info` folder from your projects. Usually followed by a `poetry install` or a `stew refresh`.\n\nUse this if you change a `[tool.poetry.scripts]` section, else the changes will not be honored.\n\n\n## `stew locate <project>`\n\nReturns the path to a project:\n\n```\n$ stew locate coveo-stew\n/home/jonapich/code/stew/coveo-stew\n```\n\n# Configuration\n\nConfiguration is done through each `pyproject.toml` file; default values are shown:\n\n```\n[tool.stew.ci]\nmypy = true\npytest = false\nblack = false\npoetry-check = true\ncheck-outdated = true\noffline-build = false\n```\n\nYou don\'t have to include the `[tool.stew.ci]` section at all if these defaults suit you!\n\n\n# Runners (stew ci)\n\n*Changed in coveo-stew 3.0*: mypy and black are no longer provided out-of-the-box.\n\nIn order to use a builtin or custom runner, you must have it installed. These locations are supported:\n\n- Recommended: The runner is in the project\'s virtual environment (most likely as a dev dependency in `pyproject.toml`)\n- Alternative: The runner is installed in your system and available through the PATH\n\nWe strongly suggest pinning them to your\n`pyproject.toml` file in the `[tool.poetry.dev-dependencies]` section.\n\nThis way, mypy won\'t surprise you with new failures when they release new versions! 😎\n\nNote: You can override and customize most runners by [rewriting them as custom runners.](#custom-runners)\n\n\n## Builtin Runners\n\n### mypy\n\nA strict mypy configuration is provided. \n\nYou can provide your own mypy configuration, but you\'ll have to specify the `set-config` option: \n\n```\n[tool.stew.ci]\n\n# disable stew\'s strict mypy config (i.e.: let mypy find its config)\nmypy = { set-config = False } \n\n# use a specific config (path relative to `pyproject.toml`\'s folder)\nmypy = { set-config = "mypy.ini" }\n```\n\nSee https://mypy.readthedocs.io/en/stable/config_file.html#using-a-pyproject-toml\n\n### pytest\n\nPytest is configured to run with `--doctest-modules --tb=short --durations=5` as well as JUnit report generation.\n\nSome additional options are available:\n\n```\n[tool.stew.ci]\n\n# configure the markers to test (i.e.: `-m`)\npytest = { marker-expression = \'not docker_tests\' }\n\n# disable the doctests\npytest = { doctest-modules = False }\n```\n\n\n### black\n\nBlack supports the `pyproject.toml` file natively:\n\n```\n[tool.black]\nline-length = 100\n```\n\nRef: [black documentation](https://black.readthedocs.io/en/stable/usage_and_configuration/the_basics.html#configuration-via-a-file)\n\n\n### poetry-check\n\nRuns `poetry check` on each project.\n\n\n### check-outdated\n\nRuns `stew check-outdated`.\n\nNote: This runner cannot be overridden, but it can be disabled.\n\n\n### offline-build\n\nRuns `stew build` to a temporary folder and ensures that pip is able to reinstall everything from there.\n\nNote: This runner cannot be overridden, but it can be disabled.\n\n\n## Custom Runners\n\nYou can add your own runners to `stew ci`. \nYou can also redefine a builtin runner completely.\n\nIn this example, we create runners for flake8, bandit and isort. We also redefine the pytest runner:\n\n\n```\n[tool.stew.ci.custom-runners]\nflake8 = true\nbandit = { check-args = ["--quiet", "--recursive", "."] }\n\n# some may prefer this toml syntax:\n[tool.stew.ci.custom-runners.isort]\ncheck-args = ["--check", ".", "--profile black"]\nautofix-args = [".", "--profile black"]\n\n[tool.stew.ci.custom-runners.pytest] \ncheck-args = ["--tb=long", "--junitxml=.ci/pytest-results.xml"]\n```\n\nWhen a builtin runner such as pytest is redefined as a custom runner, you must provide all the arguments.\nIn this case, not passing `--junitxml` would mean that we lose the report that used to be in the `.ci/` directory. \n\n\n### Options\n\nThe following options are supported for custom runners:\n\n- name: You can specify the module name if it differs from the name of the tool.\n  - Important: Runners are called through `python -m <name>`, not through the shell! \n- check-args: The arguments to invoke the check.\n- autofix-args: The arguments to invoke the autofix. Provide the empty string "" in order to run without arguments.\n- check-failed-exit-codes: A list of ints denoting the exit codes to consider "failed" (anything else will be "error"). 0 is always a success. default is `[1]`.\n- create-generic-report: Whether to create a generic pass/fail JUnit report for this check.\n- working-directory: The default is "project" which corresponds to the project\'s `pyproject.toml` file. You can change it to "repository" in order to run from the root.\n\nThe `args` and `check-args` can be:\n\n- A string\n  - Such as a single argument "--check"\n  - Such as a path "."\n  - Such as an option "--profile black"\n  - But NOT as a combo of the above: "--check . --profile black" will most likely not work.\n\n- A list of string:\n  - Any combination of the "string" rules explained above.\n\n\n# FAQ, Tips and Tricks\n\n## constraints vs locks - where do they apply?\n\nWhen you call `poetry install`, you end up installing packages based on the `poetry.lock` file.\nThe resulting packages will always be the same, no matter what.\nThis is the dev scenario.\n\nWhen you call `pip install`, you are installing packages based on the constraints placed in a `pyproject.toml` or a `setup.py` file.\nUnless the constraints are hard pinned versions, the resulting packages are not guaranteed and will depend on the point in time when the installation is performed, among other factors.\nThis is the shared library scenario.\n\nWhen you use poetry, you cover the two scenarios above.\n\nThe third scenario is the private business use case: you want to freeze your dependencies in time so that everything from the developer to the CI servers to the production system is identical.\nEssentially, you want `poetry install` without the dev requirements.\n\nThis functionality is provided out of the box by `stew build`, which creates a pip-installable package from the lock file that you can then stash in a private storage of your choice or pass around your deployments.\n\n\n## How to provision a business production system / how to freeze your project for "offline" distribution\n\nYou can keep `poetry` and `stew` off your production environment by creating a frozen archive of your application or library from your CI servers (docker used as example):\n\n- Use the `stew build` tool which:\n    - performs a `poetry build` on your project\n    - calls `pip download` based on the content of the lock file\n    - Moves the artifacts to the `.wheels` folder of your repo\n- Recommended: Use the `--python` switch when calling `stew build` to specify which python executable to use! Make sure to use a python interpreter that matches the os/arch/bits of the system you want to provision.\n\nThe content in `.wheels` can then be zipped and moved around. A typical scenario is to push it into a Docker Container:\n\n- Include the `.wheels` folder into your Docker build context\n- In your Dockerfile:\n    - ADD the `.wheels` folder\n    - Manage the `pip` version! Either update it to latest, or pin it to something.\n    - Prepare a python environment\n        - Use `python -m venv <location>` to create a virtual environment natively.\n        - Note the executable location... typically (`location/bin/python` or `location/Scripts/python.exe`)\n    - Install your application into the python environment you just created:\n        - Use `<venv-python-executable> -m pip install <your-package> --no-index --find-links <wheels-folder-location>`\n    - You may delete the `.wheels` folder if you want. Consider keeping a copy of the lock file within the docker image, for reference.\n\nTo make sure you use the python interpreter that matches the os/arch/bits of the system you want to provision, you can run `stew build` directly when building the container image.\nIn order to do so without packaging `stew` in production, you can use [multi-stage builds](https://docs.docker.com/develop/develop-images/multistage-build/).\n\n## How to hook your IDE with the virtual environment\n\nIf your IDE supports poetry, it should detect and use the `pyproject.toml` file.\n\nTo set it up manually:\n\n1. Call `poetry install` from the location of the `pyproject.toml` file\n1. Obtain the location of the virtual environment (i.e.: `poetry env list --full-path`)\n1. Configure your IDE to use the python interpreter from that location\n\nYour IDE should proceed to analyze the environment and will pick up all imports automatically, \nregardless of your PYTHONPATH or your working directory.\nSince the local source is editable, any change to the source code will be reflected on the next interpreter run.\n\nIf you use the multiple-projects approach, you should hook your IDE to the `pydev` environment. See [this documentation](./README_MULTIPLE_LIBRARIES.md) for more information.\n\n\n## Using the virtual environment without activating it\n\nUsing the correct interpreter is all you need to do. \nThere is no activation script or environment variables to set up: the interpreter executable inside the virtual environment folder is a fully bootstrapped and isolated environment.\n\n- A python dockerfile may call `<venv-python-exec>` directly in the dockerfile\'s CMD\n- A service that spawns other processes should receive the path to the `<venv-python-exec>`\n\n[Use the `-m` switch](https://docs.python.org/3/using/cmdline.html#cmdoption-m) in order to launch your app!\n',
     'author': 'Jonathan Piché',
     'author_email': 'tools@coveo.com',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/coveo/stew',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `coveo-stew-3.0a4/PKG-INFO` & `coveo-stew-3.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coveo-stew
-Version: 3.0a4
+Version: 3.0a5
 Summary: Opinionated python packaging and development utilities
 Home-page: https://github.com/coveo/stew
 License: Apache-2.0
 Author: Jonathan Piché
 Author-email: tools@coveo.com
 Requires-Python: >3.8.0,<4
 Classifier: License :: OSI Approved :: Apache Software License
@@ -125,14 +125,15 @@
 - poetry check
 - stew check-outdated
 
 Options:
 
 - `--fix` will reformat the code if `black` fails. Additional fix routines may be added in the future.
 - `--check <runner>` will launch only that runner. This option can be repeated.
+- `--skip <runner>` will skip that runner. Takes precedence over `--check`. This option can be repeated.
 - `--quick` skips running `poetry install --remove-untracked` before running the checks.
 
 The configuration for this feature is explained in more details in the [runners](#runners-stew-ci) section.
 
 ## `stew build`
 
 Store the project and its **locked dependencies** to disk, so it can be installed without contacting a `pypi` server.
```

