# Comparing `tmp/aiopenapi3-0.2.0.tar.gz` & `tmp/aiopenapi3-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiopenapi3-0.2.0.tar", last modified: Fri Feb 10 07:49:49 2023, max compression
+gzip compressed data, was "aiopenapi3-0.2.1.tar", last modified: Thu Jun  8 08:04:07 2023, max compression
```

## Comparing `aiopenapi3-0.2.0.tar` & `aiopenapi3-0.2.1.tar`

### file list

```diff
@@ -1,71 +1,72 @@
-drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-02-10 07:49:49.516840 aiopenapi3-0.2.0/
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1519 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/LICENSE
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     3842 2023-02-10 07:49:49.516840 aiopenapi3-0.2.0/PKG-INFO
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2450 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/README.md
-drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-02-10 07:49:49.500840 aiopenapi3-0.2.0/aiopenapi3/
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      599 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/__init__.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       84 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/__main__.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    12784 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/base.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    10721 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/cli.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1991 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/errors.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      578 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/json.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     7406 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/loader.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2592 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/log.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       13 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/me.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    13082 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/model.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    25883 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/openapi.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     4402 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/plugin.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     7071 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/request.py
-drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-02-10 07:49:49.504840 aiopenapi3-0.2.0/aiopenapi3/v20/
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      164 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/__init__.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1228 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/general.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    11107 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/glue.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1184 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/info.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5632 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/parameter.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2994 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/paths.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1637 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/root.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2555 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/schemas.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1369 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/security.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      578 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/tag.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      473 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v20/xml.py
-drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-02-10 07:49:49.512840 aiopenapi3-0.2.0/aiopenapi3/v30/
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      215 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/__init__.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1566 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/components.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      582 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/example.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1348 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/general.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    12581 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/glue.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1190 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/info.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1408 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/media.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     9876 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/parameter.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5532 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/paths.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1187 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/root.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     3680 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/schemas.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2628 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/security.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      809 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/servers.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      520 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/tag.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      413 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v30/xml.py
-drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-02-10 07:49:49.516840 aiopenapi3-0.2.0/aiopenapi3/v31/
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       82 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/__init__.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1571 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/components.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      549 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/example.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1461 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/general.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1683 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/info.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1389 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/media.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1684 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/parameter.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5555 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/paths.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1511 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/root.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     6421 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/schemas.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2626 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/security.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1104 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/servers.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       26 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/tag.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       26 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/v31/xml.py
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       22 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/aiopenapi3/version.py
-drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-02-10 07:49:49.500840 aiopenapi3-0.2.0/aiopenapi3.egg-info/
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     3842 2023-02-10 07:49:49.000000 aiopenapi3-0.2.0/aiopenapi3.egg-info/PKG-INFO
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1534 2023-02-10 07:49:49.000000 aiopenapi3-0.2.0/aiopenapi3.egg-info/SOURCES.txt
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)        1 2023-02-10 07:49:49.000000 aiopenapi3-0.2.0/aiopenapi3.egg-info/dependency_links.txt
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       57 2023-02-10 07:49:49.000000 aiopenapi3-0.2.0/aiopenapi3.egg-info/entry_points.txt
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      269 2023-02-10 07:49:49.000000 aiopenapi3-0.2.0/aiopenapi3.egg-info/requires.txt
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       11 2023-02-10 07:49:49.000000 aiopenapi3-0.2.0/aiopenapi3.egg-info/top_level.txt
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1050 2023-02-10 07:49:27.000000 aiopenapi3-0.2.0/pyproject.toml
--rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1698 2023-02-10 07:49:49.516840 aiopenapi3-0.2.0/setup.cfg
+drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-06-08 08:04:07.403933 aiopenapi3-0.2.1/
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1519 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/LICENSE
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     3813 2023-06-08 08:04:07.403933 aiopenapi3-0.2.1/PKG-INFO
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2450 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/README.md
+drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-06-08 08:04:07.391933 aiopenapi3-0.2.1/aiopenapi3/
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      599 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/__init__.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       84 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/__main__.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    12784 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/base.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    10719 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/cli.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1991 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/errors.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      578 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/json.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     7406 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/loader.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2592 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/log.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       13 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/me.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    13081 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/model.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    25883 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/openapi.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     4402 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/plugin.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     7071 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/request.py
+drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-06-08 08:04:07.395933 aiopenapi3-0.2.1/aiopenapi3/v20/
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      164 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/__init__.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1228 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/general.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    12398 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/glue.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1184 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/info.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5631 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/parameter.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2994 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/paths.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1637 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/root.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2555 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/schemas.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1369 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/security.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      578 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/tag.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      473 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v20/xml.py
+drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-06-08 08:04:07.399933 aiopenapi3-0.2.1/aiopenapi3/v30/
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      215 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/__init__.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1566 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/components.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      582 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/example.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5683 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/formdata.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1348 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/general.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    18027 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/glue.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1190 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/info.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1408 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/media.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)    10417 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/parameter.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5532 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/paths.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1187 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/root.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     3680 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/schemas.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2654 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/security.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      809 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/servers.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      520 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/tag.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      413 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v30/xml.py
+drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-06-08 08:04:07.403933 aiopenapi3-0.2.1/aiopenapi3/v31/
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       82 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/__init__.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1571 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/components.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      549 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/example.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1461 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/general.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1682 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/info.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1389 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/media.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1684 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/parameter.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     5555 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/paths.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1511 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/root.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     6421 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/schemas.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     2652 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/security.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1104 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/servers.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       26 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/tag.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       26 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/aiopenapi3/v31/xml.py
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       22 2023-06-08 08:03:46.000000 aiopenapi3-0.2.1/aiopenapi3/version.py
+drwxrwxr-x   0 c01mako   (1000) c01mako   (1000)        0 2023-06-08 08:04:07.391933 aiopenapi3-0.2.1/aiopenapi3.egg-info/
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     3813 2023-06-08 08:04:07.000000 aiopenapi3-0.2.1/aiopenapi3.egg-info/PKG-INFO
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1561 2023-06-08 08:04:07.000000 aiopenapi3-0.2.1/aiopenapi3.egg-info/SOURCES.txt
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)        1 2023-06-08 08:04:07.000000 aiopenapi3-0.2.1/aiopenapi3.egg-info/dependency_links.txt
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       57 2023-06-08 08:04:07.000000 aiopenapi3-0.2.1/aiopenapi3.egg-info/entry_points.txt
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)      343 2023-06-08 08:04:07.000000 aiopenapi3-0.2.1/aiopenapi3.egg-info/requires.txt
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)       11 2023-06-08 08:04:07.000000 aiopenapi3-0.2.1/aiopenapi3.egg-info/top_level.txt
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1351 2023-06-08 07:56:26.000000 aiopenapi3-0.2.1/pyproject.toml
+-rw-rw-r--   0 c01mako   (1000) c01mako   (1000)     1739 2023-06-08 08:04:07.403933 aiopenapi3-0.2.1/setup.cfg
```

### Comparing `aiopenapi3-0.2.0/LICENSE` & `aiopenapi3-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/PKG-INFO` & `aiopenapi3-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopenapi3
-Version: 0.2.0
+Version: 0.2.1
 Summary: client and validator for OpenAPI3 3.0, OpenAPI 3.1, Swagger 2.0
 Home-page: https://github.com/commonism/aiopenapi3
 Keywords: openapi openapi3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -17,21 +17,21 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: auth
 Provides-Extra: socks
 License-File: LICENSE
 
 # aiopenapi3
 
 A Python [OpenAPI 3 Specification](https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.3.md) client and validator for Python 3.
