# Comparing `tmp/csvmove-0.2.1.tar.gz` & `tmp/csvmove-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csvmove-0.2.1.tar", max compression
+gzip compressed data, was "csvmove-0.2.2.tar", max compression
```

## Comparing `csvmove-0.2.1.tar` & `csvmove-0.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0        0 2023-03-24 17:40:59.139000 csvmove-0.2.1/csvmove/__init__.py
--rw-r--r--   0        0        0     1717 2023-03-25 21:49:48.654928 csvmove-0.2.1/csvmove/main.py
--rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 csvmove-0.2.1/LICENSE
--rw-r--r--   0        0        0      475 2023-03-25 21:49:53.657787 csvmove-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       66 2023-03-24 17:45:49.497725 csvmove-0.2.1/README.md
--rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 csvmove-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-03-24 17:40:59.139000 csvmove-0.2.2/csvmove/__init__.py
+-rw-r--r--   0        0        0     2375 2023-06-07 22:59:54.489472 csvmove-0.2.2/csvmove/main.py
+-rw-r--r--   0        0        0    35148 2023-03-21 17:20:22.235102 csvmove-0.2.2/LICENSE
+-rw-r--r--   0        0        0      475 2023-06-07 22:50:30.911396 csvmove-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       66 2023-03-24 17:45:49.497725 csvmove-0.2.2/README.md
+-rw-r--r--   0        0        0      634 1970-01-01 00:00:00.000000 csvmove-0.2.2/PKG-INFO
```

### Comparing `csvmove-0.2.1/LICENSE` & `csvmove-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `csvmove-0.2.1/PKG-INFO` & `csvmove-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csvmove
-Version: 0.2.1
+Version: 0.2.2
 Summary: CLI utility that moves files based on columns in a csv
 License: GPL-3.0-or-later
 Author: João Fauvel
 Author-email: jmmfauvel@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

