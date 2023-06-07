# Comparing `tmp/smartapp_sdk-0.6.1.tar.gz` & `tmp/smartapp_sdk-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smartapp_sdk-0.6.1.tar", max compression
+gzip compressed data, was "smartapp_sdk-0.6.2.tar", max compression
```

## Comparing `smartapp_sdk-0.6.1.tar` & `smartapp_sdk-0.6.2.tar`

### file list

```diff
@@ -1,67 +1,66 @@
--rw-r--r--   0        0        0     1877 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/Changelog
--rw-r--r--   0        0        0    11324 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/LICENSE
--rw-r--r--   0        0        0      761 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/NOTICE
--rw-r--r--   0        0        0     2167 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/PyPI.md
--rw-r--r--   0        0        0     2366 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/README.md
--rw-r--r--   0        0        0       22 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/.gitignore
--rw-r--r--   0        0        0      142 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/.sphinxignore
--rw-r--r--   0        0        0     6814 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/Makefile
--rw-r--r--   0        0        0      120 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/README.md
--rw-r--r--   0        0        0      130 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/_static/custom.css
--rw-r--r--   0        0        0     1861 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/_themes/LICENSE
--rw-r--r--   0        0        0     3905 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/_themes/flask_theme_support.py
--rw-r--r--   0        0        0    13018 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/conf.py
--rw-r--r--   0        0        0     9479 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/index.rst
--rw-r--r--   0        0        0     6709 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/docs/make.bat
--rw-r--r--   0        0        0     2781 2023-06-07 01:05:08.287151 smartapp_sdk-0.6.1/pyproject.toml
--rw-r--r--   0        0        0       29 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/__init__.py
--rw-r--r--   0        0        0     6872 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/converter.py
--rw-r--r--   0        0        0     7781 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/dispatcher.py
--rw-r--r--   0        0        0    35006 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/interface.py
--rw-r--r--   0        0        0       60 2023-06-07 01:04:49.395155 smartapp_sdk-0.6.1/src/smartapp/py.typed
--rw-r--r--   0        0        0     9939 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/src/smartapp/signature.py
--rw-r--r--   0        0        0       29 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/__init__.py
--rw-r--r--   0        0        0      213 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/live/README.md
--rw-r--r--   0        0        0     2885 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/live/request/INSTALL.1.json
--rw-r--r--   0        0        0     1011 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/README.md
--rw-r--r--   0        0        0      813 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json
--rw-r--r--   0        0        0      457 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIGURATION-PAGE.json
--rw-r--r--   0        0        0      381 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIRMATION.json
--rw-r--r--   0        0        0     1793 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-DEVICE.json
--rw-r--r--   0        0        0     1567 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-TIMER.json
--rw-r--r--   0        0        0     1327 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/INSTALL.json
--rw-r--r--   0        0        0      218 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/OAUTH_CALLBACK.json
--rw-r--r--   0        0        0     1255 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/UNINSTALL.json
--rw-r--r--   0        0        0     2152 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/request/UPDATE.json
--rw-r--r--   0        0        0      249 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-INITIALIZE.json
--rw-r--r--   0        0        0      742 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json
--rw-r--r--   0        0        0     1251 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json
--rw-r--r--   0        0        0       33 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIRMATION.json
--rw-r--r--   0        0        0       21 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/EVENT.json
--rw-r--r--   0        0        0       23 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/INSTALL.json
--rw-r--r--   0        0        0       29 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/OAUTH_CALLBACK.json
--rw-r--r--   0        0        0       25 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/UNINSTALL.json
--rw-r--r--   0        0        0       22 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/response/UPDATE.json
--rw-r--r--   0        0        0      156 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/BOOLEAN.json
--rw-r--r--   0        0        0      117 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/DECIMAL.json
--rw-r--r--   0        0        0      231 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/DEVICE.json
--rw-r--r--   0        0        0      114 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/EMAIL.json
--rw-r--r--   0        0        0      700 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ENUM-GROUP.json
--rw-r--r--   0        0        0      292 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ENUM.json
--rw-r--r--   0        0        0      152 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ICON.json
--rw-r--r--   0        0        0      146 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/IMAGE.json
--rw-r--r--   0        0        0      187 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/LINK.json
--rw-r--r--   0        0        0      108 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/NUMBER.json
--rw-r--r--   0        0        0      291 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/OAUTH.json
--rw-r--r--   0        0        0      167 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/PAGE.json
--rw-r--r--   0        0        0      185 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/PARAGRAPH.json
--rw-r--r--   0        0        0      112 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/PHONE.json
--rw-r--r--   0        0        0      165 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/TEXT.json
--rw-r--r--   0        0        0      101 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/fixtures/samples/settings/TIME.json
--rw-r--r--   0        0        0    38670 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_converter.py
--rw-r--r--   0        0        0    14130 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_dispatcher.py
--rw-r--r--   0        0        0     7893 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_interface.py
--rw-r--r--   0        0        0    25529 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/test_signature.py
--rw-r--r--   0        0        0      549 2023-06-07 01:04:49.399155 smartapp_sdk-0.6.1/tests/testutil.py
--rw-r--r--   0        0        0     3272 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.1/setup.py
--rw-r--r--   0        0        0     3660 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0     1963 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/Changelog
+-rw-r--r--   0        0        0    11324 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/LICENSE
+-rw-r--r--   0        0        0      761 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/NOTICE
+-rw-r--r--   0        0        0     2167 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/PyPI.md
+-rw-r--r--   0        0        0     2366 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/README.md
+-rw-r--r--   0        0        0       22 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/.gitignore
+-rw-r--r--   0        0        0      142 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/.sphinxignore
+-rw-r--r--   0        0        0     6814 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/Makefile
+-rw-r--r--   0        0        0      120 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/README.md
+-rw-r--r--   0        0        0      130 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/_static/custom.css
+-rw-r--r--   0        0        0     1861 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/_themes/LICENSE
+-rw-r--r--   0        0        0     3905 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/_themes/flask_theme_support.py
+-rw-r--r--   0        0        0    13018 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/conf.py
+-rw-r--r--   0        0        0     9479 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/index.rst
+-rw-r--r--   0        0        0     6709 2023-06-07 23:12:25.843753 smartapp_sdk-0.6.2/docs/make.bat
+-rw-r--r--   0        0        0     2786 2023-06-07 23:13:09.620383 smartapp_sdk-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0       29 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/src/smartapp/__init__.py
+-rw-r--r--   0        0        0     6872 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/src/smartapp/converter.py
+-rw-r--r--   0        0        0     7781 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/src/smartapp/dispatcher.py
+-rw-r--r--   0        0        0    35006 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/src/smartapp/interface.py
+-rw-r--r--   0        0        0       60 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/src/smartapp/py.typed
+-rw-r--r--   0        0        0     9939 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/src/smartapp/signature.py
+-rw-r--r--   0        0        0       29 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/__init__.py
+-rw-r--r--   0        0        0      213 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/live/README.md
+-rw-r--r--   0        0        0     2885 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/live/request/INSTALL.1.json
+-rw-r--r--   0        0        0     1011 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/README.md
+-rw-r--r--   0        0        0      813 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json
+-rw-r--r--   0        0        0      457 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/CONFIGURATION-PAGE.json
+-rw-r--r--   0        0        0      381 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/CONFIRMATION.json
+-rw-r--r--   0        0        0     1793 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/EVENT-DEVICE.json
+-rw-r--r--   0        0        0     1567 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/EVENT-TIMER.json
+-rw-r--r--   0        0        0     1327 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/INSTALL.json
+-rw-r--r--   0        0        0      218 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/OAUTH_CALLBACK.json
+-rw-r--r--   0        0        0     1255 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/UNINSTALL.json
+-rw-r--r--   0        0        0     2152 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/request/UPDATE.json
+-rw-r--r--   0        0        0      249 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/CONFIGURATION-INITIALIZE.json
+-rw-r--r--   0        0        0      742 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json
+-rw-r--r--   0        0        0     1251 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json
+-rw-r--r--   0        0        0       33 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/CONFIRMATION.json
+-rw-r--r--   0        0        0       21 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/EVENT.json
+-rw-r--r--   0        0        0       23 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/INSTALL.json
+-rw-r--r--   0        0        0       29 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/OAUTH_CALLBACK.json
+-rw-r--r--   0        0        0       25 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/UNINSTALL.json
+-rw-r--r--   0        0        0       22 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/response/UPDATE.json
+-rw-r--r--   0        0        0      156 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/BOOLEAN.json
+-rw-r--r--   0        0        0      117 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/DECIMAL.json
+-rw-r--r--   0        0        0      231 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/DEVICE.json
+-rw-r--r--   0        0        0      114 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/EMAIL.json
+-rw-r--r--   0        0        0      700 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/ENUM-GROUP.json
+-rw-r--r--   0        0        0      292 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/ENUM.json
+-rw-r--r--   0        0        0      152 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/ICON.json
+-rw-r--r--   0        0        0      146 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/IMAGE.json
+-rw-r--r--   0        0        0      187 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/LINK.json
+-rw-r--r--   0        0        0      108 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/NUMBER.json
+-rw-r--r--   0        0        0      291 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/OAUTH.json
+-rw-r--r--   0        0        0      167 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/PAGE.json
+-rw-r--r--   0        0        0      185 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/PARAGRAPH.json
+-rw-r--r--   0        0        0      112 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/PHONE.json
+-rw-r--r--   0        0        0      165 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/TEXT.json
+-rw-r--r--   0        0        0      101 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/fixtures/samples/settings/TIME.json
+-rw-r--r--   0        0        0    38670 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/test_converter.py
+-rw-r--r--   0        0        0    14130 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/test_dispatcher.py
+-rw-r--r--   0        0        0     7893 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/test_interface.py
+-rw-r--r--   0        0        0    25529 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/test_signature.py
+-rw-r--r--   0        0        0      549 2023-06-07 23:12:25.847754 smartapp_sdk-0.6.2/tests/testutil.py
+-rw-r--r--   0        0        0     3612 1970-01-01 00:00:00.000000 smartapp_sdk-0.6.2/PKG-INFO
```

### Comparing `smartapp_sdk-0.6.1/Changelog` & `smartapp_sdk-0.6.2/Changelog`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+Version 0.6.2     07 Jun 2023
+
+	* Upgrade to Poetry v1.5.1 and make related changes.
+
 Version 0.6.1     06 Jun 2023
 
 	* Fix checktabs to be safe for file named '-'.
 	* Update requests dependency for CVE-2023-32681.
 
 Version 0.6.0     09 Apr 2023
```

