# Comparing `tmp/peeling-0.2.0.tar.gz` & `tmp/peeling-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peeling-0.2.0.tar", last modified: Mon May 22 18:46:18 2023, max compression
+gzip compressed data, was "peeling-0.2.1.tar", last modified: Thu Jun  8 13:06:37 2023, max compression
```

## Comparing `peeling-0.2.0.tar` & `peeling-0.2.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.089299 peeling-0.2.0/
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1518 2023-05-10 21:26:26.000000 peeling-0.2.0/LICENSE
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     9334 2023-05-22 18:46:18.088862 peeling-0.2.0/PKG-INFO
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     7202 2023-05-22 18:16:52.000000 peeling-0.2.0/README.md
-drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.079132 peeling-0.2.0/peeling/
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-10 21:26:26.000000 peeling-0.2.0/peeling/__init__.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     3169 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cellular_compartments.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1337 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/clipantherprocessor.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     6492 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cliprocessor.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)      267 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cliuniprotcommunicator.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     3464 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/cliuserinputreader.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     4803 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/main.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     6156 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/pantherprocessor.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)    10823 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/processor.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)    12249 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/uniprotcommunicator.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     2256 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/userinputreader.py
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1595 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webpantherprocessor.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     5620 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webprocessor.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     6498 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webuniprotcommunicator.py
--rwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)     1213 2023-05-22 18:16:52.000000 peeling-0.2.0/peeling/webuserinputreader.py
-drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.087969 peeling-0.2.0/peeling.egg-info/
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     9334 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/PKG-INFO
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)      647 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/SOURCES.txt
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)        1 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/dependency_links.txt
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)       46 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/entry_points.txt
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)      522 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/requires.txt
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)        8 2023-05-22 18:46:18.000000 peeling-0.2.0/peeling.egg-info/top_level.txt
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)     1479 2023-05-22 18:21:50.000000 peeling-0.2.0/pyproject.toml
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)       38 2023-05-22 18:46:18.089386 peeling-0.2.0/setup.cfg
-drwxr-xr-x   0 clementsj (43331813) HHMI\scicomp (1573765772)        0 2023-05-22 18:46:18.088424 peeling-0.2.0/test/
--rw-r--r--   0 clementsj (43331813) HHMI\scicomp (1573765772)    15513 2023-05-10 21:26:26.000000 peeling-0.2.0/test/test.py
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.075630 peeling-0.2.1/
+-rw-r--r--   0 clementsj   (503) staff       (20)     1518 2023-05-16 19:45:54.000000 peeling-0.2.1/LICENSE
+-rw-r--r--   0 clementsj   (503) staff       (20)     9334 2023-06-08 13:06:37.075475 peeling-0.2.1/PKG-INFO
+-rw-r--r--   0 clementsj   (503) staff       (20)     7202 2023-06-07 13:14:59.000000 peeling-0.2.1/README.md
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.074262 peeling-0.2.1/peeling/
+-rw-r--r--   0 clementsj   (503) staff       (20)        0 2023-05-16 19:45:54.000000 peeling-0.2.1/peeling/__init__.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     3169 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cellular_compartments.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     1337 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/clipantherprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     6492 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cliprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)      267 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cliuniprotcommunicator.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     3464 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/cliuserinputreader.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     4803 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/main.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     6156 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/pantherprocessor.py
+-rw-r--r--   0 clementsj   (503) staff       (20)    10823 2023-06-07 18:35:54.000000 peeling-0.2.1/peeling/processor.py
+-rw-r--r--   0 clementsj   (503) staff       (20)    12249 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/uniprotcommunicator.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     2256 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/userinputreader.py
+-rw-r--r--   0 clementsj   (503) staff       (20)     1595 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/webpantherprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     5620 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/webprocessor.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     6498 2023-06-07 13:14:59.000000 peeling-0.2.1/peeling/webuniprotcommunicator.py
+-rwxr-xr-x   0 clementsj   (503) staff       (20)     1110 2023-06-07 18:42:16.000000 peeling-0.2.1/peeling/webuserinputreader.py
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.075076 peeling-0.2.1/peeling.egg-info/
+-rw-r--r--   0 clementsj   (503) staff       (20)     9334 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/PKG-INFO
+-rw-r--r--   0 clementsj   (503) staff       (20)      647 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/SOURCES.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)        1 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/dependency_links.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)       46 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/entry_points.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)      522 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/requires.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)        8 2023-06-08 13:06:37.000000 peeling-0.2.1/peeling.egg-info/top_level.txt
+-rw-r--r--   0 clementsj   (503) staff       (20)     1479 2023-06-08 12:57:26.000000 peeling-0.2.1/pyproject.toml
+-rw-r--r--   0 clementsj   (503) staff       (20)       38 2023-06-08 13:06:37.075665 peeling-0.2.1/setup.cfg
+drwxr-xr-x   0 clementsj   (503) staff       (20)        0 2023-06-08 13:06:37.075181 peeling-0.2.1/test/
+-rw-r--r--   0 clementsj   (503) staff       (20)    15513 2023-05-16 19:45:54.000000 peeling-0.2.1/test/test.py
```

### Comparing `peeling-0.2.0/LICENSE` & `peeling-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/PKG-INFO` & `peeling-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.2.0
+Version: 0.2.1
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `peeling-0.2.0/README.md` & `peeling-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/cellular_compartments.py` & `peeling-0.2.1/peeling/cellular_compartments.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/clipantherprocessor.py` & `peeling-0.2.1/peeling/clipantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/cliprocessor.py` & `peeling-0.2.1/peeling/cliprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/cliuserinputreader.py` & `peeling-0.2.1/peeling/cliuserinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/main.py` & `peeling-0.2.1/peeling/main.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/pantherprocessor.py` & `peeling-0.2.1/peeling/pantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/processor.py` & `peeling-0.2.1/peeling/processor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/uniprotcommunicator.py` & `peeling-0.2.1/peeling/uniprotcommunicator.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/userinputreader.py` & `peeling-0.2.1/peeling/userinputreader.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/webpantherprocessor.py` & `peeling-0.2.1/peeling/webpantherprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/webprocessor.py` & `peeling-0.2.1/peeling/webprocessor.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/webuniprotcommunicator.py` & `peeling-0.2.1/peeling/webuniprotcommunicator.py`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling/webuserinputreader.py` & `peeling-0.2.1/peeling/webuserinputreader.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from fastapi import UploadFile
 import pandas as pd
 import csv
 import logging
