# Comparing `tmp/MySQLPandas-0.0.18.tar.gz` & `tmp/MySQLPandas-0.0.19.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MySQLPandas-0.0.18.tar", last modified: Fri Apr 14 06:51:00 2023, max compression
+gzip compressed data, was "MySQLPandas-0.0.19.tar", last modified: Thu Jun  8 06:53:15 2023, max compression
```

## Comparing `MySQLPandas-0.0.18.tar` & `MySQLPandas-0.0.19.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.546800 MySQLPandas-0.0.18/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    18092 2023-04-11 06:04:32.000000 MySQLPandas-0.0.18/LICENSE
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       16 2023-04-14 06:31:32.000000 MySQLPandas-0.0.18/MANIFEST.in
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.534800 MySQLPandas-0.0.18/MySQLPandas/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      294 2023-04-14 06:50:35.000000 MySQLPandas-0.0.18/MySQLPandas/__init__.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    14088 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/core.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.542800 MySQLPandas-0.0.18/MySQLPandas/lib/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     6471 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/lib/DataFrameClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       92 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/lib/ErrorClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:26:18.000000 MySQLPandas-0.0.18/MySQLPandas/lib/__init__.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.539801 MySQLPandas-0.0.18/MySQLPandas.egg-info/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3464 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/PKG-INFO
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      401 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/SOURCES.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        1 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/dependency_links.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       58 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/requires.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       28 2023-04-14 06:51:00.000000 MySQLPandas-0.0.18/MySQLPandas.egg-info/top_level.txt
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3464 2023-04-14 06:51:00.545800 MySQLPandas-0.0.18/PKG-INFO
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2821 2023-04-14 06:50:30.000000 MySQLPandas-0.0.18/README.md
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       38 2023-04-14 06:51:00.546800 MySQLPandas-0.0.18/setup.cfg
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1893 2023-04-11 06:10:37.000000 MySQLPandas-0.0.18/setup.py
-drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:51:00.544800 MySQLPandas-0.0.18/tests/
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     4526 2023-04-07 04:49:44.000000 MySQLPandas-0.0.18/tests/test_DataFrameClass.py
--rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2132 2023-04-07 06:25:10.000000 MySQLPandas-0.0.18/tests/test_coreClass.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-06-08 06:53:15.969682 MySQLPandas-0.0.19/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    18092 2023-04-11 06:04:32.000000 MySQLPandas-0.0.19/LICENSE
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       16 2023-04-14 06:31:32.000000 MySQLPandas-0.0.19/MANIFEST.in
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-06-08 06:53:15.953682 MySQLPandas-0.0.19/MySQLPandas/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      294 2023-06-08 06:35:41.000000 MySQLPandas-0.0.19/MySQLPandas/__init__.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)    14088 2023-04-14 06:26:18.000000 MySQLPandas-0.0.19/MySQLPandas/core.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-06-08 06:53:15.964682 MySQLPandas-0.0.19/MySQLPandas/lib/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     6471 2023-06-08 06:27:04.000000 MySQLPandas-0.0.19/MySQLPandas/lib/DataFrameClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       92 2023-04-14 06:26:18.000000 MySQLPandas-0.0.19/MySQLPandas/lib/ErrorClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        0 2023-04-14 06:26:18.000000 MySQLPandas-0.0.19/MySQLPandas/lib/__init__.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-06-08 06:53:15.960682 MySQLPandas-0.0.19/MySQLPandas.egg-info/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3706 2023-06-08 06:53:15.000000 MySQLPandas-0.0.19/MySQLPandas.egg-info/PKG-INFO
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)      401 2023-06-08 06:53:15.000000 MySQLPandas-0.0.19/MySQLPandas.egg-info/SOURCES.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)        1 2023-06-08 06:53:15.000000 MySQLPandas-0.0.19/MySQLPandas.egg-info/dependency_links.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       58 2023-06-08 06:53:15.000000 MySQLPandas-0.0.19/MySQLPandas.egg-info/requires.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       28 2023-06-08 06:53:15.000000 MySQLPandas-0.0.19/MySQLPandas.egg-info/top_level.txt
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3706 2023-06-08 06:53:15.968682 MySQLPandas-0.0.19/PKG-INFO
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     3063 2023-06-08 06:43:10.000000 MySQLPandas-0.0.19/README.md
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)       38 2023-06-08 06:53:15.969682 MySQLPandas-0.0.19/setup.cfg
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     1893 2023-04-11 06:10:37.000000 MySQLPandas-0.0.19/setup.py
+drwxrwxr-x   0 nakashima  (1010) nakashima  (1012)        0 2023-06-08 06:53:15.967682 MySQLPandas-0.0.19/tests/
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     4526 2023-04-07 04:49:44.000000 MySQLPandas-0.0.19/tests/test_DataFrameClass.py
+-rw-rw-r--   0 nakashima  (1010) nakashima  (1012)     2132 2023-04-07 06:25:10.000000 MySQLPandas-0.0.19/tests/test_coreClass.py
```

### Comparing `MySQLPandas-0.0.18/LICENSE` & `MySQLPandas-0.0.19/LICENSE`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.18/MySQLPandas/core.py` & `MySQLPandas-0.0.19/MySQLPandas/core.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.18/MySQLPandas/lib/DataFrameClass.py` & `MySQLPandas-0.0.19/MySQLPandas/lib/DataFrameClass.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.list_for_command = None
         self.sql_command = None
         self.sql_command_list = None
         self.table_name = table_name
     
     def makeDBFrame(self) -> None:
         #create sql command
-        column_name = list(map(lambda x:x.replace(" ","_"),list(self.df.columns))) #column name list
+        column_name = list(map(lambda x:x.replace(" "," "),list(self.df.columns))) #column name list
 
         column_type = list(map(str,list(self.df.dtypes))) #column dtype list
         column_type = list(map(lambda x:x.replace("64",""),column_type)) #remove "64"
         column_type = list(map(lambda x:x.replace("object","varchar"),column_type)) #translate string column
         #append convert "float" to "double"?
         column_max_len = []
         count = 0
```

