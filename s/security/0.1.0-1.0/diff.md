# Comparing `tmp/security-0.1.0.tar.gz` & `tmp/security-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "security-0.1.0.tar", last modified: Thu Jun  8 14:25:52 2023, max compression
+gzip compressed data, was "security-1.0.0.tar", last modified: Thu Jun  8 14:31:52 2023, max compression
```

## Comparing `security-0.1.0.tar` & `security-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:25:52.582738 security-0.1.0/
--rw-r--r--   0 dani       (501) staff       (20)     1096 2023-06-08 14:04:42.000000 security-0.1.0/LICENSE.txt
--rw-r--r--   0 dani       (501) staff       (20)       29 2023-06-08 14:02:06.000000 security-0.1.0/MANIFEST.in
--rw-r--r--   0 dani       (501) staff       (20)     1594 2023-06-08 14:25:52.582479 security-0.1.0/PKG-INFO
--rw-r--r--   0 dani       (501) staff       (20)       60 2023-06-08 13:52:03.000000 security-0.1.0/README.md
--rw-r--r--   0 dani       (501) staff       (20)      293 2023-06-08 14:08:18.000000 security-0.1.0/pyproject.toml
--rw-r--r--   0 dani       (501) staff       (20)       38 2023-06-08 14:25:52.582840 security-0.1.0/setup.cfg
-drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:25:52.578986 security-0.1.0/src/
-drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:25:52.580567 security-0.1.0/src/security/
--rw-r--r--   0 dani       (501) staff       (20)        0 2023-06-08 13:54:46.000000 security-0.1.0/src/security/__init__.py
-drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:25:52.581946 security-0.1.0/src/security/safe_requests/
--rw-r--r--   0 dani       (501) staff       (20)       20 2023-06-08 14:18:37.000000 security-0.1.0/src/security/safe_requests/__init__.py
-drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:25:52.581725 security-0.1.0/src/security.egg-info/
--rw-r--r--   0 dani       (501) staff       (20)     1594 2023-06-08 14:25:52.000000 security-0.1.0/src/security.egg-info/PKG-INFO
--rw-r--r--   0 dani       (501) staff       (20)      256 2023-06-08 14:25:52.000000 security-0.1.0/src/security.egg-info/SOURCES.txt
--rw-r--r--   0 dani       (501) staff       (20)        1 2023-06-08 14:25:52.000000 security-0.1.0/src/security.egg-info/dependency_links.txt
--rw-r--r--   0 dani       (501) staff       (20)        9 2023-06-08 14:25:52.000000 security-0.1.0/src/security.egg-info/top_level.txt
+drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:31:52.451696 security-1.0.0/
+-rw-r--r--   0 dani       (501) staff       (20)     1096 2023-06-08 14:04:42.000000 security-1.0.0/LICENSE.txt
+-rw-r--r--   0 dani       (501) staff       (20)       29 2023-06-08 14:02:06.000000 security-1.0.0/MANIFEST.in
+-rw-r--r--   0 dani       (501) staff       (20)     1594 2023-06-08 14:31:52.451418 security-1.0.0/PKG-INFO
+-rw-r--r--   0 dani       (501) staff       (20)       60 2023-06-08 13:52:03.000000 security-1.0.0/README.md
+-rw-r--r--   0 dani       (501) staff       (20)      293 2023-06-08 14:31:07.000000 security-1.0.0/pyproject.toml
+-rw-r--r--   0 dani       (501) staff       (20)       38 2023-06-08 14:31:52.451757 security-1.0.0/setup.cfg
+drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:31:52.447752 security-1.0.0/src/
+drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:31:52.449378 security-1.0.0/src/security/
+-rw-r--r--   0 dani       (501) staff       (20)        0 2023-06-08 13:54:46.000000 security-1.0.0/src/security/__init__.py
+drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:31:52.450649 security-1.0.0/src/security/safe_requests/
+-rw-r--r--   0 dani       (501) staff       (20)       20 2023-06-08 14:18:37.000000 security-1.0.0/src/security/safe_requests/__init__.py
+drwxr-xr-x   0 dani       (501) staff       (20)        0 2023-06-08 14:31:52.450430 security-1.0.0/src/security.egg-info/
+-rw-r--r--   0 dani       (501) staff       (20)     1594 2023-06-08 14:31:52.000000 security-1.0.0/src/security.egg-info/PKG-INFO
+-rw-r--r--   0 dani       (501) staff       (20)      256 2023-06-08 14:31:52.000000 security-1.0.0/src/security.egg-info/SOURCES.txt
+-rw-r--r--   0 dani       (501) staff       (20)        1 2023-06-08 14:31:52.000000 security-1.0.0/src/security.egg-info/dependency_links.txt
+-rw-r--r--   0 dani       (501) staff       (20)        9 2023-06-08 14:31:52.000000 security-1.0.0/src/security.egg-info/top_level.txt
```

### Comparing `security-0.1.0/LICENSE.txt` & `security-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `security-0.1.0/PKG-INFO` & `security-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security
-Version: 0.1.0
+Version: 1.0.0
 Summary: The security toolkit for the Python comminity.
 Author-email: Dani Alcala <danalitovsky@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Dani Litovsky Alcala and others at Pixee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `security-0.1.0/src/security.egg-info/PKG-INFO` & `security-1.0.0/src/security.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: security
-Version: 0.1.0
+Version: 1.0.0
 Summary: The security toolkit for the Python comminity.
 Author-email: Dani Alcala <danalitovsky@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Dani Litovsky Alcala and others at Pixee
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