### Comparing `smartapp_sdk-0.6.1/LICENSE` & `smartapp_sdk-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/NOTICE` & `smartapp_sdk-0.6.2/NOTICE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/PyPI.md` & `smartapp_sdk-0.6.2/PyPI.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/README.md` & `smartapp_sdk-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/docs/Makefile` & `smartapp_sdk-0.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/docs/_themes/LICENSE` & `smartapp_sdk-0.6.2/docs/_themes/LICENSE`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/docs/_themes/flask_theme_support.py` & `smartapp_sdk-0.6.2/docs/_themes/flask_theme_support.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/docs/conf.py` & `smartapp_sdk-0.6.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/docs/index.rst` & `smartapp_sdk-0.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/docs/make.bat` & `smartapp_sdk-0.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/pyproject.toml` & `smartapp_sdk-0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smartapp-sdk"
-version = "0.6.1" # published version is managed using Git tags (see below)
+version = "0.6.2" # published version is managed using Git tags (see below)
 description = "Framework to build a webhook-based SmartThings SmartApp"
 authors = ["Kenneth J. Pronovici <pronovic@ieee.org>"]
 license = "Apache-2.0"
 readme = "PyPI.md"
 homepage = "https://pypi.org/project/smartapp-sdk/"
 repository = "https://github.com/pronovic/smartapp-sdk"
 include = [
@@ -89,9 +89,9 @@
 
 [tool.isort]
 profile = "black"
 line_length = 132
 skip_glob = [ "docs", "notes" ]
 
 [build-system]
-requires = ["poetry>=1.0.0", "poetry-dynamic-versioning"]
+requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
```

### Comparing `smartapp_sdk-0.6.1/src/smartapp/converter.py` & `smartapp_sdk-0.6.2/src/smartapp/converter.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/src/smartapp/dispatcher.py` & `smartapp_sdk-0.6.2/src/smartapp/dispatcher.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/src/smartapp/interface.py` & `smartapp_sdk-0.6.2/src/smartapp/interface.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/src/smartapp/signature.py` & `smartapp_sdk-0.6.2/src/smartapp/signature.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/live/request/INSTALL.1.json` & `smartapp_sdk-0.6.2/tests/fixtures/live/request/INSTALL.1.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/README.md` & `smartapp_sdk-0.6.2/tests/fixtures/samples/README.md`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/request/CONFIGURATION-INITIALIZE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-DEVICE.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/request/EVENT-DEVICE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/request/EVENT-TIMER.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/request/EVENT-TIMER.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/request/INSTALL.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/request/INSTALL.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/request/UNINSTALL.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/request/UNINSTALL.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/request/UPDATE.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/request/UPDATE.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/response/CONFIGURATION-PAGE-1of2.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/response/CONFIGURATION-PAGE-only.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/fixtures/samples/settings/ENUM-GROUP.json` & `smartapp_sdk-0.6.2/tests/fixtures/samples/settings/ENUM-GROUP.json`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/test_converter.py` & `smartapp_sdk-0.6.2/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/test_dispatcher.py` & `smartapp_sdk-0.6.2/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/test_interface.py` & `smartapp_sdk-0.6.2/tests/test_interface.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/test_signature.py` & `smartapp_sdk-0.6.2/tests/test_signature.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/tests/testutil.py` & `smartapp_sdk-0.6.2/tests/testutil.py`

 * *Files identical despite different names*

### Comparing `smartapp_sdk-0.6.1/PKG-INFO` & `smartapp_sdk-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smartapp-sdk
-Version: 0.6.1
+Version: 0.6.2
 Summary: Framework to build a webhook-based SmartThings SmartApp
 Home-page: https://pypi.org/project/smartapp-sdk/
 License: Apache-2.0
 Author: Kenneth J. Pronovici
 Author-email: pronovic@ieee.org
 Requires-Python: >=3.9,<4
 Classifier: Development Status :: 4 - Beta
@@ -13,15 +13,14 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: docs
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: attrs (>=22.2.0,<23.0.0)
 Requires-Dist: cattrs (>=22.2.0,<23.0.0)
 Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0) ; extra == "docs"
```

