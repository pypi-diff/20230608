# Comparing `tmp/pydiverse-pipedag-0.3.0.tar.gz` & `tmp/pydiverse_pipedag-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydiverse-pipedag-0.3.0.tar", max compression
+gzip compressed data, was "pydiverse_pipedag-0.4.0.tar", max compression
```

## Comparing `pydiverse-pipedag-0.3.0.tar` & `pydiverse_pipedag-0.4.0.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0     1517 2022-08-30 10:19:17.882077 pydiverse-pipedag-0.3.0/LICENSE
--rw-r--r--   0        0        0     7358 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/docs/package/README.md
--rw-r--r--   0        0        0     3426 2023-05-25 11:51:49.756305 pydiverse-pipedag-0.3.0/pyproject.toml
--rw-r--r--   0        0        0       13 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/.gitignore
--rw-r--r--   0        0        0      204 2022-12-07 13:24:39.752944 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/__init__.py
--rw-r--r--   0        0        0      749 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/_typing.py
--rw-r--r--   0        0        0       88 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/__init__.py
--rw-r--r--   0        0        0     5288 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/blob.py
--rw-r--r--   0        0        0    10555 2023-04-16 20:40:25.252504 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/lock.py
--rw-r--r--   0        0        0      177 2022-08-30 10:19:17.886078 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/__init__.py
--rw-r--r--   0        0        0    20065 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/base.py
--rw-r--r--   0        0        0     7267 2023-05-25 11:51:49.744305 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/dict.py
--rw-r--r--   0        0        0    81824 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/sql.py
--rw-r--r--   0        0        0       45 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/__init__.py
--rw-r--r--   0        0        0     1274 2023-01-06 19:08:19.182839 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
--rw-r--r--   0        0        0      456 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/pandas.py
--rw-r--r--   0        0        0    40408 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
--rw-r--r--   0        0        0    12334 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table_cache.py
--rw-r--r--   0        0        0      342 2022-12-15 12:57:17.081298 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/__init__.py
--rw-r--r--   0        0        0     7886 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/context.py
--rw-r--r--   0        0        0    25109 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/run_context.py
--rw-r--r--   0        0        0      164 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/__init__.py
--rw-r--r--   0        0        0     9075 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/flow.py
--rw-r--r--   0        0        0     2512 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/result.py
--rw-r--r--   0        0        0     5714 2023-04-16 20:40:25.256504 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/stage.py
--rw-r--r--   0        0        0     6308 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/task.py
--rw-r--r--   0        0        0      285 2022-12-14 22:29:15.934795 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/__init__.py
--rw-r--r--   0        0        0      648 2022-12-15 12:19:12.124658 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/base.py
--rw-r--r--   0        0        0     6516 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/prefect.py
--rw-r--r--   0        0        0     1380 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/sequential.py
--rw-r--r--   0        0        0     1079 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/errors/__init__.py
--rw-r--r--   0        0        0      124 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/__init__.py
--rw-r--r--   0        0        0     8965 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/cache.py
--rw-r--r--   0        0        0     4332 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/container.py
--rw-r--r--   0        0        0     7940 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/core.py
--rw-r--r--   0        0        0     2039 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/metadata.py
--rw-r--r--   0        0        0    17651 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/store.py
--rw-r--r--   0        0        0       37 2022-09-01 08:31:55.058666 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/__init__.py
--rw-r--r--   0        0        0     1104 2022-12-21 15:30:37.854038 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/cache.py
--rw-r--r--   0        0        0     4231 2023-05-05 10:44:44.012529 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/json.py
--rw-r--r--   0        0        0      228 2023-01-14 15:50:16.896380 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/__init__.py
--rw-r--r--   0        0        0    15639 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/config.py
--rw-r--r--   0        0        0     2061 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_map.py
--rw-r--r--   0        0        0     1435 2022-12-27 12:07:46.136373 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_merge.py
--rw-r--r--   0        0        0      880 2022-12-14 22:31:58.730527 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/disposable.py
--rw-r--r--   0        0        0     1707 2022-12-15 13:01:08.984954 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/import_.py
--rw-r--r--   0        0        0     8982 2023-02-08 18:46:59.148930 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/ipc.py
--rw-r--r--   0        0        0     1553 2023-05-25 11:51:49.748304 pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/naming.py
--rw-r--r--   0        0        0     9604 2023-05-25 11:52:05.977180 pydiverse-pipedag-0.3.0/setup.py
--rw-r--r--   0        0        0     9743 2023-05-25 11:52:05.977721 pydiverse-pipedag-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1517 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/LICENSE
+-rw-r--r--   0        0        0     7260 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/docs/package/README.md
+-rw-r--r--   0        0        0     3059 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0       13 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/.gitignore
+-rw-r--r--   0        0        0      313 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/__init__.py
+-rw-r--r--   0        0        0      749 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/_typing.py
+-rw-r--r--   0        0        0       88 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/__init__.py
+-rw-r--r--   0        0        0     5334 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/blob.py
+-rw-r--r--   0        0        0    10562 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/lock.py
+-rw-r--r--   0        0        0      177 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/__init__.py
+-rw-r--r--   0        0        0    20296 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/base.py
+-rw-r--r--   0        0        0     7267 2023-06-08 13:02:28.267153 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/dict.py
+-rw-r--r--   0        0        0    82994 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/sql.py
+-rw-r--r--   0        0        0       45 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/__init__.py
+-rw-r--r--   0        0        0     1274 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py
+-rw-r--r--   0        0        0      456 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/pandas.py
+-rw-r--r--   0        0        0    40457 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py
+-rw-r--r--   0        0        0    12122 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table_cache.py
+-rw-r--r--   0        0        0      342 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/__init__.py
+-rw-r--r--   0        0        0     8079 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/context.py
+-rw-r--r--   0        0        0    25913 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/run_context.py
+-rw-r--r--   0        0        0      219 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/__init__.py
+-rw-r--r--   0        0        0    13470 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/config.py
+-rw-r--r--   0        0        0     9204 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/flow.py
+-rw-r--r--   0        0        0     2544 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/result.py
+-rw-r--r--   0        0        0     5665 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/stage.py
+-rw-r--r--   0        0        0     6360 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/task.py
+-rw-r--r--   0        0        0      285 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/__init__.py
+-rw-r--r--   0        0        0      648 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/base.py
+-rw-r--r--   0        0        0     6516 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/prefect.py
+-rw-r--r--   0        0        0     1380 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/sequential.py
+-rw-r--r--   0        0        0     1079 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/errors/__init__.py
+-rw-r--r--   0        0        0      124 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/__init__.py
+-rw-r--r--   0        0        0     8908 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/cache.py
+-rw-r--r--   0        0        0     5422 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/container.py
+-rw-r--r--   0        0        0     7855 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/core.py
+-rw-r--r--   0        0        0     2039 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/metadata.py
+-rw-r--r--   0        0        0    17644 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/store.py
+-rw-r--r--   0        0        0       37 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/__init__.py
+-rw-r--r--   0        0        0     1104 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/cache.py
+-rw-r--r--   0        0        0     4231 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/json.py
+-rw-r--r--   0        0        0      177 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/__init__.py
+-rw-r--r--   0        0        0     2061 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_map.py
+-rw-r--r--   0        0        0     1435 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_merge.py
+-rw-r--r--   0        0        0      880 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/disposable.py
+-rw-r--r--   0        0        0     2927 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/import_.py
+-rw-r--r--   0        0        0     9283 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/ipc.py
+-rw-r--r--   0        0        0     1553 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/naming.py
+-rw-r--r--   0        0        0     2811 2023-06-08 13:02:28.271154 pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/structlog.py
+-rw-r--r--   0        0        0     8747 1970-01-01 00:00:00.000000 pydiverse_pipedag-0.4.0/PKG-INFO
```

### Comparing `pydiverse-pipedag-0.3.0/LICENSE` & `pydiverse_pipedag-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/docs/package/README.md` & `pydiverse_pipedag-0.4.0/docs/package/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 
 ```python
 from pydiverse.pipedag import materialize, Table, Flow, Stage
 import sqlalchemy as sa
 import pandas as pd
 
 from pydiverse.pipedag.context import StageLockContext, RunContext
-from pydiverse.pipedag.util import setup_structlog
 
 
 @materialize(lazy=True)
 def lazy_task_1():
     return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])
 
 
@@ -96,16 +95,14 @@
     with StageLockContext():
         result = f.run()
         assert result.successful
         assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1
 
 
 if __name__ == "__main__":
-    # initialize logging
-    setup_structlog()
     main()
 ```
 
 Create a file called `pipedag.yaml` in the same directory:
 
 ```yaml
 name: pipedag_tests
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/_typing.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/_typing.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/blob.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/blob.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import pickle
 import shutil
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 from pydiverse.pipedag.context import ConfigContext
+from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.util import Disposable, normalize_name
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Stage
     from pydiverse.pipedag.materialize import Blob
 
 __all__ = [
@@ -131,15 +132,15 @@
     def copy_blob_to_transaction(self, blob: Blob):
         try:
             shutil.copy2(
                 self.get_blob_path(blob.stage.name, blob.name),
                 self.get_blob_path(blob.stage.transaction_name, blob.name),
             )
         except FileNotFoundError:
-            raise RuntimeError(
+            raise CacheError(
                 f"Can't copy blob '{blob.name}' (stage: '{blob.stage.name}')"
                 " to working transaction because no such blob exists."
             ) from None
 
     def delete_blob_from_transaction(self, blob: Blob):
         try:
             os.remove(self.get_blob_path(blob.stage.transaction_name, blob.name))
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/lock.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/lock.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     A lock manager is responsible for acquiring and releasing locks on
     stage. This is necessary to prevent two flows from accessing the
     same stage at the same time (which would lead to corrupted data).
     """
 
     def __init__(self):
-        self.logger = structlog.get_logger(lock=type(self).__name__)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
 
         self.state_listeners = set()
         self.lock_states = defaultdict(lambda: LockState.UNLOCKED)
         self.__lock_state_lock = threading.Lock()
 
     @contextmanager
     def __call__(self, lock: Lockable):
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/base.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,21 @@
         internal type. This means, that in some cases it first has to
         evaluate a lazy object. For example: if a sql based table store
         receives a sql query to store, it has to execute it first.
 
         The implementation details of this get handled by the registered
         TableHooks.
         """
-        _ = task  # not needed in this kind of store_table, yet
+
+        # In case of deferred operations, inform run context that stage
+        # isn't 100% cache valid anymore.
+        if task is not None:
+            RunContext.get().set_stage_has_changed(task.stage)
+
+        # Materialize
         hook = self.get_m_table_hook(type(table.obj))
         stage_name = (
             table.stage.transaction_name if use_transaction_name else table.stage.name
         )
         hook.materialize(self, table, stage_name, task_info)
 
     def retrieve_table_obj(
@@ -154,15 +160,19 @@
                 "to dematerialize a Table."
             )
 
         hook = self.get_r_table_hook(as_type)
         stage_name = (
             table.stage.current_name if use_transaction_name else table.stage.name
         )
-        return hook.retrieve(self, table, stage_name, as_type, namer)
+
+        try:
+            return hook.retrieve(self, table, stage_name, as_type, namer)
+        except Exception as e:
+            raise RuntimeError(f"Failed to retrieve table '{table}'") from e
 
 
 class BaseTableStore(TableHookResolver):
     """Table store base class
 
     The table store is responsible for storing and retrieving various types
     of tabular data. Additionally, it also has to manage all task metadata,
@@ -185,15 +195,15 @@
     finished running *successfully* you swap the 'base schema' (original stage,
     or cache) with the 'transaction schema'. This is usually done by renaming
     them.
 
     """
 
     def __init__(self):
-        self.logger = structlog.get_logger(type(self).__name__)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
 
     def setup(self):
         """Setup function
 
         This function gets called at the beginning of a flow run.
         Unlike the __init__ method, a lock is acquired before
         the setup method gets called to prevent race conditions.
@@ -263,15 +273,14 @@
             # -> Fallback to default implementation
             return self.store_table(table, task, task_info)
 
         table_cache_info = CacheManager.lazy_table_cache_lookup(
             self, task_info.task_cache_info, table, query_hash
         )
         if not table_cache_info.is_cache_valid():
-            RunContext.get().stage_output_cache_invalid(task.stage)
             self.store_table(table, task, task_info)
 
         # At this point we MUST also update the cache info, so that any downstream
         # tasks get invalidated if the sql query string changed.
         table.cache_key = CacheManager.lazy_table_cache_key(
             task_info.task_cache_info.get_task_cache_key(), query_hash
         )
@@ -289,15 +298,15 @@
         _ = task
         query_hash = compute_cache_key("RAW-SQL", raw_sql.sql)
 
         table_cache_info = CacheManager.raw_sql_cache_lookup(
             self, task_info.task_cache_info, raw_sql, query_hash
         )
         if not table_cache_info.is_cache_valid():
-            RunContext.get().stage_output_cache_invalid(task.stage)
+            RunContext.get().set_stage_has_changed(task.stage)
             prev_tables = self.list_tables(raw_sql.stage, include_everything=True)
             self.execute_raw_sql(raw_sql)
             post_tables = self.list_tables(raw_sql.stage, include_everything=True)
             table_cache_info.store_raw_sql_metadata(self, prev_tables, post_tables)
 
         # At this point we MUST also update the cache info, so that any downstream
         # tasks get invalidated if the sql query string changed.
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/dict.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/dict.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/sql.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/sql.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,14 @@
 from __future__ import annotations
 
-import copy
 import itertools
 import json
 import re
 import textwrap
-import threading
 import time
-import traceback
 import warnings
 from collections.abc import Iterable
 from contextlib import contextmanager
 from typing import Any
 
 import pandas as pd
 import sqlalchemy as sa
@@ -44,24 +41,24 @@
     RenameTable,
     Schema,
     ibm_db_sa_fix_name,
     split_ddl_statement,
 )
 from pydiverse.pipedag.context import RunContext
 from pydiverse.pipedag.context.context import ConfigContext, StageCommitTechnique
+from pydiverse.pipedag.context.run_context import DeferredTableStoreOp
 from pydiverse.pipedag.errors import CacheError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 from pydiverse.pipedag.materialize.metadata import (
     LazyTableMetadata,
     RawSqlMetadata,
     TaskMetadata,
 )
 from pydiverse.pipedag.materialize.util import compute_cache_key
-from pydiverse.pipedag.util.ipc import human_thread_id
 from pydiverse.pipedag.util.naming import NameDisambiguator
 
 
 class SQLTableStore(BaseTableStore):
     """Table store that materializes tables to a SQL database
 
     Uses schema swapping for transactions:
@@ -318,15 +315,15 @@
             if isinstance(query, str):
                 query_str = query
             else:
                 query_str = str(
                     query.compile(self.engine, compile_kwargs={"literal_binds": True})
                 )
             pretty_query_str = self.format_sql_string(query_str)
-            self.logger.info(f"Executing sql:\n{pretty_query_str}")
+            self.logger.info("Executing sql", query=pretty_query_str)
 
         if isinstance(query, str):
             return conn.execute(sa.text(query))
         else:
             return conn.execute(query)
 
     def execute(self, query, *, conn: sa.engine.Connection = None):
@@ -580,15 +577,15 @@
 
         sql_string = raw_sql.sql
         if self.print_sql:
             print_query_string = self.format_sql_string(sql_string)
             max_length = 5000
             if len(print_query_string) >= max_length:
                 print_query_string = print_query_string[:max_length] + " [...]"
-            self.logger.info(f"Executing sql:\n{print_query_string}")
+            self.logger.info("Executing sql", query=print_query_string)
 
         pytsql.executes(
             sql_string,
             self.engine,
             isolate_top_level_statements=self.pytsql_isolate_top_level_statements,
         )
 
@@ -792,14 +789,22 @@
         # TODO: WE SHOULD NOT MODIFY THE STAGE AFTER CREATION!!!
         stage.set_transaction_name(new_transaction_name)
 
         # Call schema swap function with updated transaction name
         self._init_stage_schema_swap(stage)
 
     def commit_stage(self, stage: Stage):
+        # If the stage is 100% cache valid, then we just need to update the
+        # "in_transaction_schema" column of the metadata tables.
+        if not RunContext.get().has_stage_changed(stage):
+            with self.engine_connect() as conn:
+                self._commit_stage_update_metadata(stage, conn)
+            return
+
+        # Commit normally
         stage_commit_technique = ConfigContext.get().stage_commit_technique
         if stage_commit_technique == StageCommitTechnique.SCHEMA_SWAP:
             return self._commit_stage_schema_swap(stage)
         if stage_commit_technique == StageCommitTechnique.READ_VIEWS:
             return self._commit_stage_read_views(stage)
         raise ValueError(f"Invalid stage commit technique: {stage_commit_technique}")
 
@@ -922,162 +927,181 @@
                 conn.execute(
                     table.update()
                     .where(table.c.stage == stage.name)
                     .values(in_transaction_schema=False)
                 )
 
     def copy_table_to_transaction(self, table: Table):
-        stage = table.stage
-        schema_name = self.get_schema(stage.name).get()
+        from_schema = self.get_schema(table.stage.name)
+        from_name = table.name
+
+        if RunContext.get().has_stage_changed(table.stage):
+            self._copy_table(table, from_schema, from_name)
+        else:
+            self._deferred_copy_table(table, from_schema, from_name)
+
+    def copy_lazy_table_to_transaction(self, metadata: LazyTableMetadata, table: Table):
+        from_schema = self.get_schema(metadata.stage)
+        from_name = metadata.name
+
+        if RunContext.get().has_stage_changed(table.stage):
+            self._copy_table(table, from_schema, from_name)
+        else:
+            self._deferred_copy_table(table, from_schema, from_name)
+
+    def _copy_table(self, table: Table, from_schema: Schema, from_name: str):
+        """Copies the table immediately"""
         has_table = sa.inspect(self.engine).has_table(
-            self.name_adj(table.name), schema=self.name_adj(schema_name)
+            self.name_adj(from_name), schema=self.name_adj(from_schema.get())
         )
-        if not has_table:
-            raise RuntimeError(
-                f"Can't copy table '{table.name}' (schema: '{stage.name}')"
-                " to transaction because no such table exists."
-            )
 
-        try:
-            self.execute(
-                CopyTable(
-                    table.name,
-                    self.get_schema(stage.name),
-                    table.name,
-                    self.get_schema(stage.transaction_name),
-                )
+        if not has_table:
+            available_tables = sa.inspect(self.engine).get_table_names(
+                self.name_adj(from_schema.get())
             )
-        except Exception as _e:
             msg = (
-                f"Failed to copy table '{table.name}' (schema: '{stage.name}')"
-                " to transaction."
+                f"Can't copy table '{from_name}' (schema: '{from_schema}') to "
+                f"transaction because no such table exists.\n"
+                f"Tables in schema: {available_tables}"
             )
-            self.logger.error(
-                msg,
-                exception=traceback.format_exc(),
+            self.logger.error(msg)
+            raise CacheError(msg)
+
+        self.execute(
+            CopyTable(
+                from_name,
+                from_schema,
+                table.name,
+                self.get_schema(table.stage.transaction_name),
+                early_not_null=table.primary_key,
             )
-            raise RuntimeError(msg) from _e
-        self.add_indexes(table, self.get_schema(stage.transaction_name))
+        )
+        self.add_indexes(table, self.get_schema(table.stage.transaction_name))
 
-    def deferred_copy_lazy_table_to_transaction(
-        self, src_name: str, src_stage: Stage, table: Table
+    def _deferred_copy_table(
+        self,
+        table: Table,
+        from_schema: Schema,
+        from_name: str,
     ):
-        stage = table.stage
-        src_schema = self.get_schema(src_stage)
-        dest_schema = self.get_schema(stage.transaction_name)
-        thread_id = human_thread_id(threading.get_ident())
-        try:
-            self.logger.info(
-                "Running table copy in background",
-                thread=thread_id,
-                table=src_name,
-                src_schema=src_schema.get(),
-                dest_schema=dest_schema.get(),
-            )
-            self.execute(
-                CopyTable(
-                    src_name,
-                    src_schema,
-                    "__cpy_" + src_name,
-                    dest_schema,
-                    early_not_null=table.primary_key,
-                )
+        """Tries to perform a deferred copy
+
+        As long as the stage is determined to still be 100% cache valid, we don't
+        actually copy any tables to the transaction, and instead just create an alias
+        from the main schema to the transaction schema.
+
+        If at the end of the stage, the all tables in the stage are cache valid, then
+        we don't actually need to commit the stage, and instead just rename the
+        tables from their old names to their new names.
+
+        Otherwise, we copy the tables to the transaction schema in the background,
+        and once we're ready to commit, we replace the aliases with the copied tables.
+        """
+        assert from_schema == self.get_schema(table.stage.name)
+
+        has_table = sa.inspect(self.engine).has_table(
+            self.name_adj(from_name), schema=self.name_adj(from_schema.get())
+        )
+        if not has_table:
+            available_tables = sa.inspect(self.engine).get_table_names(
+                self.name_adj(from_schema.get())
             )
-        except Exception as _e:
             msg = (
-                f"Failed to copy lazy table {src_name} (schema:"
-                f" '{src_schema}' -> '{dest_schema}') to transaction."
+                f"Can't deferred copy table '{from_name}' (schema: '{from_schema}') to "
+                f"transaction because no such table exists.\n"
+                f"Tables in schema: {available_tables}"
             )
-            self.logger.error(
-                "Exception in table copy in background",
-                thread=thread_id,
-                table=src_name,
-                msg=msg,
-                exception=str(_e),
-            )
-            raise RuntimeError(msg) from _e
-        table = copy.deepcopy(table)
-        table.name = "__cpy_" + src_name
-        self.add_indexes(
-            table, self.get_schema(stage.transaction_name), early_not_null_possible=True
-        )
-        self.logger.info(
-            "Completed table copy in background",
-            thread=thread_id,
-            table=src_name,
-            src_schema=src_schema.get(),
-            dest_schema=dest_schema.get(),
-        )
+            self.logger.error(msg)
+            raise CacheError(msg)
 
-    def swap_alias_and_copied_table(
-        self, src_name: str, src_stage: Stage, table: Table
-    ):
-        stage = table.stage
-        dest_schema = self.get_schema(stage.transaction_name)
         try:
+            ctx = RunContext.get()
+            stage = table.stage
+
             self.execute(
-                DropAlias(
-                    src_name,
-                    dest_schema,
+                CreateAlias(
+                    from_name,
+                    from_schema,
+                    table.name,
+                    self.get_schema(stage.transaction_name),
                 )
             )
-            self.execute(
-                RenameTable(
-                    "__cpy_" + src_name,
-                    src_name,
-                    dest_schema,
-                )
+
+            table_copy = table.copy_without_obj()
+            table_copy.name = f"{table.name}__copy"
+
+            ctx.defer_table_store_op(
+                stage,
+                DeferredTableStoreOp(
+                    "_copy_table",
+                    DeferredTableStoreOp.Condition.ON_STAGE_CHANGED,
+                    (
+                        table_copy,
+                        from_schema,
+                        from_name,
+                    ),
+                ),
             )
-        except Exception as _e:
-            msg = (
-                f"Failed putting copied lazy table (__cpy_){src_name} (schema:"
-                f" '{dest_schema.get()}') in place of alias."
+            ctx.defer_table_store_op(
+                stage,
+                DeferredTableStoreOp(
+                    "_swap_alias_with_table_copy",
+                    DeferredTableStoreOp.Condition.ON_STAGE_COMMIT,
+                    (),
+                    {"table": table, "table_copy": table_copy},
+                ),
+            )
+            ctx.defer_table_store_op(
+                stage,
+                DeferredTableStoreOp(
+                    "_rename_table",
+                    DeferredTableStoreOp.Condition.ON_STAGE_ABORT,
+                    (from_name, table.name, from_schema),
+                ),
             )
-            raise RuntimeError(msg) from _e
 
-    def copy_lazy_table_to_transaction(self, metadata: LazyTableMetadata, table: Table):
-        stage = table.stage
-        schema_name = self.get_schema(metadata.stage).get()
-        has_table = sa.inspect(self.engine).has_table(
-            self.name_adj(metadata.name), schema=self.name_adj(schema_name)
-        )
-        if not has_table:
+        except Exception as _e:
             msg = (
-                f"Can't copy lazy table '{metadata.name}' (schema:"
-                f" '{metadata.stage}') to transaction because no such table"
-                " exists."
+                f"Failed to copy table {from_name} (schema: '{from_schema}') "
+                f"to transaction."
             )
-            self.logger.error(msg)
-            raise RuntimeError(msg)
+            self.logger.exception(msg)
+            raise CacheError(msg) from _e
+
+    def _swap_alias_with_table_copy(self, table: Table, table_copy: Table):
+        assert table_copy.stage.name == table.stage.name
 
+        schema = self.get_schema(table.stage.transaction_name)
         try:
             self.execute(
-                CreateAlias(
-                    metadata.name,
-                    self.get_schema(metadata.stage),
-                    metadata.name,
-                    self.get_schema(stage.transaction_name),
+                DropAlias(
+                    table.name,
+                    schema,
                 )
             )
-            RunContext.get().deferred_table_store_op_if_stage_invalid(
-                stage,
-                "deferred_copy_lazy_table_to_transaction",
-                "swap_alias_and_copied_table",
-                metadata.name,
-                metadata.stage,
-                table,
+            self.execute(
+                RenameTable(
+                    table_copy.name,
+                    table.name,
+                    schema,
+                )
             )
         except Exception as _e:
             msg = (
-                f"Failed to copy lazy table {metadata.name} (schema:"
-                f" '{metadata.stage}') to transaction."
+                f"Failed putting copied table {table_copy.name} (schema: '{schema}') "
+                f"in place of alias."
             )
-            self.logger.error(msg, exception=traceback.format_exc())
             raise RuntimeError(msg) from _e
 
+    def _rename_table(self, from_name: str, to_name: str, schema: Schema):
+        if from_name == to_name:
+            return
+        self.logger.info("RENAME", fr=from_name, to=to_name)
+        self.execute(RenameTable(from_name, to_name, schema))
+
     @engine_dispatch
     def get_view_names(self, schema: str, *, include_everything=False) -> list[str]:
         """
         List all views that are present in a schema.
 
         It may also include other database objects like stored procedures, functions,
         etc. which makes the name `get_view_names` too specific. But sqlalchemy
@@ -1163,19 +1187,20 @@
                     dest_schema,
                 )
             except Exception as _e:
                 msg = (
                     f"Failed to copy raw sql generated table {table_name} (schema:"
                     f" '{src_schema}') to transaction."
                 )
-                self.logger.error(
-                    msg,
-                    exception=traceback.format_exc(),
+                self.logger.exception(
+                    msg
+                    + " This error is treated as cache-lookup-failure and thus we can"
+                    " continue."
                 )
-                raise RuntimeError(msg) from _e
+                raise CacheError(msg) from _e
 
         views_to_copy = new_tables & set(views)
         for view_name in views_to_copy:
             self._copy_view_to_transaction(view_name, src_schema, dest_schema)
 
     @engine_dispatch
     def _copy_view_to_transaction(
@@ -1253,15 +1278,15 @@
     ) -> TaskMetadata:
         if self.disable_caching:
             raise CacheError(
                 "Caching is disabled, so we also don't even try to retrieve task"
                 f" cache: {task}"
             )
 
-        ignore_fresh_input = RunContext.get().ignore_fresh_input
+        ignore_fresh_input = ConfigContext.get().ignore_fresh_input
         try:
             with self.engine_connect() as conn:
                 result = (
                     conn.execute(
                         self.tasks_table.select()
                         .where(self.tasks_table.c.name == task.name)
                         .where(self.tasks_table.c.stage == task.stage.name)
@@ -1274,15 +1299,15 @@
                         )
                         .where(self.tasks_table.c.in_transaction_schema.in_([False]))
                     )
                     .mappings()
                     .one_or_none()
                 )
         except sa.exc.MultipleResultsFound:
-            raise RuntimeError("Multiple results found task metadata") from None
+            raise CacheError("Multiple results found task metadata") from None
 
         if result is None:
             raise CacheError(f"Couldn't retrieve task from cache: {task}")
 
         return TaskMetadata(
             name=result.name,
             stage=result.stage,
@@ -1329,15 +1354,15 @@
                             self.lazy_cache_table.c.in_transaction_schema.in_([False])
                         )
                     )
                     .mappings()
                     .one_or_none()
                 )
         except sa.exc.MultipleResultsFound:
-            raise RuntimeError(
+            raise CacheError(
                 "Multiple results found for lazy table cache key"
             ) from None
 
         if result is None:
             raise CacheError("No result found for lazy table cache key")
 
         return LazyTableMetadata(
@@ -1385,15 +1410,15 @@
                             )
                         )
                     )
                     .mappings()
                     .one_or_none()
                 )
         except sa.exc.MultipleResultsFound:
-            raise RuntimeError("Multiple results found for raw sql cache key") from None
+            raise CacheError("Multiple results found for raw sql cache key") from None
 
         if result is None:
             raise CacheError("No result found for raw sql cache key")
 
         return RawSqlMetadata(
             prev_tables=json.loads(result.prev_tables),
             tables=json.loads(result.tables),
@@ -1514,20 +1539,23 @@
         table_name = table.name
         schema = store.get_schema(stage_name).get()
         table_name, schema = store.resolve_aliases(table_name, schema)
         tbl = None
         for retry_iteration in range(4):
             # retry operation since it might have been terminated as a deadlock victim
             try:
+                alias_name = (
+                    namer.get_name(table_name) if namer is not None else table_name
+                )
                 tbl = sa.Table(
                     table_name,
                     sa.MetaData(),
                     schema=schema,
                     autoload_with=store.engine,
-                ).alias(namer.get_name(table_name))
+                ).alias(alias_name)
                 break
             except (sa.exc.SQLAlchemyError, sa.exc.DBAPIError):
                 if retry_iteration == 3:
                     raise
                 time.sleep(retry_iteration * retry_iteration * 1.2)
         return tbl
 
@@ -1658,15 +1686,16 @@
         task_info: TaskInfo | None,
     ):
         # we might try to avoid this copy for speedup / saving RAM
         df = table.obj.copy()
         schema = store.get_schema(stage_name)
         if store.print_materialize:
             store.logger.info(
-                f"Writing table '{schema.get()}.{table.name}':\n{table.obj}"
+                f"Writing table '{schema.get()}.{table.name}'",
+                table_obj=table.obj,
             )
         dtype_map = {}
         table_name = table.name
         str_type = sa.String()
         if store.engine.dialect.name == "ibm_db_sa":
             # Default string target is CLOB which can't be used for indexing.
             # We could use VARCHAR(32000), but if we change this to VARCHAR(256)
@@ -1895,19 +1924,18 @@
     def materialize(
         cls,
         store,
         table: Table[tidypolars.Tibble],
         stage_name,
         task_info: TaskInfo | None,
     ):
-        tibble = table.obj
-        table.obj = None
-        table = copy.deepcopy(table)
-        table.obj = tibble.to_polars()
-        PolarsTableHook.materialize(store, table, stage_name, task_info)
+        t = table.obj
+        table = table.copy_without_obj()
+        table.obj = t.obj.to_polars()
+        PolarsTableHook.materialize(store, t, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
@@ -1949,16 +1977,15 @@
     def materialize(
         cls, store, table: Table[pdt.Table], stage_name, task_info: TaskInfo | None
     ):
         from pydiverse.transform.eager import PandasTableImpl
         from pydiverse.transform.lazy import SQLTableImpl
 
         t = table.obj
-        table.obj = None
-        table = copy.deepcopy(table)
+        table = table.copy_without_obj()
         if isinstance(t._impl, PandasTableImpl):
             from pydiverse.transform.core.verbs import collect
 
             table.obj = t >> collect()
             # noinspection PyTypeChecker
             return PandasTableHook.materialize(store, table, stage_name, task_info)
         if isinstance(t._impl, SQLTableImpl):
@@ -2061,19 +2088,17 @@
         cls,
         store,
         table: Table[ibis_types.Table],
         stage_name,
         task_info: TaskInfo | None,
     ):
         t = table.obj
-        table.obj = None
-        # noinspection PyTypeChecker
-        sa_table = copy.deepcopy(table)  # type: Table[sa.Text]
-        sa_table.obj = sa.text(cls.lazy_query_str(store, t))
-        return SQLAlchemyTableHook.materialize(store, sa_table, stage_name, task_info)
+        table = table.copy_without_obj()
+        table.obj = sa.text(cls.lazy_query_str(store, t))
+        return SQLAlchemyTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: SQLTableStore,
         table: Table,
         stage_name: str,
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/engine_dispatch.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table/util/sql_ddl.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,17 @@
     name: str
     prefix: str
     suffix: str
 
     def get(self):
         return self.prefix + self.name + self.suffix
 
+    def __str__(self):
+        return self.get()
+
 
 class CreateSchema(DDLElement):
     def __init__(self, schema: Schema, if_not_exists=False):
         self.schema = schema
         self.if_not_exists = if_not_exists
 
 
@@ -300,15 +303,15 @@
     database_name, schema_name = full_name.split(".")
     database = compiler.preparer.format_schema(database_name)
     schema = compiler.preparer.format_schema(schema_name)
     create_schema = f"CREATE SCHEMA {schema}"
     create_database = f"CREATE DATABASE {database}"
     if create.if_not_exists:
         create_database = f"""
-            IF NOT EXISTS ( 
+            IF NOT EXISTS (
                 SELECT * FROM sys.databases WHERE name = N'{database_name}'
             )
             BEGIN {create_database} END"""
         create_schema = f"""
             IF NOT EXISTS (
                 SELECT * FROM sys.schema WHERE name = N'{schema_name}'
             )
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/backend/table_cache.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/backend/table_cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,10 @@
 from __future__ import annotations
 
-import copy
 import json
-import os
 import shutil
 import warnings
 from abc import ABC, abstractmethod
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
 import pandas as pd
@@ -34,15 +32,15 @@
     def __init__(
         self,
         obj: BaseTableCache | None,
         store_input,
         store_output,
         use_stored_input_as_cache,
     ):
-        self.logger = structlog.getLogger(module=__name__, cls=self.__class__.__name__)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
         self.obj = obj
         self.store_input = store_input
         self.store_output = store_output
         self.use_stored_input_as_cache = use_stored_input_as_cache
 
     def store_table(
         self,
@@ -134,15 +132,14 @@
     def _init_conf_(cls, config: dict[str, Any]):
         instance_id = normalize_name(ConfigContext.get().instance_id)
         base_path = Path(config["base_path"]) / instance_id
         return cls(base_path)
 
     def __init__(self, base_path: str | Path):
         self.base_path = Path(base_path).absolute()
-        os.makedirs(self.base_path, exist_ok=True)
 
     def store_table(self, table: Table, task: MaterializingTask, task_info: TaskInfo):
         _dir = self.base_path / table.stage.name
         _dir.mkdir(exist_ok=True, parents=True)
 
         super().store_table(table, task, task_info, use_transaction_name=False)
 
@@ -293,18 +290,17 @@
     def materialize(
         cls,
         store,
         table: Table[tidypolars.Tibble],
         stage_name,
         task_info: TaskInfo | None,
     ):
-        tibble = table.obj
-        table.obj = None
-        table = copy.deepcopy(table)
-        table.obj = tibble.to_polars()
+        t = table.obj
+        table = table.copy_without_obj()
+        table.obj = t.to_polars()
         PolarsParquetTableHook.materialize(store, table, stage_name, task_info)
 
     @classmethod
     def retrieve(
         cls,
         store: ParquetTableCache,
         table: Table,
@@ -344,23 +340,21 @@
     @classmethod
     def materialize(
         cls, store, table: Table[pdt.Table], stage_name, task_info: TaskInfo | None
     ):
         from pydiverse.transform.eager import PandasTableImpl
 
         t = table.obj
-        table.obj = None
-        # noinspection PyTypeChecker
-        pd_table = copy.deepcopy(table)  # type: Table[pd.DataFrame]
+        table = table.copy_without_obj()
         if isinstance(t._impl, PandasTableImpl):
             from pydiverse.transform.core.verbs import collect
 
-            pd_table.obj = t >> collect()
+            table.obj = t >> collect()
             return PandasParquetTableHook.materialize(
-                store, pd_table, stage_name, task_info
+                store, table, stage_name, task_info
             )
         raise NotImplementedError
 
     @classmethod
     def retrieve(
         cls,
         store: ParquetTableCache,
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/context.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/context.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,27 +2,26 @@
 
 from contextvars import ContextVar, Token
 from enum import Enum
 from functools import cached_property
 from threading import Lock
 from typing import TYPE_CHECKING, Any, ClassVar
 
-from pydiverse.pipedag.util.config import load_object
-from pydiverse.pipedag.util.import_ import import_object
+from pydiverse.pipedag.util.import_ import import_object, load_object
 
 if TYPE_CHECKING:
     from pydiverse.pipedag._typing import T
     from pydiverse.pipedag.backend import BaseLockManager
     from pydiverse.pipedag.context.run_context import StageLockStateHandler
     from pydiverse.pipedag.core import Flow, Stage, Task
     from pydiverse.pipedag.engine.base import OrchestrationEngine
     from pydiverse.pipedag.materialize.metadata import TaskMetadata
 
 import structlog
-from attrs import define, frozen
+from attrs import define, evolve, frozen
 
 
 class BaseContext:
     _context_var: ClassVar[ContextVar]
     _token: Token = None
     _enter_counter: int = 0
     _lock: Lock = Lock()
@@ -129,14 +128,17 @@
     strict_result_get_locking: bool
     ignore_task_version: bool
     instance_id: str  # may be used as database name or locking ID
     stage_commit_technique: StageCommitTechnique
     network_interface: str
     attrs: dict[str, Any]
 
+    # other configuration options
+    ignore_fresh_input: bool = False
+
     @cached_property
     def auto_table(self) -> tuple[type, ...]:
         return tuple(map(import_object, self.config_dict.get("auto_table", ())))
 
     @cached_property
     def auto_blob(self) -> tuple[type, ...]:
         return tuple(map(import_object, self.config_dict.get("auto_blob", ())))
@@ -188,14 +190,18 @@
 
         return PipeDAGStore(
             table=table_store,
             blob=blob_store,
             local_table_cache=local_table_cache,
         )
 
+    def evolve(self, **changes) -> ConfigContext:
+        """Create a new instance with the changes applied; Wrapper for attrs.evolve"""
+        return evolve(self, **changes)
+
     def create_lock_manager(self) -> BaseLockManager:
         return load_object(self.config_dict["lock_manager"])
 
     def create_orchestration_engine(self) -> OrchestrationEngine:
         return load_object(self.config_dict["orchestration"])
 
     def close(self):
@@ -223,15 +229,15 @@
     """
 
     lock_state_handlers: [StageLockStateHandler]
 
     _context_var = ContextVar("stage_lock_context")
 
     def __init__(self):
-        self.logger = structlog.getLogger(module=__name__, cls=self.__class__.__name__)
-        self.logger.info(f"OPEN STAGE LOCK CONTEXT {id(self)}")
+        self.logger = structlog.get_logger(logger_name=type(self).__name__, id=id(self))
+        self.logger.info("Open stage lock context")
         self.lock_state_handlers = []
 
     def close(self):
-        self.logger.info(f"CLOSE STAGE LOCK CONTEXT {id(self)}")
+        self.logger.info("Close stage lock context")
         for lock_state_handler in self.lock_state_handlers:
             lock_state_handler.dispose()
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/context/run_context.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/context/run_context.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
+import dataclasses
 import functools
 import pickle
 import time
 import traceback
 import uuid
 from collections import defaultdict
-from collections.abc import Iterable
-from concurrent.futures import ThreadPoolExecutor
+from concurrent.futures import Future, ThreadPoolExecutor
 from contextlib import contextmanager
 from contextvars import ContextVar
 from enum import Enum
-from threading import Lock
+from threading import Lock, RLock
 from typing import TYPE_CHECKING, Any
 
 import msgpack
 import structlog
 
 from pydiverse.pipedag.context.context import (
     BaseContext,
@@ -91,30 +91,26 @@
         self.stage_state = [StageState.UNINITIALIZED] * num_stages
 
         self.table_names = [set() for _ in range(num_stages)]
         self.blob_names = [set() for _ in range(num_stages)]
 
         self.task_memo: defaultdict[Any, Any] = defaultdict(lambda: MemoState.NONE)
 
-        # deferred table store operations
-        self._thread_pool = ThreadPoolExecutor(
-            max_workers=2  # TODO: make 2 configurable
-        )
-        self._deferred_table_store_ops: dict[
-            int, list[tuple[str, str, Iterable, dict]]
-        ] = {}
-        self._any_stage_changes: dict[int, bool] = {}
-        self._deferred_table_store_op_threads: dict[int, dict[int, tuple]] = {}
+        # DEFERRED TABLE STORE OPERATIONS
+        self.deferred_thread_pool = ThreadPoolExecutor()
+        self.deferred_ts_ops: dict[int, list[DeferredTableStoreOp]] = {}
+        self.deferred_ts_ops_futures: dict[int, list[Future]] = {}
+        self.changed_stages: set[int] = set()
 
         # STATE LOCKS
         self.ref_count_lock = Lock()
         self.stage_state_lock = Lock()
         self.names_lock = Lock()
         self.task_memo_lock = Lock()
-        self.deferred_ops = Lock()
+        self.deferred_ops_lock = RLock()
 
         # LOCKING
         self.lock_manager = config_ctx.create_lock_manager()
         self.lock_handler = StageLockStateHandler(self.lock_manager)
 
         try:
             # If we are inside a StageLockContext, then we shouldn't release any
@@ -145,20 +141,20 @@
         for stage in self.stages:
             for task in stage.all_tasks():
                 for s in task.upstream_stages:
                     self.ref_count[s.id] += 1
 
         self.__context_proxy = RunContext(self)
         self.__context_proxy.__enter__()
-        self._thread_pool.__enter__()
+        self.deferred_thread_pool.__enter__()
         return self.__context_proxy
 
     def __exit__(self, exc_type, exc_val, exc_tb):
-        self._thread_pool.shutdown(wait=True, cancel_futures=True)
-        self._thread_pool.__exit__(exc_type, exc_val, exc_tb)
+        self.deferred_thread_pool.shutdown(wait=True, cancel_futures=True)
+        self.deferred_thread_pool.__exit__(exc_type, exc_val, exc_tb)
         self.__context_proxy.__exit__(exc_type, exc_val, exc_tb)
 
         if not self.keep_stages_locked:
             self.lock_handler.dispose()
 
         super().__exit__(exc_type, exc_val, exc_tb)
 
@@ -169,25 +165,30 @@
             op = getattr(self, op_name)
             if not callable(op) or op_name[0] == "_":
                 raise TypeError(f"OP '{op_name}' is not allowed on RunContextServer")
 
             result = op(*args)
             return [None, result]
         except Exception as e:
-            exception_str = traceback.format_exc()
+            exception_tb = traceback.format_exc()
             try:
-                pickled_exception = pickle.dumps(e)
+                # Add more context to exception
+                exception_with_traceback = Exception(
+                    f"{type(e).__name__}: {e}\n{exception_tb}"
+                )
+                exception_with_traceback.__cause__ = e
+                pickled_exception = pickle.dumps(exception_with_traceback)
             except Exception as e2:
                 self.logger.error(
                     "failed pickling exception",
-                    exception=exception_str,
+                    traceback=exception_tb,
                     pickle_exception=str(e2),
                 )
                 pickled_exception = pickle.dumps(
-                    RuntimeError("failed pickling exception\n" + exception_str)
+                    RuntimeError("failed pickling exception\n" + exception_tb)
                 )
 
             return [pickled_exception, None]
 
     # STAGE: Reference Counting
 
     @synchronized("ref_count_lock")
@@ -213,16 +214,22 @@
             stage_id,
             success,
             StageState.INITIALIZING,
             StageState.READY,
         )
 
     def enter_commit_stage(self, stage_id: int):
-        stage_changed = self._any_stage_changes.get(stage_id, False)
-        self._join_deferred_table_store_ops(stage_id, stage_changed)
+        if self.has_stage_changed(stage_id):
+            self._trigger_deferred_ts_ops(
+                stage_id, DeferredTableStoreOp.Condition.ON_STAGE_COMMIT
+            )
+        else:
+            self.abort_stage(stage_id)
+        self._await_deferred_ts_ops(stage_id)
+
         return self._enter_stage_state_transition(
             stage_id,
             StageState.READY,
             StageState.COMMITTING,
             StageState.COMMITTED,
         )
 
@@ -298,80 +305,85 @@
             stage = self.stages[stage_id]
             self.lock_manager.release(stage)
 
     def validate_stage_lock(self, stage_id: int):
         stage = self.stages[stage_id]
         self.lock_handler.validate_stage_lock(stage)
 
-    # Deferred operations
+    # DEFERRED TABLE STORE OPERATIONS
+    # Allows deferring operations that should be run on the table store object
+    # until certain events occur. This is required to implement deferred copying
+    # of tables from one schema to another.
+
+    @synchronized("deferred_ops_lock")
+    def defer_table_store_op(self, stage_id: int, op: DeferredTableStoreOp):
+        if stage_id not in self.deferred_ts_ops:
+            self.deferred_ts_ops[stage_id] = []
+            self.deferred_ts_ops_futures[stage_id] = []
+        self.deferred_ts_ops[stage_id].append(op)
+
+        if self.has_stage_changed(stage_id):
+            self._trigger_deferred_ts_ops(
+                stage_id, DeferredTableStoreOp.Condition.ON_STAGE_CHANGED
+            )
 
-    @synchronized("deferred_ops")
-    def deferred_table_store_op_if_stage_invalid(
-        self, stage_id: int, op: str, commit_op: str, args, kwargs
+    @synchronized("deferred_ops_lock")
+    def has_stage_changed(self, stage_id: int) -> bool:
+        return stage_id in self.changed_stages
+
+    @synchronized("deferred_ops_lock")
+    def set_stage_has_changed(self, stage_id: int):
+        self.changed_stages.add(stage_id)
+        self._trigger_deferred_ts_ops(
+            stage_id, DeferredTableStoreOp.Condition.ON_STAGE_CHANGED
+        )
+
+    @synchronized("deferred_ops_lock")
+    def _trigger_deferred_ts_ops(
+        self, stage_id: int, condition: DeferredTableStoreOp.Condition
     ):
-        if stage_id not in self._deferred_table_store_ops:
-            self._deferred_table_store_ops[stage_id] = []
-        self._deferred_table_store_ops[stage_id].append((op, commit_op, args, kwargs))
-        if self._any_stage_changes.get(stage_id, False):
-            self._trigger_deferred_table_store_ops(stage_id)
-
-    @synchronized("deferred_ops")
-    def any_stage_changes(self, stage_id: int):
-        return self._any_stage_changes.get(stage_id, False)
-
-    @synchronized("deferred_ops")
-    def stage_output_cache_invalid(self, stage_id: int):
-        if not self._any_stage_changes.get(stage_id, False):
-            self._trigger_deferred_table_store_ops(stage_id)
-        self._any_stage_changes[stage_id] = True
+        # Partition deferred ops into those that should and shouldn't get executed
+        deferred_ts_ops = self.deferred_ts_ops.get(stage_id, [])
 
-    @synchronized("deferred_ops")
-    def abort_stage(self, stage_id: int):
-        return self._join_deferred_table_store_ops(stage_id, stage_changed=False)
+        ops_to_execute = [op for op in deferred_ts_ops if op.condition == condition]
+        remaining_ops = [op for op in deferred_ts_ops if op.condition != condition]
 
-    def _trigger_deferred_table_store_ops(self, stage_id: int):
-        if (
-            stage_id in self._deferred_table_store_ops
-            and len(self._deferred_table_store_ops[stage_id]) > 0
-        ):
-            if len(self._deferred_table_store_op_threads.get(stage_id, {})) == 0:
-                self._deferred_table_store_op_threads[stage_id] = {}
-                started_ops_end = 0
-            else:
-                started_ops_end = (
-                    max(self._deferred_table_store_op_threads[stage_id].keys()) + 1
-                )
-            store = self.config_ctx.store
-            for i, (op, commit_op, args, kwargs) in enumerate(
-                self._deferred_table_store_ops[stage_id][started_ops_end:]
-            ):
-                _id = started_ops_end + i
-                fn = getattr(store.table_store, op)
-                commit_fn = getattr(store.table_store, commit_op)
-                assert callable(fn) and callable(commit_fn)
-                future = self._thread_pool.submit(_call_with_args, fn, args, kwargs)
-                self._deferred_table_store_op_threads[stage_id][_id] = (
-                    future,
-                    commit_fn,
-                    args,
-                    kwargs,
-                )
+        if len(ops_to_execute) == 0:
+            return
 
-    def _join_deferred_table_store_ops(self, stage_id: int, stage_changed: bool):
-        for (
-            future,
-            commit_fn,
-            args,
-            kwargs,
-        ) in self._deferred_table_store_op_threads.get(stage_id, {}).values():
-            if stage_changed:
-                _ = future.result()  # this implies a thread join
-                commit_fn(*args, **kwargs)
-            else:
-                future.cancel()
+        # Trigger ops and store futures
+        store = self.config_ctx.store
+        for op in ops_to_execute:
+            fn = getattr(store.table_store, op.fn_name)
+            assert callable(fn)
+
+            future = self.deferred_thread_pool.submit(
+                _call_with_args, fn, op.args, op.kwargs
+            )
+            self.deferred_ts_ops_futures[stage_id].append(future)
+
+        # Remove ops that just have been executed
+        self.deferred_ts_ops[stage_id] = remaining_ops
+
+    @synchronized("deferred_ops_lock")
+    def _await_deferred_ts_ops(self, stage_id: int):
+        if stage_id not in self.deferred_ts_ops_futures:
+            return
+
+        futures = self.deferred_ts_ops_futures[stage_id]
+        for future in futures:
+            future.result()
+
+    @synchronized("deferred_ops_lock")
+    def abort_stage(self, stage_id: int):
+        self._await_deferred_ts_ops(stage_id)
+        self._trigger_deferred_ts_ops(
+            stage_id, DeferredTableStoreOp.Condition.ON_STAGE_ABORT
+        )
+        self._await_deferred_ts_ops(stage_id)
 
     # TASK
 
     def did_finish_task(self, task_id: int, final_state_value: int):
         # TODO: Do something with the final state.
         #       For example: The object returned by flow.run could have a list
         #       of tasks and their final states.
@@ -498,17 +510,14 @@
     _context_var = ContextVar("run_context_proxy")
 
     def __init__(self, server: RunContextServer):
         self.client = server.get_client()
         self.flow = server.flow
         self.run_id = server.run_id
 
-        # Configuration Options
-        self.ignore_fresh_input = False
-
     def _request(self, op: str, *args):
         error, result = self.client.request([op, args])
 
         if error is not None:
             raise RemoteProcessError("Request failed") from pickle.loads(error)
         return result
 
@@ -562,14 +571,28 @@
 
     def release_stage_lock(self, stage: Stage):
         self._request("release_stage_lock", stage.id)
 
     def validate_stage_lock(self, stage: Stage):
         self._request("validate_stage_lock", stage.id)
 
+    # DEFERRED TABLE STORE OPERATIONS
+
+    def defer_table_store_op(self, stage: Stage, op: DeferredTableStoreOp):
+        """Defer running a table store operation until a specific stage event"""
+        return self._request("defer_table_store_op", stage.id, op)
+
+    def has_stage_changed(self, stage: Stage) -> bool:
+        """Check if a stage has changed and still is 100% cache valid"""
+        return self._request("has_stage_changed", stage.id)
+
+    def set_stage_has_changed(self, stage: Stage):
+        """Inform the run context that a stage isn't 100% cache valid anymore"""
+        return self._request("set_stage_has_changed", stage.id)
+
     # TASK
 
     def did_finish_task(self, task: Task, final_state: FinalTaskState):
         self._request("did_finish_task", task.id, final_state.value)
 
     @contextmanager
     def task_memo(self, task: Task, cache_key: str):
@@ -607,35 +630,14 @@
         self._request(
             "remove_names",
             stage.id,
             [t.name for t in tables],
             [b.name for b in blobs],
         )
 
-    def deferred_table_store_op_if_stage_invalid(
-        self, stage: Stage, op: str, commit_op: str, *args, **kwargs
-    ):
-        self._request(
-            "deferred_table_store_op_if_stage_invalid",
-            stage.id,
-            op,
-            commit_op,
-            args,
-            kwargs,
-        )
-
-    def any_stage_changes(self, stage):
-        return self._request("any_stage_changes", stage.id)
-
-    def abort_stage(self, stage):
-        return self._request("abort_stage", stage.id)
-
-    def stage_output_cache_invalid(self, stage):
-        return self._request("stage_output_cache_invalid", stage.id)
-
 
 class DematerializeRunContext(BaseContext):
     """Dummy RunContext that returns `COMMITTED` as the stage state for all stages
 
     To dematerialize an object we must know it the associates state has been
     committed or not. This context replaces the RunContext created by
     RunContextServer during the execution of a flow with one that only sets the
@@ -658,15 +660,15 @@
 class StageLockStateHandler(Disposable):
     """
     Handle LockState changes (i.e. locks that may become UNCERTAIN
     or externally UNLOCKED).
     """
 
     def __init__(self, lock_manager: BaseLockManager):
-        self.logger = structlog.get_logger(cls=type(self).__name__)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
         self.lock_manager = lock_manager
         self.lock_manager.add_lock_state_listener(self._lock_state_listener)
 
     def dispose(self):
         self.logger.debug("Disposing of StageLockStateHandler")
         self.lock_manager.dispose()
         super().dispose()
@@ -745,27 +747,46 @@
 class MemoState(Enum):
     NONE = 0
     WAITING = 1
 
     FAILED = 127
 
 
+# Deferred Table Store operations
+
+
+@dataclasses.dataclass
+class DeferredTableStoreOp:
+    class Condition(Enum):
+        ON_STAGE_CHANGED = 0
+        """Some table produced in the stage is determined to be cache invalid"""
+
+        ON_STAGE_ABORT = 1
+        """The stage has finished running and all tables are still cache valid"""
+
+        ON_STAGE_COMMIT = 2
+        """The stage has finished running and some tables weren't cache valid"""
+
+    fn_name: str
+    condition: Condition
+    args: tuple | list = ()
+    kwargs: dict = dataclasses.field(default_factory=dict)
+
+
 # msgpack hooks
 # Only used to transmit Table and Blob type metadata
 
 
 def _msg_default(obj):
-    # some table implementations are not picklable
-    if hasattr(obj, "obj"):
-        save = obj.obj
-        obj.obj = None
-        ret = pickle.dumps(obj)
-        obj.obj = save
-    else:
+    try:
         ret = pickle.dumps(obj)
+    except Exception as e:
+        logger = structlog.get_logger(logger_name="RunContext msg_default")
+        logger.exception("failed to pickle object", object=obj)
+        raise e
     return msgpack.ExtType(0, ret)
 
 
 def _msg_ext_hook(code, data):
     if code == 0:
         return pickle.loads(data)
     return msgpack.ExtType(code, data)
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/flow.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/flow.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,31 +3,31 @@
 from collections import defaultdict
 from typing import TYPE_CHECKING
 
 import networkx as nx
 import structlog
 
 from pydiverse.pipedag.context import ConfigContext, DAGContext, RunContextServer
+from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.errors import DuplicateNameError, FlowError
-from pydiverse.pipedag.util.config import PipedagConfig
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core import Result, Stage, Task
     from pydiverse.pipedag.core.stage import CommitStageTask
     from pydiverse.pipedag.engine import OrchestrationEngine
 
 
 class Flow:
     def __init__(
         self,
         name: str = "default",
     ):
         self.name = name
 
-        self.logger = structlog.getLogger(module=__name__, cls=self.__class__.__name__)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
         self.stages: dict[str, Stage] = {}
         self.tasks: list[Task] = []
 
         self.graph = nx.DiGraph()
         self.explicit_graph: nx.DiGraph | None = None
 
     def __enter__(self):
@@ -241,20 +241,25 @@
         # Get the ConfigContext to use
         if config_context is None:
             try:
                 config_context = ConfigContext.get()
             except LookupError:
                 config_context = PipedagConfig.default.get()
 
-        with config_context, RunContextServer(self) as run_context:
-            # Configure Run Context
-            run_context.ignore_fresh_input = ignore_fresh_input
+        # Evolve config using the arguments passed to flow.run
+        config_context = config_context.evolve(
+            fail_fast=(
+                fail_fast if fail_fast is not None else config_context.fail_fast
+            ),
+            ignore_fresh_input=ignore_fresh_input,
+        )
 
+        with config_context, RunContextServer(self):
             if orchestration_engine is None:
                 orchestration_engine = config_context.create_orchestration_engine()
             result = orchestration_engine.run(flow=self, **kwargs)
 
-        fail_fast = config_context.fail_fast if fail_fast is None else fail_fast
+        fail_fast = config_context.fail_fast
         if not result.successful and fail_fast:
             raise result.exception or Exception("Flow run failed")
 
         return result
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/result.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/result.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         :param task: The task
         :param as_type: The type as which tables produced by this task should
             be dematerialized. If no type is specified, the input type of
             the task is used.
         :return: The results of the task.
         """
         if not self.successful:
-            logger = structlog.getLogger()
+            logger = structlog.get_logger(logger_name=type(self).__name__)
             logger.warning(
                 "Attention: getting tables from unsuccessful run is unreliable!"
             )
 
         if isinstance(task, Task):
             root_task = task
         else:
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/stage.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/stage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import structlog
 
-from pydiverse.pipedag.context import ConfigContext, DAGContext, RunContext
+from pydiverse.pipedag.context import ConfigContext, DAGContext
 from pydiverse.pipedag.core.task import Task
 from pydiverse.pipedag.errors import StageError
 from pydiverse.pipedag.util import normalize_name
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core.flow import Flow
 
@@ -58,15 +58,15 @@
         self._name = normalize_name(name)
         self._transaction_name = f"{self._name}__tmp"
 
         self.tasks: list[Task] = []
         self.commit_task: CommitStageTask = None  # type: ignore
         self.outer_stage: Stage | None = None
 
-        self.logger = structlog.get_logger(stage=self)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__, stage=self)
         self.id: int = None  # type: ignore
 
         self._did_enter = False
 
     @property
     def name(self) -> str:
         return self._name
@@ -166,16 +166,15 @@
         )
 
         self.stage = stage
         self.flow = flow
         self.upstream_stages = {stage}
         self.input_tasks = {}
 
+        self.logger = self.logger.bind(logger_name="Commit Stage", stage=stage)
+
         self._bound_args = self._signature.bind()
         self._visualize_hidden = True
 
     def fn(self):
-        self.logger.info(f"Committing stage '{self.stage.name}'")
-        if RunContext.get().any_stage_changes(self.stage):
-            ConfigContext.get().store.commit_stage(self.stage)
-        else:
-            RunContext.get().abort_stage(self.stage)
+        self.logger.info("Committing stage")
+        ConfigContext.get().store.commit_stage(self.stage)
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/core/task.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/task.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.stage: Stage = None  # type: ignore
         self.upstream_stages: list[Stage] = None  # type: ignore
         self.input_tasks: dict[int, Task] = None  # type: ignore
 
         self._signature = inspect.signature(fn)
         self._bound_args: inspect.BoundArguments = None  # type: ignore
 
-        self.logger = structlog.get_logger()
+        self.logger = structlog.get_logger(logger_name=f"Task '{self.name}'", task=self)
         self._visualize_hidden = False
 
     def __repr__(self):
         return f"<Task '{self.name}' {hex(id(self))} (id: {self.id})>"
 
     def __hash__(self):
         return id(self)
@@ -84,15 +84,15 @@
 
         if ctx.stage is None:
             raise StageError("Can't call pipedag task outside of a stage.")
 
         new = copy.copy(self_)
         new.flow = ctx.flow
         new.stage = ctx.stage
-        new.logger = structlog.get_logger(task=new)
+        new.logger = new.logger.bind(logger_name=f"Task '{new.name}'", task=new)
 
         new._bound_args = new._signature.bind(*args, **kwargs)
 
         new.flow.add_task(new)
         new.stage.tasks.append(new)
 
         # Compute input tasks
@@ -132,14 +132,15 @@
         if config_context is None:
             config_context = ConfigContext.get()
 
         with run_context, config_context:
             try:
                 result = self._run(inputs)
             except Exception as e:
+                self.logger.exception("Task failed (raised an exception)")
                 self.did_finish(FinalTaskState.FAILED)
                 raise e
             else:
                 self.did_finish(FinalTaskState.COMPLETED)
                 return result
 
     def _run(self, inputs: [int, Any]):
@@ -162,17 +163,15 @@
         with TaskContext(task=self):
             result = self.fn(*args, **kwargs)
 
         return result
 
     def did_finish(self, state: FinalTaskState):
         if state == FinalTaskState.COMPLETED:
-            self.logger.info("Task finished successfully", task=self, state=state)
-        else:
-            self.logger.warning("Task failed", task=self, state=state)
+            self.logger.info("Task finished successfully", state=state)
         RunContext.get().did_finish_task(self, state)
 
     def resolve_value(self, task_value: Any):
         return task_value
 
 
 class TaskGetItem:
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/base.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/base.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/prefect.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/prefect.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/engine/sequential.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/engine/sequential.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/errors/__init__.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/cache.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/cache.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,18 +125,15 @@
                     cache_metadata.cache_fn_hash,
                     task_cache_key,
                     cached_output,
                     cache_metadata,
                     _is_cache_valid=True,
                 )
             except CacheError as e:
-                task.logger.info(
-                    "Failed to retrieve task from cache.",
-                    exception=str(e),
-                )
+                task.logger.info("Failed to retrieve task from cache", cause=str(e))
         else:
             if not task.lazy:
                 # choose a deliberately random version since caching was disabled
                 task = copy.deepcopy(task)
                 task.version = uuid.uuid4().hex
         new_task_cache_key = CacheManager.task_cache_key(
             task, input_hash, cache_fn_hash
@@ -164,20 +161,21 @@
             # Try retrieving the table from the cache and then copying it
             # to the transaction stage
             metadata = store.retrieve_lazy_table_metadata(
                 query_hash, task_hash, table.stage
             )
             store.copy_lazy_table_to_transaction(metadata, table)
             store.logger.info(f"Lazy cache of table '{table.name}' found")
-            table.name = metadata.name
             is_cache_valid = True
         except CacheError as e:
             # Either not found in cache, or copying failed
             # -> Store using default method
-            store.logger.warning("cache miss", table=table.name, exception=str(e))
+            store.logger.warning(
+                "Cache miss", table=table.name, stage=table.stage.name, cause=str(e)
+            )
             is_cache_valid = False
 
         # Store metadata
         store.store_lazy_table_metadata(
             LazyTableMetadata(
                 name=table.name,
                 stage=table.stage.name,
@@ -204,15 +202,15 @@
             )
             store.copy_raw_sql_tables_to_transaction(metadata, raw_sql.stage)
             store.logger.info(f"Lazy cache of stage '{raw_sql.stage}' found")
             is_cache_valid = True
         except CacheError as e:
             # Either not found in cache, or copying failed
             # -> Store using default method
-            store.logger.warning("cache miss for raw-SQL", exception=str(e))
+            store.logger.warning("Cache miss for raw-SQL", cause=str(e))
             is_cache_valid = False
         return TableCacheInfo(raw_sql.stage, task_hash, query_hash, is_cache_valid)
 
     @staticmethod
     def task_cache_key(task: MaterializingTask, input_hash: str, cache_fn_hash: str):
         """Cache key used to judge cache validity of the current task output.
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/container.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/container.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import copy
 from typing import TYPE_CHECKING, Any, Generic
 
 from pydiverse.pipedag._typing import T
 from pydiverse.pipedag.util import normalize_name
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.core.stage import Stage
@@ -37,14 +38,29 @@
         self.obj = obj
         self.name = name
         self.stage = stage
         self.primary_key = primary_key
         self.indexes = indexes
         self.type_map = type_map
 
+        # Check that indexes is of type list[list[str]]
+        indexes_type_error = TypeError(
+            "Table argument 'indexes' must be of type list[list[str]]. "
+            "Make sure you provide a 2d list, not just a 1d list."
+        )
+        if self.indexes is not None:
+            if not isinstance(self.indexes, (list, tuple)):
+                raise indexes_type_error
+            for index in self.indexes:
+                if not isinstance(index, (list, tuple)):
+                    raise indexes_type_error
+                for col in index:
+                    if not isinstance(col, str):
+                        raise indexes_type_error
+
         # cache_key will be overridden shortly before handing over to downstream tasks
         # that use it to compute their input_hash for cache_invalidation due to input
         # change
         self.cache_key = None
 
     def __str__(self):
         return f"<Table: {self.name} ({self.stage.name})>"
@@ -55,14 +71,28 @@
 
     @name.setter
     def name(self, value):
         if value is not None and not isinstance(value, str):
             raise TypeError(f"Table name must be of instance 'str' not {type(value)}.")
         self._name = normalize_name(value)
 
+    def copy_without_obj(self) -> Table:
+        obj = self.obj
+        self.obj = None
+        self_copy = copy.deepcopy(self)
+        self.obj = obj
+        return self_copy
+
+    def __getstate__(self):
+        # The table `obj` field can't necessarily be pickled. That's why we remove it
+        # from the state before pickling.
+        state = self.__dict__.copy()
+        state["obj"] = None
+        return state
+
 
 class RawSql:
     """Container for raw sql strings
 
     This allows wrapping legacy sql code with pipedag before it is converted
     to proper tasks that allow tracing tables.
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/core.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -193,16 +193,14 @@
                 ctx = RunContext.get()
                 if task_cache_info.is_cache_valid():
                     ctx.store_task_memo(
                         task, memo_cache_key, task_cache_info.get_cached_output()
                     )
                     # Task isn't lazy -> copy cache to transaction stage
                     return task_cache_info.get_cached_output()
-                else:
-                    ctx.stage_output_cache_invalid(task.stage)
 
             # Not found in cache / lazy -> Evaluate Function
             args, kwargs, input_tables = store.dematerialize_task_inputs(
                 task, bound.args, bound.kwargs
             )
 
             result = self.fn(*args, **kwargs)
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/metadata.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/metadata.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/store.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
-import copy
 import itertools
 import json
 from typing import Any, Callable
 
 import structlog
 
 from pydiverse.pipedag import Blob, Stage, Table, backend
 from pydiverse.pipedag._typing import Materializable, T
 from pydiverse.pipedag.context import ConfigContext, RunContext
 from pydiverse.pipedag.context.run_context import StageState
+from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.errors import DuplicateNameError, StageError
 from pydiverse.pipedag.materialize.container import RawSql
 from pydiverse.pipedag.materialize.core import MaterializingTask, TaskInfo
 from pydiverse.pipedag.materialize.metadata import TaskMetadata
 from pydiverse.pipedag.materialize.util import json as json_util
 from pydiverse.pipedag.util import Disposable, deep_map
-from pydiverse.pipedag.util.config import PipedagConfig
 from pydiverse.pipedag.util.naming import NameDisambiguator
 
 
 class PipeDAGStore(Disposable):
     """Main storage interface for materializing tasks
 
     Depending on the use case, the store can be configured using different
@@ -123,15 +122,15 @@
             ctx.validate_stage_lock(item.stage)
             if self.local_table_cache.has_cache_table(item, as_type):
                 return self.local_table_cache.retrieve_table_obj(item, as_type, namer)
             else:
                 obj = self.table_store.retrieve_table_obj(
                     item, as_type=as_type, namer=namer
                 )
-                table = copy.deepcopy(item)
+                table = item.copy_without_obj()
                 table.obj = obj
                 self.local_table_cache.store_table(
                     table, task=None, task_info=None, is_input=True
                 )
                 return obj
         elif isinstance(item, Blob):
             ctx.validate_stage_lock(item.stage)
@@ -242,14 +241,15 @@
                     # - If no name has been provided, generate on automatically
                     # - If the provided name ends with %%, perform name mangling
                     object_number = next(auto_suffix_counter)
                     auto_suffix = (
                         f"{task_info.task_cache_info.get_task_cache_key()}"
                         f"_{object_number:04d}"
                     )
+
                     if x.name is None:
                         x.name = task.name + "_" + auto_suffix
                     elif x.name.endswith("%%"):
                         x.name = x.name[:-2] + auto_suffix
 
                 ctx.validate_stage_lock(stage)
                 if isinstance(x, Table):
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/cache.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/cache.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/materialize/util/json.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/materialize/util/json.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 from __future__ import annotations
 
 import datetime as dt
 from pathlib import Path
 
 from pydiverse.pipedag import Stage
 from pydiverse.pipedag.context import RunContext
+from pydiverse.pipedag.core.config import PipedagConfig
 from pydiverse.pipedag.materialize.container import Blob, RawSql, Table
-from pydiverse.pipedag.util.config import PipedagConfig
 
 PIPEDAG_TYPE = "_pipedag_type_"
 PIPEDAG_TYPE_TABLE = "table"
 PIPEDAG_TYPE_RAWSQL = "raw_sql"
 PIPEDAG_TYPE_BLOB = "blob"
 PIPEDAG_TYPE_STAGE = "stage"
 PIPEDAG_TYPE_PIPEDAG_CONFIG = "pipedag_config"
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/config.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/core/config.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from __future__ import annotations
 
 import copy
 import getpass
 import itertools
-import logging
 import os
 import re
-import sys
 from collections.abc import Iterable
 from pathlib import Path
 from typing import TYPE_CHECKING, Any
 
-import structlog
 import yaml
 from box import Box
 
 from pydiverse.pipedag.util.deep_merge import deep_merge
-from pydiverse.pipedag.util.import_ import import_object
 
 if TYPE_CHECKING:
     from pydiverse.pipedag.context import ConfigContext
 
 
 # noinspection PyPep8Naming
 class cached_class_property:
@@ -369,53 +365,14 @@
                 f"Could not find variable '{name}' referenced in '{string}'."
             )
         return str(variables[name])
 
     return re.sub(r"\{[a-zA-Z_]+[a-zA-Z0-9_]*\}", var_sub, string)
 
 
-def load_object(config_dict: dict):
-    """Instantiates an instance of an object given
-
-    The import path (module.Class) should be specified as the "class" value
-    of the dict. The args section of the dict get used as the instance config.
-
-    If the class defines a `_init_conf_` function, it gets called using the
-    config values, otherwise they just get passed to the class initializer.
-
-    >>> # module.Class(argument="value")
-    >>> load_object({
-    >>>     "class": "module.Class",
-    >>>     "args": {
-    >>>         "argument": "value",
-    >>>     },
-    >>> })
-    """
-
-    if "class" not in config_dict:
-        raise RuntimeError(
-            "Attribute 'class' is missing in configuration "
-            "section that supports multiple backends\n"
-            f"config section: {config_dict}"
-        )
-    cls = import_object(config_dict["class"])
-
-    args = config_dict.get("args", {})
-    if not isinstance(args, dict):
-        raise TypeError(
-            f"Invalid type for args section: {type(args)}\n"
-            f"config section: {config_dict}"
-        )
-    try:
-        init_conf = cls._init_conf_
-        return init_conf(args)
-    except AttributeError:
-        return cls(**args)
-
-
 # Nested Dictionary Utilities
 
 
 def _flatten(items):
     for x in items:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from _flatten(x)
@@ -453,33 +410,7 @@
         for p in path[:-1]:
             d = d[p]
         return d.pop(path[-1])
     except KeyError as e:
         if default == _nil:
             raise e
         return default
-
-
-def setup_structlog(
-    _log_level=logging.INFO,
-    _log_stream=sys.stderr,
-    timestamp_format="%Y-%m-%d %H:%M:%S.%f",
-):
-    logging.basicConfig(
-        stream=_log_stream,
-        format="%(asctime)s [%(levelname)s] %(message)s",
-        level=_log_level,
-    )
-    structlog.configure(
-        processors=[
-            structlog.contextvars.merge_contextvars,
-            structlog.processors.add_log_level,
-            structlog.processors.StackInfoRenderer(),
-            structlog.dev.set_exc_info,
-            structlog.processors.TimeStamper(fmt=timestamp_format),
-            structlog.dev.ConsoleRenderer(),
-        ],
-        wrapper_class=structlog.make_filtering_bound_logger(_log_level),
-        context_class=dict,
-        logger_factory=structlog.PrintLoggerFactory(_log_stream),
-        cache_logger_on_first_use=True,
-    )
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_map.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_map.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/deep_merge.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/deep_merge.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/disposable.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/disposable.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/ipc.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/ipc.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,23 +7,19 @@
 import uuid
 from functools import cached_property
 from typing import Any
 
 import msgpack
 import pynng
 import structlog
+from cryptography.fernet import Fernet
 
 from pydiverse.pipedag.errors import IPCError
 
 
-def human_thread_id(thread_ident):
-    """Return human processable number for thread ID."""
-    return hash(thread_ident) % 100
-
-
 class IPCServer(threading.Thread):
     """Server for inter process communication
 
     FORMAT:
         REQUEST: [nonce, payload]
         RESPONSE: [payload]
     """
@@ -39,50 +35,48 @@
         # Reduce recv_timeout when running pytest for better performance
         is_running_pytest = "PYDIVERSE_PIPEDAG_PYTEST" in os.environ
         recv_timeout = 200 if not is_running_pytest else 10
 
         self.socket = pynng.Rep0(listen=listen, recv_timeout=recv_timeout)
         self.nonces = set()
 
+        self._fernet = Fernet(Fernet.generate_key())
+
         self.__stop_flag = False
         self.__thread = None
-        self.logger = structlog.get_logger(cls=type(self).__name__)
+        self.logger = structlog.get_logger(logger_name=type(self).__name__)
 
         self.msg_default = msg_default
         self.msg_ext_hook = msg_ext_hook
 
     def _get_id(self, ctx_id=0):
         return dict(
             address=self.address,
-            thread=human_thread_id(threading.get_ident()),
+            thread=threading.get_ident(),
             ctx_id=ctx_id,
         )
 
     def run(self):
-        self.logger.info("start IPCServer", **self._get_id())
+        self.logger.info("Starting IPCServer", **self._get_id())
         self.run_loop()
 
     def stop(self):
         self.__stop_flag = True
-        self.logger.debug("request IPCServer to stop", **self._get_id())
+        self.logger.debug("Request IPCServer to stop", **self._get_id())
 
     def __enter__(self):
         self.__thread = self
         self.__thread.start()
-        self.logger.debug(
-            "started IPCServer thread", thread=human_thread_id(self.__thread.ident)
-        )
+        self.logger.debug("Started IPCServer thread", thread=self.__thread.ident)
         return self
 
     def __exit__(self, exc_type, exc_val, exc_tb):
         self.stop()
         if self.__thread is not None:
-            self.logger.debug(
-                "stop IPCServer thread", thread=human_thread_id(self.__thread.ident)
-            )
+            self.logger.debug("Stop IPCServer thread", thread=self.__thread.ident)
             self.__thread.join()
 
     def run_loop(self):
         """
         Run main loop for responding to client requests to this server process.
 
         We rely on a fixed request-response pattern of pynng library (Req0/Rep0)
@@ -97,19 +91,20 @@
 
         socket = None
         ctx_id = 0
         threads = []
         try:
             socket = self.socket.new_context()
             ctx_id += 1
-            self.logger.debug("new socket context", **self._get_id(ctx_id))
+            self.logger.debug("New socket context", **self._get_id(ctx_id))
             while not self.__stop_flag:
                 # noinspection PyBroadException
                 try:
                     data = socket.recv()
+                    data = self._fernet.decrypt(data)
                     unpacker = msgpack.Unpacker(
                         use_list=False, ext_hook=self.msg_ext_hook
                     )
                     unpacker.feed(data)
 
                     # Expected: (NONCE, PAYLOAD)
                     if unpacker.read_array_header() != 2:
@@ -125,71 +120,75 @@
                         self.logger.warning(
                             "Already processing request",
                             nonce=nonce_hex,
                             **self._get_id(ctx_id),
                         )
                         socket = self.socket.new_context()
                         ctx_id += 1
-                        self.logger.debug("next socket context", **self._get_id(ctx_id))
+                        self.logger.debug("Next socket context", **self._get_id(ctx_id))
                         continue
 
                     self.nonces.add(nonce)
 
                     if len(threads) >= max_threads_in_flight:
-                        self.logger.debug(
-                            "joining thread", thread=human_thread_id(threads[0].ident)
-                        )
+                        self.logger.debug("Joining thread", thread=threads[0].ident)
                         threads[0].join()
                         del threads[0]
-                    thread_logger = structlog.get_logger()
+                    thread_logger = structlog.get_logger(
+                        logger_name="IPC Worker", nonce=nonce_hex, ctx_id=ctx_id
+                    )
                     thread = threading.Thread(
                         name="IPC Worker",
                         target=self._serve,
-                        args=[thread_logger, socket, unpacker, nonce_hex, ctx_id],
+                        args=[thread_logger, socket, unpacker],
                         daemon=True,
                     )
                     socket = self.socket.new_context()
                     ctx_id += 1
                     self.logger.debug("next socket context", **self._get_id(ctx_id))
                     threads.append(thread)
                     thread.start()
                 except pynng.Timeout:
                     pass
                 except Exception:
-                    self.logger.exception("exception occurred in run_loop")
+                    self.logger.exception("Exception occurred in run_loop")
         finally:
             for thread in threads:
-                self.logger.debug(
-                    "joining thread", thread=human_thread_id(thread.ident)
-                )
+                self.logger.debug("Joining thread", thread=thread.ident)
                 thread.join()
-            self.logger.debug("closing socket", **self._get_id())
+            self.logger.debug("Closing socket", **self._get_id())
             if socket is not None:
                 socket.close()  # close the open request-response context
             self.socket.close()
-            self.logger.info("stopped IPCServer", **self._get_id())
+            self.logger.info("Stopped IPCServer", **self._get_id())
 
-    def _serve(self, thread_logger, socket, unpacker, nonce_hex, ctx_id):
-        msg = unpacker.unpack()
-        thread_logger.debug(
-            "IPCServer Received",
-            message=msg,
-            nonce=nonce_hex,
-            ctx_id=ctx_id,
-            thread=human_thread_id(threading.get_ident()),
-        )
-        reply = self.handle_request(msg)
-        thread_logger.debug(
-            "IPCServer Reply",
-            reply=reply,
-            nonce=nonce_hex,
-            ctx_id=ctx_id,
-            thread=human_thread_id(threading.get_ident()),
-        )
-        socket.send(msgpack.packb(reply, default=self.msg_default))
+    def _serve(self, thread_logger, socket: pynng.Socket, unpacker):
+        try:
+            msg = unpacker.unpack()
+            thread_logger.debug(
+                "IPCServer Received",
+                message=msg,
+                thread=threading.get_ident(),
+            )
+            reply = self.handle_request(msg)
+            thread_logger.debug(
+                "IPCServer Reply",
+                reply=reply,
+                thread=threading.get_ident(),
+            )
+            reply = msgpack.packb(reply, default=self.msg_default)
+            reply = self._fernet.encrypt(reply)
+        except Exception as e:
+            thread_logger.critical("Uncaught exception in _serve", exc_info=e)
+            reply = b""
+
+        try:
+            socket.send(reply)
+        except Exception:
+            thread_logger.exception("Failed to send reply")
 
     def handle_request(self, request: dict[str, Any]):
         return None
 
     @cached_property
     def address(self) -> str:
         address = self.socket.listeners[0].local_address
@@ -207,57 +206,63 @@
             return f"tcp://{ip.exploded}:{port}"
         else:
             return f"tcp://[{ip}]:{port}"
 
     def get_client(self) -> IPCClient:
         return IPCClient(
             addr=self.address,
+            fernet=self._fernet,
             msg_default=self.msg_default,
             msg_ext_hook=self.msg_ext_hook,
         )
 
 
 class IPCClient:
-    def __init__(self, addr: str, msg_default=None, msg_ext_hook=None):
+    def __init__(self, addr: str, fernet: Fernet, msg_default=None, msg_ext_hook=None):
         self.logger = structlog.get_logger(
-            thread=human_thread_id(threading.get_ident())
+            logger_name=type(self).__name__,
+            thread=threading.get_ident(),
         )
         self.addr = addr
-        self.socket = self._connect()
-
+        self._fernet = fernet
         self.msg_default = msg_default
         self.msg_ext_hook = msg_ext_hook
 
+        self.socket = self._connect()
+
     def _connect(self):
-        self.logger.debug("opening client connection", addr=self.addr)
+        self.logger.debug("Opening client connection", addr=self.addr)
         return pynng.Req0(dial=self.addr, resend_time=30_000)
 
     def request(self, payload: Any) -> Any:
         with self.socket.new_context() as socket:
-            self.logger.debug("client request")
-            nonce = uuid.uuid4().bytes[:8]
+            self.logger.debug("Client request")
+            nonce = uuid.uuid4().bytes[:16]
             msg = msgpack.packb((nonce, payload), default=self.msg_default)
+            msg = self._fernet.encrypt(msg)
             socket.send(msg)
 
-            response_msg = socket.recv()
-            self.logger.debug("client got response")
+            response = socket.recv()
+            self.logger.debug("Client got response")
+            response = self._fernet.decrypt(response)
             response = msgpack.unpackb(
-                response_msg, use_list=False, ext_hook=self.msg_ext_hook
+                response, use_list=False, ext_hook=self.msg_ext_hook
             )
             return response
 
     def __getstate__(self):
         state = self.__dict__.copy()
         del state["socket"]
-        del state["logger"]
         return state
 
     def __setstate__(self, state):
         self.__dict__.update(state)
-        self.logger = structlog.get_logger(threading.get_ident())
+        self.logger = self.logger.bind(
+            thread=threading.get_ident(),
+        )
         self.socket = self._connect()
 
 
 if __name__ == "__main__":
     with IPCServer() as serv:
         client = serv.get_client()
         client.request(["This is a test"])
```

