# Comparing `tmp/copyleaks-4.0.0.tar.gz` & `tmp/copyleaks-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "copyleaks-4.0.0.tar", last modified: Tue Jun  6 11:00:53 2023, max compression
+gzip compressed data, was "copyleaks-4.0.1.tar", last modified: Thu Jun  8 12:21:43 2023, max compression
```

## Comparing `copyleaks-4.0.0.tar` & `copyleaks-4.0.1.tar`

### file list

```diff
@@ -1,56 +1,55 @@
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.520353 copyleaks-4.0.0/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1143 2023-06-06 10:39:45.000000 copyleaks-4.0.0/LICENSE.txt
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2825 2023-06-06 11:00:53.520353 copyleaks-4.0.0/PKG-INFO
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2294 2023-06-06 10:39:45.000000 copyleaks-4.0.0/README.md
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.412894 copyleaks-4.0.0/copyleaks/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/__init__.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1314 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/consts.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)    19734 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/copyleaks.py
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.432978 copyleaks-4.0.0/copyleaks/exceptions/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/__init__.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1229 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/auth_expired_error.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1374 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/command_error.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1227 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/rate_limit_error.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1234 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/exceptions/under_maintenance_error.py
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.440957 copyleaks-4.0.0/copyleaks/models/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/__init__.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3429 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/delete.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     6644 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/export.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2673 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/start.py
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.447938 copyleaks-4.0.0/copyleaks/models/submit/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/__init__.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2247 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/document.py
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.517360 copyleaks-4.0.0/copyleaks/models/submit/properties/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/__init__.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1559 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/ai_generated_text.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1915 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/author.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2272 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/copyleaksDb.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1820 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/cross_languages.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1457 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/custom_metadata.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1245 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/domains_mode.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     4496 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/exclude.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1518 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/exclude_code.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     4868 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/filters.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1612 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/indexing.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)      378 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/language.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1280 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/masking_policy.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3458 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/pdf.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1234 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/pdf_version.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3035 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/report_customization_colors.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3154 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/repository.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1268 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scan_method.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1255 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scan_priority.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     9398 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scan_properties.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3965 2023-06-06 10:48:23.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scanning.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1821 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/scanning_exclude.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1263 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/submit_action.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2011 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/properties/submit_webhooks.py
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2731 2023-06-06 10:39:45.000000 copyleaks-4.0.0/copyleaks/models/submit/scanning_copyleaks_db.py
-drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 11:00:53.422360 copyleaks-4.0.0/copyleaks.egg-info/
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2825 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/PKG-INFO
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1920 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/SOURCES.txt
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        1 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/dependency_links.txt
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       30 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/requires.txt
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       10 2023-06-06 11:00:53.000000 copyleaks-4.0.0/copyleaks.egg-info/top_level.txt
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       79 2023-06-06 11:00:53.521350 copyleaks-4.0.0/setup.cfg
--rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1021 2023-06-06 10:56:55.000000 copyleaks-4.0.0/setup.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.418983 copyleaks-4.0.1/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1143 2023-06-06 10:39:45.000000 copyleaks-4.0.1/LICENSE.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2825 2023-06-08 12:21:43.418983 copyleaks-4.0.1/PKG-INFO
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2294 2023-06-06 10:39:45.000000 copyleaks-4.0.1/README.md
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.317257 copyleaks-4.0.1/copyleaks/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1314 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/consts.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)    19734 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/copyleaks.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.336204 copyleaks-4.0.1/copyleaks/exceptions/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/exceptions/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1229 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/exceptions/auth_expired_error.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1374 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/exceptions/command_error.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1227 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/exceptions/rate_limit_error.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1234 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/exceptions/under_maintenance_error.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.344183 copyleaks-4.0.1/copyleaks/models/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3429 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/delete.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     6644 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/export.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2673 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/start.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.352161 copyleaks-4.0.1/copyleaks/models/submit/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2247 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/document.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.416988 copyleaks-4.0.1/copyleaks/models/submit/properties/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/__init__.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1559 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/ai_generated_text.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1915 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/author.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2272 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/copyleaksDb.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1820 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/cross_languages.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1457 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/custom_metadata.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1245 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/domains_mode.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     4496 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/exclude.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1518 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/exclude_code.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     4868 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/filters.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1612 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/indexing.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)      378 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/language.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1280 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/masking_policy.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3458 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/pdf.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1234 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/pdf_version.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3035 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/report_customization_colors.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3154 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/repository.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1268 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/scan_method.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     9050 2023-06-08 06:50:33.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/scan_properties.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     3965 2023-06-06 10:48:23.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/scanning.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1821 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/scanning_exclude.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1263 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/submit_action.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2011 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/properties/submit_webhooks.py
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2731 2023-06-06 10:39:45.000000 copyleaks-4.0.1/copyleaks/models/submit/scanning_copyleaks_db.py
+drwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        0 2023-06-08 12:21:43.327229 copyleaks-4.0.1/copyleaks.egg-info/
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     2825 2023-06-08 12:21:43.000000 copyleaks-4.0.1/copyleaks.egg-info/PKG-INFO
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1868 2023-06-08 12:21:43.000000 copyleaks-4.0.1/copyleaks.egg-info/SOURCES.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)        1 2023-06-08 12:21:43.000000 copyleaks-4.0.1/copyleaks.egg-info/dependency_links.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       30 2023-06-08 12:21:43.000000 copyleaks-4.0.1/copyleaks.egg-info/requires.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       10 2023-06-08 12:21:43.000000 copyleaks-4.0.1/copyleaks.egg-info/top_level.txt
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)       79 2023-06-08 12:21:43.420978 copyleaks-4.0.1/setup.cfg
+-rwxrwxrwx   0 aihamar   (1000) aihamar   (1000)     1021 2023-06-08 12:20:42.000000 copyleaks-4.0.1/setup.py
```

### Comparing `copyleaks-4.0.0/LICENSE.txt` & `copyleaks-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/PKG-INFO` & `copyleaks-4.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyleaks
-Version: 4.0.0
+Version: 4.0.1
 Summary: Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.
 Home-page: https://api.copyleaks.com
 Download-URL: https://github.com/Copyleaks/Python-Plagiarism-Checker
 Author: Copyleaks ltd
 Author-email: sales@copyleaks.com
 Keywords: copyleaks,api,plagiarism,content,checker,online,academic,publishers,websites
 Description-Content-Type: text/markdown