```

### Comparing `aiopenapi3-0.2.0/README.md` & `aiopenapi3-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/__init__.py` & `aiopenapi3-0.2.1/aiopenapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/base.py` & `aiopenapi3-0.2.1/aiopenapi3/base.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/cli.py` & `aiopenapi3-0.2.1/aiopenapi3/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,14 @@
         for v in ylc.yaml_implicit_resolvers.values():
             tags |= set([i[0] for i in v])
         log("tags:")
         log("\t" + "\n\t".join(sorted(tags)) + "\n")
 
     path = yarl.URL(args.input)
     if path.scheme in ["http", "https"]:
-
         loader = WebLoader(baseurl=path.with_path("/").with_query({}), yload=ylc, session_factory=session_factory)
     else:
         locations = args.locations or [Path(args.input).parent]
         loader = ChainLoader(*[RedirectLoader(Path(l).expanduser()) for l in locations], yload=ylc)
 
     return loader, ylc
 
@@ -227,15 +226,14 @@
     cmd.add_argument("-a", "--authenticate")
     cmd.add_argument("-p", "--parameters")
     cmd.add_argument("-d", "--data")
     cmd.add_argument("-f", "--format")
     loader_args(cmd)
 
     def cmd_call(args):
-
         loader, _ = loader_prepare(args, session_factory)
 
         def prepare_arg(value):
             if value:
                 if value[0] == "@":
                     with Path(value[1:]).open("rt") as f:
                         data = json.load(f)
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/errors.py` & `aiopenapi3-0.2.1/aiopenapi3/errors.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/json.py` & `aiopenapi3-0.2.1/aiopenapi3/json.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/loader.py` & `aiopenapi3-0.2.1/aiopenapi3/loader.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/log.py` & `aiopenapi3-0.2.1/aiopenapi3/log.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/model.py` & `aiopenapi3-0.2.1/aiopenapi3/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,14 @@
     def from_schema(
         cls,
         schema: "SchemaBase",
         schemanames: List[str] = None,
         discriminators: List["DiscriminatorBase"] = None,
         extra: "SchemaBase" = None,
     ):
