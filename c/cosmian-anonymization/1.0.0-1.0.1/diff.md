# Comparing `tmp/cosmian_anonymization-1.0.0-py3-none-any.whl.zip` & `tmp/cosmian_anonymization-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19147 bytes, number of entries: 11
+Zip file size: 19952 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      169 b- defN 80-Jan-01 00:00 cosmian_anonymization/__init__.py
--rw-r--r--  2.0 unx     6088 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
--rw-r--r--  2.0 unx      602 b- defN 80-Jan-01 00:00 cosmian_anonymization/date_helper.py
--rw-r--r--  2.0 unx     3494 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
--rw-r--r--  2.0 unx     3760 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
--rw-r--r--  2.0 unx     3857 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
--rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.0.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1151 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.0.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1023 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.0.0.dist-info/RECORD
-11 files, 52580 bytes uncompressed, 17379 bytes compressed:  66.9%
+-rw-r--r--  2.0 unx     7352 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
+-rw-r--r--  2.0 unx     1763 b- defN 80-Jan-01 00:00 cosmian_anonymization/conversion_helper.py
+-rw-r--r--  2.0 unx     3495 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
+-rw-r--r--  2.0 unx     3784 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
+-rw-r--r--  2.0 unx     3887 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
+-rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1281 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/RECORD
+11 files, 55197 bytes uncompressed, 18172 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: cosmian_anonymization/__init__.py
 Comment: 
 
 Filename: cosmian_anonymization/anonymize.py
 Comment: 
 
-Filename: cosmian_anonymization/date_helper.py
+Filename: cosmian_anonymization/conversion_helper.py
 Comment: 
 
 Filename: cosmian_anonymization/method_parser.py
 Comment: 
 
 Filename: cosmian_anonymization/noise_correlation.py
 Comment: 
 
 Filename: cosmian_anonymization/noise_parser.py
 Comment: 
 
-Filename: cosmian_anonymization-1.0.0.dist-info/LICENSE.md
+Filename: cosmian_anonymization-1.0.1.dist-info/LICENSE.md
 Comment: 
 
-Filename: cosmian_anonymization-1.0.0.dist-info/METADATA
+Filename: cosmian_anonymization-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_anonymization-1.0.0.dist-info/WHEEL
+Filename: cosmian_anonymization-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: cosmian_anonymization-1.0.0.dist-info/entry_points.txt
+Filename: cosmian_anonymization-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: cosmian_anonymization-1.0.0.dist-info/RECORD
+Filename: cosmian_anonymization-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cosmian_anonymization/anonymize.py

