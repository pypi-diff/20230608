# Comparing `tmp/dbsamizdapper-0.0.4.tar.gz` & `tmp/dbsamizdapper-0.0.5a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbsamizdapper-0.0.4.tar", max compression
+gzip compressed data, was "dbsamizdapper-0.0.5a0.tar", max compression
```

## Comparing `dbsamizdapper-0.0.4.tar` & `dbsamizdapper-0.0.5a0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    32474 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/LICENSE.txt
--rw-r--r--   0        0        0     1444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/README.md
--rw-r--r--   0        0        0      338 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/__init__.py
--rw-r--r--   0        0        0     1699 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/api.py
--rw-r--r--   0        0        0     5154 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/apps.py
--rw-r--r--   0        0        0     1721 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/django_api.py
--rw-r--r--   0        0        0     2806 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/exceptions.py
--rw-r--r--   0        0        0     2444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/graphvizdot.py
--rw-r--r--   0        0        0     6173 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/libdb.py
--rw-r--r--   0        0        0     5105 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/libgraph.py
--rw-r--r--   0        0        0     2090 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/loader.py
--rw-r--r--   0        0        0      793 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/management/commands/dbsamizdat.py
--rw-r--r--   0        0        0      110 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/models.py
--rwxr-xr-x   0        0        0    15579 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/runner.py
--rw-r--r--   0        0        0    11205 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/samizdat.py
--rw-r--r--   0        0        0     7324 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/samtypes.py
--rw-r--r--   0        0        0      600 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.4/dbsamizdat/util.py
--rw-r--r--   0        0        0     1141 2023-06-06 08:02:27.616278 dbsamizdapper-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1820 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0    32474 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/LICENSE.txt
+-rw-r--r--   0        0        0     1444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/README.md
+-rw-r--r--   0        0        0      403 2023-06-08 01:46:35.326000 dbsamizdapper-0.0.5a0/dbsamizdat/__init__.py
+-rw-r--r--   0        0        0     1699 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/api.py
+-rw-r--r--   0        0        0     5197 2023-06-08 01:44:54.281475 dbsamizdapper-0.0.5a0/dbsamizdat/apps.py
+-rw-r--r--   0        0        0     1721 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/django_api.py
+-rw-r--r--   0        0        0     2806 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/exceptions.py
+-rw-r--r--   0        0        0     2444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/graphvizdot.py
+-rw-r--r--   0        0        0     6173 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/libdb.py
+-rw-r--r--   0        0        0     5105 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/libgraph.py
+-rw-r--r--   0        0        0     2224 2023-06-08 01:46:35.322002 dbsamizdapper-0.0.5a0/dbsamizdat/loader.py
+-rw-r--r--   0        0        0      793 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/management/commands/dbsamizdat.py
+-rw-r--r--   0        0        0      110 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/models.py
+-rwxr-xr-x   0        0        0    15579 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/runner.py
+-rw-r--r--   0        0        0    12385 2023-06-08 01:46:22.799134 dbsamizdapper-0.0.5a0/dbsamizdat/samizdat.py
+-rw-r--r--   0        0        0     7324 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/samtypes.py
+-rw-r--r--   0        0        0      600 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/util.py
+-rw-r--r--   0        0        0     1168 2023-06-08 01:50:30.049531 dbsamizdapper-0.0.5a0/pyproject.toml
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.5a0/PKG-INFO
```

### Comparing `dbsamizdapper-0.0.4/LICENSE.txt` & `dbsamizdapper-0.0.5a0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/README.md` & `dbsamizdapper-0.0.5a0/README.md`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/api.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/apps.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/apps.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,21 +52,21 @@
         ArgType(
             in_django=True,
             dbconn=DBCONN,
         )
     )
 
 
-def tables_affected_by(apps, plan):
+def tables_affected_by(apps, plan) -> tuple[bool, set[FQTuple]]:
     """
     Returns tables potentially affected by a migration plan.
     There are false positives, because we don't know what a view depending on a table exactly reads from that table.
     Worse, there may be false negatives, as we may not understand all types of migrations, and the migration plan is not a public API.
     """
-    tables_affected = set()
+    tables_affected: set[FQTuple] = set()
     for mig, reverse in plan:
         if reverse:
             return (
                 True,
                 tables_affected,
             )  # Too hard to think about, not too common, just nuke & recreate
         for operation in mig.operations:
```

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/django_api.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/django_api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/exceptions.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/graphvizdot.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/graphvizdot.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/libdb.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/libdb.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/libgraph.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/libgraph.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/loader.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,25 @@
 import inspect
 from importlib import import_module
 from importlib.util import find_spec
 from logging import getLogger
 from typing import Any, Type, TypeGuard
 
