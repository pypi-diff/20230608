# Comparing `tmp/magma_suite-1.5.0.1b19.tar.gz` & `tmp/magma_suite-1.5.0.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "magma_suite-1.5.0.1b19.tar", max compression
+gzip compressed data, was "magma_suite-1.5.0.1b8.tar", max compression
```

## Comparing `magma_suite-1.5.0.1b19.tar` & `magma_suite-1.5.0.1b8.tar`

### file list

```diff
@@ -1,27 +1,28 @@
--rw-r--r--   0        0        0     1083 2023-06-08 11:41:55.433089 magma_suite-1.5.0.1b19/LICENSE.txt
--rw-r--r--   0        0        0       96 2023-06-08 11:41:55.433089 magma_suite-1.5.0.1b19/README.md
--rw-r--r--   0        0        0        1 2023-06-08 11:41:55.433089 magma_suite-1.5.0.1b19/magma/__init__.py
--rw-r--r--   0        0        0     3444 2023-06-08 11:41:55.433089 magma_suite-1.5.0.1b19/magma/checkstatus.py
--rw-r--r--   0        0        0    12922 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma/inputgenerator.py
--rw-r--r--   0        0        0    15898 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma/metawfl.py
--rw-r--r--   0        0        0     8908 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma/metawflrun.py
--rw-r--r--   0        0        0     4087 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma/runupdate.py
--rw-r--r--   0        0        0        0 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/__init__.py
--rw-r--r--   0        0        0     2391 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/checkstatus.py
--rw-r--r--   0        0        0        0 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/commands/__init__.py
--rw-r--r--   0        0        0     1229 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/commands/create_meta_workflow_run.py
--rw-r--r--   0        0        0    53452 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/create_metawfr.py
--rw-r--r--   0        0        0     6670 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/import_metawfr.py
--rw-r--r--   0        0        0     5097 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/inputgenerator.py
--rw-r--r--   0        0        0      778 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/metawfl.py
--rw-r--r--   0        0        0     3162 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/metawflrun.py
--rw-r--r--   0        0        0     5032 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/parser.py
--rw-r--r--   0        0        0     6915 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/reset_metawfr.py
--rw-r--r--   0        0        0     2465 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/run_metawfr.py
--rw-r--r--   0        0        0       30 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/runupdate.py
--rw-r--r--   0        0        0     5650 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/status_metawfr.py
--rw-r--r--   0        0        0     1398 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/update_cost_metawfr.py
--rw-r--r--   0        0        0     3843 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/utils.py
--rw-r--r--   0        0        0     4066 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/magma_ff/wfrutils.py
--rw-r--r--   0        0        0     1038 2023-06-08 11:41:55.437089 magma_suite-1.5.0.1b19/pyproject.toml
--rw-r--r--   0        0        0      849 1970-01-01 00:00:00.000000 magma_suite-1.5.0.1b19/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-17 13:06:49.055030 magma_suite-1.5.0.1b8/LICENSE.txt
+-rw-r--r--   0        0        0       96 2023-04-17 13:06:49.055168 magma_suite-1.5.0.1b8/README.md
+-rw-r--r--   0        0        0        1 2023-04-17 13:06:49.056496 magma_suite-1.5.0.1b8/magma/__init__.py
+-rw-r--r--   0        0        0     3444 2023-04-17 13:06:49.056599 magma_suite-1.5.0.1b8/magma/checkstatus.py
+-rw-r--r--   0        0        0    12922 2023-04-17 13:06:49.056747 magma_suite-1.5.0.1b8/magma/inputgenerator.py
+-rw-r--r--   0        0        0    15898 2023-04-17 13:06:49.056890 magma_suite-1.5.0.1b8/magma/metawfl.py
+-rw-r--r--   0        0        0     8908 2023-04-17 13:06:49.057016 magma_suite-1.5.0.1b8/magma/metawflrun.py
+-rw-r--r--   0        0        0     4087 2023-04-17 13:06:49.057111 magma_suite-1.5.0.1b8/magma/runupdate.py
+-rw-r--r--   0        0        0        0 2023-04-17 13:06:49.057170 magma_suite-1.5.0.1b8/magma_ff/__init__.py
+-rw-r--r--   0        0        0     2391 2023-06-02 15:40:57.870914 magma_suite-1.5.0.1b8/magma_ff/checkstatus.py
+-rw-r--r--   0        0        0        0 2023-05-17 18:56:40.284445 magma_suite-1.5.0.1b8/magma_ff/commands/__init__.py
+-rw-r--r--   0        0        0     1229 2023-05-17 18:56:40.284626 magma_suite-1.5.0.1b8/magma_ff/commands/create_meta_workflow_run.py
+-rw-r--r--   0        0        0    53452 2023-05-17 18:56:40.285676 magma_suite-1.5.0.1b8/magma_ff/create_metawfr.py
+-rw-r--r--   0        0        0     6670 2023-04-17 13:06:49.057654 magma_suite-1.5.0.1b8/magma_ff/import_metawfr.py
+-rw-r--r--   0        0        0     5097 2023-04-17 13:06:49.057752 magma_suite-1.5.0.1b8/magma_ff/inputgenerator.py
+-rw-r--r--   0        0        0      778 2023-04-17 13:06:49.057830 magma_suite-1.5.0.1b8/magma_ff/metawfl.py
+-rw-r--r--   0        0        0     3162 2023-04-17 13:06:49.057893 magma_suite-1.5.0.1b8/magma_ff/metawflrun.py
+-rw-r--r--   0        0        0     5032 2023-04-17 13:06:49.058001 magma_suite-1.5.0.1b8/magma_ff/parser.py
+-rw-r--r--   0        0        0     6915 2023-04-17 13:06:49.058109 magma_suite-1.5.0.1b8/magma_ff/reset_metawfr.py
+-rw-r--r--   0        0        0     2465 2023-04-17 13:06:49.058190 magma_suite-1.5.0.1b8/magma_ff/run_metawfr.py
+-rw-r--r--   0        0        0       30 2023-04-17 13:06:49.058247 magma_suite-1.5.0.1b8/magma_ff/runupdate.py
+-rw-r--r--   0        0        0     5650 2023-04-17 13:06:49.058329 magma_suite-1.5.0.1b8/magma_ff/status_metawfr.py
+-rw-r--r--   0        0        0     1398 2023-04-17 13:06:49.058411 magma_suite-1.5.0.1b8/magma_ff/update_cost_metawfr.py
+-rw-r--r--   0        0        0     3843 2023-06-02 15:40:57.871181 magma_suite-1.5.0.1b8/magma_ff/utils.py
+-rw-r--r--   0        0        0     4066 2023-06-02 15:40:57.871562 magma_suite-1.5.0.1b8/magma_ff/wfrutils.py
+-rw-r--r--   0        0        0     1037 2023-06-02 16:22:59.429419 magma_suite-1.5.0.1b8/pyproject.toml
+-rw-r--r--   0        0        0     1133 1970-01-01 00:00:00.000000 magma_suite-1.5.0.1b8/setup.py
+-rw-r--r--   0        0        0      896 1970-01-01 00:00:00.000000 magma_suite-1.5.0.1b8/PKG-INFO
```

### Comparing `magma_suite-1.5.0.1b19/LICENSE.txt` & `magma_suite-1.5.0.1b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma/checkstatus.py` & `magma_suite-1.5.0.1b8/magma/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma/inputgenerator.py` & `magma_suite-1.5.0.1b8/magma/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma/metawfl.py` & `magma_suite-1.5.0.1b8/magma/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma/metawflrun.py` & `magma_suite-1.5.0.1b8/magma/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma/runupdate.py` & `magma_suite-1.5.0.1b8/magma/runupdate.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/checkstatus.py` & `magma_suite-1.5.0.1b8/magma_ff/checkstatus.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/commands/create_meta_workflow_run.py` & `magma_suite-1.5.0.1b8/magma_ff/commands/create_meta_workflow_run.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/create_metawfr.py` & `magma_suite-1.5.0.1b8/magma_ff/create_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/import_metawfr.py` & `magma_suite-1.5.0.1b8/magma_ff/import_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/inputgenerator.py` & `magma_suite-1.5.0.1b8/magma_ff/inputgenerator.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/metawfl.py` & `magma_suite-1.5.0.1b8/magma_ff/metawfl.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/metawflrun.py` & `magma_suite-1.5.0.1b8/magma_ff/metawflrun.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/parser.py` & `magma_suite-1.5.0.1b8/magma_ff/parser.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/reset_metawfr.py` & `magma_suite-1.5.0.1b8/magma_ff/reset_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/run_metawfr.py` & `magma_suite-1.5.0.1b8/magma_ff/run_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/status_metawfr.py` & `magma_suite-1.5.0.1b8/magma_ff/status_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/update_cost_metawfr.py` & `magma_suite-1.5.0.1b8/magma_ff/update_cost_metawfr.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/utils.py` & `magma_suite-1.5.0.1b8/magma_ff/utils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/magma_ff/wfrutils.py` & `magma_suite-1.5.0.1b8/magma_ff/wfrutils.py`

 * *Files identical despite different names*

### Comparing `magma_suite-1.5.0.1b19/pyproject.toml` & `magma_suite-1.5.0.1b8/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "magma-suite"
-version = "1.5.0.1b19"  # to become 1.5.0
+version = "1.5.0.1b8"  # to become 1.5.0
 description = "Collection of tools to manage meta-workflows automation."
 authors = ["Michele Berselli <berselli.michele@gmail.com>", "Doug Rioux", "Soo Lee", "CGAP team"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/dbmi-bgm/magma"
 homepage = "https://github.com/dbmi-bgm/magma"
 classifiers = [
```

### Comparing `magma_suite-1.5.0.1b19/PKG-INFO` & `magma_suite-1.5.0.1b8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: magma-suite
-Version: 1.5.0.1b19
+Version: 1.5.0.1b8
 Summary: Collection of tools to manage meta-workflows automation.
 Home-page: https://github.com/dbmi-bgm/magma
 License: MIT
 Author: Michele Berselli
 Author-email: berselli.michele@gmail.com
 Requires-Python: >=3.7,<3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Requires-Dist: dcicutils (>=7.5.0,<8.0.0)
 Requires-Dist: tibanna-ff (>=1.3.3,<2.0.0)
 Project-URL: Repository, https://github.com/dbmi-bgm/magma
 Description-Content-Type: text/markdown
 
 # magma
```

