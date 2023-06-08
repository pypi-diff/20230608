# Comparing `tmp/verseql-0.0.1.tar.gz` & `tmp/verseql-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "verseql-0.0.1.tar", last modified: Thu Jun  8 19:32:16 2023, max compression
+gzip compressed data, was "verseql-0.0.2.tar", last modified: Thu Jun  8 19:34:59 2023, max compression
```

## Comparing `verseql-0.0.1.tar` & `verseql-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 19:32:16.985674 verseql-0.0.1/
--rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verseql-0.0.1/LICENSE
--rw-rw-rw-   0        0        0    23543 2023-06-08 19:32:16.984684 verseql-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    22962 2023-05-21 06:49:11.000000 verseql-0.0.1/README.md
--rw-rw-rw-   0        0        0      708 2023-06-08 19:31:07.000000 verseql-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-08 19:32:16.985674 verseql-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-08 19:32:16.957748 verseql-0.0.1/verseql/
--rw-rw-rw-   0        0        0      609 2023-06-07 19:29:22.000000 verseql-0.0.1/verseql/__init__.py
--rw-rw-rw-   0        0        0     4566 2023-06-08 17:57:06.000000 verseql-0.0.1/verseql/_expression.py
--rw-rw-rw-   0        0        0     1702 2023-06-08 07:25:36.000000 verseql-0.0.1/verseql/_order.py
--rw-rw-rw-   0        0        0    19451 2023-06-08 18:26:15.000000 verseql-0.0.1/verseql/_parser_listener.py
--rw-rw-rw-   0        0        0     1459 2023-06-07 23:13:45.000000 verseql-0.0.1/verseql/_projection.py
--rw-rw-rw-   0        0        0     1617 2023-06-08 07:41:54.000000 verseql-0.0.1/verseql/_query.py
--rw-rw-rw-   0        0        0     1961 2023-06-08 19:27:28.000000 verseql-0.0.1/verseql/_verseql.py
-drwxrwxrwx   0        0        0        0 2023-06-08 19:32:16.982691 verseql-0.0.1/verseql/generated/
--rw-rw-rw-   0        0        0    17271 2023-06-08 18:23:05.000000 verseql-0.0.1/verseql/generated/VerseQLLexer.py
--rw-rw-rw-   0        0        0    89848 2023-06-08 18:23:05.000000 verseql-0.0.1/verseql/generated/VerseQLParser.py
--rw-rw-rw-   0        0        0    15381 2023-06-08 18:23:05.000000 verseql-0.0.1/verseql/generated/VerseQLParserListener.py
--rw-rw-rw-   0        0        0        0 2023-06-07 19:50:26.000000 verseql-0.0.1/verseql/generated/__init__.py
--rw-rw-rw-   0        0        0       26 2023-05-11 01:27:50.000000 verseql-0.0.1/verseql/py.typed
-drwxrwxrwx   0        0        0        0 2023-06-08 19:32:16.976696 verseql-0.0.1/verseql.egg-info/
--rw-rw-rw-   0        0        0    23543 2023-06-08 19:32:16.000000 verseql-0.0.1/verseql.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      465 2023-06-08 19:32:16.000000 verseql-0.0.1/verseql.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 19:32:16.000000 verseql-0.0.1/verseql.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2023-06-08 19:32:16.000000 verseql-0.0.1/verseql.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 19:34:59.107825 verseql-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2023-02-12 19:43:35.000000 verseql-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      605 2023-06-08 19:34:59.107825 verseql-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       22 2023-06-08 19:34:24.000000 verseql-0.0.2/README.md
+-rw-rw-rw-   0        0        0      708 2023-06-08 19:34:40.000000 verseql-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 19:34:59.107825 verseql-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 19:34:59.090726 verseql-0.0.2/verseql/
+-rw-rw-rw-   0        0        0      609 2023-06-07 19:29:22.000000 verseql-0.0.2/verseql/__init__.py
+-rw-rw-rw-   0        0        0     4566 2023-06-08 17:57:06.000000 verseql-0.0.2/verseql/_expression.py
+-rw-rw-rw-   0        0        0     1702 2023-06-08 07:25:36.000000 verseql-0.0.2/verseql/_order.py
+-rw-rw-rw-   0        0        0    19451 2023-06-08 18:26:15.000000 verseql-0.0.2/verseql/_parser_listener.py
+-rw-rw-rw-   0        0        0     1459 2023-06-07 23:13:45.000000 verseql-0.0.2/verseql/_projection.py
+-rw-rw-rw-   0        0        0     1617 2023-06-08 07:41:54.000000 verseql-0.0.2/verseql/_query.py
+-rw-rw-rw-   0        0        0     1961 2023-06-08 19:27:28.000000 verseql-0.0.2/verseql/_verseql.py
+drwxrwxrwx   0        0        0        0 2023-06-08 19:34:59.107825 verseql-0.0.2/verseql/generated/
+-rw-rw-rw-   0        0        0    17271 2023-06-08 18:23:05.000000 verseql-0.0.2/verseql/generated/VerseQLLexer.py
+-rw-rw-rw-   0        0        0    89848 2023-06-08 18:23:05.000000 verseql-0.0.2/verseql/generated/VerseQLParser.py
+-rw-rw-rw-   0        0        0    15381 2023-06-08 18:23:05.000000 verseql-0.0.2/verseql/generated/VerseQLParserListener.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 19:50:26.000000 verseql-0.0.2/verseql/generated/__init__.py
+-rw-rw-rw-   0        0        0       26 2023-05-11 01:27:50.000000 verseql-0.0.2/verseql/py.typed
+drwxrwxrwx   0        0        0        0 2023-06-08 19:34:59.105719 verseql-0.0.2/verseql.egg-info/
+-rw-rw-rw-   0        0        0      605 2023-06-08 19:34:59.000000 verseql-0.0.2/verseql.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      465 2023-06-08 19:34:59.000000 verseql-0.0.2/verseql.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 19:34:59.000000 verseql-0.0.2/verseql.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 19:34:59.000000 verseql-0.0.2/verseql.egg-info/top_level.txt
```

### Comparing `verseql-0.0.1/LICENSE` & `verseql-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/pyproject.toml` & `verseql-0.0.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "verseql"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Rapidverse", email = "verse@rapidverse.com" }]
 description = "VerseQL provides a SQL-like query language for accessing and manipulating data across many Verses."
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `verseql-0.0.1/verseql/__init__.py` & `verseql-0.0.2/verseql/__init__.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/_expression.py` & `verseql-0.0.2/verseql/_expression.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/_order.py` & `verseql-0.0.2/verseql/_order.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/_parser_listener.py` & `verseql-0.0.2/verseql/_parser_listener.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/_projection.py` & `verseql-0.0.2/verseql/_projection.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/_query.py` & `verseql-0.0.2/verseql/_query.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/_verseql.py` & `verseql-0.0.2/verseql/_verseql.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/generated/VerseQLLexer.py` & `verseql-0.0.2/verseql/generated/VerseQLLexer.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/generated/VerseQLParser.py` & `verseql-0.0.2/verseql/generated/VerseQLParser.py`

 * *Files identical despite different names*

### Comparing `verseql-0.0.1/verseql/generated/VerseQLParserListener.py` & `verseql-0.0.2/verseql/generated/VerseQLParserListener.py`

 * *Files identical despite different names*

