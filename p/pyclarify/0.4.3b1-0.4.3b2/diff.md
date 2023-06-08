# Comparing `tmp/pyclarify-0.4.3b1.tar.gz` & `tmp/pyclarify-0.4.3b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pyclarify/pyclarify/dist/.tmp-csq9k27j/pyclarify-0.4.3b1.tar", last modified: Tue May  2 13:19:34 2023, max compression
+gzip compressed data, was "/home/runner/work/pyclarify/pyclarify/dist/.tmp-52t3g8g3/pyclarify-0.4.3b2.tar", last modified: Tue May  9 09:22:12 2023, max compression
```

## Comparing `pyclarify-0.4.3b1.tar` & `pyclarify-0.4.3b2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/auxiliary.py
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/pagination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/payload.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/stopping_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/__utils__/warnings.py
--rw-r--r--   0 runner    (1001) docker     (123)    42165 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/constraints.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/fields/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/jsonrpc/oauth2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/query/
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5442 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/query/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/query/query.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify/views/
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/generics.py
--rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/items.py
--rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/src/pyclarify/views/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/src/pyclarify.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 13:19:34.000000 pyclarify-0.4.3b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_insert.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_publish_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_save_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_select_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_select_items.py
--rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-02 13:19:10.000000 pyclarify-0.4.3b1/tests/test_client_select_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      846 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/auxiliary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8063 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/payload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/stopping_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/__utils__/warnings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42165 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2506 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/fields/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify/jsonrpc/
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/jsonrpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/jsonrpc/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/jsonrpc/oauth2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/query/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/query/query.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify/views/
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12522 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/views/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5745 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/views/generics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7722 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/views/items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6155 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/src/pyclarify/views/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/src/pyclarify.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 09:22:12.000000 pyclarify-0.4.3b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/tests/test_client_insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/tests/test_client_publish_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/tests/test_client_save_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5788 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/tests/test_client_select_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/tests/test_client_select_items.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3308 2023-05-09 09:21:46.000000 pyclarify-0.4.3b2/tests/test_client_select_signals.py
```

### Comparing `pyclarify-0.4.3b1/LICENSE` & `pyclarify-0.4.3b2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/LICENSE.txt` & `pyclarify-0.4.3b2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/PKG-INFO` & `pyclarify-0.4.3b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclarify
-Version: 0.4.3b1
+Version: 0.4.3b2
 Summary: Python SDK for reading and writing signals to Clarify.
 Home-page: https://github.com/clarify/pyclarify
 Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar Aspaas
 Author-email: alexia@clarify.io, eliezer@clarify.io, odd.gunnar@clarify.io
 Project-URL: Bug Tracker, https://github.com/clarify/pyclarify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b2 Summary: Python SDK for
 reading and writing signals to Clarify. Home-page: https://github.com/clarify/
 pyclarify Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar
 Aspaas Author-email: alexia@clarify.io, eliezer@clarify.io,
 odd.gunnar@clarify.io Project-URL: Bug Tracker, https://github.com/clarify/
 pyclarify/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `pyclarify-0.4.3b1/README.md` & `pyclarify-0.4.3b2/README.md`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/setup.cfg` & `pyclarify-0.4.3b2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__init__.py` & `pyclarify-0.4.3b2/src/pyclarify/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,9 +14,9 @@
 limitations under the License.
 """
 
 from pyclarify.client import Client
 from pyclarify.views import Signal, SignalInfo, Item, ItemInfo, DataFrame
 import pyclarify.query
 
-__version__ = "0.4.3b1"
+__version__ = "0.4.3b2"
 __API_version__ = "1.1beta2"
```

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/__init__.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/auxiliary.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/exceptions.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/pagination.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/pagination.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/payload.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/payload.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/time.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/time.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/__utils__/warnings.py` & `pyclarify-0.4.3b2/src/pyclarify/__utils__/warnings.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/client.py` & `pyclarify-0.4.3b2/src/pyclarify/client.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/fields/authentication.py` & `pyclarify-0.4.3b2/src/pyclarify/fields/authentication.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/fields/constraints.py` & `pyclarify-0.4.3b2/src/pyclarify/fields/constraints.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/fields/dataframe.py` & `pyclarify-0.4.3b2/src/pyclarify/fields/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/fields/error.py` & `pyclarify-0.4.3b2/src/pyclarify/fields/error.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/fields/query.py` & `pyclarify-0.4.3b2/src/pyclarify/fields/query.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/fields/resource.py` & `pyclarify-0.4.3b2/src/pyclarify/fields/resource.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/jsonrpc/client.py` & `pyclarify-0.4.3b2/src/pyclarify/jsonrpc/client.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/jsonrpc/oauth2.py` & `pyclarify-0.4.3b2/src/pyclarify/jsonrpc/oauth2.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/query/__init__.py` & `pyclarify-0.4.3b2/src/pyclarify/query/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/query/filter.py` & `pyclarify-0.4.3b2/src/pyclarify/query/filter.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 limitations under the License.
 """
 
 from pyclarify.fields.query import Comparison, DateField, Operators
 from pydantic.class_validators import root_validator
 from pydantic import BaseModel
 from pydantic.fields import Optional
