# Comparing `tmp/django-happy-decorators-0.2.8.tar.gz` & `tmp/django-happy-decorators-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/django-happy-decorators-0.2.8.tar", last modified: Wed Mar  1 12:45:45 2023, max compression
+gzip compressed data, was "dist/django-happy-decorators-0.2.9.tar", last modified: Wed Mar  1 12:57:26 2023, max compression
```

## Comparing `django-happy-decorators-0.2.8.tar` & `django-happy-decorators-0.2.9.tar`

### file list

```diff
@@ -1,24 +1,26 @@
-drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/
--rw-r--r--   0 hatim.hoho (692240558) 610106715      726 2023-03-01 10:53:17.000000 django-happy-decorators-0.2.8/.gitignore
--rw-r--r--   0 hatim.hoho (692240558) 610106715     1073 2023-01-27 06:39:37.000000 django-happy-decorators-0.2.8/LICENSE
--rw-r--r--   0 hatim.hoho (692240558) 610106715      150 2023-01-27 06:41:06.000000 django-happy-decorators-0.2.8/MANIFEST.in
--rw-r--r--   0 hatim.hoho (692240558) 610106715     6358 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/PKG-INFO
--rw-r--r--   0 hatim.hoho (692240558) 610106715     4863 2023-03-01 09:32:39.000000 django-happy-decorators-0.2.8/README.md
-drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators/
-drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/
--rw-r--r--   0 hatim.hoho (692240558) 610106715       32 2023-03-01 09:40:09.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/__init__.py
--rw-r--r--   0 hatim.hoho (692240558) 610106715      397 2023-01-28 07:51:36.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/asgi.py
--rw-r--r--   0 hatim.hoho (692240558) 610106715     2538 2023-01-28 08:30:32.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/rate_limit.py
--rw-r--r--   0 hatim.hoho (692240558) 610106715     3281 2023-01-28 07:51:54.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/settings.py
--rw-r--r--   0 hatim.hoho (692240558) 610106715      834 2023-01-28 07:52:00.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/urls.py
--rw-r--r--   0 hatim.hoho (692240558) 610106715      397 2023-01-28 07:52:03.000000 django-happy-decorators-0.2.8/django_happy_decorators/decorators/wsgi.py
--rwxr-xr-x   0 hatim.hoho (692240558) 610106715      666 2023-01-28 07:51:13.000000 django-happy-decorators-0.2.8/django_happy_decorators/manage.py
-drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators.egg-info/
--rw-r--r--   0 hatim.hoho (692240558) 610106715     6358 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators.egg-info/PKG-INFO
--rw-r--r--   0 hatim.hoho (692240558) 610106715      614 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators.egg-info/SOURCES.txt
--rw-r--r--   0 hatim.hoho (692240558) 610106715        1 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators.egg-info/dependency_links.txt
--rw-r--r--   0 hatim.hoho (692240558) 610106715       12 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators.egg-info/requires.txt
--rw-r--r--   0 hatim.hoho (692240558) 610106715        1 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/django_happy_decorators.egg-info/top_level.txt
--rw-r--r--   0 hatim.hoho (692240558) 610106715      100 2023-01-27 07:58:11.000000 django-happy-decorators-0.2.8/pyproject.toml
--rw-r--r--   0 hatim.hoho (692240558) 610106715     1085 2023-03-01 12:45:45.000000 django-happy-decorators-0.2.8/setup.cfg
--rw-r--r--   0 hatim.hoho (692240558) 610106715      675 2023-03-01 12:45:28.000000 django-happy-decorators-0.2.8/setup.py
+drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:57:26.000000 django-happy-decorators-0.2.9/
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      726 2023-03-01 10:53:17.000000 django-happy-decorators-0.2.9/.gitignore
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     1073 2023-01-27 06:39:37.000000 django-happy-decorators-0.2.9/LICENSE
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      150 2023-01-27 06:41:06.000000 django-happy-decorators-0.2.9/MANIFEST.in
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     6743 2023-03-01 12:57:26.000000 django-happy-decorators-0.2.9/PKG-INFO
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     4863 2023-03-01 09:32:39.000000 django-happy-decorators-0.2.9/README.md
+drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:57:26.000000 django-happy-decorators-0.2.9/django_happy_decorators/
+drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:57:26.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/
+-rw-r--r--   0 hatim.hoho (692240558) 610106715       32 2023-03-01 09:40:09.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/__init__.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      397 2023-01-28 07:51:36.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/asgi.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     1652 2023-03-01 09:01:21.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/if_not.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     2538 2023-01-28 08:30:32.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/rate_limit.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     3281 2023-01-28 07:51:54.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/settings.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     4038 2023-01-29 07:08:27.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/tests.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      834 2023-01-28 07:52:00.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/urls.py
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      397 2023-01-28 07:52:03.000000 django-happy-decorators-0.2.9/django_happy_decorators/decorators/wsgi.py
+-rwxr-xr-x   0 hatim.hoho (692240558) 610106715      666 2023-01-28 07:51:13.000000 django-happy-decorators-0.2.9/django_happy_decorators/manage.py
+drwxr-xr-x   0 hatim.hoho (692240558) 610106715        0 2023-03-01 12:57:26.000000 django-happy-decorators-0.2.9/django_happy_decorators.egg-info/
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     6743 2023-03-01 12:57:25.000000 django-happy-decorators-0.2.9/django_happy_decorators.egg-info/PKG-INFO
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      703 2023-03-01 12:57:25.000000 django-happy-decorators-0.2.9/django_happy_decorators.egg-info/SOURCES.txt
+-rw-r--r--   0 hatim.hoho (692240558) 610106715        1 2023-03-01 12:57:25.000000 django-happy-decorators-0.2.9/django_happy_decorators.egg-info/dependency_links.txt
+-rw-r--r--   0 hatim.hoho (692240558) 610106715       12 2023-03-01 12:57:25.000000 django-happy-decorators-0.2.9/django_happy_decorators.egg-info/requires.txt
+-rw-r--r--   0 hatim.hoho (692240558) 610106715       24 2023-03-01 12:57:25.000000 django-happy-decorators-0.2.9/django_happy_decorators.egg-info/top_level.txt
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      100 2023-01-27 07:58:11.000000 django-happy-decorators-0.2.9/pyproject.toml
+-rw-r--r--   0 hatim.hoho (692240558) 610106715     1085 2023-03-01 12:57:26.000000 django-happy-decorators-0.2.9/setup.cfg
+-rw-r--r--   0 hatim.hoho (692240558) 610106715      225 2023-03-01 12:52:03.000000 django-happy-decorators-0.2.9/setup.py
```

### Comparing `django-happy-decorators-0.2.8/.gitignore` & `django-happy-decorators-0.2.9/.gitignore`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/LICENSE` & `django-happy-decorators-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/PKG-INFO` & `django-happy-decorators-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: django-happy-decorators
-Version: 0.2.8
-Summary: Django Happy Decorators - a collection of helper decorators for Django
+Version: 0.2.9
+Summary: Happy decorators for Django is a set of decorators for Django apps and views to make your life easier.
 Home-page: https://github.com/hatimmakki/django-happy-decorators
-Author: Hatim Makki Hoho
-Author-email: hatim.makki@gmail.com
 License: MIT
 Description: # Django Happy Decorators
         
         [![Build Status](https://travis-ci.org/rodrigobdz/django-happy-decorators.svg?branch=master)](https://travis-ci.org/rodrigobdz/django-happy-decorators)
         [![Coverage Status](https://coveralls.io/repos/github/rodrigobdz/django-happy-decorators/badge.svg?branch=master)](https://coveralls.io/github/rodrigobdz/django-happy-decorators?branch=master)
         [![PyPI version](https://badge.fury.io/py/django-happy-decorators.svg)](https://badge.fury.io/py/django-happy-decorators)
         [![Documentation Status](https://readthedocs.org/projects/django-happy-decorators/badge/?version=latest)](https://django-happy-decorators.readthedocs.io/en/latest/?badge=latest)
@@ -125,12 +123,19 @@
         
         Django Rate Limit is released under the MIT License.
         
         This is just a sample and you can adjust the content as per your package and also add more details like screenshots, sample code etc.
         
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `django-happy-decorators-0.2.8/README.md` & `django-happy-decorators-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/django_happy_decorators/decorators/rate_limit.py` & `django-happy-decorators-0.2.9/django_happy_decorators/decorators/rate_limit.py`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/django_happy_decorators/decorators/settings.py` & `django-happy-decorators-0.2.9/django_happy_decorators/decorators/settings.py`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/django_happy_decorators/decorators/urls.py` & `django-happy-decorators-0.2.9/django_happy_decorators/decorators/urls.py`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/django_happy_decorators/manage.py` & `django-happy-decorators-0.2.9/django_happy_decorators/manage.py`

 * *Files identical despite different names*

