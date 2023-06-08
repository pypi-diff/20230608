# Comparing `tmp/django-bootstrap3-9.0.0.tar.gz` & `tmp/django-bootstrap3-9.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-bootstrap3-9.0.0.tar", last modified: Tue Jul 11 17:38:21 2017, max compression
+gzip compressed data, was "dist/django-bootstrap3-9.1.0.tar", last modified: Fri Oct 27 12:01:03 2017, max compression
```

## Comparing `django-bootstrap3-9.0.0.tar` & `django-bootstrap3-9.1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/
--rw-r--r--   0 dylan      (501) staff       (20)      845 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/AUTHORS.rst
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/bootstrap3/
--rw-r--r--   0 dylan      (501) staff       (20)     6148 2013-09-18 19:12:47.000000 django-bootstrap3-9.0.0/bootstrap3/.DS_Store
--rw-r--r--   0 dylan      (501) staff       (20)       47 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/bootstrap3/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     3145 2017-05-05 05:17:43.000000 django-bootstrap3-9.0.0/bootstrap3/bootstrap.py
--rw-r--r--   0 dylan      (501) staff       (20)     1289 2017-02-23 08:09:26.000000 django-bootstrap3-9.0.0/bootstrap3/components.py
--rw-r--r--   0 dylan      (501) staff       (20)      268 2014-03-29 05:49:08.000000 django-bootstrap3-9.0.0/bootstrap3/exceptions.py
--rw-r--r--   0 dylan      (501) staff       (20)     5615 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/bootstrap3/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)      439 2015-08-15 05:34:54.000000 django-bootstrap3-9.0.0/bootstrap3/legacy.py
--rw-r--r--   0 dylan      (501) staff       (20)       75 2014-03-29 05:49:08.000000 django-bootstrap3-9.0.0/bootstrap3/models.py
--rw-r--r--   0 dylan      (501) staff       (20)    22181 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/bootstrap3/renderers.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/bootstrap3/templates/
--rw-r--r--   0 dylan      (501) staff       (20)     6148 2013-09-18 05:14:04.000000 django-bootstrap3-9.0.0/bootstrap3/templates/.DS_Store
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/
--rw-r--r--   0 dylan      (501) staff       (20)     1209 2017-02-23 08:17:17.000000 django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/bootstrap3.html
--rw-r--r--   0 dylan      (501) staff       (20)      167 2016-09-16 09:42:08.000000 django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/field_help_text_and_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      272 2014-05-08 05:43:41.000000 django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/form_errors.html
--rw-r--r--   0 dylan      (501) staff       (20)      274 2016-02-24 08:54:47.000000 django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/messages.html
--rw-r--r--   0 dylan      (501) staff       (20)     1508 2016-09-16 09:42:08.000000 django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/pagination.html
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/bootstrap3/templatetags/
--rw-r--r--   0 dylan      (501) staff       (20)       24 2013-12-05 07:45:15.000000 django-bootstrap3-9.0.0/bootstrap3/templatetags/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)    22582 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/bootstrap3/templatetags/bootstrap3.py
--rw-r--r--   0 dylan      (501) staff       (20)    29373 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/bootstrap3/tests.py
--rw-r--r--   0 dylan      (501) staff       (20)      648 2014-08-09 04:56:17.000000 django-bootstrap3-9.0.0/bootstrap3/text.py
--rw-r--r--   0 dylan      (501) staff       (20)     4573 2017-02-23 08:09:26.000000 django-bootstrap3-9.0.0/bootstrap3/utils.py
--rw-r--r--   0 dylan      (501) staff       (20)     3252 2014-01-30 14:59:43.000000 django-bootstrap3-9.0.0/CONTRIBUTING.rst
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/demo/
--rw-r--r--   0 dylan      (501) staff       (20)     8196 2014-11-19 12:03:17.000000 django-bootstrap3-9.0.0/demo/.DS_Store
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/demo/demo/
--rw-r--r--   0 dylan      (501) staff       (20)        0 2013-09-01 05:34:33.000000 django-bootstrap3-9.0.0/demo/demo/__init__.py
--rw-r--r--   0 dylan      (501) staff       (20)     1622 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/demo/demo/forms.py
--rw-r--r--   0 dylan      (501) staff       (20)     5217 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/demo/demo/settings.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/demo/demo/templates/
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/
--rw-r--r--   0 dylan      (501) staff       (20)      910 2016-02-24 08:54:47.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/base.html
--rw-r--r--   0 dylan      (501) staff       (20)      118 2014-02-28 07:38:16.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/bootstrap.html
--rw-r--r--   0 dylan      (501) staff       (20)      309 2014-07-07 10:48:46.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/form.html
--rw-r--r--   0 dylan      (501) staff       (20)      472 2017-01-06 15:11:32.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/form_by_field.html
--rw-r--r--   0 dylan      (501) staff       (20)      373 2014-08-11 06:53:51.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/form_horizontal.html
--rw-r--r--   0 dylan      (501) staff       (20)      361 2014-02-28 07:05:26.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/form_inline.html
--rw-r--r--   0 dylan      (501) staff       (20)      419 2014-03-05 10:24:27.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/form_with_files.html
--rw-r--r--   0 dylan      (501) staff       (20)      353 2014-06-04 06:00:57.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/formset.html
--rw-r--r--   0 dylan      (501) staff       (20)      199 2016-02-24 08:54:47.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/home.html
--rw-r--r--   0 dylan      (501) staff       (20)      324 2015-08-20 08:48:51.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/misc.html
--rw-r--r--   0 dylan      (501) staff       (20)      489 2013-09-06 10:19:19.000000 django-bootstrap3-9.0.0/demo/demo/templates/demo/pagination.html
--rw-r--r--   0 dylan      (501) staff       (20)      947 2016-09-16 09:42:08.000000 django-bootstrap3-9.0.0/demo/demo/urls.py
--rw-r--r--   0 dylan      (501) staff       (20)     2753 2016-02-24 08:54:47.000000 django-bootstrap3-9.0.0/demo/demo/views.py
--rw-r--r--   0 dylan      (501) staff       (20)     1428 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/demo/demo/wsgi.py
--rw-r--r--   0 dylan      (501) staff       (20)      247 2013-10-16 06:05:32.000000 django-bootstrap3-9.0.0/demo/manage.py
-drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/django_bootstrap3.egg-info/
--rw-r--r--   0 dylan      (501) staff       (20)        1 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/django_bootstrap3.egg-info/dependency_links.txt
--rw-r--r--   0 dylan      (501) staff       (20)        1 2014-02-20 06:45:20.000000 django-bootstrap3-9.0.0/django_bootstrap3.egg-info/not-zip-safe
--rw-r--r--   0 dylan      (501) staff       (20)    15830 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/django_bootstrap3.egg-info/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     1492 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/django_bootstrap3.egg-info/SOURCES.txt
--rw-r--r--   0 dylan      (501) staff       (20)       11 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/django_bootstrap3.egg-info/top_level.txt
--rw-r--r--   0 dylan      (501) staff       (20)     8341 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/HISTORY.rst
--rw-r--r--   0 dylan      (501) staff       (20)     1541 2017-07-11 17:37:49.000000 django-bootstrap3-9.0.0/LICENSE
--rw-r--r--   0 dylan      (501) staff       (20)      177 2017-02-23 08:17:17.000000 django-bootstrap3-9.0.0/MANIFEST.in
--rw-r--r--   0 dylan      (501) staff       (20)    15830 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/PKG-INFO
--rw-r--r--   0 dylan      (501) staff       (20)     2603 2017-05-05 05:17:43.000000 django-bootstrap3-9.0.0/README.rst
--rw-r--r--   0 dylan      (501) staff       (20)       38 2017-07-11 17:38:21.000000 django-bootstrap3-9.0.0/setup.cfg
--rwxr-xr-x   0 dylan      (501) staff       (20)     2024 2017-05-04 06:14:33.000000 django-bootstrap3-9.0.0/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/demo/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/demo/demo/
+-rw-r--r--   0 dylan      (501) staff       (20)        0 2013-09-01 05:34:33.000000 django-bootstrap3-9.1.0/demo/demo/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1622 2017-07-11 17:37:49.000000 django-bootstrap3-9.1.0/demo/demo/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)     5217 2017-07-11 17:37:49.000000 django-bootstrap3-9.1.0/demo/demo/settings.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/demo/demo/templates/
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/
+-rw-r--r--   0 dylan      (501) staff       (20)      118 2014-02-28 07:38:16.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/bootstrap.html
+-rw-r--r--   0 dylan      (501) staff       (20)      353 2014-06-04 06:00:57.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/formset.html
+-rw-r--r--   0 dylan      (501) staff       (20)      309 2014-07-07 10:48:46.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/form.html
+-rw-r--r--   0 dylan      (501) staff       (20)      199 2016-02-24 08:54:47.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/home.html
+-rw-r--r--   0 dylan      (501) staff       (20)      489 2013-09-06 10:19:19.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/pagination.html
+-rw-r--r--   0 dylan      (501) staff       (20)      910 2016-02-24 08:54:47.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/base.html
+-rw-r--r--   0 dylan      (501) staff       (20)      361 2014-02-28 07:05:26.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/form_inline.html
+-rw-r--r--   0 dylan      (501) staff       (20)      472 2017-01-06 15:11:32.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/form_by_field.html
+-rw-r--r--   0 dylan      (501) staff       (20)      419 2014-03-05 10:24:27.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/form_with_files.html
+-rw-r--r--   0 dylan      (501) staff       (20)      373 2014-08-11 06:53:51.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/form_horizontal.html
+-rw-r--r--   0 dylan      (501) staff       (20)      324 2015-08-20 08:48:51.000000 django-bootstrap3-9.1.0/demo/demo/templates/demo/misc.html
+-rw-r--r--   0 dylan      (501) staff       (20)      947 2016-09-16 09:42:08.000000 django-bootstrap3-9.1.0/demo/demo/urls.py
+-rw-r--r--   0 dylan      (501) staff       (20)     2753 2016-02-24 08:54:47.000000 django-bootstrap3-9.1.0/demo/demo/views.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1428 2017-07-11 17:37:49.000000 django-bootstrap3-9.1.0/demo/demo/wsgi.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8196 2014-11-19 12:03:17.000000 django-bootstrap3-9.1.0/demo/.DS_Store
+-rw-r--r--   0 dylan      (501) staff       (20)      247 2013-10-16 06:05:32.000000 django-bootstrap3-9.1.0/demo/manage.py
+-rw-r--r--   0 dylan      (501) staff       (20)    16274 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)     1541 2017-07-11 17:37:49.000000 django-bootstrap3-9.1.0/LICENSE
+-rw-r--r--   0 dylan      (501) staff       (20)     3252 2014-01-30 14:59:43.000000 django-bootstrap3-9.1.0/CONTRIBUTING.rst
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/django_bootstrap3.egg-info/
+-rw-r--r--   0 dylan      (501) staff       (20)    16274 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/django_bootstrap3.egg-info/PKG-INFO
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2014-02-20 06:45:20.000000 django-bootstrap3-9.1.0/django_bootstrap3.egg-info/not-zip-safe
+-rw-r--r--   0 dylan      (501) staff       (20)     1492 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/django_bootstrap3.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan      (501) staff       (20)       11 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/django_bootstrap3.egg-info/top_level.txt
+-rw-r--r--   0 dylan      (501) staff       (20)        1 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/django_bootstrap3.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan      (501) staff       (20)      177 2017-02-23 08:17:17.000000 django-bootstrap3-9.1.0/MANIFEST.in
+-rwxr-xr-x   0 dylan      (501) staff       (20)     2024 2017-05-04 06:14:33.000000 django-bootstrap3-9.1.0/setup.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/bootstrap3/
+-rw-r--r--   0 dylan      (501) staff       (20)     3145 2017-05-05 05:17:43.000000 django-bootstrap3-9.1.0/bootstrap3/bootstrap.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/bootstrap3/templatetags/
+-rw-r--r--   0 dylan      (501) staff       (20)    22639 2017-10-27 11:59:33.000000 django-bootstrap3-9.1.0/bootstrap3/templatetags/bootstrap3.py
+-rw-r--r--   0 dylan      (501) staff       (20)       24 2013-12-05 07:45:15.000000 django-bootstrap3-9.1.0/bootstrap3/templatetags/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)     6148 2013-09-18 19:12:47.000000 django-bootstrap3-9.1.0/bootstrap3/.DS_Store
+-rw-r--r--   0 dylan      (501) staff       (20)      439 2015-08-15 05:34:54.000000 django-bootstrap3-9.1.0/bootstrap3/legacy.py
+-rw-r--r--   0 dylan      (501) staff       (20)       75 2014-03-29 05:49:08.000000 django-bootstrap3-9.1.0/bootstrap3/models.py
+-rw-r--r--   0 dylan      (501) staff       (20)       47 2017-10-27 11:59:33.000000 django-bootstrap3-9.1.0/bootstrap3/__init__.py
+-rw-r--r--   0 dylan      (501) staff       (20)    22223 2017-10-27 11:59:33.000000 django-bootstrap3-9.1.0/bootstrap3/renderers.py
+-rw-r--r--   0 dylan      (501) staff       (20)     5615 2017-07-11 17:37:49.000000 django-bootstrap3-9.1.0/bootstrap3/forms.py
+-rw-r--r--   0 dylan      (501) staff       (20)     4573 2017-02-23 08:09:26.000000 django-bootstrap3-9.1.0/bootstrap3/utils.py
+-rw-r--r--   0 dylan      (501) staff       (20)      648 2014-08-09 04:56:17.000000 django-bootstrap3-9.1.0/bootstrap3/text.py
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/bootstrap3/templates/
+-rw-r--r--   0 dylan      (501) staff       (20)     6148 2013-09-18 05:14:04.000000 django-bootstrap3-9.1.0/bootstrap3/templates/.DS_Store
+drwxr-xr-x   0 dylan      (501) staff       (20)        0 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/
+-rw-r--r--   0 dylan      (501) staff       (20)     1508 2016-09-16 09:42:08.000000 django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/pagination.html
+-rw-r--r--   0 dylan      (501) staff       (20)      272 2014-05-08 05:43:41.000000 django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/form_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)      167 2016-09-16 09:42:08.000000 django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/field_help_text_and_errors.html
+-rw-r--r--   0 dylan      (501) staff       (20)     1209 2017-02-23 08:17:17.000000 django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/bootstrap3.html
+-rw-r--r--   0 dylan      (501) staff       (20)      274 2016-02-24 08:54:47.000000 django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/messages.html
+-rw-r--r--   0 dylan      (501) staff       (20)      268 2014-03-29 05:49:08.000000 django-bootstrap3-9.1.0/bootstrap3/exceptions.py
+-rw-r--r--   0 dylan      (501) staff       (20)     1289 2017-02-23 08:09:26.000000 django-bootstrap3-9.1.0/bootstrap3/components.py
+-rw-r--r--   0 dylan      (501) staff       (20)    30209 2017-10-27 11:59:33.000000 django-bootstrap3-9.1.0/bootstrap3/tests.py
+-rw-r--r--   0 dylan      (501) staff       (20)     8624 2017-10-27 11:59:33.000000 django-bootstrap3-9.1.0/HISTORY.rst
+-rw-r--r--   0 dylan      (501) staff       (20)      845 2017-07-11 17:37:49.000000 django-bootstrap3-9.1.0/AUTHORS.rst
+-rw-r--r--   0 dylan      (501) staff       (20)       38 2017-10-27 12:01:03.000000 django-bootstrap3-9.1.0/setup.cfg
+-rw-r--r--   0 dylan      (501) staff       (20)     2626 2017-10-27 11:59:33.000000 django-bootstrap3-9.1.0/README.rst
```

### Comparing `django-bootstrap3-9.0.0/AUTHORS.rst` & `django-bootstrap3-9.1.0/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/.DS_Store` & `django-bootstrap3-9.1.0/bootstrap3/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/bootstrap.py` & `django-bootstrap3-9.1.0/bootstrap3/bootstrap.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/components.py` & `django-bootstrap3-9.1.0/bootstrap3/components.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/forms.py` & `django-bootstrap3-9.1.0/bootstrap3/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/renderers.py` & `django-bootstrap3-9.1.0/bootstrap3/renderers.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,20 +251,22 @@
 
         self.widget = field.field.widget
         self.is_multi_widget = isinstance(field.field.widget, MultiWidget)
         self.initial_attrs = self.widget.attrs.copy()
         self.field_help = text_value(mark_safe(field.help_text)) if self.show_help and field.help_text else ''
         self.field_errors = [conditional_escape(text_value(error)) for error in field.errors]
 
