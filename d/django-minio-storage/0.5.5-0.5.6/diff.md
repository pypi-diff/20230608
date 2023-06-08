# Comparing `tmp/django-minio-storage-0.5.5.tar.gz` & `tmp/django-minio-storage-0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-minio-storage-0.5.5.tar", last modified: Wed May 31 06:43:33 2023, max compression
+gzip compressed data, was "django-minio-storage-0.5.6.tar", last modified: Thu Jun  8 16:30:48 2023, max compression
```

## Comparing `django-minio-storage-0.5.5.tar` & `django-minio-storage-0.5.6.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.806151 django-minio-storage-0.5.5/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.806151 django-minio-storage-0.5.5/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/LICENSE-APACHE
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.806151 django-minio-storage-0.5.5/django_minio_storage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/django_minio_storage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docker-compose.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/licences.md
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs/usage.md
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/docs-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/minio_storage/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/files.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/minio_storage/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/minio_storage/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/management/commands/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    16886 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/minio_storage/storage.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-31 06:43:33.000000 django-minio-storage-0.5.5/minio_storage/version.py
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/tests/django_minio_storage_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/django_minio_storage_tests/wsgi.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.810151 django-minio-storage-0.5.5/tests/test_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:33.814151 django-minio-storage-0.5.5/tests/test_app/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/bucket_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/custom_storage_class_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/delete_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/managementcommand_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/retrieve_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/settings_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/upload_tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/test_app/tests/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tests/watermelon-cat.jpg
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-31 06:43:24.000000 django-minio-storage-0.5.5/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.208122 django-minio-storage-0.5.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.196122 django-minio-storage-0.5.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.200122 django-minio-storage-0.5.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3416 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11004 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/LICENSE-APACHE
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-08 16:30:48.208122 django-minio-storage-0.5.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.200122 django-minio-storage-0.5.6/django_minio_storage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-08 16:30:48.000000 django-minio-storage-0.5.6/django_minio_storage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-08 16:30:48.000000 django-minio-storage-0.5.6/django_minio_storage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:30:48.000000 django-minio-storage-0.5.6/django_minio_storage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 16:30:48.000000 django-minio-storage-0.5.6/django_minio_storage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 16:30:48.000000 django-minio-storage-0.5.6/django_minio_storage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docker-compose.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.204122 django-minio-storage-0.5.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)    12348 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docs/licences.md
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docs/usage.md
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/docs-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.204122 django-minio-storage-0.5.6/minio_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/files.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.204122 django-minio-storage-0.5.6/minio_storage/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.204122 django-minio-storage-0.5.6/minio_storage/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8398 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/management/commands/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4108 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16825 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/minio_storage/storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 16:30:48.000000 django-minio-storage-0.5.6/minio_storage/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 16:30:48.208122 django-minio-storage-0.5.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.204122 django-minio-storage-0.5.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.208122 django-minio-storage-0.5.6/tests/django_minio_storage_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/django_minio_storage_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/django_minio_storage_tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/django_minio_storage_tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/django_minio_storage_tests/wsgi.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      283 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.208122 django-minio-storage-0.5.6/tests/test_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:48.208122 django-minio-storage-0.5.6/tests/test_app/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/bucket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4594 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/custom_storage_class_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/delete_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/managementcommand_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9632 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/retrieve_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/settings_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/upload_tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/test_app/tests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79300 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tests/watermelon-cat.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-08 16:30:36.000000 django-minio-storage-0.5.6/tox.ini
```

### Comparing `django-minio-storage-0.5.5/.github/workflows/release.yml` & `django-minio-storage-0.5.6/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/.github/workflows/tox.yml` & `django-minio-storage-0.5.6/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/CHANGELOG.md` & `django-minio-storage-0.5.6/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/LICENSE` & `django-minio-storage-0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/LICENSE-APACHE` & `django-minio-storage-0.5.6/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/PKG-INFO` & `django-minio-storage-0.5.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.5
+Version: 0.5.6
 Summary: Django file storage using the minio python client
 Author-email: Thomas Frössman <thomasf@jossystem.se>, Tom Houlé <tom@kafunsho.be>
 Maintainer-email: Thomas Frössman <thomasf@jossystem.se>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 The django-minio-storage developers
```

### Comparing `django-minio-storage-0.5.5/README.md` & `django-minio-storage-0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/django_minio_storage.egg-info/PKG-INFO` & `django-minio-storage-0.5.6/django_minio_storage.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-minio-storage
-Version: 0.5.5
+Version: 0.5.6
 Summary: Django file storage using the minio python client
 Author-email: Thomas Frössman <thomasf@jossystem.se>, Tom Houlé <tom@kafunsho.be>
 Maintainer-email: Thomas Frössman <thomasf@jossystem.se>
 License: The MIT License (MIT)
         
         Copyright (c) 2016 The django-minio-storage developers
