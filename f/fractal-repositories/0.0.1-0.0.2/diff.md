# Comparing `tmp/fractal-repositories-0.0.1.tar.gz` & `tmp/fractal_repositories-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal-repositories-0.0.1.tar", last modified: Tue May  9 08:14:00 2023, max compression
+gzip compressed data, was "fractal_repositories-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `fractal-repositories-0.0.1.tar` & `fractal_repositories-0.0.2.tar`

### file list

```diff
@@ -1,71 +1,71 @@
--rw-r--r--   0        0        0      187 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.coveragerc
--rw-r--r--   0        0        0      100 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.flake8
--rw-r--r--   0        0        0      945 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.github/workflows/build.yml
--rw-r--r--   0        0        0      662 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0      832 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.gitignore
--rw-r--r--   0        0        0      161 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.isort.cfg
--rw-r--r--   0        0        0       43 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.mypy.ini
--rw-r--r--   0        0        0     1699 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1075 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/LICENSE
--rw-r--r--   0        0        0     1557 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/Makefile
--rw-r--r--   0        0        0     2276 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/README.md
--rw-r--r--   0        0        0      780 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/align_version.py
--rw-r--r--   0        0        0      182 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/fractal_repositories/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/fractal_repositories/contrib/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.478601 fractal-repositories-0.0.1/fractal_repositories/contrib/django/__init__.py
--rw-r--r--   0        0        0     3291 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/django/mixins.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/elastic/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/gcp/__init__.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/gcp/firestore/__init__.py
--rw-r--r--   0        0        0     4991 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/gcp/firestore/mixins.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/mongo/__init__.py
--rw-r--r--   0        0        0     3240 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/mongo/mixins.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/sqlalchemy/__init__.py
--rw-r--r--   0        0        0    11960 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/contrib/sqlalchemy/mixins.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/core/__init__.py
--rw-r--r--   0        0        0     1419 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/core/entity.py
--rw-r--r--   0        0        0     2434 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/core/repositories.py
--rw-r--r--   0        0        0      343 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/mixins/__init__.py
--rw-r--r--   0        0        0     1219 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0     2965 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/mixins/file_repository_mixin.py
--rw-r--r--   0        0        0      957 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/mixins/filter_repository_mixin.py
--rw-r--r--   0        0        0     3044 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/mixins/inmemory_repository_mixin.py
--rw-r--r--   0        0        0       77 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/py.typed
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/utils/__init__.py
--rw-r--r--   0        0        0     2299 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/utils/cached_repository.py
--rw-r--r--   0        0        0     2381 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/utils/distributed_read_repository.py
--rw-r--r--   0        0        0      636 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/fractal_repositories/utils/json_encoder.py
--rw-r--r--   0        0        0      235 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/poetry.lock
--rw-r--r--   0        0        0     1667 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/pyproject.toml
--rw-r--r--   0        0        0       69 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/setup.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/__init__.py
--rw-r--r--   0        0        0       37 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/contrib/__init__.py
--rw-r--r--   0        0        0     4177 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/contrib/test_django.py
--rw-r--r--   0        0        0     4438 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/contrib/test_firestore.py
--rw-r--r--   0        0        0     4100 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/contrib/test_mongo.py
--rw-r--r--   0        0        0    12220 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/contrib/test_sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/core/__init__.py
--rw-r--r--   0        0        0     3168 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/core/test_models.py
--rw-r--r--   0        0        0     1046 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/core/test_repositories.py
--rw-r--r--   0        0        0      232 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/fixtures/__init__.py
--rw-r--r--   0        0        0     2164 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/fixtures/django/__init__.py
--rw-r--r--   0        0        0      643 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/fixtures/django/models.py
--rw-r--r--   0        0        0     1126 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/fixtures/firestore.py
--rw-r--r--   0        0        0      888 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/fixtures/mongo.py
--rw-r--r--   0        0        0     6786 2023-05-09 08:13:19.482601 fractal-repositories-0.0.1/tests/fixtures/repositories.py
--rw-r--r--   0        0        0     7674 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/fixtures/sqlalchemy.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/__init__.py
--rw-r--r--   0        0        0     1154 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/test_external_data_inmemory_repository_mixin.py
--rw-r--r--   0        0        0      601 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/test_file_file_repository_mixin.py
--rw-r--r--   0        0        0     3764 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/test_file_repository_mixin.py
--rw-r--r--   0        0        0     3542 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/test_filter_repository_mixin.py
--rw-r--r--   0        0        0      827 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/test_inmemory_file_repository_mixin.py
--rw-r--r--   0        0        0     3150 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/mixins/test_inmemory_repository_mixin.py
--rw-r--r--   0        0        0        0 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     4025 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/utils/test_cached_repository.py
--rw-r--r--   0        0        0     2381 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/utils/test_distributed_read_repository.py
--rw-r--r--   0        0        0      996 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tests/utils/test_json_encoder.py
--rw-r--r--   0        0        0      826 2023-05-09 08:13:19.486601 fractal-repositories-0.0.1/tox.ini
--rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal-repositories-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      187 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.coveragerc
+-rw-r--r--   0        0        0      100 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.flake8
+-rw-r--r--   0        0        0      945 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0      662 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      832 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.gitignore
+-rw-r--r--   0        0        0      161 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.isort.cfg
+-rw-r--r--   0        0        0       43 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.mypy.ini
+-rw-r--r--   0        0        0     1691 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1075 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1557 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/Makefile
+-rw-r--r--   0        0        0     2276 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/README.md
+-rw-r--r--   0        0        0      780 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/align_version.py
+-rw-r--r--   0        0        0      182 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/django/__init__.py
+-rw-r--r--   0        0        0     3291 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/django/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/elastic/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.673841 fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/firestore/__init__.py
+-rw-r--r--   0        0        0     5051 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/firestore/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/mongo/__init__.py
+-rw-r--r--   0        0        0     3253 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/mongo/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/sqlalchemy/__init__.py
+-rw-r--r--   0        0        0    11960 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/contrib/sqlalchemy/mixins.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/core/__init__.py
+-rw-r--r--   0        0        0     1451 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/core/entity.py
+-rw-r--r--   0        0        0     2434 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/core/repositories.py
+-rw-r--r--   0        0        0      343 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/__init__.py
+-rw-r--r--   0        0        0     1219 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0     2965 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/file_repository_mixin.py
+-rw-r--r--   0        0        0      957 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/filter_repository_mixin.py
+-rw-r--r--   0        0        0     3044 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/mixins/inmemory_repository_mixin.py
+-rw-r--r--   0        0        0       77 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/py.typed
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/__init__.py
+-rw-r--r--   0        0        0     2299 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/distributed_read_repository.py
+-rw-r--r--   0        0        0      636 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/fractal_repositories/utils/json_encoder.py
+-rw-r--r--   0        0        0      235 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/poetry.lock
+-rw-r--r--   0        0        0     1667 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       69 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/setup.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/__init__.py
+-rw-r--r--   0        0        0       37 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/__init__.py
+-rw-r--r--   0        0        0     4177 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_django.py
+-rw-r--r--   0        0        0     4438 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_firestore.py
+-rw-r--r--   0        0        0     4100 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_mongo.py
+-rw-r--r--   0        0        0    12220 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/contrib/test_sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/core/__init__.py
+-rw-r--r--   0        0        0     3168 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/core/test_models.py
+-rw-r--r--   0        0        0     1046 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/core/test_repositories.py
+-rw-r--r--   0        0        0      232 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/__init__.py
+-rw-r--r--   0        0        0     2164 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/django/__init__.py
+-rw-r--r--   0        0        0      643 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/django/models.py
+-rw-r--r--   0        0        0     1126 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/firestore.py
+-rw-r--r--   0        0        0      888 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/mongo.py
+-rw-r--r--   0        0        0     6786 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/repositories.py
+-rw-r--r--   0        0        0     7674 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/fixtures/sqlalchemy.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/__init__.py
+-rw-r--r--   0        0        0     1154 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_external_data_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0      601 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_file_file_repository_mixin.py
+-rw-r--r--   0        0        0     3764 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_file_repository_mixin.py
+-rw-r--r--   0        0        0     3542 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_filter_repository_mixin.py
+-rw-r--r--   0        0        0      827 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_inmemory_file_repository_mixin.py
+-rw-r--r--   0        0        0     3150 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/mixins/test_inmemory_repository_mixin.py
+-rw-r--r--   0        0        0        0 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/__init__.py
+-rw-r--r--   0        0        0     4025 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/test_cached_repository.py
+-rw-r--r--   0        0        0     2381 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/test_distributed_read_repository.py
+-rw-r--r--   0        0        0      996 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tests/utils/test_json_encoder.py
+-rw-r--r--   0        0        0      826 2023-06-08 07:39:25.677841 fractal_repositories-0.0.2/tox.ini
+-rw-r--r--   0        0        0     3195 1970-01-01 00:00:00.000000 fractal_repositories-0.0.2/PKG-INFO
```

