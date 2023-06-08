# Comparing `tmp/psychoanalyze-0.2.2.tar.gz` & `tmp/psychoanalyze-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "psychoanalyze-0.2.2.tar", max compression
+gzip compressed data, was "psychoanalyze-0.3.0.tar", max compression
```

## Comparing `psychoanalyze-0.2.2.tar` & `psychoanalyze-0.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    35149 2023-06-07 09:32:29.259896 psychoanalyze-0.2.2/LICENSE
--rw-r--r--   0        0        0     1002 2023-06-07 09:32:29.259896 psychoanalyze-0.2.2/README.md
--rw-r--r--   0        0        0     1250 2023-06-07 09:33:23.344771 psychoanalyze-0.2.2/psychoanalyze/__init__.py
--rw-r--r--   0        0        0     6723 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/blocks.py
--rw-r--r--   0        0        0     2133 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/data.py
--rw-r--r--   0        0        0      148 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/gescheider.py
--rw-r--r--   0        0        0     8869 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/layout.py
--rw-r--r--   0        0        0     5594 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/plot.py
--rw-r--r--   0        0        0     5036 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/points.py
--rw-r--r--   0        0        0     1784 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/schemas.py
--rw-r--r--   0        0        0     2419 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/sessions.py
--rw-r--r--   0        0        0     2380 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/simulate.py
--rw-r--r--   0        0        0       95 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/stimulus.py
--rw-r--r--   0        0        0      565 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/strength_duration.py
--rw-r--r--   0        0        0      745 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/subjects.py
--rw-r--r--   0        0        0        0 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/transformations.py
--rw-r--r--   0        0        0     4069 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/trials.py
--rw-r--r--   0        0        0     1692 2023-06-07 09:32:29.335897 psychoanalyze-0.2.2/psychoanalyze/weber.py
--rw-r--r--   0        0        0     1991 2023-06-07 09:33:23.344771 psychoanalyze-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 psychoanalyze-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-07 10:36:08.142459 psychoanalyze-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1002 2023-06-07 10:36:08.142459 psychoanalyze-0.3.0/README.md
+-rw-r--r--   0        0        0     1250 2023-06-07 10:37:04.311926 psychoanalyze-0.3.0/psychoanalyze/__init__.py
+-rw-r--r--   0        0        0     6723 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/blocks.py
+-rw-r--r--   0        0        0     2133 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/data.py
+-rw-r--r--   0        0        0      148 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/gescheider.py
+-rw-r--r--   0        0        0     8869 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/layout.py
+-rw-r--r--   0        0        0     5594 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/plot.py
+-rw-r--r--   0        0        0     5036 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/points.py
+-rw-r--r--   0        0        0     1784 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/schemas.py
+-rw-r--r--   0        0        0     2419 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/sessions.py
+-rw-r--r--   0        0        0     2380 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/simulate.py
+-rw-r--r--   0        0        0       95 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/stimulus.py
+-rw-r--r--   0        0        0      565 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/strength_duration.py
+-rw-r--r--   0        0        0      745 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/subjects.py
+-rw-r--r--   0        0        0        0 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/transformations.py
+-rw-r--r--   0        0        0     4069 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/trials.py
+-rw-r--r--   0        0        0     1692 2023-06-07 10:36:08.222461 psychoanalyze-0.3.0/psychoanalyze/weber.py
+-rw-r--r--   0        0        0     1991 2023-06-07 10:37:04.311926 psychoanalyze-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2937 1970-01-01 00:00:00.000000 psychoanalyze-0.3.0/PKG-INFO
```

### Comparing `psychoanalyze-0.2.2/LICENSE` & `psychoanalyze-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/README.md` & `psychoanalyze-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/__init__.py` & `psychoanalyze-0.3.0/psychoanalyze/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     subjects,
     stimulus,
     simulate,
 )
 
 pd.options.plotting.backend = "plotly"
 
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 __all__ = [
     "schemas",
     "plot",
     "data",
     "trial",
     "blocks",
```

### Comparing `psychoanalyze-0.2.2/psychoanalyze/blocks.py` & `psychoanalyze-0.3.0/psychoanalyze/blocks.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/data.py` & `psychoanalyze-0.3.0/psychoanalyze/data.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/layout.py` & `psychoanalyze-0.3.0/psychoanalyze/layout.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/plot.py` & `psychoanalyze-0.3.0/psychoanalyze/plot.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/points.py` & `psychoanalyze-0.3.0/psychoanalyze/points.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/schemas.py` & `psychoanalyze-0.3.0/psychoanalyze/schemas.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/sessions.py` & `psychoanalyze-0.3.0/psychoanalyze/sessions.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/simulate.py` & `psychoanalyze-0.3.0/psychoanalyze/simulate.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/strength_duration.py` & `psychoanalyze-0.3.0/psychoanalyze/strength_duration.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/subjects.py` & `psychoanalyze-0.3.0/psychoanalyze/subjects.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/trials.py` & `psychoanalyze-0.3.0/psychoanalyze/trials.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/psychoanalyze/weber.py` & `psychoanalyze-0.3.0/psychoanalyze/weber.py`

 * *Files identical despite different names*

### Comparing `psychoanalyze-0.2.2/pyproject.toml` & `psychoanalyze-0.3.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "psychoanalyze"
-version = "0.2.2"
+version = "0.3.0"
 description = "A Pythonic analysis package for psychophysics data"
 authors = ["Ty Schlichenmeyer <t.schlic@wustl.edu>"]
 license = "GPL-3.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.3"
```

### Comparing `psychoanalyze-0.2.2/PKG-INFO` & `psychoanalyze-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: psychoanalyze
-Version: 0.2.2
+Version: 0.3.0
 Summary: A Pythonic analysis package for psychophysics data
 License: GPL-3.0-or-later
 Author: Ty Schlichenmeyer
 Author-email: t.schlic@wustl.edu
 Requires-Python: ==3.11.3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

