# Comparing `tmp/myke-0.0.1a9.tar.gz` & `tmp/myke-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "myke-0.0.1a9.tar", last modified: Wed Dec  7 09:03:14 2022, max compression
+gzip compressed data, was "myke-0.1.0.tar", last modified: Wed Jun  7 23:03:58 2023, max compression
```

## Comparing `myke-0.0.1a9.tar` & `myke-0.1.0.tar`

### file list

```diff
@@ -1,33 +1,53 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/
--rw-r--r--   0 root         (0) root         (0)     1080 2022-12-07 08:59:42.000000 myke-0.0.1a9/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2022-12-07 08:59:42.000000 myke-0.0.1a9/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1324 2022-12-07 09:03:14.264223 myke-0.0.1a9/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      598 2022-12-07 08:59:42.000000 myke-0.0.1a9/README.md
--rw-r--r--   0 root         (0) root         (0)        8 2022-12-07 08:59:42.000000 myke-0.0.1a9/VERSION
--rw-r--r--   0 root         (0) root         (0)     2762 2022-12-07 09:03:14.264223 myke-0.0.1a9/setup.cfg
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-07 08:59:42.000000 myke-0.0.1a9/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.260223 myke-0.0.1a9/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/src/myke/
--rw-r--r--   0 root         (0) root         (0)      818 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/__init__.py
--rw-r--r--   0 root         (0) root         (0)       62 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/__main__.py
--rw-r--r--   0 root         (0) root         (0)       24 2022-12-07 09:03:07.000000 myke-0.0.1a9/src/myke/__version__.py
--rw-r--r--   0 root         (0) root         (0)      859 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/exceptions.py
--rw-r--r--   0 root         (0) root         (0)      206 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/globals.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/src/myke/io/
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2738 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/echo.py
--rw-r--r--   0 root         (0) root         (0)     4150 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/read.py
--rw-r--r--   0 root         (0) root         (0)     2953 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/io/write.py
--rw-r--r--   0 root         (0) root         (0)     5159 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/main.py
--rw-r--r--   0 root         (0) root         (0)        0 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/py.typed
--rw-r--r--   0 root         (0) root         (0)     2126 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/sh.py
--rw-r--r--   0 root         (0) root         (0)     6766 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/tasks.py
--rw-r--r--   0 root         (0) root         (0)      235 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/types.py
--rw-r--r--   0 root         (0) root         (0)     2120 2022-12-07 08:59:42.000000 myke-0.0.1a9/src/myke/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-07 09:03:14.264223 myke-0.0.1a9/src/myke.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1324 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      548 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       44 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      613 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2022-12-07 09:03:14.000000 myke-0.0.1a9/src/myke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.480466 myke-0.1.0/
+-rw-r--r--   0 root         (0) root         (0)    34487 2023-06-07 22:54:25.000000 myke-0.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    44520 2023-06-07 23:03:58.480466 myke-0.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-06-07 22:54:25.000000 myke-0.1.0/README.md
+-rw-r--r--   0 root         (0) root         (0)     4941 2023-06-07 22:54:25.000000 myke-0.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-07 23:03:58.480466 myke-0.1.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.460466 myke-0.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.468466 myke-0.1.0/src/myke/
+-rw-r--r--   0 root         (0) root         (0)      871 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       62 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/__main__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.476466 myke-0.1.0/src/myke/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      921 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      195 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/__main__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      148 2023-06-07 23:03:37.000000 myke-0.1.0/src/myke/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      479 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/exceptions.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      421 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/globals.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4015 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/main.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5373 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/run.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/tasks.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      577 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/types.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4640 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/__pycache__/utils.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-06-07 23:03:37.000000 myke-0.1.0/src/myke/__version__.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      206 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/globals.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.476466 myke-0.1.0/src/myke/io/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/io/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.476466 myke-0.1.0/src/myke/io/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/io/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     6365 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/io/__pycache__/echo.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     8474 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/io/__pycache__/read.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3654 2023-06-07 22:54:55.000000 myke-0.1.0/src/myke/io/__pycache__/write.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5929 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/io/echo.py
+-rw-r--r--   0 root         (0) root         (0)     7195 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/io/read.py
+-rw-r--r--   0 root         (0) root         (0)     3669 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/io/write.py
+-rw-r--r--   0 root         (0) root         (0)     6280 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/main.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/py.typed
+-rw-r--r--   0 root         (0) root         (0)     5815 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/run.py
+-rw-r--r--   0 root         (0) root         (0)     5865 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/tasks.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/types.py
+-rw-r--r--   0 root         (0) root         (0)     3988 2023-06-07 22:54:25.000000 myke-0.1.0/src/myke/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.468466 myke-0.1.0/src/myke.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    44520 2023-06-07 23:03:58.000000 myke-0.1.0/src/myke.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1253 2023-06-07 23:03:58.000000 myke-0.1.0/src/myke.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-07 23:03:58.000000 myke-0.1.0/src/myke.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       44 2023-06-07 23:03:58.000000 myke-0.1.0/src/myke.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      799 2023-06-07 23:03:58.000000 myke-0.1.0/src/myke.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-06-07 23:03:58.000000 myke-0.1.0/src/myke.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-07 23:03:58.480466 myke-0.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     4891 2023-06-07 22:54:25.000000 myke-0.1.0/tests/test_Mykefile.py
+-rw-r--r--   0 root         (0) root         (0)     4933 2023-06-07 22:54:25.000000 myke-0.1.0/tests/test_io.py
+-rw-r--r--   0 root         (0) root         (0)     1818 2023-06-07 22:54:25.000000 myke-0.1.0/tests/test_main.py
+-rw-r--r--   0 root         (0) root         (0)     2944 2023-06-07 22:54:25.000000 myke-0.1.0/tests/test_run.py
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-07 22:54:25.000000 myke-0.1.0/tests/test_utils.py
```

### Comparing `myke-0.0.1a9/src/myke/__init__.py` & `myke-0.1.0/src/myke/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,45 +1,48 @@
 from functools import lru_cache as cache
 
 from yapx import arg
 
