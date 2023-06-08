# Comparing `tmp/predictapi-0.0.3.tar.gz` & `tmp/predictapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "predictapi-0.0.3.tar", last modified: Thu Jun  8 09:43:11 2023, max compression
+gzip compressed data, was "predictapi-0.0.4.tar", last modified: Thu Jun  8 10:00:50 2023, max compression
```

## Comparing `predictapi-0.0.3.tar` & `predictapi-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,9 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 09:43:11.131833 predictapi-0.0.3/
--rw-rw-rw-   0        0        0      351 2023-06-08 09:43:11.132833 predictapi-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 09:43:11.125517 predictapi-0.0.3/predictapi.egg-info/
--rw-rw-rw-   0        0        0      351 2023-06-08 09:43:11.000000 predictapi-0.0.3/predictapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2023-06-08 09:43:11.000000 predictapi-0.0.3/predictapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 09:43:11.000000 predictapi-0.0.3/predictapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-06-08 09:43:11.000000 predictapi-0.0.3/predictapi.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      100 2023-06-08 08:45:45.000000 predictapi-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0      432 2023-06-08 09:43:11.144866 predictapi-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      127 2023-06-08 09:42:29.000000 predictapi-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 09:43:11.129799 predictapi-0.0.3/src/
--rw-rw-rw-   0        0        0       27 2023-06-08 08:25:58.000000 predictapi-0.0.3/src/__init__.py
--rw-rw-rw-   0        0        0     1003 2023-06-08 08:34:14.000000 predictapi-0.0.3/src/predict.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:50.250989 predictapi-0.0.4/
+-rw-rw-rw-   0        0        0      132 2023-06-08 10:00:50.247989 predictapi-0.0.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 10:00:50.243486 predictapi-0.0.4/predictapi.egg-info/
+-rw-rw-rw-   0        0        0      132 2023-06-08 10:00:50.000000 predictapi-0.0.4/predictapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      144 2023-06-08 10:00:50.000000 predictapi-0.0.4/predictapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:00:50.000000 predictapi-0.0.4/predictapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:00:50.000000 predictapi-0.0.4/predictapi.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:00:50.251987 predictapi-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      236 2023-06-08 09:59:50.000000 predictapi-0.0.4/setup.py
```

