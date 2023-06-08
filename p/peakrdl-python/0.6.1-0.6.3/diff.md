# Comparing `tmp/peakrdl-python-0.6.1.tar.gz` & `tmp/peakrdl-python-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peakrdl-python-0.6.1.tar", last modified: Mon May  1 18:55:38 2023, max compression
+gzip compressed data, was "peakrdl-python-0.6.3.tar", last modified: Thu Jun  8 18:15:12 2023, max compression
```

## Comparing `peakrdl-python-0.6.1.tar` & `peakrdl-python-0.6.3.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.249189 peakrdl-python-0.6.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.253189 peakrdl-python-0.6.1/src/peakrdl_python/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/__peakrdl__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/_node_walkers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.253189 peakrdl-python-0.6.1/src/peakrdl_python/lib/
--rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/lib/register.py
--rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/peakpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/safe_name_utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/systemrdl_node_utility_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.257189 peakrdl-python-0.6.1/src/peakrdl_python/templates/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_field.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_memory.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_register.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_simulation.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
--rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/baseclass_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      146 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/header.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/header_tb.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-05-01 18:55:36.000000 peakrdl-python-0.6.1/src/peakrdl_python/templates/reg_definitions.py.jinja
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 18:55:38.253189 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-01 18:55:38.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-01 18:55:37.000000 peakrdl-python-0.6.1/src/peakrdl_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:12.269019 peakrdl-python-0.6.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-08 18:15:12.269019 peakrdl-python-0.6.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:15:12.269019 peakrdl-python-0.6.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:12.265018 peakrdl-python-0.6.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:12.265018 peakrdl-python-0.6.3/src/peakrdl_python/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2421 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/__peakrdl__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/_node_walkers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18175 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:12.269019 peakrdl-python-0.6.3/src/peakrdl_python/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/lib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6940 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/lib/callbacks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27632 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/lib/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/lib/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33744 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/lib/register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7317 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/peakpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10674 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/safe_name_utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10197 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/systemrdl_node_utility_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:12.269019 peakrdl-python-0.6.3/src/peakrdl_python/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21835 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_field.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5496 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_memory.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     8910 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_register.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_simulation.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_simulation_tb.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)    72721 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/baseclass_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      146 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/header.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/header_tb.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-06-08 18:15:10.000000 peakrdl-python-0.6.3/src/peakrdl_python/templates/reg_definitions.py.jinja
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:12.269019 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-06-08 18:15:11.000000 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-06-08 18:15:12.000000 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:15:11.000000 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-08 18:15:11.000000 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 18:15:11.000000 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 18:15:11.000000 peakrdl-python-0.6.3/src/peakrdl_python.egg-info/top_level.txt
```

### Comparing `peakrdl-python-0.6.1/LICENSE` & `peakrdl-python-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/PKG-INFO` & `peakrdl-python-0.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.6.1
+Version: 0.6.3
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
@@ -31,8 +31,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `peakrdl-python-0.6.1/README.md` & `peakrdl-python-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/setup.py` & `peakrdl-python-0.6.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     package_data={"peakrdl_python.templates": ["*.py.jinga"]},
     include_package_data = True,
     entry_points= { 'console_scripts' : ['peakrdl_python=peakrdl_python.peakpython:main_function'],
                     "peakrdl.exporters": [
                         'python = peakrdl_python.__peakrdl__:Exporter'
                     ]
                     },
+    python_requires='>=3.7, <4',
     install_requires=[
         "systemrdl-compiler>=1.24.0",
         "autopep8",
         "jinja2",
         "asynctest;python_version<'3.8'",
         "peakrdl-ipxact"
     ],
```

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/__peakrdl__.py` & `peakrdl-python-0.6.3/src/peakrdl_python/__peakrdl__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/_node_walkers.py` & `peakrdl-python-0.6.3/src/peakrdl_python/_node_walkers.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/exporter.py` & `peakrdl-python-0.6.3/src/peakrdl_python/exporter.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/lib/__init__.py` & `peakrdl-python-0.6.3/src/peakrdl_python/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/lib/base.py` & `peakrdl-python-0.6.3/src/peakrdl_python/lib/base.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/lib/callbacks.py` & `peakrdl-python-0.6.3/src/peakrdl_python/lib/callbacks.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/lib/fields.py` & `peakrdl-python-0.6.3/src/peakrdl_python/lib/fields.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/lib/memory.py` & `peakrdl-python-0.6.3/src/peakrdl_python/lib/memory.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/lib/register.py` & `peakrdl-python-0.6.3/src/peakrdl_python/lib/register.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/peakpython.py` & `peakrdl-python-0.6.3/src/peakrdl_python/peakpython.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/safe_name_utility.py` & `peakrdl-python-0.6.3/src/peakrdl_python/safe_name_utility.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/systemrdl_node_utility_functions.py` & `peakrdl-python-0.6.3/src/peakrdl_python/systemrdl_node_utility_functions.py`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_field.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_field.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_memory.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_memory.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_register.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_register.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/addrmap_tb.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/addrmap_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/baseclass_tb.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/baseclass_tb.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python/templates/reg_definitions.py.jinja` & `peakrdl-python-0.6.3/src/peakrdl_python/templates/reg_definitions.py.jinja`

 * *Files identical despite different names*

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python.egg-info/PKG-INFO` & `peakrdl-python-0.6.3/src/peakrdl_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peakrdl-python
-Version: 0.6.1
+Version: 0.6.3
 Summary: Generate python wrapper for a register model compiled SystemRDL input
 Home-page: https://github.com/krcb197/PeakRDL-python
 Author: Keith Brady
 License: UNKNOWN
 Project-URL: Source, https://github.com/krcb197/PeakRDL-python
 Project-URL: Tracker, https://github.com/krcb197/PeakRDL-python/issues
 Project-URL: Documentation, https://peakrdl-python.readthedocs.io/
@@ -31,8 +31,9 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
```

### Comparing `peakrdl-python-0.6.1/src/peakrdl_python.egg-info/SOURCES.txt` & `peakrdl-python-0.6.3/src/peakrdl_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

