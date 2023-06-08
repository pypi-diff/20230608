# Comparing `tmp/switch_api-0.3.3.tar.gz` & `tmp/switch_api-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "switch_api-0.3.3.tar", last modified: Fri Apr 14 07:05:02 2023, max compression
+gzip compressed data, was "switch_api-0.4.5.tar", last modified: Thu Jun  8 04:05:26 2023, max compression
```

## Comparing `switch_api-0.3.3.tar` & `switch_api-0.4.5.tar`

### file list

```diff
@@ -1,64 +1,67 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/
--rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-04-14 07:04:48.000000 switch_api-0.3.3/AUTHORS.rst
--rw-r--r--   0 vsts      (1001) docker     (122)    25085 2023-04-14 07:04:48.000000 switch_api-0.3.3/HISTORY.md
--rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-04-14 07:04:48.000000 switch_api-0.3.3/LICENCE
--rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-04-14 07:04:48.000000 switch_api-0.3.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)    26359 2023-04-14 07:05:02.709312 switch_api-0.3.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-04-14 07:04:48.000000 switch_api-0.3.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-04-14 07:04:48.000000 switch_api-0.3.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-04-14 07:05:02.713312 switch_api-0.3.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (122)     1346 2023-04-14 07:04:48.000000 switch_api-0.3.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/
--rw-r--r--   0 vsts      (1001) docker     (122)     1358 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/_authentication/
--rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_authentication.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/_authentication/_credentials_store/
--rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_credentials_store/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_credentials_store/_credentials_store.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api/_authentication/_msal/
--rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_msal/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_authentication/_msal/_custom_application.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/_utils/
--rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3651 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/_constants.py
--rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/_platform.py
--rw-r--r--   0 vsts      (1001) docker     (122)    15497 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/_utils/_utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/analytics/
--rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/analytics/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/analytics/analytics.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/cache/
--rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/cache/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/cache/cache.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/dataset/
--rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/dataset/dataset.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/error_handlers/
--rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/error_handlers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/error_handlers/error_handlers.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/extensions/
--rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     7627 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/extensions.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/field_meta.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3051 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/extensions/pipeline.py
--rw-r--r--   0 vsts      (1001) docker     (122)     3193 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/initialize.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/integration/
--rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (122)    89587 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/integration/integration.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/pipeline/
--rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/automation.py
--rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/definitions.py
--rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/pipeline/pipeline.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.709312 switch_api-0.3.3/switch_api/platform_insights/
--rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/platform_insights/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-04-14 07:04:48.000000 switch_api-0.3.3/switch_api/platform_insights/platform_insights.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-04-14 07:05:02.705312 switch_api-0.3.3/switch_api.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)    26359 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1538 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-04-14 07:05:02.000000 switch_api-0.3.3/switch_api.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.083871 switch_api-0.4.5/
+-rw-r--r--   0 vsts      (1001) docker     (122)      249 2023-06-08 04:05:07.000000 switch_api-0.4.5/AUTHORS.rst
+-rw-r--r--   0 vsts      (1001) docker     (122)    26519 2023-06-08 04:05:07.000000 switch_api-0.4.5/HISTORY.md
+-rw-r--r--   0 vsts      (1001) docker     (122)     1093 2023-06-08 04:05:07.000000 switch_api-0.4.5/LICENCE
+-rw-r--r--   0 vsts      (1001) docker     (122)       74 2023-06-08 04:05:07.000000 switch_api-0.4.5/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (122)    27793 2023-06-08 04:05:26.083871 switch_api-0.4.5/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)      590 2023-06-08 04:05:07.000000 switch_api-0.4.5/README.md
+-rw-r--r--   0 vsts      (1001) docker     (122)      113 2023-06-08 04:05:07.000000 switch_api-0.4.5/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (122)       62 2023-06-08 04:05:26.083871 switch_api-0.4.5/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (122)     1346 2023-06-08 04:05:07.000000 switch_api-0.4.5/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1453 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_authentication/
+-rw-r--r--   0 vsts      (1001) docker     (122)      391 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7898 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_authentication.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_authentication/_credentials_store/
+-rw-r--r--   0 vsts      (1001) docker     (122)      393 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_credentials_store/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     5851 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_credentials_store/_credentials_store.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_authentication/_msal/
+-rw-r--r--   0 vsts      (1001) docker     (122)      361 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_msal/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     8752 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_authentication/_msal/_custom_application.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/_utils/
+-rw-r--r--   0 vsts      (1001) docker     (122)      462 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3651 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/_constants.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    12998 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/_platform.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    16873 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/_utils/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/analytics/
+-rw-r--r--   0 vsts      (1001) docker     (122)      578 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/analytics/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     9561 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/analytics/analytics.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/cache/
+-rw-r--r--   0 vsts      (1001) docker     (122)      480 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/cache/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     6985 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/cache/cache.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (122)      558 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7724 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/dataset/dataset.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/email/
+-rw-r--r--   0 vsts      (1001) docker     (122)      472 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/email/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     4638 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/email/email_sender.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/error_handlers/
+-rw-r--r--   0 vsts      (1001) docker     (122)     2028 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/error_handlers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11845 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/error_handlers/error_handlers.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/extensions/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1038 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     7519 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/extensions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1652 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/field_meta.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2970 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     1406 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/extensions/pipeline.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     3193 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/initialize.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/integration/
+-rw-r--r--   0 vsts      (1001) docker     (122)     1601 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    11314 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    26453 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    89676 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/integration/integration.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api/pipeline/
+-rw-r--r--   0 vsts      (1001) docker     (122)     3144 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    69447 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/automation.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    35931 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/definitions.py
+-rw-r--r--   0 vsts      (1001) docker     (122)    21094 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/pipeline/pipeline.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.083871 switch_api-0.4.5/switch_api/platform_insights/
+-rw-r--r--   0 vsts      (1001) docker     (122)      542 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/platform_insights/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (122)     2214 2023-06-08 04:05:07.000000 switch_api-0.4.5/switch_api/platform_insights/platform_insights.py
+drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-06-08 04:05:26.079871 switch_api-0.4.5/switch_api.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (122)    27793 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (122)     1600 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       84 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (122)       11 2023-06-08 04:05:26.000000 switch_api-0.4.5/switch_api.egg-info/top_level.txt
```

### Comparing `switch_api-0.3.3/HISTORY.md` & `switch_api-0.4.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,95 @@
+Metadata-Version: 2.1
+Name: switch_api
+Version: 0.4.5
+Summary: A complete package for data ingestion into the Switch Automation Platform.
+Home-page: UNKNOWN
+Author: Switch Automation Pty Ltd.
+License: MIT License
+Platform: UNKNOWN
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Intended Audience :: Other Audience
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Natural Language :: English
+Requires-Python: >=3.8.0
+Description-Content-Type: text/markdown
+License-File: LICENCE
+License-File: AUTHORS.rst
+
+# Switch Automation library for Python
+This is a package for data ingestion into the Switch Automation software platform. 
+
+You can find out more about the platform on [Switch Automation](https://www.switchautomation.com)
+
+## Getting started
+
+### Prerequisites
+* Python 3.8 or later is required to use this package. 
+* You must have a [Switch Automation user account](https://www.switchautomation.com/our-solution/) to use this package. 
+
+### Install the package
+Install the Switch Automation library for Python with [pip](https://pypi.org/project/pip/):
+
+```bash
+pip install switch_api
+```
+
 # History
 
+## 0.4.5
+
+### Added
+- Email Sender Module
+  - Send emails to active users within a Portfolio in Switch Automation Platform
+  - Limitations:
+    - Emails cannot be sent to users outside of the Portfolio including other users within the platform
+    - Maximum of five attachments per email
+    - Each attachment has a maximum size of 5mb
+  - See function code documentation and usage example below
+- New `generate_filepath` method to provide a filepath where files can be stored
+  - Works well with the attachment feature of the Email Sender Module. Store files in the generated filepath of this method and pass into email attachments
+  - See function code documentation and usage example below
+
+### Email Sender Usage
+```python
+import switch_api as sw
+
+sw.email.send_email(
+    api_inputs=api_inputs,
+    subject='',
+    body='',
+    to_recipients=[],
+    cc_recipients=[], # Optional
+    bcc_recipients=[], # Optional
+    attachments=['/file/path/to/attachment.csv'], # Optional
+    conversation_id='' # Optional
+)
+```
+
+### generate_filepath Usage
+```python
+import switch_api as sw
+
+generated_attachment_filepath = sw.generate_filepath(api_inputs=api_inputs, filename='generated_attachment.txt')
+
+# Example of where it could be used
+sw.email.send_email(
+    ...
+    attachments=[generated_attachment_filepath]
+    ...
+)
+```
+
+
+### Fixed
+- Issue where `upsert_device_sensors_ext` method was not posting metadata and tag_columns to API
+
 ## 0.3.3
 
 ### Added
 - New `upsert_device_sensors_ext` method to the `integration` module.
   - Compared to existing `upsert_device_sensors` following are supported:
     - Installation Code or Installation Id may be provided
       - BUT cannot provide mix of the two, all must have either code or id and not both.
@@ -702,7 +788,9 @@
 - `kql`
 
 Removed the `name_as_filename` and `treat_as_timeseries` parameter from the following functions:
 
 - `switch.integration.replace_data()`
 - `switch.integration.append_data()`
 - `switch.integration.upload_data()`
+
+
```

### Comparing `switch_api-0.3.3/LICENCE` & `switch_api-0.4.5/LICENCE`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/PKG-INFO` & `switch_api-0.4.5/switch_api.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: switch_api
-Version: 0.3.3
+Name: switch-api
+Version: 0.4.5
 Summary: A complete package for data ingestion into the Switch Automation Platform.
 Home-page: UNKNOWN
 Author: Switch Automation Pty Ltd.
 License: MIT License
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Intended Audience :: Other Audience
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Natural Language :: English
-Requires-Python: >=3.8.*
+Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 License-File: LICENCE
 License-File: AUTHORS.rst
 
 # Switch Automation library for Python
 This is a package for data ingestion into the Switch Automation software platform. 
 
@@ -34,14 +34,62 @@
 
 ```bash
 pip install switch_api
 ```
 
 # History
 
+## 0.4.5
+
+### Added
+- Email Sender Module
+  - Send emails to active users within a Portfolio in Switch Automation Platform
+  - Limitations:
+    - Emails cannot be sent to users outside of the Portfolio including other users within the platform
+    - Maximum of five attachments per email
+    - Each attachment has a maximum size of 5mb
+  - See function code documentation and usage example below
+- New `generate_filepath` method to provide a filepath where files can be stored
+  - Works well with the attachment feature of the Email Sender Module. Store files in the generated filepath of this method and pass into email attachments
+  - See function code documentation and usage example below
+
+### Email Sender Usage
+```python
+import switch_api as sw
+
+sw.email.send_email(
+    api_inputs=api_inputs,
+    subject='',
+    body='',
+    to_recipients=[],
+    cc_recipients=[], # Optional
+    bcc_recipients=[], # Optional
+    attachments=['/file/path/to/attachment.csv'], # Optional
+    conversation_id='' # Optional
+)
+```
+
+### generate_filepath Usage
+```python
+import switch_api as sw
+
+generated_attachment_filepath = sw.generate_filepath(api_inputs=api_inputs, filename='generated_attachment.txt')
+
+# Example of where it could be used
+sw.email.send_email(
+    ...
+    attachments=[generated_attachment_filepath]
+    ...
+)
+```
+
+
+### Fixed
+- Issue where `upsert_device_sensors_ext` method was not posting metadata and tag_columns to API
+
 ## 0.3.3
 
 ### Added
 - New `upsert_device_sensors_ext` method to the `integration` module.
   - Compared to existing `upsert_device_sensors` following are supported:
     - Installation Code or Installation Id may be provided
       - BUT cannot provide mix of the two, all must have either code or id and not both.
```

### Comparing `switch_api-0.3.3/README.md` & `switch_api-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/setup.py` & `switch_api-0.4.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 setup(
     author="Switch Automation Pty Ltd.",
     description="A complete package for data ingestion into the Switch Automation Platform.",
     long_description=open('README.md', 'r').read() + '\n\n' + open('HISTORY.md', 'r').read(),
     long_description_content_type='text/markdown',
     license='MIT License',
     name="switch_api",
-    version="0.3.3",
+    version="0.4.5",
     packages=find_packages(include=["switch_api", "switch_api.*"]),
     install_requires=['pandas', 'requests', 'azure-storage-blob', 'pandera[io]==0.7.1', 'azure-servicebus', 'msal>=1.11.0'],
-    python_requires=">=3.8.*",
+    python_requires=">=3.8.0",
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         "License :: OSI Approved :: MIT License",
         'Intended Audience :: Other Audience',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
```

### Comparing `switch_api-0.3.3/switch_api/_authentication/_authentication.py` & `switch_api-0.4.5/switch_api/_authentication/_authentication.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/_authentication/_credentials_store/_credentials_store.py` & `switch_api-0.4.5/switch_api/_authentication/_credentials_store/_credentials_store.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/_authentication/_msal/_custom_application.py` & `switch_api-0.4.5/switch_api/_authentication/_msal/_custom_application.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/_utils/_constants.py` & `switch_api-0.4.5/switch_api/_utils/_constants.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/_utils/_platform.py` & `switch_api-0.4.5/switch_api/_utils/_platform.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/_utils/_utils.py` & `switch_api-0.4.5/switch_api/_utils/_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # Licensed under the MIT License. See License.txt in the project root for
 # license information.
 # --------------------------------------------------------------------------
 """
 A module for .....
 """
 # import datetime
+import os
 import re
+import tempfile
 import uuid
 from collections import namedtuple
 from typing import Union, List
 import string
 import secrets
 import pandas
 import pandera
@@ -279,14 +281,49 @@
          
         uuid_obj = uuid.UUID(str(uuid_to_test), version=version)
     except Exception:
         return False
 
     return str(uuid_obj) == uuid_to_test
 
+def generate_filepath(api_inputs: ApiInputs, filename: str, unique: bool = True):
+    """
+    Generates a filepath given the filename. Optionally, setting unique will append uniqueness to the filepath.
+
+    Parameters
+    ----------
+    filename: str
+        Name of the file to be generated. Include file extension where applicable.
+    unique: bool
+        If True, 
+        and api_inputs.data_feed_id and api_inputs.data_feed_file_status_id are valid identifiers,
+        the filepath will include the ids. Otherwise, the filepath will generate a unique directory prefix.
+        If False, the filepath will match the parameters and uniqueness is left to the user.
+
+    Returns
+    -------
+    str
+        Filepath of the generated file.
+    """
+    
+    tempDirPath = tempfile.gettempdir()
+
+    directory = os.path.join(tempDirPath, 'SwitchTaskInsights', 'projects', api_inputs.api_project_id)
+
+    if unique:
+        if is_valid_uuid(api_inputs.data_feed_id) and is_valid_uuid(api_inputs.data_feed_file_status_id):
+            directory = os.path.join(directory, 'df', api_inputs.data_feed_id, 'dffs', api_inputs.data_feed_file_status_id)
+        else:
+            directory = os.path.join(directory, 'unq', str(uuid.uuid4()))
+
+    if not os.path.exists(directory):
+        os.makedirs(directory)
+
+    return os.path.join(directory, filename)
+
 def convert_bytes(bytes_number):
     tags = [ "Byte", "Kilobyte", "Megabyte", "Gigabyte", "Terabyte" ]
  
     i = 0
     double_bytes = bytes_number
  
     while (i < len(tags) and  bytes_number >= 1024):
```

### Comparing `switch_api-0.3.3/switch_api/analytics/__init__.py` & `switch_api-0.4.5/switch_api/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/analytics/analytics.py` & `switch_api-0.4.5/switch_api/analytics/analytics.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/cache/cache.py` & `switch_api-0.4.5/switch_api/cache/cache.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/dataset/__init__.py` & `switch_api-0.4.5/switch_api/dataset/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/dataset/dataset.py` & `switch_api-0.4.5/switch_api/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/error_handlers/__init__.py` & `switch_api-0.4.5/switch_api/error_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/error_handlers/error_handlers.py` & `switch_api-0.4.5/switch_api/error_handlers/error_handlers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/extensions/__init__.py` & `switch_api-0.4.5/switch_api/extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/extensions/extensions.py` & `switch_api-0.4.5/switch_api/extensions/extensions.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 """Module providing support for extensions to the Task classes."""
 
 from typing import List, Tuple, Union, get_type_hints
 
 from .pipeline import ExtensionTask
 from .field_meta import FieldMeta
-from .helpers import __get_code, convert_to_serializeable_fields, find_cycles_by_field_type, has_annotations, HasExtensionClsAttributeName
+from .helpers import get_code, convert_to_serializeable_fields, find_cycles_by_field_type, has_annotations, HasExtensionClsAttributeName
 
 
 def provide(field: Union[str, List[str]]):
     """Decorator used to provide an extension to the Task class 
     by setting an attribute on the class matching field
 
     Parameters
@@ -145,24 +145,23 @@
 
     cycles = find_cycles_by_field_type(serializeable_fields)
 
     if cycles:
         raise Exception(f"Found cycles in the extension dependencies: {cycles}")
 
     # Get the code of the task
-    code = __get_code(task)
+    code = get_code(task)
 
     # Loop through all the replacements and check if any of them match the type of an injected field
     for old_path, new_path in replacements:
         for field in extension_fields:
             field_type = field.field_type
             if field_type.__module__ == old_path:
                 # Replace the import statement with the new path
-                code = code.replace(f"from {field_type.__module__} import {field_type.__qualname__}",
-                                    f"from {new_path} import {field_type.__qualname__}")
+                code = code.replace(f"from {field_type.__module__}", f"from {new_path}")
 
     return code
 
 def replace_extensions_imports(task: ExtensionTask, extensions_dir: str = 'extensions') -> str:
     """
     Replaces all extensions import statements to the format of <extensions_dir>.<extension_name>
 
@@ -220,15 +219,15 @@
     """
 
 
     # Get a list of all the injected fields in the code
     injected_fields = get_extension_fields(task)
 
     # Get the code of the task
-    code = __get_code(task)
+    code = get_code(task)
 
     # Loop through all the replacements and check if any of them match the type of an injected field
     for field in injected_fields:
         field_type = field.field_type
 
         # Replace the import statement with the new path
         code = code.replace(f"from {field_type.__module__} import {field_type.__qualname__}",
```

### Comparing `switch_api-0.3.3/switch_api/extensions/field_meta.py` & `switch_api-0.4.5/switch_api/extensions/field_meta.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/extensions/helpers.py` & `switch_api-0.4.5/switch_api/extensions/helpers.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 from typing import List
 
 HasExtensionClsAttributeName = '__has_sw_extension_support__'
 """The name of the attribute that is added to a class that has extensions."""
 
-def __get_code(cls):
+def get_code(cls):
     """
     Get the code used to create the class.
 
     (Code was taken from sw.pipeline.Automation._get_task_code function)
     
     Parameters
     ----------
@@ -21,16 +21,15 @@
         The code used to create the `task`
 
     """
     task_type = type(cls)
     task_code = ''
     parent_module = inspect.getmodule(task_type)
     for codeLine in inspect.getsource(parent_module).split('\n'):
-        if codeLine.startswith('import ') or codeLine.startswith('from '):
-            task_code += codeLine + '\n'
+        task_code += codeLine + '\n'
 
     task_code += '\n'
     task_code += inspect.getsource(task_type)
     task_code += ''
     task_code += 'task = ' + task_type.__name__ + '()'
 
     return task_code
```

### Comparing `switch_api-0.3.3/switch_api/extensions/pipeline.py` & `switch_api-0.4.5/switch_api/extensions/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/initialize.py` & `switch_api-0.4.5/switch_api/initialize.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/integration/__init__.py` & `switch_api-0.4.5/switch_api/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/integration/_utils.py` & `switch_api-0.4.5/switch_api/integration/_utils.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/integration/helpers.py` & `switch_api-0.4.5/switch_api/integration/helpers.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/integration/integration.py` & `switch_api-0.4.5/switch_api/integration/integration.py`

 * *Files 0% similar despite different names*

```diff
@@ -441,19 +441,19 @@
                         'SensorUnitOfMeasure', 'EquipmentClass', 'EquipmentLabel']
     proposed_columns = data_frame.columns.tolist()
 
     if not set(required_columns).issubset(data_frame.columns):
         logger.exception('Missing required column(s): %s', set(required_columns).difference(proposed_columns))
         return 'Integration.upsert_device_sensors(): data_frame must contain the following columns: ' + ', '.join(
             required_columns)
-    
+   
     if 'InstallationCode' not in data_frame.columns and 'InstallationId' not in data_frame.columns:
         logger.exception('Must contain InstallationCode or InstallationId')
         return 'Integration.upsert_device_sensors(): data_frame must contain either InstallationCode or InstallationId columns'
-    
+   
     if tag_columns is not None and not set(tag_columns).issubset(data_frame.columns):
         logger.exception('Missing expected tag column(s): %s', set(tag_columns).difference(proposed_columns))
         return 'Integration.upsert_device_sensors(): data_frame expected to contain the following tag column(s): ' + \
                ', '.join(tag_columns)
     elif tag_columns is None:
         tag_columns = []
 
@@ -478,29 +478,34 @@
                 j_row = row[tag_columns].to_json()
                 return str(j_row)
             else:
                 j_row = row[metadata_columns].to_json()
                 return str(j_row)
 
         data_frame['Slices'] = data_frame.apply(update_values, args="A", axis=1)
-        #data_frame['TagsJson'] = data_frame.apply(update_values, args="B", axis=1)
-        #data_frame['MetadataJson'] = data_frame.apply(update_values, args="C", axis=1)
+       
+        if tag_columns is not None:
+            data_frame['TagsJson'] = data_frame.apply(update_values, args="B", axis=1)
+
+        if metadata_columns is not None:
+            data_frame['MetadataJson'] = data_frame.apply(update_values, args="C", axis=1)
+
         data_frame = data_frame.drop(columns=slice_columns)
         slices_data_frame = data_frame[['DeviceCode', 'Slices']]
 
     headers = api_inputs.api_headers.integration
 
     url = f"{api_inputs.api_projects_endpoint}/{api_inputs.api_project_id}/devices/upsert-ingestion"
-    
+   
     def group_data_frame(df):
         if 'InstallationCode' in data_frame.columns:
             return df.groupby(['InstallationCode', 'DeviceCode'])
         else:
             return df.groupby(['InstallationId', 'DeviceCode'])
-    
+   
     data_frame_grpd = group_data_frame(data_frame)
 
 
     chunk_list = []
     for name, group in data_frame_grpd:
         logger.info("Sending request: POST %s", url)
         logger.info('Upserting data for InstallationCode = %s and DeviceCode = %s', str(name[0]), str(name[1]))
```

### Comparing `switch_api-0.3.3/switch_api/pipeline/__init__.py` & `switch_api-0.4.5/switch_api/pipeline/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/pipeline/automation.py` & `switch_api-0.4.5/switch_api/pipeline/automation.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/pipeline/definitions.py` & `switch_api-0.4.5/switch_api/pipeline/definitions.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/pipeline/pipeline.py` & `switch_api-0.4.5/switch_api/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/platform_insights/__init__.py` & `switch_api-0.4.5/switch_api/platform_insights/__init__.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api/platform_insights/platform_insights.py` & `switch_api-0.4.5/switch_api/platform_insights/platform_insights.py`

 * *Files identical despite different names*

### Comparing `switch_api-0.3.3/switch_api.egg-info/PKG-INFO` & `switch_api-0.4.5/HISTORY.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,56 @@
-Metadata-Version: 2.1
-Name: switch-api
-Version: 0.3.3
-Summary: A complete package for data ingestion into the Switch Automation Platform.
-Home-page: UNKNOWN
-Author: Switch Automation Pty Ltd.
-License: MIT License
-Platform: UNKNOWN
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Intended Audience :: Other Audience
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Natural Language :: English
-Requires-Python: >=3.8.*
-Description-Content-Type: text/markdown
-License-File: LICENCE
-License-File: AUTHORS.rst
-
-# Switch Automation library for Python
-This is a package for data ingestion into the Switch Automation software platform. 
-
-You can find out more about the platform on [Switch Automation](https://www.switchautomation.com)
-
-## Getting started
-
-### Prerequisites
-* Python 3.8 or later is required to use this package. 
-* You must have a [Switch Automation user account](https://www.switchautomation.com/our-solution/) to use this package. 
+# History
+
+## 0.4.5
 
-### Install the package
-Install the Switch Automation library for Python with [pip](https://pypi.org/project/pip/):
+### Added
+- Email Sender Module
+  - Send emails to active users within a Portfolio in Switch Automation Platform
+  - Limitations:
+    - Emails cannot be sent to users outside of the Portfolio including other users within the platform
+    - Maximum of five attachments per email
+    - Each attachment has a maximum size of 5mb
+  - See function code documentation and usage example below
+- New `generate_filepath` method to provide a filepath where files can be stored
+  - Works well with the attachment feature of the Email Sender Module. Store files in the generated filepath of this method and pass into email attachments
+  - See function code documentation and usage example below
 
-```bash
-pip install switch_api
+### Email Sender Usage
+```python
+import switch_api as sw
+
+sw.email.send_email(
+    api_inputs=api_inputs,
+    subject='',
+    body='',
+    to_recipients=[],
+    cc_recipients=[], # Optional
+    bcc_recipients=[], # Optional
+    attachments=['/file/path/to/attachment.csv'], # Optional
+    conversation_id='' # Optional
+)
 ```
 
-# History
+### generate_filepath Usage
+```python
+import switch_api as sw
+
+generated_attachment_filepath = sw.generate_filepath(api_inputs=api_inputs, filename='generated_attachment.txt')
+
+# Example of where it could be used
+sw.email.send_email(
+    ...
+    attachments=[generated_attachment_filepath]
+    ...
+)
+```
+
+
+### Fixed
+- Issue where `upsert_device_sensors_ext` method was not posting metadata and tag_columns to API
 
 ## 0.3.3
 
 ### Added
 - New `upsert_device_sensors_ext` method to the `integration` module.
   - Compared to existing `upsert_device_sensors` following are supported:
     - Installation Code or Installation Id may be provided
@@ -740,9 +750,7 @@
 - `kql`
 
 Removed the `name_as_filename` and `treat_as_timeseries` parameter from the following functions:
 
 - `switch.integration.replace_data()`
 - `switch.integration.append_data()`
 - `switch.integration.upload_data()`
-
-
```

### Comparing `switch_api-0.3.3/switch_api.egg-info/SOURCES.txt` & `switch_api-0.4.5/switch_api.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -25,14 +25,16 @@
 switch_api/_utils/_utils.py
 switch_api/analytics/__init__.py
 switch_api/analytics/analytics.py
 switch_api/cache/__init__.py
 switch_api/cache/cache.py
 switch_api/dataset/__init__.py
 switch_api/dataset/dataset.py
+switch_api/email/__init__.py
+switch_api/email/email_sender.py
 switch_api/error_handlers/__init__.py
 switch_api/error_handlers/error_handlers.py
 switch_api/extensions/__init__.py
 switch_api/extensions/extensions.py
 switch_api/extensions/field_meta.py
 switch_api/extensions/helpers.py
 switch_api/extensions/pipeline.py
```

