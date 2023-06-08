# Comparing `tmp/ebank-2023.6.8.tar.gz` & `tmp/ebank-2023.6.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebank-2023.6.8.tar", last modified: Thu Jun  8 02:26:36 2023, max compression
+gzip compressed data, was "ebank-2023.6.8.1.tar", last modified: Thu Jun  8 03:20:03 2023, max compression
```

## Comparing `ebank-2023.6.8.tar` & `ebank-2023.6.8.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.297787 ebank-2023.6.8/
--rw-rw-rw-   0        0        0       55 2023-06-08 02:26:36.296781 ebank-2023.6.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.249082 ebank-2023.6.8/ebank/
--rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-2023.6.8/ebank/__init__.py
--rw-rw-rw-   0        0        0     4766 2023-06-07 09:17:41.000000 ebank-2023.6.8/ebank/balance.py
--rw-rw-rw-   0        0        0     1211 2023-06-07 09:24:29.000000 ebank-2023.6.8/ebank/constants.py
--rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-2023.6.8/ebank/receipt.py
--rw-rw-rw-   0        0        0     6639 2023-06-07 08:48:28.000000 ebank-2023.6.8/ebank/trans.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.292780 ebank-2023.6.8/ebank/utils/
--rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-2023.6.8/ebank/utils/__init__.py
--rw-rw-rw-   0        0        0     2156 2023-06-06 09:41:09.000000 ebank-2023.6.8/ebank/utils/baiduocr.py
--rw-rw-rw-   0        0        0     1516 2023-06-06 09:40:51.000000 ebank-2023.6.8/ebank/utils/chaojiying.py
--rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-2023.6.8/ebank/utils/filesearch.py
--rw-rw-rw-   0        0        0     4816 2023-06-07 07:26:54.000000 ebank-2023.6.8/ebank/utils/sfun.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.267513 ebank-2023.6.8/ebank.egg-info/
--rw-rw-rw-   0        0        0       55 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-08 02:26:36.000000 ebank-2023.6.8/ebank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 02:26:36.297787 ebank-2023.6.8/setup.cfg
--rw-rw-rw-   0        0        0      506 2023-06-08 02:26:29.000000 ebank-2023.6.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:20:03.034013 ebank-2023.6.8.1/
+-rw-rw-rw-   0        0        0       57 2023-06-08 03:20:03.030912 ebank-2023.6.8.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 03:20:02.976911 ebank-2023.6.8.1/ebank/
+-rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-2023.6.8.1/ebank/__init__.py
+-rw-rw-rw-   0        0        0     4797 2023-06-08 03:14:11.000000 ebank-2023.6.8.1/ebank/balance.py
+-rw-rw-rw-   0        0        0     1217 2023-06-08 03:05:32.000000 ebank-2023.6.8.1/ebank/constants.py
+-rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-2023.6.8.1/ebank/receipt.py
+-rw-rw-rw-   0        0        0     6670 2023-06-08 03:11:01.000000 ebank-2023.6.8.1/ebank/trans.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:20:03.025912 ebank-2023.6.8.1/ebank/utils/
+-rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-2023.6.8.1/ebank/utils/__init__.py
+-rw-rw-rw-   0        0        0     2168 2023-06-08 03:11:54.000000 ebank-2023.6.8.1/ebank/utils/baiduocr.py
+-rw-rw-rw-   0        0        0     1528 2023-06-08 03:11:40.000000 ebank-2023.6.8.1/ebank/utils/chaojiying.py
+-rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-2023.6.8.1/ebank/utils/filesearch.py
+-rw-rw-rw-   0        0        0     4816 2023-06-07 07:26:54.000000 ebank-2023.6.8.1/ebank/utils/sfun.py
+drwxrwxrwx   0        0        0        0 2023-06-08 03:20:03.001915 ebank-2023.6.8.1/ebank.egg-info/
+-rw-rw-rw-   0        0        0       57 2023-06-08 03:20:02.000000 ebank-2023.6.8.1/ebank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-08 03:20:02.000000 ebank-2023.6.8.1/ebank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 03:20:02.000000 ebank-2023.6.8.1/ebank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-08 03:20:02.000000 ebank-2023.6.8.1/ebank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 03:20:02.000000 ebank-2023.6.8.1/ebank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 03:20:03.035932 ebank-2023.6.8.1/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-06-08 03:19:48.000000 ebank-2023.6.8.1/setup.py
```

### Comparing `ebank-2023.6.8/ebank/balance.py` & `ebank-2023.6.8.1/ebank/balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sqlite3
 from abc import ABC, abstractmethod
 from datetime import datetime
 