+from pydantic.datetime_parse import parse_datetime
 from typing import ForwardRef, Union, List, Dict
 from datetime import datetime
 
 
 Filter = ForwardRef("Filter")
 
 
@@ -154,17 +155,17 @@
 
     @root_validator(pre=False, allow_reuse=True)
     def field_must_reflect_operator(cls, values):
         gte = values["gte"] if "gte" in values.keys() else None
         lt = values["lt"] if "lt" in values.keys() else None
 
         if gte:
-            values["gte"] = DateField(operator=Operators.GTE, time=gte)
+            values["gte"] = DateField(operator=Operators.GTE, time=parse_datetime(gte).astimezone().isoformat())
         if lt:
-            values["lt"] = DateField(operator=Operators.LT, time=lt)
+            values["lt"] = DateField(operator=Operators.LT, time=parse_datetime(lt).astimezone().isoformat())
 
         return values
 
     def to_query(self):
         q = {}
         if self.gte:
             gte = self.gte.dict()["query"]
```

### Comparing `pyclarify-0.4.3b1/src/pyclarify/query/query.py` & `pyclarify-0.4.3b2/src/pyclarify/query/query.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/views/__init__.py` & `pyclarify-0.4.3b2/src/pyclarify/views/__init__.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/views/dataframe.py` & `pyclarify-0.4.3b2/src/pyclarify/views/dataframe.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/views/generics.py` & `pyclarify-0.4.3b2/src/pyclarify/views/generics.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/views/items.py` & `pyclarify-0.4.3b2/src/pyclarify/views/items.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify/views/signals.py` & `pyclarify-0.4.3b2/src/pyclarify/views/signals.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/src/pyclarify.egg-info/PKG-INFO` & `pyclarify-0.4.3b2/src/pyclarify.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyclarify
-Version: 0.4.3b1
+Version: 0.4.3b2
 Summary: Python SDK for reading and writing signals to Clarify.
 Home-page: https://github.com/clarify/pyclarify
 Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar Aspaas
 Author-email: alexia@clarify.io, eliezer@clarify.io, odd.gunnar@clarify.io
 Project-URL: Bug Tracker, https://github.com/clarify/pyclarify/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b1 Summary: Python SDK for
+Metadata-Version: 2.1 Name: pyclarify Version: 0.4.3b2 Summary: Python SDK for
 reading and writing signals to Clarify. Home-page: https://github.com/clarify/
 pyclarify Author: Alexia Artemis Baikas, Eliezer de Souza da Silva, Odd Gunnar
 Aspaas Author-email: alexia@clarify.io, eliezer@clarify.io,
 odd.gunnar@clarify.io Project-URL: Bug Tracker, https://github.com/clarify/
 pyclarify/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.7 Description-Content-Type: text/markdown
```

### Comparing `pyclarify-0.4.3b1/src/pyclarify.egg-info/SOURCES.txt` & `pyclarify-0.4.3b2/src/pyclarify.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/tests/test_client_insert.py` & `pyclarify-0.4.3b2/tests/test_client_insert.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/tests/test_client_publish_signals.py` & `pyclarify-0.4.3b2/tests/test_client_publish_signals.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/tests/test_client_save_signals.py` & `pyclarify-0.4.3b2/tests/test_client_save_signals.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/tests/test_client_select_dataframe.py` & `pyclarify-0.4.3b2/tests/test_client_select_dataframe.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/tests/test_client_select_items.py` & `pyclarify-0.4.3b2/tests/test_client_select_items.py`

 * *Files identical despite different names*

### Comparing `pyclarify-0.4.3b1/tests/test_client_select_signals.py` & `pyclarify-0.4.3b2/tests/test_client_select_signals.py`

 * *Files identical despite different names*

