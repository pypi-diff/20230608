# Comparing `tmp/pyiron-0.4.7.tar.gz` & `tmp/pyiron-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiron-0.4.7.tar", last modified: Mon Oct 17 15:08:51 2022, max compression
+gzip compressed data, was "pyiron-0.5.0.tar", last modified: Thu Jun  8 03:39:06 2023, max compression
```

## Comparing `pyiron-0.4.7.tar` & `pyiron-0.5.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:08:51.421601 pyiron-0.4.7/
--rw-r--r--   0 runner    (1001) docker     (121)     1593 2022-10-17 15:08:48.000000 pyiron-0.4.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       65 2022-10-17 15:08:48.000000 pyiron-0.4.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-10-17 15:08:51.421601 pyiron-0.4.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     6003 2022-10-17 15:08:48.000000 pyiron-0.4.7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:08:51.421601 pyiron-0.4.7/pyiron/
--rw-r--r--   0 runner    (1001) docker     (121)     1553 2022-10-17 15:08:48.000000 pyiron-0.4.7/pyiron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      496 2022-10-17 15:08:51.421601 pyiron-0.4.7/pyiron/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-17 15:08:51.421601 pyiron-0.4.7/pyiron.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-10-17 15:08:51.000000 pyiron-0.4.7/pyiron.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      250 2022-10-17 15:08:51.000000 pyiron-0.4.7/pyiron.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-17 15:08:51.000000 pyiron-0.4.7/pyiron.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       26 2022-10-17 15:08:51.000000 pyiron-0.4.7/pyiron.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-10-17 15:08:51.000000 pyiron-0.4.7/pyiron.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-10-17 15:08:51.421601 pyiron-0.4.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1367 2022-10-17 15:08:51.000000 pyiron-0.4.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)    68611 2022-10-17 15:08:48.000000 pyiron-0.4.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:39:06.606850 pyiron-0.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-08 03:39:00.000000 pyiron-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 03:39:00.000000 pyiron-0.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 03:39:06.606850 pyiron-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5995 2023-06-08 03:39:00.000000 pyiron-0.5.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:39:06.606850 pyiron-0.5.0/pyiron/
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-06-08 03:39:00.000000 pyiron-0.5.0/pyiron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-06-08 03:39:06.606850 pyiron-0.5.0/pyiron/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 03:39:06.606850 pyiron-0.5.0/pyiron.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-08 03:39:06.000000 pyiron-0.5.0/pyiron.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 03:39:06.000000 pyiron-0.5.0/pyiron.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 03:39:06.000000 pyiron-0.5.0/pyiron.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 03:39:06.000000 pyiron-0.5.0/pyiron.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 03:39:06.000000 pyiron-0.5.0/pyiron.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-08 03:39:06.606850 pyiron-0.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-06-08 03:39:05.000000 pyiron-0.5.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-06-08 03:39:00.000000 pyiron-0.5.0/versioneer.py
```

### Comparing `pyiron-0.4.7/LICENSE` & `pyiron-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyiron-0.4.7/PKG-INFO` & `pyiron-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron
-Version: 0.4.7
+Version: 0.5.0
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron-0.4.7/README.rst` & `pyiron-0.5.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pyiron
 ======
 
-.. image:: https://coveralls.io/repos/github/pyiron/pyiron/badge.svg?branch=master
-    :target: https://coveralls.io/github/pyiron/pyiron?branch=master
+.. image:: https://coveralls.io/repos/github/pyiron/pyiron/badge.svg?branch=main
+    :target: https://coveralls.io/github/pyiron/pyiron?branch=main
     :alt: Coverage Status
 
 .. image:: https://api.codacy.com/project/badge/Grade/c513254f10004df5a1f5c76425c6584b
     :target: https://app.codacy.com/app/pyiron-runner/pyiron?utm_source=github.com&utm_medium=referral&utm_content=pyiron/pyiron&utm_campaign=Badge_Grade_Settings
     :alt: Codacy Badge
 
 .. image:: https://anaconda.org/conda-forge/pyiron/badges/latest_release_date.svg
@@ -48,15 +48,15 @@
    **pyiron**: This is the documentation page for the pyiron meta package, that combines the other packages in a common
    interface.  The API documentation for `pyiron_base <https://pyiron_base.readthedocs.io/en/latest/>`_ and
    `pyiron_atomistics <https://pyiron_atomistics.readthedocs.io/en/latest/>`_ are available as separate pages.
 
 
 Installation
 ------------
-You can test pyiron on `Mybinder.org (beta) <https://mybinder.org/v2/gh/pyiron/pyiron/master?urlpath=lab>`_.
+You can test pyiron on `Mybinder.org (beta) <https://mybinder.org/v2/gh/pyiron/pyiron/main?urlpath=lab>`_.
 For a local installation we recommend to install pyiron inside an `anaconda <https://www.anaconda.com>`_  environment::
 
     conda install -c conda-forge pyiron
 
 
 After the installation of pyiron you need to configure pyiron. The default configuration can be generated automatically. Start a new Python session and import pyiron::
 
@@ -93,15 +93,15 @@
 
 
 Getting started:
 ----------------
 Test pyiron with mybinder:
 
 .. image:: https://mybinder.org/badge_logo.svg
-     :target: https://mybinder.org/v2/gh/pyiron/pyiron/master
+     :target: https://mybinder.org/v2/gh/pyiron/pyiron/main
      :alt: mybinder
 
 
 License and Acknowledgments
 ---------------------------
 ``pyiron`` is licensed under the BSD license.
```

### Comparing `pyiron-0.4.7/pyiron/__init__.py` & `pyiron-0.5.0/pyiron/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiron-0.4.7/pyiron.egg-info/PKG-INFO` & `pyiron-0.5.0/pyiron.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiron
-Version: 0.4.7
+Version: 0.5.0
 Summary: pyiron - an integrated development environment (IDE) for computational materials science.
 Home-page: https://github.com/pyiron/pyiron
 Author: Max-Planck-Institut für Eisenforschung GmbH - Computational Materials Design (CM) Department
 Author-email: janssen@mpie.de
 License: BSD
 Keywords: pyiron
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `pyiron-0.4.7/setup.py` & `pyiron-0.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,12 +25,12 @@
                  'Programming Language :: Python :: 3.8',
                  'Programming Language :: Python :: 3.9',
                  'Programming Language :: Python :: 3.10'],
 
     keywords='pyiron',
     packages=find_packages(exclude=["*tests*", "*docs*", "*binder*", "*conda*", "*notebooks*", "*.ci_support*"]),
     install_requires=[
-        'pyiron_atomistics>=0.2.58'
+        'pyiron_atomistics>=0.3.0'
     ],
     cmdclass=versioneer.get_cmdclass(),
 
     )
```

### Comparing `pyiron-0.4.7/versioneer.py` & `pyiron-0.5.0/versioneer.py`

 * *Files identical despite different names*

