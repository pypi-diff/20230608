# Comparing `tmp/django-categories-api-0.0.1.tar.gz` & `tmp/django-categories-api-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-categories-api-0.0.1.tar", last modified: Thu Apr 13 14:34:37 2023, max compression
+gzip compressed data, was "django-categories-api-0.0.2.tar", last modified: Thu Jun  8 13:13:21 2023, max compression
```

## Comparing `django-categories-api-0.0.1.tar` & `django-categories-api-0.0.2.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.309781 django-categories-api-0.0.1/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3344 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.changelog-config.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.editorconfig
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.301781 django-categories-api-0.0.1/.github/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.301781 django-categories-api-0.0.1/.github/changelog_templates/
--rw-rw-r--   0 petr      (1000) petr      (1000)      298 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.github/changelog_templates/commit.md.jinja
--rw-rw-r--   0 petr      (1000) petr      (1000)      214 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.github/changelog_templates/version_heading.md.jinja
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/.github/workflows/
--rw-rw-r--   0 petr      (1000) petr      (1000)      878 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.github/workflows/publish-docs.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)     1153 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.github/workflows/publish-package.yml
--rw-rw-r--   0 petr      (1000) petr      (1000)     1283 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.github/workflows/publish-package.yml.orig
--rw-rw-r--   0 petr      (1000) petr      (1000)     1180 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.github/workflows/run-tests.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)     2523 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.gitignore
--rw-rw-r--   0 petr      (1000) petr      (1000)     1507 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/.pre-commit-config.yaml
--rw-rw-r--   0 petr      (1000) petr      (1000)       73 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/CHANGELOG.md
--rw-rw-r--   0 petr      (1000) petr      (1000)      589 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/CREDITS.md
--rw-rw-r--   0 petr      (1000) petr      (1000)    11357 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/LICENSE.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      620 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/MANIFEST.in
--rw-rw-r--   0 petr      (1000) petr      (1000)     3168 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/Makefile
--rw-rw-r--   0 petr      (1000) petr      (1000)      298 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/NOTICES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      867 2023-04-13 14:34:37.309781 django-categories-api-0.0.1/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)      426 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/README.md
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/categories_api/
--rw-rw-r--   0 petr      (1000) petr      (1000)       51 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/categories_api/api/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/api/__init__.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/categories_api/api/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/api/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2124 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/api/tests/test_api.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      185 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/api/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3498 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/api/viewsets.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/categories_api/tests/
--rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/tests/__init__.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2124 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/tests/test_api.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      185 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/urls.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     3507 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/categories_api/viewsets.py
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/django_categories_api.egg-info/
--rw-rw-r--   0 petr      (1000) petr      (1000)      867 2023-04-13 14:34:37.000000 django-categories-api-0.0.1/django_categories_api.egg-info/PKG-INFO
--rw-rw-r--   0 petr      (1000) petr      (1000)     2308 2023-04-13 14:34:37.000000 django-categories-api-0.0.1/django_categories_api.egg-info/SOURCES.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-13 14:34:37.000000 django-categories-api-0.0.1/django_categories_api.egg-info/dependency_links.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-04-13 14:34:37.000000 django-categories-api-0.0.1/django_categories_api.egg-info/not-zip-safe
--rw-rw-r--   0 petr      (1000) petr      (1000)       18 2023-04-13 14:34:37.000000 django-categories-api-0.0.1/django_categories_api.egg-info/requires.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       15 2023-04-13 14:34:37.000000 django-categories-api-0.0.1/django_categories_api.egg-info/top_level.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/
--rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/Makefile
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.301781 django-categories-api-0.0.1/doc_src/_static/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/_static/css/
--rw-rw-r--   0 petr      (1000) petr      (1000)      516 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/_static/css/custom.css
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.301781 django-categories-api-0.0.1/doc_src/_templates/
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/_templates/autosummary/
--rw-rw-r--   0 petr      (1000) petr      (1000)      208 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/_templates/autosummary/base.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      672 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/_templates/autosummary/class.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1387 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/_templates/autosummary/module.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/api/
--rw-rw-r--   0 petr      (1000) petr      (1000)       69 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/api/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       10 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/api.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/changelog.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     1999 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/conf.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      903 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/getting_started.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      708 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      865 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/index.rst.orig
--rw-rw-r--   0 petr      (1000) petr      (1000)      411 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/installation.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3091 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/make.bat
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/reference/
--rw-rw-r--   0 petr      (1000) petr      (1000)      135 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/reference/index.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/reference/management_commands.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3269 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/reference/models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     3404 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/reference/settings.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     9483 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/reference/templatetags.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)       43 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/requirements.txt
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/user_guide/
--rw-rw-r--   0 petr      (1000) petr      (1000)     1699 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/adding_the_fields.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     1717 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/admin_settings.rst
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.305781 django-categories-api-0.0.1/doc_src/user_guide/code_examples/
--rw-rw-r--   0 petr      (1000) petr      (1000)      200 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories1.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      233 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories2.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     1185 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories3.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      549 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories4.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      174 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories5.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      411 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories6.py
--rw-rw-r--   0 petr      (1000) petr      (1000)      704 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories7.py
--rw-rw-r--   0 petr      (1000) petr      (1000)     2420 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/custom_categories.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/index.md
--rw-rw-r--   0 petr      (1000) petr      (1000)     4542 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/registering_models.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)     2259 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/usage.rst
--rw-rw-r--   0 petr      (1000) petr      (1000)      837 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/doc_src/user_guide/usage_example_template.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     2852 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/patch
--rw-rw-r--   0 petr      (1000) petr      (1000)     1640 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/pyproject.toml
-drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-04-13 14:34:37.309781 django-categories-api-0.0.1/requirements/
--rw-rw-r--   0 petr      (1000) petr      (1000)       80 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/requirements/dev.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       18 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/requirements/prod.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)      172 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/requirements/test.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/requirements.txt
--rw-rw-r--   0 petr      (1000) petr      (1000)     1389 2023-04-13 14:34:37.309781 django-categories-api-0.0.1/setup.cfg
--rw-rw-r--   0 petr      (1000) petr      (1000)     1421 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/setup.py
--rw-rw-r--   0 petr      (1000) petr      (1000)    23977 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/test.html
--rw-rw-r--   0 petr      (1000) petr      (1000)     1093 2023-04-13 14:34:36.000000 django-categories-api-0.0.1/tox.ini
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.687022 django-categories-api-0.0.2/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3344 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.changelog-config.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      331 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.editorconfig
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.675022 django-categories-api-0.0.2/.github/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.679021 django-categories-api-0.0.2/.github/changelog_templates/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      298 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.github/changelog_templates/commit.md.jinja
+-rw-rw-r--   0 petr      (1000) petr      (1000)      214 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.github/changelog_templates/version_heading.md.jinja
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.679021 django-categories-api-0.0.2/.github/workflows/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      878 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.github/workflows/publish-docs.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1153 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.github/workflows/publish-package.yml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1283 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.github/workflows/publish-package.yml.orig
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1180 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.github/workflows/run-tests.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2523 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.gitignore
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1507 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/.pre-commit-config.yaml
+-rw-rw-r--   0 petr      (1000) petr      (1000)      229 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/CHANGELOG.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)      589 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/CREDITS.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)    11357 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/LICENSE.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      620 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/MANIFEST.in
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3168 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/Makefile
+-rw-rw-r--   0 petr      (1000) petr      (1000)      298 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/NOTICES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1420 2023-06-08 13:13:21.687022 django-categories-api-0.0.2/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1055 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/README.md
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/categories_api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       51 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/categories_api/api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/api/__init__.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/categories_api/api/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/api/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2124 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/api/tests/test_api.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      185 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/api/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3498 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/api/viewsets.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/categories_api/tests/
+-rw-rw-r--   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/tests/__init__.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2144 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/tests/test_api.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      185 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/urls.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3790 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/categories_api/viewsets.py
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/django_categories_api.egg-info/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1420 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/django_categories_api.egg-info/PKG-INFO
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2308 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/django_categories_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/django_categories_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)        1 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/django_categories_api.egg-info/not-zip-safe
+-rw-rw-r--   0 petr      (1000) petr      (1000)       18 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/django_categories_api.egg-info/requires.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       15 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/django_categories_api.egg-info/top_level.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/doc_src/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3170 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/Makefile
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.679021 django-categories-api-0.0.2/doc_src/_static/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/doc_src/_static/css/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      516 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/_static/css/custom.css
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.679021 django-categories-api-0.0.2/doc_src/_templates/
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/doc_src/_templates/autosummary/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      208 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/_templates/autosummary/base.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      672 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/_templates/autosummary/class.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1387 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/_templates/autosummary/module.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/doc_src/api/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       69 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/api/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       10 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/api.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       33 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/changelog.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1999 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/conf.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      903 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/getting_started.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      708 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      865 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/index.rst.orig
+-rw-rw-r--   0 petr      (1000) petr      (1000)      411 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/installation.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3091 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/make.bat
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.683022 django-categories-api-0.0.2/doc_src/reference/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      135 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/reference/index.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1024 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/reference/management_commands.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3269 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/reference/models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     3404 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/reference/settings.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     9483 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/reference/templatetags.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)       43 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/requirements.txt
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.687022 django-categories-api-0.0.2/doc_src/user_guide/
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1699 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/adding_the_fields.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1717 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/admin_settings.rst
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.687022 django-categories-api-0.0.2/doc_src/user_guide/code_examples/
+-rw-rw-r--   0 petr      (1000) petr      (1000)      200 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories1.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      233 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories2.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1185 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories3.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      549 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories4.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      174 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories5.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      411 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories6.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)      704 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories7.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2420 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/custom_categories.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      127 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/index.md
+-rw-rw-r--   0 petr      (1000) petr      (1000)     4542 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/registering_models.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2259 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/usage.rst
+-rw-rw-r--   0 petr      (1000) petr      (1000)      837 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/doc_src/user_guide/usage_example_template.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     2852 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/patch
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1640 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/pyproject.toml
+drwxrwxr-x   0 petr      (1000) petr      (1000)        0 2023-06-08 13:13:21.687022 django-categories-api-0.0.2/requirements/
+-rw-rw-r--   0 petr      (1000) petr      (1000)       80 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/requirements/dev.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       18 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/requirements/prod.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      172 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/requirements/test.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)       25 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/requirements.txt
+-rw-rw-r--   0 petr      (1000) petr      (1000)      875 2023-06-08 13:13:21.687022 django-categories-api-0.0.2/setup.cfg
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1421 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/setup.py
+-rw-rw-r--   0 petr      (1000) petr      (1000)    23977 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/test.html
+-rw-rw-r--   0 petr      (1000) petr      (1000)     1093 2023-06-08 13:13:21.000000 django-categories-api-0.0.2/tox.ini
```

### Comparing `django-categories-api-0.0.1/.changelog-config.yaml` & `django-categories-api-0.0.2/.changelog-config.yaml`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/.github/workflows/publish-docs.yml` & `django-categories-api-0.0.2/.github/workflows/publish-docs.yml`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/.github/workflows/publish-package.yml` & `django-categories-api-0.0.2/.github/workflows/publish-package.yml`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/.github/workflows/publish-package.yml.orig` & `django-categories-api-0.0.2/.github/workflows/publish-package.yml.orig`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/.github/workflows/run-tests.yaml` & `django-categories-api-0.0.2/.github/workflows/run-tests.yaml`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/.gitignore` & `django-categories-api-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/.pre-commit-config.yaml` & `django-categories-api-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/CREDITS.md` & `django-categories-api-0.0.2/CREDITS.md`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/LICENSE.txt` & `django-categories-api-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/MANIFEST.in` & `django-categories-api-0.0.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/Makefile` & `django-categories-api-0.0.2/Makefile`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/categories_api/api/tests/test_api.py` & `django-categories-api-0.0.2/categories_api/api/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/categories_api/api/viewsets.py` & `django-categories-api-0.0.2/categories_api/api/viewsets.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/categories_api/tests/test_api.py` & `django-categories-api-0.0.2/categories_api/tests/test_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 
 from categories.models import Category
 
 User = get_user_model()
 
 
 class MeViewTests(APITestCase):
+    maxDiff = None
+
     def setUp(self):
         self.user = User.objects.create_superuser("test-user", "foo@bar.baz", "test-password")
         self.client.force_authenticate(user=self.user)
 
         category = Category.tree.create(name="Foo category", slug="foo_category", active=True, order=0, parent=None)
         baker.make(
             "SimpleText",
```

