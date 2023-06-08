# Comparing `tmp/simple_openid_connect-0.2.5.tar.gz` & `tmp/simple_openid_connect-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_openid_connect-0.2.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "simple_openid_connect-0.3.0.tar", last modified: Thu Jun  8 15:33:25 2023, max compression
```

## Comparing `simple_openid_connect-0.2.5.tar` & `simple_openid_connect-0.3.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
--rw-r--r--   0        0        0       50 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.gitattributes
--rw-r--r--   0        0        0     1584 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.github/workflows/checks.yml
--rw-r--r--   0        0        0      136 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.gitignore
--rw-r--r--   0        0        0      795 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0      177 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/.readthedocs.yaml
--rw-r--r--   0        0        0      298 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/DEVELOPMENT.md
--rw-r--r--   0        0        0     1116 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/LICENSE
--rw-r--r--   0        0        0     4447 2023-05-11 13:50:35.101827 simple_openid_connect-0.2.5/README.md
--rw-r--r--   0        0        0      679 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/Makefile
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/_static/.gitkeep
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/_templates/.gitkeep
--rw-r--r--   0        0        0      320 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/api.rst
--rw-r--r--   0        0        0     1790 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/conf.py
--rw-r--r--   0        0        0     5754 2023-05-25 12:12:58.573729 simple_openid_connect-0.2.5/docs/django-integration.rst
--rw-r--r--   0        0        0     2615 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/drf-integration.rst
--rw-r--r--   0        0        0      708 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/index.rst
--rw-r--r--   0        0        0     1247 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/installation.rst
--rw-r--r--   0        0        0     4868 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/docs/usage.rst
--rw-r--r--   0        0        0     2391 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/pyproject.toml
--rw-r--r--   0        0        0      211 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/requirements.dev.txt
--rw-r--r--   0        0        0      127 2023-06-01 11:14:30.712722 simple_openid_connect-0.2.5/src/simple_openid_connect/__init__.py
--rw-r--r--   0        0        0     4204 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/src/simple_openid_connect/base_data.py
--rw-r--r--   0        0        0    10682 2023-05-25 12:13:07.757788 simple_openid_connect-0.2.5/src/simple_openid_connect/client.py
--rw-r--r--   0        0        0     3443 2023-05-11 13:50:35.105827 simple_openid_connect-0.2.5/src/simple_openid_connect/client_authentication.py
--rw-r--r--   0        0        0    57273 2023-05-25 12:16:39.699145 simple_openid_connect-0.2.5/src/simple_openid_connect/data.py
--rw-r--r--   0        0        0     1819 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/discovery.py
--rw-r--r--   0        0        0     1174 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/exceptions.py
--rw-r--r--   0        0        0      343 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/__init__.py
--rw-r--r--   0        0        0     5631 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
--rw-r--r--   0        0        0     5823 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/client.py
--rw-r--r--   0        0        0     2208 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/__init__.py
--rw-r--r--   0        0        0     1583 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/client.py
--rw-r--r--   0        0        0       53 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/__init__.py
--rw-r--r--   0        0        0       61 2023-05-11 13:50:35.109827 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/__init__.py
--rw-r--r--   0        0        0     5467 2023-05-12 09:43:09.751399 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/apps.py
--rw-r--r--   0        0        0     4555 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/decorators.py
--rw-r--r--   0        0        0     2630 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/migrations/__init__.py
--rw-r--r--   0        0        0     5728 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/models.py
--rw-r--r--   0        0        0      381 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
--rw-r--r--   0        0        0      729 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/urls.py
--rw-r--r--   0        0        0     2338 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/user_mapping.py
--rw-r--r--   0        0        0     4415 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/views.py
--rw-r--r--   0        0        0      306 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/__init__.py
--rw-r--r--   0        0        0     4648 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/authentication.py
--rw-r--r--   0        0        0      957 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
--rw-r--r--   0        0        0     2531 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/permissions.py
--rw-r--r--   0        0        0      472 2023-05-12 09:43:09.751399 simple_openid_connect-0.2.5/src/simple_openid_connect/jwk.py
--rw-r--r--   0        0        0      621 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/rp_initiated_logout.py
--rw-r--r--   0        0        0     1509 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/token_introspection.py
--rw-r--r--   0        0        0     1566 2023-05-11 13:50:35.113828 simple_openid_connect-0.2.5/src/simple_openid_connect/token_refresh.py
--rw-r--r--   0        0        0     1393 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/src/simple_openid_connect/userinfo.py
--rw-r--r--   0        0        0      781 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/src/simple_openid_connect/utils.py
--rw-r--r--   0        0        0    16938 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/conftest.py
--rw-r--r--   0        0        0        0 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/__init__.py
--rw-r--r--   0        0        0     2785 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/settings.py
--rw-r--r--   0        0        0     2586 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/conftest.py
--rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
--rw-r--r--   0        0        0      633 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
--rw-r--r--   0        0        0     5247 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_login.py
--rw-r--r--   0        0        0      687 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_logout.py
--rw-r--r--   0        0        0     1248 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/urls.py
--rw-r--r--   0        0        0      639 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/views.py
--rw-r--r--   0        0        0      415 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/wsgi.py
--rwxr-xr-x   0        0        0      675 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/django_test_project/manage.py
--rw-r--r--   0        0        0     1746 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/interactive_tests/conftest.py
--rw-r--r--   0        0        0     2001 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/interactive_tests/test_google.py
--rw-r--r--   0        0        0     1668 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_authorization_code_flow.py
--rw-r--r--   0        0        0     3115 2023-06-01 11:14:39.765067 simple_openid_connect-0.2.5/tests/test_client.py
--rw-r--r--   0        0        0      934 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_client_auth.py
--rw-r--r--   0        0        0     1378 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_direct_access_grant.py
--rw-r--r--   0        0        0     1541 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_discovery.py
--rw-r--r--   0        0        0      590 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_jwk.py
--rw-r--r--   0        0        0     2274 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_message_encoding.py
--rw-r--r--   0        0        0      581 2023-05-11 13:50:35.117828 simple_openid_connect-0.2.5/tests/test_rp_initiated_logout.py
--rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.2.5/PKG-INFO
+-rw-r--r--   0        0        0       50 2022-11-30 14:49:54.727128 simple_openid_connect-0.3.0/.gitattributes
+-rw-r--r--   0        0        0     1584 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/.github/workflows/checks.yml
+-rw-r--r--   0        0        0      136 2022-11-24 12:36:21.336726 simple_openid_connect-0.3.0/.gitignore
+-rw-r--r--   0        0        0      795 2023-05-01 11:17:06.824014 simple_openid_connect-0.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      177 2022-11-12 20:14:29.642701 simple_openid_connect-0.3.0/.readthedocs.yaml
+-rw-r--r--   0        0        0      298 2023-05-01 11:41:49.264155 simple_openid_connect-0.3.0/DEVELOPMENT.md
+-rw-r--r--   0        0        0     1116 2022-11-11 18:16:08.603350 simple_openid_connect-0.3.0/LICENSE
+-rw-r--r--   0        0        0     4447 2023-05-01 11:17:53.814441 simple_openid_connect-0.3.0/README.md
+-rw-r--r--   0        0        0      679 2022-11-13 10:21:55.698024 simple_openid_connect-0.3.0/docs/Makefile
+-rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.3.0/docs/_static/.gitkeep
+-rw-r--r--   0        0        0        0 2022-11-11 18:16:08.603350 simple_openid_connect-0.3.0/docs/_templates/.gitkeep
+-rw-r--r--   0        0        0      320 2022-12-01 10:05:47.886671 simple_openid_connect-0.3.0/docs/api.rst
+-rw-r--r--   0        0        0     1790 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/docs/conf.py
+-rw-r--r--   0        0        0     5754 2023-05-25 12:20:30.617684 simple_openid_connect-0.3.0/docs/django-integration.rst
+-rw-r--r--   0        0        0     2615 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/docs/drf-integration.rst
+-rw-r--r--   0        0        0      708 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/docs/index.rst
+-rw-r--r--   0        0        0     1247 2023-05-01 09:33:59.061101 simple_openid_connect-0.3.0/docs/installation.rst
+-rw-r--r--   0        0        0     4868 2022-11-30 16:29:18.260734 simple_openid_connect-0.3.0/docs/usage.rst
+-rw-r--r--   0        0        0     2391 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      211 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/requirements.dev.txt
+-rw-r--r--   0        0        0      127 2023-06-08 15:32:31.583919 simple_openid_connect-0.3.0/src/simple_openid_connect/__init__.py
+-rw-r--r--   0        0        0     4204 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/src/simple_openid_connect/base_data.py
+-rw-r--r--   0        0        0    13090 2023-06-08 15:31:32.543916 simple_openid_connect-0.3.0/src/simple_openid_connect/client.py
+-rw-r--r--   0        0        0     3443 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/client_authentication.py
+-rw-r--r--   0        0        0    57274 2023-06-08 15:31:32.543916 simple_openid_connect-0.3.0/src/simple_openid_connect/data.py
+-rw-r--r--   0        0        0     1819 2022-11-30 12:04:05.293339 simple_openid_connect-0.3.0/src/simple_openid_connect/discovery.py
+-rw-r--r--   0        0        0     1174 2022-12-01 11:36:58.020255 simple_openid_connect-0.3.0/src/simple_openid_connect/exceptions.py
+-rw-r--r--   0        0        0      343 2023-05-01 11:17:53.814441 simple_openid_connect-0.3.0/src/simple_openid_connect/flows/__init__.py
+-rw-r--r--   0        0        0     5631 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/flows/authorization_code_flow/__init__.py
+-rw-r--r--   0        0        0     5823 2023-06-08 15:31:32.533916 simple_openid_connect-0.3.0/src/simple_openid_connect/flows/authorization_code_flow/client.py
+-rw-r--r--   0        0        0     2208 2023-05-01 11:18:30.258106 simple_openid_connect-0.3.0/src/simple_openid_connect/flows/direct_access_grant/__init__.py
+-rw-r--r--   0        0        0     1583 2023-05-01 11:18:30.258106 simple_openid_connect-0.3.0/src/simple_openid_connect/flows/direct_access_grant/client.py
+-rw-r--r--   0        0        0       53 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/__init__.py
+-rw-r--r--   0        0        0       61 2022-12-01 10:05:47.886671 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/__init__.py
+-rw-r--r--   0        0        0     5467 2023-05-01 11:22:04.083382 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/apps.py
+-rw-r--r--   0        0        0     4555 2022-12-01 10:05:47.886671 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/decorators.py
+-rw-r--r--   0        0        0     2630 2023-05-01 11:22:04.076716 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2022-12-01 10:05:47.886671 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/migrations/__init__.py
+-rw-r--r--   0        0        0     5728 2022-12-01 11:42:37.006937 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/models.py
+-rw-r--r--   0        0        0      381 2022-12-01 10:05:47.886671 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/templates/simple_openid_connect/login_failed.html
+-rw-r--r--   0        0        0      729 2022-12-08 12:24:29.349860 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/urls.py
+-rw-r--r--   0        0        0     2338 2022-12-01 10:05:47.886671 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/user_mapping.py
+-rw-r--r--   0        0        0     4415 2023-06-08 15:31:32.537250 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/views.py
+-rw-r--r--   0        0        0      306 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/__init__.py
+-rw-r--r--   0        0        0     4648 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/authentication.py
+-rw-r--r--   0        0        0      957 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py
+-rw-r--r--   0        0        0     2531 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/permissions.py
+-rw-r--r--   0        0        0      472 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/jwk.py
+-rw-r--r--   0        0        0      621 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/rp_initiated_logout.py
+-rw-r--r--   0        0        0     1509 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/token_introspection.py
+-rw-r--r--   0        0        0     1566 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/token_refresh.py
+-rw-r--r--   0        0        0     1393 2022-11-12 19:48:31.467498 simple_openid_connect-0.3.0/src/simple_openid_connect/userinfo.py
+-rw-r--r--   0        0        0      781 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/src/simple_openid_connect/utils.py
+-rw-r--r--   0        0        0    16938 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/tests/conftest.py
+-rw-r--r--   0        0        0        0 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/__init__.py
+-rw-r--r--   0        0        0     2785 2022-12-01 10:05:47.890004 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/settings.py
+-rw-r--r--   0        0        0     2586 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/conftest.py
+-rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py
+-rw-r--r--   0        0        0      633 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py
+-rw-r--r--   0        0        0     5247 2023-06-08 15:31:32.537250 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_login.py
+-rw-r--r--   0        0        0      687 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_logout.py
+-rw-r--r--   0        0        0     1248 2022-12-01 10:05:47.890004 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/urls.py
+-rw-r--r--   0        0        0      639 2022-12-01 10:05:47.890004 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/views.py
+-rw-r--r--   0        0        0      415 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/wsgi.py
+-rwxr-xr-x   0        0        0      675 2022-11-16 07:19:49.333600 simple_openid_connect-0.3.0/tests/django_test_project/manage.py
+-rw-r--r--   0        0        0     1746 2022-11-30 13:30:16.836909 simple_openid_connect-0.3.0/tests/interactive_tests/conftest.py
+-rw-r--r--   0        0        0     2001 2022-12-08 12:24:29.353193 simple_openid_connect-0.3.0/tests/interactive_tests/test_google.py
+-rw-r--r--   0        0        0     1668 2022-12-08 12:24:29.366526 simple_openid_connect-0.3.0/tests/test_authorization_code_flow.py
+-rw-r--r--   0        0        0     3115 2023-06-08 15:31:32.537250 simple_openid_connect-0.3.0/tests/test_client.py
+-rw-r--r--   0        0        0      934 2022-12-08 12:24:29.366526 simple_openid_connect-0.3.0/tests/test_client_auth.py
+-rw-r--r--   0        0        0     1378 2023-05-01 11:18:29.554766 simple_openid_connect-0.3.0/tests/test_direct_access_grant.py
+-rw-r--r--   0        0        0     1541 2022-12-08 12:24:29.366526 simple_openid_connect-0.3.0/tests/test_discovery.py
+-rw-r--r--   0        0        0      590 2022-12-08 12:24:29.366526 simple_openid_connect-0.3.0/tests/test_jwk.py
+-rw-r--r--   0        0        0     2274 2022-11-13 10:28:27.455234 simple_openid_connect-0.3.0/tests/test_message_encoding.py
+-rw-r--r--   0        0        0      581 2022-11-12 19:48:31.434164 simple_openid_connect-0.3.0/tests/test_rp_initiated_logout.py
+-rw-r--r--   0        0        0     5760 1970-01-01 00:00:00.000000 simple_openid_connect-0.3.0/PKG-INFO
```

### Comparing `simple_openid_connect-0.2.5/.github/workflows/checks.yml` & `simple_openid_connect-0.3.0/.github/workflows/checks.yml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/.pre-commit-config.yaml` & `simple_openid_connect-0.3.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/LICENSE` & `simple_openid_connect-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/README.md` & `simple_openid_connect-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/Makefile` & `simple_openid_connect-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/conf.py` & `simple_openid_connect-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/django-integration.rst` & `simple_openid_connect-0.3.0/docs/django-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/drf-integration.rst` & `simple_openid_connect-0.3.0/docs/drf-integration.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/index.rst` & `simple_openid_connect-0.3.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/installation.rst` & `simple_openid_connect-0.3.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/docs/usage.rst` & `simple_openid_connect-0.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/pyproject.toml` & `simple_openid_connect-0.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/base_data.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/base_data.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/client.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 """
 A more contiguous client implementation of the Openid-Connect protocol that offers simpler APIs at the cost of losing some flexibility.
 """
 
