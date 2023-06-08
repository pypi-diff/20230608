# Comparing `tmp/toolium-3.0.2.tar.gz` & `tmp/toolium-3.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toolium-3.0.2.tar", last modified: Thu Jun  8 10:41:15 2023, max compression
+gzip compressed data, was "toolium-3.0.2.dev0.tar", last modified: Fri May 19 09:08:23 2023, max compression
```

## Comparing `toolium-3.0.2.tar` & `toolium-3.0.2.dev0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:15.035309 toolium-3.0.2/
--rw-rw-rw-   0        0        0    30467 2023-06-08 10:40:12.000000 toolium-3.0.2/CHANGELOG.rst
--rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.2/LICENSE
--rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     5521 2023-06-08 10:41:15.035309 toolium-3.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.2/README.rst
--rw-rw-rw-   0        0        0        7 2023-06-08 10:40:12.000000 toolium-3.0.2/VERSION
--rw-rw-rw-   0        0        0      225 2023-05-29 15:01:04.000000 toolium-3.0.2/requirements.txt
--rw-rw-rw-   0        0        0      236 2023-05-19 07:42:34.000000 toolium-3.0.2/requirements_dev.txt
--rw-rw-rw-   0        0        0       70 2023-06-08 10:41:15.036312 toolium-3.0.2/setup.cfg
--rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:14.897264 toolium-3.0.2/toolium/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2/toolium/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:14.917134 toolium-3.0.2/toolium/behave/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2/toolium/behave/__init__.py
--rw-rw-rw-   0        0        0    12880 2023-05-19 07:42:34.000000 toolium-3.0.2/toolium/behave/env_utils.py
--rw-rw-rw-   0        0        0    11018 2023-05-17 13:54:12.000000 toolium-3.0.2/toolium/behave/environment.py
--rw-rw-rw-   0        0        0    21019 2023-05-08 11:36:54.000000 toolium-3.0.2/toolium/config_driver.py
--rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/config_files.py
--rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/config_parser.py
--rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/driver_wrapper.py
--rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/driver_wrappers_pool.py
--rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/jira.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:14.968259 toolium-3.0.2/toolium/pageelements/
--rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/__init__.py
--rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/button_page_element.py
--rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/checkbox_page_element.py
--rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/group_page_element.py
--rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/input_radio_page_element.py
--rw-rw-rw-   0        0        0     2731 2023-05-10 11:35:00.000000 toolium-3.0.2/toolium/pageelements/input_text_page_element.py
--rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/link_page_element.py
--rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/page_element.py
--rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/page_elements.py
--rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/select_page_element.py
--rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageelements/text_page_element.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:14.984990 toolium-3.0.2/toolium/pageobjects/
--rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2/toolium/pageobjects/__init__.py
--rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageobjects/common_object.py
--rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageobjects/mobile_page_object.py
--rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pageobjects/page_object.py
--rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/pytest_fixtures.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:14.998003 toolium-3.0.2/toolium/resources/
--rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.2/toolium/resources/VisualTests.css
--rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.2/toolium/resources/VisualTests.js
--rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.2/toolium/resources/VisualTestsTemplate.html
--rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/selenoid.py
--rw-rw-rw-   0        0        0     8733 2023-05-08 11:36:54.000000 toolium-3.0.2/toolium/test_cases.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:15.034309 toolium-3.0.2/toolium/utils/
--rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/__init__.py
--rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/data_generator.py
--rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.2/toolium/utils/dataset.py
--rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/download_files.py
--rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/driver_utils.py
--rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/driver_wait_utils.py
--rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/path_utils.py
--rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/utils/poeditor.py
--rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.2/toolium/visual_test.py
-drwxrwxrwx   0        0        0        0 2023-06-08 10:41:14.904264 toolium-3.0.2/toolium.egg-info/
--rw-rw-rw-   0        0        0     5521 2023-06-08 10:41:14.000000 toolium-3.0.2/toolium.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1564 2023-06-08 10:41:14.000000 toolium-3.0.2/toolium.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 10:41:14.000000 toolium-3.0.2/toolium.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      124 2023-06-08 10:41:14.000000 toolium-3.0.2/toolium.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-08 10:41:14.000000 toolium-3.0.2/toolium.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.986533 toolium-3.0.2.dev0/
+-rw-rw-rw-   0        0        0    30389 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/CHANGELOG.rst
+-rw-rw-rw-   0        0        0    11560 2016-08-02 09:48:30.000000 toolium-3.0.2.dev0/LICENSE
+-rw-rw-rw-   0        0        0      151 2021-03-20 20:19:53.000000 toolium-3.0.2.dev0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5526 2023-05-19 09:08:22.986533 toolium-3.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     4031 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/README.rst
+-rw-rw-rw-   0        0        0       12 2023-05-09 09:50:47.000000 toolium-3.0.2.dev0/VERSION
+-rw-rw-rw-   0        0        0      225 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/requirements.txt
+-rw-rw-rw-   0        0        0      236 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       70 2023-05-19 09:08:22.988535 toolium-3.0.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     3229 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.630532 toolium-3.0.2.dev0/toolium/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.669533 toolium-3.0.2.dev0/toolium/behave/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/behave/__init__.py
+-rw-rw-rw-   0        0        0    12880 2023-05-19 07:42:34.000000 toolium-3.0.2.dev0/toolium/behave/env_utils.py
+-rw-rw-rw-   0        0        0    11018 2023-05-17 13:54:12.000000 toolium-3.0.2.dev0/toolium/behave/environment.py
+-rw-rw-rw-   0        0        0    21019 2023-05-08 11:36:54.000000 toolium-3.0.2.dev0/toolium/config_driver.py
+-rw-rw-rw-   0        0        0     2461 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/config_files.py
+-rw-rw-rw-   0        0        0     8412 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/config_parser.py
+-rw-rw-rw-   0        0        0    16655 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/driver_wrapper.py
+-rw-rw-rw-   0        0        0    18000 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/driver_wrappers_pool.py
+-rw-rw-rw-   0        0        0     6669 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/jira.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.801534 toolium-3.0.2.dev0/toolium/pageelements/
+-rw-rw-rw-   0        0        0     1645 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/__init__.py
+-rw-rw-rw-   0        0        0     1485 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/button_page_element.py
+-rw-rw-rw-   0        0        0     1556 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/checkbox_page_element.py
+-rw-rw-rw-   0        0        0     4013 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/group_page_element.py
+-rw-rw-rw-   0        0        0     1290 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/input_radio_page_element.py
+-rw-rw-rw-   0        0        0     2731 2023-05-10 11:35:00.000000 toolium-3.0.2.dev0/toolium/pageelements/input_text_page_element.py
+-rw-rw-rw-   0        0        0      942 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/link_page_element.py
+-rw-rw-rw-   0        0        0    14652 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/page_element.py
+-rw-rw-rw-   0        0        0     6195 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/page_elements.py
+-rw-rw-rw-   0        0        0     1517 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/select_page_element.py
+-rw-rw-rw-   0        0        0      930 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageelements/text_page_element.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.852537 toolium-3.0.2.dev0/toolium/pageobjects/
+-rw-rw-rw-   0        0        0        0 2016-11-17 08:39:31.000000 toolium-3.0.2.dev0/toolium/pageobjects/__init__.py
+-rw-rw-rw-   0        0        0     1996 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/common_object.py
+-rw-rw-rw-   0        0        0     2273 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/mobile_page_object.py
+-rw-rw-rw-   0        0        0     3535 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pageobjects/page_object.py
+-rw-rw-rw-   0        0        0     2086 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/pytest_fixtures.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.882536 toolium-3.0.2.dev0/toolium/resources/
+-rw-rw-rw-   0        0        0     1383 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTests.css
+-rw-rw-rw-   0        0        0      757 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTests.js
+-rw-rw-rw-   0        0        0      752 2023-04-27 16:56:50.000000 toolium-3.0.2.dev0/toolium/resources/VisualTestsTemplate.html
+-rw-rw-rw-   0        0        0    12193 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/selenoid.py
+-rw-rw-rw-   0        0        0     8733 2023-05-08 11:36:54.000000 toolium-3.0.2.dev0/toolium/test_cases.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.983535 toolium-3.0.2.dev0/toolium/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/__init__.py
+-rw-rw-rw-   0        0        0     4089 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/data_generator.py
+-rw-rw-rw-   0        0        0    31957 2023-05-05 08:33:04.000000 toolium-3.0.2.dev0/toolium/utils/dataset.py
+-rw-rw-rw-   0        0        0     9480 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/download_files.py
+-rw-rw-rw-   0        0        0    18455 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/driver_utils.py
+-rw-rw-rw-   0        0        0    19112 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/driver_wait_utils.py
+-rw-rw-rw-   0        0        0     1608 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/path_utils.py
+-rw-rw-rw-   0        0        0    12916 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/utils/poeditor.py
+-rw-rw-rw-   0        0        0    22678 2023-04-27 16:57:03.000000 toolium-3.0.2.dev0/toolium/visual_test.py
+drwxrwxrwx   0        0        0        0 2023-05-19 09:08:22.649538 toolium-3.0.2.dev0/toolium.egg-info/
+-rw-rw-rw-   0        0        0     5526 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1564 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      124 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-19 09:08:22.000000 toolium-3.0.2.dev0/toolium.egg-info/top_level.txt
```

### Comparing `toolium-3.0.2/CHANGELOG.rst` & `toolium-3.0.2.dev0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Toolium Changelog
 =================
 
 v3.0.2
 ------
 