-
         if schemanames is None:
             schemanames = []
 
         if discriminators is None:
             discriminators = []
 
         # do not create models for primitive types
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/openapi.py` & `aiopenapi3-0.2.1/aiopenapi3/openapi.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/plugin.py` & `aiopenapi3-0.2.1/aiopenapi3/plugin.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/request.py` & `aiopenapi3-0.2.1/aiopenapi3/request.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/general.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/general.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/glue.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/glue.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,19 @@
 
 from ..base import SchemaBase, ParameterBase
 from ..request import RequestBase, AsyncRequestBase
 from ..errors import HTTPStatusError, ContentTypeError, ResponseSchemaError, ResponseDecodingError
 
 from .parameter import Parameter
 
+try:
+    import httpx_auth
+except:
+    httpx_auth = None
+
 
 class Request(RequestBase):
     @property
     def security(self):
         return self.api._security
 
     @property
@@ -71,17 +76,20 @@
                 sorted(map(lambda x: f"{{{x}}}", [" and ".join(sorted(i.__root__.keys())) for i in security]))
             )
             raise ValueError(
                 f"No security requirement satisfied (accepts {options} given {{{' and '.join(sorted(self.security.keys()))}}})"
             )
 
     def _prepare_secschemes(self, scheme: str, value: Union[str, List[str]]):
-        """
-        https://swagger.io/specification/v2/#security-scheme-object
-        """
+        if httpx_auth is not None:
+            return self._prepare_secschemes_extra(scheme, value)
+        else:
+            return self._prepare_secschemes_default(scheme, value)
+
+    def _prepare_secschemes_default(self, scheme: str, value: Union[str, List[str]]):
         ss = self.root.securityDefinitions[scheme]
 
         if ss.type == "basic":
             value = cast(List[str], value)
             self.req.auth = httpx.BasicAuth(*value)
 
         value = cast(str, value)
@@ -90,14 +98,31 @@
                 # apiKey in query parameter
                 self.req.params[ss.name] = value
 
             if ss.in_ == "header":
                 # apiKey in query header data
                 self.req.headers[ss.name] = value
 
+    def _prepare_secschemes_extra(self, scheme: str, value: Union[str, List[str]]):
+        ss = self.root.securityDefinitions[scheme]
+
+        if ss.type == "basic":
+            value = cast(List[str], value)
+            self.req.auth = httpx_auth.Basic(*value)
+
+        value = cast(str, value)
+        if ss.type == "apiKey":
+            if ss.in_ == "query":
+                # apiKey in query parameter
+                self.req.auth = httpx_auth.QueryApiKey(value, ss.name)
+
+            if ss.in_ == "header":
+                # apiKey in query header data
+                self.req.auth = httpx_auth.HeaderApiKey(value, ss.name)
+
     def _prepare_parameters(self, provided):
         provided = provided or dict()
         possible = {_.name: _ for _ in self.operation.parameters + self.root.paths[self.path].parameters}
 
         parameters = {i.name: i.default for i in filter(lambda x: x.default is not None, possible.values())}
         parameters.update(provided)
 
@@ -118,20 +143,23 @@
         for name, value in parameters.items():
             spec = possible[name]
 
             values = spec._encode(name, value)
             assert isinstance(values, dict)
 
             if spec.in_ == "formData":
-                if "multipart/form-data" not in self.operation.consumes:
-                    raise ValueError(f"operation does not consume form data but parameter {name} is formData")
-                if spec.type == "file":
-                    self.req.files.update(values)
-                else:
+                if "multipart/form-data" in self.operation.consumes:
+                    if spec.type == "file":
+                        self.req.files.update(values)
+                    else:
+                        self.req.data.update(values)
+                elif "application/x-www-form-urlencoded" in self.operation.consumes:
                     self.req.data.update(values)
+                else:
+                    raise ValueError(f"operation does not consume form data but parameter {name} is formData")
 
             if spec.in_ == "path":
                 # The string method `format` is incapable of partial updates,
                 # as such we need to collect all the path parameters before
                 # applying them to the format string.
                 path_parameters.update(values)
 
