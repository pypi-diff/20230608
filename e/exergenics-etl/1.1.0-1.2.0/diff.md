# Comparing `tmp/exergenics-etl-1.1.0.tar.gz` & `tmp/exergenics-etl-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exergenics-etl-1.1.0.tar", last modified: Fri Jun  2 07:03:40 2023, max compression
+gzip compressed data, was "exergenics-etl-1.2.0.tar", last modified: Thu Jun  8 00:19:55 2023, max compression
```

## Comparing `exergenics-etl-1.1.0.tar` & `exergenics-etl-1.2.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50236 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/src/exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/src/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    34199 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/test_exergenics_etl.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-02 07:03:37.000000 exergenics-etl-1.1.0/app/exergenics_etl/test/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-02 07:03:40.000000 exergenics-etl-1.1.0/app/exergenics_etl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-02 07:03:40.080631 exergenics-etl-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-02 07:03:39.000000 exergenics-etl-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.376217 exergenics-etl-1.2.0/app/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.376217 exergenics-etl-1.2.0/app/exergenics_etl/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/app/exergenics_etl/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52545 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/src/exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4620 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/src/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/app/exergenics_etl/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34705 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/test_exergenics_etl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-08 00:19:52.000000 exergenics-etl-1.2.0/app/exergenics_etl/test/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:19:55.376217 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 00:19:55.000000 exergenics-etl-1.2.0/app/exergenics_etl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:19:55.380217 exergenics-etl-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-08 00:19:54.000000 exergenics-etl-1.2.0/setup.py
```

### Comparing `exergenics-etl-1.1.0/LICENSE` & `exergenics-etl-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.1.0/app/exergenics_etl/__init__.py` & `exergenics-etl-1.2.0/app/exergenics_etl/__init__.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.1.0/app/exergenics_etl/src/exergenics_etl.py` & `exergenics-etl-1.2.0/app/exergenics_etl/src/exergenics_etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import zipfile
 import sqlalchemy
 try:
     from ..src.logger import ETLLogger as Logger
 except:
     from logger import ETLLogger as Logger
 import pandas as pd
+import numpy as np
 from pytz import timezone
 from datetime import datetime
 from typing import Union, Dict, Callable
 from exergenics import exergenics
 from urllib.parse import quote_plus
 from sqlalchemy import create_engine
 from Levenshtein import distance as levenshtein_distance
@@ -137,25 +138,26 @@
         raise TypeError(
             f"Input password is not a string: password = {password}")
     engine = create_engine(url)
 
     return engine
 
 
-def get_time_now() -> str:
+def get_time_now(timestampFormat="%Y_%m_%d_%H%M") -> str:
     """Returns the current date and time in Melbourne the format 'YYYY_MM_DD_HHMM'.
 
     Returns:
         str: A string representing the current date and time in Melbourne.
     """
     now = datetime.now().astimezone(tz=timezone('Australia/Melbourne'))
-    dt_string = now.strftime("%Y_%m_%d_%H%M")
+    dt_string = now.strftime(timestampFormat)
     return dt_string
 
 
+
 def structure_slack_message(bCode: str = "", jobId: Union[int, str] = "", message: str = "") -> str:
     """Creates a formatted Slack message string.
 
     Args:
         bCode (str, optional): The building code associated with the job. Defaults to "".
         jobId (Union[int, str], optional): The job ID. Defaults to "".
         message (str, optional): The message to be sent to a Slack channel. Defaults to "".
@@ -562,33 +564,60 @@
                 raise EtlError(userMessage)
 
         logger.info(
             'Verifying timestamp column header ... Timestamp header is VALID!')
         return True
 
     def _check_for_wide_format(self, df: pd.DataFrame) -> bool:
-        """Method check whether input file is in a wide format.
+        """Method check whether input dataframe is in a wide format.
 
         Args:
             df (pd.DataFrame): Pandas DataFrame to apply format checking on. 
 
+        Raises:
+            EtlError: If the input dataframe is in a long format.
+
         Returns:
             bool: True if input is in a wide format.
         """
 
         # If there are only 3 columns in this data file
         if df.shape[1] == N_COLUMN_LONG_DATA:
 
+            # Check if the 2nd or 3rd column is a variable name column
+
             # If none of the values in the 2nd column can be converted to float
