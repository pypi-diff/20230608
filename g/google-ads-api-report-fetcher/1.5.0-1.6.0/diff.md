# Comparing `tmp/google-ads-api-report-fetcher-1.5.0.tar.gz` & `tmp/google-ads-api-report-fetcher-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-ads-api-report-fetcher-1.5.0.tar", last modified: Mon May 29 10:53:28 2023, max compression
+gzip compressed data, was "google-ads-api-report-fetcher-1.6.0.tar", last modified: Thu Jun  8 13:13:24 2023, max compression
```

## Comparing `google-ads-api-report-fetcher-1.5.0.tar` & `google-ads-api-report-fetcher-1.6.0.tar`

### file list

```diff
@@ -1,48 +1,53 @@
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.5.0/README.md
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.531231 google-ads-api-report-fetcher-1.5.0/gaarf/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.5.0/gaarf/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-04-13 10:50:21.000000 google-ads-api-report-fetcher-1.5.0/gaarf/api_clients.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.5.0/gaarf/base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3744 2023-05-22 11:14:44.000000 google-ads-api-report-fetcher-1.5.0/gaarf/bq_executor.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/gaarf/cli/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4053 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/bq.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     8203 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/gaarf.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3586 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/simulator.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10557 2023-05-18 10:21:29.000000 google-ads-api-report-fetcher-1.5.0/gaarf/cli/utils.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/gaarf/io/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/formatter.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.5.0/gaarf/io/writer.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.5.0/gaarf/parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.5.0/gaarf/query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    11371 2023-05-04 10:22:26.000000 google-ads-api-report-fetcher-1.5.0/gaarf/query_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     5655 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/gaarf/report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.5.0/gaarf/simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.5.0/gaarf/utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.5.0/gaarf/wip.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     4222 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1033 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      184 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/requires.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-05-29 10:53:28.000000 google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/top_level.txt
--rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-05-29 10:53:28.539231 google-ads-api-report-fetcher-1.5.0/setup.cfg
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1679 2023-05-29 10:48:29.000000 google-ads-api-report-fetcher-1.5.0/setup.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/tests/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.5.0/tests/__init__.py
-drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-05-29 10:53:28.535231 google-ads-api-report-fetcher-1.5.0/tests/unit/
--rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/__init__.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_base_query.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     1400 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_bq_executor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)    10945 2023-04-07 06:54:54.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_cli_utils.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_parsers.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_query_editor.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_reader.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     6927 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_report.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_simulation.py
--rw-r-----   0 amarkin  (454256) primarygroup (89939)     3864 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.5.0/tests/unit/test_writer.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3489 2023-03-16 20:20:32.000000 google-ads-api-report-fetcher-1.6.0/README.md
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.347265 google-ads-api-report-fetcher-1.6.0/gaarf/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.6.0/gaarf/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7756 2023-04-13 10:50:21.000000 google-ads-api-report-fetcher-1.6.0/gaarf/api_clients.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      916 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.6.0/gaarf/base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2717 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.6.0/gaarf/bq_executor.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/gaarf/cli/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3188 2023-06-07 14:43:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/bq.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7494 2023-06-07 14:43:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/gaarf.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4210 2023-06-07 13:55:49.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/postprocessor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3586 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/simulator.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3099 2023-06-07 14:43:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/sql.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    13434 2023-06-07 14:43:52.000000 google-ads-api-report-fetcher-1.6.0/gaarf/cli/utils.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/gaarf/io/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1842 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/formatter.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1870 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9991 2023-03-16 19:54:17.000000 google-ads-api-report-fetcher-1.6.0/gaarf/io/writer.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10596 2023-05-29 10:48:19.000000 google-ads-api-report-fetcher-1.6.0/gaarf/parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     9680 2023-03-10 13:35:15.000000 google-ads-api-report-fetcher-1.6.0/gaarf/query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    11597 2023-06-07 20:34:00.000000 google-ads-api-report-fetcher-1.6.0/gaarf/query_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2399 2023-06-06 14:27:05.000000 google-ads-api-report-fetcher-1.6.0/gaarf/query_post_processor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     5655 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.6.0/gaarf/report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4088 2023-03-06 16:43:36.000000 google-ads-api-report-fetcher-1.6.0/gaarf/simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1275 2023-06-07 14:38:11.000000 google-ads-api-report-fetcher-1.6.0/gaarf/sql_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2295 2023-05-16 06:16:06.000000 google-ads-api-report-fetcher-1.6.0/gaarf/utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      158 2023-02-13 15:07:14.000000 google-ads-api-report-fetcher-1.6.0/gaarf/wip.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     4202 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/PKG-INFO
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1169 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        1 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/dependency_links.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      214 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/entry_points.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      192 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/requires.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       12 2023-06-08 13:13:24.000000 google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/top_level.txt
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)       63 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/setup.cfg
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     1723 2023-06-07 14:40:20.000000 google-ads-api-report-fetcher-1.6.0/setup.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/tests/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2022-10-03 10:44:40.000000 google-ads-api-report-fetcher-1.6.0/tests/__init__.py
+drwxr-x---   0 amarkin  (454256) primarygroup (89939)        0 2023-06-08 13:13:24.351265 google-ads-api-report-fetcher-1.6.0/tests/unit/
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)        0 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/__init__.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      748 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_base_query.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      423 2023-06-06 14:22:27.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_bq_executor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)    10945 2023-04-07 06:54:54.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_cli_utils.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     7168 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_parsers.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3890 2023-02-24 15:33:44.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_editor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3982 2023-06-08 13:13:05.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_post_processor.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)      891 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_reader.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     6927 2023-05-29 08:35:12.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_report.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     2487 2023-02-13 15:07:42.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_simulation.py
+-rw-r-----   0 amarkin  (454256) primarygroup (89939)     3882 2023-06-06 14:23:09.000000 google-ads-api-report-fetcher-1.6.0/tests/unit/test_writer.py
```

### Comparing `google-ads-api-report-fetcher-1.5.0/PKG-INFO` & `google-ads-api-report-fetcher-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.5.0
+Version: 1.6.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -121,9 +120,7 @@
     * `PROTOBUF` - convert Google Ads API response to protobuf before parsing
         (speeds up query execution 5x times but forces conversion of ENUMs to integers instead of strings)
     * `BATCH` -  converts all response of Ads API to a list and then parses its content in parallel
     * `BATCH_PROTOBUF` - combines `BATCH` and `PROTOBUF` approaches.
 
 ## Disclaimer
 This is not an officially supported Google product.
