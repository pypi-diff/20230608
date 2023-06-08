# Comparing `tmp/django-log-outgoing-requests-0.1.0.tar.gz` & `tmp/django-log-outgoing-requests-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-log-outgoing-requests-0.1.0.tar", last modified: Mon Apr  3 13:32:54 2023, max compression
+gzip compressed data, was "django-log-outgoing-requests-0.2.0.tar", last modified: Thu Jun  8 10:46:08 2023, max compression
```

## Comparing `django-log-outgoing-requests-0.1.0.tar` & `django-log-outgoing-requests-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,39 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 13:32:54.706598 django-log-outgoing-requests-0.1.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     1052 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)      259 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/MANIFEST.in
--rw-r--r--   0 alex      (1000) alex      (1000)     5520 2023-04-03 13:32:54.710598 django-log-outgoing-requests-0.1.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     4108 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/README.rst
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 13:32:54.706598 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     5520 2023-04-03 13:32:54.000000 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)      741 2023-04-03 13:32:54.000000 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-04-03 13:32:54.000000 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-04-03 13:32:54.000000 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/not-zip-safe
--rw-r--r--   0 alex      (1000) alex      (1000)      197 2023-04-03 13:32:54.000000 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       22 2023-04-03 13:32:54.000000 django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/top_level.txt
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 13:32:54.706598 django-log-outgoing-requests-0.1.0/log_outgoing_requests/
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1152 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/admin.py
--rw-r--r--   0 alex      (1000) alex      (1000)      250 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/apps.py
--rw-r--r--   0 alex      (1000) alex      (1000)      884 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/formatters.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1744 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/handlers.py
--rw-r--r--   0 alex      (1000) alex      (1000)      969 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/log_requests.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 13:32:54.706598 django-log-outgoing-requests-0.1.0/log_outgoing_requests/migrations/
--rw-r--r--   0 alex      (1000) alex      (1000)     4799 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/migrations/0001_initial.py
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/migrations/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2913 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/models.py
--rw-r--r--   0 alex      (1000) alex      (1000)        0 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/log_outgoing_requests/py.typed
--rw-r--r--   0 alex      (1000) alex      (1000)     2258 2023-04-03 13:32:54.710598 django-log-outgoing-requests-0.1.0/setup.cfg
--rw-r--r--   0 alex      (1000) alex      (1000)       38 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-04-03 13:32:54.706598 django-log-outgoing-requests-0.1.0/tests/
--rw-r--r--   0 alex      (1000) alex      (1000)     5843 2023-04-03 13:31:59.000000 django-log-outgoing-requests-0.1.0/tests/test_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.147759 django-log-outgoing-requests-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-08 10:46:08.147759 django-log-outgoing-requests-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5358 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.143759 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-06-08 10:46:08.000000 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-08 10:46:08.000000 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:46:08.000000 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 10:46:08.000000 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-08 10:46:08.000000 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-08 10:46:08.000000 django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.147759 django-log-outgoing-requests-0.2.0/log_outgoing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      518 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/datastructures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1273 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/formatters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      981 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/log_requests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.147759 django-log-outgoing-requests-0.2.0/log_outgoing_requests/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6186 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.143759 django-log-outgoing-requests-0.2.0/log_outgoing_requests/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.147759 django-log-outgoing-requests-0.2.0/log_outgoing_requests/templates/log_outgoing_requests/
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/templates/log_outgoing_requests/change_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)     5066 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/log_outgoing_requests/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-06-08 10:46:08.151759 django-log-outgoing-requests-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 10:46:08.147759 django-log-outgoing-requests-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4664 2023-06-08 10:46:02.000000 django-log-outgoing-requests-0.2.0/tests/test_utils.py
```

### Comparing `django-log-outgoing-requests-0.1.0/LICENSE` & `django-log-outgoing-requests-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.1.0/PKG-INFO` & `django-log-outgoing-requests-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-outgoing-requests
-Version: 0.1.0
+Version: 0.2.0
 Summary: Log outgoing requests made by the requests python library
 Home-page: https://github.com/maykinmedia/django-log-outgoing-requests
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://django-log-outgoing-requests.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/django-log-outgoing-requests/blob/main/CHANGELOG.rst
@@ -15,15 +15,14 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
@@ -39,36 +38,39 @@
 :Keywords: logging
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
 