### Comparing `django-categories-api-0.0.1/categories_api/viewsets.py` & `django-categories-api-0.0.2/categories_api/viewsets.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from django.utils.decorators import method_decorator
 from django.views.decorators.cache import cache_page
+from django.conf import settings
 from rest_framework import mixins, permissions, serializers, viewsets
 
 from categories.models import Category
 
 
 class CategorySerializer(serializers.ModelSerializer):
     children = serializers.SerializerMethodField(method_name="_get_children")
@@ -27,21 +28,24 @@
         ]
 
     def _get_children(self, obj):
         children = obj.get_children()
         return CategorySerializer(children, many=True).data
 
 
+if hasattr(settings, "CATEGORIES_SETTINGS"):
+    countable_field_names = getattr(settings, "CATEGORIES_SETTINGS").get("COUNTABLE_FIELD_RELATED_NAMES", [])
+else:
+    countable_field_names = []
 countable_fields = [
     f
     for f in Category._meta.get_fields()
-    if f.is_relation and f.name not in ["parent", "children", "categoryrelation"]
+    if f.is_relation and f.name not in ["parent", "children", "categoryrelation"] and f.name in countable_field_names
 ]
 
-
 for field in countable_fields:
     CategorySerializer._declared_fields[f"{field.name}_count"] = serializers.SerializerMethodField()
 
     def field_count(self, obj, field=field):
         return getattr(obj, f"{field.name}_count", "-")
 
     setattr(CategorySerializer, f"get_{field.name}_count", field_count)
