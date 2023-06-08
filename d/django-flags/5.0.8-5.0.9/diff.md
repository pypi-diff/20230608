# Comparing `tmp/django-flags-5.0.8.tar.gz` & `tmp/django-flags-5.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-flags-5.0.8.tar", last modified: Wed Jan 26 15:44:56 2022, max compression
+gzip compressed data, was "dist/django-flags-5.0.9.tar", last modified: Mon Mar 14 17:47:10 2022, max compression
```

## Comparing `django-flags-5.0.8.tar` & `django-flags-5.0.9.tar`

### file list

```diff
@@ -1,85 +1,85 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-01-26 15:44:46.000000 django-flags-5.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-01-26 15:44:46.000000 django-flags-5.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-01-26 15:44:56.000000 django-flags-5.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-01-26 15:44:46.000000 django-flags-5.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/django_flags.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-01-26 15:44:55.000000 django-flags-5.0.8/django_flags.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-01-26 15:44:56.000000 django-flags-5.0.8/django_flags.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-26 15:44:55.000000 django-flags-5.0.8/django_flags.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-01-26 15:44:55.000000 django-flags-5.0.8/django_flags.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-01-26 15:44:55.000000 django-flags-5.0.8/django_flags.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/docs/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/docs/theme-overrides/
--rw-r--r--   0 runner    (1001) docker     (121)      298 2022-01-26 15:44:46.000000 django-flags-5.0.8/docs/theme-overrides/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/
--rw-r--r--   0 runner    (1001) docker     (121)      100 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      223 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/checks.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/conditions/
--rw-r--r--   0 runner    (1001) docker     (121)      540 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/conditions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3442 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/conditions/conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/conditions/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/conditions/validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/forms.py
--rw-r--r--   0 runner    (1001) docker     (121)      504 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/jinja2tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/management/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/management/commands/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/management/commands/disable_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      683 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/management/commands/enable_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      390 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/migrations/0012_replace_migrations_for_wagtail_independence.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/migrations/0013_add_required_field.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      716 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/panels.py
--rw-r--r--   0 runner    (1001) docker     (121)     6058 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/state.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/templates/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/templates/flags/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/templates/flags/panels/
--rw-r--r--   0 runner    (1001) docker     (121)      576 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/templates/flags/panels/flag_checks.html
--rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/templates/flags/panels/flags.html
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/templatetags/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      870 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/templatetags/feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/templatetags/flags_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2191 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     8989 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_conditions_conditions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_conditions_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_conditions_validators.py
--rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_forms.py
--rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_jinja2tags.py
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_management_commands_disable_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_management_commands_enable_flag.py
--rw-r--r--   0 runner    (1001) docker     (121)      556 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (121)      610 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_panels.py
--rw-r--r--   0 runner    (1001) docker     (121)     7717 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_sources.py
--rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_state.py
--rw-r--r--   0 runner    (1001) docker     (121)     4565 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_templatetags_feature_flags.py
--rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_templatetags_flags_debug.py
--rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/tests/testapp/
--rw-r--r--   0 runner    (1001) docker     (121)       62 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/testapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      155 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/testapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:56.000000 django-flags-5.0.8/flags/tests/testapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)      775 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/testapp/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/testapp/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/tests/testapp/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     4977 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-01-26 15:44:46.000000 django-flags-5.0.8/flags/views.py
--rw-r--r--   0 runner    (1001) docker     (121)      287 2022-01-26 15:44:46.000000 django-flags-5.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-26 15:44:56.000000 django-flags-5.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-01-26 15:44:46.000000 django-flags-5.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7048 2022-03-14 17:46:58.000000 django-flags-5.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-03-14 17:46:58.000000 django-flags-5.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-03-14 17:47:10.000000 django-flags-5.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1952 2022-03-14 17:46:58.000000 django-flags-5.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/django_flags.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     3149 2022-03-14 17:47:10.000000 django-flags-5.0.9/django_flags.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2022-03-14 17:47:10.000000 django-flags-5.0.9/django_flags.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-14 17:47:10.000000 django-flags-5.0.9/django_flags.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-03-14 17:47:10.000000 django-flags-5.0.9/django_flags.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-03-14 17:47:10.000000 django-flags-5.0.9/django_flags.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/docs/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/docs/theme-overrides/
+-rw-r--r--   0 runner    (1001) docker     (121)      298 2022-03-14 17:46:58.000000 django-flags-5.0.9/docs/theme-overrides/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/
+-rw-r--r--   0 runner    (1001) docker     (121)      100 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      223 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/checks.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/conditions/
+-rw-r--r--   0 runner    (1001) docker     (121)      540 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/conditions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3498 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/conditions/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/conditions/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1470 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/conditions/validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1515 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1455 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)      630 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/jinja2tags.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/management/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      690 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/management/commands/disable_flag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      683 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/management/commands/enable_flag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      390 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1391 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/migrations/0012_replace_migrations_for_wagtail_independence.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/migrations/0013_add_required_field.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      716 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1752 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/panels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6058 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2739 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/state.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/templates/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/templates/flags/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/templates/flags/panels/
+-rw-r--r--   0 runner    (1001) docker     (121)      576 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/templates/flags/panels/flag_checks.html
+-rw-r--r--   0 runner    (1001) docker     (121)     1042 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/templates/flags/panels/flags.html
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      870 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/templatetags/feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3471 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/templatetags/flags_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2206 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      673 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1115 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7760 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_conditions_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1544 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_conditions_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3422 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_conditions_validators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3987 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_forms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1351 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_jinja2tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_management_commands_disable_flag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_management_commands_enable_flag.py
+-rw-r--r--   0 runner    (1001) docker     (121)      556 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (121)      610 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1814 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_panels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7717 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_sources.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3131 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4565 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_templatetags_feature_flags.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5956 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_templatetags_flags_debug.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9973 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3235 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/tests/testapp/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/testapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      155 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/testapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-14 17:47:10.000000 django-flags-5.0.9/flags/tests/testapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)      775 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/testapp/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/testapp/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/tests/testapp/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4977 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1532 2022-03-14 17:46:58.000000 django-flags-5.0.9/flags/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      287 2022-03-14 17:46:58.000000 django-flags-5.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-14 17:47:10.000000 django-flags-5.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1244 2022-03-14 17:46:58.000000 django-flags-5.0.9/setup.py
```

### Comparing `django-flags-5.0.8/LICENSE` & `django-flags-5.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/PKG-INFO` & `django-flags-5.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flags
-Version: 5.0.8
+Version: 5.0.9
 Summary: Feature flags for Django projects
 Home-page: https://github.com/cfpb/django-flags
 Author: CFPB
 Author-email: tech@cfpb.gov
 License: CC0
 Description: # Django-Flags