+        self.label = kwargs.get('label', field.label)
+
         if 'placeholder' in kwargs:
             # Find the placeholder in kwargs, even if it's empty
             self.placeholder = kwargs['placeholder']
         elif get_bootstrap_setting('set_placeholder'):
             # If not found, see if we set the label
-            self.placeholder = field.label
+            self.placeholder = self.label
         else:
             # Or just set it to empty
             self.placeholder = ''
         if self.placeholder:
             self.placeholder = text_value(mark_safe(self.placeholder))
 
         self.addon_before = kwargs.get('addon_before', self.widget.attrs.pop('addon_before', ''))
@@ -386,15 +388,15 @@
         for k, v in mapping:
             html = html.replace(k, v)
         return html
 
     def put_inside_label(self, html):
         content = '{field} {label}'.format(
             field=html,
-            label=self.field.label,
+            label=self.label,
         )
         return render_label(
             content=mark_safe(content),
             label_for=self.field.id_for_label,
             label_title=escape(strip_tags(self.field_help))
         )
 
@@ -499,15 +501,15 @@
             label_class = add_css_class(label_class, 'sr-only')
         return add_css_class(label_class, 'control-label')
 
     def get_label(self):
         if isinstance(self.widget, CheckboxInput):
             label = None
         else:
-            label = self.field.label
+            label = self.label
         if self.layout == 'horizontal' and not label:
             return mark_safe('&#160;')
         return label
 
     def add_label(self, html):
         label = self.get_label()
         if label:
