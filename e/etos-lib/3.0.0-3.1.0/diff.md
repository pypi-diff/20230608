# Comparing `tmp/etos_lib-3.0.0.tar.gz` & `tmp/etos_lib-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etos_lib-3.0.0.tar", last modified: Thu Jun  1 07:09:10 2023, max compression
+gzip compressed data, was "etos_lib-3.1.0.tar", last modified: Thu Jun  8 05:46:27 2023, max compression
```

## Comparing `etos_lib-3.0.0.tar` & `etos_lib-3.1.0.tar`

### file list

```diff
@@ -1,69 +1,67 @@
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-03-09 08:23:58.000000 etos_lib-3.0.0/.coveragerc
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/.github/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/.github/workflows/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-03-09 08:23:58.000000 etos_lib-3.0.0/.github/workflows/main.yml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      542 2023-06-01 07:09:02.000000 etos_lib-3.0.0/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-03-09 08:23:58.000000 etos_lib-3.0.0/AUTHORS.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-03-09 08:23:58.000000 etos_lib-3.0.0/CODEOWNERS
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-03-09 08:23:58.000000 etos_lib-3.0.0/LICENSE.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:09:10.410018 etos_lib-3.0.0/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-03-09 08:23:58.000000 etos_lib-3.0.0/README.rst
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/docs/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/Makefile
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/docs/_static/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/_static/.gitignore
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/authors.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/changelog.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-05-31 11:37:56.000000 etos_lib-3.0.0/docs/conf.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/index.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/license.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/readme.rst
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-03-09 08:23:58.000000 etos_lib-3.0.0/docs/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      177 2023-06-01 07:09:02.000000 etos_lib-3.0.0/requirements.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1473 2023-06-01 07:09:10.414018 etos_lib-3.0.0/setup.cfg
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-03-09 08:23:58.000000 etos_lib-3.0.0/setup.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5386 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/etos.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/graphql/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/graphql/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/graphql/query_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/kubernetes/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/kubernetes/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3355 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/kubernetes/base.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3292 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/kubernetes/jobs.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/lib/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2152 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/auth.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4814 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/lib/config.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/database.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     5143 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/lib/debug.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/lib/events.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/exceptions.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-05-31 11:37:56.000000 etos_lib-3.0.0/src/etos_lib/lib/feature_flags.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/http.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/monitor.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2632 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/secrets.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/lib/utils.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib/logging/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/logging/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-05-26 11:19:01.000000 etos_lib-3.0.0/src/etos_lib/logging/default_config.yaml
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/logging/filter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-03-09 08:23:58.000000 etos_lib-3.0.0/src/etos_lib/logging/formatter.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1967 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/logging/log_publisher.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     6817 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/logging/logger.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     2331 2023-06-01 07:09:02.000000 etos_lib-3.0.0/src/etos_lib/logging/rabbitmq_handler.py
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/src/etos_lib.egg-info/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/PKG-INFO
--rw-r--r--   0 tobiaspn (21118) axusers    (500)     1369 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/SOURCES.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/dependency_links.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-05-26 11:39:50.000000 etos_lib-3.0.0/src/etos_lib.egg-info/not-zip-safe
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      185 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/requires.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-01 07:09:10.000000 etos_lib-3.0.0/src/etos_lib.egg-info/top_level.txt
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-03-09 08:23:58.000000 etos_lib-3.0.0/test-requirements.txt
-drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-01 07:09:10.410018 etos_lib-3.0.0/tests/
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-03-09 08:23:58.000000 etos_lib-3.0.0/tests/__init__.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-03-09 08:23:58.000000 etos_lib-3.0.0/tests/conftest.py
--rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-03-09 08:23:58.000000 etos_lib-3.0.0/tox.ini
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.840068 etos_lib-3.1.0/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      591 2023-06-08 05:45:47.000000 etos_lib-3.1.0/.coveragerc
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/.github/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/.github/workflows/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      850 2023-06-08 05:45:47.000000 etos_lib-3.1.0/.github/workflows/main.yml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      542 2023-06-08 05:45:47.000000 etos_lib-3.1.0/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      174 2023-06-08 05:45:47.000000 etos_lib-3.1.0/AUTHORS.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       37 2023-06-08 05:45:47.000000 etos_lib-3.1.0/CODEOWNERS
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10850 2023-06-08 05:45:47.000000 etos_lib-3.1.0/LICENSE.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-08 05:46:27.840068 etos_lib-3.1.0/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      721 2023-06-08 05:45:47.000000 etos_lib-3.1.0/README.rst
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/docs/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     7610 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/Makefile
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/docs/_static/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       18 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/_static/.gitignore
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       41 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/authors.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       43 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/changelog.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     9175 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/conf.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      457 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/index.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       74 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/license.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       39 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/readme.rst
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       59 2023-06-08 05:45:47.000000 etos_lib-3.1.0/docs/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-06-08 05:45:47.000000 etos_lib-3.1.0/requirements.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1413 2023-06-08 05:46:27.840068 etos_lib-3.1.0/setup.cfg
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      552 2023-06-08 05:45:47.000000 etos_lib-3.1.0/setup.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1093 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4915 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/etos.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/graphql/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      702 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/graphql/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2692 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/graphql/query_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/kubernetes/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      727 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/kubernetes/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3103 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/kubernetes/base.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3288 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/kubernetes/jobs.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib/lib/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      701 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4814 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/config.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     3911 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/database.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     5164 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/debug.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    15885 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/events.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2480 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/exceptions.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      810 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/feature_flags.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4331 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/http.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4605 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/monitor.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)    10944 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/lib/utils.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.840068 etos_lib-3.1.0/src/etos_lib/logging/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      693 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)       66 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/default_config.yaml
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2223 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/filter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     4094 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/formatter.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1967 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/log_publisher.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     6829 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/logger.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     2331 2023-06-08 05:45:47.000000 etos_lib-3.1.0/src/etos_lib/logging/rabbitmq_handler.py
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.836068 etos_lib-3.1.0/src/etos_lib.egg-info/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1334 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/PKG-INFO
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)     1316 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        1 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/not-zip-safe
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      128 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/requires.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)        9 2023-06-08 05:46:27.000000 etos_lib-3.1.0/src/etos_lib.egg-info/top_level.txt
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      241 2023-06-08 05:45:47.000000 etos_lib-3.1.0/test-requirements.txt
+drwxr-xr-x   0 tobiaspn (21118) axusers    (500)        0 2023-06-08 05:46:27.840068 etos_lib-3.1.0/tests/
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      692 2023-06-08 05:45:47.000000 etos_lib-3.1.0/tests/__init__.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      196 2023-06-08 05:45:47.000000 etos_lib-3.1.0/tests/conftest.py
+-rw-r--r--   0 tobiaspn (21118) axusers    (500)      410 2023-06-08 05:45:47.000000 etos_lib-3.1.0/tox.ini
```

### Comparing `etos_lib-3.0.0/.coveragerc` & `etos_lib-3.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/.github/workflows/main.yml` & `etos_lib-3.1.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/.gitignore` & `etos_lib-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/LICENSE.txt` & `etos_lib-3.1.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/PKG-INFO` & `etos_lib-3.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos_lib
-Version: 3.0.0
+Version: 3.1.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-3.0.0/README.rst` & `etos_lib-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/docs/Makefile` & `etos_lib-3.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/docs/conf.py` & `etos_lib-3.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/setup.cfg` & `etos_lib-3.1.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -19,23 +19,20 @@
 zip_safe = False
 packages = find:
 include_package_data = True
 package_dir = 
 	=src
 setup_requires = pyscaffold>=3.2a0,<3.3a0
 install_requires = 
