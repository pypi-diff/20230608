# Comparing `tmp/dj-easy-pdf-0.4.6.tar.gz` & `tmp/dj-easy-pdf-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-easy-pdf-0.4.6.tar", last modified: Thu Jun  8 09:27:18 2023, max compression
+gzip compressed data, was "dj-easy-pdf-0.4.7.tar", last modified: Thu Jun  8 09:40:30 2023, max compression
```

## Comparing `dj-easy-pdf-0.4.6.tar` & `dj-easy-pdf-0.4.7.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/easy_pdf/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.417601 dj-easy-pdf-0.4.6/easy_pdf/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/easy_pdf/templates/easy_pdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/templates/easy_pdf/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-08 09:27:18.425601 dj-easy-pdf-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:40:30.549098 dj-easy-pdf-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-08 09:40:30.549098 dj-easy-pdf-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:40:30.545097 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-08 09:40:30.000000 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-08 09:40:30.000000 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:40:30.000000 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:40:30.000000 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 09:40:30.000000 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 09:40:30.000000 dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:40:30.545097 dj-easy-pdf-0.4.7/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:40:30.545097 dj-easy-pdf-0.4.7/easy_pdf/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:40:30.549098 dj-easy-pdf-0.4.7/easy_pdf/templates/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/templates/easy_pdf/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/easy_pdf/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-08 09:40:30.549098 dj-easy-pdf-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1706 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:40:30.549098 dj-easy-pdf-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-08 09:40:12.000000 dj-easy-pdf-0.4.7/tests/tests.py
```

### Comparing `dj-easy-pdf-0.4.6/CONTRIBUTING.rst` & `dj-easy-pdf-0.4.7/CONTRIBUTING.rst`

 * *Files 4% similar despite different names*

```diff
@@ -56,20 +56,20 @@
 ============
 
 Ready to contribute? Here's how to set up `dj-easy-pdf` for local development.
 
 1. Fork the `dj-easy-pdf` repo on GitHub.
 2. Clone your fork locally::
 
-    $ git clone git@github.com:your_name_here/django-easy-pdf.git
+    $ git clone git@github.com:your_name_here/dj-easy-pdf.git
 
 3. Install your local copy into a virtualenv. Assuming you have virtualenvwrapper installed, this is how you set up your fork for local development::
 
-    $ mkvirtualenv django-easy-pdf
-    $ cd django-easy-pdf/
+    $ mkvirtualenv dj-easy-pdf
+    $ cd dj-easy-pdf/
     $ python setup.py develop
 
 4. Create a branch for local development::
 
     $ git checkout -b name-of-your-bugfix-or-feature
 
 Now you can make your changes locally.
```

### Comparing `dj-easy-pdf-0.4.6/LICENSE` & `dj-easy-pdf-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/PKG-INFO` & `dj-easy-pdf-0.4.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dj-easy-pdf
-Version: 0.4.6
+Version: 0.4.7
 Summary: Django PDF views, easily convert html responses to pdf responses
-Home-page: https://github.com/WilliamOtieno/django-easy-pdf
+Home-page: https://github.com/WilliamOtieno/dj-easy-pdf
 Author: William Otieno
 Author-email: jimmywilliamotieno@gmail.com
 License: MIT
 Keywords: dj-easy-pdf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -30,15 +30,15 @@
 .. image:: https://img.shields.io/pypi/v/dj-easy-pdf.svg
     :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: Latest Version
 .. image:: https://img.shields.io/badge/wheel-yes-green.svg
     :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: Wheel
 .. image:: https://img.shields.io/pypi/l/dj-easy-pdf.svg
-    :target: https://pypi.python.org/pypi/django-easy-pdf/
+    :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: License
 
 Developed by `William Otieno <https://github.com/WilliamOtieno/>`_.
 
 
 Overview
 --------
@@ -106,15 +106,15 @@
 
 The full documentation is at `dj-easy-pdf.readthedocs.io <https://dj-easy-pdf.readthedocs.io/>`_.
 
 
 Dependencies
 ------------
 
-``django-easy-pdf`` depends on:
+``dj-easy-pdf`` depends on:
 
     - ``django>=3.2``
     - ``xhtml2pdf``
     - ``reportlab``
 
 
 License
