# Comparing `tmp/pytest-doctestplus-0.8.0.dev0.tar.gz` & `tmp/pytest-doctestplus-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pytest-doctestplus-0.8.0.dev0.tar", last modified: Fri Jul 31 20:58:46 2020, max compression
+gzip compressed data, was "pytest-doctestplus-0.9.0.tar", last modified: Fri Jan 15 01:19:55 2021, max compression
```

## Comparing `pytest-doctestplus-0.8.0.dev0.tar` & `pytest-doctestplus-0.9.0.tar`

### file list

```diff
@@ -1,33 +1,47 @@
-drwxr-sr-x   0 lim       (4661) ssb        (528)        0 2020-07-31 20:58:46.436920 pytest-doctestplus-0.8.0.dev0/
--rw-r--r--   0 lim       (4661) ssb        (528)     2832 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/CHANGES.rst
--rw-r--r--   0 lim       (4661) ssb        (528)     1496 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/LICENSE.rst
--rw-r--r--   0 lim       (4661) ssb        (528)      131 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/MANIFEST.in
--rw-r--r--   0 lim       (4661) ssb        (528)    13509 2020-07-31 20:58:46.437920 pytest-doctestplus-0.8.0.dev0/PKG-INFO
--rw-r--r--   0 lim       (4661) ssb        (528)    10344 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/README.rst
-drwxr-sr-x   0 lim       (4661) ssb        (528)        0 2020-07-31 20:58:46.434920 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/
--rw-r--r--   0 lim       (4661) ssb        (528)      178 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/__init__.py
--rw-r--r--   0 lim       (4661) ssb        (528)    11050 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/output_checker.py
--rw-r--r--   0 lim       (4661) ssb        (528)    24181 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/plugin.py
--rw-r--r--   0 lim       (4661) ssb        (528)     2853 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/utils.py
-drwxr-sr-x   0 lim       (4661) ssb        (528)        0 2020-07-31 20:58:46.435920 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/
--rw-r--r--   0 lim       (4661) ssb        (528)    13509 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/PKG-INFO
--rw-r--r--   0 lim       (4661) ssb        (528)      702 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/SOURCES.txt
--rw-r--r--   0 lim       (4661) ssb        (528)        1 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/dependency_links.txt
--rw-r--r--   0 lim       (4661) ssb        (528)       59 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/entry_points.txt
--rw-r--r--   0 lim       (4661) ssb        (528)        1 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/not-zip-safe
--rw-r--r--   0 lim       (4661) ssb        (528)       16 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/requires.txt
--rw-r--r--   0 lim       (4661) ssb        (528)       19 2020-07-31 20:58:46.000000 pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/top_level.txt
--rw-r--r--   0 lim       (4661) ssb        (528)      268 2020-07-31 20:58:46.437920 pytest-doctestplus-0.8.0.dev0/setup.cfg
--rwxr-xr-x   0 lim       (4661) ssb        (528)     1501 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/setup.py
-drwxr-sr-x   0 lim       (4661) ssb        (528)        0 2020-07-31 20:58:46.436920 pytest-doctestplus-0.8.0.dev0/tests/
--rw-r--r--   0 lim       (4661) ssb        (528)     1271 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/conftest.py
-drwxr-sr-x   0 lim       (4661) ssb        (528)        0 2020-07-31 20:58:46.436920 pytest-doctestplus-0.8.0.dev0/tests/docs/
--rw-r--r--   0 lim       (4661) ssb        (528)      643 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/docs/skip_all.rst
--rw-r--r--   0 lim       (4661) ssb        (528)      856 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/docs/skip_all.tex
--rw-r--r--   0 lim       (4661) ssb        (528)     1421 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/docs/skip_some.rst
--rw-r--r--   0 lim       (4661) ssb        (528)     1409 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/docs/skip_some.tex
-drwxr-sr-x   0 lim       (4661) ssb        (528)        0 2020-07-31 20:58:46.436920 pytest-doctestplus-0.8.0.dev0/tests/python/
--rw-r--r--   0 lim       (4661) ssb        (528)     2117 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/python/doctests.py
--rw-r--r--   0 lim       (4661) ssb        (528)      604 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/python/skip_doctests.py
--rw-r--r--   0 lim       (4661) ssb        (528)    18451 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/test_doctestplus.py
--rw-r--r--   0 lim       (4661) ssb        (528)      871 2020-07-31 20:55:19.000000 pytest-doctestplus-0.8.0.dev0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (116)     1128 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (116)     1684 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/.github/workflows/python-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (116)      648 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (116)     3072 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1496 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      131 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)    14911 2021-01-15 01:19:55.924952 pytest-doctestplus-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)    11408 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (116)      236 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1504 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/licenses/SYMPY_LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      140 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/pytest_doctestplus/
+-rw-r--r--   0 runner    (1001) docker     (116)      117 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    11111 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/output_checker.py
+-rw-r--r--   0 runner    (1001) docker     (116)    26277 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/pytest_doctestplus/sphinx/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/sphinx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1983 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/sphinx/doctestplus.py
+-rw-r--r--   0 runner    (1001) docker     (116)      835 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      142 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus/version.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)    14911 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      957 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       59 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (116)       31 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       19 2021-01-15 01:19:55.000000 pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)     1437 2021-01-15 01:19:55.924952 pytest-doctestplus-0.9.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (116)      149 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)     1271 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/tests/docs/
+-rw-r--r--   0 runner    (1001) docker     (116)      643 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/docs/skip_all.rst
+-rw-r--r--   0 runner    (1001) docker     (116)      856 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/docs/skip_all.tex
+-rw-r--r--   0 runner    (1001) docker     (116)     1421 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/docs/skip_some.rst
+-rw-r--r--   0 runner    (1001) docker     (116)     1409 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/docs/skip_some.tex
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-01-15 01:19:55.920952 pytest-doctestplus-0.9.0/tests/python/
+-rw-r--r--   0 runner    (1001) docker     (116)     2117 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/python/doctests.py
+-rw-r--r--   0 runner    (1001) docker     (116)      604 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/python/skip_doctests.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20686 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/test_doctestplus.py
+-rw-r--r--   0 runner    (1001) docker     (116)      340 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (116)      903 2021-01-15 01:19:47.000000 pytest-doctestplus-0.9.0/tox.ini
```

### Comparing `pytest-doctestplus-0.8.0.dev0/CHANGES.rst` & `pytest-doctestplus-0.9.0/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+0.9.0 (2021-01-14)
+==================
+
+- Declare ``setuptools`` runtime dependency [#93]
+
+- Add ``SHOW_WARNINGS`` flag to show warnings. [#136]
+
+- Add the doctestplus sphinx extension. [#113]
+
+- Compatibility with pytest>=6.3 [#140, #141]
+
 0.8.0 (2020-07-31)
 ==================
 
 - Compatibility with ``pytest`` 6.0.0. [#120]
 
 0.7.0 (2020-05-20)
 ==================
```

### Comparing `pytest-doctestplus-0.8.0.dev0/LICENSE.rst` & `pytest-doctestplus-0.9.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/PKG-INFO` & `pytest-doctestplus-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-doctestplus
-Version: 0.8.0.dev0
+Version: 0.9.0
 Summary: Pytest plugin with advanced doctest features.
-Home-page: https://astropy.org
+Home-page: https://github.com/astropy/pytest-doctestplus
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD
 Description: ==================
         pytest-doctestplus
         ==================
         
         This package contains a plugin for the `pytest`_ framework that provides
         advanced doctest support and enables the testing of `reStructuredText`_
         (".rst") files. It was originally part of the `astropy`_ core package, but has
         been moved to a separate package in order to be of more general use.
         
         .. _pytest: https://pytest.org/en/latest/
-        .. _astropy: https://astropy.org/en/latest/
+        .. _astropy: https://astropy.org/
         .. _reStructuredText: https://en.wikipedia.org/wiki/ReStructuredText
         
         
         Motivation
         ----------
         
         This plugin provides advanced features for testing example Python code that is
@@ -53,15 +53,15 @@
             $ pip install pytest-doctestplus
         
         It is also possible to install the latest development version from the source
         repository::
         
             $ git clone https://github.com/astropy/pytest-doctestplus
             $ cd pytest-doctestplus
-            $ python ./setup.py install
+            $ pip install .
         
         In either case, the plugin will automatically be registered for use with
         ``pytest``.
         
         Usage
         -----
         
@@ -151,14 +151,31 @@
         
         .. code-block:: python
         
           >>> import numpy as np
           >>> np.mean([])  # doctest: +IGNORE_WARNINGS
           np.nan
         
+        Showing warnings
+        ~~~~~~~~~~~~~~~~
+        
+        If code in a doctest emits a warning and you want to make sure that warning is
+        shown, you can make use of the ``SHOW_WARNINGS`` flag. This is useful when
+        warnings are turned into errors by pytest, and also because by default warnings
+        are printed to stderr. This is the opposite from ``IGNORE_WARNINGS`` so
+        obviously the two flags should not be used together. For example:
+        
+        .. code-block:: python
+        
+          >>> import numpy as np
+          >>> np.mean([])  # doctest: +SHOW_WARNINGS
+          RuntimeWarning: Mean of empty slice.
+          RuntimeWarning: invalid value encountered in double_scalars
+          np.nan
+        
         Skipping Tests
         ~~~~~~~~~~~~~~
         
         Doctest provides the ``+SKIP`` directive for skipping statements that should
         not be executed when testing documentation.
         
         .. code-block:: python
@@ -265,20 +282,31 @@
         The ``+REMOTE_DATA`` directive indicates that the marked statement should only
         be executed if the ``--remote-data`` option is given. By default, all
         statements marked with ``--remote-data`` will be skipped.
         
         .. _pytest-remotedata: https://github.com/astropy/pytest-remotedata
         __ pytest-remotedata_
         
+        Sphinx Compatibility
+        ~~~~~~~~~~~~~~~~~~~~
+        
+        To use the additional directives when building your documentation with sphinx
+        you may want to enable the sphinx extension which registers these directives
+        with sphinx. Doing so ensures that sphinx correctly ignores these directives,
+        running the doctests with sphinx is not supported. To do this, add
+        ``'pytest_doctestplus.sphinx.doctestplus'`` to your ``extensions`` list in your
+        ``conf.py`` file.
+        
+        
         Development Status
         ------------------
         
-        .. image:: https://travis-ci.org/astropy/pytest-doctestplus.svg
-            :target: https://travis-ci.org/astropy/pytest-doctestplus
-            :alt: Travis CI Status
+        .. image:: https://github.com/astropy/pytest-doctestplus/workflows/Run%20unit%20tests/badge.svg
+            :target: https://github.com/astropy/pytest-doctestplus/actions
+            :alt: CI Status
         
         Questions, bug reports, and feature requests can be submitted on `github`_.
         
         .. _github: https://github.com/astropy/pytest-doctestplus
         
         License
         -------
@@ -290,14 +318,16 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
```

### Comparing `pytest-doctestplus-0.8.0.dev0/README.rst` & `pytest-doctestplus-0.9.0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 This package contains a plugin for the `pytest`_ framework that provides
 advanced doctest support and enables the testing of `reStructuredText`_
 (".rst") files. It was originally part of the `astropy`_ core package, but has
 been moved to a separate package in order to be of more general use.
 
 .. _pytest: https://pytest.org/en/latest/
-.. _astropy: https://astropy.org/en/latest/
+.. _astropy: https://astropy.org/
 .. _reStructuredText: https://en.wikipedia.org/wiki/ReStructuredText
 
 
 Motivation
 ----------
 
 This plugin provides advanced features for testing example Python code that is
@@ -45,15 +45,15 @@
     $ pip install pytest-doctestplus
 
 It is also possible to install the latest development version from the source
 repository::
 
     $ git clone https://github.com/astropy/pytest-doctestplus
     $ cd pytest-doctestplus
-    $ python ./setup.py install
+    $ pip install .
 
 In either case, the plugin will automatically be registered for use with
 ``pytest``.
 
 Usage
 -----
 
@@ -143,14 +143,31 @@
 
 .. code-block:: python
 
   >>> import numpy as np
   >>> np.mean([])  # doctest: +IGNORE_WARNINGS
   np.nan
 
+Showing warnings
+~~~~~~~~~~~~~~~~
+
+If code in a doctest emits a warning and you want to make sure that warning is
+shown, you can make use of the ``SHOW_WARNINGS`` flag. This is useful when
+warnings are turned into errors by pytest, and also because by default warnings
+are printed to stderr. This is the opposite from ``IGNORE_WARNINGS`` so
+obviously the two flags should not be used together. For example:
+
+.. code-block:: python
+
+  >>> import numpy as np
+  >>> np.mean([])  # doctest: +SHOW_WARNINGS
+  RuntimeWarning: Mean of empty slice.
+  RuntimeWarning: invalid value encountered in double_scalars
+  np.nan
+
 Skipping Tests
 ~~~~~~~~~~~~~~
 
 Doctest provides the ``+SKIP`` directive for skipping statements that should
 not be executed when testing documentation.
 
 .. code-block:: python
@@ -257,20 +274,31 @@
 The ``+REMOTE_DATA`` directive indicates that the marked statement should only
 be executed if the ``--remote-data`` option is given. By default, all
 statements marked with ``--remote-data`` will be skipped.
 
 .. _pytest-remotedata: https://github.com/astropy/pytest-remotedata
 __ pytest-remotedata_
 
+Sphinx Compatibility
+~~~~~~~~~~~~~~~~~~~~
+
+To use the additional directives when building your documentation with sphinx
+you may want to enable the sphinx extension which registers these directives
+with sphinx. Doing so ensures that sphinx correctly ignores these directives,
+running the doctests with sphinx is not supported. To do this, add
+``'pytest_doctestplus.sphinx.doctestplus'`` to your ``extensions`` list in your
+``conf.py`` file.
+
+
 Development Status
 ------------------
 
-.. image:: https://travis-ci.org/astropy/pytest-doctestplus.svg
-    :target: https://travis-ci.org/astropy/pytest-doctestplus
-    :alt: Travis CI Status
+.. image:: https://github.com/astropy/pytest-doctestplus/workflows/Run%20unit%20tests/badge.svg
+    :target: https://github.com/astropy/pytest-doctestplus/actions
+    :alt: CI Status
 
 Questions, bug reports, and feature requests can be submitted on `github`_.
 
 .. _github: https://github.com/astropy/pytest-doctestplus
 
 License
 -------
```

### Comparing `pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/output_checker.py` & `pytest-doctestplus-0.9.0/pytest_doctestplus/output_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 FIX = doctest.register_optionflag('FIX')
 FLOAT_CMP = doctest.register_optionflag('FLOAT_CMP')
 REMOTE_DATA = doctest.register_optionflag('REMOTE_DATA')
 IGNORE_OUTPUT = doctest.register_optionflag('IGNORE_OUTPUT')
 IGNORE_OUTPUT_3 = doctest.register_optionflag('IGNORE_OUTPUT_3')
 IGNORE_WARNINGS = doctest.register_optionflag('IGNORE_WARNINGS')
+SHOW_WARNINGS = doctest.register_optionflag('SHOW_WARNINGS')
 
 # These might appear in some doctests and are used in the default pytest
 # doctest plugin. This plugin doesn't actually implement these flags but this
 # allows them to appear in docstrings.
 ALLOW_BYTES = doctest.register_optionflag('ALLOW_BYTES')
 ALLOW_UNICODE = doctest.register_optionflag('ALLOW_UNICODE')
```

### Comparing `pytest-doctestplus-0.8.0.dev0/pytest_doctestplus/plugin.py` & `pytest-doctestplus-0.9.0/pytest_doctestplus/plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,43 +5,42 @@
 """
 import doctest
 import fnmatch
 import os
 import re
 import sys
 import warnings
-
-from packaging.version import Version
+from pathlib import Path
+from textwrap import indent
 
 import pytest
+from packaging.version import Version
 
 from pytest_doctestplus.utils import ModuleChecker
-from .output_checker import FIX, IGNORE_WARNINGS, OutputChecker, REMOTE_DATA
 
-try:
-    from textwrap import indent
-except ImportError:  # PY2
-    def indent(text, prefix):
-        return '\n'.join([prefix + line for line in text.splitlines()])
+from .output_checker import (FIX, IGNORE_WARNINGS, REMOTE_DATA, SHOW_WARNINGS,
+                             OutputChecker)
 
-PYTEST_GT_5 = Version(pytest.__version__) > Version('5.9.9')
+_pytest_version = Version(pytest.__version__)
+PYTEST_GT_5 = _pytest_version > Version('5.9.9')
+PYTEST_GE_6_3 = _pytest_version.is_devrelease or _pytest_version >= Version('6.3')
 
 comment_characters = {
     '.txt': '#',
     '.tex': '%',
     '.rst': r'\.\.'
 }
 
 
-# For the IGNORE_WARNINGS option, we create a context manager that doesn't
-# require us to add any imports to the example list and contains everything
-# that is needed to silence warnings.
+# For the IGNORE_WARNINGS and SHOW_WARNINGS option, we create a context manager
+# that doesn't require us to add any imports to the example list and contains
+# everything that is needed to silence or print warnings.
 
 IGNORE_WARNINGS_CONTEXT = """
-class _doctestplus_ignore_all_warnings(object):
+class _doctestplus_ignore_all_warnings:
 
     def __init__(self):
         import warnings
         self._cw = warnings.catch_warnings()
 
     def __enter__(self, *args, **kwargs):
         result = self._cw.__enter__(*args, **kwargs)
@@ -50,14 +49,34 @@
         return result
 
     def __exit__(self, *args, **kwargs):
         return self._cw.__exit__(*args, **kwargs)
 """.lstrip()
 
 
+SHOW_WARNINGS_CONTEXT = """
+class _doctestplus_show_all_warnings:
+
+    def __init__(self):
+        import warnings
+        self._cw = warnings.catch_warnings(record=True)
+
+    def __enter__(self, *args, **kwargs):
+        self.result = self._cw.__enter__(*args, **kwargs)
+        import warnings
+        warnings.simplefilter('always')
+        return self.result
+
+    def __exit__(self, *args, **kwargs):
+        self._cw.__exit__(*args, **kwargs)
+        for warn in self.result:
+            print(f'{warn._category_name}: {warn.message}')
+""".lstrip()
+
+
 # these pytest hooks allow us to mark tests and run the marked tests with
 # specific command line options.
 def pytest_addoption(parser):
     parser.addoption("--doctest-plus", action="store_true",
                      help="enable running doctests with additional "
                           "features not found in the normal doctest "
                           "plugin")
@@ -169,15 +188,18 @@
         # handling __doctest_skip__) doesn't happen.
         def collect(self):
             # When running directly from pytest we need to make sure that we
             # don't accidentally import setup.py!
             if self.fspath.basename == "setup.py":
                 return
             elif self.fspath.basename == "conftest.py":
-                if PYTEST_GT_5:
+                if PYTEST_GE_6_3:
+                    module = self.config.pluginmanager._importconftest(
+                        Path(self.fspath), self.config.getoption("importmode"))
+                elif PYTEST_GT_5:
                     module = self.config.pluginmanager._importconftest(
                         self.fspath, self.config.getoption("importmode"))
                 else:
                     module = self.config.pluginmanager._importconftest(
                         self.fspath)
             else:
                 try:
@@ -196,31 +218,43 @@
                 verbose=False, optionflags=options, checker=OutputChecker())
 
             for test in finder.find(module):
                 if test.examples:  # skip empty doctests
                     if config.getoption('remote_data', 'none') != 'any':
 
                         ignore_warnings_context_needed = False
+                        show_warnings_context_needed = False
 
                         for example in test.examples:
 
                             # If warnings are to be ignored we need to catch them by
                             # wrapping the source in a context manager.
                             if example.options.get(IGNORE_WARNINGS, False):
                                 example.source = ("with _doctestplus_ignore_all_warnings():\n"
                                                   + indent(example.source, '    '))
                                 ignore_warnings_context_needed = True
 
+                            # Same for SHOW_WARNINGS
+                            if example.options.get(SHOW_WARNINGS, False):
+                                example.source = ("with _doctestplus_show_all_warnings():\n"
+                                                  + indent(example.source, '    '))
+                                show_warnings_context_needed = True
+
                             if example.options.get(REMOTE_DATA):
                                 example.options[doctest.SKIP] = True
 
                         # We insert the definition of the context manager to ignore
                         # warnings at the start of the file if needed.
                         if ignore_warnings_context_needed:
-                            test.examples.insert(0, doctest.Example(source=IGNORE_WARNINGS_CONTEXT, want=''))
+                            test.examples.insert(0, doctest.Example(
+                                source=IGNORE_WARNINGS_CONTEXT, want=''))
+
+                        if show_warnings_context_needed:
+                            test.examples.insert(0, doctest.Example(
+                                source=SHOW_WARNINGS_CONTEXT, want=''))
 
                     try:
                         yield doctest_plugin.DoctestItem.from_parent(
                             self, name=test.name, runner=runner, dtest=test
                         )
                     except AttributeError:
                         # pytest < 5.4
@@ -285,14 +319,15 @@
                 warnings.warn("file format '{}' is not recognized, assuming "
                               "'{}' as the comment character."
                               .format(ext, comment_characters['.rst']))
                 ext = '.rst'
             comment_char = comment_characters[ext]
 
             ignore_warnings_context_needed = False
+            show_warnings_context_needed = False
 
             for entry in result:
 
                 if isinstance(entry, str) and entry:
                     required = []
                     skip_next = False
                     lines = entry.strip().splitlines()
@@ -340,26 +375,35 @@
                     # If warnings are to be ignored we need to catch them by
                     # wrapping the source in a context manager.
                     if entry.options.get(IGNORE_WARNINGS, False):
                         entry.source = ("with _doctestplus_ignore_all_warnings():\n"
                                         + indent(entry.source, '    '))
                         ignore_warnings_context_needed = True
 
+                    # Same to show warnings
+                    if entry.options.get(SHOW_WARNINGS, False):
+                        entry.source = ("with _doctestplus_show_all_warnings():\n"
+                                        + indent(entry.source, '    '))
+                        show_warnings_context_needed = True
+
                     has_required_modules = DocTestFinderPlus.check_required_modules(required)
                     if skip_all or skip_next or not has_required_modules:
                         entry.options[doctest.SKIP] = True
 
                     if config.getoption('remote_data', 'none') != 'any' and entry.options.get(REMOTE_DATA):
                         entry.options[doctest.SKIP] = True
 
             # We insert the definition of the context manager to ignore
             # warnings at the start of the file if needed.
             if ignore_warnings_context_needed:
                 result.insert(0, doctest.Example(source=IGNORE_WARNINGS_CONTEXT, want=''))
 
+            if show_warnings_context_needed:
+                result.insert(0, doctest.Example(source=SHOW_WARNINGS_CONTEXT, want=''))
+
             return result
 
     config.pluginmanager.register(
         DoctestPlus(
             DocTestModulePlus,
             DocTestTextfilePlus,
             config.option.doctestglob,
@@ -387,15 +431,19 @@
         self._ignore_paths = []
 
     def pytest_ignore_collect(self, path, config):
         """
         Skip paths that match any of the doctest_norecursedirs patterns or
         if doctest_only is True then skip all regular test files (eg test_*.py).
         """
-        collect_ignore = config._getconftest_pathlist("collect_ignore", path=path.dirpath())
+        if PYTEST_GE_6_3:
+            dirpath = Path(path).parent
+        else:
+            dirpath = path.dirpath()
+        collect_ignore = config._getconftest_pathlist("collect_ignore", path=dirpath)
 
         # The collect_ignore conftest.py variable should cause all test
         # runners to ignore this file and all subfiles and subdirectories
         if collect_ignore is not None and path in collect_ignore:
             return True
 
         if config.option.doctest_only:
```

### Comparing `pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/PKG-INFO` & `pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: pytest-doctestplus
-Version: 0.8.0.dev0
+Version: 0.9.0
 Summary: Pytest plugin with advanced doctest features.
-Home-page: https://astropy.org
+Home-page: https://github.com/astropy/pytest-doctestplus
 Author: The Astropy Developers
 Author-email: astropy.team@gmail.com
 License: BSD
 Description: ==================
         pytest-doctestplus
         ==================
         
         This package contains a plugin for the `pytest`_ framework that provides
         advanced doctest support and enables the testing of `reStructuredText`_
         (".rst") files. It was originally part of the `astropy`_ core package, but has
         been moved to a separate package in order to be of more general use.
         
         .. _pytest: https://pytest.org/en/latest/
-        .. _astropy: https://astropy.org/en/latest/
+        .. _astropy: https://astropy.org/
         .. _reStructuredText: https://en.wikipedia.org/wiki/ReStructuredText
         
         
         Motivation
         ----------
         
         This plugin provides advanced features for testing example Python code that is
@@ -53,15 +53,15 @@
             $ pip install pytest-doctestplus
         
         It is also possible to install the latest development version from the source
         repository::
         
             $ git clone https://github.com/astropy/pytest-doctestplus
             $ cd pytest-doctestplus
-            $ python ./setup.py install
+            $ pip install .
         
         In either case, the plugin will automatically be registered for use with
         ``pytest``.
         
         Usage
         -----
         
@@ -151,14 +151,31 @@
         
         .. code-block:: python
         
           >>> import numpy as np
           >>> np.mean([])  # doctest: +IGNORE_WARNINGS
           np.nan
         
+        Showing warnings
+        ~~~~~~~~~~~~~~~~
+        
+        If code in a doctest emits a warning and you want to make sure that warning is
+        shown, you can make use of the ``SHOW_WARNINGS`` flag. This is useful when
+        warnings are turned into errors by pytest, and also because by default warnings
+        are printed to stderr. This is the opposite from ``IGNORE_WARNINGS`` so
+        obviously the two flags should not be used together. For example:
+        
+        .. code-block:: python
+        
+          >>> import numpy as np
+          >>> np.mean([])  # doctest: +SHOW_WARNINGS
+          RuntimeWarning: Mean of empty slice.
+          RuntimeWarning: invalid value encountered in double_scalars
+          np.nan
+        
         Skipping Tests
         ~~~~~~~~~~~~~~
         
         Doctest provides the ``+SKIP`` directive for skipping statements that should
         not be executed when testing documentation.
         
         .. code-block:: python
@@ -265,20 +282,31 @@
         The ``+REMOTE_DATA`` directive indicates that the marked statement should only
         be executed if the ``--remote-data`` option is given. By default, all
         statements marked with ``--remote-data`` will be skipped.
         
         .. _pytest-remotedata: https://github.com/astropy/pytest-remotedata
         __ pytest-remotedata_
         
+        Sphinx Compatibility
+        ~~~~~~~~~~~~~~~~~~~~
+        
+        To use the additional directives when building your documentation with sphinx
+        you may want to enable the sphinx extension which registers these directives
+        with sphinx. Doing so ensures that sphinx correctly ignores these directives,
+        running the doctests with sphinx is not supported. To do this, add
+        ``'pytest_doctestplus.sphinx.doctestplus'`` to your ``extensions`` list in your
+        ``conf.py`` file.
+        
+        
         Development Status
         ------------------
         
-        .. image:: https://travis-ci.org/astropy/pytest-doctestplus.svg
-            :target: https://travis-ci.org/astropy/pytest-doctestplus
-            :alt: Travis CI Status
+        .. image:: https://github.com/astropy/pytest-doctestplus/workflows/Run%20unit%20tests/badge.svg
+            :target: https://github.com/astropy/pytest-doctestplus/actions
+            :alt: CI Status
         
         Questions, bug reports, and feature requests can be submitted on `github`_.
         
         .. _github: https://github.com/astropy/pytest-doctestplus
         
         License
         -------
@@ -290,14 +318,16 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
 Requires-Python: >=3.6
+Description-Content-Type: text/x-rst
```

### Comparing `pytest-doctestplus-0.8.0.dev0/pytest_doctestplus.egg-info/SOURCES.txt` & `pytest-doctestplus-0.9.0/pytest_doctestplus.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,34 @@
+.gitignore
 CHANGES.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
+pyproject.toml
 setup.cfg
 setup.py
+tox.ini
+.github/workflows/publish.yml
+.github/workflows/python-tests.yml
+licenses/README.rst
+licenses/SYMPY_LICENSE.rst
 pytest_doctestplus/__init__.py
 pytest_doctestplus/output_checker.py
 pytest_doctestplus/plugin.py
 pytest_doctestplus/utils.py
+pytest_doctestplus/version.py
 pytest_doctestplus.egg-info/PKG-INFO
 pytest_doctestplus.egg-info/SOURCES.txt
 pytest_doctestplus.egg-info/dependency_links.txt
 pytest_doctestplus.egg-info/entry_points.txt
 pytest_doctestplus.egg-info/not-zip-safe
 pytest_doctestplus.egg-info/requires.txt
 pytest_doctestplus.egg-info/top_level.txt
+pytest_doctestplus/sphinx/__init__.py
+pytest_doctestplus/sphinx/doctestplus.py
 tests/conftest.py
 tests/test_doctestplus.py
 tests/test_utils.py
 tests/docs/skip_all.rst
 tests/docs/skip_all.tex
 tests/docs/skip_some.rst
 tests/docs/skip_some.tex
```

### Comparing `pytest-doctestplus-0.8.0.dev0/setup.py` & `pytest-doctestplus-0.9.0/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,60 @@
-#!/usr/bin/env python
-# Licensed under a 3-clause BSD style license - see LICENSE.rst
-# -*- encoding: utf-8 -*-
-
-from setuptools import setup, find_packages
-
-
-def readme():
-    with open('README.rst') as ff:
-        return ff.read()
-
-
-setup(
-    name='pytest-doctestplus',
-    version='0.8.0.dev0',
-    license='BSD',
-    description='Pytest plugin with advanced doctest features.',
-    long_description=readme(),
-    author='The Astropy Developers',
-    author_email='astropy.team@gmail.com',
-    url='https://astropy.org',
-    packages=find_packages(exclude=['tests']),
-    include_package_data=True,
-    zip_safe=False,
-    classifiers=[
-        'Development Status :: 3 - Alpha',
-        'Framework :: Pytest',
-        'Intended Audience :: Developers',
-        'License :: OSI Approved :: BSD License',
-        'Operating System :: OS Independent',
-        'Programming Language :: Python',
-        'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
-        'Programming Language :: Python :: Implementation :: CPython',
-        'Topic :: Software Development :: Testing',
-        'Topic :: Utilities',
-    ],
-    keywords=['doctest', 'rst', 'pytest', 'py.test'],
-    install_requires=['pytest>=4.0', 'pip'],
-    python_requires='>=3.6',
-    entry_points={
-        'pytest11': [
-            'pytest_doctestplus = pytest_doctestplus.plugin',
-        ],
-    },
-)
+[metadata]
+name = pytest-doctestplus
+url = https://github.com/astropy/pytest-doctestplus
+author = The Astropy Developers
+author_email = astropy.team@gmail.com
+classifiers = 
+	Development Status :: 3 - Alpha
+	Framework :: Pytest
+	Intended Audience :: Developers
+	License :: OSI Approved :: BSD License
+	Operating System :: OS Independent
+	Programming Language :: Python
+	Programming Language :: Python :: 3
+	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.6
+	Programming Language :: Python :: 3.7
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: Implementation :: CPython
+	Topic :: Software Development :: Testing
+	Topic :: Utilities
+license = BSD
+description = Pytest plugin with advanced doctest features.
+long_description = file: README.rst
+long_description_content_type = text/x-rst
+keywords = doctest, rst, pytest, py.test
+
+[options]
+zip_safe = False
+packages = find:
+python_requires = >=3.6
+setup_requires = 
+	setuptools_scm
+install_requires = 
+	pytest>=4.6
+	setuptools>=30.3.0
+
+[options.entry_points]
+pytest11 = 
+	pytest_doctestplus = pytest_doctestplus.plugin
+
+[options.packages.find]
+exclude = 
+	tests
+
+[tool:pytest]
+minversion = 4.6
+testpaths = tests pytest_doctestplus
+xfail_strict = true
+filterwarnings = 
+	error
+	ignore:file format.*:UserWarning
+	ignore:.*non-empty pattern match.*:FutureWarning
+
+[flake8]
+max-line-length = 100
+
+[egg_info]
+tag_build = 
+tag_date = 0
+
```

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/conftest.py` & `pytest-doctestplus-0.9.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/docs/skip_all.rst` & `pytest-doctestplus-0.9.0/tests/docs/skip_all.rst`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/docs/skip_all.tex` & `pytest-doctestplus-0.9.0/tests/docs/skip_all.tex`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/docs/skip_some.rst` & `pytest-doctestplus-0.9.0/tests/docs/skip_some.rst`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/docs/skip_some.tex` & `pytest-doctestplus-0.9.0/tests/docs/skip_some.tex`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/python/doctests.py` & `pytest-doctestplus-0.9.0/tests/python/doctests.py`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/python/skip_doctests.py` & `pytest-doctestplus-0.9.0/tests/python/skip_doctests.py`

 * *Files identical despite different names*

### Comparing `pytest-doctestplus-0.8.0.dev0/tests/test_doctestplus.py` & `pytest-doctestplus-0.9.0/tests/test_doctestplus.py`

 * *Files 6% similar despite different names*

```diff
@@ -450,14 +450,80 @@
             >>> warnings.warn('A warning occurred', UserWarning)  # doctest: +IGNORE_WARNINGS
         """)
     reprec = testdir.inline_run(p, "--doctest-plus", "--doctest-rst",
                                 "--text-file-format=rst", "-W error")
     reprec.assertoutcome(failed=0, passed=1)
 
 
+def test_show_warnings_module(testdir):
+
+    p = testdir.makepyfile(
+        """
+        def myfunc():
+            '''
+            >>> import warnings
+            >>> warnings.warn('A warning occurred', UserWarning)  # doctest: +SHOW_WARNINGS
+            UserWarning: A warning occurred
+            '''
+            pass
+        """)
+    reprec = testdir.inline_run(p, "--doctest-plus", "-W error")
+    reprec.assertoutcome(failed=0, passed=1)
+
+    # Make sure it fails if warning message is missing
+    p = testdir.makepyfile(
+        """
+        def myfunc():
+            '''
+            >>> import warnings
+            >>> warnings.warn('A warning occurred', UserWarning)  # doctest: +SHOW_WARNINGS
+            '''
+            pass
+        """)
+    reprec = testdir.inline_run(p, "--doctest-plus", "-W error")
+    reprec.assertoutcome(failed=1, passed=0)
+
+
+def test_show_warnings_rst(testdir):
+
+    p = testdir.makefile(".rst",
+        """
+        ::
+            >>> import warnings
+            >>> warnings.warn('A warning occurred', UserWarning)  # doctest: +SHOW_WARNINGS
+            UserWarning: A warning occurred
+        """)
+    reprec = testdir.inline_run(p, "--doctest-plus", "--doctest-rst",
+                                "--text-file-format=rst", "-W error")
+    reprec.assertoutcome(failed=0, passed=1)
+
+    # Make sure it fails if warning message is missing
+    p = testdir.makefile(".rst",
+        """
+        ::
+            >>> import warnings
+            >>> warnings.warn('A warning occurred', UserWarning)  # doctest: +SHOW_WARNINGS
+        """)
+    reprec = testdir.inline_run(p, "--doctest-plus", "--doctest-rst",
+                                "--text-file-format=rst", "-W error")
+    reprec.assertoutcome(failed=1, passed=0)
+
+    # Make sure it fails if warning message is missing
+    p = testdir.makefile(".rst",
+        """
+        ::
+            >>> import warnings
+            >>> warnings.warn('A warning occurred', UserWarning)  # doctest: +SHOW_WARNINGS
+            Warning: Another warning occurred
+        """)
+    reprec = testdir.inline_run(p, "--doctest-plus", "--doctest-rst",
+                                "--text-file-format=rst", "-W error")
+    reprec.assertoutcome(failed=1, passed=0)
+
+
 def test_doctest_glob(testdir):
     testdir.makefile(
         '.rst',
         foo_1=">>> 1 + 1\n2",
     )
     testdir.makefile(
         '.rst',
```

