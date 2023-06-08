# Comparing `tmp/ebank-2023.6.8.3.tar.gz` & `tmp/ebank-2023.6.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebank-2023.6.8.3.tar", last modified: Thu Jun  8 05:44:03 2023, max compression
+gzip compressed data, was "ebank-2023.6.8.4.tar", last modified: Thu Jun  8 05:51:53 2023, max compression
```

## Comparing `ebank-2023.6.8.3.tar` & `ebank-2023.6.8.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 05:44:03.029901 ebank-2023.6.8.3/
--rw-rw-rw-   0        0        0       57 2023-06-08 05:44:03.027855 ebank-2023.6.8.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 05:44:02.967704 ebank-2023.6.8.3/ebank/
--rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-2023.6.8.3/ebank/__init__.py
--rw-rw-rw-   0        0        0     4797 2023-06-08 03:14:11.000000 ebank-2023.6.8.3/ebank/balance.py
--rw-rw-rw-   0        0        0     1435 2023-06-08 05:43:00.000000 ebank-2023.6.8.3/ebank/constants.py
--rw-rw-rw-   0        0        0     1665 2023-06-08 05:42:45.000000 ebank-2023.6.8.3/ebank/factory.py
--rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-2023.6.8.3/ebank/receipt.py
--rw-rw-rw-   0        0        0     6670 2023-06-08 03:11:01.000000 ebank-2023.6.8.3/ebank/trans.py
-drwxrwxrwx   0        0        0        0 2023-06-08 05:44:03.024996 ebank-2023.6.8.3/ebank/utils/
--rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-2023.6.8.3/ebank/utils/__init__.py
--rw-rw-rw-   0        0        0     2168 2023-06-08 03:11:54.000000 ebank-2023.6.8.3/ebank/utils/baiduocr.py
--rw-rw-rw-   0        0        0     1528 2023-06-08 03:11:40.000000 ebank-2023.6.8.3/ebank/utils/chaojiying.py
--rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-2023.6.8.3/ebank/utils/filesearch.py
--rw-rw-rw-   0        0        0     4919 2023-06-08 03:37:54.000000 ebank-2023.6.8.3/ebank/utils/sfun.py
-drwxrwxrwx   0        0        0        0 2023-06-08 05:44:03.004793 ebank-2023.6.8.3/ebank.egg-info/
--rw-rw-rw-   0        0        0       57 2023-06-08 05:44:02.000000 ebank-2023.6.8.3/ebank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-06-08 05:44:02.000000 ebank-2023.6.8.3/ebank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 05:44:02.000000 ebank-2023.6.8.3/ebank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      128 2023-06-08 05:44:02.000000 ebank-2023.6.8.3/ebank.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 05:44:02.000000 ebank-2023.6.8.3/ebank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 05:44:03.029901 ebank-2023.6.8.3/setup.cfg
--rw-rw-rw-   0        0        0      508 2023-06-08 05:43:57.000000 ebank-2023.6.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:51:53.800091 ebank-2023.6.8.4/
+-rw-rw-rw-   0        0        0       57 2023-06-08 05:51:53.797760 ebank-2023.6.8.4/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 05:51:53.757790 ebank-2023.6.8.4/ebank/
+-rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-2023.6.8.4/ebank/__init__.py
+-rw-rw-rw-   0        0        0     4797 2023-06-08 03:14:11.000000 ebank-2023.6.8.4/ebank/balance.py
+-rw-rw-rw-   0        0        0     1409 2023-06-08 05:50:52.000000 ebank-2023.6.8.4/ebank/constants.py
+-rw-rw-rw-   0        0        0     1665 2023-06-08 05:51:16.000000 ebank-2023.6.8.4/ebank/factory.py
+-rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-2023.6.8.4/ebank/receipt.py
+-rw-rw-rw-   0        0        0     6670 2023-06-08 03:11:01.000000 ebank-2023.6.8.4/ebank/trans.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:51:53.793752 ebank-2023.6.8.4/ebank/utils/
+-rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-2023.6.8.4/ebank/utils/__init__.py
+-rw-rw-rw-   0        0        0     2168 2023-06-08 03:11:54.000000 ebank-2023.6.8.4/ebank/utils/baiduocr.py
+-rw-rw-rw-   0        0        0     1528 2023-06-08 03:11:40.000000 ebank-2023.6.8.4/ebank/utils/chaojiying.py
+-rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-2023.6.8.4/ebank/utils/filesearch.py
+-rw-rw-rw-   0        0        0     4919 2023-06-08 03:37:54.000000 ebank-2023.6.8.4/ebank/utils/sfun.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:51:53.776752 ebank-2023.6.8.4/ebank.egg-info/
+-rw-rw-rw-   0        0        0       57 2023-06-08 05:51:53.000000 ebank-2023.6.8.4/ebank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-06-08 05:51:53.000000 ebank-2023.6.8.4/ebank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 05:51:53.000000 ebank-2023.6.8.4/ebank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-08 05:51:53.000000 ebank-2023.6.8.4/ebank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 05:51:53.000000 ebank-2023.6.8.4/ebank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 05:51:53.800755 ebank-2023.6.8.4/setup.cfg
+-rw-rw-rw-   0        0        0      508 2023-06-08 05:51:28.000000 ebank-2023.6.8.4/setup.py
```

### Comparing `ebank-2023.6.8.3/ebank/balance.py` & `ebank-2023.6.8.4/ebank/balance.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/constants.py` & `ebank-2023.6.8.4/ebank/constants.py`

 * *Files 15% similar despite different names*

```diff
@@ -21,16 +21,13 @@
 }
 
 SQL_INSERT_TRANS = 'insert into trans(file_path,bank_name,acc_name,acc_no,trans_date,flow_no,rec_amt,pay_amt,' + \
     ' balance,other_acc_name,other_acc_no,other_bank_name,purpose,abstract,remark,rct_path, task_id,' + \
     ' create_date,update_date,status) ' + \
     ' values(?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?,?)'
 
-SQL_QUERY_TRANS_BYDATE = 'SELECT * FROM	trans ' + \
-    'WHERE	trans_date ' + \
-    'BETWEEN ''{0}'' AND ''{1}'''
-
+SQL_QUERY_TRANS_BYDATE = 'SELECT * FROM trans WHERE trans_date BETWEEN \'{0}\' AND \'{1}\''
 
 SQL_INSERT_BALANCE = 'insert into balance(file_path,bank_name,acc_name,acc_no,' + \
     ' balance, query_date,currency,task_id,' + \
     ' create_date,update_date,status) ' + \
     ' values(?,?,?,?,?,?,?,?,?,?,?)'
```

### Comparing `ebank-2023.6.8.3/ebank/factory.py` & `ebank-2023.6.8.4/ebank/factory.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/receipt.py` & `ebank-2023.6.8.4/ebank/receipt.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/trans.py` & `ebank-2023.6.8.4/ebank/trans.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/utils/baiduocr.py` & `ebank-2023.6.8.4/ebank/utils/baiduocr.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/utils/chaojiying.py` & `ebank-2023.6.8.4/ebank/utils/chaojiying.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/utils/filesearch.py` & `ebank-2023.6.8.4/ebank/utils/filesearch.py`

 * *Files identical despite different names*

### Comparing `ebank-2023.6.8.3/ebank/utils/sfun.py` & `ebank-2023.6.8.4/ebank/utils/sfun.py`

 * *Files identical despite different names*

