# Comparing `tmp/CausalPy-0.0.8.tar.gz` & `tmp/CausalPy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CausalPy-0.0.8.tar", last modified: Wed Jan  4 14:16:43 2023, max compression
+gzip compressed data, was "CausalPy-0.0.9.tar", last modified: Wed Jan  4 19:28:08 2023, max compression
```

## Comparing `CausalPy-0.0.8.tar` & `CausalPy-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 14:16:43.163128 CausalPy-0.0.8/
--rw-r--r--   0 benjamv    (501) staff       (20)     3514 2022-12-01 15:41:43.000000 CausalPy-0.0.8/CONTRIBUTING.md
-drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 14:16:43.160029 CausalPy-0.0.8/CausalPy.egg-info/
--rw-r--r--   0 benjamv    (501) staff       (20)     9594 2023-01-04 14:16:43.000000 CausalPy-0.0.8/CausalPy.egg-info/PKG-INFO
--rw-r--r--   0 benjamv    (501) staff       (20)     1084 2023-01-04 14:16:43.000000 CausalPy-0.0.8/CausalPy.egg-info/SOURCES.txt
--rw-r--r--   0 benjamv    (501) staff       (20)        1 2023-01-04 14:16:43.000000 CausalPy-0.0.8/CausalPy.egg-info/dependency_links.txt
--rw-r--r--   0 benjamv    (501) staff       (20)      144 2023-01-04 14:16:43.000000 CausalPy-0.0.8/CausalPy.egg-info/requires.txt
--rw-r--r--   0 benjamv    (501) staff       (20)        9 2023-01-04 14:16:43.000000 CausalPy-0.0.8/CausalPy.egg-info/top_level.txt
--rw-r--r--   0 benjamv    (501) staff       (20)    11357 2022-10-28 10:08:58.000000 CausalPy-0.0.8/LICENSE
--rw-r--r--   0 benjamv    (501) staff       (20)       60 2022-11-24 10:00:18.000000 CausalPy-0.0.8/MANIFEST.in
--rw-r--r--   0 benjamv    (501) staff       (20)     9594 2023-01-04 14:16:43.163204 CausalPy-0.0.8/PKG-INFO
--rw-r--r--   0 benjamv    (501) staff       (20)     9289 2023-01-04 11:05:40.000000 CausalPy-0.0.8/README.md
-drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 14:16:43.160820 CausalPy-0.0.8/causalpy/
--rw-r--r--   0 benjamv    (501) staff       (20)      242 2022-11-24 10:00:18.000000 CausalPy-0.0.8/causalpy/__init__.py
-drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 14:16:43.162381 CausalPy-0.0.8/causalpy/data/
--rw-r--r--   0 benjamv    (501) staff       (20)    11574 2022-11-30 15:35:27.000000 CausalPy-0.0.8/causalpy/data/GDP_in_dollars_billions.csv
--rw-r--r--   0 benjamv    (501) staff       (20)       90 2022-11-23 17:12:53.000000 CausalPy-0.0.8/causalpy/data/__init__.py
--rw-r--r--   0 benjamv    (501) staff       (20)     7852 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/data/ancova_generated.csv
--rw-r--r--   0 benjamv    (501) staff       (20)    77216 2022-11-23 10:37:32.000000 CausalPy-0.0.8/causalpy/data/banks.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     1212 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/data/datasets.py
--rw-r--r--   0 benjamv    (501) staff       (20)     7379 2022-12-02 14:17:13.000000 CausalPy-0.0.8/causalpy/data/deaths_and_temps_england_wales.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     1339 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/data/did.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     9109 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/data/drinking.csv
--rw-r--r--   0 benjamv    (501) staff       (20)    29149 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/data/geolift1.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     4778 2022-10-28 10:08:58.000000 CausalPy-0.0.8/causalpy/data/its.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     4830 2022-10-28 10:08:58.000000 CausalPy-0.0.8/causalpy/data/its_simple.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     4520 2022-10-28 10:08:58.000000 CausalPy-0.0.8/causalpy/data/regression_discontinuity.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     9444 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/data/simulate_data.py
--rw-r--r--   0 benjamv    (501) staff       (20)    17645 2022-10-28 17:54:16.000000 CausalPy-0.0.8/causalpy/data/synthetic_control.csv
--rw-r--r--   0 benjamv    (501) staff       (20)     1273 2023-01-04 14:07:00.000000 CausalPy-0.0.8/causalpy/plot_utils.py
--rw-r--r--   0 benjamv    (501) staff       (20)    29737 2023-01-04 14:07:00.000000 CausalPy-0.0.8/causalpy/pymc_experiments.py
--rw-r--r--   0 benjamv    (501) staff       (20)     4263 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/pymc_models.py
--rw-r--r--   0 benjamv    (501) staff       (20)    13951 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/skl_experiments.py
--rw-r--r--   0 benjamv    (501) staff       (20)     1104 2022-11-15 15:51:03.000000 CausalPy-0.0.8/causalpy/skl_models.py
-drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 14:16:43.163030 CausalPy-0.0.8/causalpy/tests/
--rw-r--r--   0 benjamv    (501) staff       (20)        0 2022-11-25 13:01:06.000000 CausalPy-0.0.8/causalpy/tests/__init__.py
--rw-r--r--   0 benjamv    (501) staff       (20)      188 2022-12-04 17:29:41.000000 CausalPy-0.0.8/causalpy/tests/conftest.py
--rw-r--r--   0 benjamv    (501) staff       (20)      462 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/tests/test_data_loading.py
--rw-r--r--   0 benjamv    (501) staff       (20)     9376 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/tests/test_integration_pymc_examples.py
--rw-r--r--   0 benjamv    (501) staff       (20)     3327 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/tests/test_integration_skl_examples.py
--rw-r--r--   0 benjamv    (501) staff       (20)     3274 2023-01-04 11:05:40.000000 CausalPy-0.0.8/causalpy/tests/test_pymc_models.py
--rw-r--r--   0 benjamv    (501) staff       (20)       22 2023-01-04 14:16:17.000000 CausalPy-0.0.8/causalpy/version.py
--rw-r--r--   0 benjamv    (501) staff       (20)      893 2023-01-04 11:05:40.000000 CausalPy-0.0.8/pyproject.toml
--rw-r--r--   0 benjamv    (501) staff       (20)      144 2022-12-01 19:06:29.000000 CausalPy-0.0.8/requirements.txt
--rw-r--r--   0 benjamv    (501) staff       (20)      198 2023-01-04 14:16:43.163477 CausalPy-0.0.8/setup.cfg
--rw-r--r--   0 benjamv    (501) staff       (20)     1097 2022-12-08 19:21:49.000000 CausalPy-0.0.8/setup.py
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 19:28:08.751420 CausalPy-0.0.9/
+-rw-r--r--   0 benjamv    (501) staff       (20)     3514 2022-12-01 15:41:43.000000 CausalPy-0.0.9/CONTRIBUTING.md
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 19:28:08.747447 CausalPy-0.0.9/CausalPy.egg-info/
+-rw-r--r--   0 benjamv    (501) staff       (20)     9594 2023-01-04 19:28:08.000000 CausalPy-0.0.9/CausalPy.egg-info/PKG-INFO
+-rw-r--r--   0 benjamv    (501) staff       (20)     1084 2023-01-04 19:28:08.000000 CausalPy-0.0.9/CausalPy.egg-info/SOURCES.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)        1 2023-01-04 19:28:08.000000 CausalPy-0.0.9/CausalPy.egg-info/dependency_links.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)      144 2023-01-04 19:28:08.000000 CausalPy-0.0.9/CausalPy.egg-info/requires.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)        9 2023-01-04 19:28:08.000000 CausalPy-0.0.9/CausalPy.egg-info/top_level.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)    11357 2022-10-28 10:08:58.000000 CausalPy-0.0.9/LICENSE
+-rw-r--r--   0 benjamv    (501) staff       (20)       60 2022-11-24 10:00:18.000000 CausalPy-0.0.9/MANIFEST.in
+-rw-r--r--   0 benjamv    (501) staff       (20)     9594 2023-01-04 19:28:08.751507 CausalPy-0.0.9/PKG-INFO
+-rw-r--r--   0 benjamv    (501) staff       (20)     9289 2023-01-04 11:05:40.000000 CausalPy-0.0.9/README.md
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 19:28:08.748511 CausalPy-0.0.9/causalpy/
+-rw-r--r--   0 benjamv    (501) staff       (20)      242 2022-11-24 10:00:18.000000 CausalPy-0.0.9/causalpy/__init__.py
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 19:28:08.750316 CausalPy-0.0.9/causalpy/data/
+-rw-r--r--   0 benjamv    (501) staff       (20)    11574 2022-11-30 15:35:27.000000 CausalPy-0.0.9/causalpy/data/GDP_in_dollars_billions.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)       90 2022-11-23 17:12:53.000000 CausalPy-0.0.9/causalpy/data/__init__.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     7852 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/data/ancova_generated.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)    77216 2022-11-23 10:37:32.000000 CausalPy-0.0.9/causalpy/data/banks.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     1212 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/data/datasets.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     7379 2022-12-02 14:17:13.000000 CausalPy-0.0.9/causalpy/data/deaths_and_temps_england_wales.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     1339 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/data/did.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     9109 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/data/drinking.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)    29149 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/data/geolift1.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     4778 2022-10-28 10:08:58.000000 CausalPy-0.0.9/causalpy/data/its.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     4830 2022-10-28 10:08:58.000000 CausalPy-0.0.9/causalpy/data/its_simple.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     4520 2022-10-28 10:08:58.000000 CausalPy-0.0.9/causalpy/data/regression_discontinuity.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     9444 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/data/simulate_data.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    17645 2022-10-28 17:54:16.000000 CausalPy-0.0.9/causalpy/data/synthetic_control.csv
+-rw-r--r--   0 benjamv    (501) staff       (20)     1273 2023-01-04 14:07:00.000000 CausalPy-0.0.9/causalpy/plot_utils.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    30218 2023-01-04 19:26:36.000000 CausalPy-0.0.9/causalpy/pymc_experiments.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     4263 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/pymc_models.py
+-rw-r--r--   0 benjamv    (501) staff       (20)    15888 2023-01-04 19:26:36.000000 CausalPy-0.0.9/causalpy/skl_experiments.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     1104 2022-11-15 15:51:03.000000 CausalPy-0.0.9/causalpy/skl_models.py
+drwxr-xr-x   0 benjamv    (501) staff       (20)        0 2023-01-04 19:28:08.751294 CausalPy-0.0.9/causalpy/tests/
+-rw-r--r--   0 benjamv    (501) staff       (20)        0 2022-11-25 13:01:06.000000 CausalPy-0.0.9/causalpy/tests/__init__.py
+-rw-r--r--   0 benjamv    (501) staff       (20)      188 2022-12-04 17:29:41.000000 CausalPy-0.0.9/causalpy/tests/conftest.py
+-rw-r--r--   0 benjamv    (501) staff       (20)      462 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/tests/test_data_loading.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     9704 2023-01-04 19:26:36.000000 CausalPy-0.0.9/causalpy/tests/test_integration_pymc_examples.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     3392 2023-01-04 19:26:36.000000 CausalPy-0.0.9/causalpy/tests/test_integration_skl_examples.py
+-rw-r--r--   0 benjamv    (501) staff       (20)     3274 2023-01-04 11:05:40.000000 CausalPy-0.0.9/causalpy/tests/test_pymc_models.py
+-rw-r--r--   0 benjamv    (501) staff       (20)       22 2023-01-04 19:26:41.000000 CausalPy-0.0.9/causalpy/version.py
+-rw-r--r--   0 benjamv    (501) staff       (20)      893 2023-01-04 11:05:40.000000 CausalPy-0.0.9/pyproject.toml
+-rw-r--r--   0 benjamv    (501) staff       (20)      144 2022-12-01 19:06:29.000000 CausalPy-0.0.9/requirements.txt
+-rw-r--r--   0 benjamv    (501) staff       (20)      198 2023-01-04 19:28:08.751794 CausalPy-0.0.9/setup.cfg
+-rw-r--r--   0 benjamv    (501) staff       (20)     1097 2022-12-08 19:21:49.000000 CausalPy-0.0.9/setup.py
```

### Comparing `CausalPy-0.0.8/CONTRIBUTING.md` & `CausalPy-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/CausalPy.egg-info/PKG-INFO` & `CausalPy-0.0.9/CausalPy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CausalPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Causal inference for quasi-experiments in Python
 Home-page: https://github.com/pymc-labs/CausalPy
 Maintainer: Benjamin T. Vincent
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CausalPy-0.0.8/CausalPy.egg-info/SOURCES.txt` & `CausalPy-0.0.9/CausalPy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/LICENSE` & `CausalPy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/PKG-INFO` & `CausalPy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CausalPy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Causal inference for quasi-experiments in Python
 Home-page: https://github.com/pymc-labs/CausalPy
 Maintainer: Benjamin T. Vincent
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `CausalPy-0.0.8/README.md` & `CausalPy-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/GDP_in_dollars_billions.csv` & `CausalPy-0.0.9/causalpy/data/GDP_in_dollars_billions.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/ancova_generated.csv` & `CausalPy-0.0.9/causalpy/data/ancova_generated.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/banks.csv` & `CausalPy-0.0.9/causalpy/data/banks.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/datasets.py` & `CausalPy-0.0.9/causalpy/data/datasets.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/deaths_and_temps_england_wales.csv` & `CausalPy-0.0.9/causalpy/data/deaths_and_temps_england_wales.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/did.csv` & `CausalPy-0.0.9/causalpy/data/did.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/drinking.csv` & `CausalPy-0.0.9/causalpy/data/drinking.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/geolift1.csv` & `CausalPy-0.0.9/causalpy/data/geolift1.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/its.csv` & `CausalPy-0.0.9/causalpy/data/its.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/its_simple.csv` & `CausalPy-0.0.9/causalpy/data/its_simple.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/regression_discontinuity.csv` & `CausalPy-0.0.9/causalpy/data/regression_discontinuity.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/simulate_data.py` & `CausalPy-0.0.9/causalpy/data/simulate_data.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/data/synthetic_control.csv` & `CausalPy-0.0.9/causalpy/data/synthetic_control.csv`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/plot_utils.py` & `CausalPy-0.0.9/causalpy/plot_utils.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/pymc_experiments.py` & `CausalPy-0.0.9/causalpy/pymc_experiments.py`

 * *Files 3% similar despite different names*

```diff
@@ -336,41 +336,46 @@
             .first()
             .reset_index()
         )
         assert not self.x_pred_treatment.empty
         (new_x,) = build_design_matrices([self._x_design_info], self.x_pred_treatment)
         self.y_pred_treatment = self.model.predict(np.asarray(new_x))
 