-	graphql-core==2.2.1
-	gql==0.1.0
-	cryptography==3.1
-	redis==3.5.3
-	eiffellib[rabbitmq]==2.4.1
-	pydantic==1.6
-	requests==2.24.0
-	kubernetes==7.0.1
-	python-box==5.2.0
+	gql[requests]~=3.4
+	redis~=4.5
+	eiffellib[rabbitmq]~=2.4
+	requests~=2.31
+	kubernetes~=26.1
+	pyyaml~=6.0
 python_requires = >=3.4
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
```

### Comparing `etos_lib-3.0.0/setup.py` & `etos_lib-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/__init__.py` & `etos_lib-3.1.0/src/etos_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/etos.py` & `etos_lib-3.1.0/src/etos_lib/etos.py`

 * *Files 9% similar despite different names*

```diff
@@ -12,47 +12,43 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """ETOS Library module."""
 from eiffellib.subscribers import RabbitMQSubscriber
 from eiffellib.publishers import RabbitMQPublisher
-from .lib.auth import Auth
 from .lib.config import Config
 from .lib.events import Events
 from .lib.monitor import Monitor
 from .lib.utils import Utils
 from .lib.http import Http
 from .lib.debug import Debug
 from .lib.feature_flags import FeatureFlags
 from .lib.database import Database
