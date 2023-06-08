# Comparing `tmp/tgr_wdn_query_lang-1.1.5.tar.gz` & `tmp/tgr_wdn_query_lang-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgr_wdn_query_lang-1.1.5.tar", max compression
+gzip compressed data, was "tgr_wdn_query_lang-1.1.7.tar", max compression
```

## Comparing `tgr_wdn_query_lang-1.1.5.tar` & `tgr_wdn_query_lang-1.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      700 2023-02-24 06:19:45.645389 tgr_wdn_query_lang-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       41 2023-02-23 07:21:26.467811 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/__init__.py
--rw-r--r--   0        0        0     7142 2023-02-23 17:17:42.851962 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprLexer.interp
--rw-r--r--   0        0        0     7198 2023-02-23 17:17:42.944380 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprLexer.py
--rw-r--r--   0        0        0      177 2023-02-23 17:17:42.946668 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprLexer.tokens
--rw-r--r--   0        0        0     1235 2023-02-23 17:17:43.279788 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParser.interp
--rw-r--r--   0        0        0     8309 2023-02-23 17:17:43.433926 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParser.py
--rw-r--r--   0        0        0      177 2023-02-23 17:17:43.442542 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParser.tokens
--rw-r--r--   0        0        0      908 2023-02-23 17:17:43.437355 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParserListener.py
--rw-r--r--   0        0        0      705 2023-02-23 17:17:43.440150 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParserVisitor.py
--rw-r--r--   0        0        0        0 2023-02-23 07:21:26.470647 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/__init__.py
--rw-r--r--   0        0        0     7278 2023-02-24 06:19:45.646436 tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/query.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 tgr_wdn_query_lang-1.1.5/setup.py
--rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 tgr_wdn_query_lang-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0      732 2023-06-08 02:01:39.469739 tgr_wdn_query_lang-1.1.7/COPYRIGHT
+-rw-r--r--   0        0        0      721 2023-06-08 02:10:44.491629 tgr_wdn_query_lang-1.1.7/pyproject.toml
+-rw-r--r--   0        0        0       41 2023-06-08 01:21:05.368137 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/__init__.py
+-rw-r--r--   0        0        0     7142 2023-06-08 01:21:05.368269 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprLexer.interp
+-rw-r--r--   0        0        0     7198 2023-06-08 01:21:05.368367 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprLexer.py
+-rw-r--r--   0        0        0      177 2023-06-08 01:21:05.368434 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprLexer.tokens
+-rw-r--r--   0        0        0     1235 2023-06-08 01:21:05.368502 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParser.interp
+-rw-r--r--   0        0        0     8309 2023-06-08 01:21:05.368600 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParser.py
+-rw-r--r--   0        0        0      177 2023-06-08 01:21:05.368675 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParser.tokens
+-rw-r--r--   0        0        0      908 2023-06-08 01:21:05.368758 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParserListener.py
+-rw-r--r--   0        0        0      705 2023-06-08 01:21:05.368836 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParserVisitor.py
+-rw-r--r--   0        0        0        0 2023-06-08 01:21:05.368867 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/__init__.py
+-rw-r--r--   0        0        0     7278 2023-06-08 01:21:05.368968 tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/query.py
+-rw-r--r--   0        0        0     1271 1970-01-01 00:00:00.000000 tgr_wdn_query_lang-1.1.7/PKG-INFO
```

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprLexer.interp` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprLexer.interp`

 * *Files identical despite different names*

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprLexer.py` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprLexer.py`

 * *Files identical despite different names*

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParser.interp` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParser.interp`

 * *Files identical despite different names*

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParser.py` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParser.py`

 * *Files identical despite different names*

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParserListener.py` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParserListener.py`

 * *Files identical despite different names*

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/generated/QueryExprParserVisitor.py` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/generated/QueryExprParserVisitor.py`

 * *Files identical despite different names*

### Comparing `tgr_wdn_query_lang-1.1.5/src/tgr_wdn_query_lang/query.py` & `tgr_wdn_query_lang-1.1.7/src/tgr_wdn_query_lang/query.py`

 * *Files identical despite different names*

