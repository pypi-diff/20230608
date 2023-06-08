# Comparing `tmp/django-pgactivity-1.1.1.tar.gz` & `tmp/django_pgactivity-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-pgactivity-1.1.1.tar", max compression
+gzip compressed data, was "django_pgactivity-1.2.0.tar", max compression
```

## Comparing `django-pgactivity-1.1.1.tar` & `django_pgactivity-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,16 @@
--rw-r--r--   0        0        0     1456 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/LICENSE
--rw-r--r--   0        0        0     4188 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/README.rst
--rw-r--r--   0        0        0      266 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/__init__.py
--rw-r--r--   0        0        0     1641 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/config.py
--rw-r--r--   0        0        0     1171 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/contrib.py
--rw-r--r--   0        0        0     4419 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/core.py
--rw-r--r--   0        0        0        0 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/management/__init__.py
--rw-r--r--   0        0        0        0 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/management/commands/__init__.py
--rw-r--r--   0        0        0     4305 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/management/commands/pgactivity.py
--rw-r--r--   0        0        0      308 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/middleware.py
--rw-r--r--   0        0        0     8577 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/models.py
--rw-r--r--   0        0        0     2344 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/runtime.py
--rw-r--r--   0        0        0      373 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/utils.py
--rw-r--r--   0        0        0      155 2022-10-25 03:25:40.846950 django-pgactivity-1.1.1/pgactivity/version.py
--rw-r--r--   0        0        0     2406 2022-10-25 03:26:31.527233 django-pgactivity-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     5177 1970-01-01 00:00:00.000000 django-pgactivity-1.1.1/setup.py
--rw-r--r--   0        0        0     5612 1970-01-01 00:00:00.000000 django-pgactivity-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/LICENSE
+-rw-r--r--   0        0        0     4202 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/README.rst
+-rw-r--r--   0        0        0      266 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/__init__.py
+-rw-r--r--   0        0        0     1641 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/config.py
+-rw-r--r--   0        0        0     1171 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/contrib.py
+-rw-r--r--   0        0        0     5072 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/core.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/management/commands/__init__.py
+-rw-r--r--   0        0        0     4305 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/management/commands/pgactivity.py
+-rw-r--r--   0        0        0      308 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/middleware.py
+-rw-r--r--   0        0        0     8577 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/models.py
+-rw-r--r--   0        0        0     2344 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/runtime.py
+-rw-r--r--   0        0        0     1085 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/utils.py
+-rw-r--r--   0        0        0      155 2023-06-08 21:42:12.696383 django_pgactivity-1.2.0/pgactivity/version.py
+-rw-r--r--   0        0        0     2400 2023-06-08 21:42:44.556468 django_pgactivity-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     5477 1970-01-01 00:00:00.000000 django_pgactivity-1.2.0/PKG-INFO
```

### Comparing `django-pgactivity-1.1.1/LICENSE` & `django_pgactivity-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-pgactivity-1.1.1/README.rst` & `django_pgactivity-1.2.0/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
     def my_operation():
         # Any queries in this operation that take over 500 milliseconds will throw
         # django.db.utils.OperationalError.
 
 Compatibility
 =============
 
-``django-pgactivity`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 15.
+``django-pgactivity`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
 
 Documentation
 =============
 
 `View the django-pgactivity docs here
 <https://django-pgactivity.readthedocs.io/>`_ to learn more about:
```

### Comparing `django-pgactivity-1.1.1/pgactivity/config.py` & `django_pgactivity-1.2.0/pgactivity/config.py`

 * *Files identical despite different names*

### Comparing `django-pgactivity-1.1.1/pgactivity/contrib.py` & `django_pgactivity-1.2.0/pgactivity/contrib.py`

 * *Files identical despite different names*

### Comparing `django-pgactivity-1.1.1/pgactivity/core.py` & `django_pgactivity-1.2.0/pgactivity/core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,21 @@
 import contextlib
 import datetime as dt
 import threading
 
 from django.db import connections, DEFAULT_DB_ALIAS
-import psycopg2.extensions
+
+from pgactivity import utils
+
+if utils.psycopg_maj_version == 2:
+    import psycopg2.extensions
+elif utils.psycopg_maj_version == 3:
+    import psycopg.pq
+else:
+    raise AssertionError
 
 
 _timeout = threading.local()
 _unset = object()
 
 
 def _cast_timeout(timeout):
@@ -19,14 +27,29 @@
 
     if timeout < dt.timedelta(milliseconds=1):
         timeout = dt.timedelta()
 
     return timeout
 
 