-from .lib.secrets import Secrets
 from .lib.exceptions import (
     PublisherConfigurationMissing,
     SubscriberConfigurationMissing,
     PublisherNotStarted,
 )
 from .graphql.query_handler import GraphQLQueryHandler
 
 
 class ETOS:  # pylint: disable=too-many-instance-attributes
     """ETOS Library."""
 
     publisher = None
     subscriber = None
-    __auth = None
     __config = None
     __events = None
     __monitor = None
     __utils = None
     __graphql = None
     __http = None
     __debug = None
     __feature_flags = None
-    __secrets = None
     __database = None
 
     def __init__(self, service_name, host, name, domain_id=None):
         """Initialize source and service name."""
         source = {"name": name, "host": host}
         if domain_id is not None:
             source["domainId"] = domain_id
@@ -111,21 +107,14 @@
         if self.__events is None:
             if self.publisher is None and not self.debug.disable_sending_events:
                 raise PublisherNotStarted
             self.__events = Events(self.publisher)
         return self.__events
 
     @property
-    def auth(self):
-        """Entry for ETOS Library auth service."""
-        if self.__auth is None:
-            self.__auth = Auth()
-        return self.__auth
-
-    @property
     def config(self):
         """Entry for ETOS Library config service."""
         if self.__config is None:
             self.__config = Config()
         return self.__config
 
     @property
@@ -151,14 +140,7 @@
 
     @property
     def database(self):
         """Entry to ETOS Library database service."""
         if self.__database is None:
             self.__database = Database()
         return self.__database
-
-    @property
-    def secrets(self):
-        """Entry to ETOS Library secret service."""
-        if self.__secrets is None:
-            self.__secrets = Secrets()
-        return self.__secrets
```

### Comparing `etos_lib-3.0.0/src/etos_lib/graphql/__init__.py` & `etos_lib-3.1.0/src/etos_lib/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/graphql/query_handler.py` & `etos_lib-3.1.0/src/etos_lib/graphql/query_handler.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/kubernetes/__init__.py` & `etos_lib-3.1.0/src/etos_lib/kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/kubernetes/base.py` & `etos_lib-3.1.0/src/etos_lib/kubernetes/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,14 @@
 
 class Kubernetes:
     """Base kubernetes library."""
 
     __batch = None
     __core = None
     __apps = None
