# Comparing `tmp/django-pgbulk-1.3.0.tar.gz` & `tmp/django_pgbulk-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgbulk-1.3.0.tar", max compression
+gzip compressed data, was "django_pgbulk-1.4.0.tar", max compression
```

## Comparing `django-pgbulk-1.3.0.tar` & `django_pgbulk-1.4.0.tar`

### file list

```diff
@@ -1,8 +1,7 @@
--rw-r--r--   0        0        0     1456 2022-12-12 16:58:29.256836 django-pgbulk-1.3.0/LICENSE
--rw-r--r--   0        0        0     1578 2022-12-12 16:58:29.256836 django-pgbulk-1.3.0/README.rst
--rw-r--r--   0        0        0      237 2022-12-12 16:58:29.256836 django-pgbulk-1.3.0/pgbulk/__init__.py
--rw-r--r--   0        0        0    26259 2022-12-12 16:58:29.256836 django-pgbulk-1.3.0/pgbulk/core.py
--rw-r--r--   0        0        0      151 2022-12-12 16:58:29.256836 django-pgbulk-1.3.0/pgbulk/version.py
--rw-r--r--   0        0        0     2301 2022-12-12 16:59:17.969299 django-pgbulk-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     2417 1970-01-01 00:00:00.000000 django-pgbulk-1.3.0/setup.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 django-pgbulk-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-08 21:12:37.500882 django_pgbulk-1.4.0/LICENSE
+-rw-r--r--   0        0        0     1718 2023-06-08 21:12:37.500882 django_pgbulk-1.4.0/README.rst
+-rw-r--r--   0        0        0      237 2023-06-08 21:12:37.504882 django_pgbulk-1.4.0/pgbulk/__init__.py
+-rw-r--r--   0        0        0    27591 2023-06-08 21:12:37.504882 django_pgbulk-1.4.0/pgbulk/core.py
+-rw-r--r--   0        0        0      151 2023-06-08 21:12:37.504882 django_pgbulk-1.4.0/pgbulk/version.py
+-rw-r--r--   0        0        0     2345 2023-06-08 21:13:14.204992 django_pgbulk-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2975 1970-01-01 00:00:00.000000 django_pgbulk-1.4.0/PKG-INFO
```

### Comparing `django-pgbulk-1.3.0/LICENSE` & `django_pgbulk-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgbulk-1.3.0/README.rst` & `django_pgbulk-1.4.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -17,14 +17,19 @@
 3. ``sync`` - For syncing a list of models with a table. Does a bulk
    upsert and also deletes any rows in the source queryset that were not
    part of the input data.
 
 For more examples, see the
 `django-pgbulk docs <https://django-pgbulk.readthedocs.io/>`_.
 
+Compatibility
+=============
+
+``django-pgbulk`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 `View the django-pgbulk docs here <https://django-pgbulk.readthedocs.io/>`_.
 
 Installation
 ============
```

### Comparing `django-pgbulk-1.3.0/pgbulk/core.py` & `django_pgbulk-1.4.0/pgbulk/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,56 @@
 from collections import namedtuple, UserString
 import itertools
 
+from django.core.exceptions import ImproperlyConfigured
 from django.db import connections
 from django.db import models
 from django.db.models.sql.compiler import SQLCompiler
 from django.utils import timezone
-from psycopg2.extensions import AsIs
+from django.utils.version import get_version_tuple
+
+
+def _psycopg_version():
+    try:
+        import psycopg as Database
+    except ImportError:
+        import psycopg2 as Database
+    except ImportError:  # pragma: no cover
+        raise ImproperlyConfigured("Error loading psycopg2 or psycopg module")
+
+    version_tuple = get_version_tuple(Database.__version__.split(" ", 1)[0])
+
+    if version_tuple[0] not in (2, 3):  # pragma: no cover
+        raise ImproperlyConfigured(f"Pysocpg version {version_tuple[0]} not supported")
+
+    return version_tuple
+
+
+psycopg_version = _psycopg_version()
+psycopg_maj_version = psycopg_version[0]
+
+
+if psycopg_maj_version == 2:
+    from psycopg2.extensions import AsIs as Literal
+elif psycopg_maj_version == 3:
+    import psycopg.adapt
+
+    class Literal:  # pragma: no cover
+        def __init__(self, val):
+            self.val = val
+
+    class LiteralDumper(psycopg.adapt.Dumper):  # pragma: no cover
+        def dump(self, obj):
+            return obj.val.encode("utf-8")
+
+        def quote(self, obj):
+            return self.dump(obj)
+
+else:
+    raise AssertionError
 
 
 class UpdateField(UserString):
     def __init__(self, field, expression=None):
         self.data = field
         self.expression = expression
 
