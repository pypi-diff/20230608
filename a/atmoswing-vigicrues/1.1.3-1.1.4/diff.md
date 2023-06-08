# Comparing `tmp/atmoswing-vigicrues-1.1.3.tar.gz` & `tmp/atmoswing-vigicrues-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "atmoswing-vigicrues-1.1.3.tar", last modified: Sat May 20 13:18:21 2023, max compression
+gzip compressed data, was "atmoswing-vigicrues-1.1.4.tar", last modified: Thu Jun  8 20:28:56 2023, max compression
```

## Comparing `atmoswing-vigicrues-1.1.3.tar` & `atmoswing-vigicrues-1.1.4.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-20 13:18:21.045803 atmoswing-vigicrues-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.037803 atmoswing-vigicrues-1.1.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.037803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/dissemination.py
--rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/postaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8123 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/preaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     8105 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
--rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-20 13:18:21.000000 atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 13:18:21.041803 atmoswing-vigicrues-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_download_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_export_bdapbp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_export_prv.py
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_in.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_out.py
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_transform_gfs.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-20 13:18:02.000000 atmoswing-vigicrues-1.1.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.488468 atmoswing-vigicrues-1.1.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.488468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11414 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/dissemination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4866 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8460 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/postaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/preaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8269 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3602 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3316 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.488468 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 20:28:56.000000 atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 20:28:56.492468 atmoswing-vigicrues-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6878 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2972 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_download_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_export_bdapbp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_export_prv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3208 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_in.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_out.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_transform_gfs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-06-08 20:28:37.000000 atmoswing-vigicrues-1.1.4/tests/test_utils.py
```

### Comparing `atmoswing-vigicrues-1.1.3/LICENSE` & `atmoswing-vigicrues-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/PKG-INFO` & `atmoswing-vigicrues-1.1.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.3
+Version: 1.1.4
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atmoswing-vigicrues-1.1.3/README.md` & `atmoswing-vigicrues-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/pyproject.toml` & `atmoswing-vigicrues-1.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "atmoswing-vigicrues"
-version = "1.1.3"
+version = "1.1.4"
 authors = [
   { name="Pascal Horton", email="pascal.horton@terranum.ch" },
 ]
 description = "Package to integrate AtmoSwing in the Vigicrues network."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__init__.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__init__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/__main__.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/__main__.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/controller.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/dissemination.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/dissemination.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/disseminations/transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/exceptions.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/options.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_bdapbp.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/export_prv.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/postactions/postaction.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/postactions/postaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/download_gfs.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/download_gfs.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,21 +144,24 @@
             sub_product = 'pgrb2full'
 
         files_count = 0
         for time_step_back in range(0, self.time_step_back):
             date_ref = date - datetime.timedelta(
                 hours=self.time_increment * time_step_back
             )
+
+            date_msg = date_ref.strftime('%d/%m/%Y %Hh')
+            print(f"  -> Téléchargement des prévisions du : {date_msg}.")
+            forecast_date, forecast_hour = self._format_forecast_date(date_ref)
+
             for lead_time in range(0, self.lead_time_max + 1, 6):
                 lead_time_str = f'{lead_time:03d}'
 
                 for variable in self.variables:
 
-                    forecast_date, forecast_hour = self._format_forecast_date(date_ref)
-
                     url = f"https://nomads.ncep.noaa.gov/cgi-bin/filter_gfs_{resol}." \
                           f"pl?file=gfs.t{forecast_hour}z.{sub_product}.{resol}." \
                           f"f{lead_time_str}&{levels}var_{variable.upper()}=on&" \
                           f"{subregion}&dir=%2Fgfs.{forecast_date}%2F" \
                           f"{forecast_hour}%2Fatmos"
 
                     file_name = f'{forecast_date}{forecast_hour}.NWS_GFS.' \
```

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/preaction.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/preaction.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transfer_sftp_in.py`

 * *Files 3% similar despite different names*