### Comparing `pydiverse-pipedag-0.3.0/src/pydiverse/pipedag/util/naming.py` & `pydiverse_pipedag-0.4.0/src/pydiverse/pipedag/util/naming.py`

 * *Files identical despite different names*

### Comparing `pydiverse-pipedag-0.3.0/PKG-INFO` & `pydiverse_pipedag-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,61 +1,41 @@
 Metadata-Version: 2.1
 Name: pydiverse-pipedag
-Version: 0.3.0
+Version: 0.4.0
 Summary: A pipeline orchestration library executing tasks within one python session. It takes care of SQL table (de)materialization, caching and cache invalidation. Blob storage is supported as well for example for storing model files.
 License: BSD-3-Clause
 Author: QuantCo, Inc.
-Requires-Python: >=3.9,<3.11
+Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: SQL
 Classifier: Topic :: Database
-Provides-Extra: docs
 Provides-Extra: filelock
-Provides-Extra: ibis
-Provides-Extra: ibm_db2
-Provides-Extra: mssql
-Provides-Extra: pdtransform
-Provides-Extra: polars
-Provides-Extra: prefect
 Provides-Extra: zookeeper
 Requires-Dist: PyYAML (>=6.0)
 Requires-Dist: SQLAlchemy (>=1.4.39)