```diff
@@ -2,29 +2,67 @@
 import argparse
 import json
 from typing import Dict, Optional
 
 import pandas as pd
 from humps import decamelize
 
+from .conversion_helper import convert_config_types
 from .method_parser import create_transformation_function
 from .noise_correlation import NoiseCorrelationTask, parse_noise_correlation_config
 
 
+def create_output_dataframe(df: pd.DataFrame, config: Dict, inplace: bool):
+    """Create an output DataFrame based on a configuration.
+    Check that the input data match the configuration provided.
+
+    Args:
+        df (pd.DataFrame): The input DataFrame.
+        config (Dict): The configuration specifying the desired output columns and their types.
+        inplace (bool): Whether to modify the input DataFrame in-place or create a new DataFrame.
+
+    Returns:
+        pd.DataFrame: The output DataFrame with columns in the specified order.
+
+    Raises:
+        ValueError: If a column specified in the configuration is missing from the input DataFrame.
+    """
+    output_df = df
+    if not inplace:
+        output_df = pd.DataFrame()
+
+    # List of the column names in the config's order
+    sorted_output_columns = []
+    for column_metadata in config["metadata"]:
+        col_name = column_metadata["name"]
+        col_type = column_metadata["type"]
+
+        if col_name not in df:
+            # Column missing from the dataset
+            raise ValueError(f"Missing column from data: {col_name}.")
+
+        # Add this column as output to match the config's order
+        sorted_output_columns.append(col_name)
+
+        # Make sure the type of the pandas column is the same as the one in the config
+        output_df[col_name] = convert_config_types(df[col_name], col_type)
+
+    # Return the output dataframe with columns in the config's order
+    return output_df[sorted_output_columns]
+
+
 def apply_anonymization_column(
-    df: pd.DataFrame,
-    name: str,
+    values: pd.Series,
     method: Optional[str] = None,
     method_options: Dict = {},
-    **kwargs,
 ):
     """Apply anonymization to a specific column in a DataFrame.
 
     Args:
-        df (pd.DataFrame): The DataFrame to apply anonymization to.
+        values (pd.Series): The values to apply anonymization to.
         name (str): The name of the column to anonymize.
         method (Optional[str], optional): The method to use for anonymization. Defaults to None.
         method_options (Dict, optional): Additional options for the anonymization method. Defaults to {}.
         **kwargs: Additional config fields are ignored.
 
     Returns:
         pd.Series: The anonymized column.
@@ -33,43 +71,39 @@
         ValueError: If the specified column is missing from the DataFrame.
 
     Notes:
         - If `method` is None, the original column is returned without applying any anonymization.
         - In case of noise with correlation, the function returns None.
 
     """
-    if name not in df:
-        # Column missing from the dataset
-        raise ValueError(f"Missing column from data: {name}.")
-
-    if method is None:
+    if method is None or "correlation" in method_options:
         # No method to apply for this column
-        return df[name]
+        return values
 
     if "correlation" in method_options:
         # Correlation is done later in a dedicated function: `apply_correlation_columns`
-        return None
+        return values
 
     # Create a transformation function based on the selected technique.
     transform_func = create_transformation_function(method, method_options)
-    return df[name].map(transform_func)
+    return values.map(transform_func)
 
 
-def apply_correlation_columns(df: pd.DataFrame, task: NoiseCorrelationTask):
+def apply_correlation_columns(values: pd.Series, task: NoiseCorrelationTask):
     """Apply noise correlation to specified columns in a DataFrame.
 
     Args:
-        df (pd.DataFrame): The DataFrame to apply noise correlation to.
+        values (pd.Series): The values to apply noise correlation to.
         task (NoiseCorrelationTask): The task containing column names and transformation function.
 
     Returns:
         pd.DataFrame: The columns with noise correlation applied.
     """
     transform_func = task.generate_transformation()
-    return df[task.column_names].apply(transform_func, axis=1, raw=True)
+    return values.apply(transform_func, axis=1, raw=True)
 
 
 def anonymize_dataframe(
     df: pd.DataFrame, config: Dict, inplace: bool = False
 ) -> pd.DataFrame:
     """
     Anonymizes a Pandas DataFrame by applying the specified techniques to selected columns.
@@ -79,39 +113,38 @@
         config: A dictionary containing the metadata for each column to anonymize.
         inplace: If True, applies the anonymization directly to the input DataFrame.
             If False, creates a new DataFrame with the anonymized data.
     """
     # Convert config from camel case to snake case
     config = decamelize(config)
 
-    sorted_output_columns = []
-    anonymized_df = df
-    if not inplace:
-        anonymized_df = pd.DataFrame()
+    # Init output dataframe to match the config columns
+    output_df = create_output_dataframe(df, config, inplace)
 
     # Iterate over each column to anonymize.
     for column_metadata in config["metadata"]:
         col_name: str = column_metadata["name"]
-        # Add this column as output to match the config's order
-        sorted_output_columns.append(col_name)
-
-        anonymized_column = apply_anonymization_column(df, **column_metadata)
-        # Return column could be None for correlation methods
-        if anonymized_column is not None:
-            anonymized_df[col_name] = anonymized_column
+        # Anonymize the column
+        output_df[col_name] = apply_anonymization_column(
+            output_df[col_name],
+            column_metadata["method"],
+            column_metadata["method_options"],
+        )
 
     # -- Noise correlation --
     # Read through the config to find all correlation tasks
     noise_corr_tasks = parse_noise_correlation_config(config)
     # Apply correlation on each groups
     for task in noise_corr_tasks.values():
-        anonymized_df[task.column_names] = apply_correlation_columns(df, task)
+        output_df[task.column_names] = apply_correlation_columns(
+            output_df[task.column_names], task
+        )
 
-    # Return the anonymized data with columns in the config's order
-    return anonymized_df[sorted_output_columns]
+    # Return the anonymized data
+    return output_df
 
 
 def anonymize_from_files(data_path: str, config_path: str, output_path: str) -> None:
     """
     Reads the configuration file and data file, anonymizes the data according to the configuration,
     and writes the anonymized data to a new file.
```