```

### Comparing `django-flags-5.0.8/README.md` & `django-flags-5.0.9/README.md`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/django_flags.egg-info/PKG-INFO` & `django-flags-5.0.9/django_flags.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-flags
-Version: 5.0.8
+Version: 5.0.9
 Summary: Feature flags for Django projects
 Home-page: https://github.com/cfpb/django-flags
 Author: CFPB
 Author-email: tech@cfpb.gov
 License: CC0
 Description: # Django-Flags
```

### Comparing `django-flags-5.0.8/django_flags.egg-info/SOURCES.txt` & `django-flags-5.0.9/django_flags.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/checks.py` & `django-flags-5.0.9/flags/checks.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/conditions/__init__.py` & `django-flags-5.0.9/flags/conditions/__init__.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/conditions/conditions.py` & `django-flags-5.0.9/flags/conditions/conditions.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
 @register("user", validator=validate_user)
 def user_condition(username, request=None, **kwargs):
     """Does request.user match the expected username?"""
     if request is None:
         raise RequiredForCondition("request is required for condition 'user'")
 
+    if request.user.is_anonymous:
+        return False
+
     return getattr(request.user, get_user_model().USERNAME_FIELD) == username
 
 
 @register("anonymous", validator=validate_boolean)
 def anonymous_condition(boolean_value, request=None, **kwargs):
     """request.user an anonymous user, true or false based on boolean_value"""
     if request is None:
```

### Comparing `django-flags-5.0.8/flags/conditions/registry.py` & `django-flags-5.0.9/flags/conditions/registry.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/conditions/validators.py` & `django-flags-5.0.9/flags/conditions/validators.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/decorators.py` & `django-flags-5.0.9/flags/decorators.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/forms.py` & `django-flags-5.0.9/flags/forms.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/management/commands/disable_flag.py` & `django-flags-5.0.9/flags/management/commands/disable_flag.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/management/commands/enable_flag.py` & `django-flags-5.0.9/flags/management/commands/enable_flag.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/migrations/0012_replace_migrations_for_wagtail_independence.py` & `django-flags-5.0.9/flags/migrations/0012_replace_migrations_for_wagtail_independence.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/models.py` & `django-flags-5.0.9/flags/models.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/panels.py` & `django-flags-5.0.9/flags/panels.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/sources.py` & `django-flags-5.0.9/flags/sources.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/state.py` & `django-flags-5.0.9/flags/state.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/templates/flags/panels/flag_checks.html` & `django-flags-5.0.9/flags/templates/flags/panels/flag_checks.html`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/templates/flags/panels/flags.html` & `django-flags-5.0.9/flags/templates/flags/panels/flags.html`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/templatetags/feature_flags.py` & `django-flags-5.0.9/flags/templatetags/feature_flags.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/templatetags/flags_debug.py` & `django-flags-5.0.9/flags/templatetags/flags_debug.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/settings.py` & `django-flags-5.0.9/flags/tests/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,14 +49,16 @@
             ]
         },
     }
 ]
 
 STATIC_URL = "/static/"
 
+USE_TZ = True
+
 FLAGS = {
     "FLAG_ENABLED": [("boolean", True)],
     "FLAG_ENABLED_WITH_KWARG": [("flag_enabled_with_kwarg", (2 + 2))],
     "FLAG_DISABLED": [("boolean", False)],
     "DB_FLAG": [],
 }
```

### Comparing `django-flags-5.0.8/flags/tests/test_admin.py` & `django-flags-5.0.9/flags/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_checks.py` & `django-flags-5.0.9/flags/tests/test_checks.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_conditions_conditions.py` & `django-flags-5.0.9/flags/tests/test_conditions_conditions.py`

 * *Files 18% similar despite different names*

```diff
@@ -54,25 +54,34 @@
 
     def test_user_valid(self):
         self.assertTrue(user_condition("testuser", request=self.request))
 
     def test_user_invalid(self):
         self.assertFalse(user_condition("nottestuser", request=self.request))
 
+    def test_user_anonymous(self):
+        self.request.user = AnonymousUser()
+        self.assertFalse(user_condition("somebody", request=self.request))
+
     def test_request_required(self):
         with self.assertRaises(RequiredForCondition):
             user_condition("testuser")
 
     @override_settings(AUTH_USER_MODEL="testapp.MyUserModel")
     def test_custom_user_model_valid(self):
         user = get_user_model()(identifier="customuser")
         user.save()
         self.request.user = user
         self.assertTrue(user_condition("customuser", request=self.request))
 
+    @override_settings(AUTH_USER_MODEL="testapp.MyUserModel")
+    def test_custom_user_model_valid_anonymous(self):
+        self.request.user = AnonymousUser()
+        self.assertFalse(user_condition("somebody", request=self.request))
+
 
 class AnonymousConditionTestCase(TestCase):
     def setUp(self):
         self.request = HttpRequest()
 
     def test_anonymous_valid(self):
         self.request.user = AnonymousUser()
@@ -155,89 +164,53 @@
 
 class AfterDateConditionTestCase(TestCase):
     def setUp(self):
         # Set up some datetimes relative to now for testing
         delta = timedelta(days=1)
 
         self.past_datetime_tz = timezone.now() - delta
-        self.past_datetime_notz = self.past_datetime_tz.replace(tzinfo=None)
         self.past_datetime_tz_str = self.past_datetime_tz.isoformat()
-        self.past_datetime_notz_str = self.past_datetime_notz.isoformat()
 
         self.future_datetime_tz = timezone.now() + delta
-        self.future_datetime_notz = self.future_datetime_tz.replace(
-            tzinfo=None
-        )
         self.future_datetime_tz_str = self.future_datetime_tz.isoformat()
-        self.future_datetime_notz_str = self.future_datetime_notz.isoformat()
 
     def test_date_timeone_true(self):
         self.assertTrue(after_date_condition(self.past_datetime_tz))
 
-    def test_date_no_timeone_true(self):
-        self.assertTrue(after_date_condition(self.past_datetime_notz))
-
     def test_date_str_timeone_true(self):
         self.assertTrue(after_date_condition(self.past_datetime_tz_str))
 
-    def test_date_str_no_timeone_true(self):
-        self.assertTrue(after_date_condition(self.past_datetime_notz_str))
-
     def test_date_timeone_false(self):
         self.assertFalse(after_date_condition(self.future_datetime_tz))
 
-    def test_date_no_timeone_false(self):
-        self.assertFalse(after_date_condition(self.future_datetime_notz))
-
     def test_date_str_timeone_false(self):
         self.assertFalse(after_date_condition(self.future_datetime_tz_str))
 