-Log and save outgoing requests made by requests library
+Log and save outgoing requests
+
+The current library logs only the requests made by the `requests`_ library
 
 .. contents::
 
 .. section-numbering::
 
 Features
 ========
 
-* Log outgoing requests
+* Log outgoing requests made by requests library
 * Save logs in database
 * Overview of the saved logs in the admin page
 
 Installation
 ============
 
 Requirements
 ------------
 
 * Python 3.7 or above
 * setuptools 30.3.0 or above
 * Django 3.2 or newer
+* requests
 
 
 Install
 -------
 
 .. code-block:: bash
 
@@ -123,32 +125,57 @@
                     "level": "DEBUG",
                     "propagate": True,
                 },
             },
         }
 
         LOG_OUTGOING_REQUESTS_DB_SAVE = True # save logs enabled/disabled based on the boolean value
+        LOG_OUTGOING_REQUESTS_DB_SAVE_BODY = True # save request/response body
+        LOG_OUTGOING_REQUESTS_EMIT_BODY = True # log request/response body
+        LOG_OUTGOING_REQUESTS_CONTENT_TYPES = [
+                "text/*",
+                "application/json",
+                "application/xml",
+                "application/soap+xml",
+        ] # save request/response bodies with matching content type
+        LOG_OUTGOING_REQUESTS_MAX_CONTENT_LENGTH = 524_288  # maximal size (in bytes) for the request/response body
+        LOG_OUTGOING_REQUESTS_LOG_BODY_TO_STDOUT = True
+
 
 #.  Run the migrations
 
     .. code-block:: bash
 
         python manage.py migrate
 
+#.  Make some requests using requests library within the Django context, for example using ``python manage.py shell``
+
+    .. code-block:: console
+
+        import requests
+        res = requests.get("https://httpbin.org/json")
+        print(res.json())
+
+#.  Check stdout for the printable output, and navigate to ``Admin > Miscellaneous > Outgoing Requests Logs``
+    to see the saved log records. In order to override the settings for saving logs, navigate to
+    ``Admin > Miscellaneous > Outgoing Requests Log Configuration``.
+
 
 Local development
 =================
 
 To install and develop the library locally, use:
 
 .. code-block:: bash
 
     pip install -e --no-build-isolation .[tests,coverage,docs,pep8,release]
 
 
+.. _`requests`: https://pypi.org/project/requests/
+
 .. _`documentation`: https://docs.djangoproject.com/en/4.1/topics/logging/
 
 .. |build-status| image:: https://github.com/maykinmedia/django-log-outgoing-requests/workflows/Run%20CI/badge.svg
     :alt: Build status
     :target: https://github.com/maykinmedia/django-log-outgoing-requests/actions?query=workflow%3A%22Run+CI%22
 
 .. |code-quality| image:: https://github.com/maykinmedia/django-log-outgoing-requests/workflows/Code%20quality%20checks/badge.svg
```

### Comparing `django-log-outgoing-requests-0.1.0/README.rst` & `django-log-outgoing-requests-0.2.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -6,36 +6,39 @@
 :Keywords: logging
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
 
-Log and save outgoing requests made by requests library
+Log and save outgoing requests
+
+The current library logs only the requests made by the `requests`_ library
 
 .. contents::
 
 .. section-numbering::
 
 Features
 ========
 
-* Log outgoing requests
+* Log outgoing requests made by requests library
 * Save logs in database
 * Overview of the saved logs in the admin page
 
 Installation
 ============
 
 Requirements
 ------------
 
 * Python 3.7 or above
 * setuptools 30.3.0 or above
 * Django 3.2 or newer
+* requests
 
 
 Install
 -------
 
 .. code-block:: bash
 
@@ -90,32 +93,57 @@
                     "level": "DEBUG",
                     "propagate": True,
                 },
             },
         }
 
         LOG_OUTGOING_REQUESTS_DB_SAVE = True # save logs enabled/disabled based on the boolean value
+        LOG_OUTGOING_REQUESTS_DB_SAVE_BODY = True # save request/response body
+        LOG_OUTGOING_REQUESTS_EMIT_BODY = True # log request/response body
+        LOG_OUTGOING_REQUESTS_CONTENT_TYPES = [
+                "text/*",
+                "application/json",
+                "application/xml",
+                "application/soap+xml",
+        ] # save request/response bodies with matching content type
+        LOG_OUTGOING_REQUESTS_MAX_CONTENT_LENGTH = 524_288  # maximal size (in bytes) for the request/response body
+        LOG_OUTGOING_REQUESTS_LOG_BODY_TO_STDOUT = True
+
 
 #.  Run the migrations
 
     .. code-block:: bash
 
         python manage.py migrate
 