@@ -90,18 +131,21 @@
         for f in auto_field_names:
             setattr(value, f, now)
 
     return values
 
 
 def _prep_sql_args(queryset, connection, cursor, sql_args):
+    if psycopg_maj_version == 3:
+        cursor.adapters.register_dumper(Literal, LiteralDumper)
+
     compiler = SQLCompiler(query=queryset.query, connection=connection, using=queryset.using)
 
     return [
-        AsIs(cursor.mogrify(*sql_arg.as_sql(compiler, connection)).decode("utf-8"))
+        Literal(cursor.mogrify(*sql_arg.as_sql(compiler, connection)).decode("utf-8"))
         if hasattr(sql_arg, "as_sql")
         else sql_arg
         for sql_arg in sql_args
     ]
 
 
 def _get_field_db_val(queryset, field, value, connection):
@@ -217,17 +261,19 @@
     }
     if update_expressions:
         connection = connections[queryset.db]
         compiler = SQLCompiler(query=queryset.query, connection=connection, using=queryset.using)
         with connection.cursor() as cursor:
             for field_name, expr in update_expressions.items():
                 expr = expr.resolve_expression(queryset.query, allow_joins=False, for_save=True)
-                update_fields_expressions[
-                    model._meta.get_field(field_name).column
-                ] = cursor.mogrify(*expr.as_sql(compiler, connection)).decode("utf-8")
+                val = cursor.mogrify(*expr.as_sql(compiler, connection))
+                if isinstance(val, bytes):  # Psycopg 2/3 return different types
+                    val = val.decode("utf-8")
+
+                update_fields_expressions[model._meta.get_field(field_name).column] = val
 
     update_fields_sql = ", ".join(
         f"{_quote(field.column)} = {update_fields_expressions[field.column]}"
         for field in update_fields
     )
 
     return_sql = (
```

### Comparing `django-pgbulk-1.3.0/pyproject.toml` & `django_pgbulk-1.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 name = "django-pgbulk"
 packages = [
   { include = "pgbulk" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.3.0"
+version = "1.4.0"
 description = "Native postgres bulk update and upsert operations."
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
 homepage = "https://github.com/Opus10/django-pgbulk"
 repository = "https://github.com/Opus10/django-pgbulk"
@@ -64,21 +65,21 @@
 dj-database-url = "0.5.0"
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
 pip = "*"
 poetry-core = "1.3.2"
 pre-commit = "2.13.0"
-psycopg2-binary = "2.9.3"
+psycopg2-binary = "2.9.6"
 pytest = "7.0.0"
 pytest-cov = "3.0.0"
 pytest-dotenv = "0.5.2"
 pytest-django = "4.5.2"
 requests = "2.25.1"
 Sphinx = "4.4.0"
 sphinx-rtd-theme = "1.0.0"
```

### Comparing `django-pgbulk-1.3.0/PKG-INFO` & `django_pgbulk-1.4.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,33 @@
 Metadata-Version: 2.1
 Name: django-pgbulk
-Version: 1.3.0
+Version: 1.4.0
 Summary: Native postgres bulk update and upsert operations.
 Home-page: https://github.com/Opus10/django-pgbulk
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
 Project-URL: Documentation, https://django-pgbulk.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgbulk
 Description-Content-Type: text/x-rst
 
 django-pgbulk
 #############
 
@@ -50,14 +47,19 @@
 3. ``sync`` - For syncing a list of models with a table. Does a bulk
    upsert and also deletes any rows in the source queryset that were not
    part of the input data.
 
 For more examples, see the
 `django-pgbulk docs <https://django-pgbulk.readthedocs.io/>`_.
 
+Compatibility
+=============
+
+``django-pgbulk`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 `View the django-pgbulk docs here <https://django-pgbulk.readthedocs.io/>`_.
 
 Installation
 ============
```

