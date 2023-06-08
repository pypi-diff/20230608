# Comparing `tmp/finqual-0.1.6.tar.gz` & `tmp/finqual-0.1.7.tar.gz`

## Comparing `finqual-0.1.6.tar` & `finqual-0.1.7.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.6/finqual/__init__.py
--rw-r--r--   0        0        0   118885 2020-02-02 00:00:00.000000 finqual-0.1.6/finqual/finqual.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.6/LICENSE.txt
--rw-r--r--   0        0        0     1612 2020-02-02 00:00:00.000000 finqual-0.1.6/README.md
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 finqual-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     2089 2020-02-02 00:00:00.000000 finqual-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 finqual-0.1.7/finqual/__init__.py
+-rw-r--r--   0        0        0   118812 2020-02-02 00:00:00.000000 finqual-0.1.7/finqual/finqual.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 finqual-0.1.7/LICENSE.txt
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 finqual-0.1.7/README.md
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 finqual-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     2409 2020-02-02 00:00:00.000000 finqual-0.1.7/PKG-INFO
```

### Comparing `finqual-0.1.6/finqual/finqual.py` & `finqual-0.1.7/finqual/finqual.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Import packages
 import pandas as pd
 import numpy as np
 import requests
-import json
-import datetime as dt
 import ratelimit
-from ratelimit import sleep_and_retry
 
 # Node class and respective functions
 """
 Tree class
 """
 
 class Node():
@@ -2106,8 +2103,8 @@
 cce9_4 = Node("PaymentsForCapitalImprovements", attribute="credit", parent=cce8_1)
 cce9_5 = Node("PaymentsToAcquireResidentialRealEstate", attribute="credit", parent=cce8_1)
 cce9_6 = Node("PaymentsToAcquireLand", attribute="credit", parent=cce8_1)
 cce9_7 = Node("PaymentsToAcquireLandHeldForUse", attribute="credit", parent=cce8_1)
 cce9_8 = Node("PaymentsToAcquireHeldForSaleRealEstate", attribute="credit", parent=cce8_1)
 cce9_9 = Node("PaymentsToAcquireOtherRealEstate", attribute="credit", parent=cce8_1)
 
-cce9_10 = Node("", attribute="credit", parent=cce8_1)
+cce9_10 = Node("", attribute="credit", parent=cce8_1)
```

### Comparing `finqual-0.1.6/LICENSE.txt` & `finqual-0.1.7/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `finqual-0.1.6/README.md` & `finqual-0.1.7/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -2,30 +2,42 @@
 
 This is a work in progress package that enables users to programmatically access the SEC EDGAR API database to retrieve financial information such as income statement, balance sheet or cash flow statement.
 
 ## Features
 Ability to call the income statement, balance sheet or cash flow statement for any company on the within EDGAR, the SEC's Electronic Data Gathering, Analysis, and Retrieval system.
 
 This has two key features that enable better programmatic access compared to other providers:
-- Ability to call upto 10 requests per second
+- Ability to call up to 10 requests per second, with built-in rate limiter
 - No restriction on the number of calls within a certain timeframe
 
-## Functions
-First, import the package using:
+## Functionality
+
+First, ensure that the required packages are installed (see the "Dependencies" section). Import the package using:
 ```
 from finqual import finqual as fq
 ```
+
 From there, use a "Ticker" class to call the desired stock and the desired financial statement. For example:
 ```
 fq.Ticker("TSLA").income(2020,2022)
 fq.Ticker("TSLA").balance(2020,2022, quarter = True)
 fq.Ticker("TSLA").cashflow(2020,2022)
 ```
 
 Note that the financial statement function takes a mandatory timeframe input and then an optional input to return the quarterly results within that timeframe (default to annual results if not inputted).
 
+## Dependencies
+
+Only four packages are required, with the following versions confirmed to be working:
+
+| Package   | Version  |
+|-----------|----------|
+| pandas    | ≥ 2.0.2  |
+| numpy     | ≥ 1.24.3 |
+| requests  | ≥ 2.31.0 |
+| ratelimit | ≥ 2.2.1  |
+
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
-- More comprehensive mappings from known tags 
-- No built-in way to restrict requests to 10 per second yet
+- More comprehensive mappings from known tags
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `finqual-0.1.6/pyproject.toml` & `finqual-0.1.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "finqual"
-version = "0.1.6"
+version = "0.1.7"
 authors = [
   { name="Myztika"},
 ]
 description = "A package to retrieve historical fundamental financial data such as income statement, balance sheet and cashflow statement directly from the SEC with no request caps and fast request rate limits"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `finqual-0.1.6/PKG-INFO` & `finqual-0.1.7/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: finqual
-Version: 0.1.6
+Version: 0.1.7
 Summary: A package to retrieve historical fundamental financial data such as income statement, balance sheet and cashflow statement directly from the SEC with no request caps and fast request rate limits
 Author: Myztika
 License-File: LICENSE.txt
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
@@ -14,30 +14,42 @@
 
 This is a work in progress package that enables users to programmatically access the SEC EDGAR API database to retrieve financial information such as income statement, balance sheet or cash flow statement.
 
 ## Features
 Ability to call the income statement, balance sheet or cash flow statement for any company on the within EDGAR, the SEC's Electronic Data Gathering, Analysis, and Retrieval system.
 
 This has two key features that enable better programmatic access compared to other providers:
-- Ability to call upto 10 requests per second
+- Ability to call up to 10 requests per second, with built-in rate limiter
 - No restriction on the number of calls within a certain timeframe
 
-## Functions
-First, import the package using:
+## Functionality
+
+First, ensure that the required packages are installed (see the "Dependencies" section). Import the package using:
 ```
 from finqual import finqual as fq
 ```
+
 From there, use a "Ticker" class to call the desired stock and the desired financial statement. For example:
 ```
 fq.Ticker("TSLA").income(2020,2022)
 fq.Ticker("TSLA").balance(2020,2022, quarter = True)
 fq.Ticker("TSLA").cashflow(2020,2022)
 ```
 
 Note that the financial statement function takes a mandatory timeframe input and then an optional input to return the quarterly results within that timeframe (default to annual results if not inputted).
 
+## Dependencies
+
+Only four packages are required, with the following versions confirmed to be working:
+
+| Package   | Version  |
+|-----------|----------|
+| pandas    | ≥ 2.0.2  |
+| numpy     | ≥ 1.24.3 |
+| requests  | ≥ 2.31.0 |
+| ratelimit | ≥ 2.2.1  |
+
 ## Limitations
 Currently, there are several known limitations that I am aware of from my own testing. These are still to be looked at:
 
 - Missing data values for companies, this is mostly due to companies using custom tags that are not accessible via the SEC database, and quite prevalent for quarterly reports as well
-- More comprehensive mappings from known tags 
-- No built-in way to restrict requests to 10 per second yet
+- More comprehensive mappings from known tags
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

