# Comparing `tmp/django_ninja_extra-0.18.9.tar.gz` & `tmp/django_ninja_extra-0.19.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ninja_extra-0.18.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_ninja_extra-0.19.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_ninja_extra-0.18.9.tar` & `django_ninja_extra-0.19.0.tar`

### file list

```diff
@@ -1,127 +1,127 @@
--rw-r--r--   0        0        0      269 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.coveragerc
--rw-r--r--   0        0        0       64 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.dockerignore
--rw-r--r--   0        0        0      126 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.flake8
--rw-r--r--   0        0        0      528 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.github/dependabot.yml
--rw-r--r--   0        0        0      661 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.github/workflows/publish.yml
--rw-r--r--   0        0        0      571 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.github/workflows/test.yml
--rw-r--r--   0        0        0     1323 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.github/workflows/test_full.yml
--rw-r--r--   0        0        0      114 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.gitignore
--rw-r--r--   0        0        0       52 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.isort.cfg
--rw-r--r--   0        0        0     1069 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1082 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/LICENSE
--rw-r--r--   0        0        0      968 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/Makefile
--rw-r--r--   0        0        0     3989 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/README.md
--rw-r--r--   0        0        0     3371 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/docs/api_controller/api_controller_permission.md
--rw-r--r--   0        0        0     3476 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/docs/api_controller/api_controller_route.md
--rw-r--r--   0        0        0     1546 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/docs/api_controller/api_controller_router.md
--rw-r--r--   0        0        0     7774 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/docs/api_controller/index.md
--rw-r--r--   0        0        0    51900 2023-05-29 13:27:19.155984 django_ninja_extra-0.18.9/docs/images/benchmark.png
--rw-r--r--   0        0        0  1100522 2023-05-29 13:27:19.163984 django_ninja_extra-0.18.9/docs/images/custom_exception.gif
--rwxr-xr-x   0        0        0  5136836 2023-05-29 13:27:19.203986 django_ninja_extra-0.18.9/docs/images/pagination_example.gif
--rw-r--r--   0        0        0  1478750 2023-05-29 13:27:19.211986 django_ninja_extra-0.18.9/docs/images/ui_swagger_preview_readme.gif
--rw-r--r--   0        0        0     4038 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/index.md
--rw-r--r--   0        0        0     5705 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/route_context.md
--rw-r--r--   0        0        0    12801 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/service_module_injector.md
--rw-r--r--   0        0        0     2028 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/settings.md
--rw-r--r--   0        0        0     2694 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/authentication.md
--rw-r--r--   0        0        0     1497 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/body_request.md
--rw-r--r--   0        0        0      975 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/custom_exception.md
--rw-r--r--   0        0        0     1025 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/form.md
--rw-r--r--   0        0        0     2958 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/index.md
--rw-r--r--   0        0        0     2782 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/ordering.md
--rw-r--r--   0        0        0     2324 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/pagination.md
--rw-r--r--   0        0        0      595 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/path.md
--rw-r--r--   0        0        0      756 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/query.md
--rw-r--r--   0        0        0     1276 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/schema.md
--rw-r--r--   0        0        0     3621 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/searching.md
--rw-r--r--   0        0        0     1847 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/testing.md
--rw-r--r--   0        0        0     7330 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/throttling.md
--rw-r--r--   0        0        0     2064 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/docs/tutorial/versioning.md
--rw-r--r--   0        0        0     1778 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/mkdocs.yml
--rw-r--r--   0        0        0      414 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/mypy.ini
--rw-r--r--   0        0        0     1087 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/__init__.py
--rw-r--r--   0        0        0     1291 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/apps.py
--rw-r--r--   0        0        0      440 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/compatible.py
--rw-r--r--   0        0        0       55 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/conf/__init__.py
--rw-r--r--   0        0        0     3554 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/conf/settings.py
--rw-r--r--   0        0        0      276 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/constants.py
--rw-r--r--   0        0        0      700 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/__init__.py
--rw-r--r--   0        0        0    17997 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/base.py
--rw-r--r--   0        0        0     1313 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/registry.py
--rw-r--r--   0        0        0     6265 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/response.py
--rw-r--r--   0        0        0    25969 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/route/__init__.py
--rw-r--r--   0        0        0     1125 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/route/context.py
--rw-r--r--   0        0        0     7744 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/controllers/route/route_functions.py
--rw-r--r--   0        0        0     1434 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/dependency_resolver.py
--rw-r--r--   0        0        0     1876 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/details.py
--rw-r--r--   0        0        0     8814 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/exceptions.py
--rw-r--r--   0        0        0     1775 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/generic.py
--rw-r--r--   0        0        0      597 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/helper.py
--rw-r--r--   0        0        0      670 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/lazy.py
--rw-r--r--   0        0        0       61 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/logger.py
--rw-r--r--   0        0        0     4322 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/main.py
--rw-r--r--   0        0        0     1305 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/modules.py
--rw-r--r--   0        0        0    19913 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/operation.py
--rw-r--r--   0        0        0     8324 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/ordering.py
--rw-r--r--   0        0        0     8259 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/pagination.py
--rw-r--r--   0        0        0      281 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/permissions/__init__.py
--rw-r--r--   0        0        0     5311 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/permissions/base.py
--rw-r--r--   0        0        0     1622 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/permissions/common.py
--rw-r--r--   0        0        0        0 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/py.typed
--rw-r--r--   0        0        0     2194 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/router.py
--rw-r--r--   0        0        0      313 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/schemas/__init__.py
--rw-r--r--   0        0        0     3573 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/schemas/response.py
--rw-r--r--   0        0        0     9412 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/searching.py
--rw-r--r--   0        0        0      748 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/security/__init__.py
--rw-r--r--   0        0        0      880 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/security/api_key.py
--rw-r--r--   0        0        0     1705 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/security/http.py
--rw-r--r--   0        0        0      542 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/security/session.py
--rw-r--r--   0        0        0     2516 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/shortcuts.py
--rw-r--r--   0        0        0      103 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/signals.py
--rw-r--r--   0        0        0     2515 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/status.py
--rw-r--r--   0        0        0      112 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/testing/__init__.py
--rw-r--r--   0        0        0     2059 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/testing/client.py
--rw-r--r--   0        0        0      318 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/throttling/__init__.py
--rw-r--r--   0        0        0     3921 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/throttling/decorator.py
--rw-r--r--   0        0        0     8211 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/throttling/model.py
--rw-r--r--   0        0        0      267 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/types.py
--rw-r--r--   0        0        0     1116 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/ninja_extra/urls.py
--rw-r--r--   0        0        0     2392 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/pyproject.toml
--rwxr-xr-x   0        0        0       61 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/pytest.ini
--rw-r--r--   0        0        0        0 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/__init__.py
--rw-r--r--   0        0        0     2181 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/conftest.py
--rw-r--r--   0        0        0     1332 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/controllers.py
--rw-r--r--   0        0        0      495 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/models.py
--rw-r--r--   0        0        0       89 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/schemas.py
--rw-r--r--   0        0        0     2121 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_api_instance.py
--rw-r--r--   0        0        0     7322 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_async_auth.py
--rw-r--r--   0        0        0    13342 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_controller.py
--rw-r--r--   0        0        0     1571 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_controller_registry.py
--rw-r--r--   0        0        0     2725 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_controller_response.py
--rw-r--r--   0        0        0     1871 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_dependency_resolver.py
--rw-r--r--   0        0        0     1059 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_django_model.py
--rw-r--r--   0        0        0     3533 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_django_ninja_router.py
--rw-r--r--   0        0        0     2157 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_event_controller.py
--rw-r--r--   0        0        0     6706 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_exceptions.py
--rw-r--r--   0        0        0     2048 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_generic_patch.py
--rw-r--r--   0        0        0      460 2023-05-29 13:27:19.215986 django_ninja_extra-0.18.9/tests/test_lazy_import.py
--rw-r--r--   0        0        0     4227 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_operation.py
--rw-r--r--   0        0        0    14220 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_ordering.py
--rw-r--r--   0        0        0    12132 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_pagination.py
--rw-r--r--   0        0        0    10048 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_permissions.py
--rw-r--r--   0        0        0    15512 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_route.py
--rw-r--r--   0        0        0    13597 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_searching.py
--rw-r--r--   0        0        0     2316 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_settings.py
--rw-r--r--   0        0        0     2466 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_shortcuts.py
--rw-r--r--   0        0        0     1051 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_status.py
--rw-r--r--   0        0        0     1274 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_testclient.py
--rw-r--r--   0        0        0        0 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/__init__.py
--rw-r--r--   0        0        0      461 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/sample_models.py
--rw-r--r--   0        0        0    10309 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/test_decorator.py
--rw-r--r--   0        0        0     7286 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/test_models.py
--rw-r--r--   0        0        0     2797 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/test_throttle_controller.py
--rw-r--r--   0        0        0     3536 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/test_throttle_decorator_on_controllers.py
--rw-r--r--   0        0        0     3345 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/test_throthling/test_throttling_xxf.py
--rw-r--r--   0        0        0      293 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/urls.py
--rw-r--r--   0        0        0     1769 2023-05-29 13:27:19.219987 django_ninja_extra-0.18.9/tests/utils.py
--rw-r--r--   0        0        0     6958 1970-01-01 00:00:00.000000 django_ninja_extra-0.18.9/PKG-INFO
+-rw-r--r--   0        0        0      269 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.coveragerc
+-rw-r--r--   0        0        0       64 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.dockerignore
+-rw-r--r--   0        0        0      126 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.flake8
+-rw-r--r--   0        0        0      528 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/dependabot.yml
+-rw-r--r--   0        0        0      661 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/workflows/publish.yml
+-rw-r--r--   0        0        0      571 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/workflows/test.yml
+-rw-r--r--   0        0        0     1323 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.github/workflows/test_full.yml
+-rw-r--r--   0        0        0      114 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.gitignore
+-rw-r--r--   0        0        0       52 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.isort.cfg
+-rw-r--r--   0        0        0     1069 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1082 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/LICENSE
+-rw-r--r--   0        0        0      968 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/Makefile
+-rw-r--r--   0        0        0     3989 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/README.md
+-rw-r--r--   0        0        0     3371 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/api_controller_permission.md
+-rw-r--r--   0        0        0     3476 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/api_controller_route.md
+-rw-r--r--   0        0        0     1546 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/api_controller_router.md
+-rw-r--r--   0        0        0     7774 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/api_controller/index.md
+-rw-r--r--   0        0        0    51900 2023-06-08 21:53:49.989941 django_ninja_extra-0.19.0/docs/images/benchmark.png
+-rw-r--r--   0        0        0  1100522 2023-06-08 21:53:49.993941 django_ninja_extra-0.19.0/docs/images/custom_exception.gif
+-rwxr-xr-x   0        0        0  5136836 2023-06-08 21:53:50.021942 django_ninja_extra-0.19.0/docs/images/pagination_example.gif
+-rw-r--r--   0        0        0  1478750 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/images/ui_swagger_preview_readme.gif
+-rw-r--r--   0        0        0     4038 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/index.md
+-rw-r--r--   0        0        0     5705 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/route_context.md
+-rw-r--r--   0        0        0    12801 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/service_module_injector.md
+-rw-r--r--   0        0        0     2028 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/settings.md
+-rw-r--r--   0        0        0     2694 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/authentication.md
+-rw-r--r--   0        0        0     1497 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/body_request.md
+-rw-r--r--   0        0        0      975 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/custom_exception.md
+-rw-r--r--   0        0        0     1025 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/form.md
+-rw-r--r--   0        0        0     2958 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/index.md
+-rw-r--r--   0        0        0     2782 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/ordering.md
+-rw-r--r--   0        0        0     2324 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/pagination.md
+-rw-r--r--   0        0        0      595 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/path.md
+-rw-r--r--   0        0        0      756 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/query.md
+-rw-r--r--   0        0        0     1276 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/schema.md
+-rw-r--r--   0        0        0     3621 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/searching.md
+-rw-r--r--   0        0        0     1847 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/testing.md
+-rw-r--r--   0        0        0     7330 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/throttling.md
+-rw-r--r--   0        0        0     2064 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/docs/tutorial/versioning.md
+-rw-r--r--   0        0        0     1778 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/mkdocs.yml
+-rw-r--r--   0        0        0      414 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/mypy.ini
+-rw-r--r--   0        0        0     1087 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/__init__.py
+-rw-r--r--   0        0        0     1291 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/apps.py
+-rw-r--r--   0        0        0      440 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/compatible.py
+-rw-r--r--   0        0        0       55 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/conf/__init__.py
+-rw-r--r--   0        0        0     3554 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/conf/settings.py
+-rw-r--r--   0        0        0      276 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/constants.py
+-rw-r--r--   0        0        0      700 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/__init__.py
+-rw-r--r--   0        0        0    17997 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/base.py
+-rw-r--r--   0        0        0     1313 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/registry.py
+-rw-r--r--   0        0        0     6265 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/response.py
+-rw-r--r--   0        0        0    25969 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/route/__init__.py
+-rw-r--r--   0        0        0     1125 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/route/context.py
+-rw-r--r--   0        0        0     7744 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/controllers/route/route_functions.py
+-rw-r--r--   0        0        0     1434 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/dependency_resolver.py
+-rw-r--r--   0        0        0     1876 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/details.py
+-rw-r--r--   0        0        0     8814 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/exceptions.py
+-rw-r--r--   0        0        0     1775 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/generic.py
+-rw-r--r--   0        0        0      597 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/helper.py
+-rw-r--r--   0        0        0      670 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/lazy.py
+-rw-r--r--   0        0        0       61 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/logger.py
+-rw-r--r--   0        0        0     4322 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/main.py
+-rw-r--r--   0        0        0     1305 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/modules.py
+-rw-r--r--   0        0        0    19913 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/operation.py
+-rw-r--r--   0        0        0     8324 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/ordering.py
+-rw-r--r--   0        0        0     8259 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/pagination.py
+-rw-r--r--   0        0        0      281 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/permissions/__init__.py
+-rw-r--r--   0        0        0     5311 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/permissions/base.py
+-rw-r--r--   0        0        0     1622 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/permissions/common.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/py.typed
+-rw-r--r--   0        0        0     2194 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/router.py
+-rw-r--r--   0        0        0      313 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/schemas/__init__.py
+-rw-r--r--   0        0        0     3573 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/schemas/response.py
+-rw-r--r--   0        0        0     9412 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/searching.py
+-rw-r--r--   0        0        0      748 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/__init__.py
+-rw-r--r--   0        0        0      880 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/api_key.py
+-rw-r--r--   0        0        0     1705 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/http.py
+-rw-r--r--   0        0        0      542 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/security/session.py
+-rw-r--r--   0        0        0     2516 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/shortcuts.py
+-rw-r--r--   0        0        0      103 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/signals.py
+-rw-r--r--   0        0        0     2515 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/status.py
+-rw-r--r--   0        0        0      112 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/testing/__init__.py
+-rw-r--r--   0        0        0     2059 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/testing/client.py
+-rw-r--r--   0        0        0      318 2023-06-08 21:53:50.029942 django_ninja_extra-0.19.0/ninja_extra/throttling/__init__.py
+-rw-r--r--   0        0        0     3921 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/throttling/decorator.py
+-rw-r--r--   0        0        0     8211 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/throttling/model.py
+-rw-r--r--   0        0        0      267 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/types.py
+-rw-r--r--   0        0        0     1116 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/ninja_extra/urls.py
+-rw-r--r--   0        0        0     2392 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/pyproject.toml
+-rwxr-xr-x   0        0        0       61 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/pytest.ini
+-rw-r--r--   0        0        0        0 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/__init__.py
+-rw-r--r--   0        0        0     2181 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/conftest.py
+-rw-r--r--   0        0        0     1332 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/controllers.py
+-rw-r--r--   0        0        0      495 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/models.py
+-rw-r--r--   0        0        0       89 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/schemas.py
+-rw-r--r--   0        0        0     2121 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_api_instance.py
+-rw-r--r--   0        0        0     7322 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_async_auth.py
+-rw-r--r--   0        0        0    13342 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_controller.py
+-rw-r--r--   0        0        0     1571 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_controller_registry.py
+-rw-r--r--   0        0        0     2725 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_controller_response.py
+-rw-r--r--   0        0        0     1871 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_dependency_resolver.py
+-rw-r--r--   0        0        0     1059 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_django_model.py
+-rw-r--r--   0        0        0     3533 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_django_ninja_router.py
+-rw-r--r--   0        0        0     2157 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_event_controller.py
+-rw-r--r--   0        0        0     6706 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0     2048 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_generic_patch.py
+-rw-r--r--   0        0        0      460 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_lazy_import.py
+-rw-r--r--   0        0        0     4227 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_operation.py
+-rw-r--r--   0        0        0    14220 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_ordering.py
+-rw-r--r--   0        0        0    12132 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_pagination.py
+-rw-r--r--   0        0        0    10048 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_permissions.py
+-rw-r--r--   0        0        0    15512 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_route.py
+-rw-r--r--   0        0        0    13597 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_searching.py
+-rw-r--r--   0        0        0     2316 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_settings.py
+-rw-r--r--   0        0        0     2466 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_shortcuts.py
+-rw-r--r--   0        0        0     1051 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_status.py
+-rw-r--r--   0        0        0     1274 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_testclient.py
+-rw-r--r--   0        0        0        0 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/__init__.py
+-rw-r--r--   0        0        0      461 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/sample_models.py
+-rw-r--r--   0        0        0    10309 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_decorator.py
+-rw-r--r--   0        0        0     7286 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_models.py
+-rw-r--r--   0        0        0     2797 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_controller.py
+-rw-r--r--   0        0        0     3536 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_decorator_on_controllers.py
+-rw-r--r--   0        0        0     3345 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/test_throthling/test_throttling_xxf.py
+-rw-r--r--   0        0        0      293 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/urls.py
+-rw-r--r--   0        0        0     1769 2023-06-08 21:53:50.033942 django_ninja_extra-0.19.0/tests/utils.py
+-rw-r--r--   0        0        0     6958 1970-01-01 00:00:00.000000 django_ninja_extra-0.19.0/PKG-INFO
```

