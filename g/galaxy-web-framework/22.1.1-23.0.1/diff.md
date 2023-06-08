# Comparing `tmp/galaxy-web-framework-22.1.1.tar.gz` & `tmp/galaxy-web-framework-23.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-web-framework-22.1.1.tar", last modified: Mon Aug 22 19:46:09 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/web_framework/dist/.tmp-rwefxay5/galaxy-web-framework-23.0.1.tar", last modified: Thu Jun  8 17:44:37 2023, max compression
```

## Comparing `galaxy-web-framework-22.1.1.tar` & `galaxy-web-framework-23.0.1.tar`

### file list

```diff
@@ -1,71 +1,57 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.779518 galaxy-web-framework-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      332 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-web-framework-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       28 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1662 2022-08-22 19:46:09.779657 galaxy-web-framework-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      308 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.767488 galaxy-web-framework-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       91 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      422 2022-08-22 19:45:30.000000 galaxy-web-framework-22.1.1/galaxy/project_galaxy_web_framework.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.768513 galaxy-web-framework-22.1.1/galaxy/web/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1163 2022-08-18 15:49:02.000000 galaxy-web-framework-22.1.1/galaxy/web/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      394 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/buildapp.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      436 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/galaxy/web/form_builder.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.769358 galaxy-web-framework-22.1.1/galaxy/web/framework/
--rw-r--r--   0 mvandenb   (501) staff       (20)      785 2022-08-18 15:49:02.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    19648 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/base.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    19471 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/decorators.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.770278 galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/
--rw-r--r--   0 mvandenb   (501) staff       (20)     3745 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    42184 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/grids.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2990 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/tags.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.773616 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/
--rw-r--r--   0 mvandenb   (501) staff       (20)       25 2022-02-02 10:06:09.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     7625 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/batch.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    17925 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/error.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     5640 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/profile.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     9883 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/remoteuser.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      374 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/request_id.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      838 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/sqldebug.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2557 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/static.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1469 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/statsd.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     4612 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/translogger.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     1030 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/xforwardedhost.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.774143 galaxy-web-framework-22.1.1/galaxy/web/legacy_framework/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/galaxy/web/legacy_framework/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    38679 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/legacy_framework/grids.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.774495 galaxy-web-framework-22.1.1/galaxy/web/proxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)    13087 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.775289 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/
--rw-r--r--   0 mvandenb   (501) staff       (20)      614 2022-02-02 10:06:09.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/Dockerfile
--rw-r--r--   0 mvandenb   (501) staff       (20)       62 2022-02-02 10:06:09.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/README.md
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.776090 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/
--rwxr-xr-x   0 mvandenb   (501) staff       (20)     1311 2022-02-02 10:06:09.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/main.js
--rw-r--r--   0 mvandenb   (501) staff       (20)     2073 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/mapper.js
--rw-r--r--   0 mvandenb   (501) staff       (20)     5590 2022-02-02 10:06:09.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/proxy.js
--rw-r--r--   0 mvandenb   (501) staff       (20)      490 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/galaxy/web/proxy/js/package.json
--rw-r--r--   0 mvandenb   (501) staff       (20)     3083 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/galaxy/web/statsd_client.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.777839 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1662 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)     1785 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)      117 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-08-22 19:46:09.000000 galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      117 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.778624 galaxy-web-framework-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:46:09.786251 galaxy-web-framework-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2920 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/test-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.778879 galaxy-web-framework-22.1.1/tests/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-web-framework-22.1.1/tests/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.779077 galaxy-web-framework-22.1.1/tests/web_framework/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:14.000000 galaxy-web-framework-22.1.1/tests/web_framework/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:09.779290 galaxy-web-framework-22.1.1/tests/web_framework/framework/
--rw-r--r--   0 mvandenb   (501) staff       (20)      778 2022-08-22 19:45:28.000000 galaxy-web-framework-22.1.1/tests/web_framework/framework/test_framework_base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-08 17:37:03.000000 galaxy-web-framework-23.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/form_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21135 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19565 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43001 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/grids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17408 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9999 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/remoteuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/request_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/sqldebug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/statsd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4549 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/translogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1227 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/xforwardedhost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/legacy_framework/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/legacy_framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38893 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/legacy_framework/grids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/
+-rw-r--r--   0 runner    (1001) docker     (123)    13254 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1311 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/main.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/mapper.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/proxy.js
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/proxy/js/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy/web/short_term_storage/
+-rw-r--r--   0 runner    (1001) docker     (123)    11361 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/short_term_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/galaxy/web/statsd_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-08 17:44:37.000000 galaxy-web-framework-23.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 17:37:04.000000 galaxy-web-framework-23.0.1/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-web-framework-22.1.1/LICENSE` & `galaxy-web-framework-23.0.1/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-web-framework-22.1.1/PKG-INFO` & `galaxy-web-framework-23.0.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 22.1.1
-Summary: Galaxy Web Framework
+Version: 23.0.1
+Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-framework.svg
    :target: https://pypi.org/project/galaxy-web-framework/
 
 
 Overview
 --------
 
 The Galaxy_ web framework.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
+
 
+=========
+Bug fixes
+=========
 