```

### Comparing `copyleaks-4.0.0/README.md` & `copyleaks-4.0.1/README.md`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/consts.py` & `copyleaks-4.0.1/copyleaks/consts.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/copyleaks.py` & `copyleaks-4.0.1/copyleaks/copyleaks.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/exceptions/auth_expired_error.py` & `copyleaks-4.0.1/copyleaks/exceptions/auth_expired_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/exceptions/command_error.py` & `copyleaks-4.0.1/copyleaks/exceptions/command_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/exceptions/rate_limit_error.py` & `copyleaks-4.0.1/copyleaks/exceptions/rate_limit_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/exceptions/under_maintenance_error.py` & `copyleaks-4.0.1/copyleaks/exceptions/under_maintenance_error.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/delete.py` & `copyleaks-4.0.1/copyleaks/models/delete.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/export.py` & `copyleaks-4.0.1/copyleaks/models/export.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/start.py` & `copyleaks-4.0.1/copyleaks/models/start.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/document.py` & `copyleaks-4.0.1/copyleaks/models/submit/document.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/ai_generated_text.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/ai_generated_text.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/author.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/author.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/copyleaksDb.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/copyleaksDb.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/cross_languages.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/cross_languages.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/custom_metadata.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/custom_metadata.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/domains_mode.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/domains_mode.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/exclude.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/exclude.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/exclude_code.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/exclude_code.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/filters.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/filters.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/indexing.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/indexing.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/masking_policy.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/masking_policy.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/pdf.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/pdf.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/pdf_version.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/pdf_version.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/report_customization_colors.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/report_customization_colors.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/repository.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/repository.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/scan_method.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/scan_method.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/scan_priority.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/submit_action.py`

 * *Files 9% similar despite different names*