-from . import exceptions, utils
+from . import exceptions, types, utils
 from .__version__ import __version__
 from .globals import TASKS
 from .io.echo import echo
 from .io.read import read
 from .io.write import write
 from .main import main
-from .sh import require, sh, sh_stdout, sh_stdout_lines
-from .tasks import (
-    add_tasks,
-    import_module,
-    install_module,
-    task,
-    task_sh,
-    task_sh_stdout,
-    task_sh_stdout_lines,
+from .run import (
+    require,
+    run,
+    run_stdout,
+    run_stdout_lines,
+    sh,
+    sh_stdout,
+    sh_stdout_lines,
 )
+from .tasks import add_tasks, import_module, import_mykefile, shell_task, task, task_sh
 
 __all__ = [
     "__version__",
     "TASKS",
     "task",
+    "shell_task",
     "task_sh",
-    "task_sh_stdout",
-    "task_sh_stdout_lines",
     "add_tasks",
+    "import_mykefile",
     "import_module",
-    "install_module",
+    "run",
+    "run_stdout",
+    "run_stdout_lines",
     "sh",
     "sh_stdout",
     "sh_stdout_lines",
     "require",
     "arg",
     "main",
     "read",
     "write",
     "utils",
     "exceptions",
     "cache",
     "echo",
+    "types",
 ]
```

### Comparing `myke-0.0.1a9/src/myke/main.py` & `myke-0.1.0/src/myke/main.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,147 +1,180 @@
-from __future__ import annotations
-
 import os
 import sys
+from contextlib import suppress
 from dataclasses import dataclass
+from fnmatch import fnmatch
 from inspect import getsource
-from typing import Any, Callable
+from pathlib import Path
+from typing import Any, Callable, List, Optional, Union
 
 import yapx
 
 from .__version__ import __version__
 from .exceptions import NoTasksFoundError
 from .globals import DEFAULT_MYKEFILE, MYKE_VAR_NAME, ROOT_TASK_KEY, TASKS
 from .io.echo import echo
-from .io.read import read
 from .io.write import write
-from .tasks import import_module
+from .tasks import import_module, import_mykefile
+from .types import Annotated
+from .utils import get_repo_root
 
 __all__ = ["__version__", "main", "sys"]
 
 
-def main(_file: str | None = None) -> None:
+def main(_file: Optional[Union[str, Path]] = None) -> None:
     @dataclass
     class MykeArgs(yapx.types.Dataclass):
-        file: str = yapx.arg(
-            default=_file if _file else DEFAULT_MYKEFILE,
-            flags=["--myke-file"],
-            env="MYKE_FILE",
-            group="myke args",
-        )
-        file_paths: list[str] = yapx.arg(
-            default=lambda: [os.path.expanduser("~"), os.getcwd()],
-            flags=["--myke-file-paths"],
-            env="MYKE_FILE_PATHS",
-            group="myke args",
-        )
-        env_file: None | str = yapx.arg(
-            default=None,
-            flags=["--myke-env-file"],
-            env="MYKE_ENV_FILE",
-            group="myke args",
-        )
-        update_modules: bool = yapx.arg(
-            default=False,
-            flags=["--myke-update-modules"],
-            env="MYKE_UPDATE_MODULES",
-            group="myke args",
-        )
-        no_pydantic: bool = yapx.arg(
-            default=False, group="myke args", flags=["--myke-no-pydantic"]
-        )
-        task_help: bool = yapx.arg(
-            default=False, group="myke args", exclusive=True, flags=["-h", "--help"]
-        )
-        task_help_all: bool = yapx.arg(
-            default=False, group="myke args", exclusive=True, flags=["--help-all"]
-        )
-        help: bool = yapx.arg(
-            default=False, group="myke args", exclusive=True, flags=["--myke-help"]
-        )
-        explain: bool = yapx.arg(
-            default=False, group="myke args", exclusive=True, flags=["--myke-explain"]
-        )
-        version: bool = yapx.arg(
-            default=False, group="myke args", exclusive=True, flags=["--myke-version"]
-        )
-        create: bool = yapx.arg(
-            default=False, group="myke args", exclusive=True, flags=["--myke-create"]
-        )
+        file: Annotated[
+            Optional[Path],
+            yapx.arg(
+                default=_file if _file else None,
+                flags=["--myke-file"],
+                env="MYKE_FILE",
+                group="myke args",
+            ),
+        ]
+        module: Annotated[
+            Optional[str],
+            yapx.arg(
+                default=None,
+                flags=["--myke-module"],
+                env="MYKE_MODULE",
+                group="myke args",
+            ),
+        ]
+        task_help: Annotated[
+            Optional[bool],
+            yapx.arg(
+                default=None,
+                group="myke args",
+                exclusive=True,
+                flags=["-h", "--help"],
+            ),
+        ]
+        task_help_full: Annotated[
+            Optional[bool],
+            yapx.arg(
+                default=None,
+                group="myke args",
+                exclusive=True,
+                flags=["--help-full"],
+            ),
+        ]
+        help: Annotated[
+            Optional[bool],
+            yapx.arg(
+                default=None,
+                group="myke args",
+                exclusive=True,
+                flags=["--myke-help"],
+            ),
+        ]
+        explain: Annotated[
+            Optional[bool],
+            yapx.arg(
+                default=None,
+                group="myke args",
+                exclusive=True,
+                flags=["--myke-explain"],
+            ),
+        ]
+        create: Annotated[
+            Optional[bool],
+            yapx.arg(
+                default=None,
+                group="myke args",
+                exclusive=True,
+                flags=["--myke-create"],
+            ),
+        ]
+        version: Annotated[
+            Optional[bool],
+            yapx.arg(
+                default=None,
+                group="myke args",
+                exclusive=True,
+                flags=["--myke-version"],
+            ),
+        ]
 
-    prog: str = _file if _file else MYKE_VAR_NAME
+    prog: str = str(_file) if _file else MYKE_VAR_NAME
 
     parser = yapx.ArgumentParser(
         prog=prog,
         add_help=False,
-        description="Parameters for Myke:",
     )
     parser.add_arguments(MykeArgs)
 
     myke_args: MykeArgs
-    task_args: list[str]
+    task_args: List[str]
     myke_args, task_args = parser.parse_known_args_to_model(
-        sys.argv[1:], args_model=MykeArgs, use_pydantic=False
+        sys.argv[1:],
+        args_model=MykeArgs,
+        skip_pydantic_validation=True,
     )
     assert isinstance(myke_args, MykeArgs)
 
     if myke_args.version:
         echo(__version__)
         parser.exit()
-    elif myke_args.create:
-        write.mykefile(myke_args.file)
-        echo(f"Created: {myke_args.file}")
-        parser.exit()
-
-    if myke_args.env_file:
-        os.environ.update(read.envfile(myke_args.env_file))
-
-    if myke_args.update_modules:
-        os.environ["MYKE_UPDATE_MODULES"] = "1"
 
     if _file:
-        if not os.path.exists(_file):
+        if not isinstance(_file, Path):
+            _file = Path(_file)
+        if not _file.exists():
             raise FileNotFoundError(_file)
         if not TASKS:
             raise NoTasksFoundError(_file)
-        _file = os.path.abspath(_file)
+        _file = _file.absolute()
 
-    mykefiles: list[str] = (
-        [myke_args.file]
-        if os.path.dirname(myke_args.file)
-        else [
-            y
-            for x in myke_args.file_paths
-            for y in [os.path.join(x, myke_args.file)]
-            if os.path.exists(y)
-        ]
-    )
+    if myke_args.file:
+        myke_args.file = myke_args.file.absolute()
+    elif Path(DEFAULT_MYKEFILE).exists():
+        myke_args.file = Path(DEFAULT_MYKEFILE).absolute()
+
+    with suppress(FileNotFoundError):
+        repo_root: Optional[Path] = get_repo_root()
+        if repo_root:
+            os.chdir(repo_root)
+
+    if not myke_args.file and Path(DEFAULT_MYKEFILE).exists():
+        myke_args.file = Path(DEFAULT_MYKEFILE).absolute()
+
+    if myke_args.create:
+        out_file: Path = myke_args.file if myke_args.file else Path(DEFAULT_MYKEFILE)
+        write.mykefile(str(out_file))
+        echo(f"Created: {out_file}")
+        parser.exit()
 
-    for f in mykefiles:
-        f = os.path.abspath(f)
-        try:
-            if f != _file:
-                import_module(f)
-            elif not TASKS:
-                raise NoTasksFoundError(f)
-        except FileNotFoundError:
-            parser.print_help()
-            echo(
+    try:
+        if myke_args.file and (not _file or not myke_args.file.samefile(_file)):
+            import_mykefile(str(myke_args.file))
+            os.environ["MYKE_FILE"] = str(myke_args.file)
+    except FileNotFoundError:
+        parser.print_help()
+        echo(
+            (
                 f"{os.linesep}"
                 f"'{myke_args.file}' not found. Create it using:"
                 f"{os.linesep}"
-                f"> {prog} --myke-create --myke-file '{f}'"
+                f"> {prog} --myke-create --myke-file '{myke_args.file}'"
                 f"{os.linesep}"
-            )
-            parser.exit()
+            ),
+        )
+        parser.exit()
+
+    if myke_args.module:
+        import_module(myke_args.module)
+        os.environ["MYKE_MODULE"] = myke_args.module
 
-    root_task: Callable[..., Any] | None = TASKS.pop(ROOT_TASK_KEY, None)
+    root_task: Optional[Callable[..., Any]] = TASKS.pop(ROOT_TASK_KEY, None)
 
     if myke_args.explain:
-        explain_this: None | Callable[..., Any] = None
+        explain_this: Optional[Callable[..., Any]] = None
 
         if not task_args or task_args[0].startswith("-"):
             explain_this = root_task
             if explain_this is None:
                 echo("There is no root task. Provide a task name to explain.")
         else:
             explain_this = TASKS.get(task_args[0], None)
@@ -149,23 +182,40 @@
                 echo(f"Given task name not found: {task_args[0]}")
 
         if explain_this:
             echo(getsource(explain_this))
 
         parser.exit()
 
-    if myke_args.help or (not task_args and not myke_args.task_help_all):
+    show_tui: bool = False
+    if not task_args and not myke_args.help:
+        show_tui = yapx.utils.is_tui_available()
+        myke_args.help = not show_tui
+
+    if myke_args.help:
         parser.print_help()
         echo.tasks(prog=prog)
         parser.exit()
 
+    if task_args:
+        for k in list(TASKS):
+            if not fnmatch(k, task_args[0]):
+                del TASKS[k]
+        if not TASKS and not myke_args.task_help_full:
+            echo.tasks(prog=prog)
+            parser.exit()
+
     if myke_args.task_help:
         task_args.append("--help")
 
+    tui_flags: Optional[List[str]] = ["--tui"] if show_tui else None
+    if tui_flags:
+        task_args.extend(tui_flags)
+
     yapx.run(
         root_task,
         _args=task_args,
         _prog=prog,
-        _print_help=myke_args.task_help_all,
-        _use_pydantic=(not myke_args.no_pydantic),
+        _print_help=bool(myke_args.task_help_full),
+        _tui_flags=tui_flags,
         **TASKS,
     )
```

### Comparing `myke-0.0.1a9/src/myke/tasks.py` & `myke-0.1.0/src/myke/tasks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,108 +1,134 @@
+"""> Functions for registering tasks with myke."""
+
 from __future__ import annotations
 
 import collections.abc
 import os
 from functools import partial, wraps
+from subprocess import CompletedProcess
 from types import ModuleType
 from typing import Any, Callable, Sequence
 
-from .exceptions import MykeNotFoundError, NoTasksFoundError, TaskAlreadyRegisteredError
-from .globals import MYKE_VAR_NAME, ROOT_TASK_KEY, TASKS
-from .io.read import read
-from .io.write import write
-from .sh import sh
-from .utils import (
-    _MykeSourceFileLoader,
-    convert_to_command_string,
-    make_executable,
-    split_and_trim_text,
-)
+from .exceptions import NoTasksFoundError, TaskAlreadyRegisteredError
+from .globals import ROOT_TASK_KEY, TASKS
+from .run import sh
+from .utils import _MykeSourceFileLoader, convert_to_command_string
 
 
 def add_tasks(*args: Callable[..., Any], **kwargs: Callable[..., Any]) -> None:
+    """Register the given callable(s) with myke.
 
+    Arguments:
+        *args:
+        **kwargs:
+
+    Raises:
+        TaskAlreadyRegisteredError:
+
+    Examples:
+        >>> import myke
+        ...
+        >>> def say_hello(name):
+        ...    print(f'Hello {name}.')
+        ...
+        >>> def say_goodbye(name):
+        ...    print(f'Goodbye {name}.')
+        ...
+        >>> myke.add_tasks(say_hello, say_goodbye)
+    """
     kwargs.update({x.__name__: x for x in args})
 
     kwargs = {
         (ROOT_TASK_KEY if k == ROOT_TASK_KEY else convert_to_command_string(k)): v
         for k, v in kwargs.items()
     }
 
     for k, v in kwargs.items():
         v_existing: Callable[..., Any] | None = TASKS.get(k, None)
         if v_existing:
             raise TaskAlreadyRegisteredError(
-                f"Failed to import module '{v.__module__}': "
-                f"Task '{k}' already defined from module '{v_existing.__module__}'"
+                (
+                    f"Failed to import module '{v.__module__}': "
+                    f"Task '{k}' already defined from module '{v_existing.__module__}'"
+                ),
             )
         TASKS[k] = v
 
 
-def import_module(*mykefiles: str, overwrite: bool | None = None) -> None:
-    n_tasks_before: int = len(TASKS)
-    for m in mykefiles:
-        if m.startswith("https://"):
-            m = install_module(m, overwrite=overwrite)
-
-        loader = _MykeSourceFileLoader(os.path.relpath(m), m)
-        mod: ModuleType = ModuleType(loader.name)
-        loader.exec_module(mod)
-
-        if not hasattr(mod, MYKE_VAR_NAME):
-            raise MykeNotFoundError(m)
+def import_mykefile(path: str) -> None:
+    """Import tasks from another Mykefile.
 
-        n_tasks_after: int = len(TASKS)
-        if n_tasks_after <= n_tasks_before:
-            raise NoTasksFoundError(m)
-        n_tasks_before = n_tasks_after
+    Args:
+        path: path to the Mykefile
 
+    Raises:
+        NoTasksFoundError:
 
-def install_module(
-    url: str,
-    path: str | None = None,
-    fail_if_exists: bool | None = None,
-    overwrite: bool | None = None,
-) -> str:
-    if overwrite is None:
-        overwrite = bool(os.getenv("MYKE_UPDATE_MODULES"))
-
-    if not url.startswith("https://"):
-        raise ValueError("Download URLs must start with 'https://'")
+    Examples:
+        >>> import myke
+        ...
+        >>> myke.import_mykefile('/path/to/tasks.py')  # doctest: +SKIP
+    """
+    n_tasks_before: int = len(TASKS)
 
-    if path is None:
-        path = "tasks"
+    loader = _MykeSourceFileLoader(os.path.relpath(path), path)
+    mod: ModuleType = ModuleType(loader.name)
+    loader.exec_module(mod)
 
-        if not os.path.exists(path):
-            os.mkdir(path)
+    if len(TASKS) <= n_tasks_before:
+        raise NoTasksFoundError(path)
 
-        path = os.path.join(path, os.path.basename(url))
 
-    if not overwrite and not fail_if_exists and os.path.exists(path):
-        return path
+def import_module(name: str) -> None:
+    """Import tasks from the given Python module.
 
-    resp_text: str = read.url(url)
+    Args:
+        name: name of the module.
 
-    import_myke: str = f"import {MYKE_VAR_NAME}"
-    if import_myke not in resp_text:
-        raise MykeNotFoundError(f'"{import_myke}" not found response text of {url}')
+    Raises:
+        NoTasksFoundError:
 
-    write(resp_text, path=path, overwrite=overwrite)
+    Examples:
+        >>> import myke
+        ...
+        >>> myke.import_module('python_pkg.python_module')  # doctest: +SKIP
+    """
+    n_tasks_before: int = len(TASKS)
 
-    make_executable(path)
+    __import__(name)
 
-    return path
+    if len(TASKS) <= n_tasks_before:
+        raise NoTasksFoundError(name)
 
 
 def task(
     func: Callable[..., Any] | None = None,
     *,
     name: str | None = None,
     root: bool | None = False,
 ) -> Callable[..., Any] | Callable[..., Callable[..., Any]]:
+    """Function decorator to register functions with myke.
+
+    Args:
+        name: name of the command.
+        root: if True, import this as the root command.
+
+    Examples:
+        >>> from myke import task
+        ...
+        >>> @task  # doctest: +SKIP
+        ... def say_hello(name):
+        ...    print(f'Hello {name}.')
+        ...
+        >>> @task  # doctest: +SKIP
+        ... def say_goodbye(name):
+        ...    print(f'Goodbye {name}.')
+        ...
+    """
 
     if not func:
         return partial(task, name=name, root=root)
 
     if root:
         name = ROOT_TASK_KEY
 
@@ -110,34 +136,55 @@
         add_tasks(**{name: func})
     else:
         add_tasks(func)
 
     return func
 
 
-def task_sh(
+def shell_task(
     func: Callable[..., str | Sequence[str]] | None = None,
     *,
     name: str | None = None,
     root: bool | None = False,
     capture_output: bool | None = False,
     echo: bool | None = True,
     check: bool | None = True,
     cwd: str | None = None,
     env: dict[str, str] | None = None,
-    env_update: dict[str, str] | None = None,
+    env_update: dict[str, str | None] | None = None,
     timeout: float | None = None,
     executable: str | None = None,
 ) -> (
-    Callable[..., tuple[str | None, str | None, int]]
-    | Callable[..., Callable[..., tuple[str | None, str | None, int]]]
+    Callable[..., CompletedProcess[bytes | str]]
+    | Callable[..., Callable[..., CompletedProcess[bytes | str]]]
 ):
+    """Function decorator to register shell commands with myke.
+
+    myke expects the function to return a string of one or more shell-commands,
+    and will invoke the commands using `myke.run(..., shell=True)`.
+
+    Args:
+        name: name of the command.
+        root: if True, import this as the root command.
+
+    Examples:
+        >>> from myke import shell_task
+        ...
+        >>> @shell_task  # doctest: +SKIP
+        ... def say_hello(name):
+        ...    return f"echo 'Hello {name}.'"
+        ...
+        >>> @shell_task  # doctest: +SKIP
+        ... def say_goodbye(name):
+        ...    return f"echo 'Goodbye {name}.'"
+        ...
+    """
     if not func:
         return partial(
-            task_sh,
+            shell_task,
             name=name,
             root=root,
             capture_output=capture_output,
             echo=echo,
             check=check,
             cwd=cwd,
             env=env,
@@ -146,21 +193,22 @@
             executable=executable,
         )
 
     @wraps(func)
     def _inner_func(*args: Any, **kwargs: Any) -> tuple[str | None, str | None, int]:
         assert func
 
-        func_script: str | Sequence[str] = func(*args, **kwargs)
+        func_script: str = func(*args, **kwargs)
 
         if not isinstance(func_script, str) and not isinstance(
-            func_script, collections.abc.Sequence
+            func_script,
+            collections.abc.Sequence,
         ):
             raise TypeError(
-                "Expected a string or list of strings to be returned for `sh` function"
+                "Expected a string to be returned for the `shell_task`",
             )
 
         return sh(
             func_script,
             capture_output=capture_output,
             echo=echo,
             check=check,
@@ -173,73 +221,9 @@
 
     if not name:
         name = func.__name__
 
     return task(_inner_func, name=name, root=root)
 
 
-def _task_sh_stdout_lines(
-    func: Callable[..., str | Sequence[str]] | None = None,
-    *,
-    name: str | None = None,
-    root: bool | None = False,
-    echo: bool | None = False,
-    check: bool | None = True,
-    cwd: str | None = None,
-    env: dict[str, str] | None = None,
-    env_update: dict[str, str] | None = None,
-    timeout: float | None = None,
-    executable: str | None = None,
-    join_lines: bool | None = False,
-) -> (Callable[..., str | list[str]] | Callable[..., Callable[..., str | list[str]]]):
-    if not func:
-        return partial(
-            task_sh_stdout_lines,
-            name=name,
-            root=root,
-            echo=echo,
-            check=check,
-            cwd=cwd,
-            env=env,
-            env_update=env_update,
-            timeout=timeout,
-            executable=executable,
-        )
-
-    @wraps(func)
-    def _inner_func(*args: Any, **kwargs: Any) -> str | list[str]:
-        assert func
-        stdout, *_ = sh(
-            func(*args, **kwargs),
-            capture_output=True,
-            echo=echo,
-            check=check,
-            cwd=cwd,
-            env=env,
-            env_update=env_update,
-            timeout=timeout,
-            executable=executable,
-        )
-
-        stdout_split: list[str] = split_and_trim_text(stdout)
-
-        return os.linesep.join(stdout_split) if join_lines else stdout_split
-
-    if not name:
-        name = func.__name__
-
-    return task(_inner_func, name=name, root=root)
-
-
-@wraps(_task_sh_stdout_lines)
-def task_sh_stdout_lines(
-    *args: Any, **kwargs: Any
-) -> Callable[..., list[str]] | Callable[..., Callable[..., list[str]]]:
-    return _task_sh_stdout_lines(*args, **kwargs)  # type: ignore
-
-
-@wraps(_task_sh_stdout_lines)
-def task_sh_stdout(
-    *args: Any, **kwargs: Any
-) -> Callable[..., str] | Callable[..., Callable[..., str]]:
-    kwargs["join_lines"] = True
-    return _task_sh_stdout_lines(*args, **kwargs)  # type: ignore
+# TODO: deprecate
+task_sh = shell_task
```