@@ -276,8 +304,13 @@
                 content_type,
                 f"Unexpected Content-Type {content_type} returned for operation {self.operation.operationId} (expected application/json)",
                 result,
             )
 
 
 class AsyncRequest(Request, AsyncRequestBase):
-    pass
+    def _prepare_secschemes(self, scheme: str, value: Union[str, List[str]]):
+        """
+        httpx_auth does not support async yet
+        https://github.com/Colin-b/httpx_auth/pull/48
+        """
+        return self._prepare_secschemes_default(scheme, value)
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/info.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/info.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/parameter.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
     """
     Describing Parameters
 
     https://swagger.io/docs/specification/2-0/describing-parameters/
     """
 
     def _encode__collection(self, values):
-
         sep = self.SEPERATOR_VALUES.get(self.collectionFormat, None)
         if sep:
             if self.type == "array":
                 values = [self.items._encode(None, i) for i in values]
             return sep.join(map(str, values))
         elif self.collectionFormat == "multi":
             # foo=value&foo=another_value
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/paths.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/paths.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/root.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/root.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/schemas.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/schemas.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/security.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/security.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v20/tag.py` & `aiopenapi3-0.2.1/aiopenapi3/v20/tag.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/components.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/components.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/example.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/example.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/general.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/general.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/glue.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/glue.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,37 @@
 from typing import List, Union, cast
 import json
+import urllib.parse
 
 import httpx
+
+try:
+    import httpx_auth
+    from httpx_auth.authentication import SupportMultiAuth
+except:
+    httpx_auth = None
+
+if httpx_auth is not None:
+    import inspect
+
+    HTTPX_AUTH_METHODS = {
+        name.lower(): getattr(httpx_auth, name)
+        for name in httpx_auth.__all__
+        if inspect.isclass((class_ := getattr(httpx_auth, name)))
+        if issubclass(class_, httpx.Auth)
+    }
+
 import pydantic
 import pydantic.json
 
+import aiopenapi3.v30.media
 from ..base import SchemaBase, ParameterBase
 from ..request import RequestBase, AsyncRequestBase
 from ..errors import HTTPStatusError, ContentTypeError, ResponseDecodingError, ResponseSchemaError
