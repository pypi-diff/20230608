# Comparing `tmp/django_rest_tsg-0.1.7-py3-none-any.whl.zip` & `tmp/django_rest_tsg-0.1.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 14232 bytes, number of entries: 16
--rw-r--r--  2.0 unx      817 b- defN 80-Jan-01 00:00 CHANGELOG.rst
+Zip file size: 14242 bytes, number of entries: 16
+-rw-r--r--  2.0 unx      868 b- defN 80-Jan-01 00:00 CHANGELOG.rst
 -rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 LICENSE
 -rw-r--r--  2.0 unx     3511 b- defN 80-Jan-01 00:00 README.rst
 -rw-r--r--  2.0 unx      197 b- defN 80-Jan-01 00:00 django_rest_tsg/__init__.py
 -rw-r--r--  2.0 unx      193 b- defN 80-Jan-01 00:00 django_rest_tsg/apps.py
 -rw-r--r--  2.0 unx     7304 b- defN 80-Jan-01 00:00 django_rest_tsg/build.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_rest_tsg/management/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_rest_tsg/management/commands/__init__.py
 -rw-r--r--  2.0 unx     1196 b- defN 80-Jan-01 00:00 django_rest_tsg/management/commands/buildtypescript.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 django_rest_tsg/py.typed
 -rw-r--r--  2.0 unx      595 b- defN 80-Jan-01 00:00 django_rest_tsg/templates.py
 -rw-r--r--  2.0 unx    14154 b- defN 80-Jan-01 00:00 django_rest_tsg/typescript.py
--rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 django_rest_tsg-0.1.7.dist-info/LICENSE
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 django_rest_tsg-0.1.7.dist-info/WHEEL
-?rw-r--r--  2.0 unx     4987 b- defN 16-Jan-01 00:00 django_rest_tsg-0.1.7.dist-info/METADATA
-?rw-r--r--  2.0 unx     1322 b- defN 16-Jan-01 00:00 django_rest_tsg-0.1.7.dist-info/RECORD
-16 files, 36495 bytes uncompressed, 12038 bytes compressed:  67.0%
+-rw-r--r--  2.0 unx     1068 b- defN 80-Jan-01 00:00 django_rest_tsg-0.1.8.dist-info/LICENSE
+?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 django_rest_tsg-0.1.8.dist-info/WHEEL
+?rw-r--r--  2.0 unx     5026 b- defN 16-Jan-01 00:00 django_rest_tsg-0.1.8.dist-info/METADATA
+?rw-r--r--  2.0 unx     1322 b- defN 16-Jan-01 00:00 django_rest_tsg-0.1.8.dist-info/RECORD
+16 files, 36585 bytes uncompressed, 12048 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: django_rest_tsg/templates.py
 Comment: 
 
 Filename: django_rest_tsg/typescript.py
 Comment: 
 
-Filename: django_rest_tsg-0.1.7.dist-info/LICENSE
+Filename: django_rest_tsg-0.1.8.dist-info/LICENSE
 Comment: 
 
-Filename: django_rest_tsg-0.1.7.dist-info/WHEEL
+Filename: django_rest_tsg-0.1.8.dist-info/WHEEL
 Comment: 
 
-Filename: django_rest_tsg-0.1.7.dist-info/METADATA
+Filename: django_rest_tsg-0.1.8.dist-info/METADATA
 Comment: 
 
-Filename: django_rest_tsg-0.1.7.dist-info/RECORD
+Filename: django_rest_tsg-0.1.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## CHANGELOG.rst

```diff
@@ -1,7 +1,11 @@
+0.1.8
+-------------
+* Bump django version to 4.2.
+
 0.1.7
 -------------
 * Bump django version to 4.1.
 * Bump djangorestframework version to 3.14.
 
 0.1.6
 -------------
```

## django_rest_tsg/__init__.py

