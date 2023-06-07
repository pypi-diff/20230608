# Comparing `tmp/dj-easy-pdf-0.2.4.tar.gz` & `tmp/dj-easy-pdf-0.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dj-easy-pdf-0.2.4.tar", last modified: Wed Jun  7 20:29:36 2023, max compression
+gzip compressed data, was "dj-easy-pdf-0.3.6.tar", last modified: Wed Jun  7 21:58:50 2023, max compression
```

## Comparing `dj-easy-pdf-0.2.4.tar` & `dj-easy-pdf-0.3.6.tar`

### file list

```diff
@@ -1,30 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 20:29:36.000000 dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/easy_pdf/
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/rendering.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.763068 dj-easy-pdf-0.2.4/easy_pdf/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/easy_pdf/templates/easy_pdf/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/templates/easy_pdf/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/easy_pdf/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 20:29:36.771068 dj-easy-pdf-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 20:29:36.767068 dj-easy-pdf-0.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-07 20:29:20.000000 dj-easy-pdf-0.2.4/tests/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1112 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.448764 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3985 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 21:58:50.000000 dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/rendering.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.448764 dj-easy-pdf-0.3.6/easy_pdf/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/easy_pdf/templates/easy_pdf/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/templates/easy_pdf/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/easy_pdf/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 21:58:50.452764 dj-easy-pdf-0.3.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-06-07 21:58:36.000000 dj-easy-pdf-0.3.6/tests/tests.py
```

### Comparing `dj-easy-pdf-0.2.4/CONTRIBUTING.rst` & `dj-easy-pdf-0.3.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/LICENSE` & `dj-easy-pdf-0.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/PKG-INFO` & `dj-easy-pdf-0.3.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-easy-pdf
-Version: 0.2.4
+Version: 0.3.6
 Summary: Django PDF views, the easy way
 Home-page: https://github.com/WilliamOtieno/django-easy-pdf
 Author: William Otieno
 Author-email: jimmywilliamotieno@gmail.com
 License: MIT
 Keywords: dj-easy-pdf
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,15 +55,15 @@
 
 Quickstart
 ----------
 
 1. Include ``dj-easy-pdf``, ``xhtml2pdf`` in your ``requirements.txt`` file.
    If you are on Python 3 you need to install the latest version of Reportlab and the beta version of xhtml2pdf::
 
-    $ pip install xhtml2pdf
+    $ pip install dj-easy-pdf
 
 2. Add ``easy_pdf`` to ``INSTALLED_APPS``.
 
 3. Create HTML template for PDF document and add a view that will render it:
 
     .. code-block:: css+django
```

### Comparing `dj-easy-pdf-0.2.4/README.rst` & `dj-easy-pdf-0.3.6/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 Quickstart
 ----------
 
 1. Include ``dj-easy-pdf``, ``xhtml2pdf`` in your ``requirements.txt`` file.
    If you are on Python 3 you need to install the latest version of Reportlab and the beta version of xhtml2pdf::
 
-    $ pip install xhtml2pdf
+    $ pip install dj-easy-pdf
 
 2. Add ``easy_pdf`` to ``INSTALLED_APPS``.
 
 3. Create HTML template for PDF document and add a view that will render it:
 
     .. code-block:: css+django
```

### Comparing `dj-easy-pdf-0.2.4/dj_easy_pdf.egg-info/PKG-INFO` & `dj-easy-pdf-0.3.6/dj_easy_pdf.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dj-easy-pdf
-Version: 0.2.4
+Version: 0.3.6
 Summary: Django PDF views, the easy way
 Home-page: https://github.com/WilliamOtieno/django-easy-pdf
 Author: William Otieno
 Author-email: jimmywilliamotieno@gmail.com
 License: MIT
 Keywords: dj-easy-pdf
 Classifier: Development Status :: 5 - Production/Stable
@@ -55,15 +55,15 @@
 
 Quickstart
 ----------
 
 1. Include ``dj-easy-pdf``, ``xhtml2pdf`` in your ``requirements.txt`` file.
    If you are on Python 3 you need to install the latest version of Reportlab and the beta version of xhtml2pdf::
 