-    def test_date_str_no_timeone_false(self):
-        self.assertFalse(after_date_condition(self.future_datetime_notz_str))
-
     def test_not_valid_date_str(self):
         self.assertFalse(after_date_condition("I am not a valid date"))
 
 
 class BeforeDateConditionTestCase(TestCase):
     def setUp(self):
         # Set up some datetimes relative to now for testing
         delta = timedelta(days=1)
 
         self.past_datetime_tz = timezone.now() - delta
-        self.past_datetime_notz = self.past_datetime_tz.replace(tzinfo=None)
         self.past_datetime_tz_str = self.past_datetime_tz.isoformat()
-        self.past_datetime_notz_str = self.past_datetime_notz.isoformat()
 
         self.future_datetime_tz = timezone.now() + delta
-        self.future_datetime_notz = self.future_datetime_tz.replace(
-            tzinfo=None
-        )
         self.future_datetime_tz_str = self.future_datetime_tz.isoformat()
-        self.future_datetime_notz_str = self.future_datetime_notz.isoformat()
 
     def test_date_timeone_true(self):
         self.assertTrue(before_date_condition(self.future_datetime_tz))
 
-    def test_date_no_timeone_true(self):
-        self.assertTrue(before_date_condition(self.future_datetime_notz))
-
     def test_date_str_timeone_true(self):
         self.assertTrue(before_date_condition(self.future_datetime_tz_str))
 
-    def test_date_str_no_timeone_true(self):
-        self.assertTrue(before_date_condition(self.future_datetime_notz_str))
-
     def test_date_timeone_false(self):
         self.assertFalse(before_date_condition(self.past_datetime_tz))
 
-    def test_date_no_timeone_false(self):
-        self.assertFalse(before_date_condition(self.past_datetime_notz))
-
     def test_date_str_timeone_false(self):
         self.assertFalse(before_date_condition(self.past_datetime_tz_str))
 
-    def test_date_str_no_timeone_false(self):
-        self.assertFalse(before_date_condition(self.past_datetime_notz_str))
-
     def test_not_valid_date_str(self):
         self.assertFalse(before_date_condition("I am not a valid date"))
```

### Comparing `django-flags-5.0.8/flags/tests/test_conditions_registry.py` & `django-flags-5.0.9/flags/tests/test_conditions_registry.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_conditions_validators.py` & `django-flags-5.0.9/flags/tests/test_conditions_validators.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_decorators.py` & `django-flags-5.0.9/flags/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_forms.py` & `django-flags-5.0.9/flags/tests/test_forms.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_jinja2tags.py` & `django-flags-5.0.9/flags/tests/test_jinja2tags.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_management_commands_disable_flag.py` & `django-flags-5.0.9/flags/tests/test_management_commands_disable_flag.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_management_commands_enable_flag.py` & `django-flags-5.0.9/flags/tests/test_management_commands_enable_flag.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_middleware.py` & `django-flags-5.0.9/flags/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_models.py` & `django-flags-5.0.9/flags/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_panels.py` & `django-flags-5.0.9/flags/tests/test_panels.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_sources.py` & `django-flags-5.0.9/flags/tests/test_sources.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_state.py` & `django-flags-5.0.9/flags/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_templatetags_feature_flags.py` & `django-flags-5.0.9/flags/tests/test_templatetags_feature_flags.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_templatetags_flags_debug.py` & `django-flags-5.0.9/flags/tests/test_templatetags_flags_debug.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_urls.py` & `django-flags-5.0.9/flags/tests/test_urls.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/test_views.py` & `django-flags-5.0.9/flags/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/tests/testapp/migrations/0001_initial.py` & `django-flags-5.0.9/flags/tests/testapp/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/urls.py` & `django-flags-5.0.9/flags/urls.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/flags/views.py` & `django-flags-5.0.9/flags/views.py`

 * *Files identical despite different names*

### Comparing `django-flags-5.0.8/setup.py` & `django-flags-5.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     url="https://github.com/cfpb/django-flags",
     author="CFPB",
     author_email="tech@cfpb.gov",
     description="Feature flags for Django projects",
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     license="CC0",
-    version="5.0.8",
+    version="5.0.9",
     include_package_data=True,
     packages=find_packages(),
     python_requires=">=3.6",
     install_requires=install_requires,
     extras_require={"testing": testing_extras, "docs": docs_extras},
     classifiers=[
         "Framework :: Django",
```