### Comparing `fractal-repositories-0.0.1/.github/workflows/build.yml` & `fractal_repositories-0.0.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/.github/workflows/publish.yml` & `fractal_repositories-0.0.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/.gitignore` & `fractal_repositories-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/.pre-commit-config.yaml` & `fractal_repositories-0.0.2/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 repos:
-#  - repo: local
-#    hooks:
-#      - id: package-version
-#        name: Update package version
-#        entry: bash -c 'if ! git diff --cached | grep "+version" && ! git diff | grep "+version"; then poetry version patch; fi'
-#        language: system
-#        pass_filenames: false
-#        always_run: true
+  - repo: local
+    hooks:
+      - id: package-version
+        name: Update package version
+        entry: bash -c 'if ! git diff --cached | grep "+version" && ! git diff | grep "+version"; then poetry version patch; fi'
+        language: system
+        pass_filenames: false
+        always_run: true
   - repo: local
     hooks:
       - id: align-version
         name: Align package version
         entry: python align_version.py fractal_repositories
         language: system
         pass_filenames: false
```

### Comparing `fractal-repositories-0.0.1/LICENSE` & `fractal_repositories-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/Makefile` & `fractal_repositories-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/README.md` & `fractal_repositories-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/align_version.py` & `fractal_repositories-0.0.2/align_version.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/contrib/django/mixins.py` & `fractal_repositories-0.0.2/fractal_repositories/contrib/django/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/contrib/gcp/firestore/mixins.py` & `fractal_repositories-0.0.2/fractal_repositories/contrib/gcp/firestore/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
     FirestoreSpecificationBuilder,
 )
 from fractal_specifications.generic.specification import Specification
 from google.cloud.firestore_v1 import Client, Query
 from google.cloud.firestore_v1.base_collection import BaseCollectionReference
 from google.cloud.firestore_v1.base_query import BaseQuery
 