+#.  Make some requests using requests library within the Django context, for example using ``python manage.py shell``
+
+    .. code-block:: console
+
+        import requests
+        res = requests.get("https://httpbin.org/json")
+        print(res.json())
+
+#.  Check stdout for the printable output, and navigate to ``Admin > Miscellaneous > Outgoing Requests Logs``
+    to see the saved log records. In order to override the settings for saving logs, navigate to
+    ``Admin > Miscellaneous > Outgoing Requests Log Configuration``.
+
 
 Local development
 =================
 
 To install and develop the library locally, use:
 
 .. code-block:: bash
 
     pip install -e --no-build-isolation .[tests,coverage,docs,pep8,release]
 
 
+.. _`requests`: https://pypi.org/project/requests/
+
 .. _`documentation`: https://docs.djangoproject.com/en/4.1/topics/logging/
 
 .. |build-status| image:: https://github.com/maykinmedia/django-log-outgoing-requests/workflows/Run%20CI/badge.svg
     :alt: Build status
     :target: https://github.com/maykinmedia/django-log-outgoing-requests/actions?query=workflow%3A%22Run+CI%22
 
 .. |code-quality| image:: https://github.com/maykinmedia/django-log-outgoing-requests/workflows/Code%20quality%20checks/badge.svg
```

### Comparing `django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/PKG-INFO` & `django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-log-outgoing-requests
-Version: 0.1.0
+Version: 0.2.0
 Summary: Log outgoing requests made by the requests python library
 Home-page: https://github.com/maykinmedia/django-log-outgoing-requests
 Author: Maykin Media
 Author-email: support@maykinmedia.nl
 License: MIT
 Project-URL: Documentation, http://django-log-outgoing-requests.readthedocs.io/en/latest/
 Project-URL: Changelog, https://github.com/maykinmedia/django-log-outgoing-requests/blob/main/CHANGELOG.rst
@@ -15,15 +15,14 @@
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.1
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Microsoft :: Windows
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: tests
 Provides-Extra: pep8
 Provides-Extra: coverage
@@ -39,36 +38,39 @@
 :Keywords: logging
 :PythonVersion: 3.9
 
 |build-status| |code-quality| |black| |coverage| |docs|
 
 |python-versions| |django-versions| |pypi-version|
 
-Log and save outgoing requests made by requests library
+Log and save outgoing requests
+
+The current library logs only the requests made by the `requests`_ library
 
 .. contents::
 
 .. section-numbering::
 
 Features
 ========
 
-* Log outgoing requests
+* Log outgoing requests made by requests library
 * Save logs in database
 * Overview of the saved logs in the admin page
 
 Installation
 ============
 
 Requirements
 ------------
 
 * Python 3.7 or above
 * setuptools 30.3.0 or above
 * Django 3.2 or newer
+* requests
 
 
 Install
 -------
 
 .. code-block:: bash
 
@@ -123,32 +125,57 @@
                     "level": "DEBUG",
                     "propagate": True,
                 },
             },
         }
 
         LOG_OUTGOING_REQUESTS_DB_SAVE = True # save logs enabled/disabled based on the boolean value
+        LOG_OUTGOING_REQUESTS_DB_SAVE_BODY = True # save request/response body
+        LOG_OUTGOING_REQUESTS_EMIT_BODY = True # log request/response body
+        LOG_OUTGOING_REQUESTS_CONTENT_TYPES = [
+                "text/*",
+                "application/json",
+                "application/xml",
+                "application/soap+xml",
+        ] # save request/response bodies with matching content type
+        LOG_OUTGOING_REQUESTS_MAX_CONTENT_LENGTH = 524_288  # maximal size (in bytes) for the request/response body
+        LOG_OUTGOING_REQUESTS_LOG_BODY_TO_STDOUT = True
+
 
 #.  Run the migrations
 
     .. code-block:: bash
 
         python manage.py migrate
 
