# Comparing `tmp/text_mods-1.40.tar.gz` & `tmp/text_mods-1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
+gzip compressed data, was "text_mods-1.41.tar", last modified: Thu Jun  8 00:39:27 2023, max compression
```

## Comparing `text_mods-1.40.tar` & `text_mods-1.41.tar`

### file list

```diff
@@ -1,18 +1,9 @@
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 text_mods-1.40/src/Example.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 text_mods-1.40/src/__init__.py
--rw-r--r--   0        0        0      131 2020-02-02 00:00:00.000000 text_mods-1.40/src/setup.py
--rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.py
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 text_mods-1.40/src/dist/text_mods-1.30-py3-none-any.whl
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 text_mods-1.40/src/dist/text_mods-1.30.tar.gz
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/PKG-INFO
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/src/text_mods.egg-info/top_level.txt
--rw-r--r--   0        0        0       54 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/PKG-INFO
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/SOURCES.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/dependency_links.txt
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 text_mods-1.40/text_mods.egg-info/top_level.txt
--rw-r--r--   0        0        0     2558 2020-02-02 00:00:00.000000 text_mods-1.40/LICENSE.txt
--rw-r--r--   0        0        0     2527 2020-02-02 00:00:00.000000 text_mods-1.40/README.md
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 text_mods-1.40/pyproject.toml
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 text_mods-1.40/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 00:39:27.037390 text_mods-1.41/
+-rw-rw-rw-   0        0        0       55 2023-06-08 00:39:27.036385 text_mods-1.41/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-08 00:39:27.037390 text_mods-1.41/setup.cfg
+-rw-rw-rw-   0        0        0      131 2023-06-08 00:39:07.000000 text_mods-1.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 00:39:27.036385 text_mods-1.41/text_mods.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-06-08 00:39:27.000000 text_mods-1.41/text_mods.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      140 2023-06-08 00:39:27.000000 text_mods-1.41/text_mods.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 00:39:27.000000 text_mods-1.41/text_mods.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 00:39:27.000000 text_mods-1.41/text_mods.egg-info/top_level.txt
```