## cosmian_anonymization/method_parser.py

```diff
@@ -9,15 +9,15 @@
     NumberScaler,
     WordMasker,
     WordPatternMasker,
     WordTokenizer,
 )
 from cloudproof_py.fpe import Alphabet, Float, Integer
 
-from .date_helper import date_to_rfc3339
+from .conversion_helper import date_to_rfc3339
 from .noise_parser import create_noise_generator, parse_date_noise_options
 
 
 def parse_date_aggregation_options(time_unit: str) -> Callable[[str], str]:
     """
     Parses the date aggregation options and returns a function that applies the aggregation.
 
@@ -58,15 +58,15 @@
         encoding (str): The encoding to use when converting the input string to bytes.
     """
     salt = None
     if salt_value:
         salt = salt_value.encode(encoding)
     hasher = Hasher(hash_type, salt)
 
-    return lambda val: hasher.apply_str(str(val))
+    return lambda val: hasher.apply_str(val)
 
 
 def create_transformation_function(method_name: str, method_opts: Dict) -> Callable:
     """
     Given a method name and options, returns a callable that applies the desired transformation.
     """
     parsing_functions: Dict[str, Callable] = {
```

## cosmian_anonymization/noise_correlation.py

```diff
@@ -1,7 +1,8 @@
+# -*- coding: utf-8 -*-
 from typing import Callable, Dict, List
 
 from .noise_parser import create_date_noise_generator, create_noise_generator
 
 
 class NoiseCorrelationTask:
     """
```

## cosmian_anonymization/noise_parser.py

```diff
@@ -1,12 +1,13 @@
+# -*- coding: utf-8 -*-
 from typing import Callable, Dict, Optional
 
 from cloudproof_anonymization import NoiseGenerator
 
-from .date_helper import DURATION_IN_SECONDS, date_to_rfc3339
+from .conversion_helper import DURATION_IN_SECONDS, date_to_rfc3339
 
 
 def create_noise_generator(
     distribution: str,
     mean: Optional[float] = None,
     std_dev: Optional[float] = None,
     lower_boundary: Optional[float] = None,
```

## Comparing `cosmian_anonymization-1.0.0.dist-info/LICENSE.md` & `cosmian_anonymization-1.0.1.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `cosmian_anonymization-1.0.0.dist-info/METADATA` & `cosmian_anonymization-1.0.1.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmian-anonymization
-Version: 1.0.0
+Version: 1.0.1
 Summary: Cosmian Anonymization library in Python
 Author: Hugo Rosenkranz-Costa
 Author-email: hugo.rosenkranz@cosmian.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -23,15 +23,19 @@
 ## Usage
 
 - As a library
 
 ```python
 from cosmian_anonymization import anonymize_dataframe
 
-df_anonymized = anonymize_dataframe(df_raw, config)
+try:
+    # Anonymize the raw data according to a configuration.
+    anonymized_df = anonymize_dataframe(df_raw, config)
+except ValueError as e:
+    print("Anonymization failed:", e)
 ```
 
 - From command line
 
 ```bash
 cosmian-anonymize <input_csv> <input_config> <output_csv>
 ```
```