-    $ pip install xhtml2pdf
+    $ pip install dj-easy-pdf
 
 2. Add ``easy_pdf`` to ``INSTALLED_APPS``.
 
 3. Create HTML template for PDF document and add a view that will render it:
 
     .. code-block:: css+django
```

### Comparing `dj-easy-pdf-0.2.4/easy_pdf/exceptions.py` & `dj-easy-pdf-0.3.6/easy_pdf/exceptions.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/easy_pdf/rendering.py` & `dj-easy-pdf-0.3.6/easy_pdf/rendering.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,52 +1,51 @@
 # coding=utf-8
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import logging
 import os
+from urllib.parse import quote as urlquote
 
+import xhtml2pdf.default
 from django.conf import settings
-from django.template import loader
 from django.http import HttpResponse
+from django.template import loader
 from six import BytesIO
-from urllib.parse import quote as urlquote
-import xhtml2pdf.default
 from xhtml2pdf import pisa
 
-from .exceptions import UnsupportedMediaPathException, PDFRenderingError
+from .exceptions import PDFRenderingError
+from .utils import validate_image_url
 
 logger = logging.getLogger("app.pdf")
 logger_x2p = logging.getLogger("app.pdf.xhtml2pdf")
 
 
-def fetch_resources(uri, rel):
+def fetch_resources(uri, rel=None):
     """
     Retrieves embeddable resource from given ``uri``.
 
     For now only local resources (images, fonts) are supported.
 
     :param str uri: path or url to image or font resource
+    :param str rel: used internally by xhtmltopdf
     :returns: path to local resource file.
     :rtype: str
     :raises: :exc:`~easy_pdf.exceptions.UnsupportedMediaPathException`
     """
     if settings.STATIC_URL and uri.startswith(settings.STATIC_URL):
         path = os.path.join(settings.STATIC_ROOT, uri.replace(settings.STATIC_URL, ""))
     elif settings.MEDIA_URL and uri.startswith(settings.MEDIA_URL):
         path = os.path.join(settings.MEDIA_ROOT, uri.replace(settings.MEDIA_URL, ""))
     else:
         path = os.path.join(settings.STATIC_ROOT, uri)
 
     if not os.path.isfile(path):
-        raise UnsupportedMediaPathException(
-            "media urls must start with {} or {}".format(
-                settings.MEDIA_ROOT, settings.STATIC_ROOT
-            )
-        )
+        if validate_image_url(uri):
+            return uri
 
     return path.replace("\\", "/")
 
 
 def html_to_pdf(content, encoding="utf-8",
                 link_callback=fetch_resources, **kwargs):
     """
```

### Comparing `dj-easy-pdf-0.2.4/easy_pdf/templates/easy_pdf/base.html` & `dj-easy-pdf-0.3.6/easy_pdf/templates/easy_pdf/base.html`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/easy_pdf/tests.py` & `dj-easy-pdf-0.3.6/easy_pdf/tests.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/easy_pdf/views.py` & `dj-easy-pdf-0.3.6/easy_pdf/views.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/setup.py` & `dj-easy-pdf-0.3.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 try:
     from setuptools import setup
 except ImportError:
     from distutils.core import setup
 
-version = "0.2.4"
+version = "0.3.6"
 
 if sys.argv[-1] == "publish":
     os.system("python setup.py sdist bdist_wheel upload")
     print("You probably want to also tag the version now:")
     print("  git tag -a %s -m 'version %s'" % (version, version))
     print("  git push --tags")
     sys.exit()
@@ -32,15 +32,16 @@
     packages=[
         "easy_pdf",
     ],
     include_package_data=True,
     install_requires=[
         "django>=3.2",
         "xhtml2pdf>=0.2",
-        "reportlab>=3"
+        "reportlab>=3",
+        "requests"
     ],
     zip_safe=False,
     keywords="dj-easy-pdf",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Django",
```

### Comparing `dj-easy-pdf-0.2.4/tests/test_settings.py` & `dj-easy-pdf-0.3.6/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dj-easy-pdf-0.2.4/tests/tests.py` & `dj-easy-pdf-0.3.6/tests/tests.py`

 * *Files identical despite different names*

