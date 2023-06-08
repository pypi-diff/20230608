# Comparing `tmp/tor_python_easy-0.1.6.tar.gz` & `tmp/tor_python_easy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tor_python_easy-0.1.6.tar", max compression
+gzip compressed data, was "tor_python_easy-0.1.7.tar", max compression
```

## Comparing `tor_python_easy-0.1.6.tar` & `tor_python_easy-0.1.7.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     1071 2023-06-08 17:20:00.891541 tor_python_easy-0.1.6/LICENSE.md
--rw-r--r--   0        0        0     2336 2023-06-08 17:20:00.891541 tor_python_easy-0.1.6/README.md
--rw-r--r--   0        0        0      471 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/tor_python_easy/__init__.py
--rw-r--r--   0        0        0     1340 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/tor_python_easy/tor_control_port_client.py
--rw-r--r--   0        0        0      359 2023-06-08 17:20:00.895541 tor_python_easy-0.1.6/tor_python_easy/tor_socks_get_ip_client.py
--rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 tor_python_easy-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-08 19:39:19.797217 tor_python_easy-0.1.7/LICENSE.md
+-rw-r--r--   0        0        0     2336 2023-06-08 19:39:19.797217 tor_python_easy-0.1.7/README.md
+-rw-r--r--   0        0        0      471 2023-06-08 19:39:19.801218 tor_python_easy-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-08 19:39:19.801218 tor_python_easy-0.1.7/tor_python_easy/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-08 19:39:19.801218 tor_python_easy-0.1.7/tor_python_easy/py.typed
+-rw-r--r--   0        0        0     1340 2023-06-08 19:39:19.801218 tor_python_easy-0.1.7/tor_python_easy/tor_control_port_client.py
+-rw-r--r--   0        0        0      359 2023-06-08 19:39:19.801218 tor_python_easy-0.1.7/tor_python_easy/tor_socks_get_ip_client.py
+-rw-r--r--   0        0        0     2972 1970-01-01 00:00:00.000000 tor_python_easy-0.1.7/PKG-INFO
```

### Comparing `tor_python_easy-0.1.6/LICENSE.md` & `tor_python_easy-0.1.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tor_python_easy-0.1.6/README.md` & `tor_python_easy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `tor_python_easy-0.1.6/tor_python_easy/tor_control_port_client.py` & `tor_python_easy-0.1.7/tor_python_easy/tor_control_port_client.py`

 * *Files identical despite different names*

### Comparing `tor_python_easy-0.1.6/PKG-INFO` & `tor_python_easy-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tor-python-easy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Simple library to manage tor proxy and IP changes
 Home-page: https://github.com/markowanga/tor-python-easy
 Author: Marcin Wątroba
 Author-email: markowanga@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