+* Various fixes to path prefix handling by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16033 <https://github.com/galaxyproject/galaxy/pull/16033>`_
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/__init__.py` & `galaxy-web-framework-23.0.1/galaxy/web/__init__.py`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/base.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,49 +1,80 @@
 """
 A simple WSGI application/framework.
 """
 import io
+import json
 import logging
 import os
 import socket
 import tarfile
 import tempfile
 import time
 import types
-from http.cookies import CookieError, SimpleCookie
+from http.cookies import (
+    CookieError,
+    SimpleCookie,
+)
 from importlib import import_module
+from urllib.parse import urljoin
 
 import routes
 import webob.compat
 import webob.cookies
 import webob.exc
-import webob.exc as httpexceptions  # noqa: F401
+import webob.exc as httpexceptions
+
 # We will use some very basic HTTP/wsgi utilities from the paste library
 from paste.response import HeaderDict
 
 from galaxy.util import smart_str
+from galaxy.util.resources import resource_string
 
 log = logging.getLogger(__name__)
 
 #: time of the most recent server startup
 server_starttime = int(time.time())
+try:
+    meta_json = json.loads(resource_string(__package__, "meta.json"))
+    server_starttime = meta_json.get("epoch") or server_starttime
+except Exception:
+    meta_json = {}
 
 
 def __resource_with_deleted(self, member_name, collection_name, **kwargs):
     """
     Method to monkeypatch on to routes.mapper.Mapper which does the same thing
     as resource() with the addition of standardized routes for handling
     elements in Galaxy's "deleted but not really deleted" fashion.
     """
     collection_path = f"{kwargs.get('path_prefix', '')}/{collection_name}/deleted"
     member_path = f"{collection_path}/{{id}}"
-    self.connect(f"deleted_{collection_name}", collection_path, controller=collection_name, action='index', deleted=True, conditions=dict(method=['GET']))
-    self.connect(f"deleted_{member_name}", member_path, controller=collection_name, action='show', deleted=True, conditions=dict(method=['GET']))
-    self.connect(f"undelete_deleted_{member_name}", f"{member_path}/undelete", controller=collection_name, action='undelete',
-                 conditions=dict(method=['POST']))
+    self.connect(
+        f"deleted_{collection_name}",
+        collection_path,
+        controller=collection_name,
+        action="index",
+        deleted=True,
+        conditions=dict(method=["GET"]),
+    )
+    self.connect(
+        f"deleted_{member_name}",
+        member_path,
+        controller=collection_name,
+        action="show",
+        deleted=True,
+        conditions=dict(method=["GET"]),
+    )
+    self.connect(
+        f"undelete_deleted_{member_name}",
+        f"{member_path}/undelete",
+        controller=collection_name,
+        action="undelete",
+        conditions=dict(method=["POST"]),
+    )
     self.resource(member_name, collection_name, **kwargs)
 
 
 routes.Mapper.resource_with_deleted = __resource_with_deleted
 
 
 class WebApplication:
@@ -75,37 +106,35 @@
 
     def add_ui_controller(self, controller_name, controller):
         """
         Add a controller class to this application. A controller class has
         methods which handle web requests. To connect a URL to a controller's
         method use `add_route`.
         """
-        log.debug("Enabling '%s' controller, class: %s",
-                  controller_name, controller.__class__.__name__)
+        log.debug("Enabling '%s' controller, class: %s", controller_name, controller.__class__.__name__)
         self.controllers[controller_name] = controller
 
     def add_api_controller(self, controller_name, controller):
-        log.debug("Enabling '%s' API controller, class: %s",
-                  controller_name, controller.__class__.__name__)
+        log.debug("Enabling '%s' API controller, class: %s", controller_name, controller.__class__.__name__)
         self.api_controllers[controller_name] = controller
 
     def add_route(self, route, **kwargs):
         """
         Add a route to match a URL with a method. Accepts all keyword
         arguments of `routes.Mapper.connect`. Every route should result in
         at least a controller value which corresponds to one of the
         objects added with `add_controller`. It optionally may yield an
         `action` argument which will be used to locate the method to call
         on the controller. Additional arguments will be passed to the
         method as keyword args.
         """
         self.mapper.connect(route, **kwargs)
 
-    def add_client_route(self, route, controller='root'):
-        self.clientside_routes.connect(route, controller=controller, action='client')
+    def add_client_route(self, route, controller="root"):
+        self.clientside_routes.connect(route, controller=controller, action="client")
 
     def set_transaction_factory(self, transaction_factory):
         """
         Use the callable `transaction_factory` to create the transaction
         which will be passed to requests.
         """
         self.transaction_factory = transaction_factory
@@ -126,65 +155,65 @@
     def __call__(self, environ, start_response):
         """
         Call interface as specified by WSGI. Wraps the environment in user
         friendly objects, finds the appropriate method to handle the request
         and calls it.
         """
         # Immediately create request_id which we will use for logging
-        request_id = environ.get('request_id', 'unknown')
+        request_id = environ.get("request_id", "unknown")
         if self.trace_logger:
             self.trace_logger.context_set("request_id", request_id)
         self.trace(message="Starting request")
         try:
             return self.handle_request(environ, start_response)
         finally:
             self.trace(message="Handle request finished")
             if self.trace_logger:
                 self.trace_logger.context_remove("request_id")
 
     def _resolve_map_match(self, map_match, path_info, controllers, use_default=True):
         # Get the controller class
-        controller_name = map_match.pop('controller', None)
+        controller_name = map_match.pop("controller", None)
         controller = controllers.get(controller_name, None)
         if controller is None:
             raise webob.exc.HTTPNotFound(f"No controller for {path_info}")
         # Resolve action method on controller
         # This is the easiest way to make the controller/action accessible for
         # url_for invocations.  Specifically, grids.
-        action = map_match.pop('action', 'index')
+        action = map_match.pop("action", "index")
         method = getattr(controller, action, None)
         if method is None and not use_default:
             # Skip default, we do this, for example, when we want to fail
             # through to another mapper.
             raise webob.exc.HTTPNotFound(f"No action for {path_info}")
         if method is None:
             # no matching method, we try for a default
-            method = getattr(controller, 'default', None)
+            method = getattr(controller, "default", None)
         if method is None:
             raise webob.exc.HTTPNotFound(f"No action for {path_info}")
         # Is the method exposed
-        if not getattr(method, 'exposed', False):
+        if not getattr(method, "exposed", False):
             raise webob.exc.HTTPNotFound(f"Action not exposed for {path_info}")
         # Is the method callable
         if not callable(method):
             raise webob.exc.HTTPNotFound(f"Action not callable for {path_info}")
         return (controller_name, controller, action, method)
 
     def handle_request(self, environ, start_response, body_renderer=None):
         # Grab the request_id (should have been set by middleware)
-        request_id = environ.get('request_id', 'unknown')
+        request_id = environ.get("request_id", "unknown")
         # Map url using routes
-        path_info = environ.get('PATH_INFO', '')
+        path_info = environ.get("PATH_INFO", "")
         client_match = self.clientside_routes.match(path_info, environ)
         map_match = self.mapper.match(path_info, environ) or client_match
-        if path_info.startswith('/api'):
-            environ['is_api_request'] = True
+        if path_info.startswith("/api"):
+            environ["is_api_request"] = True
             controllers = self.api_controllers
         else:
-            environ['is_api_request'] = False
+            environ["is_api_request"] = False
             controllers = self.controllers
         if map_match is None:
             raise webob.exc.HTTPNotFound(f"No route for {path_info}")
         self.trace(path_info=path_info, map_match=map_match)
         # Setup routes
         rc = routes.request_config()
         rc.mapper = self.mapper
@@ -194,29 +223,35 @@
         trans = self.transaction_factory(environ)
         trans.request_id = request_id
         rc.redirect = trans.response.send_redirect
         # Resolve mapping to controller/method
         try:
             # We don't use default methods if there's a clientside match for this route.
             use_default = client_match is None
-            controller_name, controller, action, method = self._resolve_map_match(map_match, path_info, controllers, use_default=use_default)
+            controller_name, controller, action, method = self._resolve_map_match(
+                map_match, path_info, controllers, use_default=use_default
+            )
         except webob.exc.HTTPNotFound:
             # Failed, let's check client routes
-            if not environ['is_api_request'] and client_match is not None:
-                controller_name, controller, action, method = self._resolve_map_match(client_match, path_info, controllers)
+            if not environ["is_api_request"] and client_match is not None:
+                controller_name, controller, action, method = self._resolve_map_match(
+                    client_match, path_info, controllers
+                )
             else:
                 raise
         trans.controller = controller_name
         trans.action = action
-        environ['controller_action_key'] = f"{'api' if environ['is_api_request'] else 'web'}.{controller_name}.{action or 'default'}"
+        environ[
+            "controller_action_key"
+        ] = f"{'api' if environ['is_api_request'] else 'web'}.{controller_name}.{action or 'default'}"
         # Combine mapper args and query string / form args and call
         kwargs = trans.request.params.mixed()
         kwargs.update(map_match)
         # Special key for AJAX debugging, remove to avoid confusing methods
-        kwargs.pop('_', None)
+        kwargs.pop("_", None)
         try:
             body = method(trans, **kwargs)
         except Exception as e:
             body = self.handle_controller_exception(e, trans, **kwargs)
             if not body:
                 raise
         body_renderer = body_renderer or self._render_body
@@ -227,23 +262,21 @@
         # a smart way
         if callable(body):
             # Assume the callable is another WSGI application to run
             return body(environ, start_response)
         elif isinstance(body, tarfile.ExFileObject):
             # Stream the tarfile member back to the browser
             body = iterate_file(body)
-            start_response(trans.response.wsgi_status(),
-                           trans.response.wsgi_headeritems())
+            start_response(trans.response.wsgi_status(), trans.response.wsgi_headeritems())
             return body
         elif isinstance(body, io.IOBase):
             # Stream the file back to the browser
             return send_file(start_response, trans, body)
         else:
-            start_response(trans.response.wsgi_status(),
-                           trans.response.wsgi_headeritems())
+            start_response(trans.response.wsgi_status(), trans.response.wsgi_headeritems())
             return self.make_body_iterable(trans, body)
 
     def make_body_iterable(self, trans, body):
         if isinstance(body, (types.GeneratorType, list, tuple)):
             # Recursively stream the iterable
             return flatten(body)
         elif body is None:
@@ -263,15 +296,15 @@
 class WSGIEnvironmentProperty:
     """
     Descriptor that delegates a property to a key in the environ member of the
     associated object (provides property style access to keys in the WSGI
     environment)
     """
 
-    def __init__(self, key, default=''):
+    def __init__(self, key, default=""):
         self.key = key
         self.default = default
 
     def __get__(self, obj, type=None):
         if obj is None:
             return self
         return obj.environ.get(self.key, self.default)
@@ -312,31 +345,31 @@
 
     @lazy_property
     def session(self):
         """
         Get the user's session state. This is laze since we rarely use it
         and the creation/serialization cost is high.
         """
-        if 'com.saddi.service.session' in self.environ:
-            return self.environ['com.saddi.service.session'].session
-        elif 'beaker.session' in self.environ:
-            return self.environ['beaker.session']
+        if "com.saddi.service.session" in self.environ:
+            return self.environ["com.saddi.service.session"].session
+        elif "beaker.session" in self.environ:
+            return self.environ["beaker.session"]
         else:
             return None
 
 
 def _make_file(self, binary=None):
     # For request.params, override cgi.FieldStorage.make_file to create persistent
     # tempfiles.  Necessary for externalizing the upload tool.  It's a little hacky
     # but for performance reasons it's way better to use Paste's tempfile than to
     # create a new one and copy.
     if self._binary_file or self.length >= 0:
         return tempfile.NamedTemporaryFile("wb+", delete=False)
     else:
-        return tempfile.NamedTemporaryFile("w+", encoding=self.encoding, newline='\n', delete=False)
+        return tempfile.NamedTemporaryFile("w+", encoding=self.encoding, newline="\n", delete=False)
 
 
 def _read_lines(self):
     # Always make a new file
     self.file = self.make_file()
     # Adapt `self.__file = None` to Python name mangling of class-private attributes.
     # We need to patch the original FieldStorage class attribute, not the cgi_FieldStorage
@@ -358,15 +391,16 @@
     """
 
     def __init__(self, environ):
         """
         Create a new request wrapping the WSGI environment `environ`
         """
         #  self.environ = environ
-        webob.Request.__init__(self, environ, charset='utf-8')
+        webob.Request.__init__(self, environ, charset="utf-8")
+
     # Properties that are computed and cached on first use
 
     @lazy_property
     def remote_host(self):
         try:
             return socket.gethostbyname(self.remote_addr)
         except OSError:
@@ -381,49 +415,53 @@
 
     @lazy_property
     def cookies(self):
         cookies = SimpleCookie()
         cookie_header = self.environ.get("HTTP_COOKIE")
         if cookie_header:
             all_cookies = webob.cookies.parse_cookie(cookie_header)
-            galaxy_cookies = {k.decode(): v.decode() for k, v in all_cookies if k.startswith(b'galaxy')}
+            galaxy_cookies = {k.decode(): v.decode() for k, v in all_cookies if k.startswith(b"galaxy")}
             if galaxy_cookies:
                 try:
                     cookies.load(galaxy_cookies)
                 except CookieError:
                     pass
         return cookies
 
     @lazy_property
     def base(self):
-        return (f"{self.scheme}://{self.host}")
+        return f"{self.scheme}://{self.host}"
+
+    @lazy_property
+    def url_path(self):
+        return urljoin(self.base, self.environ.get("SCRIPT_NAME", ""))
 
     # @lazy_property
     # def params( self ):
     #     return parse_formvars( self.environ )
 
     @lazy_property
     def path(self):
-        return self.environ.get('SCRIPT_NAME', '') + self.environ['PATH_INFO']
+        return self.environ.get("SCRIPT_NAME", "") + self.environ["PATH_INFO"]
 
     @lazy_property
     def browser_url(self):
         return self.base + self.path
 
     # Descriptors that map properties to the associated environment
 
     # scheme = WSGIEnvironmentProperty( 'wsgi.url_scheme' )
     # remote_addr = WSGIEnvironmentProperty( 'REMOTE_ADDR' )
 
-    remote_port = WSGIEnvironmentProperty('REMOTE_PORT')
+    remote_port = WSGIEnvironmentProperty("REMOTE_PORT")
 
     # method = WSGIEnvironmentProperty( 'REQUEST_METHOD' )
     # script_name = WSGIEnvironmentProperty( 'SCRIPT_NAME' )
 
-    protocol = WSGIEnvironmentProperty('SERVER_PROTOCOL')
+    protocol = WSGIEnvironmentProperty("SERVER_PROTOCOL")
 
     # query_string = WSGIEnvironmentProperty( 'QUERY_STRING' )
     # path_info = WSGIEnvironmentProperty( 'PATH_INFO' )
 
 
 class Response:
     """
@@ -459,15 +497,15 @@
     def wsgi_headeritems(self):
         """
         Return headers in format appropriate for WSGI `start_response`
         """
         result = self.headers.headeritems()
         # Add cookie to header
         for crumb in self.cookies.values():
-            header, value = str(crumb).split(': ', 1)
+            header, value = str(crumb).split(": ", 1)
             result.append((header, value))
         return result
 
     def wsgi_status(self):
         """
         Return status line in format appropriate for WSGI `start_response`
         """
@@ -476,47 +514,66 @@
             return "%d %s" % (exception.code, exception.title)
         else:
             return self.status
 
 
 # ---- Utilities ------------------------------------------------------------
 
-CHUNK_SIZE = 2 ** 16
+CHUNK_SIZE = 2**16
 
 
 def send_file(start_response, trans, body):
     # If configured use X-Accel-Redirect header for nginx
     base = trans.app.config.nginx_x_accel_redirect_base
     apache_xsendfile = trans.app.config.apache_xsendfile
     if base:
-        trans.response.headers.pop('content-length', None)
-        trans.response.headers['X-Accel-Redirect'] = \
-            base + os.path.abspath(body.name)
+        trans.response.headers.pop("content-length", None)
+        trans.response.headers["X-Accel-Redirect"] = base + os.path.abspath(body.name)
         body = [b""]
     elif apache_xsendfile:
-        trans.response.headers.pop('content-length', None)
-        trans.response.headers['X-Sendfile'] = os.path.abspath(body.name)
+        trans.response.headers.pop("content-length", None)
+        trans.response.headers["X-Sendfile"] = os.path.abspath(body.name)
         body = [b""]
     # Fall back on sending the file in chunks
     else:
-        body = iterate_file(body)
-    start_response(trans.response.wsgi_status(),
-                   trans.response.wsgi_headeritems())
+        trans.response.headers["accept-ranges"] = "bytes"
+        start = None
+        end = None
+        if trans.request.range:
+            start = trans.request.range.start
+            end = trans.request.range.end
+            file_size = trans.response.headers["content-length"]
+            trans.response.headers["content-length"] = str(end - start)
+            trans.response.headers["content-range"] = f"bytes {start}-{end - 1}/{file_size}"
+            trans.response.status = 206
+        body = iterate_file(body, start, end)
+    start_response(trans.response.wsgi_status(), trans.response.wsgi_headeritems())
     return body
 
 
-def iterate_file(fh):
+def iterate_file(fh, start=None, stop=None):
     """
     Progressively return chunks from `file`.
     """
+    length = None
+    if start:
+        fh.seek(start)
+    if stop:
+        length = stop - start
     while 1:
-        chunk = fh.read(CHUNK_SIZE)
+        read_size = CHUNK_SIZE
+        if length:
+            read_size = min(CHUNK_SIZE, length)
+            length -= read_size
+        chunk = fh.read(read_size)
         if not chunk:
             break
         yield chunk
+        if length is not None and length == 0:
+            break
 
 
 def flatten(seq):
     """
     Flatten a possible nested set of iterables
     """
     for x in seq:
@@ -527,12 +584,23 @@
             yield smart_str(x)
 
 
 def walk_controller_modules(package_name):
     package = import_module(package_name)
     controller_dir = package.__path__[0]
     for fname in os.listdir(controller_dir):
-        if not(fname.startswith("_")) and fname.endswith(".py"):
+        if not (fname.startswith("_")) and fname.endswith(".py"):
             name = fname[:-3]
             module_name = f"{package_name}.{name}"
             module = import_module(module_name)
             yield name, module
+
+
+__all__ = (
+    "DefaultWebTransaction",
+    "httpexceptions",
+    "lazy_property",
+    "routes",
+    "server_starttime",
+    "walk_controller_modules",
+    "WebApplication",
+)
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/decorators.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/decorators.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,33 +12,33 @@
     error_codes,
     MessageException,
     RequestParameterInvalidException,
     RequestParameterMissingException,
 )
 from galaxy.util import (
     parse_non_hex_float,
-    unicodify
+    unicodify,
 )
 from galaxy.util.json import safe_dumps
 from galaxy.web.framework import url_for
 
 log = logging.getLogger(__name__)
 
 JSON_CONTENT_TYPE = "application/json; charset=UTF-8"
 JSONP_CONTENT_TYPE = "application/javascript"
-JSONP_CALLBACK_KEY = 'callback'
+JSONP_CALLBACK_KEY = "callback"
 
 
 def error(message):
-    raise MessageException(message, type='error')
+    raise MessageException(message, type="error")
 
 
 # ----------------------------------------------------------------------------- web controller decorators
 def _save_orig_fn(wrapped, orig):
-    if not hasattr(orig, '_orig'):
+    if not hasattr(orig, "_orig"):
         wrapped._orig = orig
     return wrapped
 
 
 def expose(func):
     """
     Decorator: mark a function as 'exposed' and thus web accessible
@@ -48,26 +48,27 @@
 
 
 def json(func, pretty=False):
     """
     Format the response as JSON and set the response content type to
     JSON_CONTENT_TYPE.
     """
+
     @wraps(func)
     def call_and_format(self, trans, *args, **kwargs):
         # pull out any callback argument to the api endpoint and set the content type to json or javascript
         jsonp_callback = kwargs.pop(JSONP_CALLBACK_KEY, None)
         if jsonp_callback:
             trans.response.set_content_type(JSONP_CONTENT_TYPE)
         else:
             trans.response.set_content_type(JSON_CONTENT_TYPE)
         rval = func(self, trans, *args, **kwargs)
         return format_return_as_json(rval, jsonp_callback, pretty=(pretty or trans.debug))
 
-    if not hasattr(func, '_orig'):
+    if not hasattr(func, "_orig"):
         call_and_format._orig = func
     return expose(_save_orig_fn(call_and_format, func))
 
 
 def json_pretty(func):
     """
     Indent and sort returned JSON.
@@ -79,41 +80,42 @@
     def argcatcher(func):
         @wraps(func)
         def decorator(self, trans, *args, **kwargs):
             if trans.get_user():
                 return func(self, trans, *args, **kwargs)
             else:
                 redirect_url = url_for(controller=trans.controller, action=trans.action)
-                query_string = trans.environ.get('QUERY_STRING', '')
+                query_string = trans.environ.get("QUERY_STRING", "")
                 if query_string:
                     redirect_url = f"{redirect_url}?{query_string}"
-                href = url_for(controller='login', redirect=redirect_url)
+                href = url_for(controller="login", redirect=redirect_url)
                 return trans.show_error_message(
-                    f'You must be <a target="galaxy_main" href="{href}">logged in</a> to {verb}.',
-                    use_panels=use_panels
+                    f'You must be <a target="galaxy_main" href="{href}" class="require-login-link">logged in</a> to {verb}.',
+                    use_panels=use_panels,
                 )
+
         return decorator
+
     return argcatcher
 
 
 def require_admin(func):
     @wraps(func)
     def decorator(self, trans, *args, **kwargs):
         if not trans.user_is_admin:
             msg = require_admin_message(trans.app.config, trans.get_user())
             trans.response.status = 403
             content_type = trans.response.get_content_type()
             # content_type for instance may be... application/json; charset=UTF-8
-            if 'application/json' in content_type:
-                return __api_error_dict(
-                    trans, status_code=403, err_code=error_codes.ADMIN_REQUIRED, err_msg=msg
-                )
+            if "application/json" in content_type:
+                return __api_error_dict(trans, status_code=403, err_code=error_codes.ADMIN_REQUIRED, err_msg=msg)
             else:
                 return trans.show_error_message(msg)
         return func(self, trans, *args, **kwargs)
+
     return decorator
 
 
 def require_admin_message(config, user):
     if not config.admin_users_list:
         msg = "You must be logged in as an administrator to access this feature, but no administrators are set in the Galaxy configuration."
     elif not user:
@@ -123,64 +125,68 @@
     return msg
 
 
 def do_not_cache(func):
     """
     Sets cache-prevention headers for the request.
     """
+
     @wraps(func)
     def set_nocache_headers(self, trans, *args, **kwargs):
-        trans.response.headers['Cache-Control'] = ['no-cache', 'no-store', 'must-revalidate']
-        trans.response.headers['Pragma'] = 'no-cache'
-        trans.response.headers['Expires'] = '0'
+        trans.response.headers["Cache-Control"] = ["no-cache", "no-store", "must-revalidate"]
+        trans.response.headers["Pragma"] = "no-cache"
+        trans.response.headers["Expires"] = "0"
         return func(self, trans, *args, **kwargs)
+
     return set_nocache_headers
 
 
 # ----------------------------------------------------------------------------- (original) api decorators
 def legacy_expose_api(func, to_json=True, user_required=True):
     """
     Expose this function via the API.
     """
+
     @wraps(func)
     def decorator(self, trans, *args, **kwargs):
         def error(environ, start_response):
-            start_response(error_status, [('Content-type', 'text/plain')])
+            start_response(error_status, [("Content-type", "text/plain")])
             return error_message
-        error_status = '403 Forbidden'
+
+        error_status = "403 Forbidden"
         if trans.error_message:
             return trans.error_message
         if user_required and trans.anonymous:
             error_message = "API Authentication Required for this request"
             return error
         if trans.request.body:
             try:
-                kwargs['payload'] = __extract_payload_from_request(trans, func, kwargs)
+                kwargs["payload"] = __extract_payload_from_request(trans, func, kwargs)
             except ValueError:
-                error_status = '400 Bad Request'
-                error_message = 'Your request did not appear to be valid JSON, please consult the API documentation'
+                error_status = "400 Bad Request"
+                error_message = "Your request did not appear to be valid JSON, please consult the API documentation"
                 return error
 
         # pull out any callback argument to the api endpoint and set the content type to json or javascript
         jsonp_callback = kwargs.pop(JSONP_CALLBACK_KEY, None)
         if jsonp_callback:
             trans.response.set_content_type(JSONP_CONTENT_TYPE)
         else:
             trans.response.set_content_type(JSON_CONTENT_TYPE)
 
         # send 'do not cache' headers to handle IE's caching of ajax get responses
-        trans.response.headers['Cache-Control'] = "max-age=0,no-cache,no-store"
+        trans.response.headers["Cache-Control"] = "max-age=0,no-cache,no-store"
 
         # Perform api_run_as processing, possibly changing identity
-        if 'payload' in kwargs and isinstance(kwargs['payload'], dict) and 'run_as' in kwargs['payload']:
+        if "payload" in kwargs and isinstance(kwargs["payload"], dict) and "run_as" in kwargs["payload"]:
             if not trans.user_can_do_run_as:
-                error_message = 'User does not have permissions to run jobs as another user'
+                error_message = "User does not have permissions to run jobs as another user"
                 return error
             try:
-                decoded_user_id = trans.security.decode_id(kwargs['payload']['run_as'])
+                decoded_user_id = trans.security.decode_id(kwargs["payload"]["run_as"])
             except TypeError:
                 trans.response.status = 400
                 return f"Malformed user id ( {str(kwargs['payload']['run_as'])} ) specified, unable to decode."
             try:
                 user = trans.sa_session.query(trans.app.model.User).get(decoded_user_id)
                 trans.set_user(user)
             except Exception:
@@ -190,22 +196,23 @@
             rval = func(self, trans, *args, **kwargs)
             if to_json:
                 rval = format_return_as_json(rval, jsonp_callback, pretty=trans.debug)
             return rval
         except paste.httpexceptions.HTTPException:
             raise  # handled
         except Exception:
-            log.exception('Uncaught exception in exposed API method:')
+            log.exception("Uncaught exception in exposed API method:")
             raise paste.httpexceptions.HTTPServerError()
+
     return expose(_save_orig_fn(decorator, func))
 
 
 def __extract_payload_from_request(trans, func, kwargs):
-    content_type = trans.request.headers.get('content-type', '')
-    if content_type.startswith('application/x-www-form-urlencoded') or content_type.startswith('multipart/form-data'):
+    content_type = trans.request.headers.get("content-type", "")
+    if content_type.startswith("application/x-www-form-urlencoded") or content_type.startswith("multipart/form-data"):
         # If the content type is a standard type such as multipart/form-data, the wsgi framework parses the request body
         # and loads all field values into kwargs. However, kwargs also contains formal method parameters etc. which
         # are not a part of the request body. This is a problem because it's not possible to differentiate between values
         # which are a part of the request body, and therefore should be a part of the payload, and values which should not be
         # in the payload. Therefore, the decorated method's formal arguments are discovered through reflection and removed from
         # the payload dictionary. This helps to prevent duplicate argument conflicts in downstream methods.
         payload = kwargs.copy()
@@ -218,24 +225,24 @@
                     # note: parse_non_hex_float only needed here for single string values where something like
                     # 40000000000000e5 will be parsed as a scientific notation float. This is as opposed to hex strings
                     # in larger JSON structures where quoting prevents this (further below)
                     payload[k] = loads(v, parse_float=parse_non_hex_float)
                 except Exception:
                     # may not actually be json, just continue
                     pass
-    elif content_type == 'application/offset+octet-stream':
+    elif content_type == "application/offset+octet-stream":
         return unicodify(trans.request.body)
     else:
         # Assume application/json content type and parse request body manually, since wsgi won't do it. However, the order of this check
         # should ideally be in reverse, with the if clause being a check for application/json and the else clause assuming a standard encoding
         # such as multipart/form-data. Leaving it as is for backward compatibility, just in case.
         payload = loads(unicodify(trans.request.body))
-    run_as = trans.request.headers.get('run-as')
+    run_as = trans.request.headers.get("run-as")
     if run_as:
-        payload['run_as'] = run_as
+        payload["run_as"] = run_as
     return payload
 
 
 def legacy_expose_api_raw(func):
     """
     Expose this function via the API but don't dump the results
     to JSON.
@@ -259,56 +266,66 @@
 
 
 # ----------------------------------------------------------------------------- (new) api decorators
 def expose_api(func, to_json=True, user_required=True, user_or_session_required=True, handle_jsonp=True):
     """
     Expose this function via the API.
     """
+
     @wraps(func)
     def decorator(self, trans, *args, **kwargs):
         # errors passed in from trans._authenicate_api
         if trans.error_message:
-            return __api_error_response(trans, status_code=403, err_code=error_codes.USER_NO_API_KEY,
-                                        err_msg=trans.error_message)
+            return __api_error_response(
+                trans, status_code=403, err_code=error_codes.USER_NO_API_KEY, err_msg=trans.error_message
+            )
         if trans.anonymous:
             # error if anon and user required
             if user_required:
-                return __api_error_response(trans, status_code=403, err_code=error_codes.USER_NO_API_KEY,
-                                            err_msg="API authentication required for this request")
+                return __api_error_response(
+                    trans,
+                    status_code=403,
+                    err_code=error_codes.USER_NO_API_KEY,
+                    err_msg="API authentication required for this request",
+                )
             # error if anon and no session
             if not trans.galaxy_session and user_or_session_required:
-                return __api_error_response(trans, status_code=403, err_code=error_codes.USER_NO_API_KEY,
-                                            err_msg="API authentication or Galaxy session required for this request")
+                return __api_error_response(
+                    trans,
+                    status_code=403,
+                    err_code=error_codes.USER_NO_API_KEY,
+                    err_msg="API authentication or Galaxy session required for this request",
+                )
 
         if trans.request.body:
             try:
-                kwargs['payload'] = __extract_payload_from_request(trans, func, kwargs)
+                kwargs["payload"] = __extract_payload_from_request(trans, func, kwargs)
             except ValueError:
                 error_code = error_codes.USER_INVALID_JSON
                 return __api_error_response(trans, status_code=400, err_code=error_code)
 
         # pull out any callback argument to the api endpoint and set the content type to json or javascript
         # TODO: use handle_jsonp to NOT overwrite existing tool_shed JSONP
         jsonp_callback = kwargs.pop(JSONP_CALLBACK_KEY, None) if handle_jsonp else None
         if jsonp_callback:
             trans.response.set_content_type(JSONP_CONTENT_TYPE)
         else:
             trans.response.set_content_type(JSON_CONTENT_TYPE)
 
         # send 'do not cache' headers to handle IE's caching of ajax get responses
-        trans.response.headers['Cache-Control'] = "max-age=0,no-cache,no-store"
+        trans.response.headers["Cache-Control"] = "max-age=0,no-cache,no-store"
 
         # TODO: Refactor next block out into a helper procedure.
         # Perform api_run_as processing, possibly changing identity
-        if 'payload' in kwargs and 'run_as' in kwargs['payload']:
+        if "payload" in kwargs and "run_as" in kwargs["payload"]:
             if not trans.user_can_do_run_as:
                 error_code = error_codes.USER_CANNOT_RUN_AS
                 return __api_error_response(trans, err_code=error_code, status_code=403)
             try:
-                decoded_user_id = trans.security.decode_id(kwargs['payload']['run_as'])
+                decoded_user_id = trans.security.decode_id(kwargs["payload"]["run_as"])
             except (TypeError, ValueError):
                 error_message = f"Malformed user id ( {str(kwargs['payload']['run_as'])} ) specified, unable to decode."
                 error_code = error_codes.USER_INVALID_RUN_AS
                 return __api_error_response(trans, err_code=error_code, err_msg=error_message, status_code=400)
             try:
                 user = trans.sa_session.query(trans.app.model.User).get(decoded_user_id)
                 trans.set_user(user)
@@ -327,25 +344,26 @@
             traceback_string = format_exc()
             return __api_error_response(trans, exception=e, traceback=traceback_string)
         except paste.httpexceptions.HTTPException:
             # TODO: Allow to pass or format for the API???
             raise  # handled
         except Exception as e:
             traceback_string = format_exc()
-            error_message = 'Uncaught exception in exposed API method:'
+            error_message = "Uncaught exception in exposed API method:"
             log.exception(error_message)
             return __api_error_response(
                 trans,
                 status_code=500,
                 exception=e,
                 traceback=traceback_string,
                 err_msg=error_message,
-                err_code=error_codes.UNKNOWN
+                err_code=error_codes.UNKNOWN,
             )
-    if not hasattr(func, '_orig'):
+
+    if not hasattr(func, "_orig"):
         decorator._orig = func
     decorator.exposed = True
     return decorator
 
 
 def format_return_as_json(rval, jsonp_callback=None, pretty=False):
     """
@@ -359,15 +377,15 @@
     else:
         json = safe_dumps(rval, **dumps_kwargs)
     if jsonp_callback:
         json = f"{jsonp_callback}({json});"
     return json
 
 
-def validation_error_to_message_exception(e):
+def validation_error_to_message_exception(e: ValidationError) -> MessageException:
     invalid_found = False
     missing_found = False
     for error in e.errors():
         if error["type"] == "value_error.missing" or error["type"] == "type_error.none.not_allowed":
             missing_found = True
         elif error["type"].startswith("type_error"):
             invalid_found = True
@@ -379,15 +397,15 @@
 
 def api_error_message(trans, **kwds):
     exception = kwds.get("exception", None)
     if exception:
         # If we are passed a MessageException use err_msg.
         default_error_code = getattr(exception, "err_code", error_codes.UNKNOWN)
         default_error_message = getattr(exception, "err_msg", default_error_code.default_error_message)
-        extra_error_info = getattr(exception, 'extra_error_info', {})
+        extra_error_info = getattr(exception, "extra_error_info", {})
         if not isinstance(extra_error_info, dict):
             extra_error_info = {}
     else:
         default_error_message = "Error processing API request."
         default_error_code = error_codes.UNKNOWN
         extra_error_info = {}
     traceback_string = kwds.get("traceback", "No traceback available.")
@@ -453,14 +471,8 @@
 
 def expose_api_raw_anonymous(func):
     return expose_api(func, to_json=False, user_required=False)
 
 
 def expose_api_raw_anonymous_and_sessionless(func):
     # TODO: tool_shed api implemented JSONP first on a method-by-method basis, don't overwrite that for now
-    return expose_api(
-        func,
-        to_json=False,
-        user_required=False,
-        user_or_session_required=False,
-        handle_jsonp=False
-    )
+    return expose_api(func, to_json=False, user_required=False, user_or_session_required=False, handle_jsonp=False)
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/__init__.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,66 +1,65 @@
 """
 Galaxy web framework helpers
 
 The functions in this module should be considered part of the API used by
 visualizations in their mako files through the `$h` object, see
 GalaxyWebTransaction in galaxy/webapps/base/webapp.py
 """
-from datetime import datetime, timedelta
+from datetime import (
+    datetime,
+    timedelta,
+)
 
 from babel import default_locale
 from babel.dates import format_timedelta
 from routes import url_for
 
-from galaxy.util import (
-    hash_util,
-    smart_str,
-    unicodify,
-)
+from galaxy.util import unicodify
 from galaxy.util.json import safe_dumps as dumps  # noqa: F401
 from .tags import (
     javascript_link,
-    stylesheet_link
+    stylesheet_link,
 )
 from ..base import server_starttime
 
 
 def time_ago(x):
     """
     Convert a datetime to a string.
     """
     # If the date is more than one week ago, then display the actual date instead of in words
     if datetime.utcnow() - x > timedelta(weeks=1):  # Greater than a week difference
         return x.strftime("%b %d, %Y")
     else:
         # Workaround https://github.com/python-babel/babel/issues/137
         kwargs = dict()
-        if not default_locale('LC_TIME'):
-            kwargs['locale'] = 'en_US_POSIX'
-        return format_timedelta(x - datetime.utcnow(), threshold=1, add_direction=True, **kwargs)
+        if not default_locale("LC_TIME"):
+            kwargs["locale"] = "en_US_POSIX"
+        return format_timedelta(x - datetime.utcnow(), threshold=1, add_direction=True, **kwargs)  # type: ignore[arg-type] # https://github.com/python/mypy/issues/9676
 
 
 def iff(a, b, c):
     """
     Ternary shortcut
     """
     if a:
         return b
     else:
         return c
 
 
-def truncate(content, length=100, suffix='...'):
+def truncate(content, length=100, suffix="..."):
     """
     Smart string truncation
     """
     if len(content) <= length:
         return content
     else:
-        return content[:length].rsplit(' ', 1)[0] + suffix
+        return content[:length].rsplit(" ", 1)[0] + suffix
 
 
 # Quick helpers for static content
 def css(*args):
     """
     Take a list of stylesheet names (no extension) and return appropriate string
     of link tags.
@@ -92,41 +91,31 @@
 
 
 def dist_js(*args):
     """
     Take a prefix and list of javascript names and return appropriate
     string of script tags.
     """
-    return js_helper('static/dist/', *args)
-
-
-# Hashes
-def md5(s):
-    """
-    Return hex encoded md5 hash of string s
-    """
-    m = hash_util.md5()
-    m.update(smart_str(s))
-    return m.hexdigest()
+    return js_helper("static/dist/", *args)
 
 
 # Unicode help
 def to_unicode(a_string):
     """
     Convert a string to unicode in utf-8 format; if string is already unicode,
     does nothing because string's encoding cannot be determined by introspection.
     """
-    return unicodify(a_string, 'utf-8')
+    return unicodify(a_string, "utf-8")
 
 
 def is_true(val):
     """
     Returns true if input is a boolean and true or is a string and looks like a true value.
     """
-    return val is True or val in ['True', 'true', 'T', 't']
+    return val is True or val in ["True", "true", "T", "t"]
 
 
 def to_js_bool(val):
     """
     Prints javascript boolean for passed value.
     TODO: isn't there a standard python JSON parser we should
     be using instead of all these manual conversions?
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/grids.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/grids.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,45 +1,82 @@
 import logging
 import math
-from json import dumps, loads
-from typing import Dict, List, Optional
+from json import (
+    dumps,
+    loads,
+)
+from typing import (
+    Dict,
+    List,
+    Optional,
+)
 
 from markupsafe import escape
-from sqlalchemy.sql.expression import and_, false, func, null, or_, true
-
-from galaxy.model.item_attrs import get_foreign_key, UsesAnnotations, UsesItemRatings
-from galaxy.util import restore_text, sanitize_text, unicodify
-from galaxy.web.framework import decorators, url_for
-
+from sqlalchemy.sql.expression import (
+    and_,
+    false,
+    func,
+    null,
+    or_,
+    true,
+)
+
+from galaxy.model.item_attrs import (
+    get_foreign_key,
+    UsesAnnotations,
+    UsesItemRatings,
+)
+from galaxy.util import (
+    restore_text,
+    sanitize_text,
+    unicodify,
+)
+from galaxy.web.framework import (
+    decorators,
+    url_for,
+)
 
 log = logging.getLogger(__name__)
 
 
 class GridColumn:
-    def __init__(self, label, key=None, model_class=None, method=None, format=None,
-                 link=None, attach_popup=False, visible=True, nowrap=False,
-                 # Valid values for filterable are ['standard', 'advanced', None]
-                 filterable=None, sortable=True, label_id_prefix=None, target=None,
-                 delayed=False):
+    def __init__(
+        self,
+        label,
+        key=None,
+        model_class=None,
+        method=None,
+        format=None,
+        link=None,
+        attach_popup=False,
+        visible=True,
+        nowrap=False,
+        # Valid values for filterable are ['standard', 'advanced', None]
+        filterable=None,
+        sortable=True,
+        label_id_prefix=None,
+        target=None,
+        delayed=False,
+    ):
         """Create a grid column."""
         self.label = label
         self.key = key
         self.model_class = model_class
         self.method = method
         self.format = format
         self.link = link
         self.target = target
         self.nowrap = nowrap
         self.attach_popup = attach_popup
         self.visible = visible
         self.filterable = filterable
         self.delayed = delayed
         # Column must have a key to be sortable.
-        self.sortable = (self.key is not None and sortable)
-        self.label_id_prefix = label_id_prefix or ''
+        self.sortable = self.key is not None and sortable
+        self.label_id_prefix = label_id_prefix or ""
 
     def get_value(self, trans, grid, item):
         if self.method:
             value = getattr(grid, self.method)(trans, item)
         elif self.key and hasattr(item, self.key):
             value = getattr(item, self.key)
         else:
@@ -50,25 +87,25 @@
 
     def get_link(self, trans, grid, item):
         if self.link and self.link(item):
             return self.link(item)
         return None
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to reflect the column filter. """
+        """Modify query to reflect the column filter."""
         if column_filter == "All":
             pass
         if column_filter == "True":
             query = query.filter_by(**{self.key: True})
         elif column_filter == "False":
             query = query.filter_by(**{self.key: False})
         return query
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filters_vals = ["False", "True", "All"]
         accepted_filters = []
         for val in accepted_filters_vals:
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(val, args))
         return accepted_filters
 
@@ -83,33 +120,33 @@
             query = query.order_by(column.asc())
         else:
             query = query.order_by(column.desc())
         return query
 
 
 class ReverseSortColumn(GridColumn):
-    """ Column that reverses sorting; this is useful when the natural sort is descending. """
+    """Column that reverses sorting; this is useful when the natural sort is descending."""
 
     def sort(self, trans, query, ascending, column_name=None):
         return GridColumn.sort(self, trans, query, (not ascending), column_name=column_name)
 
 
 class TextColumn(GridColumn):
-    """ Generic column that employs freetext and, hence, supports freetext, case-independent filtering. """
+    """Generic column that employs freetext and, hence, supports freetext, case-independent filtering."""
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter using free text, case independence. """
+        """Modify query to filter using free text, case independence."""
         if column_filter == "All":
             pass
         elif column_filter:
             query = query.filter(self.get_filter(trans, user, column_filter))
         return query
 
     def get_filter(self, trans, user, column_filter):
-        """ Returns a SQLAlchemy criterion derived from column_filter. """
+        """Returns a SQLAlchemy criterion derived from column_filter."""
         if isinstance(column_filter, str):
             return self.get_single_filter(user, column_filter)
         elif isinstance(column_filter, list):
             clause_list = []
             for filter in column_filter:
                 clause_list.append(self.get_single_filter(user, filter))
             return and_(*clause_list)
@@ -117,16 +154,16 @@
     def get_single_filter(self, user, a_filter):
         """
         Returns a SQLAlchemy criterion derived for a single filter. Single filter
         is the most basic filter--usually a string--and cannot be a list.
         """
         # Queries that include table joins cannot guarantee that table column names will be
         # unique, so check to see if a_filter is of type <TableName>.<ColumnName>.
-        if self.key.find('.') > -1:
-            a_key = self.key.split('.')[1]
+        if self.key.find(".") > -1:
+            a_key = self.key.split(".")[1]
         else:
             a_key = self.key
         model_class_key_field = getattr(self.model_class, a_key)
         return func.lower(model_class_key_field).like(f"%{a_filter.lower()}%")
 
     def sort(self, trans, query, ascending, column_name=None):
         """Sort column using case-insensitive alphabetical sorting."""
@@ -147,16 +184,16 @@
 
 class BooleanColumn(TextColumn):
     def sort(self, trans, query, ascending, column_name=None):
         """Sort query using this column."""
         return GridColumn.sort(self, trans, query, ascending, column_name=column_name)
 
     def get_single_filter(self, user, a_filter):
-        if self.key.find('.') > -1:
-            a_key = self.key.split('.')[1]
+        if self.key.find(".") > -1:
+            a_key = self.key.split(".")[1]
         else:
             a_key = self.key
         model_class_key_field = getattr(self.model_class, a_key)
         return model_class_key_field == a_filter
 
 
 class IntegerColumn(TextColumn):
@@ -184,95 +221,118 @@
 
     def sort(self, trans, query, ascending, column_name=None):
         """Sort query using this column."""
         return GridColumn.sort(self, trans, query, ascending, column_name=column_name)
 
 
 class CommunityRatingColumn(GridColumn, UsesItemRatings):
-    """ Column that displays community ratings for an item. """
+    """Column that displays community ratings for an item."""
 
     def get_value(self, trans, grid, item):
         if not hasattr(item, "average_rating"):
             # No prefetched column property, generate it on the fly.
-            ave_item_rating, num_ratings = self.get_ave_item_rating_data(trans.sa_session, item, webapp_model=trans.model)
+            ave_item_rating, num_ratings = self.get_ave_item_rating_data(
+                trans.sa_session, item, webapp_model=trans.model
+            )
         else:
             ave_item_rating = item.average_rating
             num_ratings = 2  # just used for pluralization
         if not ave_item_rating:
             ave_item_rating = 0
-        return trans.fill_template("tool_shed_rating.mako",
-                                   ave_item_rating=ave_item_rating,
-                                   num_ratings=num_ratings,
-                                   item_id=trans.security.encode_id(item.id))
+        return trans.fill_template(
+            "tool_shed_rating.mako",
+            ave_item_rating=ave_item_rating,
+            num_ratings=num_ratings,
+            item_id=trans.security.encode_id(item.id),
+        )
 
     def sort(self, trans, query, ascending, column_name=None):
         # Get the columns that connect item's table and item's rating association table.
-        item_rating_assoc_class = getattr(trans.model, f'{self.model_class.__name__}RatingAssociation')
+        item_rating_assoc_class = getattr(trans.model, f"{self.model_class.__name__}RatingAssociation")
         foreign_key = get_foreign_key(item_rating_assoc_class, self.model_class)
         fk_col = foreign_key.parent
         referent_col = foreign_key.get_referent(self.model_class.table)
         # Do sorting using a subquery.
         # Subquery to get average rating for each item.
-        ave_rating_subquery = trans.sa_session.query(fk_col,
-                                                     func.avg(item_rating_assoc_class.table.c.rating).label('avg_rating')) \
-            .group_by(fk_col).subquery()
+        ave_rating_subquery = (
+            trans.sa_session.query(fk_col, func.avg(item_rating_assoc_class.table.c.rating).label("avg_rating"))
+            .group_by(fk_col)
+            .subquery()
+        )
         # Integrate subquery into main query.
         query = query.outerjoin((ave_rating_subquery, referent_col == ave_rating_subquery.columns[fk_col.name]))
         # Sort using subquery results; use coalesce to avoid null values.
-        if not ascending:  # TODO: for now, reverse sorting b/c first sort is ascending, and that should be the natural sort.
+        if (
+            not ascending
+        ):  # TODO: for now, reverse sorting b/c first sort is ascending, and that should be the natural sort.
             query = query.order_by(func.coalesce(ave_rating_subquery.c.avg_rating, 0).asc())
         else:
             query = query.order_by(func.coalesce(ave_rating_subquery.c.avg_rating, 0).desc())
         return query
 
 
 class OwnerAnnotationColumn(TextColumn, UsesAnnotations):
-    """ Column that displays and filters item owner's annotations. """
+    """Column that displays and filters item owner's annotations."""
 
     def __init__(self, col_name, key, model_class=None, model_annotation_association_class=None, filterable=None):
         GridColumn.__init__(self, col_name, key=key, model_class=model_class, filterable=filterable)
         self.sortable = False
         self.model_annotation_association_class = model_annotation_association_class
 
     def get_value(self, trans, grid, item):
-        """ Returns first 150 characters of annotation. """
+        """Returns first 150 characters of annotation."""
         annotation = self.get_item_annotation_str(trans.sa_session, item.user, item)
         if annotation:
             ann_snippet = annotation[:155]
             if len(annotation) > 155:
-                ann_snippet = ann_snippet[:ann_snippet.rfind(' ')]
+                ann_snippet = ann_snippet[: ann_snippet.rfind(" ")]
                 ann_snippet += "..."
         else:
             ann_snippet = ""
         return escape(ann_snippet)
 
     def get_single_filter(self, user, a_filter):
-        """ Filter by annotation and annotation owner. """
+        """Filter by annotation and annotation owner."""
         return self.model_class.annotations.any(
-            and_(func.lower(self.model_annotation_association_class.annotation).like(f"%{a_filter.lower()}%"),
-               # TODO: not sure why, to filter by owner's annotations, we have to do this rather than
-               # 'self.model_class.user==self.model_annotation_association_class.user'
-               self.model_annotation_association_class.table.c.user_id == self.model_class.table.c.user_id))
+            and_(
+                func.lower(self.model_annotation_association_class.annotation).like(f"%{a_filter.lower()}%"),
+                # TODO: not sure why, to filter by owner's annotations, we have to do this rather than
+                # 'self.model_class.user==self.model_annotation_association_class.user'
+                self.model_annotation_association_class.table.c.user_id == self.model_class.table.c.user_id,
+            )
+        )
 
 
 class CommunityTagsColumn(TextColumn):
-    """ Column that supports community tags. """
+    """Column that supports community tags."""
 
-    def __init__(self, col_name, key, model_class=None, model_tag_association_class=None, filterable=None, grid_name=None):
-        GridColumn.__init__(self, col_name, key=key, model_class=model_class, nowrap=True, filterable=filterable, sortable=False)
+    def __init__(
+        self, col_name, key, model_class=None, model_tag_association_class=None, filterable=None, grid_name=None
+    ):
+        GridColumn.__init__(
+            self, col_name, key=key, model_class=model_class, nowrap=True, filterable=filterable, sortable=False
+        )
         self.model_tag_association_class = model_tag_association_class
         # Column-specific attributes.
         self.grid_name = grid_name
 
     def get_value(self, trans, grid, item):
-        return trans.fill_template("/tagging_common.mako", tag_type="community", trans=trans, user=trans.get_user(), tagged_item=item, elt_context=self.grid_name,
-                                   tag_click_fn="add_tag_to_grid_filter", use_toggle_link=True)
+        return trans.fill_template(
+            "/tagging_common.mako",
+            tag_type="community",
+            trans=trans,
+            user=trans.get_user(),
+            tagged_item=item,
+            elt_context=self.grid_name,
+            tag_click_fn="add_tag_to_grid_filter",
+            use_toggle_link=True,
+        )
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter model_class by tag. Multiple filters are ANDed. """
+        """Modify query to filter model_class by tag. Multiple filters are ANDed."""
         if column_filter == "All":
             pass
         elif column_filter:
             query = query.filter(self.get_filter(trans, user, column_filter))
         return query
 
     def get_filter(self, trans, user, column_filter):
@@ -281,59 +341,83 @@
             # Collapse list of tags into a single string; this is redundant but effective. TODO: fix this by iterating over tags.
             column_filter = ",".join(column_filter)
         raw_tags = trans.app.tag_handler.parse_tags(column_filter)
         clause_list = []
         for name, value in raw_tags:
             if name:
                 # Filter by all tags.
-                clause_list.append(self.model_class.tags.any(func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%")))
+                clause_list.append(
+                    self.model_class.tags.any(
+                        func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%")
+                    )
+                )
                 if value:
                     # Filter by all values.
-                    clause_list.append(self.model_class.tags.any(func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%")))
+                    clause_list.append(
+                        self.model_class.tags.any(
+                            func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%")
+                        )
+                    )
         return and_(*clause_list)
 
 
 class IndividualTagsColumn(CommunityTagsColumn):
-    """ Column that supports individual tags. """
+    """Column that supports individual tags."""
 
     def get_value(self, trans, grid, item):
-        return trans.fill_template("/tagging_common.mako",
-                                   tag_type="individual",
-                                   user=trans.user,
-                                   tagged_item=item,
-                                   elt_context=self.grid_name,
-                                   tag_click_fn="add_tag_to_grid_filter",
-                                   use_toggle_link=True)
+        return trans.fill_template(
+            "/tagging_common.mako",
+            tag_type="individual",
+            user=trans.user,
+            tagged_item=item,
+            elt_context=self.grid_name,
+            tag_click_fn="add_tag_to_grid_filter",
+            use_toggle_link=True,
+        )
 
     def get_filter(self, trans, user, column_filter):
         # Parse filter to extract multiple tags.
         if isinstance(column_filter, list):
             # Collapse list of tags into a single string; this is redundant but effective. TODO: fix this by iterating over tags.
             column_filter = ",".join(column_filter)
         raw_tags = trans.app.tag_handler.parse_tags(column_filter)
         clause_list = []
         for name, value in raw_tags:
             if name:
                 # Filter by individual's tag names.
-                clause_list.append(self.model_class.tags.any(and_(func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%"), self.model_tag_association_class.user == user)))
+                clause_list.append(
+                    self.model_class.tags.any(
+                        and_(
+                            func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%"),
+                            self.model_tag_association_class.user == user,
+                        )
+                    )
+                )
                 if value:
                     # Filter by individual's tag values.
-                    clause_list.append(self.model_class.tags.any(and_(func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%"), self.model_tag_association_class.user == user)))
+                    clause_list.append(
+                        self.model_class.tags.any(
+                            and_(
+                                func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%"),
+                                self.model_tag_association_class.user == user,
+                            )
+                        )
+                    )
         return and_(*clause_list)
 
 
 class MulticolFilterColumn(TextColumn):
-    """ Column that performs multicolumn filtering. """
+    """Column that performs multicolumn filtering."""
 
     def __init__(self, col_name, cols_to_filter, key, visible, filterable="default"):
         GridColumn.__init__(self, col_name, key=key, visible=visible, filterable=filterable)
         self.cols_to_filter = cols_to_filter
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter model_class by tag. Multiple filters are ANDed. """
+        """Modify query to filter model_class by tag. Multiple filters are ANDed."""
         if column_filter == "All":
             return query
         if isinstance(column_filter, list):
             clause_list = []
             for filter in column_filter:
                 part_clause_list = []
                 for column in self.cols_to_filter:
@@ -345,47 +429,47 @@
             for column in self.cols_to_filter:
                 clause_list.append(column.get_filter(trans, user, column_filter))
             complete_filter = or_(*clause_list)
         return query.filter(complete_filter)
 
 
 class OwnerColumn(TextColumn):
-    """ Column that lists item's owner. """
+    """Column that lists item's owner."""
 
     def get_value(self, trans, grid, item):
         return item.user.username
 
     def sort(self, trans, query, ascending, column_name=None):
-        """ Sort column using case-insensitive alphabetical sorting on item's username. """
+        """Sort column using case-insensitive alphabetical sorting on item's username."""
         if ascending:
             query = query.order_by(func.lower(self.model_class.username).asc())
         else:
             query = query.order_by(func.lower(self.model_class.username).desc())
         return query
 
 
 class PublicURLColumn(TextColumn):
-    """ Column displays item's public URL based on username and slug. """
+    """Column displays item's public URL based on username and slug."""
 
     def get_link(self, trans, grid, item):
         if item.user.username and item.slug:
-            return dict(action='display_by_username_and_slug', username=item.user.username, slug=item.slug)
+            return dict(action="display_by_username_and_slug", username=item.user.username, slug=item.slug)
         elif not item.user.username:
             # TODO: provide link to set username.
             return None
         elif not item.user.slug:
             # TODO: provide link to set slug.
             return None
 
 
 class DeletedColumn(GridColumn):
-    """ Column that tracks and filters for items with deleted attribute. """
+    """Column that tracks and filters for items with deleted attribute."""
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filter_labels_and_vals = {"active": "False", "deleted": "True", "all": "All"}
         accepted_filters = []
         for label, val in accepted_filter_labels_and_vals.items():
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(label, args))
         return accepted_filters
 
@@ -395,18 +479,18 @@
             pass
         elif column_filter in ["True", "False"]:
             query = query.filter(self.model_class.deleted == (column_filter == "True"))
         return query
 
 
 class PurgedColumn(GridColumn):
-    """ Column that tracks and filters for items with purged attribute. """
+    """Column that tracks and filters for items with purged attribute."""
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filter_labels_and_vals = {"nonpurged": "False", "purged": "True", "all": "All"}
         accepted_filters = []
         for label, val in accepted_filter_labels_and_vals.items():
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(label, args))
         return accepted_filters
 
@@ -436,24 +520,24 @@
             pass
         elif column_filter in [v for k, v in self.model_class.states.items()]:
             query = query.filter(self.model_class.state == column_filter)
         return query
 
     def get_accepted_filters(self):
         """Returns a list of accepted filters for this column."""
-        all = GridColumnFilter('all', {self.key: 'All'})
+        all = GridColumnFilter("all", {self.key: "All"})
         accepted_filters = [all]
         for v in self.model_class.states.values():
             args = {self.key: v}
             accepted_filters.append(GridColumnFilter(v, args))
         return accepted_filters
 
 
 class SharingStatusColumn(GridColumn):
-    """ Grid column to indicate sharing status. """
+    """Grid column to indicate sharing status."""
 
     def __init__(self, *args, **kwargs):
         self.use_shared_with_count = kwargs.pop("use_shared_with_count", False)
         super().__init__(*args, **kwargs)
 
     def get_value(self, trans, grid, item):
         # Delete items cannot be shared.
@@ -473,15 +557,15 @@
         if self.use_shared_with_count:
             # optimization to skip join for users_shared_with and loading in that data.
             return item.users_shared_with_count > 0
 
         return item.users_shared_with
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter histories by sharing status. """
+        """Modify query to filter histories by sharing status."""
         if column_filter == "All":
             pass
         elif column_filter:
             if column_filter == "private":
                 query = query.filter(self.model_class.users_shared_with == null())
                 query = query.filter(self.model_class.importable == false())
             elif column_filter == "shared":
@@ -489,32 +573,42 @@
             elif column_filter == "accessible":
                 query = query.filter(self.model_class.importable == true())
             elif column_filter == "published":
                 query = query.filter(self.model_class.published == true())
         return query
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filter_labels_and_vals = {}
         accepted_filter_labels_and_vals["private"] = "private"
         accepted_filter_labels_and_vals["shared"] = "shared"
         accepted_filter_labels_and_vals["accessible"] = "accessible"
         accepted_filter_labels_and_vals["published"] = "published"
         accepted_filter_labels_and_vals["all"] = "All"
         accepted_filters = []
         for label, val in accepted_filter_labels_and_vals.items():
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(label, args))
         return accepted_filters
 
 
 class GridOperation:
-    def __init__(self, label, key=None, condition=None, allow_multiple=True, allow_popup=True,
-                 target=None, url_args=None, async_compatible=False, confirm=None,
-                 global_operation=None):
+    def __init__(
+        self,
+        label,
+        key=None,
+        condition=None,
+        allow_multiple=True,
+        allow_popup=True,
+        target=None,
+        url_args=None,
+        async_compatible=False,
+        confirm=None,
+        global_operation=None,
+    ):
         self.label = label
         self.key = key
         self.allow_multiple = allow_multiple
         self.allow_popup = allow_popup
         self.condition = condition
         self.target = target
         self.url_args = url_args
@@ -529,31 +623,31 @@
 
     def get_url_args(self, item):
         if self.url_args:
             if callable(self.url_args):
                 url_args = self.url_args(item)
             else:
                 url_args = dict(self.url_args)
-            url_args['id'] = item.id
+            url_args["id"] = item.id
             return url_args
         else:
             return dict(operation=self.label, id=item.id)
 
     def allowed(self, item):
         if self.condition:
             return bool(self.condition(item))
         else:
             return True
 
 
 class DisplayByUsernameAndSlugGridOperation(GridOperation):
-    """ Operation to display an item by username and slug. """
+    """Operation to display an item by username and slug."""
 
     def get_url_args(self, item):
-        return {'action': 'display_by_username_and_slug', 'username': item.user.username, 'slug': item.slug}
+        return {"action": "display_by_username_and_slug", "username": item.user.username, "slug": item.slug}
 
 
 class GridAction:
     def __init__(self, label=None, url_args=None, target=None):
         self.label = label
         self.url_args = url_args
         self.target = target
@@ -571,14 +665,15 @@
         return rval
 
 
 class Grid:
     """
     Specifies the content and format of a grid (data table).
     """
+
     title = ""
     model_class: Optional[type] = None
     show_item_checkboxes = False
     use_hide_message = True
     global_actions: List[GridAction] = []
     columns: List[GridColumn] = []
     operations: List[GridOperation] = []
@@ -608,33 +703,33 @@
         for column in self.columns:
             if not column.model_class:
                 column.model_class = self.model_class
 
     def __call__(self, trans, **kwargs):
         # Get basics.
         # FIXME: pretty sure this is only here to pass along, can likely be eliminated
-        status = kwargs.get('status', None)
-        message = kwargs.get('message', None)
+        status = kwargs.get("status", None)
+        message = kwargs.get("message", None)
         # Build a base filter and sort key that is the combination of the saved state and defaults.
         # Saved state takes preference over defaults.
         base_filter = {}
         if self.default_filter:
             # default_filter is a dictionary that provides a default set of filters based on the grid's columns.
             base_filter = self.default_filter.copy()
         base_sort_key = self.default_sort_key
         # Build initial query
         query = self.build_initial_query(trans, **kwargs)
         query = self.apply_query_filter(trans, query, **kwargs)
         # Maintain sort state in generated urls
         extra_url_args = {}
         # Determine whether use_default_filter flag is set.
-        use_default_filter_str = kwargs.get('use_default_filter')
+        use_default_filter_str = kwargs.get("use_default_filter")
         use_default_filter = False
         if use_default_filter_str:
-            use_default_filter = (use_default_filter_str.lower() == 'true')
+            use_default_filter = use_default_filter_str.lower() == "true"
         # Process filtering arguments to (a) build a query that represents the filter and (b) build a
         # dictionary that denotes the current filter.
         cur_filter_dict = {}
         for column in self.columns:
             if column.key:
                 # Get the filter criterion for the column. Precedence is (a) if using default filter, only look there; otherwise,
                 # (b) look in kwargs; and (c) look in base filter.
@@ -665,34 +760,35 @@
                         except ValueError:
                             decoded_list = [str(item)]
                     elif isinstance(item, list):
                         for element in item:
                             a_list = loads_recurse(element)
                             decoded_list = decoded_list + a_list
                     return decoded_list
+
                 # If column filter found, apply it.
                 if column_filter is not None:
                     # TextColumns may have a mix of json and strings.
                     if isinstance(column, TextColumn):
                         column_filter = loads_recurse(column_filter)
                         if len(column_filter) == 1:
                             column_filter = column_filter[0]
                     # Interpret ',' as a separator for multiple terms.
-                    if isinstance(column_filter, str) and column_filter.find(',') != -1:
-                        column_filter = column_filter.split(',')
+                    if isinstance(column_filter, str) and column_filter.find(",") != -1:
+                        column_filter = column_filter.split(",")
 
                     # Check if filter is empty
                     if isinstance(column_filter, list):
                         # Remove empty strings from filter list
-                        column_filter = [x for x in column_filter if x != '']
+                        column_filter = [x for x in column_filter if x != ""]
                         if len(column_filter) == 0:
                             continue
                     elif isinstance(column_filter, str):
                         # If filter criterion is empty, do nothing.
-                        if column_filter == '':
+                        if column_filter == "":
                             continue
 
                     # Update query.
                     query = column.filter(trans, trans.user, query, column_filter)
                     # Upate current filter dict.
                     # Column filters are rendered in various places, sanitize them all here.
                     cur_filter_dict[column.key] = sanitize_text(column_filter)
@@ -702,55 +798,55 @@
                         # Filter is a list; process each item.
                         extra_url_args[f"f-{column.key}"] = dumps(column_filter)
                     else:
                         # Process singleton filter.
                         extra_url_args[f"f-{column.key}"] = column_filter
         # Process sort arguments.
         sort_key = None
-        if 'sort' in kwargs:
-            sort_key = kwargs['sort']
+        if "sort" in kwargs:
+            sort_key = kwargs["sort"]
         elif base_sort_key:
             sort_key = base_sort_key
         if sort_key:
-            ascending = not(sort_key.startswith("-"))
+            ascending = not (sort_key.startswith("-"))
             # Queries that include table joins cannot guarantee unique column names.  This problem is
             # handled by setting the column_filter value to <TableName>.<ColumnName>.
             table_name = None
-            if sort_key.find('.') > -1:
-                a_list = sort_key.split('.')
+            if sort_key.find(".") > -1:
+                a_list = sort_key.split(".")
                 if ascending:
                     table_name = a_list[0]
                 else:
                     table_name = a_list[0][1:]
                 column_name = a_list[1]
             elif ascending:
                 column_name = sort_key
             else:
                 column_name = sort_key[1:]
             # Sort key is a column key.
             for column in self.columns:
-                if column.key and column.key.find('.') > -1:
-                    column_key = column.key.split('.')[1]
+                if column.key and column.key.find(".") > -1:
+                    column_key = column.key.split(".")[1]
                 else:
                     column_key = column.key
                 if (table_name is None or table_name == column.model_class.__name__) and column_key == column_name:
                     query = column.sort(trans, query, ascending, column_name=column_name)
                     break
-            extra_url_args['sort'] = sort_key
+            extra_url_args["sort"] = sort_key
         # There might be a current row
         current_item = self.get_current_item(trans, **kwargs)
         # Process page number.
         num_pages = None
         total_row_count_query = query  # query without limit applied to get total number of rows.
         if self.use_paging:
-            if 'page' in kwargs:
-                if kwargs['page'] == 'all':
+            if "page" in kwargs:
+                if kwargs["page"] == "all":
                     page_num = 0
                 else:
-                    page_num = int(kwargs['page'])
+                    page_num = int(kwargs["page"])
             else:
                 page_num = 1
             if page_num == 0:
                 num_pages = 1
                 page_num = 1
             else:
                 query = query.limit(self.num_rows_per_page).offset((page_num - 1) * self.num_rows_per_page)
@@ -760,175 +856,176 @@
         # There are some places in grid templates where it's useful for a grid
         # to have its current filter.
         self.cur_filter_dict = cur_filter_dict
 
         # Log grid view.
         context = str(self.__class__.__name__)
         params = cur_filter_dict.copy()
-        params['sort'] = sort_key
+        params["sort"] = sort_key
 
         # Render grid.
         def url(*args, **kwargs):
-            route_name = kwargs.pop('__route_name__', None)
+            route_name = kwargs.pop("__route_name__", None)
             # Only include sort/filter arguments if not linking to another
             # page. This is a bit of a hack.
-            if 'action' in kwargs:
+            if "action" in kwargs:
                 new_kwargs = dict()
             else:
                 new_kwargs = dict(extra_url_args)
             # Extend new_kwargs with first argument if found
             if len(args) > 0:
                 new_kwargs.update(args[0])
             new_kwargs.update(kwargs)
             # We need to encode item ids
-            if 'id' in new_kwargs:
-                id = new_kwargs['id']
+            if "id" in new_kwargs:
+                id = new_kwargs["id"]
                 if isinstance(id, list):
-                    new_kwargs['id'] = [trans.security.encode_id(i) for i in id]
+                    new_kwargs["id"] = [trans.security.encode_id(i) for i in id]
                 else:
-                    new_kwargs['id'] = trans.security.encode_id(id)
+                    new_kwargs["id"] = trans.security.encode_id(id)
             # The url_for invocation *must* include a controller and action.
-            if 'controller' not in new_kwargs:
-                new_kwargs['controller'] = trans.controller
-            if 'action' not in new_kwargs:
-                new_kwargs['action'] = trans.action
+            if "controller" not in new_kwargs:
+                new_kwargs["controller"] = trans.controller
+            if "action" not in new_kwargs:
+                new_kwargs["action"] = trans.action
             if route_name:
                 return url_for(route_name, **new_kwargs)
             return url_for(**new_kwargs)
 
-        self.use_panels = (kwargs.get('use_panels', False) in [True, 'True', 'true'])
-        self.advanced_search = (kwargs.get('advanced_search', False) in [True, 'True', 'true'])
+        self.use_panels = kwargs.get("use_panels", False) in [True, "True", "true"]
+        self.advanced_search = kwargs.get("advanced_search", False) in [True, "True", "true"]
         # Currently, filling the template returns a str object; this requires decoding the string into a
         # unicode object within mako templates. What probably should be done is to return the template as
         # utf-8 unicode; however, this would require encoding the object as utf-8 before returning the grid
         # results via a controller method, which is require substantial changes. Hence, for now, return grid
         # as str.
         grid_config = {
-            'title': self.title,
-            'title_id': getattr(self, "title_id", None),
-            'url_base': trans.request.path_url,
-            'async_ops': [],
-            'categorical_filters': {},
-            'filters': cur_filter_dict,
-            'sort_key': sort_key,
-            'show_item_checkboxes': self.show_item_checkboxes or kwargs.get('show_item_checkboxes', '') in ['True', 'true'],
-            'cur_page_num': page_num,
-            'num_page_links': self.num_page_links,
-            'status': status,
-            'message': restore_text(message),
-            'global_actions': [],
-            'operations': [],
-            'items': [],
-            'columns': [],
-            'model_class': str(self.model_class),
-            'use_paging': self.use_paging,
-            'legend': self.legend,
-            'current_item_id': False,
-            'use_hide_message': self.use_hide_message,
-            'default_filter_dict': self.default_filter,
-            'advanced_search': self.advanced_search,
-            'info_text': self.info_text,
-            'url': url(dict()),
-            'refresh_frames': kwargs.get('refresh_frames', [])
+            "title": self.title,
+            "title_id": getattr(self, "title_id", None),
+            "url_base": trans.request.path_url,
+            "async_ops": [],
+            "categorical_filters": {},
+            "filters": cur_filter_dict,
+            "sort_key": sort_key,
+            "show_item_checkboxes": self.show_item_checkboxes
+            or kwargs.get("show_item_checkboxes", "") in ["True", "true"],
+            "cur_page_num": page_num,
+            "num_page_links": self.num_page_links,
+            "status": status,
+            "message": restore_text(message),
+            "global_actions": [],
+            "operations": [],
+            "items": [],
+            "columns": [],
+            "model_class": str(self.model_class),
+            "use_paging": self.use_paging,
+            "legend": self.legend,
+            "current_item_id": False,
+            "use_hide_message": self.use_hide_message,
+            "default_filter_dict": self.default_filter,
+            "advanced_search": self.advanced_search,
+            "info_text": self.info_text,
+            "url": url(dict()),
+            "refresh_frames": kwargs.get("refresh_frames", []),
         }
         if current_item:
-            grid_config['current_item_id'] = current_item.id
+            grid_config["current_item_id"] = current_item.id
         for column in self.columns:
-            extra = ''
+            extra = ""
             if column.sortable:
                 if sort_key.endswith(column.key):
                     if not sort_key.startswith("-"):
                         extra = "&darr;"
                     else:
                         extra = "&uarr;"
-            grid_config['columns'].append({
-                'key': column.key,
-                'visible': column.visible,
-                'nowrap': column.nowrap,
-                'attach_popup': column.attach_popup,
-                'label_id_prefix': column.label_id_prefix,
-                'sortable': column.sortable,
-                'label': column.label,
-                'filterable': column.filterable,
-                'delayed': column.delayed,
-                'is_text': isinstance(column, TextColumn),
-                'extra': extra
-            })
+            grid_config["columns"].append(
+                {
+                    "key": column.key,
+                    "visible": column.visible,
+                    "nowrap": column.nowrap,
+                    "attach_popup": column.attach_popup,
+                    "label_id_prefix": column.label_id_prefix,
+                    "sortable": column.sortable,
+                    "label": column.label,
+                    "filterable": column.filterable,
+                    "delayed": column.delayed,
+                    "is_text": isinstance(column, TextColumn),
+                    "extra": extra,
+                }
+            )
         for operation in self.operations:
-            grid_config['operations'].append({
-                'allow_multiple': operation.allow_multiple,
-                'allow_popup': operation.allow_popup,
-                'target': operation.target,
-                'label': operation.label,
-                'confirm': operation.confirm,
-                'href': url(**operation.url_args) if isinstance(operation.url_args, dict) else None,
-                'global_operation': False
-            })
+            grid_config["operations"].append(
+                {
+                    "allow_multiple": operation.allow_multiple,
+                    "allow_popup": operation.allow_popup,
+                    "target": operation.target,
+                    "label": operation.label,
+                    "confirm": operation.confirm,
+                    "href": url(**operation.url_args) if isinstance(operation.url_args, dict) else None,
+                    "global_operation": False,
+                }
+            )
             if operation.allow_multiple:
-                grid_config['show_item_checkboxes'] = True
+                grid_config["show_item_checkboxes"] = True
             if operation.global_operation:
-                grid_config['global_operation'] = url(** (operation.global_operation()))
+                grid_config["global_operation"] = url(**(operation.global_operation()))
         for action in self.global_actions:
-            grid_config['global_actions'].append({
-                'url_args': url(**action.url_args),
-                'label': action.label,
-                'target': action.target
-            })
+            grid_config["global_actions"].append(
+                {"url_args": url(**action.url_args), "label": action.label, "target": action.target}
+            )
         for operation in [op for op in self.operations if op.async_compatible]:
-            grid_config['async_ops'].append(operation.label.lower())
+            grid_config["async_ops"].append(operation.label.lower())
         for column in self.columns:
             if column.filterable is not None and not isinstance(column, TextColumn):
-                grid_config['categorical_filters'][column.key] = {filter.label: filter.args for filter in column.get_accepted_filters()}
+                grid_config["categorical_filters"][column.key] = {
+                    filter.label: filter.args for filter in column.get_accepted_filters()
+                }
         for item in query:
             item_dict = {
-                'id': item.id,
-                'encode_id': trans.security.encode_id(item.id),
-                'link': [],
-                'operation_config': {},
-                'column_config': {}
+                "id": item.id,
+                "encode_id": trans.security.encode_id(item.id),
+                "link": [],
+                "operation_config": {},
+                "column_config": {},
             }
             for column in self.columns:
                 if column.visible:
                     link = column.get_link(trans, self, item)
                     if link:
                         link = url(**link)
                     else:
                         link = None
                     target = column.target
                     value = unicodify(column.get_value(trans, self, item))
                     if value:
-                        value = value.replace('/', '//')
-                    item_dict['column_config'][column.label] = {
-                        'link': link,
-                        'value': value,
-                        'target': target
-                    }
+                        value = value.replace("/", "//")
+                    item_dict["column_config"][column.label] = {"link": link, "value": value, "target": target}
             for operation in self.operations:
-                item_dict['operation_config'][operation.label] = {
-                    'allowed': operation.allowed(item),
-                    'url_args': url(**operation.get_url_args(item)),
-                    'target': operation.target
+                item_dict["operation_config"][operation.label] = {
+                    "allowed": operation.allowed(item),
+                    "url_args": url(**operation.get_url_args(item)),
+                    "target": operation.target,
                 }
-            grid_config['items'].append(item_dict)
+            grid_config["items"].append(item_dict)
 
         if self.use_paging and num_pages is None:
             # TODO: it would be better to just return this as None, render, and fire
             # off a second request for this count I think.
             total_num_rows = total_row_count_query.count()
             num_pages = int(math.ceil(float(total_num_rows) / self.num_rows_per_page))
 
         grid_config["num_pages"] = num_pages
 
         trans.log_action(trans.get_user(), "grid.view", context, params)
         return grid_config
 
     def get_ids(self, **kwargs):
         id = []
-        if 'id' in kwargs:
-            id = kwargs['id']
+        if "id" in kwargs:
+            id = kwargs["id"]
             # Coerce ids to list
             if not isinstance(id, list):
                 id = id.split(",")
             # Ensure ids are integers
             try:
                 id = list(map(int, id))
             except Exception:
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/helpers/tags.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/helpers/tags.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,18 +18,16 @@
     >>> format_attrs(p=2, q=3) == u' p="2" q="3"'
     True
     >>> format_attrs(p=2, q=None) == u' p="2"'
     True
     >>> format_attrs(p=None) == u''
     True
     """
-    strings = [f' {attr}="{escape_silent(value)}"'
-        for attr, value in sorted(attrs.items())
-        if value is not None]
-    return ''.join(strings)
+    strings = [f' {attr}="{escape_silent(value)}"' for attr, value in sorted(attrs.items()) if value is not None]
+    return "".join(strings)
 
 
 def javascript_link(*urls, **attrs):
     """Return script include tags for the specified javascript URLs.
 
     ``urls`` should be the exact URLs desired.  A previous version of this
     helper added magic prefixes; this is no longer the case.
@@ -43,24 +41,24 @@
         <script src="/javascripts/prototype.js" type="text/javascript"></script>
         <script src="/other-javascripts/util.js" type="text/javascript"></script>
 
         >>> print(javascript_link('/app.js', '/test/test.1.js'))
         <script src="/app.js" type="text/javascript"></script>
         <script src="/test/test.1.js" type="text/javascript"></script>
     """
-    if 'defer' in attrs:
-        if attrs['defer']:
-            attrs['defer'] = 'defer'
+    if "defer" in attrs:
+        if attrs["defer"]:
+            attrs["defer"] = "defer"
         else:
-            del attrs['defer']
-    attrs['type'] = 'text/javascript'
-    tag_template = '<script%s></script>'
+            del attrs["defer"]
+    attrs["type"] = "text/javascript"
+    tag_template = "<script%s></script>"
     tags = []
     for url in urls:
-        attrs['src'] = url
+        attrs["src"] = url
         tag = tag_template % format_attrs(**attrs)
         tags.append(tag)
     return "\n".join(tags)
 
 
 def stylesheet_link(*urls, **attrs):
     """Return CSS link tags for the specified stylesheet URLs.
@@ -77,14 +75,14 @@
         <link href="/stylesheets/dir/file.css" media="all" rel="stylesheet" type="text/css" />
     """
     if "href" in attrs:
         raise TypeError("keyword arg 'href' not allowed")
     attrs.setdefault("rel", "stylesheet")
     attrs.setdefault("type", "text/css")
     attrs.setdefault("media", "screen")
-    tag_template = '<link%s />'
+    tag_template = "<link%s />"
     tags = []
     for url in urls:
-        attrs['href'] = url
+        attrs["href"] = url
         tag = tag_template % format_attrs(**attrs)
         tags.append(tag)
     return "\n".join(tags)
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/error.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/error.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,24 +13,28 @@
 import traceback
 from io import StringIO
 from typing import cast
 
 import markupsafe
 from paste import (
     request,
-    wsgilib
+    wsgilib,
+)
+from paste.exceptions import (
+    collector,
+    formatter,
+    reporter,
 )
-from paste.exceptions import collector, formatter, reporter
 
-__all__ = ('ErrorMiddleware', 'handle_exception')
+__all__ = ("ErrorMiddleware", "handle_exception")
 
 
 class _NoDefault:
     def __repr__(self):
-        return '<NoDefault>'
+        return "<NoDefault>"
 
 
 NoDefault = _NoDefault()
 
 
 class ErrorMiddleware:
 
@@ -84,88 +88,93 @@
           (but probably shouldn't be) installed above this middleware,
           and wants to get certain exceptions.  Exceptions raised after
           ``start_response`` have been called are always caught since
           by definition they are no longer expected.
 
     """
 
-    def __init__(self, application, global_conf=None,
-                 debug=NoDefault,
-                 error_email=None,
-                 error_log=None,
-                 show_exceptions_in_wsgi_errors=NoDefault,
-                 from_address=None,
-                 smtp_server=None,
-                 smtp_username=None,
-                 smtp_password=None,
-                 smtp_use_tls=False,
-                 error_subject_prefix=None,
-                 error_message=None,
-                 xmlhttp_key=None):
+    def __init__(
+        self,
+        application,
+        global_conf=None,
+        debug=NoDefault,
+        error_email=None,
+        error_log=None,
+        show_exceptions_in_wsgi_errors=NoDefault,
+        from_address=None,
+        smtp_server=None,
+        smtp_username=None,
+        smtp_password=None,
+        smtp_use_tls=False,
+        error_subject_prefix=None,
+        error_message=None,
+        xmlhttp_key=None,
+    ):
         from paste.util import converters
+
         self.application = application
         # @@: global_conf should be handled elsewhere in a separate
         # function for the entry point
         if global_conf is None:
             global_conf = {}
         if debug is NoDefault:
-            debug = converters.asbool(global_conf.get('debug'))
+            debug = converters.asbool(global_conf.get("debug"))
         if show_exceptions_in_wsgi_errors is NoDefault:
-            show_exceptions_in_wsgi_errors = converters.asbool(global_conf.get('show_exceptions_in_wsgi_errors'))
+            show_exceptions_in_wsgi_errors = converters.asbool(global_conf.get("show_exceptions_in_wsgi_errors"))
         self.debug_mode = converters.asbool(debug)
         if error_email is None:
-            error_email = (global_conf.get('error_email')
-                           or global_conf.get('admin_email')
-                           or global_conf.get('webmaster_email')
-                           or global_conf.get('sysadmin_email'))
+            error_email = (
+                global_conf.get("error_email")
+                or global_conf.get("admin_email")
+                or global_conf.get("webmaster_email")
+                or global_conf.get("sysadmin_email")
+            )
         self.error_email = converters.aslist(error_email)
         self.error_log = error_log
         self.show_exceptions_in_wsgi_errors = show_exceptions_in_wsgi_errors
         if from_address is None:
-            from_address = global_conf.get('error_from_address', 'errors@localhost')
+            from_address = global_conf.get("error_from_address", "errors@localhost")
         self.from_address = from_address
         if smtp_server is None:
-            smtp_server = global_conf.get('smtp_server', 'localhost')
+            smtp_server = global_conf.get("smtp_server", "localhost")
         self.smtp_server = smtp_server
-        self.smtp_username = smtp_username or global_conf.get('smtp_username')
-        self.smtp_password = smtp_password or global_conf.get('smtp_password')
-        self.smtp_use_tls = smtp_use_tls or converters.asbool(global_conf.get('smtp_use_tls'))
-        self.error_subject_prefix = error_subject_prefix or ''
+        self.smtp_username = smtp_username or global_conf.get("smtp_username")
+        self.smtp_password = smtp_password or global_conf.get("smtp_password")
+        self.smtp_use_tls = smtp_use_tls or converters.asbool(global_conf.get("smtp_use_tls"))
+        self.error_subject_prefix = error_subject_prefix or ""
         if error_message is None:
-            error_message = global_conf.get('error_message')
+            error_message = global_conf.get("error_message")
         self.error_message = error_message
         if xmlhttp_key is None:
-            xmlhttp_key = global_conf.get('xmlhttp_key', '_')
+            xmlhttp_key = global_conf.get("xmlhttp_key", "_")
         self.xmlhttp_key = xmlhttp_key
 
     def __call__(self, environ, start_response):
         """
         The WSGI application interface.
         """
         # We want to be careful about not sending headers twice,
         # and the content type that the app has committed to (if there
         # is an exception in the iterator body of the response)
-        if environ.get('paste.throw_errors'):
+        if environ.get("paste.throw_errors"):
             return self.application(environ, start_response)
-        environ['paste.throw_errors'] = True
+        environ["paste.throw_errors"] = True
 
         try:
             __traceback_supplement__ = Supplement, self, environ
             sr_checker = ResponseStartChecker(start_response)
             app_iter = self.application(environ, sr_checker)
             return self.make_catching_iter(app_iter, environ, sr_checker)
         except Exception:
             exc_info = sys.exc_info()
             try:
-                for expect in environ.get('paste.expected_exceptions', []):
+                for expect in environ.get("paste.expected_exceptions", []):
                     if isinstance(exc_info[1], expect):
                         raise
-                start_response('500 Internal Server Error',
-                               [('content-type', 'text/html')],
-                               exc_info)
+                start_response("500 Internal Server Error", [("content-type", "text/html")], exc_info)
                 # @@: it would be nice to deal with bad content types here
                 response = self.exception_handler(exc_info, environ)
                 return [response]
             finally:
                 # clean up locals...
                 exc_info = None
 
@@ -178,29 +187,31 @@
     def exception_handler(self, exc_info, environ):
         simple_html_error = False
         if self.xmlhttp_key:
             get_vars = wsgilib.parse_querystring(environ)
             if dict(get_vars).get(self.xmlhttp_key):
                 simple_html_error = True
         return handle_exception(
-            exc_info, environ['wsgi.errors'],
+            exc_info,
+            environ["wsgi.errors"],
             html=True,
             debug_mode=self.debug_mode,
             error_email=self.error_email,
             error_log=self.error_log,
             show_exceptions_in_wsgi_errors=self.show_exceptions_in_wsgi_errors,
             error_email_from=self.from_address,
             smtp_server=self.smtp_server,
             smtp_username=self.smtp_username,
             smtp_password=self.smtp_password,
             smtp_use_tls=self.smtp_use_tls,
             error_subject_prefix=self.error_subject_prefix,
             error_message=self.error_message,
             simple_html_error=simple_html_error,
-            environ=environ)
+            environ=environ,
+        )
 
 
 class ResponseStartChecker:
     def __init__(self, start_response):
         self.start_response = start_response
         self.response_started = False
 
@@ -227,16 +238,15 @@
         self.error_middleware = error_middleware
         self.closed = False
 
     def __iter__(self):
         return self
 
     def __next__(self):
-        __traceback_supplement__ = (
-            Supplement, self.error_middleware, self.environ)
+        __traceback_supplement__ = (Supplement, self.error_middleware, self.environ)
         if self.closed:
             raise StopIteration
         try:
             return next(self.app_iterator)
         except StopIteration:
             self.closed = True
             close_response = self._close()
@@ -244,43 +254,38 @@
                 return close_response
             else:
                 raise StopIteration
         except Exception:
             self.closed = True
             close_response = self._close()
             exc_info = sys.exc_info()
-            response = self.error_middleware.exception_handler(
-                exc_info, self.environ)
+            response = self.error_middleware.exception_handler(exc_info, self.environ)
             if close_response is not None:
-                response += (
-                    f'<hr noshade>Error in .close():<br>{close_response}')
+                response += f"<hr noshade>Error in .close():<br>{close_response}"
 
             if not self.start_checker.response_started:
-                self.start_checker('500 Internal Server Error',
-                                   [('content-type', 'text/html')],
-                                   exc_info)
+                self.start_checker("500 Internal Server Error", [("content-type", "text/html")], exc_info)
 
             return response
 
     def close(self):
         # This should at least print something to stderr if the
         # close method fails at this point
         if not self.closed:
             self._close()
 
     def _close(self):
         """Close and return any error message"""
-        if not hasattr(self.app_iterable, 'close'):
+        if not hasattr(self.app_iterable, "close"):
             return None
         try:
             self.app_iterable.close()
             return None
         except Exception:
-            close_response = self.error_middleware.exception_handler(
-                sys.exc_info(), self.environ)
+            close_response = self.error_middleware.exception_handler(sys.exc_info(), self.environ)
             return close_response
 
 
 class Supplement:
 
     """
     This is a supplement used to display standard WSGI information in
@@ -290,67 +295,74 @@
     def __init__(self, middleware, environ):
         self.middleware = middleware
         self.environ = environ
         self.source_url = request.construct_url(environ)
 
     def extraData(self):
         data = {}
-        cgi_vars = data[('extra', 'CGI Variables')] = {}
-        wsgi_vars = data[('extra', 'WSGI Variables')] = {}
-        hide_vars = ['paste.config', 'wsgi.errors', 'wsgi.input',
-                     'wsgi.multithread', 'wsgi.multiprocess',
-                     'wsgi.run_once', 'wsgi.version',
-                     'wsgi.url_scheme']
+        cgi_vars = data[("extra", "CGI Variables")] = {}
+        wsgi_vars = data[("extra", "WSGI Variables")] = {}
+        hide_vars = [
+            "paste.config",
+            "wsgi.errors",
+            "wsgi.input",
+            "wsgi.multithread",
+            "wsgi.multiprocess",
+            "wsgi.run_once",
+            "wsgi.version",
+            "wsgi.url_scheme",
+        ]
         for name, value in self.environ.items():
             if name.upper() == name:
                 if value:
                     cgi_vars[name] = value
             elif name not in hide_vars:
                 wsgi_vars[name] = value
-        if self.environ['wsgi.version'] != (1, 0):
-            wsgi_vars['wsgi.version'] = self.environ['wsgi.version']
-        proc_desc = tuple(int(bool(self.environ[key])) for key in (
-            'wsgi.multiprocess',
-            'wsgi.multithread',
-            'wsgi.run_once'
-        ))
-        wsgi_vars['wsgi process'] = self.process_combos[proc_desc]
-        wsgi_vars['application'] = self.middleware.application
-        if 'paste.config' in self.environ:
-            data[('extra', 'Configuration')] = dict(self.environ['paste.config'])
+        if self.environ["wsgi.version"] != (1, 0):
+            wsgi_vars["wsgi.version"] = self.environ["wsgi.version"]
+        proc_desc = tuple(
+            int(bool(self.environ[key])) for key in ("wsgi.multiprocess", "wsgi.multithread", "wsgi.run_once")
+        )
+        wsgi_vars["wsgi process"] = self.process_combos[proc_desc]
+        wsgi_vars["application"] = self.middleware.application
+        if "paste.config" in self.environ:
+            data[("extra", "Configuration")] = dict(self.environ["paste.config"])
         return data
 
     process_combos = {
         # multiprocess, multithread, run_once
-        (0, 0, 0): 'Non-concurrent server',
-        (0, 1, 0): 'Multithreaded',
-        (1, 0, 0): 'Multiprocess',
-        (1, 1, 0): 'Multi process AND threads (?)',
-        (0, 0, 1): 'Non-concurrent CGI',
-        (0, 1, 1): 'Multithread CGI (?)',
-        (1, 0, 1): 'CGI',
-        (1, 1, 1): 'Multi thread/process CGI (?)',
+        (0, 0, 0): "Non-concurrent server",
+        (0, 1, 0): "Multithreaded",
+        (1, 0, 0): "Multiprocess",
+        (1, 1, 0): "Multi process AND threads (?)",
+        (0, 0, 1): "Non-concurrent CGI",
+        (0, 1, 1): "Multithread CGI (?)",
+        (1, 0, 1): "CGI",
+        (1, 1, 1): "Multi thread/process CGI (?)",
     }
 
 
-def handle_exception(exc_info, error_stream, html=True,
-                     debug_mode=False,
-                     error_email=None,
-                     error_log=None,
-                     show_exceptions_in_wsgi_errors=False,
-                     error_email_from='errors@localhost',
-                     smtp_server='localhost',
-                     smtp_username=None,
-                     smtp_password=None,
-                     smtp_use_tls=False,
-                     error_subject_prefix='',
-                     error_message=None,
-                     simple_html_error=False,
-                     environ=None
-                     ):
+def handle_exception(
+    exc_info,
+    error_stream,
+    html=True,
+    debug_mode=False,
+    error_email=None,
+    error_log=None,
+    show_exceptions_in_wsgi_errors=False,
+    error_email_from="errors@localhost",
+    smtp_server="localhost",
+    smtp_username=None,
+    smtp_password=None,
+    smtp_use_tls=False,
+    error_subject_prefix="",
+    error_message=None,
+    simple_html_error=False,
+    environ=None,
+):
     """
     For exception handling outside of a web context
 
     Use like::
 
         import sys
         from paste.exceptions.errormiddleware import handle_exception
@@ -362,74 +374,71 @@
 
     If you want to report, but not fully catch the exception, call
     ``raise`` after ``handle_exception``, which (when given no argument)
     will reraise the exception.
     """
     reported = False
     exc_data = collector.collect_exception(*exc_info)
-    extra_data = ''
+    extra_data = ""
     if error_email:
         rep = reporter.EmailReporter(
             to_addresses=error_email,
             from_address=error_email_from,
             smtp_server=smtp_server,
             smtp_username=smtp_username,
             smtp_password=smtp_password,
             smtp_use_tls=smtp_use_tls,
-            subject_prefix=error_subject_prefix)
+            subject_prefix=error_subject_prefix,
+        )
         rep_err = send_report(rep, exc_data, html=html)
         if rep_err:
             extra_data += rep_err
         else:
             reported = True
     if error_log:
-        rep = reporter.LogReporter(
-            filename=error_log)
+        rep = reporter.LogReporter(filename=error_log)
         rep_err = send_report(rep, exc_data, html=html)
         if rep_err:
             extra_data += rep_err
         else:
             reported = True
     if show_exceptions_in_wsgi_errors:
-        rep = reporter.FileReporter(
-            file=error_stream)
+        rep = reporter.FileReporter(file=error_stream)
         rep_err = send_report(rep, exc_data, html=html)
         if rep_err:
             extra_data += rep_err
         else:
             reported = True
     else:
-        error_stream.write('Error - {}: {}\n'.format(
-            exc_data.exception_type, exc_data.exception_value))
+        error_stream.write(f"Error - {exc_data.exception_type}: {exc_data.exception_value}\n")
     if html:
         if debug_mode and simple_html_error:
             return_error = formatter.format_html(
-                exc_data, include_hidden_frames=False,
-                include_reusable=False, show_extra_data=False)
+                exc_data, include_hidden_frames=False, include_reusable=False, show_extra_data=False
+            )
             reported = True
         elif debug_mode and not simple_html_error:
-            error_html = formatter.format_html(
-                exc_data,
-                include_hidden_frames=True,
-                include_reusable=False)
+            error_html = formatter.format_html(exc_data, include_hidden_frames=True, include_reusable=False)
             head_html = formatter.error_css + formatter.hide_display_js
-            return_error = error_template(
-                head_html, error_html, extra_data)
-            extra_data = ''
+            return_error = error_template(head_html, error_html, extra_data)
+            extra_data = ""
             reported = True
         else:
-            msg = error_message or '''
+            msg = (
+                error_message
+                or """
             An error occurred.
-            '''
+            """
+            )
             extra = "<p><b>The error has been logged to our team.</b>"
-            if 'sentry_event_id' in environ:
+            if "sentry_event_id" in environ:
                 extra += " If you want to contact us about this error, please reference the following<br><br>"
                 extra += f"<b><large>GURU MEDITATION: #{environ['sentry_event_id']}</large></b>"
             extra += "</p>"
-            return_error = error_template('', msg, extra)
+            return_error = error_template("", msg, extra)
     else:
         return_error = None
     if not reported and error_stream:
         err_report = formatter.format_text(exc_data, show_hidden_frames=True)
         err_report += f"\n{'-' * 60}\n"
         error_stream.write(err_report)
     if extra_data:
@@ -445,25 +454,24 @@
         traceback.print_exc(file=output)
         if html:
             return """
             <p>Additionally an error occurred while sending the {} report:
 
             <pre>{}</pre>
             </p>""".format(
-                markupsafe.escape(str(rep)), output.getvalue())
+                markupsafe.escape(str(rep)), output.getvalue()
+            )
         else:
-            return (
-                "Additionally an error occurred while sending the "
-                "%s report:\n%s" % (str(rep), output.getvalue()))
+            return "Additionally an error occurred while sending the " "%s report:\n%s" % (str(rep), output.getvalue())
     else:
-        return ''
+        return ""
 
 
 def error_template(head_html, exception, extra):
-    return '''
+    return """
     <!DOCTYPE HTML>
     <html>
     <head>
     <style type="text/css">
     body {{ color: #303030; background: #dfe5f9; font-family:"Lucida Grande",verdana,arial,helvetica,sans-serif; font-size:12px; line-height:16px; }}
     .content {{ max-width: 720px; margin: auto; margin-top: 50px; }}
     </style>
@@ -479,20 +487,22 @@
     <p>{}</p>
 
     This may be an intermittent problem due to load or other unpredictable factors, reloading the page may address the problem.
 
     {}
     </div>
     </body>
-    </html>'''.format(head_html, exception, extra)
+    </html>""".format(
+        head_html, exception, extra
+    )
 
 
 def make_error_middleware(app, global_conf, **kw):
     return ErrorMiddleware(app, global_conf=global_conf, **kw)
 
 
 doc_lines = cast(str, ErrorMiddleware.__doc__).splitlines(True)
 for i in range(len(doc_lines)):
-    if doc_lines[i].strip().startswith('Settings'):
-        make_error_middleware.__doc__ = ''.join(doc_lines[i:])
+    if doc_lines[i].strip().startswith("Settings"):
+        make_error_middleware.__doc__ = "".join(doc_lines[i:])
         break
 del i, doc_lines
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/profile.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/profile.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 import cProfile
 import pstats
 import threading
 
 import markupsafe
 from paste import response
 
-
 template = """
 <script>
 function show_profile_output()
 {
 var win = window.open("", "win"); // a window object
 var doc = win.document;
 doc.open("text/html", "replace");
@@ -59,57 +58,62 @@
         def replace_start_response(status, headers, exc_info=None):
             catch_response.extend([status, headers])
             start_response(status, headers, exc_info)
             return body.append
 
         def run_app():
             body.extend(self.app(environ, replace_start_response))
+
         # Run in profiler
         prof = cProfile.Profile()
         prof.runctx("run_app()", globals(), locals())
         # Build up body with stats
-        body = ''.join(body)
+        body = "".join(body)
         headers = catch_response[1]
-        content_type = response.header_value(headers, 'content-type')
-        if not content_type.startswith('text/html'):
+        content_type = response.header_value(headers, "content-type")
+        if not content_type.startswith("text/html"):
             # We can't add info to non-HTML output
             return [body]
         stats = pstats.Stats(prof)
         stats.strip_dirs()
-        stats.sort_stats('time', 'calls')
+        stats.sort_stats("time", "calls")
         output = pstats_as_html(stats, self.limit)
         body += template % output
         return [body]
 
 
 def pstats_as_html(stats, *sel_list):
     """
     Return an HTML representation of a pstats.Stats object.
     """
     rval = []
     # Number of function calls, primitive calls, total time
-    rval.append("<div>%d function calls (%d primitive) in %0.3f CPU seconds</div>"
-                % (stats.total_calls, stats.prim_calls, stats.total_tt))
+    rval.append(
+        "<div>%d function calls (%d primitive) in %0.3f CPU seconds</div>"
+        % (stats.total_calls, stats.prim_calls, stats.total_tt)
+    )
     # Extract functions that match 'sel_list'
     funcs, order_message, select_message = get_func_list(stats, sel_list)
     # Deal with any ordering or selection messages
     if order_message:
         rval.append(f"<div>{markupsafe.escape(order_message)}</div>")
     if select_message:
         rval.append(f"<div>{markupsafe.escape(select_message)}</div>")
     # Build a table for the functions
-    if list:
+    if funcs:
         rval.append("<table>")
         # Header
-        rval.append("<tr><th>ncalls</th>"
-                    "<th>tottime</th>"
-                    "<th>percall</th>"
-                    "<th>cumtime</th>"
-                    "<th>percall</th>"
-                    "<th>filename:lineno(function)</th></tr>")
+        rval.append(
+            "<tr><th>ncalls</th>"
+            "<th>tottime</th>"
+            "<th>percall</th>"
+            "<th>cumtime</th>"
+            "<th>percall</th>"
+            "<th>filename:lineno(function)</th></tr>"
+        )
         for func in funcs:
             rval.append("<tr>")
             # Calculate each field
             cc, nc, tt, ct, callers = stats.stats[func]
             # ncalls
             ncalls = str(nc)
             if nc != cc:
@@ -159,16 +163,16 @@
     return list, order_message, select_message
 
 
 def func_std_string(func_name):
     """
     Match what old profile produced
     """
-    if func_name[:2] == ('~', 0):
+    if func_name[:2] == ("~", 0):
         # special case for built-in functions
         name = func_name[2]
-        if name.startswith('<') and name.endswith('>'):
-            return '{%s}' % name[1:-1]
+        if name.startswith("<") and name.endswith(">"):
+            return "{%s}" % name[1:-1]
         else:
             return name
     else:
         return "%s:%d(%s)" % func_name
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/remoteuser.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/remoteuser.py`

 * *Files 8% similar despite different names*

