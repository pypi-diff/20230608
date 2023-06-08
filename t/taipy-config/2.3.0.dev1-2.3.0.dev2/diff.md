# Comparing `tmp/taipy-config-2.3.0.dev1.tar.gz` & `tmp/taipy-config-2.3.0.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taipy-config-2.3.0.dev1.tar", last modified: Mon Jun  5 15:43:13 2023, max compression
+gzip compressed data, was "taipy-config-2.3.0.dev2.tar", last modified: Thu Jun  8 19:22:56 2023, max compression
```

## Comparing `taipy-config-2.3.0.dev1.tar` & `taipy-config-2.3.0.dev2.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/
--rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.339733 taipy-config-2.3.0.dev1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/config/
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.343733 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_comparator_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_config_comparator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.347733 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_base_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_json_serializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_toml_serializer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.347733 taipy-config-2.3.0.dev1/src/taipy/config/checker/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.347733 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_auth_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_global_config_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/issue.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/checker/issue_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/config/common/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_classproperty.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_config_blocker.py
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_repr_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_template_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/_validate_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/frequency.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/common/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)    10599 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    35422 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/config.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/config/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/config/global_app/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/global_app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6993 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/global_app/global_app_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/section.py
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/unique_section.py
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/version.json
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/config/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.351733 taipy-config-2.3.0.dev1/src/taipy/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-05 15:42:57.000000 taipy-config-2.3.0.dev1/src/taipy/logger/_taipy_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 15:43:13.355733 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 15:43:05.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 15:43:13.000000 taipy-config-2.3.0.dev1/src/taipy_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11353 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2324 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/taipy/
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/taipy/_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.254503 taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      607 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3261 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7439 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_comparator_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7781 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_config_comparator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7277 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_base_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_json_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_toml_serializer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/checker/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_auth_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_global_config_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/issue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/checker/issue_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_classproperty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_config_blocker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_repr_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5757 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_template_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/_validate_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/frequency.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/common/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10597 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35445 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/config.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.258504 taipy-config-2.3.0.dev2/src/taipy/config/global_app/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/global_app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7350 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/global_app/global_app_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/section.py
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/unique_section.py
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/version.json
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/config/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/src/taipy/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1590 2023-06-08 19:22:42.000000 taipy-config-2.3.0.dev2/src/taipy/logger/_taipy_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 19:22:56.262503 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3249 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 19:22:49.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-08 19:22:56.000000 taipy-config-2.3.0.dev2/src/taipy_config.egg-info/top_level.txt
```

### Comparing `taipy-config-2.3.0.dev1/LICENSE` & `taipy-config-2.3.0.dev2/LICENSE`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/PKG-INFO` & `taipy-config-2.3.0.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.3.0.dev1/README.md` & `taipy-config-2.3.0.dev2/README.md`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/setup.py` & `taipy-config-2.3.0.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -47,14 +47,15 @@
             get_latest_job,
             get_parents,
             get_pipelines,
             get_primary,
             get_primary_scenarios,
             get_scenarios,
             get_tasks,
+            is_deletable,
             set,
             set_primary,
             submit,
             subscribe_pipeline,
             subscribe_scenario,
             tag,
             unsubscribe_pipeline,
@@ -63,14 +64,19 @@
         )
         from taipy.core.task.task import Task
         from taipy.core.task.task_id import TaskId
 
     if find_spec("taipy.gui"):
         from taipy.gui import Gui
 
+        if find_spec("taipy.gui_core"):
+            from taipy.gui_core.GuiCoreLib import GuiCore
+
+            Gui.add_library(GuiCore())
+
         if find_spec("taipy.enterprise") and find_spec("taipy.enterprise.gui"):
             from taipy.enterprise.gui import _init_gui_enterprise
 
             _init_gui_enterprise(Gui)
 
     if find_spec("taipy.rest"):
         from taipy.rest import Rest
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy/_cli/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/_cli/_base_cli/_cli.py` & `taipy-config-2.3.0.dev2/src/taipy/_cli/_base_cli/_cli.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_config.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -21,34 +21,42 @@
     DEFAULT_KEY = "default"
 
     def __init__(self):
         self._sections: Dict[str, Dict[str, Section]] = {}
         self._unique_sections: Dict[str, UniqueSection] = {}
         self._global_config: GlobalAppConfig = GlobalAppConfig()
 
+    def _clean(self):
+        self._global_config._clean()
+        for unique_section in self._unique_sections.values():
+            unique_section._clean()
+        for sections in self._sections.values():
+            for section in sections.values():
+                section._clean()
+
     @classmethod
     def _default_config(cls):
         config = _Config()
         config._global_config = GlobalAppConfig.default_config()
         return config
 
     def _update(self, other_config):
         self._global_config._update(other_config._global_config._to_dict())
         if other_config._unique_sections:
             for section_name, other_section in other_config._unique_sections.items():
                 if section := self._unique_sections.get(section_name, None):
                     section._update(other_section._to_dict())
                 else:
-                    self._unique_sections[section_name] = other_config._unique_sections[section_name]
+                    self._unique_sections[section_name] = copy(other_config._unique_sections[section_name])
         if other_config._sections:
             for section_name, other_non_unique_sections in other_config._sections.items():
                 if non_unique_sections := self._sections.get(section_name, None):
                     self.__update_sections(non_unique_sections, other_non_unique_sections, None)
                 else:
-                    self._sections[section_name] = other_non_unique_sections
+                    self._sections[section_name] = {k: copy(v) for k, v in other_non_unique_sections.items()}
 
     def __update_sections(self, entity_config, other_entity_configs, _class):
         if self.DEFAULT_KEY in other_entity_configs:
             if self.DEFAULT_KEY in entity_config:
                 entity_config[self.DEFAULT_KEY]._update(other_entity_configs[self.DEFAULT_KEY]._to_dict())
             else:
                 entity_config[self.DEFAULT_KEY] = other_entity_configs[self.DEFAULT_KEY]
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_comparator_result.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_comparator_result.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_config_comparator/_config_comparator.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_config_comparator/_config_comparator.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_base_serializer.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_base_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_json_serializer.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_json_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/_serializer/_toml_serializer.py` & `taipy-config-2.3.0.dev2/src/taipy/config/_serializer/_toml_serializer.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checker.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_auth_config_checker.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_auth_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_config_checker.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/_checkers/_global_config_checker.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/_checkers/_global_config_checker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/issue.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/issue.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/checker/issue_collector.py` & `taipy-config-2.3.0.dev2/src/taipy/config/checker/issue_collector.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/_classproperty.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/_classproperty.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/_config_blocker.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/_config_blocker.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/_repr_enum.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/_repr_enum.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/_template_handler.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/_template_handler.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/_validate_id.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/_validate_id.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/frequency.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/frequency.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/common/scope.py` & `taipy-config-2.3.0.dev2/src/taipy/config/common/scope.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/config.py` & `taipy-config-2.3.0.dev2/src/taipy/config/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,17 +29,17 @@
 class Config:
     """Configuration singleton."""
 
     _ENVIRONMENT_VARIABLE_NAME_WITH_CONFIG_PATH = "TAIPY_CONFIG_PATH"
     __logger = _TaipyLogger._get_logger()
     _default_config = _Config._default_config()
     _python_config = _Config()
-    _file_config = None
-    _env_file_config = None
-    _applied_config = _Config._default_config()
+    _file_config = _Config()
+    _env_file_config = _Config()
+    _applied_config = _Config()
     _collector = IssueCollector()
     _serializer = _TomlSerializer()
     __json_serializer = _JsonSerializer()
     _comparator: _ConfigComparator = _ConfigComparator()
 
     @_Classproperty
     def unique_sections(cls) -> Dict[str, UniqueSection]:
@@ -55,15 +55,17 @@
     def global_config(cls) -> GlobalAppConfig:
         """Return configuration values related to the global application as a `GlobalAppConfig^`."""
         return cls._applied_config._global_config
 
     @classmethod
     @_ConfigBlocker._check()
     def load(cls, filename):
-        """Load a configuration file to replace the current python config and trigger the Config compilation.
+        """Load a configuration file.
+
+        The current Python configuration is replaced and the Config compilation is triggered.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
         cls.__logger.info(f"Loading configuration. Filename: '{filename}'")
         cls._python_config = cls._serializer._read(filename)
         cls._compile_configs()