-    __extensions = None
 
     def __init__(
         self, namespace=os.getenv("ETOS_NAMESPACE"), context=None, in_cluster=True
     ):
         """Initialize kubernetes library and load kubernetes configuration.
 
         :param namespace: Which namespace to operate in.
@@ -88,19 +87,12 @@
     def batch_v1(self):
         """BatchV1Api for Kubernetes."""
         if self.__batch is None:
             self.__batch = client.BatchV1Api()
         return self.__batch
 
     @property
-    def extensions(self):
-        """Create a ExtensionsV1beta1Api endpoint."""
-        if self.__extensions is None:
-            self.__extensions = client.ExtensionsV1beta1Api()
-        return self.__extensions
-
-    @property
     def core(self):
         """Create a CoreV1Api endpoint."""
         if self.__core is None:
             self.__core = client.CoreV1Api()
         return self.__core
```

### Comparing `etos_lib-3.0.0/src/etos_lib/kubernetes/jobs.py` & `etos_lib-3.1.0/src/etos_lib/kubernetes/jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,8 +86,8 @@
 
     def delete_job(self, job_name):
         """Delete a kubernetes job.
 
         :param job_name: Name of job to remove.
         :type job_name: str
         """
-        self.batch_v1.delete_namespaced_job(job_name, self.namespace, {})
+        self.batch_v1.delete_namespaced_job(job_name, self.namespace)
```

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/__init__.py` & `etos_lib-3.1.0/src/etos_lib/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/auth.py` & `etos_lib-3.1.0/src/etos_lib/logging/log_publisher.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,54 @@
-# Copyright 2020 Axis Communications AB.
+# Copyright Axis Communications AB.
 #
 # For a full list of individual contributors, please see the commit history.
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS Library authentication handler.
+"""ETOS rabbitmq log publisher."""
+import time
+import json
+import pika
 
-DEPRECATED: Use kubernetes secrets instead!
-"""
-import configparser
-from cryptography.fernet import Fernet
+from eiffellib.publishers import RabbitMQPublisher
 
 
-class Auth:
-    """Authentication helper for ETOS.
+class RabbitMQLogPublisher(RabbitMQPublisher):
+    """A RabbitMQ publisher that can send JSON strings instead of Eiffel events."""
 
-    Example:
-        auth = Auth()
-        auth.load_password_file("password.secret")
-        username, password = auth.credentials("my_service")
-    """
+    def send_event(self, event, block=True, routing_key="#"):
+        """Overload the send_event from the eiffellib rabbitmq publisher to send strings.
 
-    config = None
-    key = None
-
-    def load_password_file(self, _file):
-        """Load a password file into memory.
-
-        :param _file: Path to file to load.
-        :type _file: str
-        """
-        self.config = configparser.ConfigParser()
-        self.config.read(_file)
-        self.key = self.config["global"]["key"]
-
-    def decrypt(self, token):
-        """Decrypt a password hash into a password.
-
-        :param token: Password hash to decrypt.
-        :type token: str
-        :return: Password in clear-text.
-        :rtype: str
-        """
-        cipher_suite = Fernet(self.key)
-        uncipher_text = cipher_suite.decrypt(token.encode("utf-8"))
-        return bytes(uncipher_text).decode("utf-8")
-
-    def credentials(self, service):
-        """Get credentials from a specific service defined in password file.
-
-        :param service: Which service to get credentials for.
-        :type service: str
-        :return: Username and password for service.
-        :rtype: tuple
+        This method differs slightly from its parent in that it takes the routing_key as input.
         """
-        service = self.config[service]
-        return service.get("username"), self.decrypt(service.get("password"))
+        if block:
+            self.wait_start()
+            while self._channel is None or not self._channel.is_open:
+                time.sleep(0.1)
+        properties = pika.BasicProperties(
+            content_type="application/json", delivery_mode=2
+        )
+        if not isinstance(event, str):
+            event = json.dumps(event)
+
+        with self._lock:
+            try:
+                self._channel.basic_publish(
+                    self.exchange,
+                    routing_key,
+                    event,
+                    properties,
+                )
+            except:  # pylint:disable=bare-except
+                self._nacked_deliveries.append(event)
+                return
+            self._delivered += 1
+            self._deliveries[self._delivered] = event
```

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/config.py` & `etos_lib-3.1.0/src/etos_lib/lib/config.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/database.py` & `etos_lib-3.1.0/src/etos_lib/lib/database.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/debug.py` & `etos_lib-3.1.0/src/etos_lib/lib/debug.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,19 +29,14 @@
         maxlen=int(os.getenv("ETOS_PUBLISHED_EVENT_HISTORY_SIZE", "100"))
     )
     __events_received = deque(
         maxlen=int(os.getenv("ETOS_RECEIVED_EVENT_HISTORY_SIZE", "100"))
     )
 
     @property
-    def default_secret_path(self):
-        """Path to k8s secrets."""
-        return os.getenv("ETOS_SECRET_PATH", "/etc/")
-
-    @property
     def default_log_path(self):
         """Log path."""
         path = os.getenv("ETOS_LOG_PATH")
         if path is None:
             path = Path.home().joinpath("logs/log.json")
         else:
             path = Path(path)
@@ -54,14 +49,19 @@
 
     @property
     def disable_sending_events(self):
         """Disable sending eiffel events."""
         return bool(os.getenv("ETOS_DISABLE_SENDING_EVENTS", None))
 
     @property
+    def enable_sending_logs(self):
+        """Disable sending eiffel events."""
+        return bool(os.getenv("ETOS_ENABLE_SENDING_LOGS", None))
+
+    @property
     def disable_receiving_events(self):
         """Disable receiving eiffel events."""
         return bool(os.getenv("ETOS_DISABLE_RECEIVING_EVENTS", None))
 
     @property
     def default_http_timeout(self):
         """Timeout for HTTP requests."""
```

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/events.py` & `etos_lib-3.1.0/src/etos_lib/lib/events.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/exceptions.py` & `etos_lib-3.1.0/src/etos_lib/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/feature_flags.py` & `etos_lib-3.1.0/src/etos_lib/lib/feature_flags.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/http.py` & `etos_lib-3.1.0/src/etos_lib/lib/http.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/monitor.py` & `etos_lib-3.1.0/src/etos_lib/lib/monitor.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/lib/utils.py` & `etos_lib-3.1.0/src/etos_lib/lib/utils.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/logging/__init__.py` & `etos_lib-3.1.0/src/etos_lib/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/logging/filter.py` & `etos_lib-3.1.0/src/etos_lib/logging/filter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/logging/formatter.py` & `etos_lib-3.1.0/src/etos_lib/logging/formatter.py`

 * *Files identical despite different names*

### Comparing `etos_lib-3.0.0/src/etos_lib/logging/log_publisher.py` & `etos_lib-3.1.0/src/etos_lib/logging/rabbitmq_handler.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,46 +9,60 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-"""ETOS rabbitmq log publisher."""
-import time
+"""ETOS rabbitmq handler."""
 import json
-import pika
+import logging
 
-from eiffellib.publishers import RabbitMQPublisher
 
+class RabbitMQHandler(logging.StreamHandler):
+    """A RabbitMQ log handler that sends logs tagged with user_log to RabbitMQ.
 