+from fractal_repositories.core.entity import Entity
 from fractal_repositories.core.repositories import EntityType, Repository
 
 
 class FirestoreClient(object):
     instance = None
 
     def __new__(cls, *args, **kwargs):
@@ -49,15 +50,15 @@
 
 
 class FirestoreRepositoryMixin(Repository[EntityType]):
     """
     https://github.com/GoogleCloudPlatform/python-docs-samples/blob/46fa5a588858021ea32350584a4ee178cd7c1f33/firestore/cloud-client/snippets.py#L62-L66
     """
 
-    entity = EntityType
+    entity: EntityType = Entity
 
     def __init__(self, collection: str = "", *, collection_prefix: str = ""):
         super(FirestoreRepositoryMixin, self).__init__()
 
         client: Client = FirestoreClient().get_firestore_client()
         if not collection:
             collection = self.entity.__name__
```

### Comparing `fractal-repositories-0.0.1/fractal_repositories/contrib/mongo/mixins.py` & `fractal_repositories-0.0.2/fractal_repositories/contrib/mongo/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 def setup_mongo_connection(
     host, port, username, password, database
 ) -> Tuple[MongoClient, Database]:
     if host == "mongo-mock":
         import mongomock
 
-        client = mongomock.MongoClient()
+        client: MongoClient = mongomock.MongoClient()
     else:
         if username:
             connection_string = f"mongodb+srv://{username}:{password}@{host}/{database}"
         else:
             connection_string = f"mongodb://{host}:{port}/{database}"
         connection_string += "?retryWrites=true&w=majority&connect=false"
         client = MongoClient(connection_string)
```

### Comparing `fractal-repositories-0.0.1/fractal_repositories/contrib/sqlalchemy/mixins.py` & `fractal_repositories-0.0.2/fractal_repositories/contrib/sqlalchemy/mixins.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/core/entity.py` & `fractal_repositories-0.0.2/fractal_repositories/core/entity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 from dataclasses import dataclass, fields
 from datetime import date
 from decimal import Decimal
 from typing import Any, Dict
 
 
 @dataclass
-class Entity:
-    id: Any
-
+class Model:
     @classmethod
     def clean(cls, **kwargs):
         field_names = set(f.name for f in fields(cls))
         return cls(**{k: v for k, v in kwargs.items() if k in field_names})  # NOQA
 
     @classmethod
     def from_dict(cls, data):
@@ -42,7 +40,12 @@
 
         ret = {k: _asdict(v) for k, v in self.__dict__.items() if k in field_names}
         return ret
 
     @staticmethod
     def calculated_fields():
         return []
+
+
+@dataclass
+class Entity(Model):
+    id: Any
```

### Comparing `fractal-repositories-0.0.1/fractal_repositories/core/repositories.py` & `fractal_repositories-0.0.2/fractal_repositories/core/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.2/fractal_repositories/mixins/external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/mixins/file_repository_mixin.py` & `fractal_repositories-0.0.2/fractal_repositories/mixins/file_repository_mixin.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,20 @@
         if current or upsert:
             if current:
                 self.remove_one(Specification.parse(id=current.id))
             return self.add(entity)
         raise self._object_not_found()
 
     def remove_one(self, specification: Specification):