```

### Comparing `django-bootstrap3-9.0.0/bootstrap3/templates/.DS_Store` & `django-bootstrap3-9.1.0/bootstrap3/templates/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/bootstrap3.html` & `django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/bootstrap3.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/templates/bootstrap3/pagination.html` & `django-bootstrap3-9.1.0/bootstrap3/templates/bootstrap3/pagination.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/templatetags/bootstrap3.py` & `django-bootstrap3-9.1.0/bootstrap3/templatetags/bootstrap3.py`

 * *Files 1% similar despite different names*

```diff
@@ -439,15 +439,18 @@
             One of the following values:
 
                 * ``'small'``
                 * ``'medium'``
                 * ``'large'``
 
         placeholder
-            Sets the placeholder text of a textbox
+            Set/overwrite the field's placeholder.
+
+        label
+            Overwrite the field's label.
 
         horizontal_label_class
             Class used on the label when the ``layout`` is set to ``horizontal``.
 
             :default: ``'col-md-3'``. Can be changed in :doc:`settings`
 
         horizontal_field_class
@@ -675,15 +678,15 @@
 
     **Usage**::
 
         {% bootstrap_alert content %}
 
     **Example**::
 
-        {% bootstrap_alert "Something went wrong" alert_type='error' %}
+        {% bootstrap_alert "Something went wrong" alert_type='danger' %}
 
     """
     return render_alert(content, alert_type, dismissable)
 
 
 @register.tag('buttons')
 def bootstrap_buttons(parser, token):
```

### Comparing `django-bootstrap3-9.0.0/bootstrap3/tests.py` & `django-bootstrap3-9.1.0/bootstrap3/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import re
 
 from django import forms
 from django.contrib.admin.widgets import AdminSplitDateTime
 from django.contrib.messages import constants as DEFAULT_MESSAGE_LEVELS
 from django.forms.formsets import formset_factory
 from django.template import engines
-from django.test import TestCase
+from django.test import TestCase, override_settings
 
 from .bootstrap import DBS3_SET_REQUIRED_SET_DISABLED
 from .exceptions import BootstrapError
 from .text import text_value, text_concat
 from .utils import add_css_class, render_tag
 
 try:
@@ -127,15 +127,15 @@
 
 class TestFormWithoutRequiredClass(TestForm):
     required_css_class = ''
 
 
 def render_template(text, context=None):
     """