```diff
@@ -37,62 +37,73 @@
         </div>
     </body>
 </html>
 """
 
 
 class RemoteUser:
-
-    def __init__(self, app, maildomain=None, display_servers=None, admin_users=None,
-                 single_user=None, remote_user_header=None, remote_user_secret_header=None,
-                 normalize_remote_user_email=False):
+    def __init__(
+        self,
+        app,
+        maildomain=None,
+        display_servers=None,
+        admin_users=None,
+        single_user=None,
+        remote_user_header=None,
+        remote_user_secret_header=None,
+        normalize_remote_user_email=False,
+    ):
         self.app = app
         self.maildomain = maildomain
         self.display_servers = display_servers or []
         self.admin_users = admin_users or []
-        self.remote_user_header = remote_user_header or 'HTTP_REMOTE_USER'
+        self.remote_user_header = remote_user_header or "HTTP_REMOTE_USER"
         self.single_user = single_user
         self.config_secret_header = remote_user_secret_header
         self.normalize_remote_user_email = normalize_remote_user_email
 
     def __call__(self, environ, start_response):
         # Allow display servers
-        if self.display_servers and 'REMOTE_ADDR' in environ:
+        if self.display_servers and "REMOTE_ADDR" in environ:
             try:
-                host = socket.gethostbyaddr(environ['REMOTE_ADDR'])[0]
-            except(OSError, socket.herror, socket.gaierror, socket.timeout):
+                host = socket.gethostbyaddr(environ["REMOTE_ADDR"])[0]
+            except (OSError, socket.herror, socket.gaierror, socket.timeout):
                 # in the event of a lookup failure, deny access
                 host = None
             if host in self.display_servers:
-                environ[self.remote_user_header] = 'remote_display_server@%s' % (self.maildomain or 'example.org')
+                environ[self.remote_user_header] = "remote_display_server@%s" % (self.maildomain or "example.org")
                 return self.app(environ, start_response)
 
         if self.single_user:
             assert self.remote_user_header not in environ
             environ[self.remote_user_header] = self.single_user
 
-        if environ.get(self.remote_user_header, '').startswith('(null)'):
+        if environ.get(self.remote_user_header, "").startswith("(null)"):
             # Throw away garbage headers.
             # Apache sets REMOTE_USER to the string '(null)' when using the
             # Rewrite* method for passing REMOTE_USER and a user is not authenticated.
             # Any other possible values need to go here as well.
-            log.debug("Discarding invalid remote user header %s:%s.", self.remote_user_header, environ.get(self.remote_user_header, None))
+            log.debug(
+                "Discarding invalid remote user header %s:%s.",
+                self.remote_user_header,
+                environ.get(self.remote_user_header, None),
+            )
             environ.pop(self.remote_user_header)
         if self.remote_user_header in environ:
             # process remote user with configuration options.
             if self.normalize_remote_user_email:
                 environ[self.remote_user_header] = environ[self.remote_user_header].lower()
-            if self.maildomain and '@' not in environ[self.remote_user_header]:
+            if self.maildomain and "@" not in environ[self.remote_user_header]:
                 environ[self.remote_user_header] = f"{environ[self.remote_user_header]}@{self.maildomain}"
 
-        path_info = environ.get('PATH_INFO', '')
+        path_info = environ.get("PATH_INFO", "")
 
         # The API handles its own authentication via keys
         # Check for API key before checking for header
-        if path_info.startswith('/api/'):
+        if path_info.startswith("/api/"):
             return self.app(environ, start_response)
 
         # If the secret header is enabled, we expect upstream to send along some key
         # in HTTP_GX_SECRET, so we'll need to compare that here to the correct value
         #
         # This is not an ideal location for this function.  The reason being
         # that because this check is done BEFORE the REMOTE_USER check,  it is
@@ -100,43 +111,43 @@
         # credentials. However, that's why it's not "ideal", but it is "good
         # enough". The only users able to exploit this are ones with access to
         # the local system (unless Galaxy is listening on 0.0.0.0....). It
         # seems improbable that an attacker with access to the server hosting
         # Galaxy would not have access to Galaxy itself, and be attempting to
         # attack the system
         if self.config_secret_header is not None:
-            if environ.get('HTTP_GX_SECRET') is None:
+            if environ.get("HTTP_GX_SECRET") is None:
                 title = "Access to Galaxy is denied"
                 message = """
                 Galaxy is configured to authenticate users via an external
                 method (such as HTTP authentication in Apache), but
                 no shared secret key was provided by the
                 upstream (proxy) server.</p>
                 <p>Please contact your local Galaxy administrator.  The
                 variable <code>remote_user_secret</code> and
                 <code>GX_SECRET</code> header must be set before you may
                 access Galaxy.
                 """
                 return self.error(start_response, title, message)
-            if not safe_str_cmp(environ.get('HTTP_GX_SECRET', ''), self.config_secret_header):
+            if not safe_str_cmp(environ.get("HTTP_GX_SECRET", ""), self.config_secret_header):
                 title = "Access to Galaxy is denied"
                 message = """
                 Galaxy is configured to authenticate users via an external
                 method (such as HTTP authentication in Apache), but an
                 incorrect shared secret key was provided by the
                 upstream (proxy) server.</p>
                 <p>Please contact your local Galaxy administrator.  The
                 variable <code>remote_user_secret</code> and
                 <code>GX_SECRET</code> header must be set before you may
                 access Galaxy.
                 """
                 return self.error(start_response, title, message)
 
         if environ.get(self.remote_user_header, None):
-            if not environ[self.remote_user_header].count('@'):
+            if not environ[self.remote_user_header].count("@"):
                 if self.maildomain is not None:
                     environ[self.remote_user_header] += f"@{self.maildomain}"
                 else:
                     title = "Access to Galaxy is denied"
                     message = """
                         Galaxy is configured to authenticate users via an external
                         method (such as HTTP authentication in Apache), but only a
@@ -145,46 +156,47 @@
                         addresses, a default mail domain must be set.</p>
                         <p>Please contact your local Galaxy administrator.  The
                         variable <code>remote_user_maildomain</code> must be set
                         before you may access Galaxy.
                     """
                     return self.error(start_response, title, message)
             user_accessible_paths = (
-                '/users',
-                '/user/api_key',
-                '/user/edit_username',
-                '/user/dbkeys',
-                '/user/logout',
-                '/user/toolbox_filters',
-                '/user/set_default_permissions',
+                "/users",
+                "/user/api_key",
+                "/user/edit_username",
+                "/user/dbkeys",
+                "/user/logout",
+                "/user/toolbox_filters",
+                "/user/set_default_permissions",
             )
 
             admin_accessible_paths = (
-                '/user/create',
-                '/user/logout',
-                '/user/manage_user_info',
-                '/user/edit_info',
-                '/userskeys/all_users',
-                '/userskeys/admin_api_keys',
+                "/user/create",
+                "/user/logout",
+                "/user/manage_user_info",
+                "/user/edit_info",
+                "/userskeys/all_users",
+                "/userskeys/admin_api_keys",
             )
 
-            if not path_info.startswith('/user'):
+            if not path_info.startswith("/user"):
                 # shortcut the following allowlist for non-user-controller
                 # requests.
                 pass
-            elif environ[self.remote_user_header] in self.admin_users and \
-                    any(path_info.startswith(prefix) for prefix in admin_accessible_paths):
+            elif environ[self.remote_user_header] in self.admin_users and any(
+                path_info.startswith(prefix) for prefix in admin_accessible_paths
+            ):
                 # If the user is an admin user, and any of the admin accessible paths match..., allow them to execute that action.
                 pass
             elif any(path_info.startswith(prefix) for prefix in user_accessible_paths):
                 # If the user is allowed to access the path, pass
                 pass
-            elif path_info == '/user' or path_info == '/user/':
+            elif path_info == "/user" or path_info == "/user/":
                 pass  # We do allow access to the root user preferences page.
-            elif path_info.startswith('/user'):
+            elif path_info.startswith("/user"):
                 # Any other endpoint in the user controller is off limits
                 title = "Access to Galaxy user controls is disabled"
                 message = """
                     User controls are disabled when Galaxy is configured
                     for external authentication.
                 """
                 return self.error(start_response, title, message)
@@ -201,9 +213,9 @@
                 was not provided by the upstream (proxy) server.  This is
                 generally due to a misconfiguration in the upstream server.</p>
                 <p>Please contact your local Galaxy administrator.
             """
             return self.error(start_response, title, message)
 
     def error(self, start_response, title="Access denied", message="Please contact your local Galaxy administrator."):
-        start_response('403 Forbidden', [('Content-type', 'text/html')])
+        start_response("403 Forbidden", [("Content-type", "text/html")])
         return [errorpage % (title, message)]
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/sqldebug.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/sqldebug.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 """
 Per-request SQL debugging middleware.
 """
 import logging
 
-from galaxy.model.orm.engine_factory import log_request_query_counts, reset_request_query_counts
+from galaxy.model.orm.engine_factory import (
+    log_request_query_counts,
+    reset_request_query_counts,
+)
 
 log = logging.getLogger(__name__)
 
 
 class SQLDebugMiddleware:
-
     def __init__(self, application, galaxy, config=None):
         #: the wrapped webapp
         self.application = application
 
     def __call__(self, environ, start_response):
-        query_string = environ.get('QUERY_STRING')
+        query_string = environ.get("QUERY_STRING")
         if "sql_debug=1" in query_string:
             import galaxy.app
+
             if galaxy.app.app.model.thread_local_log:
                 galaxy.app.app.model.thread_local_log.log = True
 
         try:
             reset_request_query_counts()
             return self.application(environ, start_response)
         finally:
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/static.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/static.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,69 @@
 import os
-from typing import List, Tuple
+from typing import (
+    List,
+    Tuple,
+)
 
 from paste import request
 from paste.fileapp import FileApp
 from paste.httpheaders import ETAG
 from paste.urlparser import StaticURLParser
 
 
 class CacheableStaticURLParser(StaticURLParser):
-
     def __init__(self, directory, cache_seconds=None, directory_per_host=None):
         StaticURLParser.__init__(self, directory)
         self.cache_seconds = cache_seconds
         self.directory_per_host = directory_per_host
 
     def __call__(self, environ, start_response):
-        path_info = environ.get('PATH_INFO', '')
+        path_info = environ.get("PATH_INFO", "")
         if not path_info:
             # See if this is a static file hackishly mapped.
             if os.path.exists(self.directory) and os.path.isfile(self.directory):
                 app = FileApp(self.directory)
                 if self.cache_seconds:
                     app.cache_control(max_age=int(self.cache_seconds))
                 return app(environ, start_response)
             return self.add_slash(environ, start_response)
-        if path_info == '/':
+        if path_info == "/":
             # @@: This should obviously be configurable
-            filename = 'index.html'
+            filename = "index.html"
         else:
             filename = request.path_info_pop(environ)
 
         directory = self.directory
-        host = environ.get('HTTP_HOST')
+        host = environ.get("HTTP_HOST")
         if self.directory_per_host and host:
             for host_key, host_val in self.directory_per_host.items():
                 if host_key in host:
                     directory = host_val
                     break
 
-        full = os.path.join(directory, filename)
+        full = self.normpath(os.path.join(directory, filename))
+        if not full.startswith(directory):
+            # Out of bounds
+            return self.not_found(environ, start_response)
+
         if not os.path.exists(full):
             return self.not_found(environ, start_response)
         if os.path.isdir(full):
             # @@: Cache?
             return self.__class__(full)(environ, start_response)
-        if environ.get('PATH_INFO') and environ.get('PATH_INFO') != '/':
+        if environ.get("PATH_INFO") and environ.get("PATH_INFO") != "/":
             return self.error_extra_path(environ, start_response)
-        if_none_match = environ.get('HTTP_IF_NONE_MATCH')
+        if_none_match = environ.get("HTTP_IF_NONE_MATCH")
         if if_none_match:
             mytime = os.stat(full).st_mtime
             if str(mytime) == if_none_match:
                 headers: List[Tuple[str, str]] = []
                 ETAG.update(headers, mytime)
-                start_response('304 Not Modified', headers)
-                return ['']  # empty body
+                start_response("304 Not Modified", headers)
+                return [""]  # empty body
         app = FileApp(full)
         if self.cache_seconds:
             app.cache_control(max_age=int(self.cache_seconds))
         return app(environ, start_response)
 
 
 def make_static(global_conf, document_root, cache_seconds=None):
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/statsd.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/statsd.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,37 +10,33 @@
 
 class StatsdMiddleware:
     """
     This middleware will log request durations to the configured statsd
     instance.
     """
 
-    def __init__(self,
-                 application,
-                 statsd_host,
-                 statsd_port,
-                 statsd_prefix,
-                 statsd_influxdb,
-                 statsd_mock_calls):
+    def __init__(self, application, statsd_host, statsd_port, statsd_prefix, statsd_influxdb, statsd_mock_calls):
         self.application = application
         self.galaxy_stasd_client = GalaxyStatsdClient(
             statsd_host,
             statsd_port,
             statsd_prefix,
             statsd_influxdb,
             statsd_mock_calls,
         )
 
     def __call__(self, environ, start_response):
         start_time = time.time()
         req = self.application(environ, start_response)
         dt = int((time.time() - start_time) * 1000)
-        page = environ.get('controller_action_key', None) or environ.get('PATH_INFO', "NOPATH").strip('/').replace('/', '.')
+        page = environ.get("controller_action_key", None) or environ.get("PATH_INFO", "NOPATH").strip("/").replace(
+            "/", "."
+        )
         self.galaxy_stasd_client.timing(page, dt)
         try:
             times = QUERY_COUNT_LOCAL.times
-            self.galaxy_stasd_client.timing(f"sql.{page}", sum(times) * 1000.)
+            self.galaxy_stasd_client.timing(f"sql.{page}", sum(times) * 1000.0)
             self.galaxy_stasd_client.incr(f"sqlqueries.{page}", len(times))
         except AttributeError:
             # Not logging query counts, skip
             pass
         return req
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/translogger.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/translogger.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,106 +14,115 @@
     They are, by default, sent to a logger named ``'wsgi'`` at the
     INFO level.
 
     If ``setup_console_handler`` is true, then messages for the named
     logger will be sent to the console.
     """
 
-    format = ('%(REMOTE_ADDR)s - %(REMOTE_USER)s [%(time)s] '
-              '"%(REQUEST_METHOD)s %(REQUEST_URI)s %(HTTP_VERSION)s" '
-              '%(status)s %(bytes)s "%(HTTP_REFERER)s" "%(HTTP_USER_AGENT)s"')
-
-    def __init__(self, application,
-                 logger=None,
-                 format=None,
-                 logging_level=logging.INFO,
-                 logger_name='wsgi',
-                 setup_console_handler=True,
-                 set_logger_level=logging.DEBUG):
+    format = (
+        "%(REMOTE_ADDR)s - %(REMOTE_USER)s [%(time)s] "
+        '"%(REQUEST_METHOD)s %(REQUEST_URI)s %(HTTP_VERSION)s" '
+        '%(status)s %(bytes)s "%(HTTP_REFERER)s" "%(HTTP_USER_AGENT)s"'
+    )
+
+    def __init__(
+        self,
+        application,
+        logger=None,
+        format=None,
+        logging_level=logging.INFO,
+        logger_name="wsgi",
+        setup_console_handler=True,
+        set_logger_level=logging.DEBUG,
+    ):
         if format is not None:
             self.format = format
         self.application = application
         self.logging_level = logging_level
         self.logger_name = logger_name
         if logger is None:
             self.logger = logging.getLogger(self.logger_name)
             if setup_console_handler:
                 console = logging.StreamHandler()
                 console.setLevel(logging.DEBUG)
                 # We need to control the exact format:
-                console.setFormatter(logging.Formatter('%(message)s'))
+                console.setFormatter(logging.Formatter("%(message)s"))
                 self.logger.addHandler(console)
                 self.logger.propagate = False
             if set_logger_level is not None:
                 self.logger.setLevel(set_logger_level)
         else:
             self.logger = logger
 
     def __call__(self, environ, start_response):
         start = time.localtime()
-        req_uri = quote(environ.get('SCRIPT_NAME', '')
-                        + environ.get('PATH_INFO', ''))
-        if environ.get('QUERY_STRING'):
+        req_uri = quote(environ.get("SCRIPT_NAME", "") + environ.get("PATH_INFO", ""))
+        if environ.get("QUERY_STRING"):
             req_uri += f"?{environ['QUERY_STRING']}"
-        method = environ['REQUEST_METHOD']
+        method = environ["REQUEST_METHOD"]
 
         def replacement_start_response(status, headers, exc_info=None):
             # @@: Ideally we would count the bytes going by if no
             # content-length header was provided; but that does add
             # some overhead, so at least for now we'll be lazy.
             bytes = None
             for name, value in headers:
-                if name.lower() == 'content-length':
+                if name.lower() == "content-length":
                     bytes = value
             self.write_log(environ, method, req_uri, start, status, bytes)
             return start_response(status, headers, exc_info)
+
         return self.application(environ, replacement_start_response)
 
     def write_log(self, environ, method, req_uri, start, status, bytes):
         if bytes is None:
-            bytes = '-'
+            bytes = "-"
         if time.daylight:
             offset = time.altzone / 60 / 60 * -100
         else:
             offset = time.timezone / 60 / 60 * -100
         if offset >= 0:
             offset = "+%0.4d" % (offset)
         elif offset < 0:
             offset = "%0.4d" % (offset)
         d = {
-            'REMOTE_ADDR': environ.get('REMOTE_ADDR') or '-',
-            'REMOTE_USER': environ.get('REMOTE_USER') or '-',
-            'REQUEST_METHOD': method,
-            'REQUEST_URI': req_uri,
-            'HTTP_VERSION': environ.get('SERVER_PROTOCOL'),
-            'time': time.strftime('%d/%b/%Y:%H:%M:%S ', start) + offset,
-            'status': status.split(None, 1)[0],
-            'bytes': bytes,
-            'HTTP_REFERER': environ.get('HTTP_REFERER', '-'),
-            'HTTP_USER_AGENT': environ.get('HTTP_USER_AGENT', '-'),
+            "REMOTE_ADDR": environ.get("REMOTE_ADDR") or "-",
+            "REMOTE_USER": environ.get("REMOTE_USER") or "-",
+            "REQUEST_METHOD": method,
+            "REQUEST_URI": req_uri,
+            "HTTP_VERSION": environ.get("SERVER_PROTOCOL"),
+            "time": time.strftime("%d/%b/%Y:%H:%M:%S ", start) + offset,
+            "status": status.split(None, 1)[0],
+            "bytes": bytes,
+            "HTTP_REFERER": environ.get("HTTP_REFERER", "-"),
+            "HTTP_USER_AGENT": environ.get("HTTP_USER_AGENT", "-"),
         }
         message = self.format % d
         self.logger.log(self.logging_level, message)
 
 
 def make_filter(
-        app, global_conf,
-        logger_name='wsgi',
-        format=None,
-        logging_level=logging.INFO,
-        setup_console_handler=True,
-        set_logger_level=logging.DEBUG):
+    app,
+    global_conf,
+    logger_name="wsgi",
+    format=None,
+    logging_level=logging.INFO,
+    setup_console_handler=True,
+    set_logger_level=logging.DEBUG,
+):
     from paste.util.converters import asbool
+
     if isinstance(logging_level, str):
         logging_level = logging._levelNames[logging_level]
     if isinstance(set_logger_level, str):
         set_logger_level = logging._levelNames[set_logger_level]
     return TransLogger(
         app,
         format=format or None,
         logging_level=logging_level,
         logger_name=logger_name,
         setup_console_handler=asbool(setup_console_handler),
-        set_logger_level=set_logger_level)
+        set_logger_level=set_logger_level,
+    )
 
 
 make_filter.__doc__ = TransLogger.__doc__
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/framework/middleware/xforwardedhost.py` & `galaxy-web-framework-23.0.1/galaxy/web/framework/middleware/xforwardedhost.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,20 +4,23 @@
     based on the X-Forwarded-Host header IF found
     """
 
     def __init__(self, app, global_conf=None):
         self.app = app
 
     def __call__(self, environ, start_response):
-        x_forwarded_host = environ.get('HTTP_X_FORWARDED_HOST', None)
+        x_forwarded_host = environ.get("HTTP_X_FORWARDED_HOST", None)
         if x_forwarded_host:
-            environ['ORGINAL_HTTP_HOST'] = environ['HTTP_HOST']
-            environ['HTTP_HOST'] = x_forwarded_host.split(', ', 1)[0]
-        x_forwarded_for = environ.get('HTTP_X_FORWARDED_FOR', None)
+            environ["ORGINAL_HTTP_HOST"] = environ["HTTP_HOST"]
+            environ["HTTP_HOST"] = x_forwarded_host.split(", ", 1)[0]
+        x_forwarded_for = environ.get("HTTP_X_FORWARDED_FOR", None)
         if x_forwarded_for:
-            environ['ORGINAL_REMOTE_ADDR'] = environ['REMOTE_ADDR']
-            environ['REMOTE_ADDR'] = x_forwarded_for.split(', ', 1)[0]
-        x_url_scheme = environ.get('HTTP_X_URL_SCHEME', None)
+            environ["ORGINAL_REMOTE_ADDR"] = environ["REMOTE_ADDR"]
+            environ["REMOTE_ADDR"] = x_forwarded_for.split(",", 1)[0].strip()
+        x_forwarded_proto = environ.get("HTTP_X_FORWARDED_PROTO", None)
+        if x_forwarded_proto:
+            x_forwarded_proto = x_forwarded_proto.split(",", 1)[0].strip()
+        x_url_scheme = environ.get("HTTP_X_URL_SCHEME", x_forwarded_proto)
         if x_url_scheme:
-            environ['original_wsgi.url_scheme'] = environ['wsgi.url_scheme']
-            environ['wsgi.url_scheme'] = x_url_scheme
+            environ["original_wsgi.url_scheme"] = environ["wsgi.url_scheme"]
+            environ["wsgi.url_scheme"] = x_url_scheme
         return self.app(environ, start_response)
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/legacy_framework/grids.py` & `galaxy-web-framework-23.0.1/galaxy/web/legacy_framework/grids.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,44 +1,80 @@
 import logging
 import math
-from json import dumps, loads
-from typing import Dict, List, Optional
+from json import (
+    dumps,
+    loads,
+)
+from typing import (
+    Dict,
+    List,
+    Optional,
+)
 
 from markupsafe import escape
-from sqlalchemy.sql.expression import and_, false, func, null, or_, true
-
-from galaxy.model.item_attrs import get_foreign_key, UsesAnnotations, UsesItemRatings
-from galaxy.util import sanitize_text, unicodify
-from galaxy.web.framework import decorators, url_for
+from sqlalchemy.sql.expression import (
+    and_,
+    false,
+    func,
+    null,
+    or_,
+    true,
+)
+
+from galaxy.model.item_attrs import (
+    get_foreign_key,
+    UsesAnnotations,
+    UsesItemRatings,
+)
+from galaxy.util import (
+    sanitize_text,
+    unicodify,
+)
+from galaxy.web.framework import (
+    decorators,
+    url_for,
+)
 from galaxy.web.framework.helpers import iff
 
-
 log = logging.getLogger(__name__)
 
 
 class GridColumn:
-    def __init__(self, label, key=None, model_class=None, method=None, format=None,
-                 link=None, attach_popup=False, visible=True, nowrap=False,
-                 # Valid values for filterable are ['standard', 'advanced', None]
-                 filterable=None, sortable=True, label_id_prefix=None, target=None):
+    def __init__(
+        self,
+        label,
+        key=None,
+        model_class=None,
+        method=None,
+        format=None,
+        link=None,
+        attach_popup=False,
+        visible=True,
+        nowrap=False,
+        # Valid values for filterable are ['standard', 'advanced', None]
+        filterable=None,
+        sortable=True,
+        label_id_prefix=None,
+        target=None,
+    ):
         """Create a grid column."""
         self.label = label
         self.key = key
         self.model_class = model_class
         self.method = method
         self.format = format
         self.link = link
         self.target = target
         self.nowrap = nowrap
         self.attach_popup = attach_popup
         self.visible = visible
         self.filterable = filterable
         # Column must have a key to be sortable.
-        self.sortable = (self.key is not None and sortable)
-        self.label_id_prefix = label_id_prefix or ''
+        self.sortable = self.key is not None and sortable
+        self.label_id_prefix = label_id_prefix or ""
 
     def get_value(self, trans, grid, item):
         if self.method:
             value = getattr(grid, self.method)(trans, item)
         elif self.key:
             value = getattr(item, self.key)
         else:
@@ -49,25 +85,25 @@
 
     def get_link(self, trans, grid, item):
         if self.link and self.link(item):
             return self.link(item)
         return None
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to reflect the column filter. """
+        """Modify query to reflect the column filter."""
         if column_filter == "All":
             pass
         if column_filter == "True":
             query = query.filter_by(**{self.key: True})
         elif column_filter == "False":
             query = query.filter_by(**{self.key: False})
         return query
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filters_vals = ["False", "True", "All"]
         accepted_filters = []
         for val in accepted_filters_vals:
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(val, args))
         return accepted_filters
 
@@ -79,33 +115,33 @@
             query = query.order_by(self.model_class.table.c.get(column_name).asc())
         else:
             query = query.order_by(self.model_class.table.c.get(column_name).desc())
         return query
 
 
 class ReverseSortColumn(GridColumn):
-    """ Column that reverses sorting; this is useful when the natural sort is descending. """
+    """Column that reverses sorting; this is useful when the natural sort is descending."""
 
     def sort(self, trans, query, ascending, column_name=None):
         return GridColumn.sort(self, trans, query, (not ascending), column_name=column_name)
 
 
 class TextColumn(GridColumn):
-    """ Generic column that employs freetext and, hence, supports freetext, case-independent filtering. """
+    """Generic column that employs freetext and, hence, supports freetext, case-independent filtering."""
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter using free text, case independence. """
+        """Modify query to filter using free text, case independence."""
         if column_filter == "All":
             pass
         elif column_filter:
             query = query.filter(self.get_filter(trans, user, column_filter))
         return query
 
     def get_filter(self, trans, user, column_filter):
-        """ Returns a SQLAlchemy criterion derived from column_filter. """
+        """Returns a SQLAlchemy criterion derived from column_filter."""
         if isinstance(column_filter, str):
             return self.get_single_filter(user, column_filter)
         elif isinstance(column_filter, list):
             clause_list = []
             for filter in column_filter:
                 clause_list.append(self.get_single_filter(user, filter))
             return and_(*clause_list)
@@ -113,16 +149,16 @@
     def get_single_filter(self, user, a_filter):
         """
         Returns a SQLAlchemy criterion derived for a single filter. Single filter
         is the most basic filter--usually a string--and cannot be a list.
         """
         # Queries that include table joins cannot guarantee that table column names will be
         # unique, so check to see if a_filter is of type <TableName>.<ColumnName>.
-        if self.key.find('.') > -1:
-            a_key = self.key.split('.')[1]
+        if self.key.find(".") > -1:
+            a_key = self.key.split(".")[1]
         else:
             a_key = self.key
         model_class_key_field = getattr(self.model_class, a_key)
         return func.lower(model_class_key_field).like(f"%{a_filter.lower()}%")
 
     def sort(self, trans, query, ascending, column_name=None):
         """Sort column using case-insensitive alphabetical sorting."""
@@ -143,16 +179,16 @@
 
 class BooleanColumn(TextColumn):
     def sort(self, trans, query, ascending, column_name=None):
         """Sort query using this column."""
         return GridColumn.sort(self, trans, query, ascending, column_name=column_name)
 
     def get_single_filter(self, user, a_filter):
-        if self.key.find('.') > -1:
-            a_key = self.key.split('.')[1]
+        if self.key.find(".") > -1:
+            a_key = self.key.split(".")[1]
         else:
             a_key = self.key
         model_class_key_field = getattr(self.model_class, a_key)
         return model_class_key_field == a_filter
 
 
 class IntegerColumn(TextColumn):
@@ -180,88 +216,109 @@
 
     def sort(self, trans, query, ascending, column_name=None):
         """Sort query using this column."""
         return GridColumn.sort(self, trans, query, ascending, column_name=column_name)
 
 
 class CommunityRatingColumn(GridColumn, UsesItemRatings):
-    """ Column that displays community ratings for an item. """
+    """Column that displays community ratings for an item."""
 
     def get_value(self, trans, grid, item):
         ave_item_rating, num_ratings = self.get_ave_item_rating_data(trans.sa_session, item, webapp_model=trans.model)
-        return trans.fill_template("tool_shed_rating.mako",
-                                   ave_item_rating=ave_item_rating,
-                                   num_ratings=num_ratings,
-                                   item_id=trans.security.encode_id(item.id))
+        return trans.fill_template(
+            "tool_shed_rating.mako",
+            ave_item_rating=ave_item_rating,
+            num_ratings=num_ratings,
+            item_id=trans.security.encode_id(item.id),
+        )
 
     def sort(self, trans, query, ascending, column_name=None):
         # Get the columns that connect item's table and item's rating association table.
-        item_rating_assoc_class = getattr(trans.model, f'{self.model_class.__name__}RatingAssociation')
+        item_rating_assoc_class = getattr(trans.model, f"{self.model_class.__name__}RatingAssociation")
         foreign_key = get_foreign_key(item_rating_assoc_class, self.model_class)
         fk_col = foreign_key.parent
         referent_col = foreign_key.get_referent(self.model_class.table)
         # Do sorting using a subquery.
         # Subquery to get average rating for each item.
-        ave_rating_subquery = trans.sa_session.query(fk_col,
-                                                     func.avg(item_rating_assoc_class.table.c.rating).label('avg_rating')) \
-            .group_by(fk_col).subquery()
+        ave_rating_subquery = (
+            trans.sa_session.query(fk_col, func.avg(item_rating_assoc_class.table.c.rating).label("avg_rating"))
+            .group_by(fk_col)
+            .subquery()
+        )
         # Integrate subquery into main query.
         query = query.outerjoin((ave_rating_subquery, referent_col == ave_rating_subquery.columns[fk_col.name]))
         # Sort using subquery results; use coalesce to avoid null values.
-        if not ascending:  # TODO: for now, reverse sorting b/c first sort is ascending, and that should be the natural sort.
+        if (
+            not ascending
+        ):  # TODO: for now, reverse sorting b/c first sort is ascending, and that should be the natural sort.
             query = query.order_by(func.coalesce(ave_rating_subquery.c.avg_rating, 0).asc())
         else:
             query = query.order_by(func.coalesce(ave_rating_subquery.c.avg_rating, 0).desc())
         return query
 
 
 class OwnerAnnotationColumn(TextColumn, UsesAnnotations):
-    """ Column that displays and filters item owner's annotations. """
+    """Column that displays and filters item owner's annotations."""
 
     def __init__(self, col_name, key, model_class=None, model_annotation_association_class=None, filterable=None):
         GridColumn.__init__(self, col_name, key=key, model_class=model_class, filterable=filterable)
         self.sortable = False
         self.model_annotation_association_class = model_annotation_association_class
 
     def get_value(self, trans, grid, item):
-        """ Returns first 150 characters of annotation. """
+        """Returns first 150 characters of annotation."""
         annotation = self.get_item_annotation_str(trans.sa_session, item.user, item)
         if annotation:
             ann_snippet = annotation[:155]
             if len(annotation) > 155:
-                ann_snippet = ann_snippet[:ann_snippet.rfind(' ')]
+                ann_snippet = ann_snippet[: ann_snippet.rfind(" ")]
                 ann_snippet += "..."
         else:
             ann_snippet = ""
         return escape(ann_snippet)
 
     def get_single_filter(self, user, a_filter):
-        """ Filter by annotation and annotation owner. """
+        """Filter by annotation and annotation owner."""
         return self.model_class.annotations.any(
-            and_(func.lower(self.model_annotation_association_class.annotation).like(f"%{a_filter.lower()}%"),
-               # TODO: not sure why, to filter by owner's annotations, we have to do this rather than
-               # 'self.model_class.user==self.model_annotation_association_class.user'
-               self.model_annotation_association_class.table.c.user_id == self.model_class.table.c.user_id))
+            and_(
+                func.lower(self.model_annotation_association_class.annotation).like(f"%{a_filter.lower()}%"),
+                # TODO: not sure why, to filter by owner's annotations, we have to do this rather than
+                # 'self.model_class.user==self.model_annotation_association_class.user'
+                self.model_annotation_association_class.table.c.user_id == self.model_class.table.c.user_id,
+            )
+        )
 
 
 class CommunityTagsColumn(TextColumn):
-    """ Column that supports community tags. """
+    """Column that supports community tags."""
 
-    def __init__(self, col_name, key, model_class=None, model_tag_association_class=None, filterable=None, grid_name=None):
-        GridColumn.__init__(self, col_name, key=key, model_class=model_class, nowrap=True, filterable=filterable, sortable=False)
+    def __init__(
+        self, col_name, key, model_class=None, model_tag_association_class=None, filterable=None, grid_name=None
+    ):
+        GridColumn.__init__(
+            self, col_name, key=key, model_class=model_class, nowrap=True, filterable=filterable, sortable=False
+        )
         self.model_tag_association_class = model_tag_association_class
         # Column-specific attributes.
         self.grid_name = grid_name
 
     def get_value(self, trans, grid, item):
-        return trans.fill_template("/tagging_common.mako", tag_type="community", trans=trans, user=trans.get_user(), tagged_item=item, elt_context=self.grid_name,
-                                   tag_click_fn="add_tag_to_grid_filter", use_toggle_link=True)
+        return trans.fill_template(
+            "/tagging_common.mako",
+            tag_type="community",
+            trans=trans,
+            user=trans.get_user(),
+            tagged_item=item,
+            elt_context=self.grid_name,
+            tag_click_fn="add_tag_to_grid_filter",
+            use_toggle_link=True,
+        )
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter model_class by tag. Multiple filters are ANDed. """
+        """Modify query to filter model_class by tag. Multiple filters are ANDed."""
         if column_filter == "All":
             pass
         elif column_filter:
             query = query.filter(self.get_filter(trans, user, column_filter))
         return query
 
     def get_filter(self, trans, user, column_filter):
@@ -270,59 +327,83 @@
             # Collapse list of tags into a single string; this is redundant but effective. TODO: fix this by iterating over tags.
             column_filter = ",".join(column_filter)
         raw_tags = trans.app.tag_handler.parse_tags(column_filter.encode("utf-8"))
         clause_list = []
         for name, value in raw_tags:
             if name:
                 # Filter by all tags.
-                clause_list.append(self.model_class.tags.any(func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%")))
+                clause_list.append(
+                    self.model_class.tags.any(
+                        func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%")
+                    )
+                )
                 if value:
                     # Filter by all values.
-                    clause_list.append(self.model_class.tags.any(func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%")))
+                    clause_list.append(
+                        self.model_class.tags.any(
+                            func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%")
+                        )
+                    )
         return and_(*clause_list)
 
 
 class IndividualTagsColumn(CommunityTagsColumn):
-    """ Column that supports individual tags. """
+    """Column that supports individual tags."""
 
     def get_value(self, trans, grid, item):
-        return trans.fill_template("/tagging_common.mako",
-                                   tag_type="individual",
-                                   user=trans.user,
-                                   tagged_item=item,
-                                   elt_context=self.grid_name,
-                                   tag_click_fn="add_tag_to_grid_filter",
-                                   use_toggle_link=True)
+        return trans.fill_template(
+            "/tagging_common.mako",
+            tag_type="individual",
+            user=trans.user,
+            tagged_item=item,
+            elt_context=self.grid_name,
+            tag_click_fn="add_tag_to_grid_filter",
+            use_toggle_link=True,
+        )
 
     def get_filter(self, trans, user, column_filter):
         # Parse filter to extract multiple tags.
         if isinstance(column_filter, list):
             # Collapse list of tags into a single string; this is redundant but effective. TODO: fix this by iterating over tags.
             column_filter = ",".join(column_filter)
         raw_tags = trans.app.tag_handler.parse_tags(column_filter.encode("utf-8"))
         clause_list = []
         for name, value in raw_tags:
             if name:
                 # Filter by individual's tag names.
-                clause_list.append(self.model_class.tags.any(and_(func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%"), self.model_tag_association_class.user == user)))
+                clause_list.append(
+                    self.model_class.tags.any(
+                        and_(
+                            func.lower(self.model_tag_association_class.user_tname).like(f"%{name.lower()}%"),
+                            self.model_tag_association_class.user == user,
+                        )
+                    )
+                )
                 if value:
                     # Filter by individual's tag values.
-                    clause_list.append(self.model_class.tags.any(and_(func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%"), self.model_tag_association_class.user == user)))
+                    clause_list.append(
+                        self.model_class.tags.any(
+                            and_(
+                                func.lower(self.model_tag_association_class.user_value).like(f"%{value.lower()}%"),
+                                self.model_tag_association_class.user == user,
+                            )
+                        )
+                    )
         return and_(*clause_list)
 
 
 class MulticolFilterColumn(TextColumn):
-    """ Column that performs multicolumn filtering. """
+    """Column that performs multicolumn filtering."""
 
     def __init__(self, col_name, cols_to_filter, key, visible, filterable="default"):
         GridColumn.__init__(self, col_name, key=key, visible=visible, filterable=filterable)
         self.cols_to_filter = cols_to_filter
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter model_class by tag. Multiple filters are ANDed. """
+        """Modify query to filter model_class by tag. Multiple filters are ANDed."""
         if column_filter == "All":
             return query
         if isinstance(column_filter, list):
             clause_list = []
             for filter in column_filter:
                 part_clause_list = []
                 for column in self.cols_to_filter:
@@ -334,47 +415,47 @@
             for column in self.cols_to_filter:
                 clause_list.append(column.get_filter(trans, user, column_filter))
             complete_filter = or_(*clause_list)
         return query.filter(complete_filter)
 
 
 class OwnerColumn(TextColumn):
-    """ Column that lists item's owner. """
+    """Column that lists item's owner."""
 
     def get_value(self, trans, grid, item):
         return item.user.username
 
     def sort(self, trans, query, ascending, column_name=None):
-        """ Sort column using case-insensitive alphabetical sorting on item's username. """
+        """Sort column using case-insensitive alphabetical sorting on item's username."""
         if ascending:
             query = query.order_by(func.lower(self.model_class.username).asc())
         else:
             query = query.order_by(func.lower(self.model_class.username).desc())
         return query
 
 
 class PublicURLColumn(TextColumn):
-    """ Column displays item's public URL based on username and slug. """
+    """Column displays item's public URL based on username and slug."""
 
     def get_link(self, trans, grid, item):
         if item.user.username and item.slug:
-            return dict(action='display_by_username_and_slug', username=item.user.username, slug=item.slug)
+            return dict(action="display_by_username_and_slug", username=item.user.username, slug=item.slug)
         elif not item.user.username:
             # TODO: provide link to set username.
             return None
         elif not item.user.slug:
             # TODO: provide link to set slug.
             return None
 
 
 class DeletedColumn(GridColumn):
-    """ Column that tracks and filters for items with deleted attribute. """
+    """Column that tracks and filters for items with deleted attribute."""
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filter_labels_and_vals = {"active": "False", "deleted": "True", "all": "All"}
         accepted_filters = []
         for label, val in accepted_filter_labels_and_vals.items():
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(label, args))
         return accepted_filters
 
@@ -401,24 +482,24 @@
             pass
         elif column_filter in list(self.model_class.states):
             query = query.filter(self.model_class.state == column_filter)
         return query
 
     def get_accepted_filters(self):
         """Returns a list of accepted filters for this column."""
-        all = GridColumnFilter('all', {self.key: 'All'})
+        all = GridColumnFilter("all", {self.key: "All"})
         accepted_filters = [all]
         for state in self.model_class.states:
             args = {self.key: state.value}
             accepted_filters.append(GridColumnFilter(state.value, args))
         return accepted_filters
 
 
 class SharingStatusColumn(GridColumn):
-    """ Grid column to indicate sharing status. """
+    """Grid column to indicate sharing status."""
 
     def get_value(self, trans, grid, item):
         # Delete items cannot be shared.
         if item.deleted:
             return ""
         # Build a list of sharing for this item.
         sharing_statuses = []
@@ -432,15 +513,15 @@
 
     def get_link(self, trans, grid, item):
         if not item.deleted and (item.users_shared_with or item.importable or item.published):
             return dict(operation="share or publish", id=item.id)
         return None
 
     def filter(self, trans, user, query, column_filter):
-        """ Modify query to filter histories by sharing status. """
+        """Modify query to filter histories by sharing status."""
         if column_filter == "All":
             pass
         elif column_filter:
             if column_filter == "private":
                 query = query.filter(self.model_class.users_shared_with == null())
                 query = query.filter(self.model_class.importable == false())
             elif column_filter == "shared":
@@ -448,32 +529,42 @@
             elif column_filter == "accessible":
                 query = query.filter(self.model_class.importable == true())
             elif column_filter == "published":
                 query = query.filter(self.model_class.published == true())
         return query
 
     def get_accepted_filters(self):
-        """ Returns a list of accepted filters for this column. """
+        """Returns a list of accepted filters for this column."""
         accepted_filter_labels_and_vals = {}
         accepted_filter_labels_and_vals["private"] = "private"
         accepted_filter_labels_and_vals["shared"] = "shared"
         accepted_filter_labels_and_vals["accessible"] = "accessible"
         accepted_filter_labels_and_vals["published"] = "published"
         accepted_filter_labels_and_vals["all"] = "All"
         accepted_filters = []
         for label, val in accepted_filter_labels_and_vals.items():
             args = {self.key: val}
             accepted_filters.append(GridColumnFilter(label, args))
         return accepted_filters
 
 
 class GridOperation:
-    def __init__(self, label, key=None, condition=None, allow_multiple=True, allow_popup=True,
-                 target=None, url_args=None, async_compatible=False, confirm=None,
-                 global_operation=None):
+    def __init__(
+        self,
+        label,
+        key=None,
+        condition=None,
+        allow_multiple=True,
+        allow_popup=True,
+        target=None,
+        url_args=None,
+        async_compatible=False,
+        confirm=None,
+        global_operation=None,
+    ):
         self.label = label
         self.key = key
         self.allow_multiple = allow_multiple
         self.allow_popup = allow_popup
         self.condition = condition
         self.target = target
         self.url_args = url_args
@@ -488,31 +579,31 @@
 
     def get_url_args(self, item):
         if self.url_args:
             if callable(self.url_args):
                 url_args = self.url_args(item)
             else:
                 url_args = dict(self.url_args)
-            url_args['id'] = item.id
+            url_args["id"] = item.id
             return url_args
         else:
             return dict(operation=self.label, id=item.id)
 
     def allowed(self, item):
         if self.condition:
             return bool(self.condition(item))
         else:
             return True
 
 
 class DisplayByUsernameAndSlugGridOperation(GridOperation):
-    """ Operation to display an item by username and slug. """
+    """Operation to display an item by username and slug."""
 
     def get_url_args(self, item):
-        return {'action': 'display_by_username_and_slug', 'username': item.user.username, 'slug': item.slug}
+        return {"action": "display_by_username_and_slug", "username": item.user.username, "slug": item.slug}
 
 
 class GridAction:
     def __init__(self, label=None, url_args=None, target=None):
         self.label = label
         self.url_args = url_args
         self.target = target
@@ -530,14 +621,15 @@
         return rval
 
 
 class Grid:
     """
     Specifies the content and format of a grid (data table).
     """
+
     title = ""
     model_class: Optional[type] = None
     show_item_checkboxes = False
     template = "legacy/grid_base.mako"
     async_template = "legacy/grid_base_async.mako"
     use_async = False
     use_hide_message = True
@@ -571,33 +663,33 @@
         for column in self.columns:
             if not column.model_class:
                 column.model_class = self.model_class
 
     def __call__(self, trans, **kwargs):
         # Get basics.
         # FIXME: pretty sure this is only here to pass along, can likely be eliminated
-        status = kwargs.get('status', None)
-        message = kwargs.get('message', None)
+        status = kwargs.get("status", None)
+        message = kwargs.get("message", None)
         # Build a base filter and sort key that is the combination of the saved state and defaults.
         # Saved state takes preference over defaults.
         base_filter = {}
         if self.default_filter:
             # default_filter is a dictionary that provides a default set of filters based on the grid's columns.
             base_filter = self.default_filter.copy()
         base_sort_key = self.default_sort_key
         # Build initial query
         query = self.build_initial_query(trans, **kwargs)
         query = self.apply_query_filter(trans, query, **kwargs)
         # Maintain sort state in generated urls
         extra_url_args = {}
         # Determine whether use_default_filter flag is set.
-        use_default_filter_str = kwargs.get('use_default_filter')
+        use_default_filter_str = kwargs.get("use_default_filter")
         use_default_filter = False
         if use_default_filter_str:
-            use_default_filter = (use_default_filter_str.lower() == 'true')
+            use_default_filter = use_default_filter_str.lower() == "true"
         # Process filtering arguments to (a) build a query that represents the filter and (b) build a
         # dictionary that denotes the current filter.
         cur_filter_dict = {}
         for column in self.columns:
             if column.key:
                 # Get the filter criterion for the column. Precedence is (a) if using default filter, only look there; otherwise,
                 # (b) look in kwargs; and (c) look in base filter.
@@ -628,98 +720,99 @@
                         except ValueError:
                             decoded_list = [str(item)]
                     elif isinstance(item, list):
                         for element in item:
                             a_list = loads_recurse(element)
                             decoded_list = decoded_list + a_list
                     return decoded_list
+
                 # If column filter found, apply it.
                 if column_filter is not None:
                     # TextColumns may have a mix of json and strings.
                     if isinstance(column, TextColumn):
                         column_filter = loads_recurse(column_filter)
                         if len(column_filter) == 1:
                             column_filter = column_filter[0]
                     # Interpret ',' as a separator for multiple terms.
-                    if isinstance(column_filter, str) and column_filter.find(',') != -1:
-                        column_filter = column_filter.split(',')
+                    if isinstance(column_filter, str) and column_filter.find(",") != -1:
+                        column_filter = column_filter.split(",")
 
                     # Check if filter is empty
                     if isinstance(column_filter, list):
                         # Remove empty strings from filter list
-                        column_filter = [x for x in column_filter if x != '']
+                        column_filter = [x for x in column_filter if x != ""]
                         if len(column_filter) == 0:
                             continue
                     elif isinstance(column_filter, str):
                         # If filter criterion is empty, do nothing.
-                        if column_filter == '':
+                        if column_filter == "":
                             continue
 
                     # Update query.
                     query = column.filter(trans, trans.user, query, column_filter)
                     # Upate current filter dict.
                     # Column filters are rendered in various places, sanitize them all here.
                     cur_filter_dict[column.key] = sanitize_text(column_filter)
                     # Carry filter along to newly generated urls; make sure filter is a string so
                     # that we can encode to UTF-8 and thus handle user input to filters.
                     if isinstance(column_filter, list):
                         # Filter is a list; process each item.
-                        column_filter = [str(_).encode('utf-8') if not isinstance(_, str) else _ for _ in column_filter]
+                        column_filter = [str(_).encode("utf-8") if not isinstance(_, str) else _ for _ in column_filter]
                         extra_url_args[f"f-{column.key}"] = dumps(column_filter)
                     else:
                         # Process singleton filter.
                         if not isinstance(column_filter, str):
                             column_filter = str(column_filter)
                         extra_url_args[f"f-{column.key}"] = column_filter.encode("utf-8")
         # Process sort arguments.
         sort_key = None
-        if 'sort' in kwargs:
-            sort_key = kwargs['sort']
+        if "sort" in kwargs:
+            sort_key = kwargs["sort"]
         elif base_sort_key:
             sort_key = base_sort_key
         if sort_key:
-            ascending = not(sort_key.startswith("-"))
+            ascending = not (sort_key.startswith("-"))
             # Queries that include table joins cannot guarantee unique column names.  This problem is
             # handled by setting the column_filter value to <TableName>.<ColumnName>.
             table_name = None
-            if sort_key.find('.') > -1:
-                a_list = sort_key.split('.')
+            if sort_key.find(".") > -1:
+                a_list = sort_key.split(".")
                 if ascending:
                     table_name = a_list[0]
                 else:
                     table_name = a_list[0][1:]
                 column_name = a_list[1]
             elif ascending:
                 column_name = sort_key
             else:
                 column_name = sort_key[1:]
             # Sort key is a column key.
             for column in self.columns:
-                if column.key and column.key.find('.') > -1:
-                    column_key = column.key.split('.')[1]
+                if column.key and column.key.find(".") > -1:
+                    column_key = column.key.split(".")[1]
                 else:
                     column_key = column.key
                 if (table_name is None or table_name == column.model_class.__name__) and column_key == column_name:
                     query = column.sort(trans, query, ascending, column_name=column_name)
                     break
-            extra_url_args['sort'] = sort_key
+            extra_url_args["sort"] = sort_key
         # There might be a current row
         current_item = self.get_current_item(trans, **kwargs)
         # Process page number.
         if self.use_paging:
-            if 'page' in kwargs:
-                if kwargs['page'] == 'all':
+            if "page" in kwargs:
+                if kwargs["page"] == "all":
                     page_num = 0
                     if self.allow_fetching_all_results:
                         page_num = 0
                     else:
                         # Should make it harder to return all results at once
                         page_num = 1
                 else:
-                    page_num = int(kwargs['page'])
+                    page_num = int(kwargs["page"])
             else:
                 page_num = 1
             if page_num == 0:
                 # Show all rows in page.
                 total_num_rows = query.count()
                 page_num = 1
                 num_pages = 1
@@ -736,92 +829,95 @@
         # There are some places in grid templates where it's useful for a grid
         # to have its current filter.
         self.cur_filter_dict = cur_filter_dict
 
         # Log grid view.
         context = str(self.__class__.__name__)
         params = cur_filter_dict.copy()
-        params['sort'] = sort_key
-        params['async'] = ('async' in kwargs)
+        params["sort"] = sort_key
+        params["async"] = "async" in kwargs
 
         # TODO:??
         # commenting this out; when this fn calls session.add( action ) and session.flush the query from this fn
         # is effectively 'wiped' out. Nate believes it has something to do with our use of session( autocommit=True )
         # in mapping.py. If you change that to False, the log_action doesn't affect the query
         # Below, I'm rendering the template first (that uses query), then calling log_action, then returning the page
         # trans.log_action( trans.get_user(), text_type( "grid.view" ), context, params )
 
         # Render grid.
         def url(*args, **kwargs):
-            route_name = kwargs.pop('__route_name__', None)
+            route_name = kwargs.pop("__route_name__", None)
             # Only include sort/filter arguments if not linking to another
             # page. This is a bit of a hack.
-            if 'action' in kwargs:
+            if "action" in kwargs:
                 new_kwargs = dict()
             else:
                 new_kwargs = dict(extra_url_args)
             # Extend new_kwargs with first argument if found
             if len(args) > 0:
                 new_kwargs.update(args[0])
             new_kwargs.update(kwargs)
             # We need to encode item ids
-            if 'id' in new_kwargs:
-                id = new_kwargs['id']
+            if "id" in new_kwargs:
+                id = new_kwargs["id"]
                 if isinstance(id, list):
-                    new_kwargs['id'] = [trans.security.encode_id(i) for i in id]
+                    new_kwargs["id"] = [trans.security.encode_id(i) for i in id]
                 else:
-                    new_kwargs['id'] = trans.security.encode_id(id)
+                    new_kwargs["id"] = trans.security.encode_id(id)
             # The url_for invocation *must* include a controller and action.
-            if 'controller' not in new_kwargs:
-                new_kwargs['controller'] = trans.controller
-            if 'action' not in new_kwargs:
-                new_kwargs['action'] = trans.action
+            if "controller" not in new_kwargs:
+                new_kwargs["controller"] = trans.controller
+            if "action" not in new_kwargs:
+                new_kwargs["action"] = trans.action
             if route_name:
                 return url_for(route_name, **new_kwargs)
             return url_for(**new_kwargs)
 
-        self.use_panels = (kwargs.get('use_panels', False) in [True, 'True', 'true'])
-        self.advanced_search = (kwargs.get('advanced_search', False) in [True, 'True', 'true'])
-        async_request = ((self.use_async) and (kwargs.get('async', False) in [True, 'True', 'true']))
+        self.use_panels = kwargs.get("use_panels", False) in [True, "True", "true"]
+        self.advanced_search = kwargs.get("advanced_search", False) in [True, "True", "true"]
+        async_request = (self.use_async) and (kwargs.get("async", False) in [True, "True", "true"])
         # Currently, filling the template returns a str object; this requires decoding the string into a
         # unicode object within mako templates. What probably should be done is to return the template as
         # utf-8 unicode; however, this would require encoding the object as utf-8 before returning the grid
         # results via a controller method, which is require substantial changes. Hence, for now, return grid
         # as str.
-        page = trans.fill_template(iff(async_request, self.async_template, self.template),
-                                   grid=self,
-                                   query=query,
-                                   cur_page_num=page_num,
-                                   num_pages=num_pages,
-                                   num_page_links=self.num_page_links,
-                                   allow_fetching_all_results=self.allow_fetching_all_results,
-                                   default_filter_dict=self.default_filter,
-                                   cur_filter_dict=cur_filter_dict,
-                                   sort_key=sort_key,
-                                   current_item=current_item,
-                                   ids=kwargs.get('id', []),
-                                   url=url,
-                                   status=status,
-                                   message=message,
-                                   info_text=self.info_text,
-                                   use_panels=self.use_panels,
-                                   use_hide_message=self.use_hide_message,
-                                   advanced_search=self.advanced_search,
-                                   show_item_checkboxes=(self.show_item_checkboxes
-                                                         or kwargs.get('show_item_checkboxes', '') in ['True', 'true']),
-                                   # Pass back kwargs so that grid template can set and use args without
-                                   # grid explicitly having to pass them.
-                                   kwargs=kwargs)
+        page = trans.fill_template(
+            iff(async_request, self.async_template, self.template),
+            grid=self,
+            query=query,
+            cur_page_num=page_num,
+            num_pages=num_pages,
+            num_page_links=self.num_page_links,
+            allow_fetching_all_results=self.allow_fetching_all_results,
+            default_filter_dict=self.default_filter,
+            cur_filter_dict=cur_filter_dict,
+            sort_key=sort_key,
+            current_item=current_item,
+            ids=kwargs.get("id", []),
+            url=url,
+            status=status,
+            message=message,
+            info_text=self.info_text,
+            use_panels=self.use_panels,
+            use_hide_message=self.use_hide_message,
+            advanced_search=self.advanced_search,
+            show_item_checkboxes=(
+                self.show_item_checkboxes or kwargs.get("show_item_checkboxes", "") in ["True", "true"]
+            ),
+            # Pass back kwargs so that grid template can set and use args without
+            # grid explicitly having to pass them.
+            kwargs=kwargs,
+        )
         trans.log_action(trans.get_user(), "grid.view", context, params)
         return page
 
     def get_ids(self, **kwargs):
         id = []
-        if 'id' in kwargs:
-            id = kwargs['id']
+        if "id" in kwargs:
+            id = kwargs["id"]
             # Coerce ids to list
             if not isinstance(id, list):
                 id = id.split(",")
             # Ensure ids are integers
             try:
                 id = list(map(int, id))
             except Exception:
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/proxy/__init__.py` & `galaxy-web-framework-23.0.1/galaxy/web/proxy/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,46 +5,53 @@
 from collections import namedtuple
 
 import requests
 
 from galaxy.util import (
     sockets,
     sqlite,
-    unique_id
+    unique_id,
 )
 from galaxy.util.filelock import FileLock
-from galaxy.util.lazy_process import LazyProcess, NoOpLazyProcess
+from galaxy.util.lazy_process import (
+    LazyProcess,
+    NoOpLazyProcess,
+)
 from galaxy.web.framework import url_for
 
 log = logging.getLogger(__name__)
 
 
 DEFAULT_PROXY_TO_HOST = "localhost"
 SECURE_COOKIE = "galaxysession"
 # Randomly generate a password every launch
 
 
 class ProxyManager:
-
     valid_update_keys = (
-        'host',
-        'port',
+        "host",
+        "port",
     )
 
     def __init__(self, config):
-        for option in ["manage_dynamic_proxy", "dynamic_proxy_bind_port",
-                       "dynamic_proxy_bind_ip", "dynamic_proxy_debug",
-                       "dynamic_proxy_external_proxy", "dynamic_proxy_prefix",
-                       "proxy_session_map",
-                       "dynamic_proxy", "cookie_path",
-                       "dynamic_proxy_golang_noaccess",
-                       "dynamic_proxy_golang_clean_interval",
-                       "dynamic_proxy_golang_docker_address",
-                       "dynamic_proxy_golang_api_key"]:
-
+        for option in [
+            "manage_dynamic_proxy",
+            "dynamic_proxy_bind_port",
+            "dynamic_proxy_bind_ip",
+            "dynamic_proxy_debug",
+            "dynamic_proxy_external_proxy",
+            "dynamic_proxy_prefix",
+            "proxy_session_map",
+            "dynamic_proxy",
+            "cookie_path",
+            "dynamic_proxy_golang_noaccess",
+            "dynamic_proxy_golang_clean_interval",
+            "dynamic_proxy_golang_docker_address",
+            "dynamic_proxy_golang_api_key",
+        ]:
             setattr(self, option, getattr(config, option))
 
         if self.manage_dynamic_proxy:
             self.lazy_process = self.__setup_lazy_process(config)
         else:
             self.lazy_process = NoOpLazyProcess()
 
@@ -52,46 +59,55 @@
             self.dynamic_proxy_golang_api_key = unique_id()
 
         self.proxy_ipc = proxy_ipc(config)
 
     def shutdown(self):
         self.lazy_process.shutdown()
 
-    def setup_proxy(self, trans, host=DEFAULT_PROXY_TO_HOST, port=None, proxy_prefix="", route_name="", container_ids=None, container_interface=None):
+    def setup_proxy(
+        self,
+        trans,
+        host=DEFAULT_PROXY_TO_HOST,
+        port=None,
+        proxy_prefix="",
+        route_name="",
+        container_ids=None,
+        container_interface=None,
+    ):
         if self.manage_dynamic_proxy:
             log.info("Attempting to start dynamic proxy process")
             log.debug(f"Cmd: {' '.join(self.lazy_process.command_and_args)}")
             self.lazy_process.start_process()
 
         if container_ids is None:
             container_ids = []
 
         authentication = AuthenticationToken(trans)
         proxy_requests = ProxyRequests(host=host, port=port)
         self.proxy_ipc.handle_requests(
             authentication,
             proxy_requests,
-            f'/{route_name}',
+            f"/{route_name}",
             container_ids,
             container_interface,
         )
         # TODO: These shouldn't need to be request.host and request.scheme -
         # though they are reasonable defaults.
         host = trans.request.host
-        if ':' in host:
-            host = host[0:host.index(':')]
+        if ":" in host:
+            host = host[0 : host.index(":")]
         scheme = trans.request.scheme
         if not self.dynamic_proxy_external_proxy:
-            proxy_url = '%s://%s:%d' % (scheme, host, self.dynamic_proxy_bind_port)
+            proxy_url = "%s://%s:%d" % (scheme, host, self.dynamic_proxy_bind_port)
         else:
-            proxy_url = f'{scheme}://{host}{proxy_prefix}'
+            proxy_url = f"{scheme}://{host}{proxy_prefix}"
         return {
-            'proxy_url': proxy_url,
-            'proxied_port': proxy_requests.port,
-            'proxied_host': proxy_requests.host,
+            "proxy_url": proxy_url,
+            "proxied_port": proxy_requests.port,
+            "proxied_host": proxy_requests.host,
         }
 
     def update_proxy(self, trans, **kwargs):
         authentication = AuthenticationToken(trans)
         for k in kwargs.keys():
             if k not in self.valid_update_keys:
                 raise Exception(f"Invalid proxy request update key: {k}")
@@ -112,71 +128,75 @@
         elif self.dynamic_proxy == "golang":
             return GolangProxyLauncher()
         else:
             raise Exception("Unknown proxy type")
 
 
 class ProxyLauncher:
-
     def launch_proxy_command(self, config):
         raise NotImplementedError()
 
 
 class NodeProxyLauncher:
-
     def launch_proxy_command(self, config):
         args = [
-            "--sessions", config.proxy_session_map,
-            "--ip", config.dynamic_proxy_bind_ip,
-            "--port", str(config.dynamic_proxy_bind_port),
+            "--sessions",
+            config.proxy_session_map,
+            "--ip",
+            config.dynamic_proxy_bind_ip,
+            "--port",
+            str(config.dynamic_proxy_bind_port),
             "--reverseProxy",
         ]
         if config.dynamic_proxy_debug:
             args.append("--verbose")
 
         parent_directory = os.path.dirname(__file__)
         path_to_application = os.path.join(parent_directory, "js", "lib", "main.js")
         command = [path_to_application] + args
         return command
 
 
 class GolangProxyLauncher:
-
     def launch_proxy_command(self, config):
         args = [
             "gxproxy",  # Must be on path. TODO: wheel?
-            "--listenAddr", '%s:%d' % (
+            "--listenAddr",
+            "%s:%d"
+            % (
                 config.dynamic_proxy_bind_ip,
                 config.dynamic_proxy_bind_port,
             ),
-            "--listenPath", "/".join((
-                (config.cookie_path or url_for('/')),
-                config.dynamic_proxy_prefix
-            )),
-            "--cookieName", "galaxysession",
-            "--storage", config.proxy_session_map.replace('.sqlite', '.xml'),  # just in case.
-            "--apiKey", config.dynamic_proxy_golang_api_key,
-            "--noAccess", config.dynamic_proxy_golang_noaccess,
-            "--cleanInterval", config.dynamic_proxy_golang_clean_interval,
-            "--dockerAddr", config.dynamic_proxy_golang_docker_address,
+            "--listenPath",
+            "/".join(((config.cookie_path or url_for("/")), config.dynamic_proxy_prefix)),
+            "--cookieName",
+            "galaxysession",
+            "--storage",
+            config.proxy_session_map.replace(".sqlite", ".xml"),  # just in case.
+            "--apiKey",
+            config.dynamic_proxy_golang_api_key,
+            "--noAccess",
+            config.dynamic_proxy_golang_noaccess,
+            "--cleanInterval",
+            config.dynamic_proxy_golang_clean_interval,
+            "--dockerAddr",
+            config.dynamic_proxy_golang_docker_address,
         ]
         if config.dynamic_proxy_debug:
             args.append("--verbose")
         return args
 
 
 class AuthenticationToken:
-
     def __init__(self, trans):
         self.cookie_name = SECURE_COOKIE
         self.cookie_value = trans.get_cookie(self.cookie_name)
 
 
 class ProxyRequests:
-
     def __init__(self, host=None, port=None):
         if host is None:
             host = DEFAULT_PROXY_TO_HOST
         if port is None:
             port = sockets.unused_port()
             log.info("Obtained unused port %d" % port)
         self.host = host
@@ -191,169 +211,167 @@
         else:
             return JsonFileProxyIpc(proxy_session_map)
     elif config.dynamic_proxy == "golang":
         return RestGolangProxyIpc(config)
 
 
 class ProxyIpc:
-
     def handle_requests(self, authentication, proxy_requests, route_name, container_ids, container_interface):
         raise NotImplementedError()
 
     def fetch_requests(self, authentication, key):
         raise NotImplementedError()
 
 
 class JsonFileProxyIpc:
-
     def __init__(self, proxy_session_map):
         self.proxy_session_map = proxy_session_map
 
     def handle_requests(self, authentication, proxy_requests, route_name, container_ids, container_interface):
         key = authentication.cookie_value
         with FileLock(self.proxy_session_map):
             if not os.path.exists(self.proxy_session_map):
                 open(self.proxy_session_map, "w").write("{}")
             json_data = open(self.proxy_session_map).read()
             session_map = json.loads(json_data)
             session_map[key] = {
-                'host': proxy_requests.host,
-                'port': proxy_requests.port,
-                'container_ids': container_ids,
-                'container_interface': container_interface,
+                "host": proxy_requests.host,
+                "port": proxy_requests.port,
+                "container_ids": container_ids,
+                "container_interface": container_interface,
             }
             new_json_data = json.dumps(session_map)
             open(self.proxy_session_map, "w").write(new_json_data)
 
     def update_requests(self, authentication, host=None, port=None):
         key = authentication.cookie_value
         with FileLock(self.proxy_session_map):
             session_map = json.load(open(self.proxy_session_map))
-            session_map[key]['host'] = host
-            session_map[key]['port'] = port
+            session_map[key]["host"] = host
+            session_map[key]["port"] = port
             new_json_data = json.dumps(session_map)
             open(self.proxy_session_map, "w").write(new_json_data)
 
     def fetch_requests(self, authentication):
         key = authentication.cookie_value
         try:
             with open(self.proxy_session_map) as fh:
                 session_map = json.load(fh)
                 m = session_map[key]
                 return ProxyMapping(
-                    host=m['host'],
-                    port=m['port'],
-                    container_ids=m['container_ids'],
-                    container_interface=m['container_interface'],
+                    host=m["host"],
+                    port=m["port"],
+                    container_ids=m["container_ids"],
+                    container_interface=m["container_interface"],
                 )
         except (TypeError, KeyError):
-            log.warning('fetch_requests(): invalid key: %s', key)
+            log.warning("fetch_requests(): invalid key: %s", key)
             return None
 
 
 class SqliteProxyIpc:
-
     def __init__(self, proxy_session_map):
         self.proxy_session_map = proxy_session_map
 
     def handle_requests(self, authentication, proxy_requests, route_name, container_ids, container_interface):
         key = authentication.cookie_value
         with FileLock(self.proxy_session_map):
             conn = sqlite.connect(self.proxy_session_map)
             try:
                 c = conn.cursor()
                 try:
                     # Create table
-                    c.execute('''CREATE TABLE gxproxy2
+                    c.execute(
+                        """CREATE TABLE gxproxy2
                                  (key text PRIMARY KEY,
                                   host text,
                                   port integer,
                                   container_ids text,
-                                  container_interface text)''')
+                                  container_interface text)"""
+                    )
                 except Exception:
                     pass
-                delete = '''DELETE FROM gxproxy2 WHERE key=?'''
+                delete = """DELETE FROM gxproxy2 WHERE key=?"""
                 c.execute(delete, (key,))
-                insert = '''INSERT INTO gxproxy2
+                insert = """INSERT INTO gxproxy2
                             (key, host, port, container_ids, container_interface)
-                            VALUES (?, ?, ?, ?, ?)'''
-                c.execute(insert,
-                          (key,
-                           proxy_requests.host,
-                           proxy_requests.port,
-                           json.dumps(container_ids),
-                           container_interface))
+                            VALUES (?, ?, ?, ?, ?)"""
+                c.execute(
+                    insert,
+                    (key, proxy_requests.host, proxy_requests.port, json.dumps(container_ids), container_interface),
+                )
                 conn.commit()
             finally:
                 conn.close()
 
     def update_requests(self, authentication, host=None, port=None):
         key = authentication.cookie_value
         with FileLock(self.proxy_session_map):
             conn = sqlite.connect(self.proxy_session_map)
             try:
                 c = conn.cursor()
-                update = '''UPDATE gxproxy2
+                update = """UPDATE gxproxy2
                             SET host = ?, port = ?
-                            WHERE key = ?'''
+                            WHERE key = ?"""
                 c.execute(update, (host, port, key))
                 conn.commit()
             finally:
                 conn.close()
 
     def fetch_requests(self, authentication):
         key = authentication.cookie_value
         with FileLock(self.proxy_session_map):
             conn = sqlite.connect(self.proxy_session_map)
             try:
                 c = conn.cursor()
-                select = '''SELECT host, port, container_ids, container_interface
+                select = """SELECT host, port, container_ids, container_interface
                             FROM gxproxy2
-                            WHERE key=?'''
+                            WHERE key=?"""
                 c.execute(select, (key,))
                 try:
                     host, port, container_ids, container_interface = c.fetchone()
                 except TypeError:
-                    log.warning('fetch_requests(): invalid key: %s', key)
+                    log.warning("fetch_requests(): invalid key: %s", key)
                     return None
                 return ProxyMapping(
                     host=host,
                     port=port,
                     container_ids=json.loads(container_ids),
-                    container_interface=container_interface)
+                    container_interface=container_interface,
+                )
             finally:
                 conn.close()
 
 
 class RestGolangProxyIpc:
-
     def __init__(self, config):
         self.config = config
-        self.api_url = f'http://127.0.0.1:{self.config.dynamic_proxy_bind_port}/api?api_key={self.config.dynamic_proxy_golang_api_key}'
+        self.api_url = f"http://127.0.0.1:{self.config.dynamic_proxy_bind_port}/api?api_key={self.config.dynamic_proxy_golang_api_key}"
 
     def handle_requests(self, authentication, proxy_requests, route_name, container_ids, container_interface, sleep=1):
-        """Make a POST request to the GO proxy to register a route
-        """
+        """Make a POST request to the GO proxy to register a route"""
         values = {
-            'FrontendPath': route_name,
-            'BackendAddr': f"{proxy_requests.host}:{proxy_requests.port}",
-            'AuthorizedCookie': authentication.cookie_value,
-            'ContainerIds': container_ids,
+            "FrontendPath": route_name,
+            "BackendAddr": f"{proxy_requests.host}:{proxy_requests.port}",
+            "AuthorizedCookie": authentication.cookie_value,
+            "ContainerIds": container_ids,
         }
 
         # Sometimes it takes our poor little proxy a second or two to get
         # going, so if this fails, re-call ourselves with an increased timeout.
         try:
-            requests.get(self.api_url, headers={'Content-Type': 'application/json'}, data=json.dumps(values))
+            requests.get(self.api_url, headers={"Content-Type": "application/json"}, data=json.dumps(values))
         except requests.exceptions.ConnectionError as err:
             log.exception(err)
             if sleep > 5:
                 excp = f"Could not contact proxy after {sum(range(sleep + 1))} seconds"
                 raise Exception(excp)
             time.sleep(sleep)
-            self.handle_requests(authentication, proxy_requests, route_name, container_ids, container_interface, sleep=sleep + 1)
+            self.handle_requests(
+                authentication, proxy_requests, route_name, container_ids, container_interface, sleep=sleep + 1
+            )
 
 
-ProxyMapping = namedtuple('ProxyMapping', ['host', 'port', 'container_ids', 'container_interface'])
+ProxyMapping = namedtuple("ProxyMapping", ["host", "port", "container_ids", "container_interface"])
 
 
 # TODO: MQ diven proxy?
```

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/proxy/js/Dockerfile` & `galaxy-web-framework-23.0.1/galaxy/web/proxy/js/Dockerfile`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/main.js` & `galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/main.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/mapper.js` & `galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/mapper.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/proxy/js/lib/proxy.js` & `galaxy-web-framework-23.0.1/galaxy/web/proxy/js/lib/proxy.js`

 * *Files identical despite different names*