-Requires-Dist: Sphinx (>=5.1.1); extra == "docs"
 Requires-Dist: attrs (>=22.1.0)
-Requires-Dist: connectorx (>=0.3.1); extra == "polars"
-Requires-Dist: filelock (>=3.7.1); extra == "filelock"
-Requires-Dist: ibis (>=3.2.0); extra == "ibis"
-Requires-Dist: ibis-framework[postgres,mssql] (>=5.1.0,<6.0.0); extra == "ibis"
-Requires-Dist: ibm-db (>=3.1.4); extra == "ibm_db2"
-Requires-Dist: ibm-db-sa (>=0.3.8); extra == "ibm_db2"
-Requires-Dist: kazoo (>=2.8.0); extra == "zookeeper"
+Requires-Dist: cryptography (>=41.0.1)
+Requires-Dist: filelock (>=3.7.1) ; extra == "filelock"
+Requires-Dist: kazoo (>=2.8.0) ; extra == "zookeeper"
 Requires-Dist: msgpack (>=1.0.4)
 Requires-Dist: networkx (>=2.8)
 Requires-Dist: packaging (>=21.3)
 Requires-Dist: pandas (>=1.4.3)
-Requires-Dist: polars (>=0.16.18,<0.17); extra == "polars"
-Requires-Dist: prefect (>=1.3,<2); extra == "prefect"
 Requires-Dist: pyarrow (>=11.0.0)
