# Comparing `tmp/dbsamizdapper-0.0.5a0.tar.gz` & `tmp/dbsamizdapper-0.0.5a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbsamizdapper-0.0.5a0.tar", max compression
+gzip compressed data, was "dbsamizdapper-0.0.5a2.tar", max compression
```

## Comparing `dbsamizdapper-0.0.5a0.tar` & `dbsamizdapper-0.0.5a2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0    32474 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/LICENSE.txt
--rw-r--r--   0        0        0     1444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/README.md
--rw-r--r--   0        0        0      403 2023-06-08 01:46:35.326000 dbsamizdapper-0.0.5a0/dbsamizdat/__init__.py
--rw-r--r--   0        0        0     1699 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/api.py
--rw-r--r--   0        0        0     5197 2023-06-08 01:44:54.281475 dbsamizdapper-0.0.5a0/dbsamizdat/apps.py
--rw-r--r--   0        0        0     1721 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/django_api.py
--rw-r--r--   0        0        0     2806 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/exceptions.py
--rw-r--r--   0        0        0     2444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/graphvizdot.py
--rw-r--r--   0        0        0     6173 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/libdb.py
--rw-r--r--   0        0        0     5105 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/libgraph.py
--rw-r--r--   0        0        0     2224 2023-06-08 01:46:35.322002 dbsamizdapper-0.0.5a0/dbsamizdat/loader.py
--rw-r--r--   0        0        0      793 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/management/commands/dbsamizdat.py
--rw-r--r--   0        0        0      110 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/models.py
--rwxr-xr-x   0        0        0    15579 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/runner.py
--rw-r--r--   0        0        0    12385 2023-06-08 01:46:22.799134 dbsamizdapper-0.0.5a0/dbsamizdat/samizdat.py
--rw-r--r--   0        0        0     7324 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/samtypes.py
--rw-r--r--   0        0        0      600 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a0/dbsamizdat/util.py
--rw-r--r--   0        0        0     1168 2023-06-08 01:50:30.049531 dbsamizdapper-0.0.5a0/pyproject.toml
--rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.5a0/PKG-INFO
+-rw-r--r--   0        0        0    32474 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/LICENSE.txt
+-rw-r--r--   0        0        0     1444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/README.md
+-rw-r--r--   0        0        0      568 2023-06-08 05:53:52.332272 dbsamizdapper-0.0.5a2/dbsamizdat/__init__.py
+-rw-r--r--   0        0        0     1699 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/api.py
+-rw-r--r--   0        0        0     5197 2023-06-08 01:44:54.281475 dbsamizdapper-0.0.5a2/dbsamizdat/apps.py
+-rw-r--r--   0        0        0     1721 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/django_api.py
+-rw-r--r--   0        0        0     2806 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/exceptions.py
+-rw-r--r--   0        0        0     2444 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/graphvizdot.py
+-rw-r--r--   0        0        0     6173 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/libdb.py
+-rw-r--r--   0        0        0     5105 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/libgraph.py
+-rw-r--r--   0        0        0     2487 2023-06-08 05:54:02.355829 dbsamizdapper-0.0.5a2/dbsamizdat/loader.py
+-rw-r--r--   0        0        0      793 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/management/commands/dbsamizdat.py
+-rw-r--r--   0        0        0      110 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/models.py
+-rwxr-xr-x   0        0        0    15261 2023-06-08 14:24:38.652902 dbsamizdapper-0.0.5a2/dbsamizdat/runner.py
+-rw-r--r--   0        0        0    14466 2023-06-08 10:16:04.607116 dbsamizdapper-0.0.5a2/dbsamizdat/samizdat.py
+-rw-r--r--   0        0        0     7784 2023-06-08 10:21:28.526481 dbsamizdapper-0.0.5a2/dbsamizdat/samtypes.py
+-rw-r--r--   0        0        0      600 2023-06-06 07:37:57.763422 dbsamizdapper-0.0.5a2/dbsamizdat/util.py
+-rw-r--r--   0        0        0     1168 2023-06-08 09:54:40.365919 dbsamizdapper-0.0.5a2/pyproject.toml
+-rw-r--r--   0        0        0     1822 1970-01-01 00:00:00.000000 dbsamizdapper-0.0.5a2/PKG-INFO
```

### Comparing `dbsamizdapper-0.0.5a0/LICENSE.txt` & `dbsamizdapper-0.0.5a2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/README.md` & `dbsamizdapper-0.0.5a2/README.md`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/api.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/apps.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/apps.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/django_api.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/django_api.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/exceptions.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/exceptions.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/graphvizdot.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/graphvizdot.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/libdb.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/libdb.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/libgraph.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/libgraph.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/loader.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/loader.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,41 +3,56 @@
 from importlib.util import find_spec
 from logging import getLogger
 from typing import Any, Type, TypeGuard
 
 from dbsamizdat.samizdat import (
     Samizdat,
     SamizdatFunction,
+    SamizdatMaterializedModel,
     SamizdatMaterializedQuerySet,
     SamizdatMaterializedView,
+    SamizdatModel,
+    SamizdatQuerySet,
     SamizdatTrigger,
     SamizdatView,
 )
 
 SamizType = Type[
-    SamizdatFunction | SamizdatView | SamizdatMaterializedView | SamizdatTrigger | SamizdatMaterializedQuerySet
+    Samizdat
+    | SamizdatFunction
+    | SamizdatMaterializedModel
+    | SamizdatMaterializedQuerySet
+    | SamizdatMaterializedView
+    | SamizdatModel
+    | SamizdatQuerySet
+    | SamizdatTrigger
+    | SamizdatView
 ]
+
 SamizTypes = set[SamizType]
 
 logger = getLogger(__name__)
 
 AUTOLOAD_MODULENAME = "dbsamizdat_defs"
 
 
 def filter_sds(inputklass: Any) -> TypeGuard[SamizType]:
     """
     Returns subclasses of subclasses of "samizdat"
     These are the classes which would be user-specified
     """
     subclasses_of = (
         SamizdatFunction,
-        SamizdatView,
+        SamizdatMaterializedModel,
+        SamizdatMaterializedQuerySet,
         SamizdatMaterializedView,
+        SamizdatModel,
+        SamizdatQuerySet,
         SamizdatTrigger,
-        SamizdatMaterializedQuerySet,
+        SamizdatView,
     )
     return inspect.isclass(inputklass) and issubclass(inputklass, subclasses_of) and inputklass not in subclasses_of
 
 
 def get_samizdats():
     """
     Returns all subclasses of "Samizdat"
```

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/management/commands/dbsamizdat.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/management/commands/dbsamizdat.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/runner.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,22 +7,21 @@
 from importlib.util import find_spec
 from logging import getLogger
 from time import monotonic
 from typing import Generator, Iterable, Literal
 
 import dotenv
 