### Comparing `galaxy-web-framework-22.1.1/galaxy/web/statsd_client.py` & `galaxy-web-framework-23.0.1/galaxy/web/statsd_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 import sys
-from typing import Dict, Optional, Type
+from typing import (
+    Dict,
+    Optional,
+)
 
 try:
     import statsd
 except ImportError:
     statsd = None
 
 from galaxy.util import asbool
 
 
 # TODO: optimize with two separate implementations around statsd_influxdb?
 class VanillaGalaxyStatsdClient:
-
-    def __init__(self,
-                 statsd_host,
-                 statsd_port,
-                 statsd_prefix,
-                 statsd_influxdb,
-                 statsd_mock_calls=False):
+    def __init__(self, statsd_host, statsd_port, statsd_prefix, statsd_influxdb, statsd_mock_calls=False):
         if not statsd:
-            raise ImportError("Statsd logging configured, but no statsd python module found. "
-                           "Please install the python statsd module to use this functionality.")
+            raise ImportError(
+                "Statsd logging configured, but no statsd python module found. "
+                "Please install the python statsd module to use this functionality."
+            )
 
-        self.metric_infix = ''
+        self.metric_infix = ""
         self.statsd_influxdb = asbool(statsd_influxdb)
         if self.statsd_influxdb:
