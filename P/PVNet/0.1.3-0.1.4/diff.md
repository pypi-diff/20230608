# Comparing `tmp/PVNet-0.1.3.tar.gz` & `tmp/PVNet-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PVNet-0.1.3.tar", last modified: Wed Jun  7 13:05:59 2023, max compression
+gzip compressed data, was "PVNet-0.1.4.tar", last modified: Thu Jun  8 11:27:26 2023, max compression
```

## Comparing `PVNet-0.1.3.tar` & `PVNet-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.283039 PVNet-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-07 13:05:47.000000 PVNet-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-07 13:05:47.000000 PVNet-0.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 13:05:59.279039 PVNet-0.1.3/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.279039 PVNet-0.1.3/PVNet.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-07 13:05:59.000000 PVNet-0.1.3/PVNet.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-07 13:05:47.000000 PVNet-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.279039 PVNet-0.1.3/pvnet/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11091 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/optimizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/training.py
--rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-07 13:05:47.000000 PVNet-0.1.3/pvnet/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-07 13:05:47.000000 PVNet-0.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-07 13:05:47.000000 PVNet-0.1.3/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-07 13:05:47.000000 PVNet-0.1.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 13:05:59.283039 PVNet-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-07 13:05:47.000000 PVNet-0.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:59.279039 PVNet-0.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 13:05:47.000000 PVNet-0.1.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-07 13:05:47.000000 PVNet-0.1.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-07 13:05:47.000000 PVNet-0.1.3/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:27:26.346464 PVNet-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-08 11:27:07.000000 PVNet-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-08 11:27:07.000000 PVNet-0.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 11:27:26.346464 PVNet-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:27:26.346464 PVNet-0.1.4/PVNet.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-08 11:27:26.000000 PVNet-0.1.4/PVNet.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-06-08 11:27:26.000000 PVNet-0.1.4/PVNet.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 11:27:26.000000 PVNet-0.1.4/PVNet.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-08 11:27:26.000000 PVNet-0.1.4/PVNet.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-08 11:27:26.000000 PVNet-0.1.4/PVNet.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-06-08 11:27:07.000000 PVNet-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:27:26.346464 PVNet-0.1.4/pvnet/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-08 11:27:07.000000 PVNet-0.1.4/pvnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11369 2023-06-08 11:27:07.000000 PVNet-0.1.4/pvnet/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3648 2023-06-08 11:27:07.000000 PVNet-0.1.4/pvnet/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-06-08 11:27:07.000000 PVNet-0.1.4/pvnet/optimizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-06-08 11:27:07.000000 PVNet-0.1.4/pvnet/training.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10158 2023-06-08 11:27:07.000000 PVNet-0.1.4/pvnet/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-08 11:27:07.000000 PVNet-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-08 11:27:07.000000 PVNet-0.1.4/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-08 11:27:07.000000 PVNet-0.1.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 11:27:26.346464 PVNet-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-08 11:27:07.000000 PVNet-0.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 11:27:26.346464 PVNet-0.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 11:27:07.000000 PVNet-0.1.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7653 2023-06-08 11:27:07.000000 PVNet-0.1.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-06-08 11:27:08.000000 PVNet-0.1.4/tests/test_app.py
```

### Comparing `PVNet-0.1.3/LICENSE` & `PVNet-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/PKG-INFO` & `PVNet-0.1.4/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.1.3
+Version: 0.1.4
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.1.3/PVNet.egg-info/PKG-INFO` & `PVNet-0.1.4/PVNet.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PVNet
-Version: 0.1.3
+Version: 0.1.4
 Summary: PVNet
 Author: Peter Dudfield
 Author-email: info@openclimatefix.org
 License: MIT
 Description-Content-Type: text/markdown
 Provides-Extra: all_models
 License-File: LICENSE
```

### Comparing `PVNet-0.1.3/README.md` & `PVNet-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/pvnet/app.py` & `PVNet-0.1.4/pvnet/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -167,15 +167,16 @@
     """
 
     logger.info(f"Using `pvnet` library version: {pvnet.__version__}")
 
     # ---------------------------------------------------------------------------
     # 0. If inference datetime is None, round down to last 30 minutes
     if t0 is None:
-        t0 = pd.Timestamp.now(tz=None).floor(timedelta(minutes=30))
+        t0 = pd.Timestamp.now(tz="UTC").replace(tzinfo=None).floor(timedelta(minutes=30))
+
     else:
         t0 = pd.to_datetime(t0).floor(timedelta(minutes=30))
 
     logger.info(f"Making forecast for init time: {t0}")
 
     # ---------------------------------------------------------------------------
     # 1. Prepare data sources
@@ -250,22 +251,27 @@
         for i, batch in enumerate(dataloader):
             logger.info(f"Predicting for batch: {i}")
             # Run batch through model
             device_batch = copy_batch_to_device(batch_to_tensor(batch), device)
             preds = model(device_batch).detach().cpu().numpy()
 
             # Calculate unnormalised elevation and sun-dowm mask
+            logger.info("Remove predictions after sundown")
             elevation = batch[BatchKey.gsp_solar_elevation] * ELEVATION_STD + ELEVATION_MEAN
             # We only need elevation mask for forecasted values, not history
             elevation = elevation[:, -preds.shape[-1] :]
             sun_down_mask = elevation < MIN_DAY_ELEVATION
 
             # Zero out after sundown
             preds[sun_down_mask] = 0
 
+            # log max prediction
+            max_prediction = np.max(preds)
+            logger.info(f"Max prediction: {max_prediction}")
+
             normed_preds += [preds]
             logger.info(f"Completed batch: {i}")
 
     normed_preds = np.concatenate(normed_preds)
 
     # ---------------------------------------------------------------------------
     # 5. Merge batch results to pandas df
@@ -279,14 +285,15 @@
         index=pd.Index(
             [t0 + timedelta(minutes=30 * (i + 1)) for i in range(n_times)],
             name="target_datetime_utc",
         ),
     )
     # Multiply normalised forecasts by capacities and clip negatives
     df_abs = df_normed.clip(0, None) * gsp_capacities.T
+    logger.debug(f"Maximum predictions: {df_abs.max()}")
 
     # ---------------------------------------------------------------------------
     # 6. Make national total
     logger.info("Summing to national forecast")
     df_abs.insert(0, 0, df_abs.sum(axis=1))
     logger.info(f"National forecast is {df_abs[0]}")
```

### Comparing `PVNet-0.1.3/pvnet/callbacks.py` & `PVNet-0.1.4/pvnet/callbacks.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/pvnet/optimizers.py` & `PVNet-0.1.4/pvnet/optimizers.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/pvnet/training.py` & `PVNet-0.1.4/pvnet/training.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/pvnet/utils.py` & `PVNet-0.1.4/pvnet/utils.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/setup.py` & `PVNet-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/tests/conftest.py` & `PVNet-0.1.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `PVNet-0.1.3/tests/test_app.py` & `PVNet-0.1.4/tests/test_app.py`

 * *Files identical despite different names*