-        # predicted outcome for counterfactual
+        # predicted outcome for counterfactual. This is given by removing the influence
+        # of the interaction term between the group and the post_treatment variable
         self.x_pred_counterfactual = (
             self.data
             # just the treated group
             .query(f"{self.group_variable_name} == @self.treated")
             # just the treatment period(s)
             .query("post_treatment == True")
             # drop the outcome variable
             .drop(self.outcome_variable_name, axis=1)
-            # DO AN INTERVENTION. Set the post_treatment variable to False
-            .assign(post_treatment=False)
             # We may have multiple units per time point, we only want one time point
             .groupby(self.time_variable_name)
             .first()
             .reset_index()
         )
         assert not self.x_pred_counterfactual.empty
         (new_x,) = build_design_matrices(
-            [self._x_design_info], self.x_pred_counterfactual
+            [self._x_design_info], self.x_pred_counterfactual, return_type="dataframe"
         )
+        # INTERVENTION: set the interaction term between the group and the
+        # post_treatment variable to zero. This is the counterfactual.
+        for i, label in enumerate(self.labels):
+            if "post_treatment" in label and self.group_variable_name in label:
+                new_x.iloc[:, i] = 0
         self.y_pred_counterfactual = self.model.predict(np.asarray(new_x))
 
-        # calculate causal impact
-        self.causal_impact = (
-            self.y_pred_treatment["posterior_predictive"].mu.isel({"obs_ind": 1})
-            - self.y_pred_counterfactual["posterior_predictive"].mu.squeeze()
-        )
+        # calculate causal impact.
+        # This is the coefficient on the interaction term
+        coeff_names = self.idata.posterior.coords["coeffs"].data
+        for i, label in enumerate(coeff_names):
+            if "post_treatment" in label and self.group_variable_name in label:
+                self.causal_impact = self.idata.posterior["beta"].isel({"coeffs": i})
 
     def plot(self):
         """Plot the results.
         Creating the combined mean + HDI legend entries is a bit involved.
         """
         fig, ax = plt.subplots()
