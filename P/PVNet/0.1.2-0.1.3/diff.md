# Comparing `tmp/PVNet-0.1.2.tar.gz` & `tmp/PVNet-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-0.1.2.tar", last modified: Mon Jun  5 16:07:41 2023, max compression
+gzip compressed data, was "PVNet-0.1.3.tar", last modified: Wed Jun  7 13:05:59 2023, max compression
```

## Comparing `PVNet-0.1.2.tar` & `PVNet-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-05 16:07:29.000000 PVNet-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-05 16:07:29.000000 PVNet-0.1.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 16:07:41.785820 PVNet-0.1.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 16:07:41.000000 PVNet-0.1.2/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-05 16:07:29.000000 PVNet-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11061 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-05 16:07:29.000000 PVNet-0.1.2/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-05 16:07:29.000000 PVNet-0.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-05 16:07:29.000000 PVNet-0.1.2/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-05 16:07:29.000000 PVNet-0.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 16:07:41.785820 PVNet-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-05 16:07:29.000000 PVNet-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:41.785820 PVNet-0.1.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 16:07:29.000000 PVNet-0.1.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-05 16:07:29.000000 PVNet-0.1.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-05 16:07:29.000000 PVNet-0.1.2/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.283039 PVNet-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-07 13:05:47.000000 PVNet-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 13:05:47.000000 PVNet-0.1.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 13:05:59.279039 PVNet-0.1.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.279039 PVNet-0.1.3/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 13:05:47.000000 PVNet-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.279039 PVNet-0.1.3/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-07 13:05:47.000000 PVNet-0.1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 13:05:47.000000 PVNet-0.1.3/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-07 13:05:47.000000 PVNet-0.1.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:05:59.283039 PVNet-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 13:05:47.000000 PVNet-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.279039 PVNet-0.1.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:47.000000 PVNet-0.1.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-07 13:05:47.000000 PVNet-0.1.3/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 13:05:47.000000 PVNet-0.1.3/tests/test_app.py
```

### Comparing `PVNet-0.1.2/LICENSE` & `PVNet-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/PKG-INFO` & `PVNet-0.1.3/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: PVNet
-Version: 0.1.2
-Summary: PVNet
-Author: Peter Dudfield
-Author-email: info@openclimatefix.org
-License: MIT
-Description-Content-Type: text/markdown
-Provides-Extra: all_models
-License-File: LICENSE
-
 # PVNet
 [![test-release](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml/badge.svg)](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml)
 
 ## Setup
 ```bash
 git clone https://github.com/openclimatefix/PVNet.git
 cd PVNet
```

### Comparing `PVNet-0.1.2/PVNet.egg-info/PKG-INFO` & `PVNet-0.1.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.1.2
+Version: 0.1.3
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.1.2/README.md` & `PVNet-0.1.3/PVNet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: PVNet
+Version: 0.1.3
+Summary: PVNet
+Author: Peter Dudfield
+Author-email: info@openclimatefix.org
+License: MIT
+Description-Content-Type: text/markdown
+Provides-Extra: all_models
+License-File: LICENSE
+
 # PVNet
 [![test-release](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml/badge.svg)](https://github.com/openclimatefix/PVNet/actions/workflows/test-release.yml)
 
 ## Setup
 ```bash
 git clone https://github.com/openclimatefix/PVNet.git
 cd PVNet
```

### Comparing `PVNet-0.1.2/pvnet/app.py` & `PVNet-0.1.3/pvnet/app.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,22 +66,21 @@
 model_name = "openclimatefix/pvnet_v2"
 model_version = "4a0510b498c55fee00defb385eec418d5712124c"
 
 model_name_ocf_db = "pvnet_v2"
 
 # ---------------------------------------------------------------------------
 # LOGGER
-
-formatter = logging.Formatter(fmt="%(levelname)s:%(name)s:%(message)s")
-stream_handler = logging.StreamHandler()
-stream_handler.setFormatter(formatter)
+logging.basicConfig(
+    level=getattr(logging, os.getenv("LOGLEVEL", "INFO")),
+    format="[%(asctime)s] {%(pathname)s:%(lineno)d} %(levelname)s - %(message)s",
+)
 
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.INFO)
-logger.addHandler(stream_handler)
 
 # Get rid of these verbose logs
 sql_logger = logging.getLogger("sqlalchemy.engine.Engine")
 sql_logger.addHandler(logging.NullHandler())
 
 # ---------------------------------------------------------------------------
 # HELPER FUNCTIONS
@@ -285,14 +284,15 @@
     # Multiply normalised forecasts by capacities and clip negatives
     df_abs = df_normed.clip(0, None) * gsp_capacities.T
 
     # ---------------------------------------------------------------------------
     # 6. Make national total
     logger.info("Summing to national forecast")
     df_abs.insert(0, 0, df_abs.sum(axis=1))
+    logger.info(f"National forecast is {df_abs[0]}")
 
     # ---------------------------------------------------------------------------
     # Escape clause for making predictions locally
     if not write_predictions:
         return df_abs
 
     # ---------------------------------------------------------------------------
```

### Comparing `PVNet-0.1.2/pvnet/callbacks.py` & `PVNet-0.1.3/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/pvnet/optimizers.py` & `PVNet-0.1.3/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/pvnet/training.py` & `PVNet-0.1.3/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/pvnet/utils.py` & `PVNet-0.1.3/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/setup.py` & `PVNet-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/tests/conftest.py` & `PVNet-0.1.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.2/tests/test_app.py` & `PVNet-0.1.3/tests/test_app.py`

 * *Files identical despite different names*