-
-
```

### Comparing `google-ads-api-report-fetcher-1.5.0/README.md` & `google-ads-api-report-fetcher-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/api_clients.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/api_clients.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/base_query.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/cli/bq.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/cli/sql.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,101 +1,81 @@
-# Copyright 2022 Google LLC
+# Copyright 2023 Google LLC
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     https://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import sys
 import argparse
 from concurrent import futures
-import logging
-from rich.logging import RichHandler
+import sqlalchemy
 
 from gaarf.io import reader  # type: ignore
-from gaarf.bq_executor import BigQueryExecutor
-from .utils import GaarfBqConfigBuilder, ConfigSaver, initialize_runtime_parameters
+from gaarf.sql_executor import SqlAlchemyQueryExecutor
+from .utils import (GaarfSqlConfigBuilder, ConfigSaver,
+                    initialize_runtime_parameters, postprocessor_runner,
+                    init_logging)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("query", nargs="+")
     parser.add_argument("-c", "--config", dest="gaarf_config", default=None)
-    parser.add_argument("--project", dest="project")
-    parser.add_argument("--dataset-location",
-                        dest="dataset_location",
-                        default=None)
+    parser.add_argument("--conn",
+                        "--connection-string",
+                        dest="connection_string")
     parser.add_argument("--save-config",
                         dest="save_config",
                         action="store_true")
     parser.add_argument("--no-save-config",
                         dest="save_config",
                         action="store_false")
     parser.add_argument("--config-destination",
                         dest="save_config_dest",
                         default="config.yaml")
     parser.add_argument("--log", "--loglevel", dest="loglevel", default="info")
     parser.add_argument("--logger", dest="logger", default="local")
-    parser.add_argument("--dry-run",
-                        dest="dry_run",
-                        action="store_true")
+    parser.add_argument("--dry-run", dest="dry_run", action="store_true")
     parser.set_defaults(save_config=False)
     parser.set_defaults(dry_run=False)
     args = parser.parse_known_args()
     main_args = args[0]
 
