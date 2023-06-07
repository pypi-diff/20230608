# Comparing `tmp/ez_cqrs-1.1.1.tar.gz` & `tmp/ez_cqrs-1.1.3.tar.gz`

## Comparing `ez_cqrs-1.1.1.tar` & `ez_cqrs-1.1.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.tool-versions
--rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/mkdocs.yml
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.github/workflows/release.yml
--rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.github/workflows/test.yml
--rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.vscode/settings.json
--rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/docs/index.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/__init__.py
--rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/acid_exec.py
--rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/components.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/error.py
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/framework.py
--rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/handler.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/py.typed
--rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/shared_state.py
--rw-r--r--   0        0        0     4069 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/ez_cqrs/testing.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/requirements/core.txt
--rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/requirements/dev.txt
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/scripts/new_release.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/__init__.py
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/integration/conftest.py
--rw-r--r--   0        0        0     7687 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/integration/test_execution.py
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/tests/unit/test_acid_exec.py
--rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/LICENSE
--rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/README.md
--rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/pyproject.toml
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.tool-versions
+-rw-r--r--   0        0        0       19 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/mkdocs.yml
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.github/CODEOWNERS
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.github/workflows/release.yml
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.github/workflows/test.yml
+-rw-r--r--   0        0        0      852 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.vscode/settings.json
+-rw-r--r--   0        0        0      491 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/docs/index.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/__init__.py
+-rw-r--r--   0        0        0     2468 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/acid_exec.py
+-rw-r--r--   0        0        0     1226 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/components.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/error.py
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/framework.py
+-rw-r--r--   0        0        0     1536 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/handler.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/py.typed
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/shared_state.py
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/testing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/utilities/__init__.py
+-rw-r--r--   0        0        0      912 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/ez_cqrs/utilities/cli.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/requirements/core.txt
+-rw-r--r--   0        0        0     4063 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/requirements/dev.txt
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/scripts/new_release.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/__init__.py
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/integration/conftest.py
+-rw-r--r--   0        0        0     7818 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/integration/test_execution.py
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/tests/unit/test_acid_exec.py
+-rw-r--r--   0        0        0     3099 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/LICENSE
+-rw-r--r--   0        0        0       87 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/README.md
+-rw-r--r--   0        0        0     2585 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 ez_cqrs-1.1.3/PKG-INFO
```

### Comparing `ez_cqrs-1.1.1/.github/workflows/release.yml` & `ez_cqrs-1.1.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/.github/workflows/test.yml` & `ez_cqrs-1.1.3/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/.vscode/settings.json` & `ez_cqrs-1.1.3/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/ez_cqrs/acid_exec.py` & `ez_cqrs-1.1.3/ez_cqrs/acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/ez_cqrs/components.py` & `ez_cqrs-1.1.3/ez_cqrs/components.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/ez_cqrs/error.py` & `ez_cqrs-1.1.3/ez_cqrs/error.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/ez_cqrs/framework.py` & `ez_cqrs-1.1.3/ez_cqrs/framework.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,29 +24,28 @@
     from ez_cqrs.error import ExecutionError
     from ez_cqrs.handler import CommandHandler, EventDispatcher
     from ez_cqrs.shared_state import Config
 
 T = TypeVar("T")
 
 
+@final
 @dataclass(repr=True, frozen=True, eq=False)
 class EzCqrs(Generic[C, E]):
     """EzCqrs framework."""
 
     cmd_handler: CommandHandler[C, E]
     event_dispatcher: EventDispatcher[E]
 
-    @final
     async def run(
         self,
         cmd: C,
         max_transactions: int,
         config: Config,
-        expected_val: type[T],
-    ) -> Result[T, ExecutionError | pydantic.ValidationError]:
+    ) -> Result[Any, ExecutionError | pydantic.ValidationError]:
         """
         Validate and execute command, then dispatch command events.
 
         Dispatched events are returned to the caller for client specific usage.
         """
         validated = self.cmd_handler.validate(command=cmd)
         if not isinstance(validated, Ok):
@@ -69,12 +68,8 @@
         for event in list_of_events:
             event_dispatch_tasks.append(
                 self.event_dispatcher.dispatch(event=event, config=config),
             )
 
         asyncio.gather(*event_dispatch_tasks, return_exceptions=False)
 
-        if not isinstance(execution_value, expected_val):
-            msg = "Returned value from command does not match expected type."
-            raise TypeError(msg)
-
         return Ok(execution_value)