+def _is_transaction_errored(cursor):
+    """
+    True if the current transaction is in an errored state
+    """
+    if utils.psycopg_maj_version == 2:
+        return (
+            cursor.connection.get_transaction_status()
+            == psycopg2.extensions.TRANSACTION_STATUS_INERROR
+        )
+    elif utils.psycopg_maj_version == 3:
+        return cursor.connection.info.transaction_status == psycopg.pq.TransactionStatus.INERROR
+    else:
+        raise AssertionError
+
+
 @contextlib.contextmanager
 def timeout(timeout=_unset, *, using=DEFAULT_DB_ALIAS, **timedelta_kwargs):
     """Set the statement timeout as a decorator or context manager.
 
     A value of ``None`` will set an infinite statement timeout.
     A value of less than a millisecond is not permitted.
 
@@ -68,28 +91,27 @@
         _timeout.value = None
 
     old_timeout = _timeout.value
     _timeout.value = int(timeout.total_seconds() * 1000)
 
     try:
         with connections[using].cursor() as cursor:
-            cursor.execute(f"SET statement_timeout={_timeout.value}")
+            cursor.execute(f"SELECT set_config('statement_timeout', '{_timeout.value}', false)")
             yield
     finally:
         _timeout.value = old_timeout
 
         with connections[using].cursor() as cursor:
-            if (
-                not cursor.connection.get_transaction_status()
-                == psycopg2.extensions.TRANSACTION_STATUS_INERROR
-            ):
+            if not _is_transaction_errored(cursor):
                 if _timeout.value is None:
-                    cursor.execute("RESET statement_timeout")
+                    cursor.execute("SELECT set_config('statement_timeout', NULL, false)")
                 else:
-                    cursor.execute(f"SET statement_timeout={_timeout.value}")
+                    cursor.execute(
+                        f"SELECT set_config('statement_timeout', '{_timeout.value}', false)"
+                    )
 
 
 def _pg_backend_method(method, pids, using):
     assert method in ("cancel", "terminate")
 
     if pids:
         with connections[using].cursor() as cursor:
```

### Comparing `django-pgactivity-1.1.1/pgactivity/management/commands/pgactivity.py` & `django_pgactivity-1.2.0/pgactivity/management/commands/pgactivity.py`

 * *Files identical despite different names*

### Comparing `django-pgactivity-1.1.1/pgactivity/models.py` & `django_pgactivity-1.2.0/pgactivity/models.py`

 * *Files identical despite different names*

### Comparing `django-pgactivity-1.1.1/pgactivity/runtime.py` & `django_pgactivity-1.2.0/pgactivity/runtime.py`

 * *Files identical despite different names*

### Comparing `django-pgactivity-1.1.1/pyproject.toml` & `django_pgactivity-1.2.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 name = "django-pgactivity"
 packages = [
   { include = "pgactivity" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "1.1.1"
+version = "1.2.0"
 description = "Monitor, kill, and analyze Postgres queries."
 authors = ["Opus 10 Engineering"]
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
 homepage = "https://github.com/Opus10/django-pgactivity"
 repository = "https://github.com/Opus10/django-pgactivity"
@@ -66,22 +67,21 @@
 django-extensions = "3.2.1"
 flake8 = "3.9.2"
 flake8-bugbear = "22.1.11"
 flake8-comprehensions = "3.8.0"
 flake8-import-order = "0.18.1"
 flake8-logging-format = "0.6.0"
 flake8-mutable = "1.2.0"
-git-tidy = "1.1.2"
-ipython = { version = "8.5.0", python = ">=3.8" }
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
 pytest-mock = "3.10.0"
 pytest-reraise = "2.1.2"
 requests = "2.25.1"
```

### Comparing `django-pgactivity-1.1.1/setup.py` & `django_pgactivity-1.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,153 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: django-pgactivity
+Version: 1.2.0
+Summary: Monitor, kill, and analyze Postgres queries.
+Home-page: https://github.com/Opus10/django-pgactivity
+License: BSD-3-Clause
+Author: Opus 10 Engineering
+Requires-Python: >=3.7.0,<4
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
+Classifier: Framework :: Django :: 4.0
+Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Dist: django (>=2)
+Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
+Project-URL: Documentation, https://django-pgactivity.readthedocs.io
+Project-URL: Repository, https://github.com/Opus10/django-pgactivity
+Description-Content-Type: text/x-rst
 
-packages = \
-['pgactivity', 'pgactivity.management', 'pgactivity.management.commands']
+django-pgactivity
+#################
 
-package_data = \
-{'': ['*']}
+``django-pgactivity`` makes it easy to view, filter, and kill
+active Postgres queries.
 
-install_requires = \
-['django>=2']
-
-extras_require = \
-{':python_version >= "3.7" and python_version < "3.8"': ['importlib_metadata>=4']}
-
-setup_kwargs = {
-    'name': 'django-pgactivity',
-    'version': '1.1.1',
-    'description': 'Monitor, kill, and analyze Postgres queries.',
-    'long_description': 'django-pgactivity\n#################\n\n``django-pgactivity`` makes it easy to view, filter, and kill\nactive Postgres queries.\n\nSome of the features at a glance:\n\n* The ``PGActivity`` proxy model and ``pgactivity`` management command\n  for querying and filtering the `Postgres pg_stat_activity view <https://www.postgresql.org/docs/current/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW>`__.\n* ``pgactivity.context`` and ``pgactivity.middleware.ActivityMiddleware``\n  for annotating queries with application metadata, such as the request URL.\n* ``pgactivity.cancel`` and ``pgactivity.terminate`` for canceling\n  and terminating queries. The ``PGActivity`` model manager also has\n  these methods.\n* ``pgactivity.timeout`` for dynamically setting the statement timeout.\n\nQuick Start\n===========\n\nBasic Command Usage\n-------------------\n\nUse ``python manage.py pgactivity`` to view and filter active queries. Output looks like the following::\n\n    39225 | 0:01:32 | IDLE_IN_TRANSACTION | None | lock auth_user in access exclusiv\n    39299 | 0:00:15 | ACTIVE | None | SELECT "auth_user"."id", "auth_user"."password\n    39315 | 0:00:00 | ACTIVE | None | WITH _pgactivity_activity_cte AS ( SELECT pid\n\nThe default output attributes are:\n\n1. The process ID of the connection.\n2. The duration of the query.\n3. The state of the query (see the `Postgres docs <https://www.postgresql.org/docs/current/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW>`__ for values).\n4. Attached context using ``pgactivity.context``.\n5. The query SQL.\n\nApply filters with ``-f`` (or ``--filter``). Here we query for all active queries that have a duration\nlonger than a minute::\n\n    python manage.py pgactivity -f state=ACTIVE -f \'duration__gt=1 minute\'\n\nCancel or terminate activity with ``--cancel`` or ``--terminate``.\nHere we terminate a query based on the process ID::\n\n    python manage.py pgactivity 39225 --terminate\n\nAttaching Context\n-----------------\n\nYou can attach context to queries to better understand where they originate\nusing ``pgactivity.context`` or by adding ``pgactivity.middleware.ActivityMiddleware``\nto ``settings.MIDDLEWARE``.\nUnderneath the hood, a comment is added to the SQL statement and surfaced in\n``django-pgactivity``.\n\nWhen using the middleware, the ``url`` of the request and the ``method`` of\nthe request are automatically added. Here\'s what the output looks like\nwhen using the ``pgactivity`` command::\n\n    39299 | 0:00:15 | ACTIVE | {"url": "/admin/", "method": "GET"} | SELECT "auth_use\n\nProxy Model\n-----------\n\nUse the ``pgactivity.models.PGActivity`` proxy model to query\nthe `Postgres pg_stat_activity view <https://www.postgresql.org/docs/current/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW>`__.\nThe model contains most of the fields from the view, and the ``cancel`` and ``terminate``\nmethods can be applied to the queryset.\n\nSetting the Statement Timeout\n-----------------------------\n\nDynamically set the SQL statement timeout of code using ``pgactivity.timeout``:\n\n.. code-block:: python\n\n    import pgactivity\n\n    @pgactivity.timeout(0.5)\n    def my_operation():\n        # Any queries in this operation that take over 500 milliseconds will throw\n        # django.db.utils.OperationalError.\n\nCompatibility\n=============\n\n``django-pgactivity`` is compatible with Python 3.7 - 3.10, Django 2.2 - 4.1, and Postgres 10 - 15.\n\nDocumentation\n=============\n\n`View the django-pgactivity docs here\n<https://django-pgactivity.readthedocs.io/>`_ to learn more about:\n\n\n* The proxy models and custom queryset methods.\n* Attaching application context to queries.\n* Using and configuring the management command.\n* Setting dynamic statement timeouts.\n\nInstallation\n============\n\nInstall django-pgactivity with::\n\n    pip3 install django-pgactivity\n\nAfter this, add ``pgactivity`` to the ``INSTALLED_APPS``\nsetting of your Django project.\n\nContributing Guide\n==================\n\nFor information on setting up django-pgactivity for development and\ncontributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.\n\nPrimary Authors\n===============\n\n- `Wes Kendall <https://github.com/wesleykendall>`__\n- `Paul Gilmartin <https://github.com/PaulGilmartin>`__\n',
-    'author': 'Opus 10 Engineering',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/Opus10/django-pgactivity',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.7.0,<4',
-}
+Some of the features at a glance:
 
+* The ``PGActivity`` proxy model and ``pgactivity`` management command
+  for querying and filtering the `Postgres pg_stat_activity view <https://www.postgresql.org/docs/current/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW>`__.
+* ``pgactivity.context`` and ``pgactivity.middleware.ActivityMiddleware``
+  for annotating queries with application metadata, such as the request URL.
+* ``pgactivity.cancel`` and ``pgactivity.terminate`` for canceling
+  and terminating queries. The ``PGActivity`` model manager also has
+  these methods.
+* ``pgactivity.timeout`` for dynamically setting the statement timeout.
+
+Quick Start
+===========
+
+Basic Command Usage
+-------------------
+
+Use ``python manage.py pgactivity`` to view and filter active queries. Output looks like the following::
+
+    39225 | 0:01:32 | IDLE_IN_TRANSACTION | None | lock auth_user in access exclusiv
+    39299 | 0:00:15 | ACTIVE | None | SELECT "auth_user"."id", "auth_user"."password
+    39315 | 0:00:00 | ACTIVE | None | WITH _pgactivity_activity_cte AS ( SELECT pid
+
+The default output attributes are:
+
+1. The process ID of the connection.
+2. The duration of the query.
+3. The state of the query (see the `Postgres docs <https://www.postgresql.org/docs/current/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW>`__ for values).
+4. Attached context using ``pgactivity.context``.
+5. The query SQL.
+
+Apply filters with ``-f`` (or ``--filter``). Here we query for all active queries that have a duration
+longer than a minute::
+
+    python manage.py pgactivity -f state=ACTIVE -f 'duration__gt=1 minute'
+
+Cancel or terminate activity with ``--cancel`` or ``--terminate``.
+Here we terminate a query based on the process ID::
+
+    python manage.py pgactivity 39225 --terminate
+
+Attaching Context
+-----------------
+
+You can attach context to queries to better understand where they originate
+using ``pgactivity.context`` or by adding ``pgactivity.middleware.ActivityMiddleware``
+to ``settings.MIDDLEWARE``.
+Underneath the hood, a comment is added to the SQL statement and surfaced in
+``django-pgactivity``.
+
+When using the middleware, the ``url`` of the request and the ``method`` of
+the request are automatically added. Here's what the output looks like
+when using the ``pgactivity`` command::
+
+    39299 | 0:00:15 | ACTIVE | {"url": "/admin/", "method": "GET"} | SELECT "auth_use
+
+Proxy Model
+-----------
+
+Use the ``pgactivity.models.PGActivity`` proxy model to query
+the `Postgres pg_stat_activity view <https://www.postgresql.org/docs/current/monitoring-stats.html#MONITORING-PG-STAT-ACTIVITY-VIEW>`__.
+The model contains most of the fields from the view, and the ``cancel`` and ``terminate``
+methods can be applied to the queryset.
+
+Setting the Statement Timeout
+-----------------------------
+
+Dynamically set the SQL statement timeout of code using ``pgactivity.timeout``:
+
+.. code-block:: python
+
+    import pgactivity
+
+    @pgactivity.timeout(0.5)
+    def my_operation():
+        # Any queries in this operation that take over 500 milliseconds will throw
+        # django.db.utils.OperationalError.
+
+Compatibility
+=============
+
+``django-pgactivity`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
+Documentation
+=============
+
+`View the django-pgactivity docs here
+<https://django-pgactivity.readthedocs.io/>`_ to learn more about:
+
+
+* The proxy models and custom queryset methods.
+* Attaching application context to queries.
+* Using and configuring the management command.
+* Setting dynamic statement timeouts.
+
+Installation
+============
+
+Install django-pgactivity with::
+
+    pip3 install django-pgactivity
+
+After this, add ``pgactivity`` to the ``INSTALLED_APPS``
+setting of your Django project.
+
+Contributing Guide
+==================
+
+For information on setting up django-pgactivity for development and
+contributing changes, view `CONTRIBUTING.rst <CONTRIBUTING.rst>`_.
+
+Primary Authors
+===============
+
+- `Wes Kendall <https://github.com/wesleykendall>`__
+- `Paul Gilmartin <https://github.com/PaulGilmartin>`__
 
-setup(**setup_kwargs)
```