-            statsd_prefix = statsd_prefix.strip(',')
+            statsd_prefix = statsd_prefix.strip(",")
         if statsd_mock_calls:
             self.statsd_client = MockStatsClient()
         else:
             self.statsd_client = statsd.StatsClient(statsd_host, statsd_port, prefix=statsd_prefix)
 
     def timing(self, path, time, tags=None):
         infix = self._effective_infix(path, tags)
@@ -38,27 +37,26 @@
     def incr(self, path, n=1, tags=None):
         infix = self._effective_infix(path, tags)
         self.statsd_client.incr(infix + path, n)
 
     def _effective_infix(self, path, tags):
         tags = tags or {}
         if self.statsd_influxdb and tags:
-            return f",{','.join(f'{k}={v}' for k, v in tags.items())}" + ',path='
+            return f",{','.join(f'{k}={v}' for k, v in tags.items())}" + ",path="
         if self.statsd_influxdb:
-            return ',path='
+            return ",path="
         else:
-            return ''
+            return ""
 
 
 CURRENT_TEST: Optional[str] = None
 CURRENT_TEST_METRICS: Optional[Dict[str, Dict]] = None
 
 
 class PyTestGalaxyStatsdClient(VanillaGalaxyStatsdClient):
-
     def timing(self, path, time, tags=None):
         metrics = CURRENT_TEST_METRICS
         if metrics is not None:
             timing = metrics["timing"]
             if path not in timing:
                 timing[path] = []
             timing[path].append({"time": time, "tags": tags})