-            col2 = df[df.columns[1]]
-            if not any(col2.apply(convertable_to_float)):
+            secondColumnName = df.columns[1]
+            secondColumn = df[secondColumnName]
+            if not any(secondColumn.apply(convertable_to_float)):
 
                 # If the average length of the strings in the 2nd column is longer than 10
-                if col2.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
-                    return False  # We think this is a wide format dataset
+                if secondColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
+                    
+                    # Raise error when a long format dataset is detected
+                    errorMessage = 'This data file looks like in a long format. ' \
+                        + f'The 2nd column (\"{secondColumnName}\") is likely a variable name column. ' \
+                        + 'However, we currently only accept datasets in a wide format.'
+                    logger.error(errorMessage)
+                    raise EtlError(errorMessage)
+            
+            # If none of the values in the 3rd column can be converted to float
+            thirdColumnName = df.columns[2]
+            thirdColumn = df[thirdColumnName]
+            if not any(thirdColumn.apply(convertable_to_float)):
+
+                # If the average length of the strings in the 3rd column is longer than 10
+                if thirdColumn.apply(lambda x: len(x)).mean() > LENGTH_THRESHOLD:
+
+                    # Raise error when a long format dataset is detected
+                    errorMessage = 'This data file looks like in a long format. ' \
+                        + f'The 3rd column (\"{thirdColumnName}\") is likely a variable name column. ' \
+                        + 'However, we currently only accept datasets in a wide format.'
+                    logger.error(errorMessage)
+                    raise EtlError(errorMessage)
 
         return True
 
     def check_input_dataframe(self, df: pd.DataFrame) -> bool:
         """Validate the format of a dataframe read from a data file.
 
         Args:
@@ -603,17 +632,16 @@
             bool: True if all validations are passed.
         """
 
         logger = Logger()
 
         try:
             self._validate_timestamp_column_header(df)
-            assert self._check_for_wide_format(
-                df), 'This data file looks like in a long format. We currently only accept datasets in a wide format.'
-        except (AssertionError, EtlError) as e:
+            self._check_for_wide_format(df)
+        except EtlError as e:
             raise EtlError(e)
         except Exception as e:
             msg = f'Unknown error: {e}'
             logger.error(msg)
             raise e
 
         return True
@@ -1271,14 +1299,30 @@
     df.columns = ['Timestamp', 'Description', 'Value']
 
     # Round timestamp for given time interval
     df['Timestamp'] = pd.to_datetime(
         df['Timestamp'], format='%d/%m/%Y %H:%M')
     df['Timestamp'] = df['Timestamp'].dt.round(f'{freq}min')
 
+    # Get time difference before/after every row
+    interval = int(freq)
+    timeDiff1 = (df['Timestamp'] - df['Timestamp'].shift(1)).dt.seconds/60 # row_n - row_n-1
+    timeDiff1[df['Description'] != df['Description'].shift(1)] = np.nan
+    timeDiff2 = (df['Timestamp'].shift(-1) - df['Timestamp']).dt.seconds/60 # row_n+1 - row_n
+    timeDiff2[df['Description'].shift(-1) != df['Description']] = np.nan
+
+    # Identify gap type 1: two identical rounded timestamp after gap
+    # Identify gap type 2: two identical rounded timestamp before gap
+    timeGap1 = (timeDiff1 == 2*interval) & (timeDiff2 == 0)
+    timeGap2 = (timeDiff1 == 0 )& (timeDiff2 == 2*interval)
+
+    # move timestamp before/after one interval
+    df.loc[timeGap1,'Timestamp'] = df[timeGap1]['Timestamp'] - pd.Timedelta(minutes=interval)
+    df.loc[timeGap2,'Timestamp'] = df[timeGap2]['Timestamp'] + pd.Timedelta(minutes=interval)
+
     # Sort data by timestamp and ignore non-numeric data
     df.sort_values('Timestamp', inplace=True)
     df['Value'] = pd.to_numeric(df['Value'], errors='coerce')
 
     # Make log data into wide format (pivot table)
     df = pd.pivot_table(df, index='Timestamp',
                         columns='Description', values='Value')
