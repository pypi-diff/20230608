# Comparing `tmp/pars_avito-0.1.tar.gz` & `tmp/pars_avito-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pars_avito-0.1.tar", last modified: Thu Jun  8 21:42:36 2023, max compression
+gzip compressed data, was "pars_avito-0.2.tar", last modified: Thu Jun  8 21:16:36 2023, max compression
```

## Comparing `pars_avito-0.1.tar` & `pars_avito-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:42:36.418911 pars_avito-0.1/
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-08 21:42:36.418911 pars_avito-0.1/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)     1115 2023-06-08 21:40:29.000000 pars_avito-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:42:36.414911 pars_avito-0.1/pars_avito/
--rw-rw-r--   0 root         (0) root         (0)      156 2023-06-08 21:14:53.000000 pars_avito-0.1/pars_avito/__init__.py
--rw-rw-r--   0 root         (0) root         (0)     1259 2023-06-08 16:35:21.000000 pars_avito-0.1/pars_avito/pars_avito.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:42:36.414911 pars_avito-0.1/pars_avito.egg-info/
--rw-r--r--   0 root         (0) root         (0)      309 2023-06-08 21:42:36.000000 pars_avito-0.1/pars_avito.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      235 2023-06-08 21:42:36.000000 pars_avito-0.1/pars_avito.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:42:36.000000 pars_avito-0.1/pars_avito.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 21:42:36.000000 pars_avito-0.1/pars_avito.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 21:42:36.000000 pars_avito-0.1/pars_avito.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:42:36.418911 pars_avito-0.1/setup.cfg
--rw-rw-r--   0 root         (0) root         (0)      495 2023-06-08 21:41:40.000000 pars_avito-0.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:16:36.331644 pars_avito-0.2/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-08 21:16:36.331644 pars_avito-0.2/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)        0 2023-06-08 12:21:10.000000 pars_avito-0.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:16:36.331644 pars_avito-0.2/pars_avito/
+-rw-rw-r--   0 root         (0) root         (0)      156 2023-06-08 21:14:53.000000 pars_avito-0.2/pars_avito/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1259 2023-06-08 16:35:21.000000 pars_avito-0.2/pars_avito/pars_avito.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 21:16:36.331644 pars_avito-0.2/pars_avito.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      204 2023-06-08 21:16:36.000000 pars_avito-0.2/pars_avito.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      235 2023-06-08 21:16:36.000000 pars_avito-0.2/pars_avito.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 21:16:36.000000 pars_avito-0.2/pars_avito.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 21:16:36.000000 pars_avito-0.2/pars_avito.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-06-08 21:16:36.000000 pars_avito-0.2/pars_avito.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-08 21:16:36.331644 pars_avito-0.2/setup.cfg
+-rw-rw-r--   0 root         (0) root         (0)      315 2023-06-08 21:14:57.000000 pars_avito-0.2/setup.py
```

### Comparing `pars_avito-0.1/pars_avito/pars_avito.py` & `pars_avito-0.2/pars_avito/pars_avito.py`

 * *Files identical despite different names*

