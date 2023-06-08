# Comparing `tmp/py_dev_support-0.1.14.tar.gz` & `tmp/py_dev_support-0.1.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_dev_support-0.1.14.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "py_dev_support-0.1.15.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `py_dev_support-0.1.14.tar` & `py_dev_support-0.1.15.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2023-06-08 06:23:21.645584 py_dev_support-0.1.14/LICENSE
--rw-r--r--   0        0        0       48 2023-06-08 06:41:14.413449 py_dev_support-0.1.14/py_dev_support/__init__.py
--rw-r--r--   0        0        0      392 2023-06-08 07:05:37.377215 py_dev_support-0.1.14/py_dev_support/release.py
--rw-r--r--   0        0        0      895 2023-06-08 07:01:11.777248 py_dev_support-0.1.14/py_dev_support/version.py
--rw-r--r--   0        0        0      465 2023-06-08 07:13:04.129142 py_dev_support-0.1.14/pyproject.toml
--rw-r--r--   0        0        0      162 1970-01-01 00:00:00.000000 py_dev_support-0.1.14/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-08 06:23:21.645584 py_dev_support-0.1.15/LICENSE
+-rw-r--r--   0        0        0       48 2023-06-08 06:41:14.413449 py_dev_support-0.1.15/py_dev_support/__init__.py
+-rw-r--r--   0        0        0      392 2023-06-08 07:05:37.377215 py_dev_support-0.1.15/py_dev_support/release.py
+-rw-r--r--   0        0        0      895 2023-06-08 07:01:11.777248 py_dev_support-0.1.15/py_dev_support/version.py
+-rw-r--r--   0        0        0      469 2023-06-08 07:16:19.465102 py_dev_support-0.1.15/pyproject.toml
+-rw-r--r--   0        0        0      220 1970-01-01 00:00:00.000000 py_dev_support-0.1.15/PKG-INFO
```

### Comparing `py_dev_support-0.1.14/LICENSE` & `py_dev_support-0.1.15/LICENSE`

 * *Files identical despite different names*

### Comparing `py_dev_support-0.1.14/py_dev_support/version.py` & `py_dev_support-0.1.15/py_dev_support/version.py`

 * *Files identical despite different names*