-    if main_args.logger == "rich":
-        logging.basicConfig(format="%(message)s",
-                            level=main_args.loglevel.upper(),
-                            datefmt="%Y-%m-%d %H:%M:%S",
-                            handlers=[RichHandler(rich_tracebacks=True)])
-    else:
-        logging.basicConfig(
-                    format="[%(asctime)s][%(name)s][%(levelname)s] %(message)s",
-                    stream=sys.stdout,
-                    level=main_args.loglevel.upper(),
-                    datefmt="%Y-%m-%d %H:%M:%S")
-    logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
-    logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
-    logger = logging.getLogger(__name__)
+    logger = init_logging(loglevel=main_args.loglevel.upper(),
+                          logger_type=main_args.logger)
 
-    config = GaarfBqConfigBuilder(args).build()
+    config = GaarfSqlConfigBuilder(args).build()
     logger.debug("config: %s", config)
     if main_args.save_config and not main_args.gaarf_config:
         ConfigSaver(main_args.save_config_dest).save(config)
     if main_args.dry_run:
         exit()
 
     config = initialize_runtime_parameters(config)
     logger.debug("initialized config: %s", config)
 
-    bq_executor = BigQueryExecutor(project_id=config.project,
-                                   location=config.dataset_location)
-    bq_executor.create_datasets(config.params.get("macro"))
+    engine = sqlalchemy.create_engine(config.connection_string)
+    sql_executor = SqlAlchemyQueryExecutor(engine)
 
     reader_client = reader.FileReader()
 
     with futures.ThreadPoolExecutor() as executor:
         future_to_query = {
-            executor.submit(bq_executor.execute, query,
-                            reader_client.read(query), config.params): query
+            executor.submit(sql_executor.execute, query,
+                            reader_client.read(query), config.params):
+            query
             for query in main_args.query
         }
         for future in futures.as_completed(future_to_query):
             query = future_to_query[future]
-            try:
-                logger.debug("starting query %s", query)
-                future.result()
-                logger.info("%s executed successfully", query)
-            except Exception as e:
-                logger.error("%s generated an exception: %s", query, str(e))
+            postprocessor_runner(query, future.result, logger)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/cli/gaarf.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/cli/gaarf.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,16 @@
 import logging
 from rich.logging import RichHandler
 from smart_open import open
 import yaml
 
 from gaarf import api_clients, utils, query_executor
 from gaarf.io import writer, reader  # type: ignore
-from .utils import GaarfConfigBuilder, ConfigSaver, initialize_runtime_parameters, gaarf_runner
+from .utils import (GaarfConfigBuilder, ConfigSaver,
+                    initialize_runtime_parameters, gaarf_runner, init_logging)
 
 
 def main():
     parser = argparse.ArgumentParser()
     parser.add_argument("query", nargs="*")
     parser.add_argument("-c", "--config", dest="gaarf_config", default=None)
     parser.add_argument("--account", dest="customer_id", default=None)
@@ -78,30 +79,16 @@
     if main_args.version:
         import pkg_resources
         version = pkg_resources.require(
             "google-ads-api-report-fetcher")[0].version
         print(f"gaarf version {version}")
         exit()
 
-    if main_args.logger == "rich":
-        logging.basicConfig(format="%(message)s",
-                            level=main_args.loglevel.upper(),
-                            datefmt="%Y-%m-%d %H:%M:%S",
-                            handlers=[RichHandler(rich_tracebacks=True)])
-    else:
-        logging.basicConfig(
-                    format="[%(asctime)s][%(name)s][%(levelname)s] %(message)s",
-                    stream=sys.stdout,
-                    level=main_args.loglevel.upper(),
-                    datefmt="%Y-%m-%d %H:%M:%S")
-    logging.getLogger("google.ads.googleads.client").setLevel(logging.WARNING)
-    logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
-    logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
-    logger = logging.getLogger(__name__)
-
+    logger = init_logging(loglevel=main_args.loglevel.upper(),
+                          logger_type=main_args.logger)
     if not main_args.query:
         logger.error("Please provide one or more queries to run")
         exit()
 
     with open(main_args.config, "r", encoding="utf-8") as f:
         google_ads_config_dict = yaml.safe_load(f)
 