```

### Comparing `dj-easy-pdf-0.4.6/README.rst` & `dj-easy-pdf-0.4.7/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 .. image:: https://img.shields.io/pypi/v/dj-easy-pdf.svg
     :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: Latest Version
 .. image:: https://img.shields.io/badge/wheel-yes-green.svg
     :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: Wheel
 .. image:: https://img.shields.io/pypi/l/dj-easy-pdf.svg
-    :target: https://pypi.python.org/pypi/django-easy-pdf/
+    :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: License
 
 Developed by `William Otieno <https://github.com/WilliamOtieno/>`_.
 
 
 Overview
 --------
@@ -82,15 +82,15 @@
 
 The full documentation is at `dj-easy-pdf.readthedocs.io <https://dj-easy-pdf.readthedocs.io/>`_.
 
 
 Dependencies
 ------------
 
-``django-easy-pdf`` depends on:
+``dj-easy-pdf`` depends on:
 
     - ``django>=3.2``
     - ``xhtml2pdf``
     - ``reportlab``
 
 
 License
```

### Comparing `dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/PKG-INFO` & `dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: dj-easy-pdf
-Version: 0.4.6
+Version: 0.4.7
 Summary: Django PDF views, easily convert html responses to pdf responses
-Home-page: https://github.com/WilliamOtieno/django-easy-pdf
+Home-page: https://github.com/WilliamOtieno/dj-easy-pdf
 Author: William Otieno
 Author-email: jimmywilliamotieno@gmail.com
 License: MIT
 Keywords: dj-easy-pdf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
@@ -30,15 +30,15 @@
 .. image:: https://img.shields.io/pypi/v/dj-easy-pdf.svg
     :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: Latest Version
 .. image:: https://img.shields.io/badge/wheel-yes-green.svg
     :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: Wheel
 .. image:: https://img.shields.io/pypi/l/dj-easy-pdf.svg
-    :target: https://pypi.python.org/pypi/django-easy-pdf/
+    :target: https://pypi.python.org/pypi/dj-easy-pdf/
     :alt: License
 
 Developed by `William Otieno <https://github.com/WilliamOtieno/>`_.
 
 
 Overview
 --------
@@ -106,15 +106,15 @@
 
 The full documentation is at `dj-easy-pdf.readthedocs.io <https://dj-easy-pdf.readthedocs.io/>`_.
 
 
 Dependencies
 ------------
 
-``django-easy-pdf`` depends on:
+``dj-easy-pdf`` depends on:
 
     - ``django>=3.2``
     - ``xhtml2pdf``
     - ``reportlab``
 
 
 License
```

### Comparing `dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/SOURCES.txt` & `dj-easy-pdf-0.4.7/dj_easy_pdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/easy_pdf/exceptions.py` & `dj-easy-pdf-0.4.7/easy_pdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/easy_pdf/rendering.py` & `dj-easy-pdf-0.4.7/easy_pdf/rendering.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/easy_pdf/templates/easy_pdf/base.html` & `dj-easy-pdf-0.4.7/easy_pdf/templates/easy_pdf/base.html`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/easy_pdf/tests.py` & `dj-easy-pdf-0.4.7/easy_pdf/tests.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/easy_pdf/views.py` & `dj-easy-pdf-0.4.7/easy_pdf/views.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/setup.py` & `dj-easy-pdf-0.4.7/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.4.6"
+version = "0.4.7"
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel upload")
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
     sys.exit()
@@ -23,15 +23,15 @@
 setup(
     name="dj-easy-pdf",
     version=version,
     description="""Django PDF views, easily convert html responses to pdf responses""",
     license="MIT",
     author="William Otieno",
     author_email="jimmywilliamotieno@gmail.com",
-    url="https://github.com/WilliamOtieno/django-easy-pdf",
+    url="https://github.com/WilliamOtieno/dj-easy-pdf",
     long_description=readme + "\n\n",
     packages=[
         "easy_pdf",
     ],
     include_package_data=True,
     install_requires=[
         "django>=3.2",
```

### Comparing `dj-easy-pdf-0.4.6/tests/test_settings.py` & `dj-easy-pdf-0.4.7/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.4.6/tests/tests.py` & `dj-easy-pdf-0.4.7/tests/tests.py`

 * *Files identical despite different names*