-class RabbitMQLogPublisher(RabbitMQPublisher):
-    """A RabbitMQ publisher that can send JSON strings instead of Eiffel events."""
+    Example::
 
-    def send_event(self, event, block=True, routing_key="#"):
-        """Overload the send_event from the eiffellib rabbitmq publisher to send strings.
+        import logging
+        from uuid import uuid4
+        from etos_lib.logging.logger import setup_logging, FORMAT_CONFIG
 
-        This method differs slightly from its parent in that it takes the routing_key as input.
+        FORMAT_CONFIG.identifier = str(uuid4())
+        setup_logging("myApp", "1.0.0", "production")
+        logger = logging.getLogger(__name__)
+        logger.info("Hello!", extra={"user_log": True})
+    """
+
+    closing = False
+
+    def __init__(self, rabbitmq):
+        """Initialize."""
+        super().__init__()
+        self.rabbitmq = rabbitmq
+
+    def emit(self, record):
+        """Send user log to RabbitMQ, starting the connection if necessary.
+
+        The record parameter "user_log" must be set to True if a message shall be
+        sent to RabbitMQ.
         """
-        if block:
-            self.wait_start()
-            while self._channel is None or not self._channel.is_open:
-                time.sleep(0.1)
-        properties = pika.BasicProperties(
-            content_type="application/json", delivery_mode=2
-        )
-        if not isinstance(event, str):
-            event = json.dumps(event)
-
-        with self._lock:
-            try:
-                self._channel.basic_publish(
-                    self.exchange,
-                    routing_key,
-                    event,
-                    properties,
-                )
-            except:  # pylint:disable=bare-except
-                self._nacked_deliveries.append(event)
-                return
-            self._delivered += 1
-            self._deliveries[self._delivered] = event
+        if self.closing:
+            return
+
+        try:
+            send = record.user_log
+        except AttributeError:
+            send = False
+
+        msg = self.format(record)
+        try:
+            identifier = record.identifier
+        except AttributeError:
+            identifier = json.loads(msg).get("identifier", "Unknown")
+        # An unknown identifier will never be picked up by user log handler
+        # so it is unnecessary to send it.
+        routing_key = f"{identifier}.log.{record.levelname}"
+        if send and self.rabbitmq.is_alive():
+            if identifier == "Unknown":
+                raise ValueError("Trying to send a user log when identifier is not set")
+            self.rabbitmq.send_event(msg, routing_key=routing_key)
```

### Comparing `etos_lib-3.0.0/src/etos_lib/logging/logger.py` & `etos_lib-3.1.0/src/etos_lib/logging/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 """
 import sys
 import atexit
 from pathlib import Path
 import threading
 import logging
 import logging.config
-from box import Box
+from yaml import load, SafeLoader
 from etos_lib.logging.filter import EtosFilter
 from etos_lib.logging.formatter import EtosLogFormatter
 from etos_lib.logging.rabbitmq_handler import RabbitMQHandler
 from etos_lib.logging.log_publisher import RabbitMQLogPublisher
 from etos_lib.lib.config import Config
 from etos_lib.lib.debug import Debug
 
@@ -61,15 +61,15 @@
             logfile: path/to/log/file
             # Maximum number of files to rotate. Default=10
             max_files: 5
             # Maximum number of bytes in each logfile. Default=1048576/1MB
             max_bytes: 100
 
     :param config: File logging configuration.
-    :type config: :obj:`Box`
+    :type config: dict
     :param log_filter: Logfilter to add to file handler.
     :type log_filter: :obj:`EtosFilter`
     """
     loglevel = getattr(logging, config.get("loglevel", "DEBUG"))
     logfile = Path(config.get("logfile", DEFAULT_LOG_PATH))
     logfile.parent.mkdir(parents=True, exist_ok=True)
 
