# Comparing `tmp/django_pictures-1.1.0.tar.gz` & `tmp/django_pictures-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_pictures-1.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_pictures-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_pictures-1.1.0.tar` & `django_pictures-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0     1324 2023-05-24 17:01:29.714398 django_pictures-1.1.0/LICENSE
--rw-r--r--   0        0        0     9256 2023-05-24 17:01:29.714398 django_pictures-1.1.0/README.md
--rw-r--r--   0        0        0      171 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/__init__.py
--rw-r--r--   0        0        0      160 2023-05-24 17:01:49.962679 django_pictures-1.1.0/pictures/_version.py
--rw-r--r--   0        0        0      155 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/apps.py
--rw-r--r--   0        0        0     1012 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/checks.py
--rw-r--r--   0        0        0      683 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/conf.py
--rw-r--r--   0        0        0        0 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/contrib/__init__.py
--rw-r--r--   0        0        0     2343 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/contrib/rest_framework.py
--rw-r--r--   0        0        0      857 2023-05-24 17:01:42.970592 django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     1179 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3195 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/migrations.py
--rw-r--r--   0        0        0     8495 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/models.py
--rw-r--r--   0        0        0     3726 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/tasks.py
--rw-r--r--   0        0        0      165 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templates/pictures/attrs.html
--rw-r--r--   0        0        0      618 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templates/pictures/picture.html
--rw-r--r--   0        0        0        0 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templatetags/__init__.py
--rw-r--r--   0        0        0     2281 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/templatetags/pictures.py
--rw-r--r--   0        0        0      214 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/urls.py
--rw-r--r--   0        0        0     4023 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/utils.py
--rw-r--r--   0        0        0     1907 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/validators.py
--rw-r--r--   0        0        0      725 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pictures/views.py
--rw-r--r--   0        0        0     2349 2023-05-24 17:01:29.718399 django_pictures-1.1.0/pyproject.toml
--rw-r--r--   0        0        0    11381 1970-01-01 00:00:00.000000 django_pictures-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1324 2023-06-08 06:42:06.891338 django_pictures-1.1.1/LICENSE
+-rw-r--r--   0        0        0     9256 2023-06-08 06:42:06.891338 django_pictures-1.1.1/README.md
+-rw-r--r--   0        0        0      171 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/__init__.py
+-rw-r--r--   0        0        0      160 2023-06-08 06:42:52.298888 django_pictures-1.1.1/pictures/_version.py
+-rw-r--r--   0        0        0      155 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/apps.py
+-rw-r--r--   0        0        0     1012 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/checks.py
+-rw-r--r--   0        0        0      683 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/conf.py
+-rw-r--r--   0        0        0        0 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/contrib/__init__.py
+-rw-r--r--   0        0        0     2387 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/contrib/rest_framework.py
+-rw-r--r--   0        0        0      857 2023-06-08 06:42:43.710974 django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     1179 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3195 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/migrations.py
+-rw-r--r--   0        0        0     8495 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/models.py
+-rw-r--r--   0        0        0     3726 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/tasks.py
+-rw-r--r--   0        0        0      165 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templates/pictures/attrs.html
+-rw-r--r--   0        0        0      618 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templates/pictures/picture.html
+-rw-r--r--   0        0        0        0 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templatetags/__init__.py
+-rw-r--r--   0        0        0     2281 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/templatetags/pictures.py
+-rw-r--r--   0        0        0      214 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/urls.py
+-rw-r--r--   0        0        0     4023 2023-06-08 06:42:06.891338 django_pictures-1.1.1/pictures/utils.py
+-rw-r--r--   0        0        0     1907 2023-06-08 06:42:06.895338 django_pictures-1.1.1/pictures/validators.py
+-rw-r--r--   0        0        0      725 2023-06-08 06:42:06.895338 django_pictures-1.1.1/pictures/views.py
+-rw-r--r--   0        0        0     2349 2023-06-08 06:42:06.895338 django_pictures-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0    11381 1970-01-01 00:00:00.000000 django_pictures-1.1.1/PKG-INFO
```

### Comparing `django_pictures-1.1.0/LICENSE` & `django_pictures-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/README.md` & `django_pictures-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/checks.py` & `django_pictures-1.1.1/pictures/checks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/conf.py` & `django_pictures-1.1.1/pictures/conf.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/contrib/rest_framework.py` & `django_pictures-1.1.1/pictures/contrib/rest_framework.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,14 +16,16 @@
     raise TypeError(f"Type '{type(obj).__name__}' not serializable")
 
 
 class PictureField(serializers.ReadOnlyField):
     """Read-only field for all aspect ratios and sizes of the image."""
 
     def to_representation(self, obj: PictureFieldFile):
+        if not obj:
+            return None
         payload = {
             "url": obj.url,
             "width": obj.width,
             "height": obj.height,
             "ratios": {
                 ratio: {
                     "sources": {
```

### Comparing `django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.mo` & `django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/locale/de/LC_MESSAGES/django.po` & `django_pictures-1.1.1/pictures/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/migrations.py` & `django_pictures-1.1.1/pictures/migrations.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/models.py` & `django_pictures-1.1.1/pictures/models.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/tasks.py` & `django_pictures-1.1.1/pictures/tasks.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/templates/pictures/picture.html` & `django_pictures-1.1.1/pictures/templates/pictures/picture.html`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/templatetags/pictures.py` & `django_pictures-1.1.1/pictures/templatetags/pictures.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/utils.py` & `django_pictures-1.1.1/pictures/utils.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/validators.py` & `django_pictures-1.1.1/pictures/validators.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pictures/views.py` & `django_pictures-1.1.1/pictures/views.py`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/pyproject.toml` & `django_pictures-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django_pictures-1.1.0/PKG-INFO` & `django_pictures-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-pictures
-Version: 1.1.0
+Version: 1.1.1
 Summary: Responsive cross-browser image library using modern codes like AVIF & WebP.
 Keywords: pillow,Django,image,pictures,WebP,AVIF
 Author-email: Johannes Maron <johannes@maron.family>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
```