```diff
@@ -21,11 +21,11 @@
  OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
  SOFTWARE.
 '''
 
 from enum import IntEnum
 
 
-class ScanPriority(IntEnum):
-    Low = 1
-    Normal = 2
-    High = 3
+class SubmitAction(IntEnum):
+    Scan = 0
+    CheckCredits = 1
+    Index = 2
```

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/scan_properties.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/scan_properties.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,31 +85,14 @@
             Setting the developer payload parameter. This string must be no longer then 512 characters.
         '''
 
         assert value and len(value) <= 512
 
         self.developerPayload = value
 
-    def get_priority(self):
-        '''
-            Getting the scan priority.
-        '''
-        return self.priority
-
-    def set_priority(self, value):
-        '''
-            Set scan priority.
-
-            Parameters:
-                value: ScanPriority enum.
-        '''
-
-        assert value
-
-        self.priority = value
 
     def get_sandbox(self):
         '''
             Get the sandbox mode status.
         '''
         return self.sandbox
```

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/scanning.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/scanning.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/scanning_exclude.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/scanning_exclude.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/properties/submit_webhooks.py` & `copyleaks-4.0.1/copyleaks/models/submit/properties/submit_webhooks.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks/models/submit/scanning_copyleaks_db.py` & `copyleaks-4.0.1/copyleaks/models/submit/scanning_copyleaks_db.py`

 * *Files identical despite different names*

### Comparing `copyleaks-4.0.0/copyleaks.egg-info/PKG-INFO` & `copyleaks-4.0.1/copyleaks.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: copyleaks
-Version: 4.0.0
+Version: 4.0.1
 Summary: Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.
 Home-page: https://api.copyleaks.com
 Download-URL: https://github.com/Copyleaks/Python-Plagiarism-Checker
 Author: Copyleaks ltd
 Author-email: sales@copyleaks.com
 Keywords: copyleaks,api,plagiarism,content,checker,online,academic,publishers,websites
 Description-Content-Type: text/markdown
```

### Comparing `copyleaks-4.0.0/copyleaks.egg-info/SOURCES.txt` & `copyleaks-4.0.1/copyleaks.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -36,13 +36,12 @@
 copyleaks/models/submit/properties/language.py
 copyleaks/models/submit/properties/masking_policy.py
 copyleaks/models/submit/properties/pdf.py
 copyleaks/models/submit/properties/pdf_version.py
 copyleaks/models/submit/properties/report_customization_colors.py
 copyleaks/models/submit/properties/repository.py
 copyleaks/models/submit/properties/scan_method.py
-copyleaks/models/submit/properties/scan_priority.py
 copyleaks/models/submit/properties/scan_properties.py
 copyleaks/models/submit/properties/scanning.py
 copyleaks/models/submit/properties/scanning_exclude.py
 copyleaks/models/submit/properties/submit_action.py
 copyleaks/models/submit/properties/submit_webhooks.py
```

### Comparing `copyleaks-4.0.0/setup.py` & `copyleaks-4.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='copyleaks',
     packages=['copyleaks', 'copyleaks.exceptions', 'copyleaks.models', 'copyleaks.models.submit', 'copyleaks.models.submit.properties'],
-    version='4.0.0',
+    version='4.0.1',
     description='Copyleaks API gives you access to a variety of plagiarism detection technologies to protect your online content. Get the most comprehensive plagiarism report for your content that is easy to use and integrate.',
     author='Copyleaks ltd',
     author_email='sales@copyleaks.com',
     url='https://api.copyleaks.com',
     download_url='https://github.com/Copyleaks/Python-Plagiarism-Checker',
     keywords=['copyleaks', 'api', 'plagiarism', 'content', 'checker', 'online', 'academic', 'publishers', 'websites'],
     install_requires=[
```

