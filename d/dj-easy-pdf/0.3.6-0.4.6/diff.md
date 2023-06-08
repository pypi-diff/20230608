# Comparing `tmp/dj-easy-pdf-0.3.6.tar.gz` & `tmp/dj-easy-pdf-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-easy-pdf-0.3.6.tar", last modified: Wed Jun  7 21:58:50 2023, max compression
+gzip compressed data, was "dj-easy-pdf-0.4.6.tar", last modified: Thu Jun  8 09:27:18 2023, max compression
```

## Comparing `dj-easy-pdf-0.3.6.tar` & `dj-easy-pdf-0.4.6.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.448764 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/easy_pdf/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.448764 dj-easy-pdf-0.3.6/easy_pdf/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/easy_pdf/templates/easy_pdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/templates/easy_pdf/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 09:27:18.000000 dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5464 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.417601 dj-easy-pdf-0.4.6/easy_pdf/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/easy_pdf/templates/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/templates/easy_pdf/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/easy_pdf/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-08 09:27:18.425601 dj-easy-pdf-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 09:27:18.421601 dj-easy-pdf-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-08 09:27:06.000000 dj-easy-pdf-0.4.6/tests/tests.py
```

### Comparing `dj-easy-pdf-0.3.6/CONTRIBUTING.rst` & `dj-easy-pdf-0.4.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/LICENSE` & `dj-easy-pdf-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/PKG-INFO` & `dj-easy-pdf-0.4.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dj-easy-pdf
-Version: 0.3.6
-Summary: Django PDF views, the easy way
+Version: 0.4.6
+Summary: Django PDF views, easily convert html responses to pdf responses
 Home-page: https://github.com/WilliamOtieno/django-easy-pdf
 Author: William Otieno
 Author-email: jimmywilliamotieno@gmail.com
 License: MIT
 Keywords: dj-easy-pdf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 Django PDF rendering
 ====================
 
 Django PDF rendering, easily convert html responses to pdf responses
```

### Comparing `dj-easy-pdf-0.3.6/README.rst` & `dj-easy-pdf-0.4.6/README.rst`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/PKG-INFO` & `dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dj-easy-pdf
-Version: 0.3.6
-Summary: Django PDF views, the easy way
+Version: 0.4.6
+Summary: Django PDF views, easily convert html responses to pdf responses
 Home-page: https://github.com/WilliamOtieno/django-easy-pdf
 Author: William Otieno
 Author-email: jimmywilliamotieno@gmail.com
 License: MIT
 Keywords: dj-easy-pdf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
@@ -14,14 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE
 
 Django PDF rendering
 ====================
 
 Django PDF rendering, easily convert html responses to pdf responses
```

### Comparing `dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/SOURCES.txt` & `dj-easy-pdf-0.4.6/dj_easy_pdf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/easy_pdf/exceptions.py` & `dj-easy-pdf-0.4.6/easy_pdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/easy_pdf/rendering.py` & `dj-easy-pdf-0.4.6/easy_pdf/rendering.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 logger_x2p = logging.getLogger("app.pdf.xhtml2pdf")
 
 
 def fetch_resources(uri, rel=None):
     """
     Retrieves embeddable resource from given ``uri``.
 
-    For now only local resources (images, fonts) are supported.
+    Both local and remote resources are supported
 
     :param str uri: path or url to image or font resource
     :param str rel: used internally by xhtmltopdf
     :returns: path to local resource file.
     :rtype: str
     :raises: :exc:`~easy_pdf.exceptions.UnsupportedMediaPathException`
     """
```

### Comparing `dj-easy-pdf-0.3.6/easy_pdf/templates/easy_pdf/base.html` & `dj-easy-pdf-0.4.6/easy_pdf/templates/easy_pdf/base.html`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/easy_pdf/tests.py` & `dj-easy-pdf-0.4.6/easy_pdf/tests.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/easy_pdf/views.py` & `dj-easy-pdf-0.4.6/easy_pdf/views.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/setup.py` & `dj-easy-pdf-0.4.6/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.3.6"
+version = "0.4.6"
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel upload")
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
     sys.exit()
 
 readme = open("README.rst").read()
 
 setup(
     name="dj-easy-pdf",
     version=version,
-    description="""Django PDF views, the easy way""",
+    description="""Django PDF views, easily convert html responses to pdf responses""",
     license="MIT",
     author="William Otieno",
     author_email="jimmywilliamotieno@gmail.com",
     url="https://github.com/WilliamOtieno/django-easy-pdf",
     long_description=readme + "\n\n",
     packages=[
         "easy_pdf",
@@ -49,10 +49,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries :: Python Modules"
     ],
 )
```

### Comparing `dj-easy-pdf-0.3.6/tests/test_settings.py` & `dj-easy-pdf-0.4.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.3.6/tests/tests.py` & `dj-easy-pdf-0.4.6/tests/tests.py`

 * *Files identical despite different names*

