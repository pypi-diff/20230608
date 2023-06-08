# Comparing `tmp/ebank-2.0.0.tar.gz` & `tmp/ebank-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ebank-2.0.0.tar", last modified: Thu Jun  8 02:14:58 2023, max compression
+gzip compressed data, was "ebank-2023.6.8.tar", last modified: Thu Jun  8 02:26:36 2023, max compression
```

## Comparing `ebank-2.0.0.tar` & `ebank-2023.6.8.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:58.391428 ebank-2.0.0/
--rw-rw-rw-   0        0        0       52 2023-06-08 02:14:58.390414 ebank-2.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:58.348165 ebank-2.0.0/ebank/
--rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-2.0.0/ebank/__init__.py
--rw-rw-rw-   0        0        0     4766 2023-06-07 09:17:41.000000 ebank-2.0.0/ebank/balance.py
--rw-rw-rw-   0        0        0     1211 2023-06-07 09:24:29.000000 ebank-2.0.0/ebank/constants.py
--rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-2.0.0/ebank/receipt.py
--rw-rw-rw-   0        0        0     6639 2023-06-07 08:48:28.000000 ebank-2.0.0/ebank/trans.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:58.387835 ebank-2.0.0/ebank/utils/
--rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-2.0.0/ebank/utils/__init__.py
--rw-rw-rw-   0        0        0     2156 2023-06-06 09:41:09.000000 ebank-2.0.0/ebank/utils/baiduocr.py
--rw-rw-rw-   0        0        0     1516 2023-06-06 09:40:51.000000 ebank-2.0.0/ebank/utils/chaojiying.py
--rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-2.0.0/ebank/utils/filesearch.py
--rw-rw-rw-   0        0        0     4816 2023-06-07 07:26:54.000000 ebank-2.0.0/ebank/utils/sfun.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:14:58.365977 ebank-2.0.0/ebank.egg-info/
--rw-rw-rw-   0        0        0       52 2023-06-08 02:14:58.000000 ebank-2.0.0/ebank.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      358 2023-06-08 02:14:58.000000 ebank-2.0.0/ebank.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:14:58.000000 ebank-2.0.0/ebank.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      125 2023-06-08 02:14:58.000000 ebank-2.0.0/ebank.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-06-08 02:14:58.000000 ebank-2.0.0/ebank.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 02:14:58.392428 ebank-2.0.0/setup.cfg
--rw-rw-rw-   0        0        0      500 2023-06-08 02:12:32.000000 ebank-2.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.297787 ebank-2023.6.8/
+-rw-rw-rw-   0        0        0       55 2023-06-08 02:26:36.296781 ebank-2023.6.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.249082 ebank-2023.6.8/ebank/
+-rw-rw-rw-   0        0        0        4 2023-06-07 07:25:49.000000 ebank-2023.6.8/ebank/__init__.py
+-rw-rw-rw-   0        0        0     4766 2023-06-07 09:17:41.000000 ebank-2023.6.8/ebank/balance.py
+-rw-rw-rw-   0        0        0     1211 2023-06-07 09:24:29.000000 ebank-2023.6.8/ebank/constants.py
+-rw-rw-rw-   0        0        0    24486 2023-06-06 05:27:42.000000 ebank-2023.6.8/ebank/receipt.py
+-rw-rw-rw-   0        0        0     6639 2023-06-07 08:48:28.000000 ebank-2023.6.8/ebank/trans.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.292780 ebank-2023.6.8/ebank/utils/
+-rw-rw-rw-   0        0        0        2 2023-06-06 05:27:42.000000 ebank-2023.6.8/ebank/utils/__init__.py
+-rw-rw-rw-   0        0        0     2156 2023-06-06 09:41:09.000000 ebank-2023.6.8/ebank/utils/baiduocr.py
+-rw-rw-rw-   0        0        0     1516 2023-06-06 09:40:51.000000 ebank-2023.6.8/ebank/utils/chaojiying.py
+-rw-rw-rw-   0        0        0     2474 2023-06-06 05:27:42.000000 ebank-2023.6.8/ebank/utils/filesearch.py
+-rw-rw-rw-   0        0        0     4816 2023-06-07 07:26:54.000000 ebank-2023.6.8/ebank/utils/sfun.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:26:36.267513 ebank-2023.6.8/ebank.egg-info/
+-rw-rw-rw-   0        0        0       55 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      358 2023-06-08 02:26:36.000000 ebank-2023.6.8/ebank.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      128 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-06-08 02:26:35.000000 ebank-2023.6.8/ebank.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 02:26:36.297787 ebank-2023.6.8/setup.cfg
+-rw-rw-rw-   0        0        0      506 2023-06-08 02:26:29.000000 ebank-2023.6.8/setup.py
```

### Comparing `ebank-2.0.0/ebank/balance.py` & `ebank-2023.6.8/ebank/balance.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/constants.py` & `ebank-2023.6.8/ebank/constants.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/receipt.py` & `ebank-2023.6.8/ebank/receipt.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/trans.py` & `ebank-2023.6.8/ebank/trans.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/utils/baiduocr.py` & `ebank-2023.6.8/ebank/utils/baiduocr.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/utils/chaojiying.py` & `ebank-2023.6.8/ebank/utils/chaojiying.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/utils/filesearch.py` & `ebank-2023.6.8/ebank/utils/filesearch.py`

 * *Files identical despite different names*

### Comparing `ebank-2.0.0/ebank/utils/sfun.py` & `ebank-2023.6.8/ebank/utils/sfun.py`

 * *Files identical despite different names*

