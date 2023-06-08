# Comparing `tmp/django-pgtrigger-4.6.0.tar.gz` & `tmp/django_pgtrigger-4.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgtrigger-4.6.0.tar", max compression
+gzip compressed data, was "django_pgtrigger-4.7.0.tar", max compression
```

## Comparing `django-pgtrigger-4.6.0.tar` & `django_pgtrigger-4.7.0.tar`

### file list

```diff
@@ -1,21 +1,20 @@
--rw-r--r--   0        0        0     1456 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/LICENSE
--rw-r--r--   0        0        0     4702 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/README.rst
--rw-r--r--   0        0        0     1558 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/__init__.py
--rw-r--r--   0        0        0     3893 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/apps.py
--rw-r--r--   0        0        0     7467 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/compiler.py
--rw-r--r--   0        0        0     7575 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/contrib.py
--rw-r--r--   0        0        0    20102 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/core.py
--rw-r--r--   0        0        0     1116 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/features.py
--rw-r--r--   0        0        0     5088 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/installation.py
--rw-r--r--   0        0        0        0 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/management/__init__.py
--rw-r--r--   0        0        0        0 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/management/commands/__init__.py
--rw-r--r--   0        0        0     7431 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/management/commands/pgtrigger.py
--rw-r--r--   0        0        0    15898 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/migrations.py
--rw-r--r--   0        0        0      105 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/models.py
--rw-r--r--   0        0        0     4541 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/registry.py
--rw-r--r--   0        0        0     9739 2022-10-07 03:27:41.438681 django-pgtrigger-4.6.0/pgtrigger/runtime.py
--rw-r--r--   0        0        0     1577 2022-10-07 03:27:41.442681 django-pgtrigger-4.6.0/pgtrigger/utils.py
--rw-r--r--   0        0        0      154 2022-10-07 03:27:41.442681 django-pgtrigger-4.6.0/pgtrigger/version.py
--rw-r--r--   0        0        0     2514 2022-10-07 03:28:21.299129 django-pgtrigger-4.6.0/pyproject.toml
--rw-r--r--   0        0        0     5708 1970-01-01 00:00:00.000000 django-pgtrigger-4.6.0/setup.py
--rw-r--r--   0        0        0     6125 1970-01-01 00:00:00.000000 django-pgtrigger-4.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-08 18:40:09.451290 django_pgtrigger-4.7.0/LICENSE
+-rw-r--r--   0        0        0     4731 2023-06-08 18:40:09.451290 django_pgtrigger-4.7.0/README.rst
+-rw-r--r--   0        0        0     1578 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/__init__.py
+-rw-r--r--   0        0        0     3893 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/apps.py
+-rw-r--r--   0        0        0     7467 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/compiler.py
+-rw-r--r--   0        0        0     7575 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/contrib.py
+-rw-r--r--   0        0        0    20697 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/core.py
+-rw-r--r--   0        0        0     1116 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/features.py
+-rw-r--r--   0        0        0     5030 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/installation.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/management/commands/__init__.py
+-rw-r--r--   0        0        0     7431 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/management/commands/pgtrigger.py
+-rw-r--r--   0        0        0    15898 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/migrations.py
+-rw-r--r--   0        0        0      105 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/models.py
+-rw-r--r--   0        0        0     4541 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/registry.py
+-rw-r--r--   0        0        0    10590 2023-06-08 18:40:09.455289 django_pgtrigger-4.7.0/pgtrigger/runtime.py
+-rw-r--r--   0        0        0     2515 2023-06-08 18:40:09.459290 django_pgtrigger-4.7.0/pgtrigger/utils.py
+-rw-r--r--   0        0        0      154 2023-06-08 18:40:09.459290 django_pgtrigger-4.7.0/pgtrigger/version.py
+-rw-r--r--   0        0        0     2545 2023-06-08 18:40:40.967479 django_pgtrigger-4.7.0/pyproject.toml
+-rw-r--r--   0        0        0     6005 1970-01-01 00:00:00.000000 django_pgtrigger-4.7.0/PKG-INFO
```

### Comparing `django-pgtrigger-4.6.0/LICENSE` & `django_pgtrigger-4.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/README.rst` & `django_pgtrigger-4.7.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 If triggers are new to you, don't worry.
 The `pgtrigger docs <https://django-pgtrigger.readthedocs.io/>`__ cover triggers in
 more detail and provide many examples.
 
 Compatibility
 =============
 
-``django-pgtrigger`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 14.
+``django-pgtrigger`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3, and Postgres 10 - 15.
 
 Documentation
 =============
 
 `View the pgtrigger docs here <https://django-pgtrigger.readthedocs.io/>`__ to
 learn more about:
 
