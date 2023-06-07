# Comparing `tmp/acryl-datahub-classify-0.0.7.tar.gz` & `tmp/acryl-datahub-classify-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acryl-datahub-classify-0.0.7.tar", last modified: Mon Jun  5 19:21:29 2023, max compression
+gzip compressed data, was "acryl-datahub-classify-0.0.8.tar", last modified: Wed Jun  7 23:25:34 2023, max compression
```

## Comparing `acryl-datahub-classify-0.0.7.tar` & `acryl-datahub-classify-0.0.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-05 19:21:29.000000 acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/src/datahub_classify/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-05 19:21:22.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/helper_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    28228 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3238 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/src/datahub_classify/reference_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 19:21:29.020927 acryl-datahub-classify-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/tests/test_custom_infotype_predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-05 18:45:38.000000 acryl-datahub-classify-0.0.7/tests/test_infotype_predictor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:25:34.290026 acryl-datahub-classify-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-07 23:25:34.290026 acryl-datahub-classify-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-07 23:25:34.290026 acryl-datahub-classify-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:25:34.286026 acryl-datahub-classify-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:25:34.286026 acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6864 2023-06-07 23:25:34.000000 acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      633 2023-06-07 23:25:34.000000 acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:25:34.000000 acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-07 23:25:34.000000 acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-07 23:25:34.000000 acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:25:34.290026 acryl-datahub-classify-0.0.8/src/datahub_classify/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-07 23:25:25.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/helper_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28228 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/infotype_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4336 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/infotype_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/infotype_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19740 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/src/datahub_classify/reference_input.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:25:34.290026 acryl-datahub-classify-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/tests/test_custom_infotype_predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-06-07 22:31:55.000000 acryl-datahub-classify-0.0.8/tests/test_infotype_predictor.py
```

### Comparing `acryl-datahub-classify-0.0.7/PKG-INFO` & `acryl-datahub-classify-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-datahub-classify
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library to predict info types for DataHub
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/
 Project-URL: Source, https://github.com/acryldata/datahub-classify
 Project-URL: Changelog, https://github.com/acryldata/datahub-classify/releases
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,15 @@
 
 API expects following parameters in the output
 
 - `column_infos` - This is a list of ColumnInfo objects. Each ColumnInfo object contains metadata (col_name, description, datatype, etc) and values of a column.
 - `confidence_level_threshold` - If the infotype prediction confidence is greater than the confidence threshold then the prediction is considered as a proposal. This is the common threshold for all infotypes.
 - `global_config` - This dictionary contains configuration details about all supported infotypes. Refer section [Infotype Configuration](#infotype-configuration) for more information.
 - `infotypes` - This is a list of infotypes that is to be processed. This is an optional argument, if specified then it will override the default list of all supported infotypes. If user is interested in only few infotypes then this list can be specified with correct infotype names. Infotype names are case sensitive.
+- `minimum_values_threshold` - Minimum number of column values required for processing. This is an optional argument, default is 50.
 
 ### API Output
 
 API returns a list of ColumnInfo objects of length same as input ColumnInfo objects list. A populated list of Infotype proposal(s), if any, is added in the ColumnInfo object itself with a variable name as `infotype_proposals`. The infotype_proposals list contains InfotypeProposal objects which has following information
 
 - `infotype` - A proposed infotype name.
 - `confidence_level` - Overall confidence of the infotype proposal.
```

### Comparing `acryl-datahub-classify-0.0.7/README.md` & `acryl-datahub-classify-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 
 API expects following parameters in the output
 
 - `column_infos` - This is a list of ColumnInfo objects. Each ColumnInfo object contains metadata (col_name, description, datatype, etc) and values of a column.
 - `confidence_level_threshold` - If the infotype prediction confidence is greater than the confidence threshold then the prediction is considered as a proposal. This is the common threshold for all infotypes.
 - `global_config` - This dictionary contains configuration details about all supported infotypes. Refer section [Infotype Configuration](#infotype-configuration) for more information.
 - `infotypes` - This is a list of infotypes that is to be processed. This is an optional argument, if specified then it will override the default list of all supported infotypes. If user is interested in only few infotypes then this list can be specified with correct infotype names. Infotype names are case sensitive.
+- `minimum_values_threshold` - Minimum number of column values required for processing. This is an optional argument, default is 50.
 
 ### API Output
 
 API returns a list of ColumnInfo objects of length same as input ColumnInfo objects list. A populated list of Infotype proposal(s), if any, is added in the ColumnInfo object itself with a variable name as `infotype_proposals`. The infotype_proposals list contains InfotypeProposal objects which has following information
 
 - `infotype` - A proposed infotype name.
 - `confidence_level` - Overall confidence of the infotype proposal.
```

### Comparing `acryl-datahub-classify-0.0.7/setup.cfg` & `acryl-datahub-classify-0.0.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/setup.py` & `acryl-datahub-classify-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/PKG-INFO` & `acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acryl-datahub-classify
-Version: 0.0.7
+Version: 0.0.8
 Summary: Library to predict info types for DataHub
 Home-page: https://datahubproject.io/
 License: Apache License 2.0
 Project-URL: Documentation, https://datahubproject.io/docs/
 Project-URL: Source, https://github.com/acryldata/datahub-classify
 Project-URL: Changelog, https://github.com/acryldata/datahub-classify/releases
 Classifier: Development Status :: 5 - Production/Stable
@@ -44,14 +44,15 @@
 
 API expects following parameters in the output
 
 - `column_infos` - This is a list of ColumnInfo objects. Each ColumnInfo object contains metadata (col_name, description, datatype, etc) and values of a column.
 - `confidence_level_threshold` - If the infotype prediction confidence is greater than the confidence threshold then the prediction is considered as a proposal. This is the common threshold for all infotypes.
 - `global_config` - This dictionary contains configuration details about all supported infotypes. Refer section [Infotype Configuration](#infotype-configuration) for more information.
 - `infotypes` - This is a list of infotypes that is to be processed. This is an optional argument, if specified then it will override the default list of all supported infotypes. If user is interested in only few infotypes then this list can be specified with correct infotype names. Infotype names are case sensitive.
+- `minimum_values_threshold` - Minimum number of column values required for processing. This is an optional argument, default is 50.
 
 ### API Output
 
 API returns a list of ColumnInfo objects of length same as input ColumnInfo objects list. A populated list of Infotype proposal(s), if any, is added in the ColumnInfo object itself with a variable name as `infotype_proposals`. The infotype_proposals list contains InfotypeProposal objects which has following information
 
 - `infotype` - A proposed infotype name.
 - `confidence_level` - Overall confidence of the infotype proposal.
```

### Comparing `acryl-datahub-classify-0.0.7/src/acryl_datahub_classify.egg-info/SOURCES.txt` & `acryl-datahub-classify-0.0.8/src/acryl_datahub_classify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/src/datahub_classify/helper_classes.py` & `acryl-datahub-classify-0.0.8/src/datahub_classify/helper_classes.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_helper.py` & `acryl-datahub-classify-0.0.8/src/datahub_classify/infotype_helper.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_predictor.py` & `acryl-datahub-classify-0.0.8/src/datahub_classify/infotype_predictor.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 
 
 def predict_infotypes(
     column_infos: List[ColumnInfo],
     confidence_level_threshold: float,
     global_config: Dict[str, Dict],
     infotypes: Optional[List[str]] = None,
+    minimum_values_threshold: int = 50,
 ) -> List[ColumnInfo]:
     infotype_function_map = get_infotype_function_mapping(infotypes, global_config)
     logger.debug(f"Total columns to be processed --> {len(column_infos)}")
     logger.debug(f"Confidence Level Threshold set to --> {confidence_level_threshold}")
     logger.debug("===========================================================")
     basic_checks_failed_columns = []
     num_cols_with_infotype_assigned = 0
@@ -58,15 +59,19 @@
             column_info.values = [
                 val
                 for val in column_info.values
                 if str(val).strip() not in ["nan", "", "None"]
             ]
             try:
                 if perform_basic_checks(
-                    column_info.metadata, column_info.values, config_dict, infotype
+                    column_info.metadata,
+                    column_info.values,
+                    config_dict,
+                    infotype,
+                    minimum_values_threshold,
                 ):
                     confidence_level, debug_info = infotype_fn(
                         column_info.metadata, column_info.values, config_dict
                     )
                     if confidence_level > confidence_level_threshold:
                         infotype_proposal = InfotypeProposal(
                             infotype, confidence_level, debug_info
```

### Comparing `acryl-datahub-classify-0.0.7/src/datahub_classify/infotype_utils.py` & `acryl-datahub-classify-0.0.8/src/datahub_classify/infotype_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 import re
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List
 
 from datahub_classify.constants import PREDICTION_FACTORS_AND_WEIGHTS, VALUES
 from datahub_classify.helper_classes import Metadata
 
 logger = logging.getLogger(__name__)
 
 
@@ -79,18 +79,18 @@
     return False
 
 
 def perform_basic_checks(
     metadata: Metadata,
     values: List[Any],
     config_dict: Dict[str, Dict],
-    infotype: Optional[str] = None,
+    infotype: str,
+    minimum_values_threshold: int,
 ) -> bool:
     basic_checks_status = True
-    minimum_values_threshold = 50
     if (
         config_dict[PREDICTION_FACTORS_AND_WEIGHTS].get(VALUES, None)
         and len(values) < minimum_values_threshold
     ):
         basic_checks_status = False
     # TODO: Add more basic checks
     return basic_checks_status
```

### Comparing `acryl-datahub-classify-0.0.7/src/datahub_classify/reference_input.py` & `acryl-datahub-classify-0.0.8/src/datahub_classify/reference_input.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/tests/test_custom_infotype_predictor.py` & `acryl-datahub-classify-0.0.8/tests/test_custom_infotype_predictor.py`

 * *Files identical despite different names*

### Comparing `acryl-datahub-classify-0.0.7/tests/test_infotype_predictor.py` & `acryl-datahub-classify-0.0.8/tests/test_infotype_predictor.py`

 * *Files identical despite different names*