-from typing import Any, Dict, List, Literal, Mapping, Optional, Type, TypeVar, Union
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Literal,
+    Mapping,
+    Optional,
+    Type,
+    TypeVar,
+    Union,
+)
 
 from cryptojwt import JWK
 from cryptojwt.jwk.jwk import key_from_jwk_dict
 
 from simple_openid_connect import (
     jwk,
     rp_initiated_logout,
@@ -171,22 +182,58 @@
                 f"The OpenID provider {self.provider_config.issuer} does not support userinfo requests or does not advertise its userinfo endpoint"
             )
 
         return userinfo.fetch_userinfo(
             self.provider_config.userinfo_endpoint, access_token
         )
 
-    def decode_id_token(self, raw_token: str) -> IdToken:
+    def decode_id_token(
+        self,
+        raw_token: str,
+        nonce: Union[str, None] = None,
+        extra_trusted_audiences: List[str] = [],
+        min_iat: float = 0,
+        validate_acr: Union[Callable[[str], None], None] = None,
+        min_auth_time: float = 0,
+    ) -> IdToken:
         """
-        Decode and verify an encoded and signed id token
+        Decode and verify an encoded and signed id token.
+
+        Issuer and client id for validation are taken from the client configuration but extra optional validation
+        information can be supplied as well.
 
         :param raw_token: The encoded and signed id token.
             This could e.g. be retrieved as part of the authentication process and returned by the OP in :data:`TokenSuccessResponse.id_token <simple_openid_connect.flows.authorization_code_flow.data.TokenSuccessResponse.id_token>`.
-        """
-        return IdToken.parse_jws(raw_token, self.provider_keys)
+        :param nonce: The nonce that was used during authentication.
+            It is carried over by the OP into ID-Tokens and must now match.
+        :param extra_trusted_audiences: Which token audiences (client ids) to consider trusted beside this client's own client_id.
+            This is usually an empty list but if the token is intended to be used by more than one client, all of these need to be listed in the tokens :data:`IdToken.aud` field, and they all need to be known and trusted by this client.
+        :param min_iat: Minimum value that the tokens :data:`IdToken.iat` claim must be.
+            This value is a posix timestamp and defaults to 0 which allows arbitrarily old `iat` dates.
+        :param validate_acr: A callable that receives this tokens :data:`IdToken.acr` value and must perform its own validation.
+            This is necessary because the value of acr is outside OpenId-Connect specification and usage specific.
+            If not given, acr is assumed to always be valid.
+        :param min_auth_time: The point in time which is considered the minimum at which a user should have authenticated.
+            It basically means that if the user was authenticated very far in the past and reused their session, the time at which the original authentication took place must be greater than this value.
+            This is only validated if the :data:`IdToken.auth_time` is present in the token.
+            This value is a posix timestamp and default to 0 which allows arbitrarily old `auth_time` dates.
+
+        :raises ValidationError: if the validation fails
+        """
+        token = IdToken.parse_jws(raw_token, self.provider_keys)
+        token.validate_extern(
+            issuer=self.provider_config.issuer,
+            client_id=self.client_auth.client_id,
+            nonce=nonce,
+            extra_trusted_audiences=extra_trusted_audiences,
+            min_iat=min_iat,
+            validate_acr=validate_acr,
+            min_auth_time=min_auth_time,
+        )
+        return token
 
     def exchange_refresh_token(
         self, refresh_token: str
     ) -> Union[TokenSuccessResponse, TokenErrorResponse]:
         """
         Exchange a refresh token for new tokens
