# Comparing `tmp/predictapi-0.0.1.tar.gz` & `tmp/predictapi-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictapi-0.0.1.tar", last modified: Thu Jun  8 09:12:54 2023, max compression
+gzip compressed data, was "predictapi-0.0.2.tar", last modified: Thu Jun  8 09:29:08 2023, max compression
```

## Comparing `predictapi-0.0.1.tar` & `predictapi-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:54.112434 predictapi-0.0.1/
--rw-rw-rw-   0        0        0      351 2023-06-08 09:12:54.113430 predictapi-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:54.098433 predictapi-0.0.1/predictapi.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-08 09:12:54.000000 predictapi-0.0.1/predictapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      205 2023-06-08 09:12:54.000000 predictapi-0.0.1/predictapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:12:54.000000 predictapi-0.0.1/predictapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-08 09:12:54.000000 predictapi-0.0.1/predictapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      100 2023-06-08 08:45:45.000000 predictapi-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      432 2023-06-08 09:12:54.115429 predictapi-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:54.107434 predictapi-0.0.1/src/
--rw-rw-rw-   0        0        0       27 2023-06-08 08:25:58.000000 predictapi-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-06-08 08:34:14.000000 predictapi-0.0.1/src/predict.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:12:54.111432 predictapi-0.0.1/tests/
--rw-rw-rw-   0        0        0       39 2023-06-08 08:46:40.000000 predictapi-0.0.1/tests/test.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:29:08.475372 predictapi-0.0.2/
+-rw-rw-rw-   0        0        0      351 2023-06-08 09:29:08.475372 predictapi-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 09:29:08.467259 predictapi-0.0.2/predictapi.egg-info/
+-rw-rw-rw-   0        0        0      351 2023-06-08 09:29:08.000000 predictapi-0.0.2/predictapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2023-06-08 09:29:08.000000 predictapi-0.0.2/predictapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:29:08.000000 predictapi-0.0.2/predictapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-06-08 09:29:08.000000 predictapi-0.0.2/predictapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      100 2023-06-08 08:45:45.000000 predictapi-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0      432 2023-06-08 09:29:08.478376 predictapi-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0       38 2023-02-23 12:59:44.000000 predictapi-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:29:08.473375 predictapi-0.0.2/src/
+-rw-rw-rw-   0        0        0       27 2023-06-08 08:25:58.000000 predictapi-0.0.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1003 2023-06-08 08:34:14.000000 predictapi-0.0.2/src/predict.py
```

### Comparing `predictapi-0.0.1/src/predict.py` & `predictapi-0.0.2/src/predict.py`

 * *Files identical despite different names*