-Requires-Dist: pydiverse-transform (>=0.1.1); extra == "pdtransform"
 Requires-Dist: pynng (>=0.7.1)
-Requires-Dist: pyodbc (>=4.0.35); extra == "mssql"
 Requires-Dist: python-box (>=6.1.0)
-Requires-Dist: pytsql (>=1.1.4); extra == "mssql"
-Requires-Dist: sphinx-rtd-theme (>=1.0.0); extra == "docs"
-Requires-Dist: sphinxcontrib-apidoc (>=0.3.0); extra == "docs"
 Requires-Dist: structlog (>=22.1.0)
-Requires-Dist: tidypolars (>=0.2.19); extra == "polars"
-Requires-Dist: tomli (>=2.0.1)
-Requires-Dist: typing-extensions (>=4.1.0,<5)
+Requires-Dist: typing-extensions (>=4.1.0,<5.0.0)
 Description-Content-Type: text/markdown
 
 # pydiverse.pipedag
 
 [![CI](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml/badge.svg)](https://github.com/pydiverse/pydiverse.pipedag/actions/workflows/ci.yml)
 
 A pipeline orchestration library executing tasks within one python session. It takes care of SQL table
@@ -77,15 +57,14 @@
 
 ```python
 from pydiverse.pipedag import materialize, Table, Flow, Stage
 import sqlalchemy as sa
 import pandas as pd
 
 from pydiverse.pipedag.context import StageLockContext, RunContext
-from pydiverse.pipedag.util import setup_structlog
 
 
 @materialize(lazy=True)
 def lazy_task_1():
     return sa.select([sa.literal(1).label("x"), sa.literal(2).label("y")])
 
 
@@ -152,16 +131,14 @@
     with StageLockContext():
         result = f.run()
         assert result.successful
         assert result.get(lazy_1, as_type=pd.DataFrame)["x"][0] == 1
 
 
 if __name__ == "__main__":
-    # initialize logging
-    setup_structlog()
     main()
 ```
 
 Create a file called `pipedag.yaml` in the same directory:
 
 ```yaml
 name: pipedag_tests
```