```

### Comparing `ez_cqrs-1.1.1/ez_cqrs/handler.py` & `ez_cqrs-1.1.3/ez_cqrs/handler.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/ez_cqrs/shared_state.py` & `ez_cqrs-1.1.3/ez_cqrs/shared_state.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/ez_cqrs/testing.py` & `ez_cqrs-1.1.3/ez_cqrs/testing.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Testing framework."""
 from __future__ import annotations
 
+import asyncio
 import sys
 from dataclasses import dataclass, field
 from typing import TYPE_CHECKING, Any, Generic
 
 from result import Ok, Result
 
 if sys.version_info >= (3, 8):
@@ -106,18 +107,20 @@
     async def execute(
         self,
         max_transactions: int,
         config: Config,
     ) -> Self:
         """Execute command while asserting and validating framework's rules."""
         ops_registry = OpsRegistry[Any](max_lenght=max_transactions)
-        execution_result = await self.cmd_handler.handle(
-            command=self.cmd,
-            ops_registry=ops_registry,
-            config=config,
+        execution_result = await asyncio.create_task(
+            self.cmd_handler.handle(
+                command=self.cmd,
+                ops_registry=ops_registry,
+                config=config,
+            ),
         )
         if not ops_registry.is_empty():
             msg = "OpsRegistry is not empty after cmd execution."
             raise RuntimeError(msg)
 
         self._result = execution_result
         return self
```

### Comparing `ez_cqrs-1.1.1/requirements/core.txt` & `ez_cqrs-1.1.3/requirements/core.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/requirements/dev.txt` & `ez_cqrs-1.1.3/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/scripts/new_release.py` & `ez_cqrs-1.1.3/scripts/new_release.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/tests/integration/conftest.py` & `ez_cqrs-1.1.3/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/tests/integration/test_execution.py` & `ez_cqrs-1.1.3/tests/integration/test_execution.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Test handler."""
 from __future__ import annotations
 
+import asyncio
 from dataclasses import dataclass
 from typing import TYPE_CHECKING, Any, Union
 
 import pydantic
 import pytest
 from pydantic import BaseModel, ValidationError
 from result import Err, Ok, Result
@@ -155,18 +156,20 @@
         self,
         command: BankAccountCommand,
         expected_events: list[BankAccountEvent],
     ) -> None:
         """Test handle method."""
         cmd_handler = BankAccountCommandHandler()
         app_config = Config()
-        execution_result = await cmd_handler.handle(
-            command=command,
-            ops_registry=OpsRegistry[Any](max_lenght=0),
-            config=app_config,
+        execution_result = await asyncio.create_task(
+            cmd_handler.handle(
+                command=command,
+                ops_registry=OpsRegistry[Any](max_lenght=0),
+                config=app_config,
+            ),
         )
         _, resultant_events = execution_result.unwrap()
         assert resultant_events == expected_events
 
     @pytest.mark.parametrize(
         argnames=["cmd_handler", "cmd", "expected_value", "expected_events"],
         argvalues=[
@@ -197,17 +200,19 @@
             BankAccountEvent,
         ](
             cmd_handler=cmd_handler,
             cmd=cmd,
         )
 
         assert framework.validate().then_expect_is_valid()
-        await framework.execute(
-            max_transactions=0,
-            config=Config(),
+        await asyncio.create_task(
+            framework.execute(
+                max_transactions=0,
+                config=Config(),
+            ),
         )
         assert framework.then_expect_events(expected_events=expected_events)
         assert framework.then_expect_value(expected_value=expected_value)
         resultant_value, resultant_events = framework.inspect_result()
         assert resultant_value == expected_value
         assert resultant_events == expected_events
```

### Comparing `ez_cqrs-1.1.1/tests/unit/test_acid_exec.py` & `ez_cqrs-1.1.3/tests/unit/test_acid_exec.py`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/.gitignore` & `ez_cqrs-1.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/LICENSE` & `ez_cqrs-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ez_cqrs-1.1.1/pyproject.toml` & `ez_cqrs-1.1.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "ez_cqrs"
-version = "1.1.1"
+version = "1.1.3"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 authors = [
```

### Comparing `ez_cqrs-1.1.1/PKG-INFO` & `ez_cqrs-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ez_cqrs
-Version: 1.1.1
+Version: 1.1.3
 Project-URL: Documentation, https://github.com/Tomperez98/ez-cqrs#readme
 Project-URL: Issues, https://github.com/Tomperez98/ez-cqrs/issues
 Project-URL: Source, https://github.com/Tomperez98/ez-cqrs
 Author-email: Tomas Perez Alvarez <tomasperezalvarez@gmail.com>
 License-File: LICENSE
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
```

