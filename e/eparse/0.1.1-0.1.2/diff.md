# Comparing `tmp/eparse-0.1.1.tar.gz` & `tmp/eparse-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eparse-0.1.1.tar", last modified: Wed Jun  7 02:09:11 2023, max compression
+gzip compressed data, was "eparse-0.1.2.tar", last modified: Thu Jun  8 01:24:39 2023, max compression
```

## Comparing `eparse-0.1.1.tar` & `eparse-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-07 02:09:11.614096 eparse-0.1.1/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-07 01:04:55.000000 eparse-0.1.1/AUTHORS.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-07 01:07:07.000000 eparse-0.1.1/CONTRIBUTING.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       89 2023-06-07 00:07:19.000000 eparse-0.1.1/HISTORY.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-07 00:07:19.000000 eparse-0.1.1/LICENSE
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-07 00:07:19.000000 eparse-0.1.1/MANIFEST.in
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1676 2023-06-07 02:09:11.614096 eparse-0.1.1/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      897 2023-06-07 00:07:19.000000 eparse-0.1.1/README.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-07 02:09:11.614096 eparse-0.1.1/docs/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/Makefile
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/authors.rst
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/conf.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/contributing.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/history.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/index.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/installation.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/make.bat
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/readme.rst
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-07 00:07:19.000000 eparse-0.1.1/docs/usage.rst
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-07 02:09:11.614096 eparse-0.1.1/eparse/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      128 2023-06-07 02:04:42.000000 eparse-0.1.1/eparse/__init__.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9287 2023-06-07 01:46:24.000000 eparse-0.1.1/eparse/cli.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4115 2023-06-07 01:48:16.000000 eparse-0.1.1/eparse/core.py
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2745 2023-06-07 01:48:46.000000 eparse-0.1.1/eparse/interfaces.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-07 02:09:11.614096 eparse-0.1.1/eparse.egg-info/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1676 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/PKG-INFO
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      605 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/SOURCES.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/dependency_links.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/entry_points.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/not-zip-safe
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/requires.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-07 02:09:11.000000 eparse-0.1.1/eparse.egg-info/top_level.txt
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      423 2023-06-07 02:09:11.614096 eparse-0.1.1/setup.cfg
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-07 02:04:20.000000 eparse-0.1.1/setup.py
-drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-07 02:09:11.614096 eparse-0.1.1/tests/
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-07 00:07:19.000000 eparse-0.1.1/tests/__init__.py
--rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-07 01:34:28.000000 eparse-0.1.1/tests/eparse_unit_test_data.xlsx
--rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      384 2023-06-07 01:39:21.000000 eparse-0.1.1/tests/test_core.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      133 2023-06-08 00:46:57.000000 eparse-0.1.2/AUTHORS.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     3353 2023-06-08 00:46:57.000000 eparse-0.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      169 2023-06-08 01:13:37.000000 eparse-0.1.2/HISTORY.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1075 2023-06-08 00:46:57.000000 eparse-0.1.2/LICENSE
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      262 2023-06-08 00:46:57.000000 eparse-0.1.2/MANIFEST.in
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9501 2023-06-08 01:24:39.622284 eparse-0.1.2/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     8642 2023-06-08 01:12:11.000000 eparse-0.1.2/README.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/docs/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      607 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/Makefile
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/authors.rst
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)     4777 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/conf.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       33 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/contributing.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       28 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/history.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      303 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/index.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1134 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/installation.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      804 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/make.bat
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       27 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/readme.rst
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       67 2023-06-08 00:46:57.000000 eparse-0.1.2/docs/usage.rst
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/eparse/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      126 2023-06-08 01:16:11.000000 eparse-0.1.2/eparse/__init__.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9287 2023-06-08 00:46:57.000000 eparse-0.1.2/eparse/cli.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     4115 2023-06-08 00:46:57.000000 eparse-0.1.2/eparse/core.py
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     2745 2023-06-08 00:46:57.000000 eparse-0.1.2/eparse/interfaces.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/eparse.egg-info/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     9501 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/PKG-INFO
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      605 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/SOURCES.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/dependency_links.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       50 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/entry_points.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        1 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/not-zip-safe
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       58 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/requires.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)        7 2023-06-08 01:24:39.000000 eparse-0.1.2/eparse.egg-info/top_level.txt
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      423 2023-06-08 01:24:39.622284 eparse-0.1.2/setup.cfg
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)     1513 2023-06-08 01:15:23.000000 eparse-0.1.2/setup.py
+drwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)        0 2023-06-08 01:24:39.622284 eparse-0.1.2/tests/
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)       36 2023-06-08 00:46:57.000000 eparse-0.1.2/tests/__init__.py
+-rwxr-xr-x   0 cpappalardo  (1000) cpappalardo  (1000)    14990 2023-06-08 00:46:57.000000 eparse-0.1.2/tests/eparse_unit_test_data.xlsx
+-rw-r--r--   0 cpappalardo  (1000) cpappalardo  (1000)      384 2023-06-08 00:46:57.000000 eparse-0.1.2/tests/test_core.py
```

### Comparing `eparse-0.1.1/CONTRIBUTING.rst` & `eparse-0.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/LICENSE` & `eparse-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/docs/Makefile` & `eparse-0.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/docs/conf.py` & `eparse-0.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/docs/installation.rst` & `eparse-0.1.2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/docs/make.bat` & `eparse-0.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/eparse/cli.py` & `eparse-0.1.2/eparse/cli.py`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/eparse/core.py` & `eparse-0.1.2/eparse/core.py`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/eparse/interfaces.py` & `eparse-0.1.2/eparse/interfaces.py`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/eparse.egg-info/SOURCES.txt` & `eparse-0.1.2/eparse.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `eparse-0.1.1/setup.py` & `eparse-0.1.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
     'pytest',
     'tox',
 ]
 
 setup(
     author='Chris Pappalardo',
     author_email='cpappala@gmail.com',
-    python_requires='>=3.6',
+    python_requires='>=3.9',
     classifiers=[
         'Development Status :: 2 - Pre-Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.9',
@@ -54,10 +54,10 @@
     include_package_data=True,
     keywords='eparse',
     name='eparse',
     packages=find_packages(include=['eparse', 'eparse.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/ChrisPappalardo/eparse',
-    version='0.1.1',
+    version='0.1.2',
     zip_safe=False,
 )
```

### Comparing `eparse-0.1.1/tests/eparse_unit_test_data.xlsx` & `eparse-0.1.2/tests/eparse_unit_test_data.xlsx`

 * *Files identical despite different names*

