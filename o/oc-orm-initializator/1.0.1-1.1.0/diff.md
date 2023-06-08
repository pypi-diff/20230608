# Comparing `tmp/oc_orm_initializator-1.0.1-py3-none-any.whl.zip` & `tmp/oc_orm_initializator-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 6743 bytes, number of entries: 7
--rw-r--r--  2.0 unx        0 b- defN 23-May-22 07:59 oc_orm_initializator/__init__.py
--rw-r--r--  2.0 unx     2890 b- defN 23-May-22 07:59 oc_orm_initializator/orm_initializator.py
--rw-r--r--  2.0 unx    11357 b- defN 23-May-22 07:59 oc_orm_initializator-1.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx      285 b- defN 23-May-22 07:59 oc_orm_initializator-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-22 07:59 oc_orm_initializator-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       21 b- defN 23-May-22 07:59 oc_orm_initializator-1.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      635 b- defN 23-May-22 07:59 oc_orm_initializator-1.0.1.dist-info/RECORD
-7 files, 15280 bytes uncompressed, 5595 bytes compressed:  63.4%
+Zip file size: 6854 bytes, number of entries: 7
+-rw-r--r--  2.0 unx        0 b- defN 23-Jun-08 05:41 oc_orm_initializator/__init__.py
+-rw-r--r--  2.0 unx     3189 b- defN 23-Jun-08 05:41 oc_orm_initializator/orm_initializator.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-08 05:41 oc_orm_initializator-1.1.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      285 b- defN 23-Jun-08 05:41 oc_orm_initializator-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-08 05:41 oc_orm_initializator-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       21 b- defN 23-Jun-08 05:41 oc_orm_initializator-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      635 b- defN 23-Jun-08 05:41 oc_orm_initializator-1.1.0.dist-info/RECORD
+7 files, 15579 bytes uncompressed, 5706 bytes compressed:  63.4%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: oc_orm_initializator/__init__.py
 Comment: 
 
 Filename: oc_orm_initializator/orm_initializator.py
 Comment: 
 
-Filename: oc_orm_initializator-1.0.1.dist-info/LICENSE
+Filename: oc_orm_initializator-1.1.0.dist-info/LICENSE
 Comment: 
 
-Filename: oc_orm_initializator-1.0.1.dist-info/METADATA
+Filename: oc_orm_initializator-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: oc_orm_initializator-1.0.1.dist-info/WHEEL
+Filename: oc_orm_initializator-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: oc_orm_initializator-1.0.1.dist-info/top_level.txt
+Filename: oc_orm_initializator-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: oc_orm_initializator-1.0.1.dist-info/RECORD
+Filename: oc_orm_initializator-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oc_orm_initializator/orm_initializator.py

```diff
@@ -1,33 +1,39 @@
 import re
 import urllib.parse as urlparse
 import django
 from django.conf import settings
 import posixpath
+from copy import deepcopy
 
 class OrmInitializator():
     """
     A base class for DB connection via Django ORM
     """
     def __init__(self, url, user, password, installed_apps=list(), **additional_settings):
         """
         additional settings shoud include: url, user, password, installed_apps
         :param str url: URL for database connection
         :param str user: username for database authentication
         :param str password: password for database authentication
         :param list installed_apps: list of installed django applications
         :param additional_settings: Additional settings for DB connection
         """
-        settings.configure(
-            DATABASES=self._fill_db_dictionary(url=url, user=user, password=password),
-            USE_TZ=True,
-            TIME_ZONE='Etc/UTC',
-            INSTALLED_APPS=installed_apps + ['django.contrib.contenttypes', 'django.contrib.auth'],
-            **additional_settings
-        )
+        _all_settings = deepcopy(additional_settings)
+        _all_settings["DATABASES"] = self._fill_db_dictionary(url=url, user=user, password=password)
+
+        # avoid applications duplication
+        _all_settings["INSTALLED_APPS"] = list(set(installed_apps + 
+            ['django.contrib.contenttypes', 'django.contrib.auth']))
+
+        # we have to always use time zone in case we do not want to mix timestamps
+        _all_settings["USE_TZ"] = True
+        _all_settings["TIME_ZONE"] = additional_settings.get("TIME_ZONE") or "Etc/UTC"
+
+        settings.configure(**_all_settings)
 
         django.setup()
     
     def _fill_db_dictionary(self, url, user, password):
         """
         Returns django settings dictionary with PostgreSQL settings
         :param str url: URL for database connection
```

## Comparing `oc_orm_initializator-1.0.1.dist-info/LICENSE` & `oc_orm_initializator-1.1.0.dist-info/LICENSE`

 * *Files identical despite different names*