```

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/client_authentication.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/client_authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/data.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -218,15 +218,15 @@
         :param client_id: The client id of this client
         :param nonce: The nonce that was used during authentication.
             It is carried over by the OP into ID-Tokens and must now match.
         :param extra_trusted_audiences: Which token audiences (client ids) to consider trusted beside this client's own client_id.
             This is usually an empty list but if the token is intended to be used by more than one client, all of these need to be listed in the tokens :data:`IdToken.aud` field, and they all need to be known and trusted by this client.
         :param min_iat: Minimum value that the tokens :data:`IdToken.iat` claim must be.
             This value is a posix timestamp and defaults to 0 which allows arbitrarily old `iat` dates.
-        :param validate_acr: A callable that receives this tokens :data:`IdToken.acr` value and must perform it own validation.
+        :param validate_acr: A callable that receives this tokens :data:`IdToken.acr` value and must perform its own validation.
             This is necessary because the value of acr is outside OpenId-Connect specification and usage specific.
             If not given, acr is assumed to always be valid.
         :param min_auth_time: The point in time which is considered the minimum at which a user should have authenticated.
             It basically means that if the user was authenticated very far in the past and reused their session, the time at which the original authentication took place must be greater than this value.
             This is only validated if the :data:`IdToken.auth_time` is present in the token.
             This value is a posix timestamp and default to 0 which allows arbitrarily old `auth_time` dates.
```

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/discovery.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/exceptions.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/exceptions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/__init__.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/flows/authorization_code_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/authorization_code_flow/client.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/flows/authorization_code_flow/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/__init__.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/flows/direct_access_grant/__init__.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/flows/direct_access_grant/client.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/flows/direct_access_grant/client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/apps.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/apps.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/decorators.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/decorators.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/migrations/0001_initial.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/models.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/models.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/urls.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/user_mapping.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/user_mapping.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/django/views.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/django/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/authentication.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/authentication.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/drf_spectacular_schema.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/integrations/djangorestframework/permissions.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/integrations/djangorestframework/permissions.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/rp_initiated_logout.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/token_introspection.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/token_introspection.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/token_refresh.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/token_refresh.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/userinfo.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/userinfo.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/src/simple_openid_connect/utils.py` & `simple_openid_connect-0.3.0/src/simple_openid_connect/utils.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/conftest.py` & `simple_openid_connect-0.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/settings.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/settings.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/conftest.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_access_token_protected_view.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_frontchannel_logout_notifications.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_login.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/tests/test_logout.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/tests/test_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/urls.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/urls.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/django_test_project/views.py` & `simple_openid_connect-0.3.0/tests/django_test_project/django_test_project/views.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/django_test_project/manage.py` & `simple_openid_connect-0.3.0/tests/django_test_project/manage.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/interactive_tests/conftest.py` & `simple_openid_connect-0.3.0/tests/interactive_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/interactive_tests/test_google.py` & `simple_openid_connect-0.3.0/tests/interactive_tests/test_google.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_authorization_code_flow.py` & `simple_openid_connect-0.3.0/tests/test_authorization_code_flow.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_client.py` & `simple_openid_connect-0.3.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_client_auth.py` & `simple_openid_connect-0.3.0/tests/test_client_auth.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_direct_access_grant.py` & `simple_openid_connect-0.3.0/tests/test_direct_access_grant.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_discovery.py` & `simple_openid_connect-0.3.0/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_jwk.py` & `simple_openid_connect-0.3.0/tests/test_jwk.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_message_encoding.py` & `simple_openid_connect-0.3.0/tests/test_message_encoding.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/tests/test_rp_initiated_logout.py` & `simple_openid_connect-0.3.0/tests/test_rp_initiated_logout.py`

 * *Files identical despite different names*

### Comparing `simple_openid_connect-0.2.5/PKG-INFO` & `simple_openid_connect-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple_openid_connect
-Version: 0.2.5
+Version: 0.3.0
 Summary: Simple and opinionated OpenID-Connect relying party and resource server implementation
 Author-email: Finn-Thorben Sell <dev@finn-thorben.me>
 Requires-Python: ~=3.9
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Other Environment
```