+        super().remove_one(specification)
         entities = list(self.find(NotSpecification(specification)))
         with open(self._filename, "w") as fp:
             fp.writelines(
                 [json.dumps(e.asdict(), cls=EnhancedEncoder) + "\n" for e in entities]
             )
-        super().remove_one(specification)
 
 
 class FileFileRepositoryMixin(RootDirMixin, FileRepository):
     def upload_file(self, data: bytes, content_type: str, reference: str = "") -> str:
         if not reference:
             reference = str(uuid.uuid4())
         with open(os.path.join(self.root_dir, "media", reference), "wb") as fp:
```

### Comparing `fractal-repositories-0.0.1/fractal_repositories/mixins/filter_repository_mixin.py` & `fractal_repositories-0.0.2/fractal_repositories/mixins/filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/mixins/inmemory_repository_mixin.py` & `fractal_repositories-0.0.2/fractal_repositories/mixins/inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/utils/cached_repository.py` & `fractal_repositories-0.0.2/fractal_repositories/utils/cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/utils/distributed_read_repository.py` & `fractal_repositories-0.0.2/fractal_repositories/utils/distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/fractal_repositories/utils/json_encoder.py` & `fractal_repositories-0.0.2/fractal_repositories/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/pyproject.toml` & `fractal_repositories-0.0.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-repositories"
-version = "0.0.1"
+version = "0.0.2"
 description = "Fractal Repositories is an implementation of the repository pattern for building SOLID logic for your Python applications."
 authors = ["Douwe van der Meij <douwe@karibu-online.nl>"]
 
 [build-system]
 requires = ["flit_core >=2,<4"]
 build-backend = "flit_core.buildapi"
```

### Comparing `fractal-repositories-0.0.1/tests/contrib/test_django.py` & `fractal_repositories-0.0.2/tests/contrib/test_django.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/contrib/test_firestore.py` & `fractal_repositories-0.0.2/tests/contrib/test_firestore.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/contrib/test_mongo.py` & `fractal_repositories-0.0.2/tests/contrib/test_mongo.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/contrib/test_sqlalchemy.py` & `fractal_repositories-0.0.2/tests/contrib/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/core/test_models.py` & `fractal_repositories-0.0.2/tests/core/test_models.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/core/test_repositories.py` & `fractal_repositories-0.0.2/tests/core/test_repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/fixtures/django/__init__.py` & `fractal_repositories-0.0.2/tests/fixtures/django/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/fixtures/django/models.py` & `fractal_repositories-0.0.2/tests/fixtures/django/models.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/fixtures/firestore.py` & `fractal_repositories-0.0.2/tests/fixtures/firestore.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/fixtures/mongo.py` & `fractal_repositories-0.0.2/tests/fixtures/mongo.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/fixtures/repositories.py` & `fractal_repositories-0.0.2/tests/fixtures/repositories.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/fixtures/sqlalchemy.py` & `fractal_repositories-0.0.2/tests/fixtures/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/mixins/test_external_data_inmemory_repository_mixin.py` & `fractal_repositories-0.0.2/tests/mixins/test_external_data_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/mixins/test_file_file_repository_mixin.py` & `fractal_repositories-0.0.2/tests/mixins/test_file_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/mixins/test_file_repository_mixin.py` & `fractal_repositories-0.0.2/tests/mixins/test_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/mixins/test_filter_repository_mixin.py` & `fractal_repositories-0.0.2/tests/mixins/test_filter_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/mixins/test_inmemory_file_repository_mixin.py` & `fractal_repositories-0.0.2/tests/mixins/test_inmemory_file_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/mixins/test_inmemory_repository_mixin.py` & `fractal_repositories-0.0.2/tests/mixins/test_inmemory_repository_mixin.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/utils/test_cached_repository.py` & `fractal_repositories-0.0.2/tests/utils/test_cached_repository.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/utils/test_distributed_read_repository.py` & `fractal_repositories-0.0.2/tests/utils/test_distributed_read_repository.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tests/utils/test_json_encoder.py` & `fractal_repositories-0.0.2/tests/utils/test_json_encoder.py`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/tox.ini` & `fractal_repositories-0.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `fractal-repositories-0.0.1/PKG-INFO` & `fractal_repositories-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-repositories
-Version: 0.0.1
+Version: 0.0.2
 Summary: Fractal Repositories is an implementation of the repository pattern of Domain Driven Design (DDD) for building SOLID logic for your Python applications.
 Home-page: https://github.com/douwevandermeij/fractal-repositories
 Author: Douwe van der Meij
 Author-email: douwe@karibu-online.nl
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
```

