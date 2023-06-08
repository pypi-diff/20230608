# Comparing `tmp/django-phac_aspc-helpers-0.4.4.tar.gz` & `tmp/django-phac_aspc-helpers-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-phac_aspc-helpers-0.4.4.tar", last modified: Mon Mar  6 17:52:23 2023, max compression
+gzip compressed data, was "django-phac_aspc-helpers-0.5.0.tar", last modified: Thu Jun  8 13:56:10 2023, max compression
```

## Comparing `django-phac_aspc-helpers-0.4.4.tar` & `django-phac_aspc-helpers-0.5.0.tar`

### file list

```diff
@@ -1,69 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.858538 django-phac_aspc-helpers-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-03-06 17:52:23.858538 django-phac_aspc-helpers-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9927 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.846538 django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11046 2023-03-06 17:52:23.000000 django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-03-06 17:52:23.000000 django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-06 17:52:23.000000 django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-03-06 17:52:23.000000 django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-06 17:52:23.000000 django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.846538 django-phac_aspc-helpers-0.4.4/phac_aspc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.846538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.846538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.850538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/decorators/admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/decorators/test_admin_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.850538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      527 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.850538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/locale/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/locale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/locale/code.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/locale/language.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.850538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/ready/
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/ready/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/ready/ready.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/ready/test_ready.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.842538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.850538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/static/phac_aspc_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.842538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.842538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templates/phac_aspc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.842538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templates/phac_aspc/helpers/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.850538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.854538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/test_phac_aspc_localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/test_phac_aspc_wet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.854538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/urls/
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/urls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/urls/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.854538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/views/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/views/wet.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.854538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.854538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/decorators/localization_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 17:52:23.858538 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/localization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/security.py
--rw-r--r--   0 runner    (1001) docker     (123)     4462 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/wet.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-03-06 17:52:23.858538 django-phac_aspc-helpers-0.4.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-03-06 17:52:06.000000 django-phac_aspc-helpers-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15862 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16981 2023-06-08 13:56:10.000000 django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-08 13:56:10.000000 django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 13:56:10.000000 django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-08 13:56:10.000000 django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 13:56:10.000000 django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1682 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/decorators/admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/decorators/test_admin_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/auth/backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/auth/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.604959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/locale/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/locale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/locale/code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/locale/language.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/ready/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/ready/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/ready/ready.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/ready/test_ready.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.600959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/phac_aspc_helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.600959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    18943 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.600959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.600959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.600959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.608959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/test_phac_aspc_localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/test_phac_aspc_wet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/urls/
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/urls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/urls/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/urls/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/views/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/views/wet.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/decorators/localization_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/localization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2940 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5075 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/wet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-06-08 13:56:10.612959 django-phac_aspc-helpers-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-08 13:55:41.000000 django-phac_aspc-helpers-0.5.0/setup.py
```

### Comparing `django-phac_aspc-helpers-0.4.4/LICENSE` & `django-phac_aspc-helpers-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/PKG-INFO` & `django-phac_aspc-helpers-0.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac_aspc-helpers
-Version: 0.4.4
+Version: 0.5.0
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -95,63 +95,63 @@
 
 For more information, refer to the Jinja
 [documentation](https://jinja.palletsprojects.com/en/3.0.x/api/).
 
 ## Environment variables
 
 Several settings or behaviours implemented by this library can be controlled via
-environment variables.  This is done via the
+environment variables. This is done via the
 [django-environ](https://django-environ.readthedocs.io/en/latest/) library.
 (Refer to their documentation on how to format special data types like lists)
 If your project root has a `.env` file, those values will be used.
 
 If you want to use environment variables in your project's configuration, you
 can simply reference django-environ directly as it will automatically be
-installed.  For example:
+installed. For example:
 
 ```python
 import environ
 
 env = environ.Env(DEBUG=(bool, False))
 environ.Env.read_env()
 
 DEBUG = env('DEBUG')
 
 ```
 
 This library also provides a utility that automatically declares a module level
-global while checking the environment.  It is particularly useful when declaring
+global while checking the environment. It is particularly useful when declaring
 django settings.
 
 ```python
 from phac_aspc.django.settings.utils import global_from_env
 
 global_from_env(
     SESSION_COOKIE_AGE=(int, 1200),
 )
 ```
 
 The example above creates the module level global `SESSION_COOKIE_AGE` with a
 default value of 1200, unless there is an environment variable (or **.env** file
-entry) `PHAC_ASPC_SESSION_COOKIE_AGE`.  By default the declared variable name is
-prefixed with `PHAC_ASPC_`.  The prefix can be changed by providing a custom
+entry) `PHAC_ASPC_SESSION_COOKIE_AGE`. By default the declared variable name is
+prefixed with `PHAC_ASPC_`. The prefix can be changed by providing a custom
 prefix.
 
 ```python
 from phac_aspc.django.settings.utils import global_from_env
 
 global_from_env(
     prefix='MY_PREFIX_',
     SESSION_COOKIE_AGE=(int, 1200),
 )
 ```
 
 ### Environment variable list
 
-All variables are prefixed with `PHAC_ASPC_` to avoid name conflicts.  
+All variables are prefixed with `PHAC_ASPC_` to avoid name conflicts.
 
 | Variable                        | Type | Purpose                         |
 | ------------------------------- | ---- | ------------------------------- |
 | PHAC_ASPC_SESSION_COOKIE_AGE    | int  | Session expiry in seconds       |
 | PHAC_ASPC_SESSION_COOKIE_SECURE | bool | Use secure cookies (HTTPS only) |
 | PHAC_ASPC_LANGUAGE_CODE         | str  | Default language                |
 
@@ -203,14 +203,159 @@
 #### Bundled releases
 
 | Product                      | Version   |
 | ---------------------------- | --------- |
 | Web Experience Toolkit (WET) | v4.0.56.4 |
 | Canada.ca (GCWeb)            | v12.5.0   |
 
+### Sign in using Microsoft
+
+By adding a few environment variables, authentication using Microsoft's
+identity platform is automatically configured via the [Authlib](https://docs.authlib.org/en/latest/)
+library. Setting the `PHAC_ASPC_OAUTH_PROVIDER` variable to "microsoft" enables
+OAuth and adds the following new routes:
+
+- /en-ca/phac_aspc_helper_login (`phac_aspc_helper_login`)
+- /fr-ca/phac_aspc_helper_login (`phac_aspc_helper_login`)
+- /en-ca/phac_aspc_helper_authorize (`phac_aspc_authorize`)
+- /fr-ca/phac_aspc_helper_authorize (`phac_aspc_authorize`)
+
+The `phac_aspc_authorize` URLs above must be added to the list of redirect URLs
+in the Azure App Registration.
+
+The login flow is triggered by redirecting the browser to the named route
+`phac_aspc_helper_login`. The browser will automatically redirect the user to
+Microsoft's Sign in page and after successful authentication, return the user to
+the redirect route named `phac_aspc_authorize` along with a token containing
+information about the user.
+
+By default, the authentication backend will look for a user who's username is
+the user's uuid from Microsoft - if not found a new user is created.  To
+customize this behaviour, a custom authentication backend class can be specified
+via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
+
+After successful authentication, the user is redirected to `/`.  To customize
+this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
+name of the desired route.
+
+```python
+
+PHAC_ASPC_OAUTH_USE_BACKEND = "custom.authentication.backend"
+PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN = "home"
+
+# pylint: disable=wrong-import-position, unused-wildcard-import, wildcard-import
+from phac_aspc.django.settings import *
+```
+
+> **Note**
+> It is important that these settings be declared **before** the wildcard import.
+
+Here is an example custom backend that sets the user's name to the value
+provided by the identity service.
+
+```python
+from typing import Any
+
+from django.contrib.auth import get_user_model
+from django.contrib.auth.backends import BaseBackend
+from django.contrib.auth.base_user import AbstractBaseUser
+from django.http.request import HttpRequest
+
+
+class OAuthBackend(BaseBackend):
+    def _get(self, user_info, value, default=""):
+        return user_info[value] if value in user_info else default
+
+    def _should_update(self, user_info, value, current):
+        v = self._get(user_info, value)
+        return v != "" and v != current
+
+    def _sync_user(self, user, user_info, force=False):
+        if (
+            force
+            or self._should_update(user_info, "email", user.email)
+            or self._should_update(user_info, "name", user.first_name)
+        ):
+            user.email = self._get(user_info, "email", user.email)
+            user.first_name = self._get(user_info, "name", user.first_name)
+            user.save()
+
+    def authenticate(
+        self,
+        request: HttpRequest,
+        user_info: dict | None = None,
+        **kwargs: Any,
+    ) -> AbstractBaseUser | None:
+        if user_info is not None:
+            user_model = get_user_model()
+            try:
+                user = user_model.objects.get(username=user_info["oid"])
+                self._sync_user(user, user_info)
+            except user_model.DoesNotExist:
+                user = user_model(username=user_info["oid"])
+                self._sync_user(user, user_info, True)
+            return user
+        return None
+
+    def get_user(self, user_id):
+        user_model = get_user_model()
+        try:
+            return user_model.objects.get(pk=user_id)
+        except user_model.DoesNotExist:
+            return None
+
+```
+
+#### Environment Variables
+
+| Variable                          | Type | Purpose                                      |
+| --------------------------------- | ---- | -------------------------------------------- |
+| PHAC_ASPC_OAUTH_PROVIDER          | str  | Only "microsoft" is supported at the moment. |
+| PHAC_ASPC_OAUTH_APP_CLIENT_ID     | str  | Client ID (from the App Registration)        |
+| PHAC_ASPC_OAUTH_APP_CLIENT_SECRET | str  | Client Secret (from the App Registration)    |
+| PHAC_ASPC_OAUTH_MICROSOFT_TENANT  | str  | Microsoft Tenant ID                          |
+
+#### Template Tag
+
+A "Sign in with Microsoft" button is available as a template tag:
+
+```django
+{% load phac_aspc_auth %}
+{% phac_aspc_auth_signin_microsoft_button %}
+```
+
+#### Handling Errors
+
+If there are any errors during the authentication flow, they are displayed to
+the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
+template.  The template can be extended using standard django templating by
+creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
+project.
+
+#### Strings and locales
+
+Strings displayed to the user during the authentication flow are available in
+Canada's both official languages.  These strings can be customized by creating
+templates in the host project.  Here is a list of strings and templates used by
+the authentication flow:
+
+| Template                    | Context                                              |
+| --------------------------- | ---------------------------------------------------- |
+| error_title.html            | Error page title tag value                           |
+| error_page_description.html | Description of error page (meta tag)                 |
+| error_type_general.html     | Error header displayed for general exceptions        |
+| error_type_oauth.html       | Error header displayed for authentication errors     |
+| error_retry.html            | Text of retry link                                   |
+| microsoft_logo.html         | Alt text of sign the Microsoft logo in signin button |
+| signin_with_microsoft.html  | Text displayed in sign in button                     |
+
+> **Note**
+> String templates should be placed in the `templates/phac_aspc/helpers/strings`
+> directory.
+
 ### Security Controls
 
 #### AC-7 Automatic lockout of users after invalid login attempts
 
 [django-axes](https://django-axes.readthedocs.io) is used to monitor and lockout
 users who fail to successfully authenticate.
 
@@ -228,37 +373,39 @@
 ```python
 # settings.py
 
 # Examples of AXES_COOLOFF_TIME settings
 AXES_COOLOFF_TIME = None   # An administrator must unlock the account
 AXES_COOLOFF_TIME = 2      # Accounts will be locked out for 2 hours
 ```
+
 For more information regarding available configuration options, visit
 django-axes's [documentation](https://django-axes.readthedocs.io/en/latest/4_configuration.html)
 
 There are also a few command line management commands available, for example to
 remove all of the lockouts you can run:
 
 ```bash
 python -m manage axes_reset
 ```
+
 See the [usage](https://django-axes.readthedocs.io/en/latest/3_usage.html)
 documentation for more details.
 
 #### AC-11 Session Timeouts
 
 The default configuration makes the following configuration changes to django:
 
 - Sessions timeout in 20 minutes,
 - Sessions cookies are marked as secure,
 - Sessions cookies are discarded when the browser is closed,
 - Any requests to the server automatically extends the session.
 
 You can override any of these settings by adding them below the settings import
-line.  For example to use 30 minutes sessions:
+line. For example to use 30 minutes sessions:
 
 ```python
 #settings.py
 
 from phac_aspc.django.settings import *
 
 SESSION_COOKIE_AGE=1800
@@ -303,15 +450,15 @@
 > preferably in the base template for the entire site.
 >
 > For more information on session timeout, visit the
 > [documentation](https://wet-boew.github.io/wet-boew/docs/ref/session-timeout/session-timeout-en.html).
 
 ### Localization
 
-Django will be configured to support English (en-ca) and French (fr-ca).  This
+Django will be configured to support English (en-ca) and French (fr-ca). This
 can be changed in your projects settings using `LANGUAGES` and `LANGUAGE_CODE`.
 
 > For more information on Django's localization, see their
 > [documentation](https://docs.djangoproject.com/en/4.1/topics/i18n/).
 
 #### lang template tag
 
@@ -324,19 +471,18 @@
 
 Or in you're using Jinja
 
 ```jinja
 <html lang="{{ phac_aspc.localization.lang() }}">
 ```
 
-
 #### translate decorator
 
 Use this decorator on your models to add translations via
-`django-modeltranslation`.  The example below adds translations for the
+`django-modeltranslation`. The example below adds translations for the
 `title` field.
 
 ```python
 from django.db import models
 from phac_aspc.django.localization.decorators import translate
 
 @translate('title')
```

### Comparing `django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/PKG-INFO` & `django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-phac-aspc-helpers
-Version: 0.4.4
+Version: 0.5.0
 Summary: Set of helpers for Django used at PHAC-ASPC
 Home-page: https://github.com/PHACDataHub/django-phac_aspc-helpers
 Author: Luc Belliveau
 Author-email: luc.belliveau@phac-aspc.gc.ca
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -95,63 +95,63 @@
 
 For more information, refer to the Jinja
 [documentation](https://jinja.palletsprojects.com/en/3.0.x/api/).
 
 ## Environment variables
 
 Several settings or behaviours implemented by this library can be controlled via
-environment variables.  This is done via the
+environment variables. This is done via the
 [django-environ](https://django-environ.readthedocs.io/en/latest/) library.
 (Refer to their documentation on how to format special data types like lists)
 If your project root has a `.env` file, those values will be used.
 
 If you want to use environment variables in your project's configuration, you
 can simply reference django-environ directly as it will automatically be
-installed.  For example:
+installed. For example:
 
 ```python
 import environ
 
 env = environ.Env(DEBUG=(bool, False))
 environ.Env.read_env()
 
 DEBUG = env('DEBUG')
 
 ```
 
 This library also provides a utility that automatically declares a module level
-global while checking the environment.  It is particularly useful when declaring
+global while checking the environment. It is particularly useful when declaring
 django settings.
 
 ```python
 from phac_aspc.django.settings.utils import global_from_env
 
 global_from_env(
     SESSION_COOKIE_AGE=(int, 1200),
 )
 ```
 
 The example above creates the module level global `SESSION_COOKIE_AGE` with a
 default value of 1200, unless there is an environment variable (or **.env** file
-entry) `PHAC_ASPC_SESSION_COOKIE_AGE`.  By default the declared variable name is
-prefixed with `PHAC_ASPC_`.  The prefix can be changed by providing a custom
+entry) `PHAC_ASPC_SESSION_COOKIE_AGE`. By default the declared variable name is
+prefixed with `PHAC_ASPC_`. The prefix can be changed by providing a custom
 prefix.
 
 ```python
 from phac_aspc.django.settings.utils import global_from_env
 
 global_from_env(
     prefix='MY_PREFIX_',
     SESSION_COOKIE_AGE=(int, 1200),
 )
 ```
 
 ### Environment variable list
 
-All variables are prefixed with `PHAC_ASPC_` to avoid name conflicts.  
+All variables are prefixed with `PHAC_ASPC_` to avoid name conflicts.
 
 | Variable                        | Type | Purpose                         |
 | ------------------------------- | ---- | ------------------------------- |
 | PHAC_ASPC_SESSION_COOKIE_AGE    | int  | Session expiry in seconds       |
 | PHAC_ASPC_SESSION_COOKIE_SECURE | bool | Use secure cookies (HTTPS only) |
 | PHAC_ASPC_LANGUAGE_CODE         | str  | Default language                |
 
@@ -203,14 +203,159 @@
 #### Bundled releases
 
 | Product                      | Version   |
 | ---------------------------- | --------- |
 | Web Experience Toolkit (WET) | v4.0.56.4 |
 | Canada.ca (GCWeb)            | v12.5.0   |
 
+### Sign in using Microsoft
+
+By adding a few environment variables, authentication using Microsoft's
+identity platform is automatically configured via the [Authlib](https://docs.authlib.org/en/latest/)
+library. Setting the `PHAC_ASPC_OAUTH_PROVIDER` variable to "microsoft" enables
+OAuth and adds the following new routes:
+
+- /en-ca/phac_aspc_helper_login (`phac_aspc_helper_login`)
+- /fr-ca/phac_aspc_helper_login (`phac_aspc_helper_login`)
+- /en-ca/phac_aspc_helper_authorize (`phac_aspc_authorize`)
+- /fr-ca/phac_aspc_helper_authorize (`phac_aspc_authorize`)
+
+The `phac_aspc_authorize` URLs above must be added to the list of redirect URLs
+in the Azure App Registration.
+
+The login flow is triggered by redirecting the browser to the named route
+`phac_aspc_helper_login`. The browser will automatically redirect the user to
+Microsoft's Sign in page and after successful authentication, return the user to
+the redirect route named `phac_aspc_authorize` along with a token containing
+information about the user.
+
+By default, the authentication backend will look for a user who's username is
+the user's uuid from Microsoft - if not found a new user is created.  To
+customize this behaviour, a custom authentication backend class can be specified
+via `PHAC_ASPC_OAUTH_USE_BACKEND` in `settings.py`.
+
+After successful authentication, the user is redirected to `/`.  To customize
+this behaviour, set `PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN` in `settings.py` to the
+name of the desired route.
+
+```python
+
+PHAC_ASPC_OAUTH_USE_BACKEND = "custom.authentication.backend"
+PHAC_ASPC_OAUTH_REDIRECT_ON_LOGIN = "home"
+
+# pylint: disable=wrong-import-position, unused-wildcard-import, wildcard-import
+from phac_aspc.django.settings import *
+```
+
+> **Note**
+> It is important that these settings be declared **before** the wildcard import.
+
+Here is an example custom backend that sets the user's name to the value
+provided by the identity service.
+
+```python
+from typing import Any
+
+from django.contrib.auth import get_user_model
+from django.contrib.auth.backends import BaseBackend
+from django.contrib.auth.base_user import AbstractBaseUser
+from django.http.request import HttpRequest
+
+
+class OAuthBackend(BaseBackend):
+    def _get(self, user_info, value, default=""):
+        return user_info[value] if value in user_info else default
+
+    def _should_update(self, user_info, value, current):
+        v = self._get(user_info, value)
+        return v != "" and v != current
+
+    def _sync_user(self, user, user_info, force=False):
+        if (
+            force
+            or self._should_update(user_info, "email", user.email)
+            or self._should_update(user_info, "name", user.first_name)
+        ):
+            user.email = self._get(user_info, "email", user.email)
+            user.first_name = self._get(user_info, "name", user.first_name)
+            user.save()
+
+    def authenticate(
+        self,
+        request: HttpRequest,
+        user_info: dict | None = None,
+        **kwargs: Any,
+    ) -> AbstractBaseUser | None:
+        if user_info is not None:
+            user_model = get_user_model()
+            try:
+                user = user_model.objects.get(username=user_info["oid"])
+                self._sync_user(user, user_info)
+            except user_model.DoesNotExist:
+                user = user_model(username=user_info["oid"])
+                self._sync_user(user, user_info, True)
+            return user
+        return None
+
+    def get_user(self, user_id):
+        user_model = get_user_model()
+        try:
+            return user_model.objects.get(pk=user_id)
+        except user_model.DoesNotExist:
+            return None
+
+```
+
+#### Environment Variables
+
+| Variable                          | Type | Purpose                                      |
+| --------------------------------- | ---- | -------------------------------------------- |
+| PHAC_ASPC_OAUTH_PROVIDER          | str  | Only "microsoft" is supported at the moment. |
+| PHAC_ASPC_OAUTH_APP_CLIENT_ID     | str  | Client ID (from the App Registration)        |
+| PHAC_ASPC_OAUTH_APP_CLIENT_SECRET | str  | Client Secret (from the App Registration)    |
+| PHAC_ASPC_OAUTH_MICROSOFT_TENANT  | str  | Microsoft Tenant ID                          |
+
+#### Template Tag
+
+A "Sign in with Microsoft" button is available as a template tag:
+
+```django
+{% load phac_aspc_auth %}
+{% phac_aspc_auth_signin_microsoft_button %}
+```
+
+#### Handling Errors
+
+If there are any errors during the authentication flow, they are displayed to
+the user via the [error.html](phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html)
+template.  The template can be extended using standard django templating by
+creating a `templates/phac_aspc/helpers/auth/error.html` file in the host
+project.
+
+#### Strings and locales
+
+Strings displayed to the user during the authentication flow are available in
+Canada's both official languages.  These strings can be customized by creating
+templates in the host project.  Here is a list of strings and templates used by
+the authentication flow:
+
+| Template                    | Context                                              |
+| --------------------------- | ---------------------------------------------------- |
+| error_title.html            | Error page title tag value                           |
+| error_page_description.html | Description of error page (meta tag)                 |
+| error_type_general.html     | Error header displayed for general exceptions        |
+| error_type_oauth.html       | Error header displayed for authentication errors     |
+| error_retry.html            | Text of retry link                                   |
+| microsoft_logo.html         | Alt text of sign the Microsoft logo in signin button |
+| signin_with_microsoft.html  | Text displayed in sign in button                     |
+
+> **Note**
+> String templates should be placed in the `templates/phac_aspc/helpers/strings`
+> directory.
+
 ### Security Controls
 
 #### AC-7 Automatic lockout of users after invalid login attempts
 
 [django-axes](https://django-axes.readthedocs.io) is used to monitor and lockout
 users who fail to successfully authenticate.
 
@@ -228,37 +373,39 @@
 ```python
 # settings.py
 
 # Examples of AXES_COOLOFF_TIME settings
 AXES_COOLOFF_TIME = None   # An administrator must unlock the account
 AXES_COOLOFF_TIME = 2      # Accounts will be locked out for 2 hours
 ```
+
 For more information regarding available configuration options, visit
 django-axes's [documentation](https://django-axes.readthedocs.io/en/latest/4_configuration.html)
 
 There are also a few command line management commands available, for example to
 remove all of the lockouts you can run:
 
 ```bash
 python -m manage axes_reset
 ```
+
 See the [usage](https://django-axes.readthedocs.io/en/latest/3_usage.html)
 documentation for more details.
 
 #### AC-11 Session Timeouts
 
 The default configuration makes the following configuration changes to django:
 
 - Sessions timeout in 20 minutes,
 - Sessions cookies are marked as secure,
 - Sessions cookies are discarded when the browser is closed,
 - Any requests to the server automatically extends the session.
 
 You can override any of these settings by adding them below the settings import
-line.  For example to use 30 minutes sessions:
+line. For example to use 30 minutes sessions:
 
 ```python
 #settings.py
 
 from phac_aspc.django.settings import *
 
 SESSION_COOKIE_AGE=1800
@@ -303,15 +450,15 @@
 > preferably in the base template for the entire site.
 >
 > For more information on session timeout, visit the
 > [documentation](https://wet-boew.github.io/wet-boew/docs/ref/session-timeout/session-timeout-en.html).
 
 ### Localization
 
-Django will be configured to support English (en-ca) and French (fr-ca).  This
+Django will be configured to support English (en-ca) and French (fr-ca). This
 can be changed in your projects settings using `LANGUAGES` and `LANGUAGE_CODE`.
 
 > For more information on Django's localization, see their
 > [documentation](https://docs.djangoproject.com/en/4.1/topics/i18n/).
 
 #### lang template tag
 
@@ -324,19 +471,18 @@
 
 Or in you're using Jinja
 
 ```jinja
 <html lang="{{ phac_aspc.localization.lang() }}">
 ```
 
-
 #### translate decorator
 
 Use this decorator on your models to add translations via
-`django-modeltranslation`.  The example below adds translations for the
+`django-modeltranslation`. The example below adds translations for the
 `title` field.
 
 ```python
 from django.db import models
 from phac_aspc.django.localization.decorators import translate
 
 @translate('title')
```

### Comparing `django-phac_aspc-helpers-0.4.4/django_phac_aspc_helpers.egg-info/SOURCES.txt` & `django-phac_aspc-helpers-0.5.0/django_phac_aspc_helpers.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -16,26 +16,41 @@
 phac_aspc/django/admin/decorators/__init__.py
 phac_aspc/django/admin/decorators/admin_decorators.py
 phac_aspc/django/admin/decorators/test_admin_decorators.py
 phac_aspc/django/helpers/__init__.py
 phac_aspc/django/helpers/apps.py
 phac_aspc/django/helpers/test_phac_aspc_localization.py
 phac_aspc/django/helpers/test_phac_aspc_wet.py
+phac_aspc/django/helpers/auth/__init__.py
+phac_aspc/django/helpers/auth/backend.py
+phac_aspc/django/helpers/auth/views.py
 phac_aspc/django/helpers/locale/__init__.py
 phac_aspc/django/helpers/locale/code.py
 phac_aspc/django/helpers/locale/language.py
 phac_aspc/django/helpers/ready/__init__.py
 phac_aspc/django/helpers/ready/ready.py
 phac_aspc/django/helpers/ready/test_ready.py
 phac_aspc/django/helpers/static/phac_aspc_helpers/base.css
+phac_aspc/django/helpers/static/phac_aspc_helpers/auth/buttons/ms-logo.svg
+phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/error.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/auth/buttons/microsoft.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_page_description.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_retry.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_title.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_general.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/error_type_oauth.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/microsoft_logo.html
+phac_aspc/django/helpers/templates/phac_aspc/helpers/strings/signin_with_microsoft.html
 phac_aspc/django/helpers/templates/phac_aspc/helpers/wet/session_timeout.html
 phac_aspc/django/helpers/templatetags/__init__.py
+phac_aspc/django/helpers/templatetags/phac_aspc_auth.py
 phac_aspc/django/helpers/templatetags/phac_aspc_localization.py
 phac_aspc/django/helpers/templatetags/phac_aspc_wet.py
 phac_aspc/django/helpers/urls/__init__.py
+phac_aspc/django/helpers/urls/auth.py
 phac_aspc/django/helpers/urls/wet.py
 phac_aspc/django/helpers/views/__init__.py
 phac_aspc/django/helpers/views/wet.py
 phac_aspc/django/localization/__init__.py
 phac_aspc/django/localization/hooks.py
 phac_aspc/django/localization/decorators/__init__.py
 phac_aspc/django/localization/decorators/localization_decorators.py
```

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/decorators/admin_decorators.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/decorators/admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/admin/decorators/test_admin_decorators.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/admin/decorators/test_admin_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/apps.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/apps.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/locale/language.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/locale/language.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/ready/__init__.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/ready/__init__.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/ready/test_ready.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/ready/test_ready.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/static/phac_aspc_helpers/base.css`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/templatetags/phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/test_phac_aspc_wet.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/test_phac_aspc_wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/helpers/views/wet.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/helpers/views/wet.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/localization/decorators/localization_decorators.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/localization/decorators/localization_decorators.py`

 * *Files identical despite different names*

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/test_utils.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,19 +104,39 @@
 
 
 def test_configure_middleware():
     """Test that the configure_middleware utility adds the correct middleware to
     the list"""
     num = len(registry.get_checks())
     test = configure_middleware([])
-    assert test == ["axes.middleware.AxesMiddleware"]
+    assert test == [
+        "axes.middleware.AxesMiddleware",
+        "django.middleware.locale.LocaleMiddleware",
+    ]
     assert len(registry.get_checks()) == num
 
     num = len(registry.get_checks())
     test = configure_middleware(["a", "b"])
-    assert test == ["axes.middleware.AxesMiddleware", "a", "b"]
+    assert test == [
+        "axes.middleware.AxesMiddleware",
+        "django.middleware.locale.LocaleMiddleware",
+        "a",
+        "b",
+    ]
     assert len(registry.get_checks()) == num
 
     num = len(registry.get_checks())
-    test = configure_middleware(["a", "axes.middleware.AxesMiddleware", "b"])
-    assert test == ["a", "axes.middleware.AxesMiddleware", "b"]
-    assert len(registry.get_checks()) == num + 1
+    test = configure_middleware(
+        [
+            "a",
+            "axes.middleware.AxesMiddleware",
+            "django.middleware.locale.LocaleMiddleware",
+            "b",
+        ]
+    )
+    assert test == [
+        "a",
+        "axes.middleware.AxesMiddleware",
+        "django.middleware.locale.LocaleMiddleware",
+        "b",
+    ]
+    assert len(registry.get_checks()) == num + 2
```

### Comparing `django-phac_aspc-helpers-0.4.4/phac_aspc/django/settings/utils.py` & `django-phac_aspc-helpers-0.5.0/phac_aspc/django/settings/utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -52,57 +52,99 @@
 def configure_authentication_backends(backend_list):
     """Return the authentication backend list includes those required by this
     library.
 
     By default importing the settings will automatically configure the backend,
     however if you want to customize the authentication backend used by your
     project, you can use this method to ensure proper configuration."""
+    oauth_backend = (
+        [getattr(settings, "PHAC_ASPC_OAUTH_USE_BACKEND", "")]
+        if getattr(settings, "PHAC_ASPC_OAUTH_USE_BACKEND", "")
+        else []
+    )
 
     prefix_backends = warn_and_remove(
-        ["axes.backends.AxesStandaloneBackend"], backend_list
+        ["axes.backends.AxesStandaloneBackend"] + oauth_backend, backend_list
     )
     return prefix_backends + backend_list
 
 
 def configure_middleware(middleware_list):
     """Return the list of middleware configured for this library"""
-    suffix = warn_and_remove(["axes.middleware.AxesMiddleware"], middleware_list)
-    return suffix + middleware_list
+    prefix = warn_and_remove(
+        ["axes.middleware.AxesMiddleware", "django.middleware.locale.LocaleMiddleware"],
+        middleware_list,
+    )
+    return prefix + middleware_list
 
 
-def global_from_env(prefix="PHAC_ASPC_", **conf):
-    """Create named global variables based on the provided environment variable
-    scheme.  Variables defined in the scheme will be inserted into the calling
-    module's globals and prefixed with `PHAC_ASPC_` when fetching the
-    environment variable.
+def get_env_value(env, key, prefix="PHAC_ASPC_"):
+    """Return prefixed value from environment"""
+    return env(f"{prefix}{key}")
+
+
+def get_env(prefix="PHAC_ASPC_", **conf):
+    """Return django-environ configured with the provided values and
+    using the prefix.
 
     prefix can be used to change the environment variable prefix that is added
     to the beginning on the variables defined in conf.  By default this value is
     `PHAC_ASPC_`.
 
     conf is a dictionary used to generate the scheme for django-environ.
 
     See https://django-environ.readthedocs.io/en/latest/api.html#environ.Env for
     additional information on the scheme.
-
     """
 
-    mod = inspect.getmodule(inspect.stack()[1][0])
+    def _find_env_file(path):
+        # look for .env file in provided path
+        filename = os.path.join(path, ".env")
+        if os.path.isfile(filename):
+            return filename
+
+        # search the parent
+        parent = os.path.dirname(path)
+        if parent and os.path.normcase(parent) != os.path.normcase(
+            os.path.abspath(os.sep)
+        ):
+            return _find_env_file(parent)
+
+        # Not found
+        return ""
 
     scheme = {}
     for name, values in conf.items():
         scheme[f"{prefix}{name}"] = values
 
     env = environ.Env(**scheme)
-    environ.Env.read_env(
-        os.path.join(os.path.abspath(os.path.dirname(__name__)), ".env")
-    )
+    environ.Env.read_env(_find_env_file(os.path.abspath(os.path.dirname(__name__))))
+    return env
+
+
+def global_from_env(prefix="PHAC_ASPC_", **conf):
+    """Create named global variables based on the provided environment variable
+    scheme.  Variables defined in the scheme will be inserted into the calling
+    module's globals and prefixed with `PHAC_ASPC_` when fetching the
+    environment variable.
+
+    prefix can be used to change the environment variable prefix that is added
+    to the beginning on the variables defined in conf.  By default this value is
+    `PHAC_ASPC_`.
+
+    conf is a dictionary used to generate the scheme for django-environ.
+
+
+    """
+
+    mod = inspect.getmodule(inspect.stack()[1][0])
+    env = get_env(prefix, **conf)
 
     for name in conf:
-        setattr(mod, name, env(f"{prefix}{name}"))
+        setattr(mod, name, get_env_value(env, name))
 
 
 def configure_settings_for_tests():
     """
     Modify django settings so they are suitable to run unit tests.
       - Disables the Axes authentcation backend, to allow the test client
         to function.  You could instead modify the request as described here:
```

### Comparing `django-phac_aspc-helpers-0.4.4/setup.cfg` & `django-phac_aspc-helpers-0.5.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-phac_aspc-helpers
-version = 0.4.4
+version = 0.5.0
 description = Set of helpers for Django used at PHAC-ASPC
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/PHACDataHub/django-phac_aspc-helpers
 author = Luc Belliveau
 author_email = luc.belliveau@phac-aspc.gc.ca
 license = MIT
@@ -27,14 +27,15 @@
 	Topic :: Software Development :: Localization
 
 [options]
 include_package_data = true
 packages = find:
 python_requires = >=3.8
 install_requires = 
+	Authlib >= 1.2.0
 	Django >= 4.1
 	django-modeltranslation == 0.18.4
 	django-environ == 0.9.0
 	django-axes == 5.40.1
 
 [egg_info]
 tag_build =
```

