# Comparing `tmp/pubpypack-harmony-bill-melvin-0.0.1.tar.gz` & `tmp/pubpypack-harmony-bill-melvin-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pubpypack-harmony-bill-melvin-0.0.1.tar", last modified: Thu Jun  8 12:52:13 2023, max compression
+gzip compressed data, was "pubpypack-harmony-bill-melvin-0.0.2.tar", last modified: Thu Jun  8 13:00:37 2023, max compression
```

## Comparing `pubpypack-harmony-bill-melvin-0.0.1.tar` & `pubpypack-harmony-bill-melvin-0.0.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.548486 pubpypack-harmony-bill-melvin-0.0.1/
--rw-rw-r--   0 bill      (1000) bill      (1000)     1071 2023-04-06 23:40:32.000000 pubpypack-harmony-bill-melvin-0.0.1/LICENSE
--rw-rw-r--   0 bill      (1000) bill      (1000)       50 2023-04-09 12:50:08.000000 pubpypack-harmony-bill-melvin-0.0.1/MANIFEST.in
--rw-rw-r--   0 bill      (1000) bill      (1000)      600 2023-06-08 12:52:13.548486 pubpypack-harmony-bill-melvin-0.0.1/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)      171 2023-06-08 12:42:19.000000 pubpypack-harmony-bill-melvin-0.0.1/README.md
--rw-rw-r--   0 bill      (1000) bill      (1000)      167 2023-06-03 20:42:44.000000 pubpypack-harmony-bill-melvin-0.0.1/pyproject.toml
--rw-rw-r--   0 bill      (1000) bill      (1000)     1894 2023-06-08 12:52:13.552486 pubpypack-harmony-bill-melvin-0.0.1/setup.cfg
--rw-rw-r--   0 bill      (1000) bill      (1000)      145 2023-04-16 11:29:27.000000 pubpypack-harmony-bill-melvin-0.0.1/setup.py
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.536486 pubpypack-harmony-bill-melvin-0.0.1/src/
--rw-r--r--   0 bill      (1000) bill      (1000)    53248 2023-05-07 17:33:39.000000 pubpypack-harmony-bill-melvin-0.0.1/src/.coverage
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.540485 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/
--rw-rw-r--   0 bill      (1000) bill      (1000)      529 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)      660 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/SOURCES.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        1 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/dependency_links.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       48 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/entry_points.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       20 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/requires.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        7 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/top_level.txt
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.544486 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/
--rw-rw-r--   0 bill      (1000) bill      (1000)        2 2023-04-09 12:26:04.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/__init__.py
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.548486 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/__pycache__/
--rw-rw-r--   0 bill      (1000) bill      (1000)      186 2023-05-13 00:28:43.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/__pycache__/__init__.cpython-310.pyc
--rw-rw-r--   0 bill      (1000) bill      (1000)      769 2023-05-13 00:28:43.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/__pycache__/harmony.cpython-310.pyc
--rw-rw-r--   0 bill      (1000) bill      (1000)       19 2023-04-09 12:45:01.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/data.json
--rw-rw-r--   0 bill      (1000) bill      (1000)   146334 2023-04-25 13:38:37.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/harmonic_mean.c
--rw-rw-r--   0 bill      (1000) bill      (1000)      252 2023-04-25 13:38:01.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/harmonic_mean.pyx
--rw-rw-r--   0 bill      (1000) bill      (1000)      612 2023-06-02 20:07:19.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/harmony.py
--rw-rw-r--   0 bill      (1000) bill      (1000)        2 2023-06-02 20:16:27.000000 pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/py.typed
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.548486 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/
--rw-rw-r--   0 bill      (1000) bill      (1000)      600 2023-06-08 12:52:13.000000 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/PKG-INFO
--rw-rw-r--   0 bill      (1000) bill      (1000)     1004 2023-06-08 12:52:13.000000 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/SOURCES.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        1 2023-06-08 12:52:13.000000 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/dependency_links.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       48 2023-06-08 12:52:13.000000 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/entry_points.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)       20 2023-06-08 12:52:13.000000 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/requires.txt
--rw-rw-r--   0 bill      (1000) bill      (1000)        7 2023-06-08 12:52:13.000000 pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/top_level.txt
-drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 12:52:13.548486 pubpypack-harmony-bill-melvin-0.0.1/test/
--rw-rw-r--   0 bill      (1000) bill      (1000)      471 2023-06-03 20:27:47.000000 pubpypack-harmony-bill-melvin-0.0.1/test/test_harmonic_mean.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1071 2023-04-06 23:40:32.000000 pubpypack-harmony-bill-melvin-0.0.2/LICENSE
+-rw-rw-r--   0 bill      (1000) bill      (1000)       50 2023-04-09 12:50:08.000000 pubpypack-harmony-bill-melvin-0.0.2/MANIFEST.in
+-rw-rw-r--   0 bill      (1000) bill      (1000)      618 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)      189 2023-06-08 12:55:39.000000 pubpypack-harmony-bill-melvin-0.0.2/README.md
+-rw-rw-r--   0 bill      (1000) bill      (1000)      167 2023-06-03 20:42:44.000000 pubpypack-harmony-bill-melvin-0.0.2/pyproject.toml
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1894 2023-06-08 13:00:37.137678 pubpypack-harmony-bill-melvin-0.0.2/setup.cfg
+-rw-rw-r--   0 bill      (1000) bill      (1000)      145 2023-04-16 11:29:27.000000 pubpypack-harmony-bill-melvin-0.0.2/setup.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.125678 pubpypack-harmony-bill-melvin-0.0.2/src/
+-rw-r--r--   0 bill      (1000) bill      (1000)    53248 2023-05-07 17:33:39.000000 pubpypack-harmony-bill-melvin-0.0.2/src/.coverage
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.129678 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/
+-rw-rw-r--   0 bill      (1000) bill      (1000)      529 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)      660 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/SOURCES.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        1 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/dependency_links.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       48 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/entry_points.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       20 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/requires.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        7 2023-06-03 20:28:31.000000 pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/top_level.txt
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.129678 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/
+-rw-rw-r--   0 bill      (1000) bill      (1000)        2 2023-04-09 12:26:04.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__init__.py
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.129678 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/
+-rw-rw-r--   0 bill      (1000) bill      (1000)      186 2023-05-13 00:28:43.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/__init__.cpython-310.pyc
+-rw-rw-r--   0 bill      (1000) bill      (1000)      769 2023-05-13 00:28:43.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/harmony.cpython-310.pyc
+-rw-rw-r--   0 bill      (1000) bill      (1000)       19 2023-04-09 12:45:01.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/data.json
+-rw-rw-r--   0 bill      (1000) bill      (1000)   146334 2023-04-25 13:38:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmonic_mean.c
+-rw-rw-r--   0 bill      (1000) bill      (1000)      252 2023-04-25 13:38:01.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmonic_mean.pyx
+-rw-rw-r--   0 bill      (1000) bill      (1000)      612 2023-06-02 20:07:19.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmony.py
+-rw-rw-r--   0 bill      (1000) bill      (1000)        2 2023-06-02 20:16:27.000000 pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/py.typed
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/
+-rw-rw-r--   0 bill      (1000) bill      (1000)      618 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/PKG-INFO
+-rw-rw-r--   0 bill      (1000) bill      (1000)     1004 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/SOURCES.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        1 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/dependency_links.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       48 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/entry_points.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)       20 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/requires.txt
+-rw-rw-r--   0 bill      (1000) bill      (1000)        7 2023-06-08 13:00:37.000000 pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/top_level.txt
+drwxrwxr-x   0 bill      (1000) bill      (1000)        0 2023-06-08 13:00:37.133678 pubpypack-harmony-bill-melvin-0.0.2/test/
+-rw-rw-r--   0 bill      (1000) bill      (1000)      471 2023-06-03 20:27:47.000000 pubpypack-harmony-bill-melvin-0.0.2/test/test_harmonic_mean.py
```

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/LICENSE` & `pubpypack-harmony-bill-melvin-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/setup.cfg` & `pubpypack-harmony-bill-melvin-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pubpypack-harmony-bill-melvin
-version = 0.0.1
+version = 0.0.2
 url = https://github.com/wmelvin/first-python-package
 author = Bill Melvin
 author_email = "Bill Melvin" <bill@billmelvin.com>
 description = Working the exercises in Publishing Python Packages by Dane Hillard
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
```

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/.coverage` & `pubpypack-harmony-bill-melvin-0.0.2/src/.coverage`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/PKG-INFO` & `pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/PKG-INFO`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/first_python_package.egg-info/SOURCES.txt` & `pubpypack-harmony-bill-melvin-0.0.2/src/first_python_package.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/__pycache__/harmony.cpython-310.pyc` & `pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/__pycache__/harmony.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/harmonic_mean.c` & `pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmonic_mean.c`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/imppkg/harmony.py` & `pubpypack-harmony-bill-melvin-0.0.2/src/imppkg/harmony.py`

 * *Files identical despite different names*

### Comparing `pubpypack-harmony-bill-melvin-0.0.1/src/pubpypack_harmony_bill_melvin.egg-info/SOURCES.txt` & `pubpypack-harmony-bill-melvin-0.0.2/src/pubpypack_harmony_bill_melvin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