### Comparing `django_ninja_extra-0.18.9/.github/dependabot.yml` & `django_ninja_extra-0.19.0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/.github/workflows/publish.yml` & `django_ninja_extra-0.19.0/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/.github/workflows/test.yml` & `django_ninja_extra-0.19.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/.github/workflows/test_full.yml` & `django_ninja_extra-0.19.0/.github/workflows/test_full.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/.pre-commit-config.yaml` & `django_ninja_extra-0.19.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/LICENSE` & `django_ninja_extra-0.19.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/Makefile` & `django_ninja_extra-0.19.0/Makefile`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/README.md` & `django_ninja_extra-0.19.0/README.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/api_controller/api_controller_permission.md` & `django_ninja_extra-0.19.0/docs/api_controller/api_controller_permission.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/api_controller/api_controller_route.md` & `django_ninja_extra-0.19.0/docs/api_controller/api_controller_route.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/api_controller/api_controller_router.md` & `django_ninja_extra-0.19.0/docs/api_controller/api_controller_router.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/api_controller/index.md` & `django_ninja_extra-0.19.0/docs/api_controller/index.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/images/benchmark.png` & `django_ninja_extra-0.19.0/docs/images/benchmark.png`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/images/custom_exception.gif` & `django_ninja_extra-0.19.0/docs/images/custom_exception.gif`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/images/pagination_example.gif` & `django_ninja_extra-0.19.0/docs/images/pagination_example.gif`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/images/ui_swagger_preview_readme.gif` & `django_ninja_extra-0.19.0/docs/images/ui_swagger_preview_readme.gif`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/index.md` & `django_ninja_extra-0.19.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/route_context.md` & `django_ninja_extra-0.19.0/docs/route_context.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/service_module_injector.md` & `django_ninja_extra-0.19.0/docs/service_module_injector.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/settings.md` & `django_ninja_extra-0.19.0/docs/settings.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/authentication.md` & `django_ninja_extra-0.19.0/docs/tutorial/authentication.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/body_request.md` & `django_ninja_extra-0.19.0/docs/tutorial/body_request.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/custom_exception.md` & `django_ninja_extra-0.19.0/docs/tutorial/custom_exception.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/form.md` & `django_ninja_extra-0.19.0/docs/tutorial/form.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/index.md` & `django_ninja_extra-0.19.0/docs/tutorial/index.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/ordering.md` & `django_ninja_extra-0.19.0/docs/tutorial/ordering.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/pagination.md` & `django_ninja_extra-0.19.0/docs/tutorial/pagination.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/path.md` & `django_ninja_extra-0.19.0/docs/tutorial/path.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/query.md` & `django_ninja_extra-0.19.0/docs/tutorial/query.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/schema.md` & `django_ninja_extra-0.19.0/docs/tutorial/schema.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/searching.md` & `django_ninja_extra-0.19.0/docs/tutorial/searching.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/testing.md` & `django_ninja_extra-0.19.0/docs/tutorial/testing.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/throttling.md` & `django_ninja_extra-0.19.0/docs/tutorial/throttling.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/docs/tutorial/versioning.md` & `django_ninja_extra-0.19.0/docs/tutorial/versioning.md`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/mkdocs.yml` & `django_ninja_extra-0.19.0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/__init__.py` & `django_ninja_extra-0.19.0/ninja_extra/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)"""
 