+#.  Make some requests using requests library within the Django context, for example using ``python manage.py shell``
+
+    .. code-block:: console
+
+        import requests
+        res = requests.get("https://httpbin.org/json")
+        print(res.json())
+
+#.  Check stdout for the printable output, and navigate to ``Admin > Miscellaneous > Outgoing Requests Logs``
+    to see the saved log records. In order to override the settings for saving logs, navigate to
+    ``Admin > Miscellaneous > Outgoing Requests Log Configuration``.
+
 
 Local development
 =================
 
 To install and develop the library locally, use:
 
 .. code-block:: bash
 
     pip install -e --no-build-isolation .[tests,coverage,docs,pep8,release]
 
 
+.. _`requests`: https://pypi.org/project/requests/
+
 .. _`documentation`: https://docs.djangoproject.com/en/4.1/topics/logging/
 
 .. |build-status| image:: https://github.com/maykinmedia/django-log-outgoing-requests/workflows/Run%20CI/badge.svg
     :alt: Build status
     :target: https://github.com/maykinmedia/django-log-outgoing-requests/actions?query=workflow%3A%22Run+CI%22
 
 .. |code-quality| image:: https://github.com/maykinmedia/django-log-outgoing-requests/workflows/Code%20quality%20checks/badge.svg
```

### Comparing `django-log-outgoing-requests-0.1.0/django_log_outgoing_requests.egg-info/SOURCES.txt` & `django-log-outgoing-requests-0.2.0/django_log_outgoing_requests.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,15 +8,24 @@
 django_log_outgoing_requests.egg-info/dependency_links.txt
 django_log_outgoing_requests.egg-info/not-zip-safe
 django_log_outgoing_requests.egg-info/requires.txt
 django_log_outgoing_requests.egg-info/top_level.txt
 log_outgoing_requests/__init__.py
 log_outgoing_requests/admin.py
 log_outgoing_requests/apps.py
+log_outgoing_requests/compat.py
+log_outgoing_requests/constants.py
+log_outgoing_requests/datastructures.py
 log_outgoing_requests/formatters.py
 log_outgoing_requests/handlers.py
 log_outgoing_requests/log_requests.py
 log_outgoing_requests/models.py
 log_outgoing_requests/py.typed
+log_outgoing_requests/utils.py
 log_outgoing_requests/migrations/0001_initial.py
+log_outgoing_requests/migrations/0002_outgoingrequestslogconfig_and_more.py
 log_outgoing_requests/migrations/__init__.py
-tests/test_logging.py
+log_outgoing_requests/templates/log_outgoing_requests/change_form.html
+tests/test_admin.py
+tests/test_formatter.py
+tests/test_logging.py
+tests/test_utils.py
```

### Comparing `django-log-outgoing-requests-0.1.0/log_outgoing_requests/formatters.py` & `django-log-outgoing-requests-0.2.0/log_outgoing_requests/formatters.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,42 @@
 import logging
 import textwrap
 
+from django.conf import settings
+
 
 class HttpFormatter(logging.Formatter):
     def _formatHeaders(self, d):
         return "\n".join(f"{k}: {v}" for k, v in d.items())
 
+    def _formatBody(self, content: str, request_or_response: str) -> str:
+        if settings.LOG_OUTGOING_REQUESTS_EMIT_BODY:
+            return f"\n{request_or_response} body:\n{content}"
+        return ""
+
     def formatMessage(self, record):
         result = super().formatMessage(record)