-from dbsamizdat.samizdat import Samizdat, SamizdatMaterializedView
-
 from .exceptions import DatabaseError, FunctionSignatureError, SamizdatException
 from .graphvizdot import dot
 from .libdb import dbinfo_to_class, dbstate_equals_definedstate, get_dbstate
 from .libgraph import depsort_with_sidekicks, node_dump, sanity_check, subtree_depends
 from .loader import SamizType, autodiscover_samizdats, get_samizdats
-from .samtypes import Cursor, FQTuple, entitypes
+from .samizdat import sd_is_matview
+from .samtypes import Cursor, FQTuple
 from .util import nodenamefmt, sqlfmt
 
 if typing.TYPE_CHECKING:
     from argparse import ArgumentParser
 
 dotenv.load_dotenv()
 
@@ -135,15 +134,15 @@
         raise KeyError(f"Expected one of 'jumbo' or 'dryrun' or 'checkpoint'; got {txdiscipline}")
     cursor.execute(final_clause)
 
 
 def cmd_refresh(args: ArgType):
     with get_cursor(args) as cursor:
         samizdats = get_sds(args.in_django)
-        matviews: list[SamizdatMaterializedView] = [sd for sd in samizdats if sd.entity_type == entitypes.MATVIEW]
+        matviews = [sd for sd in samizdats if sd_is_matview(sd)]
 
         if args.belownodes:
             rootnodes = {FQTuple.fqify(rootnode) for rootnode in args.belownodes}
             allnodes = node_dump(samizdats)
             if rootnodes - allnodes:
                 raise ValueError(
                     """Unknown rootnodes:\n\t- %s"""
@@ -158,61 +157,60 @@
             for sd in matviews:
                 yield "refresh", sd, sd.refresh(concurrent_allowed=True)
 
         executor(refreshes(), args, cursor, max_namelen=max_namelen, timing=True)
 
 
 def cmd_sync(args: ArgType, samizdatsIn: list[SamizType] | None = None):
+    """
+    This calls the `executor` function with commands to drop / create / refresh
+    instances of Samizdats which are out of sync
+    """
     samizdats = tuple(get_sds(False, samizdatsIn)) or tuple(get_sds(args.in_django))
 
     with get_cursor(args) as cursor:
         db_compare = dbstate_equals_definedstate(cursor, samizdats)
         if db_compare.issame:
             vprint(args, "No differences, nothing to do.")
             return
 
         # Get the longest name from what's in the
         # database and defined state
         max_namelen = max(len(str(ds)) for ds in db_compare.excess_dbstate | db_compare.excess_definedstate)
-        if db_compare.excess_dbstate:
 
-            def drops():
-                for sd in db_compare.excess_dbstate:
-                    yield "drop", sd, sd.drop(if_exists=True)
-                    # we don't know the deptree; so they may have vanished
-                    # through a cascading drop of a previous object
-
-            executor(drops(), args, cursor, max_namelen=max_namelen, timing=True)
-            db_compare = dbstate_equals_definedstate(cursor, samizdats)
-            # again, we don't know the in-db deptree, so we need to re-read DB
-            # state as the rug may have been pulled out from under us with cascading
-            # drops
-        if db_compare.excess_definedstate:
+        def drops():
+            for sd in db_compare.excess_dbstate:
+                yield "drop", sd, sd.drop(if_exists=True)
+                # we don't know the deptree; so they may have vanished
+                # through a cascading drop of a previous object
 
-            def creates():
-                to_create_ids = {sd.head_id() for sd in db_compare.excess_definedstate}
-                for sd in samizdats:  # iterate in proper creation order
-                    if sd.head_id() not in to_create_ids:
-                        continue
-                    yield "create", sd, sd.create()
-                    yield "sign", sd, sd.sign(cursor)
-
-            executor(creates(), args, cursor, max_namelen=max_namelen, timing=True)
-
-            matviews_to_refresh = {
-                sd.head_id() for sd in db_compare.excess_definedstate if sd.entity_type == entitypes.MATVIEW
-            }
-            if matviews_to_refresh:
-
-                def refreshes():
-                    for sd in samizdats:  # iterate in proper creation order
-                        if sd.head_id() in matviews_to_refresh:
-                            yield "refresh", sd, sd.refresh(concurrent_allowed=False)
+        executor(drops(), args, cursor, max_namelen=max_namelen, timing=True)
+        db_compare = dbstate_equals_definedstate(cursor, samizdats)
+        # again, we don't know the in-db deptree, so we need to re-read DB
+        # state as the rug may have been pulled out from under us with cascading
+        # drops
+
+        def creates():
+            to_create_ids = {sd.head_id() for sd in db_compare.excess_definedstate}
+
+            for sd in samizdats:  # iterate in proper creation order
+                if sd.head_id() not in to_create_ids:
+                    continue
+                yield "create", sd, sd.create()
+                yield "sign", sd, sd.sign(cursor)
+
+        executor(creates(), args, cursor, max_namelen=max_namelen, timing=True)
 
-                executor(refreshes(), args, cursor, max_namelen=max_namelen, timing=True)
+        def refreshes():
+            for sd in filter(sd_is_matview, samizdats):
+                if sd not in db_compare.excess_definedstate:
+                    continue
+                yield "refresh", sd, sd.refresh(concurrent_allowed=False)
+
+        executor(refreshes(), args, cursor, max_namelen=max_namelen, timing=True)
 
 
 def cmd_diff(args: ArgType):
     with get_cursor(args) as cursor:
         samizdats = get_sds(args.in_django)
         db_compare = dbstate_equals_definedstate(cursor, samizdats)
         if db_compare.issame:
@@ -251,15 +249,15 @@
     exit(exitcode + exitflag)
 
 
 def cmd_printdot(args: ArgType):
     print("\n".join(dot(get_sds(args.in_django))))
 
 
-def cmd_nuke(args: ArgType, samizdats: list[Samizdat] | None = None):
+def cmd_nuke(args: ArgType, samizdats: list[SamizType] | None = None):
     with get_cursor(args) as cursor:
 
         def nukes():
             # If "samizdats" is not defined fetch from the database
 
             if samizdats is not None:
                 yield from (("nuke", sd, sd.drop(if_exists=True)) for sd in samizdats)
```

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/samizdat.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/samizdat.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,24 +2,32 @@
 
 import typing
 from collections import Counter
 from hashlib import md5
 from json import dumps as jsondumps
 from string import Template
 from time import time as now
+from typing import Any, TypeGuard
 
-from dbsamizdat.samtypes import FQTuple, HasRefreshTriggers, HasSidekicks, Mogrifier, ProtoSamizdat, entitypes
+from dbsamizdat.samtypes import (
+    FQTuple,
+    HasRefreshTriggers,
+    HasSidekicks,
+    Mogrifier,
+    ProtoSamizdat,
+    entitypes,
+    sql_query,
+)
 
 from .util import nodenamefmt
 
 if typing.TYPE_CHECKING:
     try:
-        from django.db import connection  # noqa: F401
-        from django.db.models import QuerySet
-    except ModuleNotFoundError:
+        from django.db.models import Model, QuerySet
+    except (ModuleNotFoundError, ImportError):
         pass
 
 _DBINFO_VERSION = 1  # Version number for signature format. For future use
 
 TRIGGER_DEPCOUNTER_PADDED_WIDTH = 5
 
 
@@ -96,15 +104,15 @@
     @classmethod
     def create(cls):
         """
         SQL to create this DB object
         """
         subst = dict(
             preamble=f"""CREATE {cls.entity_type.value} {cls.db_object_identity()} AS""",
-            postamble="WITH NO DATA" if cls.entity_type.name == "MATVIEW" else "",
+            postamble="WITH NO DATA" if sd_is_matview(cls) else "",
             samizdatname=cls.db_object_identity(),
         )
         return Template(cls.get_sql_template()).safe_substitute(subst)
 
     @classmethod
     def drop(cls, if_exists=False):
         """
@@ -156,15 +164,21 @@
         a new descriptive hash of this instance
         """
         if cls.implanted_hash:
             return cls.implanted_hash
 
         # "Functions" adapt the hash to include creation options
         return md5(
-            "|".join([cls.get_sql_template(), cls.db_object_identity(), cls.creation_identity()]).encode("utf-8")
+            "|".join(
+                [
+                    cls.get_sql_template(),
+                    cls.db_object_identity(),
+                    cls.creation_identity(),
+                ]
+            ).encode("utf-8")
         ).hexdigest()
 
     @classmethod
     def creation_function_arguments(cls) -> str:
         return getattr(cls, "function_arguments", cls.function_arguments_signature)
 
     @classmethod
@@ -197,15 +211,18 @@
         (indirectly it is, through a table.)
         Yet trigger names do not need to be unique in a schema.
         Yet we need a unique identifier for them, within the dbsamizdat collection.
         So we use the table the trigger is attached to as a component
         in the fully qualified name.
         """
 
-        return FQTuple(schema=FQTuple.fqify(cls.on_table).db_object_identity(), object_name=cls.get_name())
+        return FQTuple(
+            schema=FQTuple.fqify(cls.on_table).db_object_identity(),
+            object_name=cls.get_name(),
+        )
 
     def __str__(self):
         return nodenamefmt(self.fq())
 
     @classmethod
     def fqdeps_on_unmanaged(cls):
         return {FQTuple.fqify(n) for n in cls.deps_on_unmanaged | {cls.on_table}}
@@ -341,36 +358,106 @@
 
         counter: typing.Counter[str] = Counter()
         counter.update({cls.AUTOREFRESHER_COUNTER: 1})
         yield from cls.gen_refresh_triggerfunction()
         yield from cls.gen_refresh_tabletriggers(counter=counter)
 
 
-class SamizdatMaterializedQuerySet(SamizdatMaterializedView):
+class SamizdatQuerySet(Samizdat):
     """
     Class to convert a Django queryset into a materialized view
     Primarily this is to simplify deeply nested Django operations
     """
 
     queryset: QuerySet
 
     @classmethod
-    def _get_query(cls):
+    def get_queryset(cls):
+        return cls.queryset
+
+    @classmethod
+    def sql_template(cls):
+        return f"""${{preamble}} {cls.get_query(cls.get_queryset())} ${{postamble}}"""
+
+    @classmethod
+    def get_query(cls, queryset: QuerySet) -> sql_query:
         """
         Returns the query, as a string
         """
-        try:
-            from django.db import connection  # noqa: F811
-        except ModuleNotFoundError as E:
-            raise ModuleNotFoundError("Django is required for a materialized queryset") from E
+        from django.db import connection  # noqa: F811
 
         with connection.cursor() as c:
-            query = c.mogrify(*cls.queryset.query.sql_with_params())
+            query = c.mogrify(*queryset.query.sql_with_params())
             if isinstance(query, bytes):
                 # Some psycopg2 flavours will give str, others bytes
                 # force consistency
                 query = query.decode()
         return query
 
+
+class SamizdatMaterializedQuerySet(SamizdatQuerySet, SamizdatMaterializedView):
+    entity_type = entitypes.MATVIEW
+
+
+class SamizdatModel(SamizdatQuerySet):
+    """
+    This is an abstraction around relating a Django unmanaged model
+    to a Materialized View, defined as a Django 'query' instance.
+
+    The class takes two parameters: a "model" instance
+    and a "queryset".
+
+    The fields returned
+    """
+
+    model: Model
+
     @classmethod
-    def sql_template(cls):
-        return f"""${{preamble}} {cls._get_query()} ${{postamble}}"""
+    def _add_id(cls, queryset: QuerySet):
+        """
+        Auto add an "id" column;
+        this is required for Django's admin to
+        function correctly as it uses the primary key
+        to add a detail view
+        """
+        from django.db.models.expressions import Window
+        from django.db.models.functions import RowNumber
+
+        return queryset.annotate(id=Window(expression=RowNumber()))
+
+    @classmethod
+    def get_queryset(cls):
+        """
+        Get the 'values' associted with the fields defined on the model
+        """
+        fields = [field.attname for field in cls.model._meta.get_fields()]
+        return cls._add_id(cls.queryset).values(*fields)
+
+    @classmethod
+    def get_name(cls):
+        """
+        Use the name as Django defined it
+        """
+        return cls.model._meta.db_table
+
+
+class SamizdatMaterializedModel(SamizdatModel, SamizdatMaterializedView):
+    entity_type = entitypes.MATVIEW
+
+
+def sd_is_view(sd: Any) -> TypeGuard[SamizdatView]:
+    return getattr(sd, "entity_type", None) == entitypes.VIEW
+
+
+def sd_is_matview(sd: Any) -> TypeGuard[SamizdatMaterializedView]:
+    """
+    This is used to determine refresh methods when sync'ing
+    """
+    return getattr(sd, "entity_type", None) == entitypes.MATVIEW
+
+
+def sd_is_function(sd: Any) -> TypeGuard[SamizdatFunction]:
+    return getattr(sd, "entity_type", None) == entitypes.FUNCTION
+
+
+def sd_is_trigger(sd: Any) -> TypeGuard[SamizdatTrigger]:
+    return getattr(sd, "entity_type", None) == entitypes.TRIGGER
```

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/samtypes.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/samtypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Callable, Iterable, Type
+from typing import Any, Callable, Iterable, Protocol, Type
 
 from dbsamizdat.exceptions import UnsuitableNameError
 
 PG_IDENTIFIER_MAXLEN = 63
 PG_IDENTIFIER_VERBOTEN = set('"')
 # Actually allowed, but we'd have to escape it everywhere.
 # See https://www.postgresql.org/docs/current/sql-syntax-lexical.html#SQL-SYNTAX-IDENTIFIERS
@@ -86,14 +86,19 @@
 
         elif hasattr(arg, "fq"):
             """
             Convert a Samizdat like instance
             """
             return arg.fq()
 
+        elif hasattr(arg, "_meta"):
+            # If a django-like instance with a `_meta` prop is provided
+            # use its db_table to determine a fully qualified name
+            return cls.fqify(arg._meta.db_table)
+
         else:
             raise TypeError
 
 
 objectname = str
 schemaname = str
 sql_query = str
@@ -227,15 +232,27 @@
 
     @classmethod
     @abstractmethod
     def head_id(cls) -> str:
         ...
 
 
-FQIffable = FQTuple | HasFQ | str | ProtoSamizdat | Type[ProtoSamizdat] | tuple[str, ...]
+class DjangoModelMeta(Protocol):
+    db_table: str
+
+
+class DjangoModelLike(Protocol):
+    """
+    Allow passing a Django model where an "FQIffable" instance is expected
+    """
+
+    _meta: DjangoModelMeta
+
+
+FQIffable = FQTuple | HasFQ | str | ProtoSamizdat | Type[ProtoSamizdat] | tuple[str, ...] | DjangoModelLike
 
 
 class HasSidekicks(ABC):
     """
     Some Samizdat classes have additional
     triggers or functions
     One example is Materialized Views with `refresh_triggers`
```

### Comparing `dbsamizdapper-0.0.5a0/dbsamizdat/util.py` & `dbsamizdapper-0.0.5a2/dbsamizdat/util.py`

 * *Files identical despite different names*

### Comparing `dbsamizdapper-0.0.5a0/pyproject.toml` & `dbsamizdapper-0.0.5a2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dbsamizdapper"
-version = "0.0.5a0"
+version = "0.0.5a2"
 description = ""
 authors = ["Josh Brooks <josh@catalpa.io>",]
 readme = "README.md"
 
 packages = [
     { include = "dbsamizdat" },
 ]
```

### Comparing `dbsamizdapper-0.0.5a0/PKG-INFO` & `dbsamizdapper-0.0.5a2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbsamizdapper
-Version: 0.0.5a0
+Version: 0.0.5a2
 Summary: 
 Author: Josh Brooks
 Author-email: josh@catalpa.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