```

### Comparing `exergenics-etl-1.1.0/app/exergenics_etl/src/logger.py` & `exergenics-etl-1.2.0/app/exergenics_etl/src/logger.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.1.0/app/exergenics_etl/test/conftest.py` & `exergenics-etl-1.2.0/app/exergenics_etl/test/conftest.py`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.1.0/app/exergenics_etl/test/test_exergenics_etl.py` & `exergenics-etl-1.2.0/app/exergenics_etl/test/test_exergenics_etl.py`

 * *Files 2% similar despite different names*

```diff
@@ -241,21 +241,27 @@
         assert convertable_to_float(string) == expected
 
 
 class TestInputValidationClass:
 
     @pytest.fixture(scope='class')
     def my_wide_format_dataframe(self):
-        filePath = 'app/exergenics_etl/test/testData/wide_data.csv'
+        filePath = 'app/exergenics_etl/test/testData/wideData.csv'
         df = pd.read_csv(filePath)
         return df
 
     @pytest.fixture(scope='class')
-    def my_long_format_dataframe(self):
-        filePath = 'app/exergenics_etl/test/testData/long_data.csv'
+    def my_long_format_dataframe1(self):
+        filePath = 'app/exergenics_etl/test/testData/longData_nameColumnIn2ndColumn.csv'
+        df = pd.read_csv(filePath)
+        return df
+    
+    @pytest.fixture(scope='class')
+    def my_long_format_dataframe2(self):
+        filePath = 'app/exergenics_etl/test/testData/longData_nameColumnIn3rdColumn.csv'
         df = pd.read_csv(filePath)
         return df
 
     @pytest.fixture(scope='class')
     def my_valid_timestamp_headers(self):
         return ['datetime', 'timestamp', 'event', 'timepretty', 'ts']
 
@@ -266,23 +272,26 @@
     @pytest.fixture(scope='class')
     def my_inputValidation_object(self, my_valid_timestamp_headers, my_generic_column_headers):
         """Instantiate an InputValidation object for testing."""
         inputValidation = InputValidation(
             my_valid_timestamp_headers, my_generic_column_headers)
         return inputValidation
 
-    def test_check_for_wide_format1(self, my_inputValidation_object, my_wide_format_dataframe):
+    def test_check_for_wide_format(self, my_inputValidation_object, my_wide_format_dataframe):
         """Check for wide format when a wide format dataframe is passed."""
         assert my_inputValidation_object._check_for_wide_format(
             my_wide_format_dataframe)
 
-    def test_check_for_wide_format2(self, my_inputValidation_object, my_long_format_dataframe):
+    @pytest.mark.parametrize("my_long_format_dataframe", ['my_long_format_dataframe1', 'my_long_format_dataframe2'])
+    def test_check_for_wide_format_on_long_dataframe(self, my_inputValidation_object, my_long_format_dataframe, request):
         """Check for wide format when a long format dataframe is passed."""
-        assert not my_inputValidation_object._check_for_wide_format(
-            my_long_format_dataframe)
+        my_long_format_dataframe = request.getfixturevalue(my_long_format_dataframe)
+        with pytest.raises(EtlError):
+            my_inputValidation_object._check_for_wide_format(
+                my_long_format_dataframe)
 
     def test_check_for_generic_header1(self, my_inputValidation_object):
         myDfSameName = pd.read_csv(
             'app/exergenics_etl/test/testData/dfSameName.csv', parse_dates=['timepretty'])
         myDfNew = pd.read_csv(
             'app/exergenics_etl/test/testData/dfNew.csv', parse_dates=['timepretty'])
         myPointName = 'Ch1-kwr'
```

### Comparing `exergenics-etl-1.1.0/app/exergenics_etl.egg-info/SOURCES.txt` & `exergenics-etl-1.2.0/app/exergenics_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `exergenics-etl-1.1.0/setup.py` & `exergenics-etl-1.2.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 # with open("app/Readme.md", "r") as f:
 #     long_description = f.read()
 
 setup(
     name="exergenics-etl",
-    version="v1.1.0",
+    version="v1.2.0",
     description="Exergenics shared Data ETL functions",
     package_dir={"": "app"},
     packages=find_packages(where="app"),
     long_description="### Exergenics ETL Pytho package",
     long_description_content_type="text/markdown",
     url="",
     author="Nobel Wong",
```

