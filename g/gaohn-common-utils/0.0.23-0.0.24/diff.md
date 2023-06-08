# Comparing `tmp/gaohn-common-utils-0.0.23.tar.gz` & `tmp/gaohn-common-utils-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaohn-common-utils-0.0.23.tar", last modified: Tue Jun  6 03:03:10 2023, max compression
+gzip compressed data, was "gaohn-common-utils-0.0.24.tar", last modified: Thu Jun  8 02:02:42 2023, max compression
```

## Comparing `gaohn-common-utils-0.0.23.tar` & `gaohn-common-utils-0.0.24.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.200782 gaohn-common-utils-0.0.23/
--rw-r--r--   0 gaohn      (501) staff       (20)    11357 2023-04-26 08:56:39.000000 gaohn-common-utils-0.0.23/LICENSE
--rw-r--r--   0 gaohn      (501) staff       (20)      950 2023-06-06 03:03:10.200628 gaohn-common-utils-0.0.23/PKG-INFO
--rw-r--r--   0 gaohn      (501) staff       (20)      409 2023-05-30 02:21:40.000000 gaohn-common-utils-0.0.23/README.md
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.196909 gaohn-common-utils-0.0.23/common_utils/
--rw-r--r--   0 gaohn      (501) staff       (20)        0 2023-05-30 02:13:10.000000 gaohn-common-utils-0.0.23/common_utils/__init__.py
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.197040 gaohn-common-utils-0.0.23/common_utils/cloud/
--rw-r--r--   0 gaohn      (501) staff       (20)      930 2023-06-05 02:47:12.000000 gaohn-common-utils-0.0.23/common_utils/cloud/base.py
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.195824 gaohn-common-utils-0.0.23/common_utils/cloud/gcp/
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.197720 gaohn-common-utils-0.0.23/common_utils/cloud/gcp/storage/
--rw-r--r--   0 gaohn      (501) staff       (20)     4857 2023-06-05 05:30:04.000000 gaohn-common-utils-0.0.23/common_utils/cloud/gcp/storage/bigquery.py
--rw-r--r--   0 gaohn      (501) staff       (20)     5062 2023-06-05 05:24:26.000000 gaohn-common-utils-0.0.23/common_utils/cloud/gcp/storage/gcs.py
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.199258 gaohn-common-utils-0.0.23/common_utils/core/
--rw-r--r--   0 gaohn      (501) staff       (20)        0 2023-04-26 09:12:27.000000 gaohn-common-utils-0.0.23/common_utils/core/__init__.py
--rw-r--r--   0 gaohn      (501) staff       (20)     1952 2023-05-20 11:03:55.000000 gaohn-common-utils-0.0.23/common_utils/core/artifacts.py
--rw-r--r--   0 gaohn      (501) staff       (20)      441 2023-05-18 06:06:21.000000 gaohn-common-utils-0.0.23/common_utils/core/base.py
--rw-r--r--   0 gaohn      (501) staff       (20)     3425 2023-05-30 02:13:10.000000 gaohn-common-utils-0.0.23/common_utils/core/common.py
--rw-r--r--   0 gaohn      (501) staff       (20)     4715 2023-05-30 02:13:10.000000 gaohn-common-utils-0.0.23/common_utils/core/decorators.py
--rw-r--r--   0 gaohn      (501) staff       (20)     3036 2023-05-30 02:13:10.000000 gaohn-common-utils-0.0.23/common_utils/core/file_system_utils.py
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.196022 gaohn-common-utils-0.0.23/common_utils/versioning/
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.199423 gaohn-common-utils-0.0.23/common_utils/versioning/dvc/
--rw-r--r--   0 gaohn      (501) staff       (20)     3175 2023-06-04 09:34:56.000000 gaohn-common-utils-0.0.23/common_utils/versioning/dvc/base.py
-drwxr-xr-x   0 gaohn      (501) staff       (20)        0 2023-06-06 03:03:10.200416 gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/
--rw-r--r--   0 gaohn      (501) staff       (20)      950 2023-06-06 03:03:10.000000 gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/PKG-INFO
--rw-r--r--   0 gaohn      (501) staff       (20)      596 2023-06-06 03:03:10.000000 gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/SOURCES.txt
--rw-r--r--   0 gaohn      (501) staff       (20)        1 2023-06-06 03:03:10.000000 gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/dependency_links.txt
--rw-r--r--   0 gaohn      (501) staff       (20)      159 2023-06-06 03:03:10.000000 gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/requires.txt
--rw-r--r--   0 gaohn      (501) staff       (20)       13 2023-06-06 03:03:10.000000 gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/top_level.txt
--rw-r--r--   0 gaohn      (501) staff       (20)      898 2023-06-06 03:01:44.000000 gaohn-common-utils-0.0.23/pyproject.toml
--rw-r--r--   0 gaohn      (501) staff       (20)       38 2023-06-06 03:03:10.200824 gaohn-common-utils-0.0.23/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.360483 gaohn-common-utils-0.0.24/common_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.360483 gaohn-common-utils-0.0.24/common_utils/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/cloud/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.360483 gaohn-common-utils-0.0.24/common_utils/cloud/gcp/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/common_utils/cloud/gcp/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/cloud/gcp/storage/bigquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5062 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/cloud/gcp/storage/gcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/common_utils/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3036 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/file_system_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/core/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.360483 gaohn-common-utils-0.0.24/common_utils/versioning/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/common_utils/versioning/dvc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3176 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/common_utils/versioning/dvc/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-06-08 02:02:42.000000 gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-08 02:02:42.000000 gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 02:02:42.000000 gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-08 02:02:42.000000 gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-08 02:02:42.000000 gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2399 2023-06-08 02:02:23.000000 gaohn-common-utils-0.0.24/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 02:02:42.364483 gaohn-common-utils-0.0.24/setup.cfg
```

### Comparing `gaohn-common-utils-0.0.23/LICENSE` & `gaohn-common-utils-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/PKG-INFO` & `gaohn-common-utils-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.23
+Version: 0.0.24
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.23/common_utils/cloud/base.py` & `gaohn-common-utils-0.0.24/common_utils/cloud/base.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/common_utils/cloud/gcp/storage/bigquery.py` & `gaohn-common-utils-0.0.24/common_utils/cloud/gcp/storage/bigquery.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/common_utils/cloud/gcp/storage/gcs.py` & `gaohn-common-utils-0.0.24/common_utils/cloud/gcp/storage/gcs.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/common_utils/core/artifacts.py` & `gaohn-common-utils-0.0.24/common_utils/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/common_utils/core/common.py` & `gaohn-common-utils-0.0.24/common_utils/core/common.py`

 * *Ordering differences only*

 * *Files 2% similar despite different names*

```diff
@@ -5,18 +5,18 @@
 """
 import json
 import os
 import random
 from typing import Any, Dict, Optional
 
 import numpy as np
+import rich
 import torch
 import yaml
 from yaml import FullLoader
-import rich
 
 from common_utils.core.base import DictPersistence
 
 
 class JsonAdapter(DictPersistence):
     def save_as_dict(
         self, data: Dict[str, Any], filepath: str, **kwargs: Dict[str, Any]
```

### Comparing `gaohn-common-utils-0.0.23/common_utils/core/decorators.py` & `gaohn-common-utils-0.0.24/common_utils/core/decorators.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/common_utils/core/file_system_utils.py` & `gaohn-common-utils-0.0.24/common_utils/core/file_system_utils.py`

 * *Files identical despite different names*

### Comparing `gaohn-common-utils-0.0.23/common_utils/versioning/dvc/base.py` & `gaohn-common-utils-0.0.24/common_utils/versioning/dvc/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import os
-import json
 import hashlib
-import pandas as pd
+import json
+import os
 from datetime import datetime
 
+import pandas as pd
+
 DATA_DIR = "data_versions"
 CODE_DIR = "code_versions"
 METADATA_FILE = "metadata.json"
 
 
 def hash_file(filepath):
     """Generate MD5 hash of a file."""
```

### Comparing `gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/PKG-INFO` & `gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaohn-common-utils
-Version: 0.0.23
+Version: 0.0.24
 Summary: A small utility package
 Author-email: Gao Hongnan <hongnangao@gmail.com>
 Project-URL: Homepage, https://github.com/gao-hongnan/common-utils
 Project-URL: Bug Tracker, https://github.com/gao-hongnan/common-utils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `gaohn-common-utils-0.0.23/gaohn_common_utils.egg-info/SOURCES.txt` & `gaohn-common-utils-0.0.24/gaohn_common_utils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -7,13 +7,14 @@
 common_utils/cloud/gcp/storage/gcs.py
 common_utils/core/__init__.py
 common_utils/core/artifacts.py
 common_utils/core/base.py
 common_utils/core/common.py
 common_utils/core/decorators.py
 common_utils/core/file_system_utils.py
+common_utils/core/logger.py
 common_utils/versioning/dvc/base.py
 gaohn_common_utils.egg-info/PKG-INFO
 gaohn_common_utils.egg-info/SOURCES.txt
 gaohn_common_utils.egg-info/dependency_links.txt
 gaohn_common_utils.egg-info/requires.txt
 gaohn_common_utils.egg-info/top_level.txt
```

