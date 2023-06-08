# Comparing `tmp/iterable_etl-0.0.1rc2.tar.gz` & `tmp/iterable_etl-0.0.1rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iterable_etl-0.0.1rc2.tar", last modified: Wed Jun  7 19:28:42 2023, max compression
+gzip compressed data, was "iterable_etl-0.0.1rc3.tar", last modified: Thu Jun  8 18:42:45 2023, max compression
```

## Comparing `iterable_etl-0.0.1rc2.tar` & `iterable_etl-0.0.1rc3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.0.1rc2/MANIFEST.in
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1654 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1143 2023-06-07 19:27:23.000000 iterable_etl-0.0.1rc2/README_PUBLIC.md
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 iterable_etl-0.0.1rc2/iterable_etl/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-07 15:07:58.000000 iterable_etl-0.0.1rc2/iterable_etl/__main__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      833 2023-06-07 17:20:53.000000 iterable_etl-0.0.1rc2/iterable_etl/iterable_etl.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl/libs/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      516 2023-06-07 15:37:52.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/cnst.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/dbg.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      524 2023-06-07 19:21:02.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/network.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      636 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/spark.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      463 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/libs/transform.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl/tables/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/__init__.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      779 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1310 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_list_history.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1615 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_metrics.py
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      705 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc2/iterable_etl/tables/list.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/iterable_etl.egg-info/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1654 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/PKG-INFO
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      666 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/SOURCES.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/dependency_links.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       48 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/requires.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-07 19:28:42.000000 iterable_etl-0.0.1rc2/iterable_etl.egg-info/top_level.txt
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/setup.cfg
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      957 2023-06-07 19:27:52.000000 iterable_etl-0.0.1rc2/setup.py
-drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-07 19:28:42.312789 iterable_etl-0.0.1rc2/tests/
--rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.0.1rc2/tests/__init__.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:42:45.882534 iterable_etl-0.0.1rc3/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      307 2023-06-07 17:51:32.000000 iterable_etl-0.0.1rc3/MANIFEST.in
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1769 2023-06-08 18:42:45.882534 iterable_etl-0.0.1rc3/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1258 2023-06-07 21:56:06.000000 iterable_etl-0.0.1rc3/README_PUBLIC.md
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:42:45.878534 iterable_etl-0.0.1rc3/iterable_etl/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-02 15:40:55.000000 iterable_etl-0.0.1rc3/iterable_etl/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      154 2023-06-07 15:07:58.000000 iterable_etl-0.0.1rc3/iterable_etl/__main__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      833 2023-06-07 17:20:53.000000 iterable_etl-0.0.1rc3/iterable_etl/iterable_etl.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:42:45.878534 iterable_etl-0.0.1rc3/iterable_etl/libs/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:36:56.000000 iterable_etl-0.0.1rc3/iterable_etl/libs/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      516 2023-06-07 15:37:52.000000 iterable_etl-0.0.1rc3/iterable_etl/libs/cnst.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1629 2023-06-07 19:19:44.000000 iterable_etl-0.0.1rc3/iterable_etl/libs/dbg.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      524 2023-06-07 19:21:02.000000 iterable_etl-0.0.1rc3/iterable_etl/libs/network.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      636 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc3/iterable_etl/libs/spark.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      463 2023-06-07 19:11:13.000000 iterable_etl-0.0.1rc3/iterable_etl/libs/transform.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:42:45.878534 iterable_etl-0.0.1rc3/iterable_etl/tables/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-06 22:37:03.000000 iterable_etl-0.0.1rc3/iterable_etl/tables/__init__.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      832 2023-06-08 17:58:59.000000 iterable_etl-0.0.1rc3/iterable_etl/tables/campaign_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1359 2023-06-08 17:59:20.000000 iterable_etl-0.0.1rc3/iterable_etl/tables/campaign_list_history.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1668 2023-06-08 17:59:33.000000 iterable_etl-0.0.1rc3/iterable_etl/tables/campaign_metrics.py
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      758 2023-06-08 17:59:58.000000 iterable_etl-0.0.1rc3/iterable_etl/tables/list.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:42:45.878534 iterable_etl-0.0.1rc3/iterable_etl.egg-info/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)     1769 2023-06-08 18:42:45.000000 iterable_etl-0.0.1rc3/iterable_etl.egg-info/PKG-INFO
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      666 2023-06-08 18:42:45.000000 iterable_etl-0.0.1rc3/iterable_etl.egg-info/SOURCES.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        1 2023-06-08 18:42:45.000000 iterable_etl-0.0.1rc3/iterable_etl.egg-info/dependency_links.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       55 2023-06-08 18:42:45.000000 iterable_etl-0.0.1rc3/iterable_etl.egg-info/requires.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       13 2023-06-08 18:42:45.000000 iterable_etl-0.0.1rc3/iterable_etl.egg-info/top_level.txt
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)       38 2023-06-08 18:42:45.882534 iterable_etl-0.0.1rc3/setup.cfg
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)      967 2023-06-08 18:42:25.000000 iterable_etl-0.0.1rc3/setup.py
+drwxrwxr-x   0 agmoss    (1000) agmoss    (1000)        0 2023-06-08 18:42:45.882534 iterable_etl-0.0.1rc3/tests/
+-rw-rw-r--   0 agmoss    (1000) agmoss    (1000)        0 2023-06-05 15:58:16.000000 iterable_etl-0.0.1rc3/tests/__init__.py
```

### Comparing `iterable_etl-0.0.1rc2/PKG-INFO` & `iterable_etl-0.0.1rc3/iterable_etl.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iterable_etl
-Version: 0.0.1rc2
+Name: iterable-etl
+Version: 0.0.1rc3
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,16 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # `iterable_etl`
 
 > Replicate data from iterable in databricks
 