@@ -134,7 +134,8 @@
 
 Other Contributors
 ==================
 
 - @jzmiller1
 - @rrauenza
 - @ralokt
+- @adamchainz
```

### Comparing `django-pgtrigger-4.6.0/pgtrigger/__init__.py` & `django_pgtrigger-4.7.0/pgtrigger/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from pgtrigger.runtime import (
     constraints,
     ignore,
     schema,
 )
 from pgtrigger.version import __version__
 
-if django.VERSION < (3, 2):
+if django.VERSION < (3, 2):  # pragma: no cover
     default_app_config = "pgtrigger.apps.PGTriggerConfig"
 
 del django
 
 
 __all__ = [
     "After",
```

### Comparing `django-pgtrigger-4.6.0/pgtrigger/apps.py` & `django_pgtrigger-4.7.0/pgtrigger/apps.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/compiler.py` & `django_pgtrigger-4.7.0/pgtrigger/compiler.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/contrib.py` & `django_pgtrigger-4.7.0/pgtrigger/contrib.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/core.py` & `django_pgtrigger-4.7.0/pgtrigger/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 
 from django.db import DEFAULT_DB_ALIAS, models, router, transaction
 from django.db.models.expressions import Col
 from django.db.models.fields.related import RelatedField
 from django.db.models.sql import Query
 from django.db.models.sql.datastructures import BaseTable
 from django.db.utils import ProgrammingError
-import psycopg2.extensions
 
 from pgtrigger import compiler, features, registry, utils
 
+if utils.psycopg_maj_version == 2:
+    import psycopg2.extensions
+elif utils.psycopg_maj_version == 3:
+    import psycopg.adapt
+else:
+    raise AssertionError
+
 
 # Postgres only allows identifiers to be 63 chars max. Since "pgtrigger_"
 # is the prefix for trigger names, and since an additional "_" and
 # 5 character hash is added, the user-defined name of the trigger can only
 # be 47 chars.
 # NOTE: We can do something more sophisticated later by allowing users
 # to name their triggers and then hashing the names when actually creating
@@ -274,20 +280,32 @@
     """
     Similar to Django's ``Q`` object, allows referencing the old and new
     rows in a trigger condition.
     """
 
     def resolve(self, model):
         query = _OldNewQuery(model)
+        connection = utils.connection()
         sql, args = self.resolve_expression(query).as_sql(
             compiler=query.get_compiler("default"),
-            connection=utils.connection(),
+            connection=connection,
         )
         sql = sql.replace('"OLD"', "OLD").replace('"NEW"', "NEW")
-        args = tuple(psycopg2.extensions.adapt(arg).getquoted().decode() for arg in args)
+
+        def _quote(val):
+            """Given a value, quote it and handle psycopg2/3 differences"""
+            if utils.psycopg_maj_version == 2:
+                return psycopg2.extensions.adapt(val).getquoted()
+            elif utils.psycopg_maj_version == 3:
+                transformer = psycopg.adapt.Transformer()
+                return transformer.as_literal(val) if val is not None else b"NULL"
+            else:
+                raise AssertionError
+
+        args = tuple(_quote(arg).decode() for arg in args)
 
         return sql % args
 
 
 class Func:
     """
     Allows for rendering a function with access to the "meta", "fields",
```

### Comparing `django-pgtrigger-4.6.0/pgtrigger/features.py` & `django_pgtrigger-4.7.0/pgtrigger/features.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/installation.py` & `django_pgtrigger-4.7.0/pgtrigger/installation.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,25 +48,24 @@
 
     registered = {
         (utils.quote(model._meta.db_table), trigger.get_pgid(model))
         for model, trigger in registry.registered()
     }
 
     with utils.connection(database).cursor() as cursor:
-        pg_maj_version = int(str(cursor.connection.server_version)[:-4])
-        parent_trigger_clause = "tgparentid = 0 AND" if pg_maj_version >= 13 else ""
+        parent_trigger_clause = "tgparentid = 0 AND" if utils.pg_maj_version(cursor) >= 13 else ""
 
         # Only select triggers that are in the current search path. We accomplish
         # this by parsing the tgrelid and only selecting triggers that don't have
         # a schema name in their path
         cursor.execute(
             f"""
             SELECT tgrelid::regclass, tgname, tgenabled
                 FROM pg_trigger
-                WHERE tgname LIKE 'pgtrigger_%' AND
+                WHERE tgname LIKE 'pgtrigger_%%' AND
                       {parent_trigger_clause}
                       array_length(parse_ident(tgrelid::regclass::varchar), 1) = 1
             """
         )
         triggers = set(cursor.fetchall())
 
     return [
```

### Comparing `django-pgtrigger-4.6.0/pgtrigger/management/commands/pgtrigger.py` & `django_pgtrigger-4.7.0/pgtrigger/management/commands/pgtrigger.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/migrations.py` & `django_pgtrigger-4.7.0/pgtrigger/migrations.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/registry.py` & `django_pgtrigger-4.7.0/pgtrigger/registry.py`

 * *Files identical despite different names*

### Comparing `django-pgtrigger-4.6.0/pgtrigger/runtime.py` & `django_pgtrigger-4.7.0/pgtrigger/runtime.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,19 +2,25 @@
 Functions for runtime-configuration of triggers, such as ignoring
 them or dynamically setting the search path.
 """
 import contextlib
 import threading
 
 from django.db import connections
-import psycopg2.extensions
 
 from pgtrigger import registry
 from pgtrigger import utils
 
+if utils.psycopg_maj_version == 2:
+    import psycopg2.extensions
+elif utils.psycopg_maj_version == 3:
+    import psycopg.pq
+else:
+    raise AssertionError
+
 
 # All triggers currently being ignored
 _ignore = threading.local()
 
 # All schemas in the search path
 _schema = threading.local()
 
@@ -27,51 +33,65 @@
     return sql.startswith("create") and "concurrently" in sql
 
 
 def _is_transaction_errored(cursor):
     """
     True if the current transaction is in an errored state
     """
-    return (
-        cursor.connection.get_transaction_status()
-        == psycopg2.extensions.TRANSACTION_STATUS_INERROR
-    )
+    if utils.psycopg_maj_version == 2:
+        return (
+            cursor.connection.get_transaction_status()
+            == psycopg2.extensions.TRANSACTION_STATUS_INERROR
+        )
+    elif utils.psycopg_maj_version == 3:
+        return cursor.connection.info.transaction_status == psycopg.pq.TransactionStatus.INERROR
+    else:
+        raise AssertionError
 
 
 def _can_inject_variable(cursor, sql):
     """True if we can inject a SQL variable into a statement.
 
     A named cursor automatically prepends
     "NO SCROLL CURSOR WITHOUT HOLD FOR" to the query, which
     causes invalid SQL to be generated. There is no way
-    to override this behavior in psycopg2, so ignoring triggers
+    to override this behavior in psycopg, so ignoring triggers
     cannot happen for named cursors. Django only names cursors
     for iterators and other statements that read the database,
     so it seems to be safe to ignore named cursors.
 
     Concurrent index creation is also incompatible with local variable
     setting. Ignore these cases for now.
     """
     return (
-        not cursor.name
+        not getattr(cursor, "name", None)
         and not _is_concurrent_statement(sql)
         and not _is_transaction_errored(cursor)
     )
 
 
+def _execute_wrapper(execute_result):
+    if utils.psycopg_maj_version == 3:
+        while execute_result.nextset():
+            pass
+    return execute_result
+
+
 def _inject_pgtrigger_ignore(execute, sql, params, many, context):
     """
     A connection execution wrapper that sets a pgtrigger.ignore
     variable in the executed SQL. This lets other triggers know when
     they should ignore execution
     """
     if _can_inject_variable(context["cursor"], sql):
-        sql = "SET LOCAL pgtrigger.ignore='{" + ",".join(_ignore.value) + "}';" + sql
+        serialized_ignore = "{" + ",".join(_ignore.value) + "}"
+        sql = f"SELECT set_config('pgtrigger.ignore', %s, true); {sql}"
+        params = [serialized_ignore, *(params or ())]
 
-    return execute(sql, params, many, context)
+    return _execute_wrapper(execute(sql, params, many, context))
 
 
 @contextlib.contextmanager
 def _set_ignore_session_state(database=None):
     """Starts a session where triggers can be ignored"""
     connection = utils.connection(database)
     if _inject_pgtrigger_ignore not in connection.execute_wrappers:
@@ -79,15 +99,15 @@
             try:
                 yield
             finally:
                 if connection.in_atomic_block:
                     # We've finished ignoring triggers and are in a transaction,
                     # so flush the local variable.
                     with connection.cursor() as cursor:
-                        cursor.execute("RESET pgtrigger.ignore;")
+                        cursor.execute("SELECT set_config('pgtrigger.ignore', NULL, false);")
     else:
         yield
 
 
 @contextlib.contextmanager
 def _ignore_session(databases=None):
     """Starts a session where triggers can be ignored"""
@@ -167,48 +187,47 @@
 
 def _inject_schema(execute, sql, params, many, context):
     """
     A connection execution wrapper that sets the schema
     variable in the executed SQL.
     """
     if _can_inject_variable(context["cursor"], sql) and _schema.value:
-        sql = (
-            "SET LOCAL search_path="
-            + ",".join(utils.quote(val) for val in _schema.value)
-            + ";"
-            + sql
-        )
+        path = ", ".join(val if not val.startswith("$") else f'"{val}"' for val in _schema.value)
+        sql = f"SELECT set_config('search_path', %s, true); {sql}"
+        params = [path, *(params or ())]
 
-    return execute(sql, params, many, context)
+    return _execute_wrapper(execute(sql, params, many, context))
 
 
 @contextlib.contextmanager
 def _set_schema_session_state(database=None):
     connection = utils.connection(database)
 
     if _inject_schema not in connection.execute_wrappers:
         if connection.in_atomic_block:
             # If this is the first time we are setting the search path,
             # register the pre_execute_hook and store a reference to the original
             # search path. Note that we must use this approach because we cannot
-            # simply RESET the search_path at the end. A user may have previously
+            # simply reset the search_path at the end. A user may have previously
             # set it
             with connection.cursor() as cursor:
-                cursor.execute("SHOW search_path;")
+                cursor.execute("SELECT current_setting('search_path')")
                 initial_search_path = cursor.fetchall()[0][0]
 
         with connection.execute_wrapper(_inject_schema):
             try:
                 yield
             finally:
                 if connection.in_atomic_block:
                     # We've finished modifying the search path and are in a transaction,
                     # so flush the local variable
                     with connection.cursor() as cursor:
-                        cursor.execute(f"SET search_path={initial_search_path};")
+                        cursor.execute(
+                            "SELECT set_config('search_path', %s, false)", [initial_search_path]
+                        )
     else:
         yield
 
 
 @contextlib.contextmanager
 def _schema_session(databases=None):
     """Starts a session where the search path can be modified"""
```

### Comparing `django-pgtrigger-4.6.0/pyproject.toml` & `django_pgtrigger-4.7.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -26,30 +26,31 @@
 name = "django-pgtrigger"
 packages = [
   { include = "pgtrigger" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "4.6.0"
+version = "4.7.0"
 description = "Postgres trigger support integrated with Django models."
 authors = ["Wes Kendall"]
 classifiers = [
   "Framework :: Django",
-  "Framework :: Django :: 2.2",
   "Framework :: Django :: 3.2",
   "Framework :: Django :: 4.0",
   "Framework :: Django :: 4.1",
+  "Framework :: Django :: 4.2",
   "Intended Audience :: Developers",
   "Operating System :: OS Independent",
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3 :: Only",
   "Framework :: Django",
 ]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/Opus10/django-pgtrigger"
 repository = "https://github.com/Opus10/django-pgtrigger"
@@ -67,21 +68,20 @@
 django-postgres-extra = "2.0.4"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
-git-tidy = "1.1.2"
+git-tidy = "1.2.0"
 myst-parser = "0.18.0"
 packaging = ">=19.2"
-pip = "*"
-poetry-core = "1.1.0rc3"
+poetry-core = "1.6.1"
 pre-commit = "2.13.0"
-psycopg2-binary = "2.9.3"
+psycopg2-binary = "2.9.6"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-dotenv = "0.5.2"
 pytest-django = "4.5.2"
 pytest-mock = "3.6.1"
 requests = "2.25.1"
 Sphinx = "4.4.0"
```

### Comparing `django-pgtrigger-4.6.0/PKG-INFO` & `django_pgtrigger-4.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: django-pgtrigger
-Version: 4.6.0
+Version: 4.7.0
 Summary: Postgres trigger support integrated with Django models.
 Home-page: https://github.com/Opus10/django-pgtrigger
 License: BSD-3-Clause
 Author: Wes Kendall
 Requires-Python: >=3.7.0,<4
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
-Requires-Dist: importlib_metadata (>=4); python_version >= "3.7" and python_version < "3.8"
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-pgtrigger.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgtrigger
 Description-Content-Type: text/x-rst
 
 django-pgtrigger
 ################
 
@@ -113,15 +110,15 @@
 If triggers are new to you, don't worry.
 The `pgtrigger docs <https://django-pgtrigger.readthedocs.io/>`__ cover triggers in
 more detail and provide many examples.
 
 Compatibility
 =============
 
-``django-pgtrigger`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 14.
+``django-pgtrigger`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3, and Postgres 10 - 15.
 
 Documentation
 =============
 
 `View the pgtrigger docs here <https://django-pgtrigger.readthedocs.io/>`__ to
 learn more about:
 
@@ -167,8 +164,9 @@
 
 Other Contributors
 ==================
 
 - @jzmiller1
 - @rrauenza
 - @ralokt
+- @adamchainz
```