@@ -71,37 +73,37 @@
 
     @classmethod
     def export(cls, filename):
         """Export a configuration.
 
         The export is done in a toml file.
 
-        The exported configuration is taken from the python code configuration.
+        The exported configuration is taken from the Python code configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
-            If _filename_ already exists, it is overwritten.
+            If *filename* already exists, it is overwritten.
         """
         cls._serializer._write(cls._python_config, filename)
 
     @classmethod
     def backup(cls, filename):
         """Backup a configuration.
 
         The backup is done in a toml file.
 
         The backed up configuration is a compilation from the three possible methods to configure
-        the application: the python code configuration, the file configuration and the environment
+        the application: the Python code configuration, the file configuration and the environment
         configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
-            If _filename_ already exists, it is overwritten.
+            If *filename* already exists, it is overwritten.
         """
         cls._serializer._write(cls._applied_config, filename)
 
     @classmethod
     @_ConfigBlocker._check()
     def restore(cls, filename):
         """Restore a configuration file and replace the current applied configuration.
@@ -222,15 +224,15 @@
             cls.__logger.info(f"Loading configuration provided by environment variable. Filename: '{config_filename}'")
             cls._env_file_config = cls._serializer._read(config_filename)
             cls.__logger.info(f"Configuration '{config_filename}' successfully loaded.")
 
     @classmethod
     def _compile_configs(cls):
         Config._override_env_file()
-        cls._applied_config = _Config._default_config()
+        cls._applied_config._clean()
         if cls._default_config:
             cls._applied_config._update(cls._default_config)
         if cls._python_config:
             cls._applied_config._update(cls._python_config)
         if cls._file_config:
             cls._applied_config._update(cls._file_config)
         if cls._env_file_config:
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/config.pyi` & `taipy-config-2.3.0.dev2/src/taipy/config/config.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -37,48 +37,50 @@
     @_Classproperty
     def global_config(cls) -> GlobalAppConfig:
         """Return configuration values related to the global application as a `GlobalAppConfig^`."""
 
     @classmethod
     @_ConfigBlocker._check()
     def load(cls, filename):
-        """Load a configuration file to replace the current python config and trigger the Config compilation.
+        """Load a configuration file.
+
+        The current Python configuration is replaced and the Config compilation is triggered.
 
         Parameters:
             filename (Union[str, Path]): The path of the toml configuration file to load.
         """
 
     @classmethod
     def export(cls, filename):
         """Export a configuration.
 
         The export is done in a toml file.
 
-        The exported configuration is taken from the python code configuration.
+        The exported configuration is taken from the Python code configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
-            If _filename_ already exists, it is overwritten.
+            If *filename* already exists, it is overwritten.
         """
 
     @classmethod
     def backup(cls, filename):
         """Backup a configuration.
 
         The backup is done in a toml file.
 
         The backed up configuration is a compilation from the three possible methods to configure
-        the application: the python code configuration, the file configuration and the environment
+        the application: the Python code configuration, the file configuration and the environment
         configuration.
 
         Parameters:
             filename (Union[str, Path]): The path of the file to export.
         Note:
-            If _filename_ already exists, it is overwritten.
+            If *filename* already exists, it is overwritten.
         """
 
     @classmethod
     @_ConfigBlocker._check()
     def restore(cls, filename):
         """Restore a configuration file and replace the current applied configuration.
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/exceptions/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/config/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/exceptions/exceptions.py` & `taipy-config-2.3.0.dev2/src/taipy/config/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/global_app/global_app_config.py` & `taipy-config-2.3.0.dev2/src/taipy/config/global_app/global_app_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,14 +131,21 @@
         config._root_folder = cls._DEFAULT_ROOT_FOLDER
         config._storage_folder = cls._DEFAULT_STORAGE_FOLDER
         config._clean_entities_enabled = cls._CLEAN_ENTITIES_ENABLED_TEMPLATE
         config._repository_type = cls._DEFAULT_REPOSITORY_TYPE
         config._repository_properties = cls._DEFAULT_REPOSITORY_PROPERTIES.copy()
         return config
 
+    def _clean(self):
+        self._root_folder = self._DEFAULT_ROOT_FOLDER
+        self._storage_folder = self._DEFAULT_STORAGE_FOLDER
+        self._clean_entities_enabled = self._CLEAN_ENTITIES_ENABLED_TEMPLATE
+        self._repository_type = self._DEFAULT_REPOSITORY_TYPE
+        self._repository_properties = self._DEFAULT_REPOSITORY_PROPERTIES.copy()
+
     def _to_dict(self):
         as_dict = {}
         if self._root_folder:
             as_dict[self._ROOT_FOLDER_KEY] = self._root_folder
         if self._storage_folder:
             as_dict[self._STORAGE_FOLDER_KEY] = self._storage_folder
         if self._clean_entities_enabled is not None:
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/section.py` & `taipy-config-2.3.0.dev2/src/taipy/config/section.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 
     @property
     @abstractmethod
     def name(self):
         raise NotImplementedError
 
     @abstractmethod
+    def _clean(self):
+        raise NotImplementedError
+
+    @abstractmethod
     def _to_dict(self):
         raise NotImplementedError
 
     @classmethod
     @abstractmethod
     def _from_dict(cls, config_as_dict: Dict[str, Any], id, config):
         raise NotImplementedError
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy/config/unique_section.py` & `taipy-config-2.3.0.dev2/src/taipy/config/unique_section.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/logger/__init__.py` & `taipy-config-2.3.0.dev2/src/taipy/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy/logger/_taipy_logger.py` & `taipy-config-2.3.0.dev2/src/taipy/logger/_taipy_logger.py`

 * *Files identical despite different names*

### Comparing `taipy-config-2.3.0.dev1/src/taipy_config.egg-info/PKG-INFO` & `taipy-config-2.3.0.dev2/src/taipy_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taipy-config
-Version: 2.3.0.dev1
+Version: 2.3.0.dev2
 Summary: A Taipy package dedicated to easily configure a Taipy application.
 Home-page: https://github.com/avaiga/taipy-config
 Author: Avaiga
 Author-email: dev@taipy.io
 License: Apache License 2.0
 Keywords: taipy-config
 Classifier: Intended Audience :: Developers
```

### Comparing `taipy-config-2.3.0.dev1/src/taipy_config.egg-info/SOURCES.txt` & `taipy-config-2.3.0.dev2/src/taipy_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