@@ -98,15 +98,15 @@
             # Format to print logs with.
             # Default: [%(asctime)s][%(identifier)s] %(levelname)s:%(name)s: %(message)s
             logformat: %(message)s
             # Dateformat for %(asctime) format. Default: %Y-%m-%d %H:%M:%S
             dateformat: %Y-%d-%m %H:%M:%S
 
     :param config: Stream logging configuration.
-    :type config: :obj:`Box`
+    :type config: dict
     :param log_filter: Logfilter to add to stream handler.
     :type log_filter: :obj:`EtosFilter`
     """
     loglevel = getattr(logging, config.get("loglevel", "INFO"))
 
     logformat = config.get(
         "logformat", "[%(asctime)s][%(identifier)s] %(levelname)s:%(name)s: %(message)s"
@@ -135,17 +135,17 @@
     logging.getLogger("pika").propagate = False
     logging.getLogger("rabbitmq_publisher").propagate = False
     logging.getLogger("base_rabbitmq").propagate = False
 
     rabbitmq = RabbitMQLogPublisher(
         **Config().etos_rabbitmq_publisher_data(), routing_key=None
     )
-    if not Debug().disable_sending_events:
+    if Debug().enable_sending_logs:
         rabbitmq.start()
-    atexit.register(close_rabbit, rabbitmq)
+        atexit.register(close_rabbit, rabbitmq)
 
     rabbit_handler = RabbitMQHandler(rabbitmq)
     rabbit_handler.setFormatter(EtosLogFormatter())
     rabbit_handler.setLevel(loglevel)
     rabbit_handler.addFilter(log_filter)
 
     root_logger.addHandler(rabbit_handler)
@@ -160,16 +160,16 @@
     :type version: str
     :param environment: Environment in which this application resides.
     :type environment: str
     :param config_file: Filename of logging configuration.
     :type config_file: str
     """
     with open(config_file, encoding="utf-8") as yaml_file:
-        config = Box.from_yaml(yaml_file)
-    logging_config = config.logging
+        config = load(yaml_file, Loader=SafeLoader)
+    logging_config = config["logging"]
 
     log_filter = EtosFilter(application, version, environment, FORMAT_CONFIG)
 
     # Create a default logger which will not propagate messages
     # to the root logger. This logger will create records for all
     # messages, but not print them to stdout. Stdout printing
     # is setup in "setup_stream_logging" if the "stream" key exists
```

### Comparing `etos_lib-3.0.0/src/etos_lib.egg-info/PKG-INFO` & `etos_lib-3.1.0/src/etos_lib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etos-lib
-Version: 3.0.0
+Version: 3.1.0
 Summary: ETOS Library
 Home-page: https://github.com/eiffel-community/etos-library
 Author: Tobias Persson
 Author-email: tobias.persson@axis.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://etos.readthedocs.io/
 Platform: Linux
```

### Comparing `etos_lib-3.0.0/src/etos_lib.egg-info/SOURCES.txt` & `etos_lib-3.1.0/src/etos_lib.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -29,24 +29,22 @@
 src/etos_lib.egg-info/top_level.txt
 src/etos_lib/graphql/__init__.py
 src/etos_lib/graphql/query_handler.py
 src/etos_lib/kubernetes/__init__.py
 src/etos_lib/kubernetes/base.py
 src/etos_lib/kubernetes/jobs.py
 src/etos_lib/lib/__init__.py
-src/etos_lib/lib/auth.py
 src/etos_lib/lib/config.py
 src/etos_lib/lib/database.py
 src/etos_lib/lib/debug.py
 src/etos_lib/lib/events.py
 src/etos_lib/lib/exceptions.py
 src/etos_lib/lib/feature_flags.py
 src/etos_lib/lib/http.py
 src/etos_lib/lib/monitor.py
-src/etos_lib/lib/secrets.py
 src/etos_lib/lib/utils.py
 src/etos_lib/logging/__init__.py
 src/etos_lib/logging/default_config.yaml
 src/etos_lib/logging/filter.py
 src/etos_lib/logging/formatter.py
 src/etos_lib/logging/log_publisher.py
 src/etos_lib/logging/logger.py
```

### Comparing `etos_lib-3.0.0/tests/__init__.py` & `etos_lib-3.1.0/tests/__init__.py`

 * *Files identical despite different names*