```diff
@@ -1,7 +1,7 @@
 __title__ = "Django REST TypeScript Generator"
-__version__ = "0.1.7"
+__version__ = "0.1.8"
 __author__ = "Yinian Chin"
 __license__ = "MIT License"
 __copyright__ = "Copyright 2021-2023 Yinian Chin"
 
 VERSION = __version__
```

## Comparing `django_rest_tsg-0.1.7.dist-info/LICENSE` & `django_rest_tsg-0.1.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_rest_tsg-0.1.7.dist-info/METADATA` & `django_rest_tsg-0.1.8.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: django-rest-tsg
-Version: 0.1.7
+Version: 0.1.8
 Summary: A typescript code generator for Django Rest Framework.
 Home-page: https://github.com/jinkanhq/django-rest-tsg
 License: MIT
 Author: Yinian Chin
 Author-email: yinian@jinkan.org
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

## Comparing `django_rest_tsg-0.1.7.dist-info/RECORD` & `django_rest_tsg-0.1.8.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-CHANGELOG.rst,sha256=r5oRxXrjlwogGY6Btiv0E4GIUtkoch2BZlHvAk7IE9E,817
+CHANGELOG.rst,sha256=Q26gzsTvapUt178SfzoxB3N3jgEf3ujYl87iWiYjIPg,868
 LICENSE,sha256=DWulA8opUT_9vTrFWY5LpGQdOvyjh2lasnL8ltbw7Nk,1068
 README.rst,sha256=b26vSg-kx3jJq3PqlVCf2-YzdIwPO5we-cFuETs7UGw,3511
-django_rest_tsg/__init__.py,sha256=Z-29Ju-9l-WhAbKssJXJ1uQUjp6dMV6ii1BNEBxrQNM,197
+django_rest_tsg/__init__.py,sha256=iNG7xnjWBbndS67fxuo9XCLYwlOePE8XUCmkWeueb-I,197
 django_rest_tsg/apps.py,sha256=1BRkm-OMtz1qapO_6p1ywoxymyztBHQ7eJxO_wAuO1g,193
 django_rest_tsg/build.py,sha256=k8w-1s72jhTDBwGQ0wAXo3Psi-2mKtgdjF43QrORDsw,7304
 django_rest_tsg/management/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_rest_tsg/management/commands/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_rest_tsg/management/commands/buildtypescript.py,sha256=AtDcfFhSHgvAL0EQb3lZ2b9tA0iy5GTI_hVPXZ3PZF4,1196
 django_rest_tsg/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 django_rest_tsg/templates.py,sha256=wJO7VCPB9IFt3Tajf_iBI5sWakF3l1y9gNkLI5Qo0XE,595
 django_rest_tsg/typescript.py,sha256=2bYjV4wxPpu-s-xO_Qq6RdDxTevFNP5txveU9ml1Irw,14154
-django_rest_tsg-0.1.7.dist-info/LICENSE,sha256=DWulA8opUT_9vTrFWY5LpGQdOvyjh2lasnL8ltbw7Nk,1068
-django_rest_tsg-0.1.7.dist-info/WHEEL,sha256=y3eDiaFVSNTPbgzfNn0nYn5tEn1cX6WrdetDlQM4xWw,83
-django_rest_tsg-0.1.7.dist-info/METADATA,sha256=JHJsxEee7YPMZHF0qpRhrAiH-uIQNYuEBDRKhXbozCI,4987
-django_rest_tsg-0.1.7.dist-info/RECORD,,
+django_rest_tsg-0.1.8.dist-info/LICENSE,sha256=DWulA8opUT_9vTrFWY5LpGQdOvyjh2lasnL8ltbw7Nk,1068
+django_rest_tsg-0.1.8.dist-info/WHEEL,sha256=y3eDiaFVSNTPbgzfNn0nYn5tEn1cX6WrdetDlQM4xWw,83
+django_rest_tsg-0.1.8.dist-info/METADATA,sha256=C7fGM-9RCV2T_URMsDxwZTlpN7r5_zNHzYdpWBPCnHc,5026
+django_rest_tsg-0.1.8.dist-info/RECORD,,
```