### Comparing `django-happy-decorators-0.2.8/django_happy_decorators.egg-info/PKG-INFO` & `django-happy-decorators-0.2.9/django_happy_decorators.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 Metadata-Version: 2.1
 Name: django-happy-decorators
-Version: 0.2.8
-Summary: Django Happy Decorators - a collection of helper decorators for Django
+Version: 0.2.9
+Summary: Happy decorators for Django is a set of decorators for Django apps and views to make your life easier.
 Home-page: https://github.com/hatimmakki/django-happy-decorators
-Author: Hatim Makki Hoho
-Author-email: hatim.makki@gmail.com
 License: MIT
 Description: # Django Happy Decorators
         
         [![Build Status](https://travis-ci.org/rodrigobdz/django-happy-decorators.svg?branch=master)](https://travis-ci.org/rodrigobdz/django-happy-decorators)
         [![Coverage Status](https://coveralls.io/repos/github/rodrigobdz/django-happy-decorators/badge.svg?branch=master)](https://coveralls.io/github/rodrigobdz/django-happy-decorators?branch=master)
         [![PyPI version](https://badge.fury.io/py/django-happy-decorators.svg)](https://badge.fury.io/py/django-happy-decorators)
         [![Documentation Status](https://readthedocs.org/projects/django-happy-decorators/badge/?version=latest)](https://django-happy-decorators.readthedocs.io/en/latest/?badge=latest)
@@ -125,12 +123,19 @@
         
         Django Rate Limit is released under the MIT License.
         
         This is just a sample and you can adjust the content as per your package and also add more details like screenshots, sample code etc.
         
         
 Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: Implementation :: CPython
+Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `django-happy-decorators-0.2.8/django_happy_decorators.egg-info/SOURCES.txt` & `django-happy-decorators-0.2.9/django_happy_decorators.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -9,11 +9,13 @@
 django_happy_decorators.egg-info/PKG-INFO
 django_happy_decorators.egg-info/SOURCES.txt
 django_happy_decorators.egg-info/dependency_links.txt
 django_happy_decorators.egg-info/requires.txt
 django_happy_decorators.egg-info/top_level.txt
 django_happy_decorators/decorators/__init__.py
 django_happy_decorators/decorators/asgi.py
+django_happy_decorators/decorators/if_not.py
 django_happy_decorators/decorators/rate_limit.py
 django_happy_decorators/decorators/settings.py
+django_happy_decorators/decorators/tests.py
 django_happy_decorators/decorators/urls.py
 django_happy_decorators/decorators/wsgi.py
```

### Comparing `django-happy-decorators-0.2.8/setup.cfg` & `django-happy-decorators-0.2.9/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-happy-decorators
-version = 0.2.7
+version = 0.2.9
 description = Happy decorators for Django is a set of decorators for Django apps and views to make your life easier.
 description-file = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 url = https://github.com/hatimmakki/django-happy-decorators
 license = MIT
 classifiers =
```

