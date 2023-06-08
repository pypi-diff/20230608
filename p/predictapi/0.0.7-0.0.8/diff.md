# Comparing `tmp/predictapi-0.0.7.tar.gz` & `tmp/predictapi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictapi-0.0.7.tar", last modified: Thu Jun  8 10:14:51 2023, max compression
+gzip compressed data, was "predictapi-0.0.8.tar", last modified: Thu Jun  8 10:18:49 2023, max compression
```

## Comparing `predictapi-0.0.7.tar` & `predictapi-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 10:14:50.998795 predictapi-0.0.7/
--rw-rw-rw-   0        0        0      132 2023-06-08 10:14:50.997503 predictapi-0.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 10:14:50.996505 predictapi-0.0.7/predictapi.egg-info/
--rw-rw-rw-   0        0        0      132 2023-06-08 10:14:50.000000 predictapi-0.0.7/predictapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      144 2023-06-08 10:14:50.000000 predictapi-0.0.7/predictapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:14:50.000000 predictapi-0.0.7/predictapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:14:50.000000 predictapi-0.0.7/predictapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 10:14:50.998795 predictapi-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      236 2023-06-08 10:14:46.000000 predictapi-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:18:49.900866 predictapi-0.0.8/
+-rw-rw-rw-   0        0        0      132 2023-06-08 10:18:49.899869 predictapi-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:18:49.900866 predictapi-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      268 2023-06-08 10:18:22.000000 predictapi-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:18:49.879350 predictapi-0.0.8/src/
+-rw-rw-rw-   0        0        0       30 2023-06-08 09:47:19.000000 predictapi-0.0.8/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:18:49.898868 predictapi-0.0.8/src/predictapi.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-06-08 10:18:49.000000 predictapi-0.0.8/src/predictapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      231 2023-06-08 10:18:49.000000 predictapi-0.0.8/src/predictapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:18:49.000000 predictapi-0.0.8/src/predictapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 10:18:49.000000 predictapi-0.0.8/src/predictapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2023-06-08 10:18:49.000000 predictapi-0.0.8/src/predictapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1003 2023-06-08 08:34:14.000000 predictapi-0.0.8/src/predictapi.py
```