-        if record.name == "requests":
-            result += textwrap.dedent(
-                """
-                ---------------- request ----------------
-                {req.method} {req.url}
-                {reqhdrs}
-
-                ---------------- response ----------------
-                {res.status_code} {res.reason} {res.url}
-                {reshdrs}
 
+        if record.name != "requests":
+            return result
+
+        result += textwrap.dedent(
             """
-            ).format(
-                req=record.req,
-                res=record.res,
-                reqhdrs=self._formatHeaders(record.req.headers),
-                reshdrs=self._formatHeaders(record.res.headers),
-            )
+            ---------------- request ----------------
+            {req.method} {req.url}
+            {reqhdrs} {request_body}
+
+            ---------------- response ----------------
+            {res.status_code} {res.reason} {res.url}
+            {reshdrs} {response_body}
+
+        """
+        ).format(
+            req=record.req,
+            res=record.res,
+            reqhdrs=self._formatHeaders(record.req.headers),
+            reshdrs=self._formatHeaders(record.res.headers),
+            request_body=self._formatBody(record.req.body, "Request"),
+            response_body=self._formatBody(record.res.content, "Response"),
+        )
 
         return result
```

### Comparing `django-log-outgoing-requests-0.1.0/log_outgoing_requests/handlers.py` & `django-log-outgoing-requests-0.2.0/log_outgoing_requests/handlers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,91 @@
+# NOTE: Avoid import Django specifics at the module level to prevent circular imports.
+# The handler is loaded eagerly at django startup when configuring settings.
 import logging
 import traceback
+from datetime import datetime
+from logging import LogRecord
+from typing import Union, cast
 from urllib.parse import urlparse
 
-from django.conf import settings
+from requests.models import PreparedRequest, Response
+
+
+class RequestLogRecord(LogRecord):
+    requested_at: datetime
+    req: PreparedRequest
+    res: Response
+
+
+AnyLogRecord = Union[LogRecord, RequestLogRecord]
+
+
+def is_request_log_record(record: AnyLogRecord) -> bool:
+    attrs = ("requested_at", "req", "res")
+    if any(not hasattr(record, attr) for attr in attrs):
+        return False
+    return True
 
 
 class DatabaseOutgoingRequestsHandler(logging.Handler):
-    def emit(self, record):
-        if settings.LOG_OUTGOING_REQUESTS_DB_SAVE:
-            from .models import OutgoingRequestsLog
-
-            trace = None
-
-            # save only the requests coming from the library requests
-            if record and record.getMessage() == "Outgoing request":
-                safe_req_headers = record.req.headers.copy()
-
-                if "Authorization" in safe_req_headers:
-                    safe_req_headers["Authorization"] = "***hidden***"
-
-                if record.exc_info:
-                    trace = traceback.format_exc()
-
-                parsed_url = urlparse(record.req.url)
-                kwargs = {
-                    "url": record.req.url,
-                    "hostname": parsed_url.hostname,
-                    "params": parsed_url.params,
-                    "status_code": record.res.status_code,
-                    "method": record.req.method,
-                    "req_content_type": record.req.headers.get("Content-Type", ""),
-                    "res_content_type": record.res.headers.get("Content-Type", ""),
-                    "timestamp": record.requested_at,
-                    "response_ms": int(record.res.elapsed.total_seconds() * 1000),
-                    "req_headers": self.format_headers(safe_req_headers),
-                    "res_headers": self.format_headers(record.res.headers),
-                    "trace": trace,
-                }
+    def emit(self, record: AnyLogRecord):
+        from .models import OutgoingRequestsLog, OutgoingRequestsLogConfig
+        from .utils import process_body
+
+        config = cast(OutgoingRequestsLogConfig, OutgoingRequestsLogConfig.get_solo())
+        if not config.save_logs_enabled:
+            return
+
+        # skip requests not coming from the library requests
+        if not record or not is_request_log_record(record):
+            return
+        # Typescript type predicates would be cool here :)
+        record = cast(RequestLogRecord, record)
+
+        scrubbed_req_headers = record.req.headers.copy()
+
+        if "Authorization" in scrubbed_req_headers:
+            scrubbed_req_headers["Authorization"] = "***hidden***"
+
+        trace = traceback.format_exc() if record.exc_info else ""
+
+        parsed_url = urlparse(record.req.url)
+        kwargs = {
+            "url": record.req.url,
+            "hostname": parsed_url.netloc,
+            "params": parsed_url.params,
+            "status_code": record.res.status_code,
+            "method": record.req.method,
+            "timestamp": record.requested_at,
+            "response_ms": int(record.res.elapsed.total_seconds() * 1000),
+            "req_headers": self.format_headers(scrubbed_req_headers),
+            "res_headers": self.format_headers(record.res.headers),
+            "trace": trace,
+        }
+
+        if config.save_body_enabled:
+            # check request
+            processed_request_body = process_body(record.req, config)
+            if processed_request_body.allow_saving_to_db:
+                kwargs.update(
+                    {
+                        "req_content_type": processed_request_body.content_type,
+                        "req_body": processed_request_body.content,
+                        "req_body_encoding": processed_request_body.encoding,
+                    }
+                )
+
+            # check response
+            processed_response_body = process_body(record.res, config)
+            if processed_response_body.allow_saving_to_db:
+                kwargs.update(
+                    {
+                        "res_content_type": processed_response_body.content_type,
+                        "res_body": processed_response_body.content,
+                        "res_body_encoding": processed_response_body.encoding,
+                    }
+                )
 
-                OutgoingRequestsLog.objects.create(**kwargs)
+        OutgoingRequestsLog.objects.create(**kwargs)
 
     def format_headers(self, headers):
         return "\n".join(f"{k}: {v}" for k, v in headers.items())
```

### Comparing `django-log-outgoing-requests-0.1.0/log_outgoing_requests/log_requests.py` & `django-log-outgoing-requests-0.2.0/log_outgoing_requests/log_requests.py`

 * *Files 22% similar despite different names*

```diff
@@ -16,20 +16,20 @@
 
 
 def install_outgoing_requests_logging():
     """
     Log all outgoing requests which are made by the library requests during a session.
     """
 
-    if hasattr(Session, "_original_request"):
+    if hasattr(Session, "_initial_request"):
         logger.debug(
-            "Session is already patched OR has an ``_original_request`` attribute."
+            "Session is already patched OR has an ``_initial_request`` attribute."
         )
         return
 
-    Session._original_request = Session.request
+    Session._initial_request = Session.request  # type: ignore
 
     def new_request(self, *args, **kwargs):
         self.hooks["response"].append(hook_requests_logging)
-        return self._original_request(*args, **kwargs)
+        return self._initial_request(*args, **kwargs)
 
     Session.request = new_request
```

### Comparing `django-log-outgoing-requests-0.1.0/log_outgoing_requests/migrations/0001_initial.py` & `django-log-outgoing-requests-0.2.0/log_outgoing_requests/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-log-outgoing-requests-0.1.0/setup.cfg` & `django-log-outgoing-requests-0.2.0/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-log-outgoing-requests
-version = 0.1.0
+version = 0.2.0
 description = Log outgoing requests made by the requests python library
 long_description = file: README.rst
 url = https://github.com/maykinmedia/django-log-outgoing-requests
 project_urls = 
 	Documentation = http://django-log-outgoing-requests.readthedocs.io/en/latest/
 	Changelog = https://github.com/maykinmedia/django-log-outgoing-requests/blob/main/CHANGELOG.rst
 	Bug Tracker = https://github.com/maykinmedia/django-log-outgoing-requests/issues
@@ -18,59 +18,61 @@
 	Framework :: Django
 	Framework :: Django :: 3.2
 	Framework :: Django :: 4.1
 	Intended Audience :: Developers
 	Operating System :: Unix
 	Operating System :: MacOS
 	Operating System :: Microsoft :: Windows
-	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 zip_safe = False
 include_package_data = True
 packages = find:
 install_requires = 
 	django >= 3.2
 	requests
+	django-solo
 tests_require = 
 	pytest
 	pytest-django
 	tox
 	isort
 	black
 	flake8
 	freezegun
 	requests-mock
+	pyquery
 
 [options.packages.find]
 include = 
 	log_outgoing_requests
 	log_outgoing_requests.*
 
 [options.extras_require]
 tests = 
 	pytest
 	pytest-django
+	pyquery
 	tox
 	isort
 	black
 	flake8
 	freezegun
 	requests-mock
 pep8 = flake8
 coverage = pytest-cov
 docs = 
 	sphinx
 	sphinx-rtd-theme
 release = 
-	bumpversion
+	bump2version
 	twine
 
 [aliases]
 test = pytest
 
 [isort]
 combine_as_imports = true
@@ -85,19 +87,25 @@
 known_django = django
 known_first_party = log_outgoing_requests
 sections = FUTURE,STDLIB,DJANGO,THIRDPARTY,FIRSTPARTY,LOCALFOLDER
 
 [tool:pytest]
 testpaths = tests
 DJANGO_SETTINGS_MODULE = testapp.settings
+filterwarnings = 
+	error:DateTimeField .* received a naive datetime:RuntimeWarning:django.db.models.fields
 
 [pep8]
 
 [flake8]
 max-line-length = 88
 exclude = env,.tox,doc
 ignore = E203,W503,E501
 
+[coverage:run]
+branch = True
+source = log_outgoing_requests
+
 [egg_info]
 tag_build = 
 tag_date = 0
```