@@ -78,24 +76,22 @@
         if current_test is not None:
             tags = tags or {}
             tags["test"] = current_test
         return super()._effective_infix(path, tags)
 
 
 class MockStatsClient:
-
     def timing(self, path, time, tags=None):
         pass
 
     def incr(self, path, n=1, tags=None):
         pass
 
 
-GalaxyStatsdClient: Type[VanillaGalaxyStatsdClient]
 # Replace stats collector if in pytest environment
-if 'pytest' in sys.modules:
+if "pytest" in sys.modules:
     GalaxyStatsdClient = PyTestGalaxyStatsdClient
 else:
-    GalaxyStatsdClient = VanillaGalaxyStatsdClient
+    GalaxyStatsdClient = VanillaGalaxyStatsdClient  # type: ignore[assignment,misc]
 
 
-__all__ = ('GalaxyStatsdClient',)
+__all__ = ("GalaxyStatsdClient",)
```

### Comparing `galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/PKG-INFO` & `galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,69 +1,69 @@
 Metadata-Version: 2.1
 Name: galaxy-web-framework
-Version: 22.1.1
-Summary: Galaxy Web Framework
+Version: 23.0.1
+Summary: Galaxy web framework
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Code Generators
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-web-framework.svg
    :target: https://pypi.org/project/galaxy-web-framework/
 
 
 Overview
 --------
 
 The Galaxy_ web framework.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.1 (2023-06-08)