-    Create a template ``text`` that first loads bootstrap3.
+    Create a template ``text``
     """
     template = engines['django'].from_string(text)
     if not context:
         context = {}
     return template.render(context)
 
 
@@ -575,14 +575,33 @@
         self.assertEqual('<label for="subject">foobar</label>', res)
 
     def test_attributes_consistency(self):
         form = TestForm()
         attrs = form.fields['addon'].widget.attrs.copy()
         self.assertEqual(attrs, form.fields['addon'].widget.attrs)
 
+    def test_placeholder(self):
+        res = render_template_with_form('{% bootstrap_field form.sender %}')
+        self.assertIn('placeholder="Sender', res)
+
+    def test_overwrite_placeholder(self):
+        res = render_template_with_form('{% bootstrap_field form.sender placeholder="foo" %}')
+        self.assertIn('placeholder="foo', res)
+
+        # If set_placeholder is set, also consider label override for placeholder
+        res = render_template_with_form('{% bootstrap_field form.sender label="foo" %}')
+        self.assertNotIn('Sender', res)
+        self.assertIn('placeholder="foo', res)
+        self.assertIn('foo</label>', res)
+
+    def test_overwrite_label(self):
+        res = render_template_with_form('{% bootstrap_field form.sender label="foo" %}')
+        self.assertNotIn('Sender', res)
+        self.assertIn('foo', res)
+
 
 class ComponentsTest(TestCase):
     def test_icon(self):
         res = render_template_with_form('{% bootstrap_icon "star" %}')
         self.assertEqual(
             res.strip(), '<span class="glyphicon glyphicon-star"></span>')
         res = render_template_with_form('{% bootstrap_icon "star" title="alpha centauri" %}')
```

### Comparing `django-bootstrap3-9.0.0/bootstrap3/text.py` & `django-bootstrap3-9.1.0/bootstrap3/text.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/bootstrap3/utils.py` & `django-bootstrap3-9.1.0/bootstrap3/utils.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/CONTRIBUTING.rst` & `django-bootstrap3-9.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/.DS_Store` & `django-bootstrap3-9.1.0/demo/.DS_Store`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/demo/forms.py` & `django-bootstrap3-9.1.0/demo/demo/forms.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/demo/settings.py` & `django-bootstrap3-9.1.0/demo/demo/settings.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/demo/templates/demo/base.html` & `django-bootstrap3-9.1.0/demo/demo/templates/demo/base.html`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/demo/urls.py` & `django-bootstrap3-9.1.0/demo/demo/urls.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/demo/views.py` & `django-bootstrap3-9.1.0/demo/demo/views.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/demo/demo/wsgi.py` & `django-bootstrap3-9.1.0/demo/demo/wsgi.py`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/django_bootstrap3.egg-info/PKG-INFO` & `django-bootstrap3-9.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: django-bootstrap3
-Version: 9.0.0
+Version: 9.1.0
 Summary: Bootstrap support for Django projects
 Home-page: https://github.com/dyve/django-bootstrap3
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: Apache License 2.0
+Description-Content-Type: UNKNOWN
 Description: ======================
         Bootstrap 3 for Django
         ======================
         
         Write Django as usual, and let ``django-bootstrap3`` make template output into Bootstrap 3 code.
         
         
@@ -24,14 +25,20 @@
             :alt: Latest PyPI version
         
         .. image:: https://img.shields.io/pypi/dm/django-bootstrap3.svg
             :target: https://pypi.python.org/pypi/django-bootstrap3
             :alt: Number of PyPI downloads per month
         
         
+        Looking for Bootstrap 4?
+        ------------------------
+        
+        See https://github.com/zostera/django-bootstrap4.
+        
+        
         Requirements
         ------------
         
         - Python 2.7, 3.3, 3.4, or 3.5
         - Django >= 1.8
         - For details, see https://docs.djangoproject.com/en/dev/faq/install/#faq-python-version-support
         
@@ -49,16 +56,14 @@
         
         2. Add to INSTALLED_APPS in your ``settings.py``:
         
            ``'bootstrap3',``
         
         3. In your templates, load the ``bootstrap3`` library and use the ``bootstrap_*`` tags:
         
-        This app will soon require Django 1.8+, python 2.7+. Thanks for understanding.
-        
         
         Example template
         ----------------
         
            .. code:: Django
         
             {% load bootstrap3 %}
@@ -111,14 +116,23 @@
         
         
         
         History
         -------
         
         
+        9.1.0
+        +++++
+        
+        * Mention `django-bootstrap4 <https://github.com/zostera/django-bootstrap4/>`_ in README
+        * Rewrite `tox` test matrix to focus on Django releases rather than Python versions
+        * Add tests for Django master branch (>= 2)
+        * Add `label` override for `{% bootstrap_field %}`
+        
+        
         9.0.0 (2017-07-11)
         ++++++++++++++++++
         
         * Renamed requirements-dev.txt back to requirements.txt because that suits ReadTheDocs better
         * Added `error_types` support on bootstrap3_form (thanks @mkoistinen and @ickam)
         * **BREAKING** Default setting of `error_types` to `non_field_errors` is different fro behavior in versions < 9
```

### Comparing `django-bootstrap3-9.0.0/django_bootstrap3.egg-info/SOURCES.txt` & `django-bootstrap3-9.1.0/django_bootstrap3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/HISTORY.rst` & `django-bootstrap3-9.1.0/HISTORY.rst`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,22 @@
 .. :changelog:
 
 History
 -------
 
 
+9.1.0
++++++
+
+* Mention `django-bootstrap4 <https://github.com/zostera/django-bootstrap4/>`_ in README
+* Rewrite `tox` test matrix to focus on Django releases rather than Python versions
+* Add tests for Django master branch (>= 2)
+* Add `label` override for `{% bootstrap_field %}`
+
+
 9.0.0 (2017-07-11)
 ++++++++++++++++++
 
 * Renamed requirements-dev.txt back to requirements.txt because that suits ReadTheDocs better
 * Added `error_types` support on bootstrap3_form (thanks @mkoistinen and @ickam)
 * **BREAKING** Default setting of `error_types` to `non_field_errors` is different fro behavior in versions < 9
```

### Comparing `django-bootstrap3-9.0.0/LICENSE` & `django-bootstrap3-9.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-bootstrap3-9.0.0/PKG-INFO` & `django-bootstrap3-9.1.0/django_bootstrap3.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 1.1
 Name: django-bootstrap3
-Version: 9.0.0
+Version: 9.1.0
 Summary: Bootstrap support for Django projects
 Home-page: https://github.com/dyve/django-bootstrap3
 Author: Dylan Verheul
 Author-email: dylan@dyve.net
 License: Apache License 2.0
+Description-Content-Type: UNKNOWN
 Description: ======================
         Bootstrap 3 for Django
         ======================
         
         Write Django as usual, and let ``django-bootstrap3`` make template output into Bootstrap 3 code.
         
         
@@ -24,14 +25,20 @@
             :alt: Latest PyPI version
         
         .. image:: https://img.shields.io/pypi/dm/django-bootstrap3.svg
             :target: https://pypi.python.org/pypi/django-bootstrap3
             :alt: Number of PyPI downloads per month
         
         
+        Looking for Bootstrap 4?
+        ------------------------
+        
+        See https://github.com/zostera/django-bootstrap4.
+        
+        
         Requirements
         ------------
         
         - Python 2.7, 3.3, 3.4, or 3.5
         - Django >= 1.8
         - For details, see https://docs.djangoproject.com/en/dev/faq/install/#faq-python-version-support
         
@@ -49,16 +56,14 @@
         
         2. Add to INSTALLED_APPS in your ``settings.py``:
         
            ``'bootstrap3',``
         
         3. In your templates, load the ``bootstrap3`` library and use the ``bootstrap_*`` tags:
         
-        This app will soon require Django 1.8+, python 2.7+. Thanks for understanding.
-        
         
         Example template
         ----------------
         
            .. code:: Django
         
             {% load bootstrap3 %}
@@ -111,14 +116,23 @@
         
         
         
         History
         -------
         
         
+        9.1.0
+        +++++
+        
+        * Mention `django-bootstrap4 <https://github.com/zostera/django-bootstrap4/>`_ in README
+        * Rewrite `tox` test matrix to focus on Django releases rather than Python versions
+        * Add tests for Django master branch (>= 2)
+        * Add `label` override for `{% bootstrap_field %}`
+        
+        
         9.0.0 (2017-07-11)
         ++++++++++++++++++
         
         * Renamed requirements-dev.txt back to requirements.txt because that suits ReadTheDocs better
         * Added `error_types` support on bootstrap3_form (thanks @mkoistinen and @ickam)
         * **BREAKING** Default setting of `error_types` to `non_field_errors` is different fro behavior in versions < 9
```

### Comparing `django-bootstrap3-9.0.0/README.rst` & `django-bootstrap3-9.1.0/README.rst`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,20 @@
     :alt: Latest PyPI version
 
 .. image:: https://img.shields.io/pypi/dm/django-bootstrap3.svg
     :target: https://pypi.python.org/pypi/django-bootstrap3
     :alt: Number of PyPI downloads per month
 
 
+Looking for Bootstrap 4?
+------------------------
+
+See https://github.com/zostera/django-bootstrap4.
+
+
 Requirements
 ------------
 
 - Python 2.7, 3.3, 3.4, or 3.5
 - Django >= 1.8
 - For details, see https://docs.djangoproject.com/en/dev/faq/install/#faq-python-version-support
 
@@ -41,16 +47,14 @@
 
 2. Add to INSTALLED_APPS in your ``settings.py``:
 
    ``'bootstrap3',``
 
 3. In your templates, load the ``bootstrap3`` library and use the ``bootstrap_*`` tags:
 
-This app will soon require Django 1.8+, python 2.7+. Thanks for understanding.
-
 
 Example template
 ----------------
 
    .. code:: Django
 
     {% load bootstrap3 %}
```

### Comparing `django-bootstrap3-9.0.0/setup.py` & `django-bootstrap3-9.1.0/setup.py`

 * *Files identical despite different names*