+from .formdata import parameters_from_multipart, parameters_from_urlencoded, encode_multipart_parameters
 
 
 class Request(RequestBase):
     """
     This class is returned by instances of the OpenAPI class when members
     formatted like call_operationId are accessed, and a valid Operation is
     found, and allows calling the operation directly from the OpenAPI object
@@ -69,26 +89,33 @@
                 sorted(map(lambda x: f"{{{x}}}", [" and ".join(sorted(i.__root__.keys())) for i in security]))
             )
             raise ValueError(
                 f"No security requirement satisfied (accepts {options} given {{{' and '.join(sorted(self.security.keys()))}}}"
             )
 
     def _prepare_secschemes(self, scheme: str, value: Union[str, List[str]]):
-        ss = self.root.components.securitySchemes[scheme]
+        if httpx_auth is not None:
+            return self._prepare_secschemes_extra(scheme, value)
+        else:
+            return self._prepare_secschemes_default(scheme, value)
 
-        if ss.type == "http" and ss.scheme_ == "basic":
-            self.req.auth = httpx.BasicAuth(*value)
+    def _prepare_secschemes_default(self, scheme: str, value: Union[str, List[str]]):
+        ss = self.root.components.securitySchemes[scheme]
 
-        if ss.type == "http" and ss.scheme_ == "digest":
-            self.req.auth = httpx.DigestAuth(*value)
+        if ss.type == "http":
+            if ss.scheme_ == "basic":
+                self.req.auth = httpx.BasicAuth(*value)
+            elif ss.scheme_ == "digest":
+                self.req.auth = httpx.DigestAuth(*value)
+            elif ss.scheme_ == "bearer":
+                self.req.headers["Authorization"] = f"Bearer {value:s}"
+            else:
+                raise ValueError(f"Authentication {ss.type}/{ss.scheme_} is not supported.")
 
         value = cast(str, value)
-        if ss.type == "http" and ss.scheme_ == "bearer":
-            header = ss.bearerFormat or "Bearer {}"
-            self.req.headers["Authorization"] = header.format(value)
 
         if ss.type == "mutualTLS":
             # TLS Client certificates (mutualTLS)
             self.req.cert = value
 
         if ss.type == "apiKey":
             if ss.in_ == "query":
@@ -98,25 +125,109 @@
             if ss.in_ == "header":
                 # apiKey in query header data
                 self.req.headers[ss.name] = value
 
             if ss.in_ == "cookie":
                 self.req.cookies = {ss.name: value}
 
+    def _prepare_secschemes_extra(self, scheme: str, value: Union[str, List[str]]):
+        ss = self.root.components.securitySchemes[scheme]
+        auths = []
+
+        if ss.type == "oauth2":
+            # NOTE: refresh_url is not currently supported by httpx_auth
+            # REF: https://github.com/Colin-b/httpx_auth/issues/17
+            if flow := ss.flows.implicit:
+                auths.append(
+                    httpx_auth.OAuth2Implicit(
+                        **value,
+                        authorization_url=flow.authorizationUrl,
+                        scopes=flow.scopes,
+                        # refresh_url=flow.refreshUrl,
+                    )
+                )
+            if flow := ss.flows.password:
+                auths.append(
+                    httpx_auth.OAuth2ResourceOwnerPasswordCredentials(
+                        **value,
+                        token_url=flow.tokenUrl,
+                        scopes=flow.scopes,
+                        # refresh_url=flow.refreshUrl,
+                    )
+                )
+            if flow := ss.flows.clientCredentials:
+                auths.append(
+                    httpx_auth.OAuth2ClientCredentials(
+                        **value,
+                        token_url=flow.tokenUrl,
+                        scopes=flow.scopes,
+                        # refresh_url=flow.refreshUrl,
+                    )
+                )
+            if flow := ss.flows.authorizationCode:
+                auths.append(
+                    httpx_auth.OAuth2AuthorizationCode(
+                        **value,
+                        authorization_url=flow.authorizationUrl,
+                        token_url=flow.tokenUrl,
+                        scopes=flow.scopes,
+                        # refresh_url=flow.refreshUrl,
+                    )
+                )
+
+        if ss.type == "http":
+            if auth := HTTPX_AUTH_METHODS.get(ss.scheme_, None):
+                if isinstance(value, tuple):
+                    auths.append(auth(*value))
+                elif isinstance(value, dict):
+                    auths.append(auth(**value))
+            elif ss.scheme_ == "bearer":
+                auths.append(httpx_auth.HeaderApiKey(f"Bearer {value}", "Authorization"))
+            else:
+                raise ValueError(f"Authentication method {ss.type}/{ss.scheme_} is not supported by httpx-auth")
+
+        value = cast(str, value)
+
+        if ss.type == "mutualTLS":
+            # TLS Client certificates (mutualTLS)
+            self.req.cert = value
+
+        if ss.type == "apiKey":
+            if auth := HTTPX_AUTH_METHODS.get((ss.in_ + ss.type).lower(), None):
+                auths.append(auth(value, ss.name))
+
+            if ss.in_ == "cookie":
+                self.req.cookies = {ss.name: value}
+
+        for auth in auths:
+            if self.req.auth and isinstance(self.req.auth, SupportMultiAuth):
+                self.req.auth += auth
+            else:
+                self.req.auth = auth
+
     def _prepare_parameters(self, provided):
         """
         assigns the parameters provided to the header/path/cookie …
 
         FIXME: handle parameter location
           https://spec.openapis.org/oas/v3.0.3#parameter-object
           A unique parameter is defined by a combination of a name and location.
         """
+
         provided = provided or dict()
         possible = {_.name: _ for _ in self.operation.parameters + self.root.paths[self.path].parameters}
 
+        if self.operation.requestBody:
+            rbq = dict()  # requestBody Parameters
+            ct = "multipart/form-data"
+            if ct in self.operation.requestBody.content:
+                for k, v in self.operation.requestBody.content[ct].encoding.items():
+                    rbq.update(v.headers)
+                possible.update(rbq)
+
         parameters = {
             i.name: i.schema_.default for i in filter(lambda x: x.schema_.default is not None, possible.values())
         }
         parameters.update(provided)
 
         available = frozenset(parameters.keys())
         accepted = frozenset(possible.keys())
@@ -125,37 +236,38 @@
             raise ValueError(f"Parameter {sorted(available - accepted)} unknown (accepted {sorted(accepted)})")
         if required - available:
             raise ValueError(
                 f"Required Parameter {sorted(required - available)} missing (provided {sorted(available)})"
             )
 
         path_parameters = {}
-
+        rbqh = dict()
         for name, value in parameters.items():
             spec = possible[name]
             values = spec._encode(name, value)
             assert isinstance(values, dict)
-            if spec.in_ == "path":
+
+            if isinstance(spec, (aiopenapi3.v30.parameter.Header, aiopenapi3.v31.parameter.Header)):
+                rbqh.update(values)
+            elif spec.in_ == "header":
+                self.req.headers.update(values)
+            elif spec.in_ == "path":
                 # The string method `format` is incapable of partial updates,
                 # as such we need to collect all the path parameters before
                 # applying them to the format string.
                 path_parameters.update(values)
-
-            if spec.in_ == "query":
+            elif spec.in_ == "query":
                 self.req.params.update(values)
-
-            if spec.in_ == "header":
-                self.req.headers.update(values)
-
-            if spec.in_ == "cookie":
+            elif spec.in_ == "cookie":
                 self.req.cookies.update(values)
 
         self.req.url = self.req.url.format(**path_parameters)
+        return rbqh
 
-    def _prepare_body(self, data):
+    def _prepare_body(self, data, rbq):
         if not self.operation.requestBody:
             return
 
         if data is None and self.operation.requestBody.required:
             raise ValueError("Request Body is required but none was provided.")
 
         if "application/json" in self.operation.requestBody.content:
@@ -169,31 +281,45 @@
                 operationId=self.operation.operationId, marshalled=data
             ).marshalled
             data = json.dumps(data, default=pydantic.json.pydantic_encoder)
             data = data.encode()
             data = self.api.plugins.message.sending(operationId=self.operation.operationId, sending=data).sending
             self.req.content = data
             self.req.headers["Content-Type"] = "application/json"
-        #        elif "multipart/form-data" in self.operation.requestBody.content:
-        #            """
-        #            https://swagger.io/docs/specification/describing-request-body/multipart-requests/
-        #            """
-        #            pass
-        #        elif "multipart/mixed" in self.operation.requestBody.content:
-        #            pass
-        #        elif "multipart/form-data" in self.operation.requestBody.content:
-        #            pass
-
+        elif (ct := "multipart/form-data") in self.operation.requestBody.content:
+            """
+            https://swagger.io/docs/specification/describing-request-body/multipart-requests/
+            https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md#media-type-object
+            """
+            media: aiopenapi3.v30.media.MediaType = self.operation.requestBody.content[ct]
+            if not media.schema_ or not isinstance(data, media.schema_.get_type()):
+                """expect the data to be a model"""
+                raise TypeError((type(data), media.schema_.get_type()))
+
+            params = parameters_from_multipart(data, media, rbq)
+            msg = encode_multipart_parameters(params)
+            self.req.content = msg.as_string()
+            self.req.headers["Content-Type"] = f'{msg.get_content_type()}; boundary="{msg.get_boundary()}"'
+        elif (ct := "application/x-www-form-urlencoded") in self.operation.requestBody.content:
+            self.req.headers["Content-Type"] = ct
+            media: aiopenapi3.v30.media.MediaType = self.operation.requestBody.content[ct]
+            if not media.schema_ or not isinstance(data, media.schema_.get_type()):
+                """expect the data to be a model"""
+                raise TypeError((type(data), media.schema_.get_type()))
+
+            params = parameters_from_urlencoded(data, media)
+            msg = urllib.parse.urlencode(params, doseq=True)
+            self.req.content = msg
         else:
-            raise NotImplementedError()
+            raise NotImplementedError(self.operation.requestBody.content)
 
     def _prepare(self, data, parameters):
         self._prepare_security()
-        self._prepare_parameters(parameters)
-        self._prepare_body(data)
+        rbq = self._prepare_parameters(parameters)
+        self._prepare_body(data, rbq)
 
     def _build_req(self, session):
         req = session.build_request(
             self.method,
             str(self.api.url / self.req.url[1:]),
             headers=self.req.headers,
             cookies=self.req.cookies,
@@ -276,15 +402,14 @@
                 content_type,
                 f"Unexpected Content-Type {content_type} returned for operation {self.operation.operationId} \
                          (expected one of {options})",
                 result,
             )
 
         if content_type.lower() == "application/json":
-
             data = ctx.received
             try:
                 data = json.loads(data)
             except json.decoder.JSONDecodeError:
                 raise ResponseDecodingError(self.operation, result, data)
             data = self.api.plugins.message.parsed(
                 operationId=self.operation.operationId,
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/info.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/info.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/media.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/media.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/parameter.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import enum
+import datetime
+import decimal
+import uuid
 from typing import Union, Optional, Dict, Any
 
 from pydantic import Field, root_validator
 import more_itertools
 
 from ..base import ObjectExtended, ParameterBase as ParameterBase_
 from ..errors import ParameterFormatError
@@ -66,15 +69,14 @@
             value = ",".join([f"{k},{v}" for k, v in values.items()])
             if explode is False:
                 # ;color=R,100,G,200,B,150
                 value = f";{name}={value}"
             else:
                 # ;R=100;G=200;B=150
                 value = f";{value}"
-            pass
         return {name: value}
 
     def _encode__label(self, name, value, explode):
         """
         3.2.5.  Label Expansion with Dot-Prefix: {.var}
 
         https://www.rfc-editor.org/rfc/rfc6570#section-3.2.8
@@ -85,15 +87,14 @@
                 value = f".{value}"
             else:
                 value = "."
         elif self.schema_.type == "array":
             # .blue.black.brown
             value = "." + ".".join(value)
         elif self.schema_.type == "object":
-
             values = value if isinstance(value, dict) else dict(value._iter(to_dict=True))
             if explode:
                 # .R=100.G=200.B=150
                 value = ".".join([f"{k}={v}" for k, v in values.items()])
             else:
                 # .R.100.G.200.B.150
                 value = ".".join([f"{k}.{v}" for k, v in values.items()])
@@ -253,14 +254,26 @@
 
 
 class Parameter(ParameterBase, _ParameterCodec):
     name: str = Field(required=True)
     in_: _In = Field(required=True, alias="in")  # TODO must be one of ["query","header","path","cookie"]
 
 
+def encode_parameter(
+    name: str, value: object, style: str, explode: bool, allowReserved: bool, in_: str, schema_: Schema
+) -> Union[str, bytes]:
+    p = Parameter(name=name, style=style, explode=explode, allowReserved=allowReserved, **{"in": in_, "schema": None})
+    p.schema_ = schema_
+    r = p._encode(name, value)[name]
+    if isinstance(r, (int, float, decimal.Decimal, datetime.datetime, datetime.date, datetime.time, uuid.UUID)):
+        r = str(r)
+    assert isinstance(r, (str, bytes))
+    return r
+
+
 class Header(ParameterBase, _ParameterCodec):
     """
 
     .. _HeaderObject: https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.3.md#header-object
     """
 
     def _codec(self):
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/paths.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/paths.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/root.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/root.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/schemas.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/schemas.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/security.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Dict, List
 
-from pydantic import Field, root_validator, BaseModel
+from pydantic import BaseModel, constr, Field, root_validator
 
 from ..base import ObjectExtended
 
 
 class OAuthFlow(ObjectExtended):
     """
     Configuration details for a supported OAuth Flow
@@ -38,15 +38,15 @@
     .. _Security Scheme: https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.3.md#security-scheme-object
     """
 
     type: str = Field(...)
     description: Optional[str] = Field(default=None)
     name: Optional[str] = Field(default=None)
     in_: Optional[str] = Field(default=None, alias="in")
-    scheme_: Optional[str] = Field(default=None, alias="scheme")
+    scheme_: Optional[constr(to_lower=True)] = Field(default=None, alias="scheme")
     bearerFormat: Optional[str] = Field(default=None)
     flows: Optional[OAuthFlows] = Field(default=None)
     openIdConnectUrl: Optional[str] = Field(default=None)
 
     @root_validator
     def validate_SecurityScheme(cls, values):
         t = values.get("type", None)
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/servers.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/servers.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v30/tag.py` & `aiopenapi3-0.2.1/aiopenapi3/v30/tag.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/components.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/components.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/example.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/example.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/general.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/general.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/info.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/info.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,14 @@
 
     name: str = Field(...)
     identifier: Optional[str] = Field(default=None)
     url: Optional[AnyUrl] = Field(default=None)
 
     @root_validator
     def validate_License(cls, values):
-
         """
         A URL to the license used for the API. This MUST be in the form of a URL. The url field is mutually exclusive of the identifier field.
         """
         assert not all([values.get(i, None) is not None for i in ["identifier", "url"]])
         return values
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/media.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/media.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/parameter.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/parameter.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/paths.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/paths.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/root.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/root.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/schemas.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/schemas.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/security.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/security.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from typing import Optional, Dict, List
 
-from pydantic import Field, root_validator, BaseModel
+from pydantic import Field, root_validator, BaseModel, constr
 
 from ..base import ObjectExtended
 
 
 class OAuthFlow(ObjectExtended):
     """
     Configuration details for a supported OAuth Flow
@@ -38,15 +38,15 @@
     .. _Security Scheme: https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.1.0.md#security-scheme-object
     """
 
     type: str = Field(...)
     description: Optional[str] = Field(default=None)
     name: Optional[str] = Field(default=None)
     in_: Optional[str] = Field(default=None, alias="in")
-    scheme_: Optional[str] = Field(default=None, alias="scheme")
+    scheme_: Optional[constr(to_lower=True)] = Field(default=None, alias="scheme")
     bearerFormat: Optional[str] = Field(default=None)
     flows: Optional[OAuthFlows] = Field(default=None)
     openIdConnectUrl: Optional[str] = Field(default=None)
 
     @root_validator
     def validate_SecurityScheme(cls, values):
         t = values.get("type", None)
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3/v31/servers.py` & `aiopenapi3-0.2.1/aiopenapi3/v31/servers.py`

 * *Files identical despite different names*

### Comparing `aiopenapi3-0.2.0/aiopenapi3.egg-info/PKG-INFO` & `aiopenapi3-0.2.1/aiopenapi3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiopenapi3
-Version: 0.2.0
+Version: 0.2.1
 Summary: client and validator for OpenAPI3 3.0, OpenAPI 3.1, Swagger 2.0
 Home-page: https://github.com/commonism/aiopenapi3
 Keywords: openapi openapi3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Web Environment
 Classifier: Framework :: AsyncIO
 Classifier: Intended Audience :: Developers
@@ -17,21 +17,21 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 Provides-Extra: tests
+Provides-Extra: auth
 Provides-Extra: socks
 License-File: LICENSE
 
 # aiopenapi3
 
 A Python [OpenAPI 3 Specification](https://github.com/OAI/OpenAPI-Specification/blob/main/versions/3.0.3.md) client and validator for Python 3.
```

### Comparing `aiopenapi3-0.2.0/aiopenapi3.egg-info/SOURCES.txt` & `aiopenapi3-0.2.1/aiopenapi3.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,15 @@
 aiopenapi3/v20/schemas.py
 aiopenapi3/v20/security.py
 aiopenapi3/v20/tag.py
 aiopenapi3/v20/xml.py
 aiopenapi3/v30/__init__.py
 aiopenapi3/v30/components.py
 aiopenapi3/v30/example.py
+aiopenapi3/v30/formdata.py
 aiopenapi3/v30/general.py
 aiopenapi3/v30/glue.py
 aiopenapi3/v30/info.py
 aiopenapi3/v30/media.py
 aiopenapi3/v30/parameter.py
 aiopenapi3/v30/paths.py
 aiopenapi3/v30/root.py
```

### Comparing `aiopenapi3-0.2.0/pyproject.toml` & `aiopenapi3-0.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -10,10 +10,16 @@
     "ignore:unclosed file <_io.FileIO name='/tmp/aiopenapi3-debug.log' mode='ab' closefd=True>:ResourceWarning",
     "ignore:unclosed file <_io.TextIOWrapper name='/tmp/aiopenapi3-debug.log' mode='a' encoding='UTF-8'>:ResourceWarning",
     "ignore:unclosed <ssl.SSLSocket:ResourceWarning",
     "ignore:unclosed <socket.socket fd=:ResourceWarning",
     "ignore:Ignoring Schema with additionalProperties and named properties:UserWarning",
 #    "error::pytest.PytestUnraisableExceptionWarning",
     # note the use of single quote below to denote "raw" strings in TOML
-    'ignore:The loop argument is deprecated since Python 3.8, and scheduled for removal in Python 3.10.:DeprecationWarning',
+#    'ignore:The loop argument is deprecated since Python 3.8, and scheduled for removal in Python 3.10.:DeprecationWarning',
+    "ignore:'flask.Markup' is deprecated and will be removed in Flask 2.4. Import 'markupsafe.Markup' instead.:DeprecationWarning"
 ]
 asyncio_mode = "strict"
+
+log_cli = "yes"
+log_cli_level = "DEBUG"
+log_cli_format = "%(asctime)s [%(levelname)8s] %(message)s (%(filename)s:%(lineno)s)"
+log_cli_date_format = "%Y-%m-%d %H:%M:%S"
```

### Comparing `aiopenapi3-0.2.0/setup.cfg` & `aiopenapi3-0.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 	Topic :: Software Development
 	Topic :: Software Development :: Libraries
 	Topic :: Software Development :: Libraries :: Application Frameworks
 	Topic :: Software Development :: Libraries :: Python Modules
 	Typing :: Typed
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
 
 [options]
 packages = 
@@ -37,15 +36,15 @@
 	aiopenapi3.v20
 	aiopenapi3.v30
 	aiopenapi3.v31
 install_requires = 
 	PyYaml
 	pydantic<=1.11.0
 	pydantic[email]
-	yarl
+	yarl==1.8.1
 	httpx
 	more-itertools
 	typing_extensions; python_version<"3.8"
 	pathlib3x; python_version<"3.9"
 	jmespath
 
 [options.entry_points]
@@ -57,14 +56,21 @@
 	pytest
 	pytest-asyncio
 	pytest-httpx
 	pytest-cov
 	fastapi-versioning
 	hypercorn
 	uvloop
+	flask
+	flask_bootstrap
+	flask_wtf
+	wtforms
+	asgiref
+auth = 
+	httpx-auth
 socks = 
 	httpx_socks
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