+-------------------
+
 
+=========
+Bug fixes
+=========
 
+* Various fixes to path prefix handling by `@mvdbeek <https://github.com/mvdbeek>`_ in `#16033 <https://github.com/galaxyproject/galaxy/pull/16033>`_
 
----------------------
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-web-framework-22.1.1/galaxy_web_framework.egg-info/SOURCES.txt` & `galaxy-web-framework-23.0.1/galaxy_web_framework.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,31 +1,27 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
 dev-requirements.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 test-requirements.txt
 galaxy/__init__.py
-galaxy/project_galaxy_web_framework.py
+galaxy/py.typed
 galaxy/web/__init__.py
-galaxy/web/buildapp.py
 galaxy/web/form_builder.py
 galaxy/web/statsd_client.py
 galaxy/web/framework/__init__.py
 galaxy/web/framework/base.py
 galaxy/web/framework/decorators.py
 galaxy/web/framework/helpers/__init__.py
 galaxy/web/framework/helpers/grids.py
 galaxy/web/framework/helpers/tags.py
 galaxy/web/framework/middleware/__init__.py
-galaxy/web/framework/middleware/batch.py
 galaxy/web/framework/middleware/error.py
 galaxy/web/framework/middleware/profile.py
 galaxy/web/framework/middleware/remoteuser.py
 galaxy/web/framework/middleware/request_id.py
 galaxy/web/framework/middleware/sqldebug.py
 galaxy/web/framework/middleware/static.py
 galaxy/web/framework/middleware/statsd.py
@@ -36,20 +32,13 @@
 galaxy/web/proxy/__init__.py
 galaxy/web/proxy/js/Dockerfile
 galaxy/web/proxy/js/README.md
 galaxy/web/proxy/js/package.json
 galaxy/web/proxy/js/lib/main.js
 galaxy/web/proxy/js/lib/mapper.js
 galaxy/web/proxy/js/lib/proxy.js
+galaxy/web/short_term_storage/__init__.py
 galaxy_web_framework.egg-info/PKG-INFO
 galaxy_web_framework.egg-info/SOURCES.txt
 galaxy_web_framework.egg-info/dependency_links.txt
-galaxy_web_framework.egg-info/entry_points.txt
-galaxy_web_framework.egg-info/not-zip-safe
 galaxy_web_framework.egg-info/requires.txt
-galaxy_web_framework.egg-info/top_level.txt
-scripts/commit_version.py
-scripts/new_version.py
-scripts/print_version_for_release.py
-tests/__init__.py
-tests/web_framework/__init__.py
-tests/web_framework/framework/test_framework_base.py
+galaxy_web_framework.egg-info/top_level.txt
```