-import constants as CONSTANTS
 from encoo.logger import Logger
-from utils import sfun
+
+import ebank.constants as CONSTANTS
+from ebank.utils import sfun
 
 
 class BaseBalance(ABC):
 
     _logger = Logger("BaseBalance")
 
     def __init__(self, file_path, row_start_idx):
@@ -77,19 +78,19 @@
                 row_list.append(trans_row)
             # end for
         except Exception as ex:
             self._logger.error(f"BaseTrans extract  {ex}")
         # end try
         return row_list
 
-    def to_sqlite(self) -> None:
+    def to_sqlite(self, db_path=CONSTANTS.SQLITE3_PATH) -> None:
         rows = self.extract()
         self._logger.info(f"BaseBalance to_sqlite {rows}")
         try:
-            conn = sqlite3.connect(CONSTANTS.SQLITE3_PATH)
+            conn = sqlite3.connect(db_path)
             cur = conn.cursor()
             sql = CONSTANTS.SQL_INSERT_BALANCE
             cur.executemany(sql, rows)
             conn.commit()
 
             cur.close()
             conn.close()
```

### Comparing `ebank-2023.6.8/ebank/constants.py` & `ebank-2023.6.8.1/ebank/constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 BANK_NAME_IDX = 2
 BANK_NO_IDX = -1
-SQLITE3_PATH = r"dbs\ebank.db"
+SQLITE3_PATH = r"D:\rpadbs\ebank.db"
 
 
 BANK_NO_DICT = {
     "4301016509812100729": "江苏银行股份有限公司",
     "4301016509813100767": "江苏银行股份有限公司",
     "4301016509814104041": "江苏银行股份有限公司",
     "4301016509827101946": "江苏银行股份有限公司",
```

### Comparing `ebank-2023.6.8/ebank/receipt.py` & `ebank-2023.6.8.1/ebank/receipt.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8/ebank/trans.py` & `ebank-2023.6.8.1/ebank/trans.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sqlite3
 from abc import ABC, abstractmethod
 from datetime import datetime
 
-import constants as CONSTANTS
 from encoo.logger import Logger
-from utils import sfun
+
+import ebank.constants as CONSTANTS
+from ebank.utils import sfun
 
 
 class BaseTrans(ABC):
 
     _logger = Logger("BaseTrans")
 
     def __init__(self, file_path, row_start_idx):
@@ -110,19 +111,19 @@
                 row_list.append(trans_row)
             # end for
         except Exception as ex:
             self._logger.error(f"BaseTrans extract  {ex}")
         # end try
         return row_list
 
-    def to_sqlite(self) -> None:
+    def to_sqlite(self, db_path=CONSTANTS.SQLITE3_PATH) -> None:
         rows = self.extract()
         self._logger.info(f"BaseTrans to_sqlite {rows}")
         try:
-            conn = sqlite3.connect(CONSTANTS.SQLITE3_PATH)
+            conn = sqlite3.connect(db_path)
             cur = conn.cursor()
             sql = CONSTANTS.SQL_INSERT_TRANS
             cur.executemany(sql, rows)
             conn.commit()
 
             cur.close()
             conn.close()
```

### Comparing `ebank-2023.6.8/ebank/utils/baiduocr.py` & `ebank-2023.6.8.1/ebank/utils/baiduocr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import base64
 import json
 
 import requests
 from encoo.logger import Logger
 
-import sfun as util
+import ebank.utils.sfun as util
 
 
 class BaiduOCR:
 
     __logger = Logger("BaiduOCR")
 
     def __init__(self) -> None:
```

### Comparing `ebank-2023.6.8/ebank/utils/chaojiying.py` & `ebank-2023.6.8.1/ebank/utils/chaojiying.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 # coding:utf-8
 
 from hashlib import md5
 
 import requests
 
-import sfun as util
+import ebank.utils.sfun as util
 
 
 class Chaojiying_Client(object):
 
     def __init__(self, username, password, soft_id):
         self.username = username
         password = password.encode('utf8')
```

### Comparing `ebank-2023.6.8/ebank/utils/filesearch.py` & `ebank-2023.6.8.1/ebank/utils/filesearch.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8/ebank/utils/sfun.py` & `ebank-2023.6.8.1/ebank/utils/sfun.py`

 * *Files identical despite different names*