```

### Comparing `CausalPy-0.0.8/causalpy/pymc_models.py` & `CausalPy-0.0.9/causalpy/pymc_models.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/skl_experiments.py` & `CausalPy-0.0.9/causalpy/skl_experiments.py`

 * *Files 7% similar despite different names*

```diff
@@ -172,58 +172,100 @@
     """
 
     def __init__(
         self,
         data: pd.DataFrame,
         formula: str,
         time_variable_name: str,
+        group_variable_name: str,
+        treated: str,
+        untreated: str,
         model=None,
         **kwargs,
     ):
         super().__init__(model=model, **kwargs)
         self.data = data
         self.formula = formula
         self.time_variable_name = time_variable_name
+        self.group_variable_name = group_variable_name
+        self.treated = treated  # level of the group_variable_name that was treated
+        self.untreated = (
+            untreated  # level of the group_variable_name that was untreated
+        )
         y, X = dmatrices(formula, self.data)
         self._y_design_info = y.design_info
         self._x_design_info = X.design_info
         self.labels = X.design_info.column_names
         self.y, self.X = np.asarray(y), np.asarray(X)
         self.outcome_variable_name = y.design_info.column_names[0]
 
         # fit the model to all the data
         self.model.fit(X=self.X, y=self.y)
 
         # predicted outcome for control group
-        self.x_pred_control = pd.DataFrame(
-            {"group": [0, 0], "t": [0.0, 1.0], "post_treatment": [0, 0]}
+        self.x_pred_control = (
+            self.data
+            # just the untreated group
+            .query(f"{self.group_variable_name} == @self.untreated")
+            # drop the outcome variable
+            .drop(self.outcome_variable_name, axis=1)
+            # We may have multiple units per time point, we only want one time point
+            .groupby(self.time_variable_name)
+            .first()
+            .reset_index()
         )
         assert not self.x_pred_control.empty
         (new_x,) = build_design_matrices([self._x_design_info], self.x_pred_control)
         self.y_pred_control = self.model.predict(np.asarray(new_x))
 
         # predicted outcome for treatment group
-        self.x_pred_treatment = pd.DataFrame(
-            {"group": [1, 1], "t": [0.0, 1.0], "post_treatment": [0, 1]}
+        self.x_pred_treatment = (
+            self.data
+            # just the treated group
+            .query(f"{self.group_variable_name} == @self.treated")
+            # drop the outcome variable
+            .drop(self.outcome_variable_name, axis=1)
+            # We may have multiple units per time point, we only want one time point
+            .groupby(self.time_variable_name)
+            .first()
+            .reset_index()
         )
         assert not self.x_pred_treatment.empty
         (new_x,) = build_design_matrices([self._x_design_info], self.x_pred_treatment)
         self.y_pred_treatment = self.model.predict(np.asarray(new_x))
 
-        # predicted outcome for counterfactual
-        self.x_pred_counterfactual = pd.DataFrame(
-            {"group": [1], "t": [1.0], "post_treatment": [0]}
+        # predicted outcome for counterfactual. This is given by removing the influence
+        # of the interaction term between the group and the post_treatment variable
+        self.x_pred_counterfactual = (
+            self.data
+            # just the treated group
+            .query(f"{self.group_variable_name} == @self.treated")
+            # just the treatment period(s)
+            .query("post_treatment == True")
+            # drop the outcome variable
+            .drop(self.outcome_variable_name, axis=1)
+            # We may have multiple units per time point, we only want one time point
+            .groupby(self.time_variable_name)
+            .first()
+            .reset_index()
         )
         assert not self.x_pred_counterfactual.empty
         (new_x,) = build_design_matrices(
-            [self._x_design_info], self.x_pred_counterfactual
+            [self._x_design_info], self.x_pred_counterfactual, return_type="dataframe"
         )
+        # INTERVENTION: set the interaction term between the group and the
+        # post_treatment variable to zero. This is the counterfactual.
+        for i, label in enumerate(self.labels):
+            if "post_treatment" in label and self.group_variable_name in label:
+                new_x.iloc[:, i] = 0
         self.y_pred_counterfactual = self.model.predict(np.asarray(new_x))
 
         # calculate causal impact
+        # This is the coefficient on the interaction term
+        # TODO: THIS IS NOT YET CORRECT
         self.causal_impact = self.y_pred_treatment[1] - self.y_pred_counterfactual[0]
 
     def plot(self):
         """Plot results"""
         fig, ax = plt.subplots()
 
         # Plot raw data
```

### Comparing `CausalPy-0.0.8/causalpy/skl_models.py` & `CausalPy-0.0.9/causalpy/skl_models.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/causalpy/tests/test_integration_pymc_examples.py` & `CausalPy-0.0.9/causalpy/tests/test_integration_pymc_examples.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 
 @pytest.mark.integration
 def test_did():
     df = cp.load_data("did")
     result = cp.pymc_experiments.DifferenceInDifferences(
         df,
-        formula="y ~ 1 + group + t + group:post_treatment",
+        formula="y ~ 1 + group*post_treatment",
         time_variable_name="t",
         group_variable_name="group",
         treated=1,
         untreated=0,
         model=cp.pymc_models.LinearRegression(sample_kwargs=sample_kwargs),
     )
     assert isinstance(df, pd.DataFrame)
@@ -33,32 +33,38 @@
     df = (
         cp.load_data("banks")
         .filter(items=["bib6", "bib8", "year"])
         .rename(columns={"bib6": "Sixth District", "bib8": "Eighth District"})
         .groupby("year")
         .median()
     )
+    # SET TREATMENT TIME TO ZERO =========
+    df.index = df.index - treatment_time
+    treatment_time = 0
+    # ====================================
     df.reset_index(level=0, inplace=True)
     df_long = pd.melt(
         df,
         id_vars=["year"],
         value_vars=["Sixth District", "Eighth District"],
         var_name="district",
         value_name="bib",
     ).sort_values("year")
-    df_long["district"] = df_long["district"].astype("category")
     df_long["unit"] = df_long["district"]
     df_long["post_treatment"] = df_long.year >= treatment_time
+    df_long = df_long.replace({"district": {"Sixth District": 1, "Eighth District": 0}})
+
     result = cp.pymc_experiments.DifferenceInDifferences(
-        df_long[df_long.year.isin([1930, 1931])],
-        formula="bib ~ 1 + district + year + district:post_treatment",
+        # df_long[df_long.year.isin([1930, 1931])],
+        df_long[df_long.year.isin([-0.5, 0.5])],
+        formula="bib ~ 1 + district * post_treatment",
         time_variable_name="year",
         group_variable_name="district",
-        treated="Sixth District",
-        untreated="Eighth District",
+        treated=1,
+        untreated=0,
         model=cp.pymc_models.LinearRegression(sample_kwargs=sample_kwargs),
     )
     assert isinstance(df, pd.DataFrame)
     assert isinstance(result, cp.pymc_experiments.DifferenceInDifferences)
     assert len(result.idata.posterior.coords["chain"]) == sample_kwargs["chains"]
     assert len(result.idata.posterior.coords["draw"]) == sample_kwargs["draws"]
 
@@ -69,32 +75,37 @@
     df = (
         cp.load_data("banks")
         .filter(items=["bib6", "bib8", "year"])
         .rename(columns={"bib6": "Sixth District", "bib8": "Eighth District"})
         .groupby("year")
         .median()
     )
+    # SET TREATMENT TIME TO ZERO =========
+    df.index = df.index - treatment_time
+    treatment_time = 0
+    # ====================================
     df.reset_index(level=0, inplace=True)
     df_long = pd.melt(
         df,
         id_vars=["year"],
         value_vars=["Sixth District", "Eighth District"],
         var_name="district",
         value_name="bib",
     ).sort_values("year")
-    df_long["district"] = df_long["district"].astype("category")
     df_long["unit"] = df_long["district"]
     df_long["post_treatment"] = df_long.year >= treatment_time
+    df_long = df_long.replace({"district": {"Sixth District": 1, "Eighth District": 0}})
+
     result = cp.pymc_experiments.DifferenceInDifferences(
         df_long,
-        formula="bib ~ 1 + district + year + district:post_treatment",
+        formula="bib ~ 1 + year + district + post_treatment + district:post_treatment",
         time_variable_name="year",
         group_variable_name="district",
-        treated="Sixth District",
-        untreated="Eighth District",
+        treated=1,
+        untreated=0,
         model=cp.pymc_models.LinearRegression(sample_kwargs=sample_kwargs),
     )
     assert isinstance(df, pd.DataFrame)
     assert isinstance(result, cp.pymc_experiments.DifferenceInDifferences)
     assert len(result.idata.posterior.coords["chain"]) == sample_kwargs["chains"]
     assert len(result.idata.posterior.coords["draw"]) == sample_kwargs["draws"]
```

### Comparing `CausalPy-0.0.8/causalpy/tests/test_integration_skl_examples.py` & `CausalPy-0.0.9/causalpy/tests/test_integration_skl_examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,16 +8,19 @@
 
 
 @pytest.mark.integration
 def test_did():
     data = cp.load_data("did")
     result = cp.skl_experiments.DifferenceInDifferences(
         data,
-        formula="y ~ 1 + group + t + group:post_treatment",
+        formula="y ~ 1 + group*post_treatment",
         time_variable_name="t",
+        group_variable_name="group",
+        treated=1,
+        untreated=0,
         model=LinearRegression(),
     )
     assert isinstance(data, pd.DataFrame)
     assert isinstance(result, cp.skl_experiments.DifferenceInDifferences)
 
 
 @pytest.mark.integration
```

### Comparing `CausalPy-0.0.8/causalpy/tests/test_pymc_models.py` & `CausalPy-0.0.9/causalpy/tests/test_pymc_models.py`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/pyproject.toml` & `CausalPy-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `CausalPy-0.0.8/setup.py` & `CausalPy-0.0.9/setup.py`

 * *Files identical despite different names*