```diff
@@ -113,28 +113,29 @@
 
             # Change the directory to the desired remote directory
             sftp.chdir(self.remote_dir)
 
             # Download files
             local_path = Path(self._get_local_path(date))
             forecast_datetime = date.strftime("%Y%m%d%H")
-            files_count_dt = self._get_files(sftp, forecast_datetime, local_path)
-            if files_count_dt == 0:
+            f_exist_dt, f_new_dt = self._get_files(sftp, forecast_datetime, local_path)
+
+            if f_exist_dt + f_new_dt == 0:
                 print(f"  -> Pas de fichier disponible pour {forecast_datetime}.")
                 return False
 
             forecast_date = date.strftime("%Y%m%d")
-            files_count_d = self._get_files(sftp, forecast_date, local_path)
+            f_exist_d, f_new_d = self._get_files(sftp, forecast_date, local_path)
 
             # Close the SFTP client and transport objects
             sftp.close()
             transport.close()
 
-            files_count = files_count_dt + files_count_d
-            print(f"  -> Nombre de fichiers récupérés : {files_count}.")
+            print(f"  -> Nombre de fichiers existants : {f_exist_d - f_new_dt}.")
+            print(f"  -> Nombre de fichiers récupérés : {f_new_dt + f_new_d}.")
 
         except paramiko.ssh_exception.PasswordRequiredException as e:
             print(f"SFTP PasswordRequiredException {e}")
             return False
         except paramiko.ssh_exception.BadAuthenticationType as e:
             print(f"SFTP BadAuthenticationType {e}")
             return False
@@ -156,33 +157,35 @@
         except Exception as e:
             print(f"Le rapatriement des données par SFTP a échoué ({e}).")
             return False
 
         return True
 
     def _get_files(self, sftp, forecast_date, local_path):
-        files_count = 0
+        files_count_existing = 0
+        files_count_new = 0
         for remote_file in sftp.listdir('.'):
             pattern = f'{self.prefix.lower()}*_{forecast_date}*.*'
             if self.variables is not None:
                 for variable in self.variables:
                     pattern = f'{self.prefix.lower()}_{variable.lower()}' \
                               f'_{forecast_date}*.*'
                     if fnmatch.fnmatch(remote_file.lower(), pattern):
                         break
 
             if fnmatch.fnmatch(remote_file.lower(), pattern):
                 local_file = local_path / remote_file
                 if local_file.exists():
+                    files_count_existing += 1
                     continue
                 sftp.get(remote_file, str(local_file), prefetch=False)
                 self._unpack_if_needed(local_file, local_path)
-                files_count += 1
+                files_count_new += 1
 
-        return files_count
+        return files_count_existing, files_count_new
 
     @staticmethod
     def _chdir_or_mkdir(dir_path, sftp):
         try:
             sftp.chdir(dir_path)
         except OSError:
             sftp.mkdir(dir_path)
```

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_ecmwf.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_ecmwf.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/preactions/transform_gfs.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/preactions/transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues/utils.py` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues/utils.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/PKG-INFO` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: atmoswing-vigicrues
-Version: 1.1.3
+Version: 1.1.4
 Summary: Package to integrate AtmoSwing in the Vigicrues network.
 Author: Pascal Horton
 Author-email: Pascal Horton <pascal.horton@terranum.ch>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `atmoswing-vigicrues-1.1.3/src/atmoswing_vigicrues.egg-info/SOURCES.txt` & `atmoswing-vigicrues-1.1.4/src/atmoswing_vigicrues.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_controller.py` & `atmoswing-vigicrues-1.1.4/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_download_gfs.py` & `atmoswing-vigicrues-1.1.4/tests/test_download_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_exceptions.py` & `atmoswing-vigicrues-1.1.4/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_export_bdapbp.py` & `atmoswing-vigicrues-1.1.4/tests/test_export_bdapbp.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_export_prv.py` & `atmoswing-vigicrues-1.1.4/tests/test_export_prv.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_options.py` & `atmoswing-vigicrues-1.1.4/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_in.py` & `atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_in.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_transfer_sftp_out.py` & `atmoswing-vigicrues-1.1.4/tests/test_transfer_sftp_out.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_transform_gfs.py` & `atmoswing-vigicrues-1.1.4/tests/test_transform_gfs.py`

 * *Files identical despite different names*

### Comparing `atmoswing-vigicrues-1.1.3/tests/test_utils.py` & `atmoswing-vigicrues-1.1.4/tests/test_utils.py`

 * *Files identical despite different names*