-__version__ = "0.18.9"
+__version__ = "0.19.0"
 
 import django
 
 from ninja_extra.controllers import (
     ControllerBase,
     api_controller,
     http_delete,
```

### Comparing `django_ninja_extra-0.18.9/ninja_extra/apps.py` & `django_ninja_extra-0.19.0/ninja_extra/apps.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/conf/settings.py` & `django_ninja_extra-0.19.0/ninja_extra/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/__init__.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/base.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/base.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/registry.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/registry.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/response.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/route/__init__.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/route/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/route/context.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/route/context.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/controllers/route/route_functions.py` & `django_ninja_extra-0.19.0/ninja_extra/controllers/route/route_functions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/dependency_resolver.py` & `django_ninja_extra-0.19.0/ninja_extra/dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/details.py` & `django_ninja_extra-0.19.0/ninja_extra/details.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/exceptions.py` & `django_ninja_extra-0.19.0/ninja_extra/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/generic.py` & `django_ninja_extra-0.19.0/ninja_extra/generic.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/helper.py` & `django_ninja_extra-0.19.0/ninja_extra/helper.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/lazy.py` & `django_ninja_extra-0.19.0/ninja_extra/lazy.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/main.py` & `django_ninja_extra-0.19.0/ninja_extra/main.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/modules.py` & `django_ninja_extra-0.19.0/ninja_extra/modules.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/operation.py` & `django_ninja_extra-0.19.0/ninja_extra/operation.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/ordering.py` & `django_ninja_extra-0.19.0/ninja_extra/ordering.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/pagination.py` & `django_ninja_extra-0.19.0/ninja_extra/pagination.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/permissions/base.py` & `django_ninja_extra-0.19.0/ninja_extra/permissions/base.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/permissions/common.py` & `django_ninja_extra-0.19.0/ninja_extra/permissions/common.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/router.py` & `django_ninja_extra-0.19.0/ninja_extra/router.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/schemas/response.py` & `django_ninja_extra-0.19.0/ninja_extra/schemas/response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/searching.py` & `django_ninja_extra-0.19.0/ninja_extra/searching.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/security/__init__.py` & `django_ninja_extra-0.19.0/ninja_extra/security/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/security/api_key.py` & `django_ninja_extra-0.19.0/ninja_extra/security/api_key.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/security/http.py` & `django_ninja_extra-0.19.0/ninja_extra/security/http.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/security/session.py` & `django_ninja_extra-0.19.0/ninja_extra/security/session.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/shortcuts.py` & `django_ninja_extra-0.19.0/ninja_extra/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/status.py` & `django_ninja_extra-0.19.0/ninja_extra/status.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/testing/client.py` & `django_ninja_extra-0.19.0/ninja_extra/testing/client.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/throttling/decorator.py` & `django_ninja_extra-0.19.0/ninja_extra/throttling/decorator.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/throttling/model.py` & `django_ninja_extra-0.19.0/ninja_extra/throttling/model.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/ninja_extra/urls.py` & `django_ninja_extra-0.19.0/ninja_extra/urls.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/pyproject.toml` & `django_ninja_extra-0.19.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     "Framework :: AsyncIO",
     "Topic :: Internet :: WWW/HTTP :: HTTP Servers",
     "Topic :: Internet :: WWW/HTTP",
 ]
 
 requires = [
     "Django >= 2.2",
-    "django-ninja == 0.22.1",
+    "django-ninja == 0.22.2",
     "injector >= 0.19.0",
     "asgiref",
     "contextlib2"
 ]
 description-file = "README.md"
 requires-python = ">=3.6"
