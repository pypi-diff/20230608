# Comparing `tmp/django_pgclone-3.0.0.tar.gz` & `tmp/django_pgclone-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pgclone-3.0.0.tar", max compression
+gzip compressed data, was "django_pgclone-3.1.0.tar", max compression
```

## Comparing `django_pgclone-3.0.0.tar` & `django_pgclone-3.1.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1456 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/LICENSE
--rw-r--r--   0        0        0     2372 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/README.rst
--rw-r--r--   0        0        0      196 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/__init__.py
--rw-r--r--   0        0        0     2159 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/copy_cmd.py
--rw-r--r--   0        0        0     6054 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/db.py
--rw-r--r--   0        0        0     3487 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/dump_cmd.py
--rw-r--r--   0        0        0      438 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/exceptions.py
--rw-r--r--   0        0        0     2169 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/logging.py
--rw-r--r--   0        0        0     3521 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/ls_cmd.py
--rw-r--r--   0        0        0        0 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/management/__init__.py
--rw-r--r--   0        0        0        0 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/management/commands/__init__.py
--rw-r--r--   0        0        0     7201 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/management/commands/pgclone.py
--rw-r--r--   0        0        0     2483 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/options.py
--rw-r--r--   0        0        0     9404 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/restore_cmd.py
--rw-r--r--   0        0        0     1559 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/run.py
--rw-r--r--   0        0        0     2220 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/settings.py
--rw-r--r--   0        0        0     3505 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/storage.py
--rw-r--r--   0        0        0      152 2023-06-01 20:40:01.134009 django_pgclone-3.0.0/pgclone/version.py
--rw-r--r--   0        0        0     2333 2023-06-01 20:40:42.926421 django_pgclone-3.0.0/pyproject.toml
--rw-r--r--   0        0        0     3832 1970-01-01 00:00:00.000000 django_pgclone-3.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1456 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/LICENSE
+-rw-r--r--   0        0        0     2513 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/README.rst
+-rw-r--r--   0        0        0      196 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/__init__.py
+-rw-r--r--   0        0        0     2159 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/copy_cmd.py
+-rw-r--r--   0        0        0     6054 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/db.py
+-rw-r--r--   0        0        0     3487 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/dump_cmd.py
+-rw-r--r--   0        0        0      438 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/exceptions.py
+-rw-r--r--   0        0        0     2169 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/logging.py
+-rw-r--r--   0        0        0     3521 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/ls_cmd.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/management/commands/__init__.py
+-rw-r--r--   0        0        0     7201 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/management/commands/pgclone.py
+-rw-r--r--   0        0        0     2483 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/options.py
+-rw-r--r--   0        0        0     9404 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/restore_cmd.py
+-rw-r--r--   0        0        0     1559 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/run.py
+-rw-r--r--   0        0        0     2220 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/settings.py
+-rw-r--r--   0        0        0     3505 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/storage.py
+-rw-r--r--   0        0        0      152 2023-06-08 21:26:05.010583 django_pgclone-3.1.0/pgclone/version.py
+-rw-r--r--   0        0        0     2377 2023-06-08 21:26:37.798847 django_pgclone-3.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3772 1970-01-01 00:00:00.000000 django_pgclone-3.1.0/PKG-INFO
```

### Comparing `django_pgclone-3.0.0/LICENSE` & `django_pgclone-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/README.rst` & `django_pgclone-3.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,19 @@
 the local file system. Dump keys are in
 the format of ``<instance>/<database>/<config>/<timestamp>.dump``.
 
 When listing, use an optional prefix. Restoring
 supports the same interface, using the latest key that matches the
 prefix.
 
+Compatibility
+=============
+
+``django-pgclone`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 `View the django-pgclone docs here
 <https://django-pgclone.readthedocs.io/>`_ to learn more about:
 
 * The basics and an overview of how it works.
```

### Comparing `django_pgclone-3.0.0/pgclone/copy_cmd.py` & `django_pgclone-3.1.0/pgclone/copy_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/db.py` & `django_pgclone-3.1.0/pgclone/db.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/dump_cmd.py` & `django_pgclone-3.1.0/pgclone/dump_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/logging.py` & `django_pgclone-3.1.0/pgclone/logging.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/ls_cmd.py` & `django_pgclone-3.1.0/pgclone/ls_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/management/commands/pgclone.py` & `django_pgclone-3.1.0/pgclone/management/commands/pgclone.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/options.py` & `django_pgclone-3.1.0/pgclone/options.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/restore_cmd.py` & `django_pgclone-3.1.0/pgclone/restore_cmd.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/run.py` & `django_pgclone-3.1.0/pgclone/run.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/settings.py` & `django_pgclone-3.1.0/pgclone/settings.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pgclone/storage.py` & `django_pgclone-3.1.0/pgclone/storage.py`

 * *Files identical despite different names*

### Comparing `django_pgclone-3.0.0/pyproject.toml` & `django_pgclone-3.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,30 +25,31 @@
 name = "django-pgclone"
 packages = [
   { include = "pgclone" }
 ]
 exclude = [
   "*/tests/"
 ]
-version = "3.0.0"
+version = "3.1.0"
 description = "Dump and restore Postgres databases with Django."
 authors = ["Wes Kendall", "Ethan O'Brien"]
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
 homepage = "https://github.com/Opus10/django-pgclone"
 repository = "https://github.com/Opus10/django-pgclone"
@@ -71,15 +72,15 @@
 flake8-mutable = "1.2.0"
 git-tidy = "1.2.0"
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
 pytest-mock = "3.8.2"
 requests = "2.25.1"
 Sphinx = "4.4.0"
```

### Comparing `django_pgclone-3.0.0/PKG-INFO` & `django_pgclone-3.1.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 Metadata-Version: 2.1
 Name: django-pgclone
-Version: 3.0.0
+Version: 3.1.0
 Summary: Dump and restore Postgres databases with Django.
 Home-page: https://github.com/Opus10/django-pgclone
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
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: django (>=2)
 Requires-Dist: importlib_metadata (>=4) ; python_version >= "3.7" and python_version < "3.8"
 Project-URL: Documentation, https://django-pgclone.readthedocs.io
 Project-URL: Repository, https://github.com/Opus10/django-pgclone
 Description-Content-Type: text/x-rst
 
 django-pgclone
@@ -71,14 +67,19 @@
 the local file system. Dump keys are in
 the format of ``<instance>/<database>/<config>/<timestamp>.dump``.
 
 When listing, use an optional prefix. Restoring
 supports the same interface, using the latest key that matches the
 prefix.
 
+Compatibility
+=============
+
+``django-pgclone`` is compatible with Python 3.7 - 3.11, Django 3.2 - 4.2, Psycopg 2 - 3 and Postgres 12 - 15.
+
 Documentation
 =============
 
 `View the django-pgclone docs here
 <https://django-pgclone.readthedocs.io/>`_ to learn more about:
 
 * The basics and an overview of how it works.
```