@@ -76,16 +80,16 @@
             field.related_model,
             field.remote_field.name,
             f"{field.name}_count_cumulative",
             extra_filters=extra_filters,
             cumulative=True,
         )
 
-    if exclude_blank:
-        queryset = queryset.filter(asset_count_cumulative__gt=0)
+        if exclude_blank:
+            queryset = queryset.filter(**{f"{field.name}_count_cumulative__gt": 0})
     return queryset
 
 
 class CategoryViewSet(mixins.ListModelMixin, viewsets.GenericViewSet):
     queryset = Category.tree.filter(active=True)
     serializer_class = CategorySerializer
     extra_count_filters = {}
```

### Comparing `django-categories-api-0.0.1/django_categories_api.egg-info/SOURCES.txt` & `django-categories-api-0.0.2/django_categories_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/Makefile` & `django-categories-api-0.0.2/doc_src/Makefile`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/_static/css/custom.css` & `django-categories-api-0.0.2/doc_src/_static/css/custom.css`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/_templates/autosummary/class.rst` & `django-categories-api-0.0.2/doc_src/_templates/autosummary/class.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/_templates/autosummary/module.rst` & `django-categories-api-0.0.2/doc_src/_templates/autosummary/module.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/conf.py` & `django-categories-api-0.0.2/doc_src/conf.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/getting_started.rst` & `django-categories-api-0.0.2/doc_src/getting_started.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/index.rst` & `django-categories-api-0.0.2/doc_src/index.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/index.rst.orig` & `django-categories-api-0.0.2/doc_src/index.rst.orig`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/make.bat` & `django-categories-api-0.0.2/doc_src/make.bat`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/reference/management_commands.rst` & `django-categories-api-0.0.2/doc_src/reference/management_commands.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/reference/models.rst` & `django-categories-api-0.0.2/doc_src/reference/models.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/reference/settings.rst` & `django-categories-api-0.0.2/doc_src/reference/settings.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/reference/templatetags.rst` & `django-categories-api-0.0.2/doc_src/reference/templatetags.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/adding_the_fields.rst` & `django-categories-api-0.0.2/doc_src/user_guide/adding_the_fields.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/admin_settings.rst` & `django-categories-api-0.0.2/doc_src/user_guide/admin_settings.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories3.py` & `django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories3.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories4.py` & `django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories4.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/code_examples/custom_categories7.py` & `django-categories-api-0.0.2/doc_src/user_guide/code_examples/custom_categories7.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/custom_categories.rst` & `django-categories-api-0.0.2/doc_src/user_guide/custom_categories.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/registering_models.rst` & `django-categories-api-0.0.2/doc_src/user_guide/registering_models.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/usage.rst` & `django-categories-api-0.0.2/doc_src/user_guide/usage.rst`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/doc_src/user_guide/usage_example_template.html` & `django-categories-api-0.0.2/doc_src/user_guide/usage_example_template.html`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/patch` & `django-categories-api-0.0.2/patch`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/pyproject.toml` & `django-categories-api-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/setup.py` & `django-categories-api-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/test.html` & `django-categories-api-0.0.2/test.html`

 * *Files identical despite different names*

### Comparing `django-categories-api-0.0.1/tox.ini` & `django-categories-api-0.0.2/tox.ini`

 * *Files identical despite different names*

