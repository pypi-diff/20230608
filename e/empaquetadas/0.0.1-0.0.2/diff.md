# Comparing `tmp/empaquetadas-0.0.1.tar.gz` & `tmp/empaquetadas-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "empaquetadas-0.0.1.tar", last modified: Thu Jun  8 01:22:15 2023, max compression
+gzip compressed data, was "empaquetadas-0.0.2.tar", last modified: Thu Jun  8 01:37:53 2023, max compression
```

## Comparing `empaquetadas-0.0.1.tar` & `empaquetadas-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:22:15.725609 empaquetadas-0.0.1/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1071 2023-06-08 00:05:41.000000 empaquetadas-0.0.1/LICENSE
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1532 2023-06-08 01:22:15.725609 empaquetadas-0.0.1/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       26 2023-06-08 00:05:13.000000 empaquetadas-0.0.1/README.md
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      406 2023-06-08 00:06:25.000000 empaquetadas-0.0.1/pyproject.toml
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-08 01:22:15.725609 empaquetadas-0.0.1/setup.cfg
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:22:15.725609 empaquetadas-0.0.1/src/
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:22:15.725609 empaquetadas-0.0.1/src/empaquetadas/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      704 2023-06-08 00:18:11.000000 empaquetadas-0.0.1/src/empaquetadas/__init__.py
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     2037 2023-06-08 00:21:31.000000 empaquetadas-0.0.1/src/empaquetadas/samples.py
-drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:22:15.725609 empaquetadas-0.0.1/src/empaquetadas.egg-info/
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1532 2023-06-08 01:22:15.000000 empaquetadas-0.0.1/src/empaquetadas.egg-info/PKG-INFO
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      249 2023-06-08 01:22:15.000000 empaquetadas-0.0.1/src/empaquetadas.egg-info/SOURCES.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-08 01:22:15.000000 empaquetadas-0.0.1/src/empaquetadas.egg-info/dependency_links.txt
--rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       13 2023-06-08 01:22:15.000000 empaquetadas-0.0.1/src/empaquetadas.egg-info/top_level.txt
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1071 2023-06-08 00:05:41.000000 empaquetadas-0.0.2/LICENSE
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1532 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/PKG-INFO
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       26 2023-06-08 00:05:13.000000 empaquetadas-0.0.2/README.md
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      406 2023-06-08 01:37:06.000000 empaquetadas-0.0.2/pyproject.toml
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       38 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/setup.cfg
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/src/
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/src/empaquetadas/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      704 2023-06-08 00:18:11.000000 empaquetadas-0.0.2/src/empaquetadas/__init__.py
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     2037 2023-06-08 00:21:31.000000 empaquetadas-0.0.2/src/empaquetadas/samples.py
+drwxrwxr-x   0 rfsan     (1000) rfsan     (1000)        0 2023-06-08 01:37:53.972429 empaquetadas-0.0.2/src/empaquetadas.egg-info/
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)     1532 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/PKG-INFO
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)      249 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/SOURCES.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)        1 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/dependency_links.txt
+-rw-rw-r--   0 rfsan     (1000) rfsan     (1000)       13 2023-06-08 01:37:53.000000 empaquetadas-0.0.2/src/empaquetadas.egg-info/top_level.txt
```

### Comparing `empaquetadas-0.0.1/LICENSE` & `empaquetadas-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `empaquetadas-0.0.1/PKG-INFO` & `empaquetadas-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empaquetadas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package to calculate what would have happened if you had invested your pesos
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafael Sanabria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `empaquetadas-0.0.1/src/empaquetadas/__init__.py` & `empaquetadas-0.0.2/src/empaquetadas/__init__.py`

 * *Files identical despite different names*

### Comparing `empaquetadas-0.0.1/src/empaquetadas/samples.py` & `empaquetadas-0.0.2/src/empaquetadas/samples.py`

 * *Files identical despite different names*

### Comparing `empaquetadas-0.0.1/src/empaquetadas.egg-info/PKG-INFO` & `empaquetadas-0.0.2/src/empaquetadas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: empaquetadas
-Version: 0.0.1
+Version: 0.0.2
 Summary: Package to calculate what would have happened if you had invested your pesos
 Author-email: Rafael Sanabria <rafael.d.sanabria@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Rafael Sanabria
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

