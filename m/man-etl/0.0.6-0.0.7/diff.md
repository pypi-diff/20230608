# Comparing `tmp/man_etl-0.0.6.tar.gz` & `tmp/man_etl-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "man_etl-0.0.6.tar", last modified: Thu Jun  8 16:23:48 2023, max compression
+gzip compressed data, was "man_etl-0.0.7.tar", last modified: Thu Jun  8 16:34:17 2023, max compression
```

## Comparing `man_etl-0.0.6.tar` & `man_etl-0.0.7.tar`

### file list

```diff
@@ -1,33 +1,38 @@
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:39:00.708904 man_etl-0.0.6/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:39:00.692373 man_etl-0.0.6/PKG-INFO
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      374 2023-06-08 08:17:19.000000 man_etl-0.0.6/README.md
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:38:59.040725 man_etl-0.0.6/man_etl/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-0.0.6/man_etl/__init__.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:38:59.653783 man_etl-0.0.6/man_etl/etl_pipelines/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:17:19.000000 man_etl-0.0.6/man_etl/etl_pipelines/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1168 2023-06-08 13:36:53.000000 man_etl-0.0.6/man_etl/etl_pipelines/arctic_transform.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:39:00.250366 man_etl-0.0.6/man_etl/etl_pipelines/core/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-0.0.6/man_etl/etl_pipelines/core/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-0.0.6/man_etl/etl_pipelines/core/arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      788 2023-06-08 10:01:21.000000 man_etl-0.0.6/man_etl/etl_pipelines/core/base.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2159 2023-06-08 13:36:53.000000 man_etl-0.0.6/man_etl/etl_pipelines/core/extractors.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      468 2023-06-08 13:36:53.000000 man_etl-0.0.6/man_etl/etl_pipelines/core/storers.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1171 2023-06-08 13:36:53.000000 man_etl-0.0.6/man_etl/etl_pipelines/core/transformers.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1062 2023-06-08 16:36:50.000000 man_etl-0.0.6/man_etl/etl_pipelines/csv_to_arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      651 2023-06-08 13:36:53.000000 man_etl-0.0.6/man_etl/etl_pipelines/ons_to_arctic.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-0.0.6/man_etl/generate_db.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:39:00.634091 man_etl-0.0.6/man_etl/python/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-0.0.6/man_etl/python/__init__.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      612 2023-06-08 08:17:19.000000 man_etl-0.0.6/man_etl/python/app.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       59 2023-06-07 17:32:57.000000 man_etl-0.0.6/man_etl/python/main.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       94 2023-06-08 09:31:02.000000 man_etl-0.0.6/man_etl/python/pyarrow_client.py
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       79 2023-06-08 08:17:19.000000 man_etl-0.0.6/man_etl/python/utils.py
-drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:38:59.376304 man_etl-0.0.6/man_etl.egg-info/
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:38:53.000000 man_etl-0.0.6/man_etl.egg-info/PKG-INFO
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      765 2023-06-08 16:38:56.000000 man_etl-0.0.6/man_etl.egg-info/SOURCES.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-08 16:38:54.000000 man_etl-0.0.6/man_etl.egg-info/dependency_links.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       84 2023-06-08 16:38:54.000000 man_etl-0.0.6/man_etl.egg-info/entry_points.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       22 2023-06-08 16:38:54.000000 man_etl-0.0.6/man_etl.egg-info/requires.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-08 16:38:54.000000 man_etl-0.0.6/man_etl.egg-info/top_level.txt
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-08 16:39:00.708904 man_etl-0.0.6/setup.cfg
--rwxrwxrwx   0 shussey   (1000) shussey   (1000)      369 2023-06-08 16:37:57.000000 man_etl-0.0.6/setup.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:41.370465 man_etl-0.0.7/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:48:41.370465 man_etl-0.0.7/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      374 2023-06-08 08:17:19.000000 man_etl-0.0.7/README.md
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:39.233281 man_etl-0.0.7/man_etl/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:55.000000 man_etl-0.0.7/man_etl/__init__.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:39.902728 man_etl-0.0.7/man_etl/etl_pipelines/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:46:59.000000 man_etl-0.0.7/man_etl/etl_pipelines/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1168 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/arctic_transform.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:40.498578 man_etl-0.0.7/man_etl/etl_pipelines/core/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 08:40:26.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1363 2023-06-08 10:16:49.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      788 2023-06-08 10:01:21.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/base.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     2160 2023-06-08 16:45:40.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/extractors.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      468 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/storers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1173 2023-06-08 16:45:57.000000 man_etl-0.0.7/man_etl/etl_pipelines/core/transformers.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1062 2023-06-08 16:36:50.000000 man_etl-0.0.7/man_etl/etl_pipelines/csv_to_arctic.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      651 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/ons_to_arctic.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:40.899660 man_etl-0.0.7/man_etl/etl_pipelines/util/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:44:11.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       25 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/definitions.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)     1369 2023-06-08 13:36:53.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/transforms.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       97 2023-06-08 10:01:21.000000 man_etl-0.0.7/man_etl/etl_pipelines/util/utils.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      147 2023-06-08 08:17:19.000000 man_etl-0.0.7/man_etl/generate_db.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:41.296355 man_etl-0.0.7/man_etl/python/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-07 17:32:56.000000 man_etl-0.0.7/man_etl/python/__init__.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      612 2023-06-08 08:17:19.000000 man_etl-0.0.7/man_etl/python/app.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       59 2023-06-07 17:32:57.000000 man_etl-0.0.7/man_etl/python/main.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       94 2023-06-08 09:31:02.000000 man_etl-0.0.7/man_etl/python/pyarrow_client.py
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       79 2023-06-08 08:17:19.000000 man_etl-0.0.7/man_etl/python/utils.py
+drwxrwxrwx   0 shussey   (1000) shussey   (1000)        0 2023-06-08 16:48:39.561092 man_etl-0.0.7/man_etl.egg-info/
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       51 2023-06-08 16:48:33.000000 man_etl-0.0.7/man_etl.egg-info/PKG-INFO
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      923 2023-06-08 16:48:37.000000 man_etl-0.0.7/man_etl.egg-info/SOURCES.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        1 2023-06-08 16:48:33.000000 man_etl-0.0.7/man_etl.egg-info/dependency_links.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       84 2023-06-08 16:48:34.000000 man_etl-0.0.7/man_etl.egg-info/entry_points.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       22 2023-06-08 16:48:34.000000 man_etl-0.0.7/man_etl.egg-info/requires.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)        8 2023-06-08 16:48:34.000000 man_etl-0.0.7/man_etl.egg-info/top_level.txt
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)       38 2023-06-08 16:48:41.386800 man_etl-0.0.7/setup.cfg
+-rwxrwxrwx   0 shussey   (1000) shussey   (1000)      369 2023-06-08 16:48:24.000000 man_etl-0.0.7/setup.py
```

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/arctic_transform.py` & `man_etl-0.0.7/man_etl/etl_pipelines/arctic_transform.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/core/arctic.py` & `man_etl-0.0.7/man_etl/etl_pipelines/core/arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/core/base.py` & `man_etl-0.0.7/man_etl/etl_pipelines/core/base.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/core/extractors.py` & `man_etl-0.0.7/man_etl/etl_pipelines/core/extractors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import pandas as pd
 import logging
 from man_etl.etl_pipelines.core.base import Extractor
+from man_etl.etl_pipelines.util.definitions import TRANSFORM
 from arcticdb.version_store.library import Library
 from typing import List, Dict
 from dataclasses import dataclass
-from man_etl.etl_pipelines.util.definitions import TRANSFORM
+
 
 from pyarrow._flight import FlightClient
 from man_etl.etl_pipelines.util.utils import SERVER_MAPPINGS
 from pyarrow import flight
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('Logger')
```

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/core/transformers.py` & `man_etl-0.0.7/man_etl/etl_pipelines/core/transformers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import os
 import pandas as pd
 import logging
 from man_etl.etl_pipelines.core.base import Transformer