@@ -159,17 +146,16 @@
                     len(customer_ids), ",".join(map(str, customer_ids)))
 
         if main_args.parallel_queries:
             logger.info("Running queries in parallel")
             with futures.ThreadPoolExecutor() as executor:
                 future_to_query = {
                     executor.submit(ads_query_executor.execute,
-                                    reader_client.read(query), query,
-                                    customer_ids, writer_client, config.params,
-                                    main_args.optimize_performance): query
+                                    reader_client.read(query), query, customer_ids, writer_client, config.params, main_args.optimize_performance):
+                    query
                     for query in main_args.query
                 }
                 for future in futures.as_completed(future_to_query):
                     query = future_to_query[future]
                     gaarf_runner(query, future.result, logger)
         else:
             logger.info("Running queries sequentially")
```

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/cli/simulator.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/cli/utils.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/cli/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,15 +11,18 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from typing import Any, Callable, Dict, List, Optional, Sequence, Union
 from collections.abc import MutableSequence
 from dataclasses import dataclass, field, asdict
+import logging
+from rich.logging import RichHandler
 import os
+import sys
 import datetime
 from smart_open import open
 from dateutil.relativedelta import relativedelta
 import yaml
 from google.ads.googleads.errors import GoogleAdsException  # type: ignore
 import traceback
 
@@ -33,21 +36,39 @@
     account: str
     params: Dict[str, Any] = field(default_factory=dict)
     writer_params: Dict[str, Any] = field(default_factory=dict)
     customer_ids_query: Optional[str] = None
     customer_ids_query_file: Optional[str] = None
 
 
+class GaarfConfigException(Exception):
+    ...
+
+
 @dataclass
 class GaarfBqConfig:
     project: str
     dataset_location: Optional[str]
     params: Dict[str, Any] = field(default_factory=dict)
 
 
+class GaarfBqConfigException(Exception):
+    ...
+
+
+@dataclass
+class GaarfSqlConfig:
+    connection_string: str
+    params: Dict[str, Any] = field(default_factory=dict)
+
+
+class GaarfSqlConfigException(Exception):
+    ...
+
+
 class BaseConfigBuilder:
 
     def __init__(self, args):
         self.args = args
         if (gaarf_config_path := self.args[0].gaarf_config):
             self.type = "file"
             self.gaarf_config_path = gaarf_config_path
@@ -73,15 +94,16 @@
         super().__init__(args)
 
     def _load_gaarf_config(self) -> GaarfConfig:
         with open(self.gaarf_config_path, encoding="utf-8") as f:
             config = yaml.safe_load(f)
         gaarf_section = config.get("gaarf")
         if not gaarf_section:
-            raise ValueError("Invalid config, must have `gaarf` section!")
+            raise GaarfConfigException(
+                "Invalid config, must have `gaarf` section!")
         if not (output := gaarf_section.get("output")):
             raise ValueError("Config does not contains `output` section!")
         return GaarfConfig(
             output=gaarf_section.get("output"),
             api_version=gaarf_section.get("api_version"),
             account=gaarf_section.get("account"),
             params=gaarf_section.get("params"),
@@ -109,24 +131,56 @@
         super().__init__(args)
 
     def _load_gaarf_config(self) -> GaarfBqConfig:
         with open(self.gaarf_config_path, encoding="utf-8") as f:
             config = yaml.safe_load(f)
         gaarf_section = config.get("gaarf-bq")
         if not gaarf_section:
-            raise ValueError("Invalid config, must have `gaarf-bq` section!")
+            raise GaarfBqConfigException(
+                "Invalid config, must have `gaarf-bq` section!")
         params = gaarf_section.get("params")
-        return GaarfBqConfig(project=gaarf_section.get("project"),
-                             dataset_location=gaarf_section.get("dataset_location"),
-                             params=params)
+        return GaarfBqConfig(
+            project=gaarf_section.get("project"),
+            dataset_location=gaarf_section.get("dataset_location"),
+            params=params)
 
     def _build_gaarf_config(self) -> GaarfBqConfig:
         main_args, query_args = self.args[0], self.args[1]
         params = ParamsParser(["macro", "sql", "template"]).parse(query_args)
-        return GaarfBqConfig(project=main_args.project, dataset_location=main_args.dataset_location, params=params)
+        return GaarfBqConfig(project=main_args.project,
+                             dataset_location=main_args.dataset_location,
+                             params=params)
+
+
+class GaarfSqlConfigBuilder(BaseConfigBuilder):
+
+    def __init__(self, args):
+        import sqlalchemy
+        super().__init__(args)
+
+    def _load_gaarf_config(self) -> GaarfBqConfig:
+        with open(self.gaarf_config_path, encoding="utf-8") as f:
+            config = yaml.safe_load(f)
+        gaarf_section = config.get("gaarf-sql")
+        if not gaarf_section:
+            raise GaarfSqlConfigException(
+                "Invalid config, must have `gaarf-sql` section!")
+        params = gaarf_section.get("params")
+        return GaarfSqlConfig(
+            connection_string=gaarf_section.get("connection-string").format(
+                **dict(os.environ.items())),
+            params=params)
+
+    def _build_gaarf_config(self) -> GaarfSqlConfig:
+        main_args, query_args = self.args[0], self.args[1]
+        params = ParamsParser(["macro", "sql", "template"]).parse(query_args)
+        return GaarfSqlConfig(
+            connection_string=main_args.connection_string.format(
+                **dict(os.environ.items())),
+            params=params)
 
 
 class ParamsParser:
 
     common_params = {"date_iso": datetime.date.today().strftime("%Y%m%d")}
 
     def __init__(self, identifiers: Sequence[str]):
@@ -155,32 +209,31 @@
         key = param[0]
         if identifier not in key:
             return None
         provided_identifier, key = key.split(".")
         if provided_identifier.replace("--", "") not in self.identifiers:
             raise GaarfParamsException(
                 f"CLI argument {provided_identifier} is not supported"
-                f", supported arguments {', '.join(self.identifiers)}"
-            )
+                f", supported arguments {', '.join(self.identifiers)}")
         key = key.replace("-", "_")
         if len(param) == 2:
             return {key: param[1]}
         raise GaarfParamsException(
             f"{identifier} {key} is invalid,"
             f"--{identifier}.key=value is the correct format")
 
 
 class GaarfParamsException(Exception):
-    pass
+    ...
 
 
 def convert_date(date_string: str) -> str:
     """Converts specific dates parameters to actual dates."""
 
-    if date_string.find(":YYYY") == -1:
+    if isinstance(date_string, list) or date_string.find(":YYYY") == -1:
         return date_string
     current_date = datetime.date.today()
     date_object = date_string.split("-")
     base_date = date_object[0]
     if len(date_object) == 2:
         try:
             days_ago = int(date_object[1])
@@ -217,29 +270,34 @@
         with open(self.path, "w", encoding="utf-8") as f:
             yaml.dump(config,
                       f,
                       default_flow_style=False,
                       sort_keys=False,
                       encoding="utf-8")
 
-    def prepare_config(self, config: Dict[Any, Any],
-                       gaarf_config: Union[GaarfConfig, GaarfBqConfig]):
+    def prepare_config(
+        self, config: Dict[Any, Any],
+        gaarf_config: Union[GaarfConfig, GaarfBqConfig, GaarfSqlConfig]
+    ) -> Dict[str, Any]:
         gaarf = asdict(gaarf_config)
         if isinstance(gaarf_config, GaarfConfig):
             gaarf[gaarf_config.output] = gaarf_config.writer_params
             if not isinstance(gaarf_config.account, MutableSequence):
                 gaarf["account"] = gaarf_config.account.split(",")
             del gaarf["writer_params"]
             if gaarf_config.writer_params:
                 del gaarf["params"][gaarf_config.output]
             gaarf = _remove_empty_values(gaarf)
             config.update({"gaarf": gaarf})
         if isinstance(gaarf_config, GaarfBqConfig):
             gaarf = _remove_empty_values(gaarf)
             config.update({"gaarf-bq": gaarf})
+        if isinstance(gaarf_config, GaarfSqlConfig):
+            gaarf = _remove_empty_values(gaarf)
+            config.update({"gaarf-sql": gaarf})
         return config
 
 
 def initialize_runtime_parameters(config: Union[GaarfConfig, GaarfBqConfig]):
     for key, param in config.params.items():
         for key_param, value_param in param.items():
             config.params[key][key_param] = convert_date(value_param)
@@ -275,7 +333,36 @@
             logger.error("\tError with message %s .", error.message)
             if error.location:
                 for field in error.location.field_path_elements:
                     logger.error("\t\tOn field %s", field.field_name)
     except Exception as e:
         traceback.print_tb(e.__traceback__)
         logger.error("%s generated an exception: %s", query, str(e))
+
+
+def postprocessor_runner(query: str, callback: Callable, logger) -> None:
+    try:
+        logger.debug("starting query %s", query)
+        callback()
+        logger.info("%s executed successfully", query)
+    except Exception as e:
+        logger.error("%s generated an exception: %s", query, str(e))
+
+
+def init_logging(loglevel: str = "INFO",
+                 logger_type: str = "local",
+                 name: str = __name__) -> logging.Logger:
+    if logger_type == "rich":
+        logging.basicConfig(format="%(message)s",
+                            level=loglevel,
+                            datefmt="%Y-%m-%d %H:%M:%S",
+                            handlers=[RichHandler(rich_tracebacks=True)])
+    else:
+        logging.basicConfig(
+            format="[%(asctime)s][%(name)s][%(levelname)s] %(message)s",
+            stream=sys.stdout,
+            level=loglevel,
+            datefmt="%Y-%m-%d %H:%M:%S")
+    logging.getLogger("google.ads.googleads.client").setLevel(logging.WARNING)
+    logging.getLogger("smart_open.smart_open_lib").setLevel(logging.WARNING)
+    logging.getLogger("urllib3.connectionpool").setLevel(logging.WARNING)
+    return logging.getLogger(name)
```

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/io/formatter.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/io/formatter.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/io/reader.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/io/reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/io/writer.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/io/writer.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/parsers.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/query_editor.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/query_executor.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/query_executor.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,17 @@
 
 
 class AdsReportFetcher:
     """Class responsible for getting data from Ads API.
 
     Attributes:
         api_client: a client used for connecting to Ads API.
-        customer_ids: account_id(s) from which data will be fetches.
+        customer_ids: account_id(s) from which data will be fetched.
+          Expects list of non-MCC accounts, which can be expanded from MCC
+          by calling `utils.get_customer_ids(ads_api_client, mcc_id)` function.
     """
 
     def __init__(self, api_client: api_clients.BaseClient,
                  customer_ids: Union[Sequence[str], str]) -> None:
 
         self.api_client = api_client
         self.customer_ids = [
@@ -86,14 +88,15 @@
                 if query_specification.is_constant_resource:
                     logger.debug("Constant resource query: running only once")
                     break
             except GoogleAdsException as e:
                 logger.error("Cannot execute query %s for %s",
                              query_specification.query_title, customer_id)
                 logger.error(str(e))
+                raise
         if not total_results:
             row = self.api_client.google_ads_row
             results = [parser.parse_ads_row(row)]
             total_results.extend(results)
             is_fake_report = True
             logger.warning(
                 "Query %s generated zero results, using placeholders to infer schema",
@@ -135,14 +138,15 @@
                     response = self.api_client.get_response(
                         entity_id=str(customer_id),
                         query_text=query_specification.query_text)
         except RetryError as retry_failure:
             logger.error("Cannot fetch data from API for query '%s' %d times",
                          query_specification.query_title,
                          retry_failure.last_attempt.attempt_number)
+            raise exceptions.InternalServerError
         if optimize_strategy in (OptimizeStrategy.BATCH,
                                  OptimizeStrategy.BATCH_PROTOBUF):
             logger.warning("Running gaarf in an optimized mode")
             logger.warning("Optimize strategy is %s", optimize_strategy.name)
             if optimize_strategy == OptimizeStrategy.BATCH_PROTOBUF:
                 rows = [row._pb for batch in response for row in batch.results]
             else:
```

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/report.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/report.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/simulation.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/gaarf/utils.py` & `google-ads-api-report-fetcher-1.6.0/gaarf/utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/PKG-INFO` & `google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: google-ads-api-report-fetcher
-Version: 1.5.0
+Version: 1.6.0
 Summary: Library for fetching reports from Google Ads API and saving them locally / BigQuery.
 Home-page: https://github.com/google/ads-api-reports-fetcher
 Author: Google Inc. (gTech gPS CSE team)
 Author-email: no-reply@google.com
 License: Apache 2.0
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Operating System :: OS Independent
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
 Provides-Extra: full
@@ -121,9 +120,7 @@
     * `PROTOBUF` - convert Google Ads API response to protobuf before parsing
         (speeds up query execution 5x times but forces conversion of ENUMs to integers instead of strings)
     * `BATCH` -  converts all response of Ads API to a list and then parses its content in parallel
     * `BATCH_PROTOBUF` - combines `BATCH` and `PROTOBUF` approaches.
 
 ## Disclaimer
 This is not an officially supported Google product.
-
-
```

### Comparing `google-ads-api-report-fetcher-1.5.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt` & `google-ads-api-report-fetcher-1.6.0/google_ads_api_report_fetcher.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 gaarf/__init__.py
 gaarf/api_clients.py
 gaarf/base_query.py
 gaarf/bq_executor.py
 gaarf/parsers.py
 gaarf/query_editor.py
 gaarf/query_executor.py
+gaarf/query_post_processor.py
 gaarf/report.py
 gaarf/simulation.py
+gaarf/sql_executor.py
 gaarf/utils.py
 gaarf/wip.py
 gaarf/cli/__init__.py
 gaarf/cli/bq.py
 gaarf/cli/gaarf.py
+gaarf/cli/postprocessor.py
 gaarf/cli/simulator.py
+gaarf/cli/sql.py
 gaarf/cli/utils.py
 gaarf/io/__init__.py
 gaarf/io/formatter.py
 gaarf/io/reader.py
 gaarf/io/writer.py
 google_ads_api_report_fetcher.egg-info/PKG-INFO
 google_ads_api_report_fetcher.egg-info/SOURCES.txt
@@ -30,11 +34,12 @@
 tests/__init__.py
 tests/unit/__init__.py
 tests/unit/test_base_query.py
 tests/unit/test_bq_executor.py
 tests/unit/test_cli_utils.py
 tests/unit/test_parsers.py
 tests/unit/test_query_editor.py
+tests/unit/test_query_post_processor.py
 tests/unit/test_reader.py
 tests/unit/test_report.py
 tests/unit/test_simulation.py
 tests/unit/test_writer.py
```

### Comparing `google-ads-api-report-fetcher-1.5.0/setup.py` & `google-ads-api-report-fetcher-1.6.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     "sqlalchemy": ["sqlalchemy"],
     "simulator": ["Faker"]
 }
 EXTRAS_REQUIRE['full'] = list(set(chain(*EXTRAS_REQUIRE.values())))
 
 setup(
     name="google-ads-api-report-fetcher",
-    version="1.5.0",
+    version="1.6.0",
     description=
     "Library for fetching reports from Google Ads API and saving them locally / BigQuery.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/google/ads-api-reports-fetcher",
     author="Google Inc. (gTech gPS CSE team)",
     author_email="no-reply@google.com",
@@ -42,9 +42,10 @@
     entry_points={
         "console_scripts": [
             "gaarf=gaarf.cli.gaarf:main",
             "gaarf-py=gaarf.cli.gaarf:main",
             "gaarf-bq=gaarf.cli.bq:main",
             "gaarf-py-bq=gaarf.cli.bq:main",
             "gaarf-simulator=gaarf.cli.simulator:main",
+            "gaarf-sql=gaarf.cli.sql:main",
         ]
     })
```

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_base_query.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_base_query.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_cli_utils.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_parsers.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_parsers.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_query_editor.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_query_editor.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_reader.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_reader.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_report.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_report.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_simulation.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_simulation.py`

 * *Files identical despite different names*

### Comparing `google-ads-api-report-fetcher-1.5.0/tests/unit/test_writer.py` & `google-ads-api-report-fetcher-1.6.0/tests/unit/test_writer.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,17 +65,17 @@
     }
 
 
 def test_bq_get_correct_schema(bq_writer, sample_data):
     results, columns = sample_data.results, sample_data.column_names
     schema = bq_writer._define_schema(results, columns)
     assert schema == [
-        SchemaField('column_1', 'INT64', 'NULLABLE', None, (), None),
-        SchemaField('column_2', 'STRING', 'NULLABLE', None, (), None),
-        SchemaField('column_3', 'INT64', 'REPEATED', None, (), None)
+        SchemaField('column_1', 'INT64', 'NULLABLE', None, None, (), None),
+        SchemaField('column_2', 'STRING', 'NULLABLE', None, None, (), None),
+        SchemaField('column_3', 'INT64', 'REPEATED', None, None, (), None)
     ]
 
 
 def test_format_extension():
     default_output = writer.DestinationFormatter.format_extension(
         "test_query.sql")
     default_output_custom_extension = writer.DestinationFormatter.format_extension(
```