+from io import StringIO
 from peeling.userinputreader import UserInputReader
 
 logger = logging.getLogger('peeling')
 
 
 class WebUserInputReader(UserInputReader):
     def __init__(self, mass_file:UploadFile, num_controls, num_replicates, tolerance, plot_format, cellular_compartment):
         super().__init__(num_controls, num_replicates, tolerance, plot_format, cellular_compartment)
         self.__mass_file = mass_file
 
 
     async def __decode_uploadFile(self):
         bytes = await self.__mass_file.read()
-        lines = [line for line in bytes.decode("utf-8").split("\n") if line]
-        reader = csv.DictReader(lines, delimiter="\t", quotechar='"')
-        df = pd.DataFrame(list(reader))
+        df = pd.read_table(StringIO(bytes.decode("utf-8")))
         logger.debug(f'\n{df.head()}')
         self._check_file(df)
         return df
 
 
     # implement abstract method
     async def get_mass_data(self):
```

### Comparing `peeling-0.2.0/peeling.egg-info/PKG-INFO` & `peeling-0.2.1/peeling.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peeling
-Version: 0.2.0
+Version: 0.2.1
 Author-email: HHMI Janelia <peeling@janelia.hhmi.org>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Howard Hughes Medical Institute
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

### Comparing `peeling-0.2.0/peeling.egg-info/SOURCES.txt` & `peeling-0.2.1/peeling.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/peeling.egg-info/requires.txt` & `peeling-0.2.1/peeling.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `peeling-0.2.0/pyproject.toml` & `peeling-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "peeling"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="HHMI Janelia", email="peeling@janelia.hhmi.org" },
 ]
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `peeling-0.2.0/test/test.py` & `peeling-0.2.1/test/test.py`

 * *Files identical despite different names*

