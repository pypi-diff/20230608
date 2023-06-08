# Comparing `tmp/django-magnet-data-1.1.4.tar.gz` & `tmp/django-magnet-data-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-magnet-data-1.1.4.tar", max compression
+gzip compressed data, was "django-magnet-data-1.1.5.tar", max compression
```

## Comparing `django-magnet-data-1.1.4.tar` & `django-magnet-data-1.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1066 2022-10-14 16:58:17.859198 django-magnet-data-1.1.4/LICENSE
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/__init__.py
--rw-r--r--   0        0        0      188 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/apps.py
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/currencies/__init__.py
--rw-r--r--   0        0        0     1599 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/currencies/client.py
--rw-r--r--   0        0        0     4702 2023-05-04 20:28:56.929778 django-magnet-data-1.1.4/magnet_data/currencies/currency_pair.py
--rw-r--r--   0        0        0      291 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/currencies/enums.py
--rw-r--r--   0        0        0      802 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/currencies/exceptions.py
--rw-r--r--   0        0        0     1314 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/currencies/models.py
--rw-r--r--   0        0        0       54 2022-12-22 18:15:19.775890 django-magnet-data-1.1.4/magnet_data/currencies/urls.py
--rw-r--r--   0        0        0        0 2023-05-04 20:28:56.913778 django-magnet-data-1.1.4/magnet_data/holidays/__init__.py
--rw-r--r--   0        0        0      216 2023-05-04 20:28:56.917778 django-magnet-data-1.1.4/magnet_data/holidays/admin.py
--rw-r--r--   0        0        0    11689 2023-05-04 20:28:56.917778 django-magnet-data-1.1.4/magnet_data/holidays/enums.py
--rw-r--r--   0        0        0     2162 2023-05-04 20:28:56.917778 django-magnet-data-1.1.4/magnet_data/holidays/models.py
--rw-r--r--   0        0        0     3839 2023-05-04 20:28:56.917778 django-magnet-data-1.1.4/magnet_data/magnet_data_client.py
--rw-r--r--   0        0        0     2249 2022-12-22 18:15:19.779890 django-magnet-data-1.1.4/magnet_data/migrations/0001_initial.py
--rw-r--r--   0        0        0     6827 2023-05-04 20:28:56.917778 django-magnet-data-1.1.4/magnet_data/migrations/0002_holiday.py
--rw-r--r--   0        0        0        0 2022-12-22 18:15:19.779890 django-magnet-data-1.1.4/magnet_data/migrations/__init__.py
--rw-r--r--   0        0        0      118 2023-05-04 20:28:56.921778 django-magnet-data-1.1.4/magnet_data/models.py
--rw-r--r--   0        0        0      202 2022-12-22 18:15:19.779890 django-magnet-data-1.1.4/magnet_data/utils.py
--rw-r--r--   0        0        0      862 2023-05-04 20:29:39.381757 django-magnet-data-1.1.4/pyproject.toml
--rw-r--r--   0        0        0      748 2023-05-04 20:29:52.470196 django-magnet-data-1.1.4/setup.py
--rw-r--r--   0        0        0      861 2023-05-04 20:29:52.470388 django-magnet-data-1.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-10-14 16:58:17.859198 django-magnet-data-1.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.5/magnet_data/__init__.py
+-rw-r--r--   0        0        0      242 2023-06-08 17:23:23.426632 django-magnet-data-1.1.5/magnet_data/apps.py
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.775890 django-magnet-data-1.1.5/magnet_data/currencies/__init__.py
+-rw-r--r--   0        0        0     1599 2022-12-22 18:15:19.775890 django-magnet-data-1.1.5/magnet_data/currencies/client.py
+-rw-r--r--   0        0        0     4702 2023-05-04 20:28:56.929778 django-magnet-data-1.1.5/magnet_data/currencies/currency_pair.py
+-rw-r--r--   0        0        0      291 2022-12-22 18:15:19.775890 django-magnet-data-1.1.5/magnet_data/currencies/enums.py
+-rw-r--r--   0        0        0      802 2022-12-22 18:15:19.775890 django-magnet-data-1.1.5/magnet_data/currencies/exceptions.py
+-rw-r--r--   0        0        0     1314 2023-06-08 17:22:03.058561 django-magnet-data-1.1.5/magnet_data/currencies/models.py
+-rw-r--r--   0        0        0       54 2022-12-22 18:15:19.775890 django-magnet-data-1.1.5/magnet_data/currencies/urls.py
+-rw-r--r--   0        0        0        0 2023-05-04 20:28:56.913778 django-magnet-data-1.1.5/magnet_data/holidays/__init__.py
+-rw-r--r--   0        0        0      216 2023-05-04 20:28:56.917778 django-magnet-data-1.1.5/magnet_data/holidays/admin.py
+-rw-r--r--   0        0        0    11689 2023-05-04 20:28:56.917778 django-magnet-data-1.1.5/magnet_data/holidays/enums.py
+-rw-r--r--   0        0        0     2162 2023-06-08 17:22:03.058561 django-magnet-data-1.1.5/magnet_data/holidays/models.py
+-rw-r--r--   0        0        0     3839 2023-05-04 20:28:56.917778 django-magnet-data-1.1.5/magnet_data/magnet_data_client.py
+-rw-r--r--   0        0        0     2249 2022-12-22 18:15:19.779890 django-magnet-data-1.1.5/magnet_data/migrations/0001_initial.py
+-rw-r--r--   0        0        0     6827 2023-05-04 20:28:56.917778 django-magnet-data-1.1.5/magnet_data/migrations/0002_holiday.py
+-rw-r--r--   0        0        0        0 2022-12-22 18:15:19.779890 django-magnet-data-1.1.5/magnet_data/migrations/__init__.py
+-rw-r--r--   0        0        0      118 2023-05-04 20:28:56.921778 django-magnet-data-1.1.5/magnet_data/models.py
+-rw-r--r--   0        0        0      202 2022-12-22 18:15:19.779890 django-magnet-data-1.1.5/magnet_data/utils.py
+-rw-r--r--   0        0        0      862 2023-06-08 17:24:16.170679 django-magnet-data-1.1.5/pyproject.toml
+-rw-r--r--   0        0        0      748 2023-06-08 17:24:37.398230 django-magnet-data-1.1.5/setup.py
+-rw-r--r--   0        0        0      861 2023-06-08 17:24:37.398482 django-magnet-data-1.1.5/PKG-INFO
```

### Comparing `django-magnet-data-1.1.4/LICENSE` & `django-magnet-data-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/currencies/client.py` & `django-magnet-data-1.1.5/magnet_data/currencies/client.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/currencies/currency_pair.py` & `django-magnet-data-1.1.5/magnet_data/currencies/currency_pair.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/currencies/exceptions.py` & `django-magnet-data-1.1.5/magnet_data/currencies/exceptions.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/currencies/models.py` & `django-magnet-data-1.1.5/magnet_data/currencies/models.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/holidays/enums.py` & `django-magnet-data-1.1.5/magnet_data/holidays/enums.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/holidays/models.py` & `django-magnet-data-1.1.5/magnet_data/holidays/models.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/magnet_data_client.py` & `django-magnet-data-1.1.5/magnet_data/magnet_data_client.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/migrations/0001_initial.py` & `django-magnet-data-1.1.5/magnet_data/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/magnet_data/migrations/0002_holiday.py` & `django-magnet-data-1.1.5/magnet_data/migrations/0002_holiday.py`

 * *Files identical despite different names*

### Comparing `django-magnet-data-1.1.4/pyproject.toml` & `django-magnet-data-1.1.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-magnet-data"
-version = "1.1.4"
+version = "1.1.5"
 description = "An API client for data.magnet.cl"
 authors = ["Ignacio Munizaga <muni@magnet.cl>"]
 license = "MIT"
 repository = "https://github.com/magnet-cl/django-magnet-data"
 homepage = "https://github.com/magnet-cl/django-magnet-data"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `django-magnet-data-1.1.4/setup.py` & `django-magnet-data-1.1.5/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['django>=2.2']
 
 setup_kwargs = {
     'name': 'django-magnet-data',
-    'version': '1.1.4',
+    'version': '1.1.5',
     'description': 'An API client for data.magnet.cl',
     'long_description': None,
     'author': 'Ignacio Munizaga',
     'author_email': 'muni@magnet.cl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/magnet-cl/django-magnet-data',
```

### Comparing `django-magnet-data-1.1.4/PKG-INFO` & `django-magnet-data-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-magnet-data
-Version: 1.1.4
+Version: 1.1.5
 Summary: An API client for data.magnet.cl
 Home-page: https://github.com/magnet-cl/django-magnet-data
 License: MIT
 Author: Ignacio Munizaga
 Author-email: muni@magnet.cl
 Requires-Python: >=3.6.2,<4.0.0
 Classifier: Framework :: Django
```

