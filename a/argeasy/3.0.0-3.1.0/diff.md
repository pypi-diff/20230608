# Comparing `tmp/argeasy-3.0.0.tar.gz` & `tmp/argeasy-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "argeasy-3.0.0.tar", last modified: Fri Oct 14 04:48:22 2022, max compression
+gzip compressed data, was "argeasy-3.1.0.tar", last modified: Thu Jun  8 17:17:32 2023, max compression
```

## Comparing `argeasy-3.0.0.tar` & `argeasy-3.1.0.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2022-10-14 04:48:22.003314 argeasy-3.0.0/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2941 2022-10-14 04:48:22.003314 argeasy-3.0.0/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1998 2022-10-14 04:42:18.000000 argeasy-3.0.0/README.md
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2022-10-14 04:48:21.995314 argeasy-3.0.0/argeasy/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       83 2022-10-14 04:39:09.000000 argeasy-3.0.0/argeasy/__init__.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     8720 2022-10-14 04:46:24.000000 argeasy-3.0.0/argeasy/argeasy.py
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      288 2022-10-12 01:05:59.000000 argeasy-3.0.0/argeasy/exceptions.py
-drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2022-10-14 04:48:22.003314 argeasy-3.0.0/argeasy.egg-info/
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2941 2022-10-14 04:48:21.000000 argeasy-3.0.0/argeasy.egg-info/PKG-INFO
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      203 2022-10-14 04:48:21.000000 argeasy-3.0.0/argeasy.egg-info/SOURCES.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2022-10-14 04:48:21.000000 argeasy-3.0.0/argeasy.egg-info/dependency_links.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        8 2022-10-14 04:48:21.000000 argeasy-3.0.0/argeasy.egg-info/top_level.txt
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2022-10-14 04:48:22.003314 argeasy-3.0.0/setup.cfg
--rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      670 2022-10-14 04:47:32.000000 argeasy-3.0.0/setup.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-08 17:17:32.311860 argeasy-3.1.0/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2145 2023-06-08 17:17:32.307860 argeasy-3.1.0/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     1204 2023-06-08 17:09:37.000000 argeasy-3.1.0/README.md
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-08 17:17:32.299860 argeasy-3.1.0/argeasy/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       85 2023-06-08 17:16:58.000000 argeasy-3.1.0/argeasy/__init__.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     6687 2023-06-08 17:12:17.000000 argeasy-3.1.0/argeasy/argeasy.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      462 2023-06-07 18:32:30.000000 argeasy-3.1.0/argeasy/arguments.py
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      116 2023-06-07 20:12:02.000000 argeasy-3.1.0/argeasy/exceptions.py
+drwxrwxr-x   0 pysproxy  (1000) pysproxy  (1000)        0 2023-06-08 17:17:32.307860 argeasy-3.1.0/argeasy.egg-info/
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)     2145 2023-06-08 17:17:31.000000 argeasy-3.1.0/argeasy.egg-info/PKG-INFO
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      224 2023-06-08 17:17:32.000000 argeasy-3.1.0/argeasy.egg-info/SOURCES.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        1 2023-06-08 17:17:31.000000 argeasy-3.1.0/argeasy.egg-info/dependency_links.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)        8 2023-06-08 17:17:31.000000 argeasy-3.1.0/argeasy.egg-info/top_level.txt
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)       38 2023-06-08 17:17:32.311860 argeasy-3.1.0/setup.cfg
+-rw-rw-r--   0 pysproxy  (1000) pysproxy  (1000)      938 2023-06-08 17:16:46.000000 argeasy-3.1.0/setup.py
```