+[![pypi](https://img.shields.io/pypi/v/iterable_etl?style=for-the-badge)](https://pypi.org/project/iterable_etl/)
+
 ### CLI
 
 ```bash
 python -m iterable_etl --table <table-name>
 ```
 
 where <table-name> is one of the following: `campaign_history`, `campaign_metrics`, `campaign_list_history`, `list`, or `ALL`.
```

### Comparing `iterable_etl-0.0.1rc2/README_PUBLIC.md` & `iterable_etl-0.0.1rc3/README_PUBLIC.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # `iterable_etl`
 
 > Replicate data from iterable in databricks
 
+[![pypi](https://img.shields.io/pypi/v/iterable_etl?style=for-the-badge)](https://pypi.org/project/iterable_etl/)
+
 ### CLI
 
 ```bash
 python -m iterable_etl --table <table-name>
 ```
 
 where <table-name> is one of the following: `campaign_history`, `campaign_metrics`, `campaign_list_history`, `list`, or `ALL`.
```

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/iterable_etl.py` & `iterable_etl-0.0.1rc3/iterable_etl/iterable_etl.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/libs/cnst.py` & `iterable_etl-0.0.1rc3/iterable_etl/libs/cnst.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/libs/dbg.py` & `iterable_etl-0.0.1rc3/iterable_etl/libs/dbg.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/libs/network.py` & `iterable_etl-0.0.1rc3/iterable_etl/libs/network.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/libs/spark.py` & `iterable_etl-0.0.1rc3/iterable_etl/libs/spark.py`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_history.py` & `iterable_etl-0.0.1rc3/iterable_etl/tables/campaign_history.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """campaign_history_meta"""
 
+from pandas import DataFrame as PandasDF
 from typing import Dict, Any
 
 from iterable_etl.libs.network import get_data
 from iterable_etl.libs.transform import json_to_dataframe
 from iterable_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from iterable_etl.libs.cnst import urls, get_headers
 
@@ -12,12 +13,12 @@
     """Make a GET request to the Iterable API and return a dictionary of campaigns data."""
     data = get_data(api_url, headers)
     return data["campaigns"]
 
 
 @write_dataframe_to_csv("campaign_history")
 @print_dataframe_head
-def campaign_history_df():
+def campaign_history_df() -> PandasDF:
     """campaign_history_dataframe"""
     data = get_campaign_data(urls["campaigns"], get_headers())
     df = json_to_dataframe(data)
     return df
```

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_list_history.py` & `iterable_etl-0.0.1rc3/iterable_etl/tables/campaign_list_history.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 """campaign_list_history"""
 
 from typing import Dict, Any, List
 import pandas as pd
+from pandas import DataFrame as PandasDF
 
 from iterable_etl.libs.network import get_data
 from iterable_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from iterable_etl.libs.cnst import urls, get_headers
 
 
 def get_campaign_data(api_url: str, headers: Dict[str, str]) -> List[Dict[str, Any]]:
     """Make a GET request to the Iterable API and return a dictionary of campaigns data."""
     data = get_data(api_url, headers)
     return data["campaigns"]
 
 
-def explode_list_ids(data: List[Dict[str, Any]]) -> pd.DataFrame:
+def explode_list_ids(data: List[Dict[str, Any]]) -> PandasDF:
     """flatten listIds and associate with campaignId"""
     df_data = []
     for campaign in data:
         if "listIds" in campaign:
             for list_id in campaign["listIds"]:
                 df_data.append(
                     {
@@ -31,13 +32,13 @@
     df = pd.DataFrame(df_data)
 
     return df
 
 
 @write_dataframe_to_csv("campaign_list_history")
 @print_dataframe_head
-def campaign_list_history_df():
+def campaign_list_history_df() -> PandasDF:
     """campaign_history_dataframe"""
     data = get_campaign_data(urls["campaigns"], get_headers())
     df = explode_list_ids(data)
 
     return df
```

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/tables/campaign_metrics.py` & `iterable_etl-0.0.1rc3/iterable_etl/tables/campaign_metrics.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """campaign_metrics"""
 import time
 import os
 from typing import Dict
 import requests
 import pandas as pd
+from pandas import DataFrame as PandasDF
 
 from iterable_etl.libs.network import get_data
 from iterable_etl.libs.transform import csv_to_dataframe
 from iterable_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from iterable_etl.libs.cnst import urls, get_headers
 
 
@@ -27,15 +28,15 @@
     response = requests.get(api_url.format(campaign_id), headers=headers, timeout=10)
     response.raise_for_status()
     return response.content
 
 
 @write_dataframe_to_csv("campaign_metrics")
 @print_dataframe_head
-def campaign_metrics_df():
+def campaign_metrics_df() -> PandasDF:
     """campaign_metrics dataframe"""
     campaign_ids = get_campaign_ids(urls["campaigns"], get_headers())
     df_list = []
     for i, campaign_id in enumerate(campaign_ids):
         data = get_metrics_data(urls["metrics"], get_headers(), campaign_id)
         df = csv_to_dataframe(data)
         df_list.append(df)
```

### Comparing `iterable_etl-0.0.1rc2/iterable_etl/tables/list.py` & `iterable_etl-0.0.1rc3/iterable_etl/tables/list.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """list"""
 
+from pandas import DataFrame as PandasDF
 from typing import Dict, Any
 
 from iterable_etl.libs.network import get_data
 from iterable_etl.libs.transform import json_to_dataframe
 from iterable_etl.libs.dbg import print_dataframe_head, write_dataframe_to_csv
 from iterable_etl.libs.cnst import urls, get_headers
 
@@ -12,12 +13,12 @@
     """Make a GET request to the Iterable API and return a dictionary of list data."""
     data = get_data(api_url, headers)
     return data["lists"]
 
 
 @write_dataframe_to_csv("list")
 @print_dataframe_head
-def list_df():
+def list_df() -> PandasDF:
     """list dataframe"""
     data = get_list_data(urls["lists"], get_headers())
     df = json_to_dataframe(data)
     return df
```

### Comparing `iterable_etl-0.0.1rc2/iterable_etl.egg-info/PKG-INFO` & `iterable_etl-0.0.1rc3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: iterable-etl
-Version: 0.0.1rc2
+Name: iterable_etl
+Version: 0.0.1rc3
 Summary: Replicate iterable data in databricks
 Home-page: https://github.com/neofinancial/iterable_etl
 Author: Neo Financial
 Author-email: engineering@neofinancial.com
 License: UNLICENSED
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -14,14 +14,16 @@
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # `iterable_etl`
 
 > Replicate data from iterable in databricks
 
+[![pypi](https://img.shields.io/pypi/v/iterable_etl?style=for-the-badge)](https://pypi.org/project/iterable_etl/)
+
 ### CLI
 
 ```bash
 python -m iterable_etl --table <table-name>
 ```
 
 where <table-name> is one of the following: `campaign_history`, `campaign_metrics`, `campaign_list_history`, `list`, or `ALL`.
```

### Comparing `iterable_etl-0.0.1rc2/iterable_etl.egg-info/SOURCES.txt` & `iterable_etl-0.0.1rc3/iterable_etl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `iterable_etl-0.0.1rc2/setup.py` & `iterable_etl-0.0.1rc3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,24 +6,24 @@
     long_description = fh.read()
 
 setup(
     author="Neo Financial",
     author_email="engineering@neofinancial.com",
     python_requires=">=3.6",
     name="iterable_etl",
-    version="0.0.1rc2",
+    version="0.0.1rc3",
     description="Replicate iterable data in databricks",
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Programming Language :: Python :: 3",
     ],
     license="UNLICENSED",
     packages=find_packages(include=["iterable_etl", "iterable_etl.*"]),
     url="https://github.com/neofinancial/iterable_etl",
     include_package_data=True,
     long_description=long_description,
     long_description_content_type="text/markdown",
-    install_requires=["click", "pandas", "requests", "pyspark", "typing_extensions"],
+    install_requires=["click", "pandas", "requests", "pyspark", "loguru", "typing_extensions"],
     tests_require=["pytest"],
 )
```