### Comparing `MySQLPandas-0.0.18/MySQLPandas.egg-info/PKG-INFO` & `MySQLPandas-0.0.19/MySQLPandas.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MySQLPandas
-Version: 0.0.18
+Version: 0.0.19
 Summary: MySQLPandas: simple connector between MySQL(MariaDB) and Pandas
 Home-page: https://github.com/Sota-Nakashima/MySQLPandas
 Author: Sota-Nakashima
 Author-email: souta.nakashima2001@gmail.com
 License: GPLv2
 Keywords: Python,Pandas,Database
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![PyPI](https://img.shields.io/badge/PyPI-0.0.18-blue)](https://pypi.org/project/MySQLPandas/)
+[![PyPI](https://img.shields.io/badge/PyPI-0.0.19-blue)](https://pypi.org/project/MySQLPandas/)
 [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
@@ -48,14 +48,16 @@
 ```
 If you want to change table definition, please see below.  
 * Change string type column  
   You can change table denfiniton automatically. Please rewrite  "Strict_Mode = False" in "insertRecord" method.
 * Change int or float type column  
   Sorry, you can't change it in MySQLPandas. Please rewrite it by using "executeSQLcommand" method. 
 
+0.0.19 ~
+* Columns are no longer automatically assigned an underscore instead of a space when the database is created. However, it is recommended to replace them with underbars as much as possible, since spaces may cause unintended behavior.
 ## Setup password.ini
 In default, you need to input DB password in your console every time.  
 If you felt bothered, you avoid this by creating "password.ini" file.  
 In GitHub page, it's put [sample file](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/password_sample.ini).
 ## Requirement
 * MySQL(MariaDB)  
 The version of Auther's MariaDB is 5.5.68-MariaDB MariaDB Server.
```

### Comparing `MySQLPandas-0.0.18/PKG-INFO` & `MySQLPandas-0.0.19/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MySQLPandas
-Version: 0.0.18
+Version: 0.0.19
 Summary: MySQLPandas: simple connector between MySQL(MariaDB) and Pandas
 Home-page: https://github.com/Sota-Nakashima/MySQLPandas
 Author: Sota-Nakashima
 Author-email: souta.nakashima2001@gmail.com
 License: GPLv2
 Keywords: Python,Pandas,Database
 Classifier: Development Status :: 4 - Beta
@@ -15,15 +15,15 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![PyPI](https://img.shields.io/badge/PyPI-0.0.18-blue)](https://pypi.org/project/MySQLPandas/)
+[![PyPI](https://img.shields.io/badge/PyPI-0.0.19-blue)](https://pypi.org/project/MySQLPandas/)
 [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
@@ -48,14 +48,16 @@
 ```
 If you want to change table definition, please see below.  
 * Change string type column  
   You can change table denfiniton automatically. Please rewrite  "Strict_Mode = False" in "insertRecord" method.
 * Change int or float type column  
   Sorry, you can't change it in MySQLPandas. Please rewrite it by using "executeSQLcommand" method. 
 
+0.0.19 ~
+* Columns are no longer automatically assigned an underscore instead of a space when the database is created. However, it is recommended to replace them with underbars as much as possible, since spaces may cause unintended behavior.
 ## Setup password.ini
 In default, you need to input DB password in your console every time.  
 If you felt bothered, you avoid this by creating "password.ini" file.  
 In GitHub page, it's put [sample file](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/password_sample.ini).
 ## Requirement
 * MySQL(MariaDB)  
 The version of Auther's MariaDB is 5.5.68-MariaDB MariaDB Server.
```

### Comparing `MySQLPandas-0.0.18/README.md` & `MySQLPandas-0.0.19/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 MySQLPandas
 ============
 [![pages-build-deployment](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment/badge.svg)](https://github.com/Sota-Nakashima/MySQLPandas/actions/workflows/pages/pages-build-deployment)
 [![Version](https://img.shields.io/badge/stable-main-gree)](https://github.com/Sota-Nakashima/MySQLPandas)
-[![PyPI](https://img.shields.io/badge/PyPI-0.0.18-blue)](https://pypi.org/project/MySQLPandas/)
+[![PyPI](https://img.shields.io/badge/PyPI-0.0.19-blue)](https://pypi.org/project/MySQLPandas/)
 [![License: GPL v2](https://img.shields.io/badge/License-GPL_v2-blue.svg)](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/LICENCE)
 #  Overview
 Simple connector between MySQL(MariaDB) and Pandas
 
 ## Description
 This tool is primarily intended to help Python users easily handle databases.
 It uses Pandas as its base, so it should be easy to use even for those who are not familiar with databases.
@@ -31,14 +31,16 @@
 ```
 If you want to change table definition, please see below.  
 * Change string type column  
   You can change table denfiniton automatically. Please rewrite  "Strict_Mode = False" in "insertRecord" method.
 * Change int or float type column  
   Sorry, you can't change it in MySQLPandas. Please rewrite it by using "executeSQLcommand" method. 
 
+0.0.19 ~
+* Columns are no longer automatically assigned an underscore instead of a space when the database is created. However, it is recommended to replace them with underbars as much as possible, since spaces may cause unintended behavior.
 ## Setup password.ini
 In default, you need to input DB password in your console every time.  
 If you felt bothered, you avoid this by creating "password.ini" file.  
 In GitHub page, it's put [sample file](https://github.com/Sota-Nakashima/MySQLPandas/blob/main/password_sample.ini).
 ## Requirement
 * MySQL(MariaDB)  
 The version of Auther's MariaDB is 5.5.68-MariaDB MariaDB Server.
```

### Comparing `MySQLPandas-0.0.18/setup.py` & `MySQLPandas-0.0.19/setup.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.18/tests/test_DataFrameClass.py` & `MySQLPandas-0.0.19/tests/test_DataFrameClass.py`

 * *Files identical despite different names*

### Comparing `MySQLPandas-0.0.18/tests/test_coreClass.py` & `MySQLPandas-0.0.19/tests/test_coreClass.py`

 * *Files identical despite different names*