```

### Comparing `django-minio-storage-0.5.5/django_minio_storage.egg-info/SOURCES.txt` & `django-minio-storage-0.5.6/django_minio_storage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/docs/development.md` & `django-minio-storage-0.5.6/docs/development.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/docs/index.md` & `django-minio-storage-0.5.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/docs/licences.md` & `django-minio-storage-0.5.6/docs/licences.md`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/docs/usage.md` & `django-minio-storage-0.5.6/docs/usage.md`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,18 @@
 The following settings are available:
 
 - `MINIO_STORAGE_ENDPOINT`: the access URL for the service (for example
   `minio.example.org:9000` (note that there is no scheme)).
 
 - `MINIO_STORAGE_ACCESS_KEY` and `MINIO_STORAGE_SECRET_KEY` (mandatory)
   
-- `MINIO_STORAGE_REGION`: Allows you to specify the region. By setting this configuration option, an additional HTTP request to Minio for region checking can be prevented, resulting in improved performance and reduced latency for generating presigned URLs.
+- `MINIO_STORAGE_REGION`: Allows you to specify the region. By setting this
+  configuration option, an additional HTTP request to Minio for region checking
+  can be prevented, resulting in improved performance and reduced latency for
+  generating presigned URLs.
 
 - `MINIO_STORAGE_USE_HTTPS`: whether to use TLS or not (default: `True`). This
   affect both how how Django internally communicates with the Minio server AND
   controls if the generated the storage object URLs uses `http://` or
   `https://` schemes.
 
 - `MINIO_STORAGE_MEDIA_BUCKET_NAME`: the bucket that will act as `MEDIA` folder
```

### Comparing `django-minio-storage-0.5.5/minio_storage/files.py` & `django-minio-storage-0.5.6/minio_storage/files.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/minio_storage/management/commands/minio.py` & `django-minio-storage-0.5.6/minio_storage/management/commands/minio.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/minio_storage/policy.py` & `django-minio-storage-0.5.6/minio_storage/policy.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/minio_storage/storage.py` & `django-minio-storage-0.5.6/minio_storage/storage.py`

 * *Files 1% similar despite different names*

```diff
@@ -360,34 +360,33 @@
         # print("Attr {} : {}".format(name, getattr(settings, name, default)))
         raise ImproperlyConfigured
     else:
         return result
 
 
 def create_minio_client_from_settings(*, minio_kwargs=None):
-    kwargs = {}
     endpoint = get_setting("MINIO_STORAGE_ENDPOINT")
-    access_key = get_setting("MINIO_STORAGE_ACCESS_KEY")
-    secret_key = get_setting("MINIO_STORAGE_SECRET_KEY")
-    secure = get_setting("MINIO_STORAGE_USE_HTTPS", True)
+    kwargs = {
+        "access_key": get_setting("MINIO_STORAGE_ACCESS_KEY"),
+        "secret_key": get_setting("MINIO_STORAGE_SECRET_KEY"),
+        "secure": get_setting("MINIO_STORAGE_USE_HTTPS", True),
+    }
     region = get_setting("MINIO_STORAGE_REGION", None)
     if region:
         kwargs["region"] = region
 
     if minio_kwargs:
         kwargs.update(minio_kwargs)
+
     # Making this client deconstructible allows it to be passed directly as
     # an argument to MinioStorage, since Django needs to be able to
     # deconstruct all Storage constructor arguments for Storages referenced in
     # migrations (e.g. when using a custom storage on a FileField).
     client = deconstructible(minio.Minio)(
         endpoint,
-        access_key=access_key,
-        secret_key=secret_key,
-        secure=secure,
         **kwargs,
     )
     return client
 
 
 @deconstructible
 class MinioMediaStorage(MinioStorage):
```

### Comparing `django-minio-storage-0.5.5/pyproject.toml` & `django-minio-storage-0.5.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/django_minio_storage_tests/settings.py` & `django-minio-storage-0.5.6/tests/django_minio_storage_tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/django_minio_storage_tests/urls.py` & `django-minio-storage-0.5.6/tests/django_minio_storage_tests/urls.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/bucket_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/bucket_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/custom_storage_class_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/custom_storage_class_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/delete_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/delete_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/managementcommand_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/managementcommand_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/retrieve_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/retrieve_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/settings_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/settings_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/upload_tests.py` & `django-minio-storage-0.5.6/tests/test_app/tests/upload_tests.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/test_app/tests/utils.py` & `django-minio-storage-0.5.6/tests/test_app/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tests/watermelon-cat.jpg` & `django-minio-storage-0.5.6/tests/watermelon-cat.jpg`

 * *Files identical despite different names*

### Comparing `django-minio-storage-0.5.5/tox.ini` & `django-minio-storage-0.5.6/tox.ini`

 * *Files identical despite different names*