```

### Comparing `django_ninja_extra-0.18.9/tests/conftest.py` & `django_ninja_extra-0.19.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/controllers.py` & `django_ninja_extra-0.19.0/tests/controllers.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_api_instance.py` & `django_ninja_extra-0.19.0/tests/test_api_instance.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_async_auth.py` & `django_ninja_extra-0.19.0/tests/test_async_auth.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_controller.py` & `django_ninja_extra-0.19.0/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_controller_registry.py` & `django_ninja_extra-0.19.0/tests/test_controller_registry.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_controller_response.py` & `django_ninja_extra-0.19.0/tests/test_controller_response.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_dependency_resolver.py` & `django_ninja_extra-0.19.0/tests/test_dependency_resolver.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_django_model.py` & `django_ninja_extra-0.19.0/tests/test_django_model.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_django_ninja_router.py` & `django_ninja_extra-0.19.0/tests/test_django_ninja_router.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_event_controller.py` & `django_ninja_extra-0.19.0/tests/test_event_controller.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_exceptions.py` & `django_ninja_extra-0.19.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_generic_patch.py` & `django_ninja_extra-0.19.0/tests/test_generic_patch.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_operation.py` & `django_ninja_extra-0.19.0/tests/test_operation.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_ordering.py` & `django_ninja_extra-0.19.0/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_pagination.py` & `django_ninja_extra-0.19.0/tests/test_pagination.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_permissions.py` & `django_ninja_extra-0.19.0/tests/test_permissions.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_route.py` & `django_ninja_extra-0.19.0/tests/test_route.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_searching.py` & `django_ninja_extra-0.19.0/tests/test_searching.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_settings.py` & `django_ninja_extra-0.19.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_shortcuts.py` & `django_ninja_extra-0.19.0/tests/test_shortcuts.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_status.py` & `django_ninja_extra-0.19.0/tests/test_status.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_testclient.py` & `django_ninja_extra-0.19.0/tests/test_testclient.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_throthling/test_decorator.py` & `django_ninja_extra-0.19.0/tests/test_throthling/test_decorator.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_throthling/test_models.py` & `django_ninja_extra-0.19.0/tests/test_throthling/test_models.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_throthling/test_throttle_controller.py` & `django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_controller.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_throthling/test_throttle_decorator_on_controllers.py` & `django_ninja_extra-0.19.0/tests/test_throthling/test_throttle_decorator_on_controllers.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/test_throthling/test_throttling_xxf.py` & `django_ninja_extra-0.19.0/tests/test_throthling/test_throttling_xxf.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/tests/utils.py` & `django_ninja_extra-0.19.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `django_ninja_extra-0.18.9/PKG-INFO` & `django_ninja_extra-0.19.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ninja-extra
-Version: 0.18.9
+Version: 0.19.0
 Summary: Django Ninja Extra - Class Based Utility and more for Django Ninja(Fast Django REST framework)
 Home-page: https://github.com/eadwinCode/django-ninja-extra
 Author: Ezeudoh Tochukwu
 Author-email: tochukwu.ezeudoh@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Information Technology
@@ -35,15 +35,15 @@
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
 Classifier: Framework :: AsyncIO
 Classifier: Topic :: Internet :: WWW/HTTP :: HTTP Servers
 Classifier: Topic :: Internet :: WWW/HTTP
 Requires-Dist: Django >= 2.2
-Requires-Dist: django-ninja == 0.22.1
+Requires-Dist: django-ninja == 0.22.2
 Requires-Dist: injector >= 0.19.0
 Requires-Dist: asgiref
 Requires-Dist: contextlib2
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: mkdocs >=1.1.2,<2.0.0 ; extra == "doc"
 Requires-Dist: mkdocs-material >=7.1.9,<8.0.0 ; extra == "doc"
 Requires-Dist: mdx-include >=1.4.1,<2.0.0 ; extra == "doc"
```

