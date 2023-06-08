# Comparing `tmp/Django-Persistent-Message-1.1.1a0.tar.gz` & `tmp/Django-Persistent-Message-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Django-Persistent-Message-1.1.1a0.tar", last modified: Thu Jan 26 20:00:03 2023, max compression
+gzip compressed data, was "Django-Persistent-Message-1.2.tar", last modified: Thu Jun  8 21:54:07 2023, max compression
```

## Comparing `Django-Persistent-Message-1.1.1a0.tar` & `Django-Persistent-Message-1.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-01-26 20:00:02.000000 Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-01-26 20:00:03.000000 Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-26 20:00:02.000000 Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-26 20:00:02.000000 Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-01-26 20:00:02.000000 Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       74 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      596 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-01-26 19:59:59.000000 Django-Persistent-Message-1.1.1a0/persistent_message/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      976 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/fixtures/
--rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/fixtures/test.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      553 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/migrations/0002_auto_20220421_2356.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.641128 Django-Persistent-Message-1.1.1a0/persistent_message/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.641128 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.641128 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/css/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/css/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)     7785 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/css/vendor/bootstrap-datetimepicker.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/js/
--rw-r--r--   0 runner    (1001) docker     (122)    10652 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/js/main.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/js/vendor/
--rw-r--r--   0 runner    (1001) docker     (122)    38510 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/js/vendor/bootstrap-datetimepicker.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/templates/
--rw-r--r--   0 runner    (1001) docker     (122)      117 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/templates/access_denied.html
--rw-r--r--   0 runner    (1001) docker     (122)     5843 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/templates/manage.html
--rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/templates/manage_wrapper.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/tests/
--rw-r--r--   0 runner    (1001) docker     (122)      262 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     8270 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     8837 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (122)      595 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/persistent_message/views/
--rw-r--r--   0 runner    (1001) docker     (122)      881 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/persistent_message/views/api.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-26 20:00:03.645128 Django-Persistent-Message-1.1.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-01-26 19:59:48.000000 Django-Persistent-Message-1.1.1a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.470212 Django-Persistent-Message-1.2/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-06-08 21:54:06.000000 Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-06-08 21:54:07.000000 Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 21:54:06.000000 Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       42 2023-06-08 21:54:06.000000 Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-08 21:54:06.000000 Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       74 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      592 2023-06-08 21:54:07.470212 Django-Persistent-Message-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1928 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-06-08 21:54:05.000000 Django-Persistent-Message-1.2/persistent_message/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      976 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)     2080 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/fixtures/test.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     1912 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      553 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/migrations/0002_auto_20220421_2356.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4427 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.462212 Django-Persistent-Message-1.2/persistent_message/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.462212 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.462212 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/css/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/css/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)     7785 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/css/vendor/bootstrap-datetimepicker.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/js/
+-rw-r--r--   0 runner    (1001) docker     (122)    10652 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/js/main.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/js/vendor/
+-rw-r--r--   0 runner    (1001) docker     (122)    38510 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/static/persistent_message/js/vendor/bootstrap-datetimepicker.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.466212 Django-Persistent-Message-1.2/persistent_message/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)      117 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/templates/access_denied.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5843 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/templates/manage.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1076 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/templates/manage_wrapper.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.470212 Django-Persistent-Message-1.2/persistent_message/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)      262 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8270 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8837 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (122)      595 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 21:54:07.470212 Django-Persistent-Message-1.2/persistent_message/views/
+-rw-r--r--   0 runner    (1001) docker     (122)      881 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5360 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/persistent_message/views/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-06-08 21:54:07.470212 Django-Persistent-Message-1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1224 2023-06-08 21:53:49.000000 Django-Persistent-Message-1.2/setup.py
```

### Comparing `Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/PKG-INFO` & `Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Django-Persistent-Message
-Version: 1.1.1a0
+Version: 1.2
 Summary: Django-Persistent-Message
 Home-page: https://github.com/uw-it-aca/django-persistent-message
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `Django-Persistent-Message-1.1.1a0/Django_Persistent_Message.egg-info/SOURCES.txt` & `Django-Persistent-Message-1.2/Django_Persistent_Message.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/LICENSE` & `Django-Persistent-Message-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/PKG-INFO` & `Django-Persistent-Message-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Django-Persistent-Message
-Version: 1.1.1a0
+Version: 1.2
 Summary: Django-Persistent-Message
 Home-page: https://github.com/uw-it-aca/django-persistent-message
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `Django-Persistent-Message-1.1.1a0/README.md` & `Django-Persistent-Message-1.2/README.md`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/decorators.py` & `Django-Persistent-Message-1.2/persistent_message/decorators.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/fixtures/test.json` & `Django-Persistent-Message-1.2/persistent_message/fixtures/test.json`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/migrations/0001_initial.py` & `Django-Persistent-Message-1.2/persistent_message/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/migrations/0002_auto_20220421_2356.py` & `Django-Persistent-Message-1.2/persistent_message/migrations/0002_auto_20220421_2356.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/models.py` & `Django-Persistent-Message-1.2/persistent_message/models.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/css/vendor/bootstrap-datetimepicker.min.css` & `Django-Persistent-Message-1.2/persistent_message/static/persistent_message/css/vendor/bootstrap-datetimepicker.min.css`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/js/main.js` & `Django-Persistent-Message-1.2/persistent_message/static/persistent_message/js/main.js`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/static/persistent_message/js/vendor/bootstrap-datetimepicker.min.js` & `Django-Persistent-Message-1.2/persistent_message/static/persistent_message/js/vendor/bootstrap-datetimepicker.min.js`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/templates/manage.html` & `Django-Persistent-Message-1.2/persistent_message/templates/manage.html`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/templates/manage_wrapper.html` & `Django-Persistent-Message-1.2/persistent_message/templates/manage_wrapper.html`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/tests/test_api.py` & `Django-Persistent-Message-1.2/persistent_message/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/tests/test_models.py` & `Django-Persistent-Message-1.2/persistent_message/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/urls.py` & `Django-Persistent-Message-1.2/persistent_message/urls.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/views/__init__.py` & `Django-Persistent-Message-1.2/persistent_message/views/__init__.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/persistent_message/views/api.py` & `Django-Persistent-Message-1.2/persistent_message/views/api.py`

 * *Files identical despite different names*

### Comparing `Django-Persistent-Message-1.1.1a0/setup.py` & `Django-Persistent-Message-1.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     name='Django-Persistent-Message',
     version=VERSION,
     packages=['persistent_message'],
     author="UW-IT AXDD",
     author_email="aca-it@uw.edu",
     include_package_data=True,
     install_requires=[
-        'Django<4.0',
+        'Django>=2.2,<5',
         'python-dateutil',
         'bleach<7.0',
     ],
     license='Apache License, Version 2.0',
     description=('Django-Persistent-Message'),
     long_description=README,
     url=url,
```