+from man_etl.etl_pipelines.util.definitions import TRANSFORM
+from man_etl.etl_pipelines.util.transforms import calcs
 from typing import Dict, List
 from dataclasses import dataclass
-from man_etl.etl_pipelines.util.transforms import calcs
-from man_etl.etl_pipelines.util.definitions import TRANSFORM
+
+
 
 
 
 logging.basicConfig(level=logging.INFO)
 logger = logging.getLogger('Logger')
 
 @dataclass
```

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/csv_to_arctic.py` & `man_etl-0.0.7/man_etl/etl_pipelines/csv_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.6/man_etl/etl_pipelines/ons_to_arctic.py` & `man_etl-0.0.7/man_etl/etl_pipelines/ons_to_arctic.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.6/man_etl/python/app.py` & `man_etl-0.0.7/man_etl/python/app.py`

 * *Files identical despite different names*

### Comparing `man_etl-0.0.6/man_etl.egg-info/SOURCES.txt` & `man_etl-0.0.7/man_etl.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,12 +14,16 @@
 man_etl/etl_pipelines/ons_to_arctic.py
 man_etl/etl_pipelines/core/__init__.py
 man_etl/etl_pipelines/core/arctic.py
 man_etl/etl_pipelines/core/base.py
 man_etl/etl_pipelines/core/extractors.py
 man_etl/etl_pipelines/core/storers.py
 man_etl/etl_pipelines/core/transformers.py
+man_etl/etl_pipelines/util/__init__.py
+man_etl/etl_pipelines/util/definitions.py
+man_etl/etl_pipelines/util/transforms.py
+man_etl/etl_pipelines/util/utils.py
 man_etl/python/__init__.py
 man_etl/python/app.py
 man_etl/python/main.py
 man_etl/python/pyarrow_client.py
 man_etl/python/utils.py
```