-*Release date: 2023-06-08*
+*Release date: In development*
 
 - `context.storage` must be initialized before dynamic environment steps in `before_feature` method
 - Mark scenario as failed when a dynamic environment step fails in `before_scenario`
 - Mark all feature scenarios as failed when a dynamic environment step fails in `before_feature` and `after_feature`
-- Configure minimal Appium-Python-Client version to 2.3.0 to avoid import errors
 
 v3.0.1
 ------
 
 *Release date: 2023-05-09*
 
 - Allow to search in `context.storage` using `[CONTEXT:a.b.c]` replacement when `before_feature` method is not used
```

### Comparing `toolium-3.0.2/LICENSE` & `toolium-3.0.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/PKG-INFO` & `toolium-3.0.2.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.2
+Version: 3.0.2.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.2/README.rst` & `toolium-3.0.2.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/setup.py` & `toolium-3.0.2.dev0/setup.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/behave/env_utils.py` & `toolium-3.0.2.dev0/toolium/behave/env_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/behave/environment.py` & `toolium-3.0.2.dev0/toolium/behave/environment.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/config_driver.py` & `toolium-3.0.2.dev0/toolium/config_driver.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/config_files.py` & `toolium-3.0.2.dev0/toolium/config_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/config_parser.py` & `toolium-3.0.2.dev0/toolium/config_parser.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/driver_wrapper.py` & `toolium-3.0.2.dev0/toolium/driver_wrapper.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/driver_wrappers_pool.py` & `toolium-3.0.2.dev0/toolium/driver_wrappers_pool.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/jira.py` & `toolium-3.0.2.dev0/toolium/jira.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/__init__.py` & `toolium-3.0.2.dev0/toolium/pageelements/__init__.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/button_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/button_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/checkbox_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/checkbox_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/group_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/group_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/input_radio_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/input_radio_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/input_text_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/input_text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/link_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/link_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/page_elements.py` & `toolium-3.0.2.dev0/toolium/pageelements/page_elements.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/select_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/select_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageelements/text_page_element.py` & `toolium-3.0.2.dev0/toolium/pageelements/text_page_element.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageobjects/common_object.py` & `toolium-3.0.2.dev0/toolium/pageobjects/common_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageobjects/mobile_page_object.py` & `toolium-3.0.2.dev0/toolium/pageobjects/mobile_page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pageobjects/page_object.py` & `toolium-3.0.2.dev0/toolium/pageobjects/page_object.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/pytest_fixtures.py` & `toolium-3.0.2.dev0/toolium/pytest_fixtures.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/resources/VisualTests.css` & `toolium-3.0.2.dev0/toolium/resources/VisualTests.css`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/resources/VisualTests.js` & `toolium-3.0.2.dev0/toolium/resources/VisualTests.js`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/resources/VisualTestsTemplate.html` & `toolium-3.0.2.dev0/toolium/resources/VisualTestsTemplate.html`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/selenoid.py` & `toolium-3.0.2.dev0/toolium/selenoid.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/test_cases.py` & `toolium-3.0.2.dev0/toolium/test_cases.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/data_generator.py` & `toolium-3.0.2.dev0/toolium/utils/data_generator.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/dataset.py` & `toolium-3.0.2.dev0/toolium/utils/dataset.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/download_files.py` & `toolium-3.0.2.dev0/toolium/utils/download_files.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/driver_utils.py` & `toolium-3.0.2.dev0/toolium/utils/driver_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/driver_wait_utils.py` & `toolium-3.0.2.dev0/toolium/utils/driver_wait_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/path_utils.py` & `toolium-3.0.2.dev0/toolium/utils/path_utils.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/utils/poeditor.py` & `toolium-3.0.2.dev0/toolium/utils/poeditor.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium/visual_test.py` & `toolium-3.0.2.dev0/toolium/visual_test.py`

 * *Files identical despite different names*

### Comparing `toolium-3.0.2/toolium.egg-info/PKG-INFO` & `toolium-3.0.2.dev0/toolium.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toolium
-Version: 3.0.2
+Version: 3.0.2.dev0
 Summary: Wrapper tool of Selenium and Appium libraries to test web and mobile applications in a single project
 Home-page: https://github.com/telefonica/toolium
 Author: Rubén González Alonso, Telefónica I+D
 Author-email: ruben.gonzalezalonso@telefonica.com
 License: Apache 2.0
 Keywords: selenium appium webdriver web_automation mobile_automation page_object visual_testing bdd behave pytest
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `toolium-3.0.2/toolium.egg-info/SOURCES.txt` & `toolium-3.0.2.dev0/toolium.egg-info/SOURCES.txt`

 * *Files identical despite different names*