-from dbsamizdat.samizdat import Samizdat, SamizdatFunction, SamizdatMaterializedView, SamizdatTrigger, SamizdatView
-
-SamizType = Type[SamizdatFunction | SamizdatView | SamizdatMaterializedView | SamizdatTrigger]
+from dbsamizdat.samizdat import (
+    Samizdat,
+    SamizdatFunction,
+    SamizdatMaterializedQuerySet,
+    SamizdatMaterializedView,
+    SamizdatTrigger,
+    SamizdatView,
+)
+
+SamizType = Type[
+    SamizdatFunction | SamizdatView | SamizdatMaterializedView | SamizdatTrigger | SamizdatMaterializedQuerySet
+]
 SamizTypes = set[SamizType]
 
 logger = getLogger(__name__)
 
 AUTOLOAD_MODULENAME = "dbsamizdat_defs"
 
 
@@ -20,14 +29,15 @@
     These are the classes which would be user-specified
     """
     subclasses_of = (
         SamizdatFunction,
         SamizdatView,
         SamizdatMaterializedView,
         SamizdatTrigger,
+        SamizdatMaterializedQuerySet,
     )
     return inspect.isclass(inputklass) and issubclass(inputklass, subclasses_of) and inputklass not in subclasses_of
 
 
 def get_samizdats():
     """
     Returns all subclasses of "Samizdat"
```

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/management/commands/dbsamizdat.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/management/commands/dbsamizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/runner.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/runner.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/samizdat.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/samizdat.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,21 @@
 from string import Template
 from time import time as now
 
 from dbsamizdat.samtypes import FQTuple, HasRefreshTriggers, HasSidekicks, Mogrifier, ProtoSamizdat, entitypes
 
 from .util import nodenamefmt
 
+if typing.TYPE_CHECKING:
+    try:
+        from django.db import connection  # noqa: F401
+        from django.db.models import QuerySet
+    except ModuleNotFoundError:
+        pass
+
 _DBINFO_VERSION = 1  # Version number for signature format. For future use
 
 TRIGGER_DEPCOUNTER_PADDED_WIDTH = 5
 
 
 class Samizdat(ProtoSamizdat):
     """
@@ -328,11 +335,42 @@
         """
         Yields "functions" and "triggers"
         to help manage this Materialized View
         """
         if not cls.refresh_triggers:
             return
 
-        counter = Counter()
+        counter: typing.Counter[str] = Counter()
         counter.update({cls.AUTOREFRESHER_COUNTER: 1})
         yield from cls.gen_refresh_triggerfunction()
         yield from cls.gen_refresh_tabletriggers(counter=counter)
+
+
+class SamizdatMaterializedQuerySet(SamizdatMaterializedView):
+    """
+    Class to convert a Django queryset into a materialized view
+    Primarily this is to simplify deeply nested Django operations
+    """
+
+    queryset: QuerySet
+
+    @classmethod
+    def _get_query(cls):
+        """
+        Returns the query, as a string
+        """
+        try:
+            from django.db import connection  # noqa: F811
+        except ModuleNotFoundError as E:
+            raise ModuleNotFoundError("Django is required for a materialized queryset") from E
+
+        with connection.cursor() as c:
+            query = c.mogrify(*cls.queryset.query.sql_with_params())
+            if isinstance(query, bytes):
+                # Some psycopg2 flavours will give str, others bytes
+                # force consistency
+                query = query.decode()
+        return query
+
+    @classmethod
+    def sql_template(cls):
+        return f"""${{preamble}} {cls._get_query()} ${{postamble}}"""
```

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/samtypes.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/samtypes.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/dbsamizdat/util.py` & `dbsamizdapper-0.0.5a0/dbsamizdat/util.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.4/pyproject.toml` & `dbsamizdapper-0.0.5a0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbsamizdapper"
-version = "0.0.4"
+version = "0.0.5a0"
 description = ""
 authors = ["Josh Brooks <josh@catalpa.io>",]
 readme = "README.md"
 
 packages = [
     { include = "dbsamizdat" },
 ]
@@ -24,14 +24,16 @@
 isort = "^5.12.0"
 pre-commit = "^3.3.2"
 pytest = "^7.3.1"
 mypy = "^1.3.0"
 types-toposort = "^1.10.0.0"
 pytest-cov = "^4.1.0"
 python-dotenv = "^1.0.0"
+django-stubs = "^4.2.1"
+
 
 # In addition you will need one of
 # psycopg / psycopg2
 
 # One option:
 
 # psycopg = {extras = ["binary"], version = "^3.1.9"}
```

### Comparing `dbsamizdapper-0.0.4/PKG-INFO` & `dbsamizdapper-0.0.5a0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbsamizdapper
-Version: 0.0.4
+Version: 0.0.5a0
 Summary: 
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

