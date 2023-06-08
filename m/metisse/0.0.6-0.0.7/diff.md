# Comparing `tmp/metisse-0.0.6.tar.gz` & `tmp/metisse-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\metisse-0.0.6.tar", last modified: Tue Apr 18 02:34:46 2023, max compression
+gzip compressed data, was "dist\metisse-0.0.7.tar", last modified: Thu Jun  8 12:05:05 2023, max compression
```

## Comparing `metisse-0.0.6.tar` & `metisse-0.0.7.tar`

### file list

```diff
@@ -1,54 +1,68 @@
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.163861 metisse-0.0.6/
--rw-rw-rw-   0        0        0     9787 2023-04-17 02:58:36.000000 metisse-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     4519 2023-04-18 02:34:46.163861 metisse-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     4005 2023-04-18 02:19:32.000000 metisse-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:45.982755 metisse-0.0.6/metisse/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.012673 metisse-0.0.6/metisse/clients/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.025609 metisse-0.0.6/metisse/clients/android/
--rw-rw-rw-   0        0        0       26 2023-04-17 07:32:05.000000 metisse-0.0.6/metisse/clients/android/__init__.py
--rw-rw-rw-   0        0        0     1331 2023-04-17 07:32:05.000000 metisse-0.0.6/metisse/clients/android/adb.py
--rw-rw-rw-   0        0        0      701 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/client.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.038604 metisse-0.0.6/metisse/clients/ios/
--rw-rw-rw-   0        0        0       26 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/ios/__init__.py
--rw-rw-rw-   0        0        0     1853 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/clients/ios/wda.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.047583 metisse-0.0.6/metisse/example/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:45.943828 metisse-0.0.6/metisse/example/example_data/
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.050543 metisse-0.0.6/metisse/example/example_data/icon/
--rw-rw-rw-   0        0        0    90781 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/icon/example_template_face.png
--rw-rw-rw-   0        0        0    55904 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/icon/example_template_hand.png
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.053535 metisse-0.0.6/metisse/example/example_data/temp_image/
--rw-rw-rw-   0        0        0  2503418 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/temp_image/tmp0.png
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.126064 metisse-0.0.6/metisse/example/example_data/ui/
--rw-rw-rw-   0        0        0      313 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/gui_settings.py
--rw-rw-rw-   0        0        0    16964 2023-04-17 10:34:42.000000 metisse-0.0.6/metisse/example/example_data/ui/script_gui.py
--rw-rw-rw-   0        0        0     3934 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main.ui
--rw-rw-rw-   0        0        0     4195 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main_ui.py
--rw-rw-rw-   0        0        0     2287 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub.ui
--rw-rw-rw-   0        0        0     3568 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2.ui
--rw-rw-rw-   0        0        0     3740 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
--rw-rw-rw-   0        0        0      685 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3.ui
--rw-rw-rw-   0        0        0     1020 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
--rw-rw-rw-   0        0        0     2326 2023-04-17 02:59:18.000000 metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
--rw-rw-rw-   0        0        0     7076 2023-04-17 10:04:33.000000 metisse-0.0.6/metisse/example/generate_example.py
--rw-rw-rw-   0        0        0    22532 2023-04-17 10:04:58.000000 metisse-0.0.6/metisse/metisse.py
--rw-rw-rw-   0        0        0     1843 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/params.py
--rw-rw-rw-   0        0        0      205 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/settings.py
--rw-rw-rw-   0        0        0     2047 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/template_metis.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.161867 metisse-0.0.6/metisse/utils/
--rw-rw-rw-   0        0        0        0 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/__init__.py
--rw-rw-rw-   0        0        0     1539 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/image_recognition.py
--rw-rw-rw-   0        0        0     2190 2023-04-17 07:32:05.000000 metisse-0.0.6/metisse/utils/metisse_log.py
--rw-rw-rw-   0        0        0     6585 2023-04-17 09:13:34.000000 metisse-0.0.6/metisse/utils/metisse_path.py
--rw-rw-rw-   0        0        0      774 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/opencv_utils.py
--rw-rw-rw-   0        0        0     1051 2023-04-17 02:58:36.000000 metisse-0.0.6/metisse/utils/ui_client.py
-drwxrwxrwx   0        0        0        0 2023-04-18 02:34:46.005692 metisse-0.0.6/metisse.egg-info/
--rw-rw-rw-   0        0        0     4519 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1465 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      116 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-18 02:34:45.000000 metisse-0.0.6/metisse.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-18 02:34:46.163861 metisse-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1121 2023-04-18 02:30:34.000000 metisse-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.967091 metisse-0.0.7/
+-rw-rw-rw-   0        0        0     5998 2023-06-08 12:05:05.967091 metisse-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     4513 2023-06-08 09:03:19.000000 metisse-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.940093 metisse-0.0.7/metisse/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.949092 metisse-0.0.7/metisse/clients/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/clients/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.950091 metisse-0.0.7/metisse/clients/android/
+-rw-rw-rw-   0        0        0       26 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/clients/android/__init__.py
+-rw-rw-rw-   0        0        0     1331 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/clients/android/adb.py
+-rw-rw-rw-   0        0        0      701 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/clients/client.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.950091 metisse-0.0.7/metisse/clients/ios/
+-rw-rw-rw-   0        0        0       26 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/clients/ios/__init__.py
+-rw-rw-rw-   0        0        0     1853 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/clients/ios/wda.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.951091 metisse-0.0.7/metisse/example/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.935374 metisse-0.0.7/metisse/example/example_data/
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.952091 metisse-0.0.7/metisse/example/example_data/icon/
+-rw-rw-rw-   0        0        0    90781 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/icon/example_template_face.png
+-rw-rw-rw-   0        0        0    55904 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/icon/example_template_hand.png
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.952091 metisse-0.0.7/metisse/example/example_data/temp_image/
+-rw-rw-rw-   0        0        0  2503418 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/temp_image/tmp0.png
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.959092 metisse-0.0.7/metisse/example/example_data/ui/
+-rw-rw-rw-   0        0        0      313 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/gui_settings.py
+-rw-rw-rw-   0        0        0    16964 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/script_gui.py
+-rw-rw-rw-   0        0        0     3934 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_main.ui
+-rw-rw-rw-   0        0        0     4195 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_main_ui.py
+-rw-rw-rw-   0        0        0     2287 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub.ui
+-rw-rw-rw-   0        0        0     3568 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub2.ui
+-rw-rw-rw-   0        0        0     3740 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py
+-rw-rw-rw-   0        0        0      685 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub3.ui
+-rw-rw-rw-   0        0        0     1020 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
+-rw-rw-rw-   0        0        0     2326 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub_ui.py
+-rw-rw-rw-   0        0        0     6882 2023-06-08 10:58:25.000000 metisse-0.0.7/metisse/example/generate_example.py
+-rw-rw-rw-   0        0        0    22324 2023-06-08 10:43:17.000000 metisse-0.0.7/metisse/metisse.py
+-rw-rw-rw-   0        0        0     1843 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/params.py
+-rw-rw-rw-   0        0        0      205 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/settings.py
+-rw-rw-rw-   0        0        0     2047 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/template_metis.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.961091 metisse-0.0.7/metisse/utils/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/utils/__init__.py
+-rw-rw-rw-   0        0        0     1539 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/utils/image_recognition.py
+-rw-rw-rw-   0        0        0     2190 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/utils/metisse_log.py
+-rw-rw-rw-   0        0        0     6585 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/utils/metisse_path.py
+-rw-rw-rw-   0        0        0      774 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/utils/opencv_utils.py
+-rw-rw-rw-   0        0        0     1051 2023-06-08 09:03:19.000000 metisse-0.0.7/metisse/utils/ui_client.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.948091 metisse-0.0.7/metisse.egg-info/
+-rw-rw-rw-   0        0        0     5998 2023-06-08 12:05:05.000000 metisse-0.0.7/metisse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1957 2023-06-08 12:05:05.000000 metisse-0.0.7/metisse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:05:05.000000 metisse-0.0.7/metisse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      116 2023-06-08 12:05:05.000000 metisse-0.0.7/metisse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-08 12:05:05.000000 metisse-0.0.7/metisse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 12:05:05.967091 metisse-0.0.7/pytest_metisse/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/__init__.py
+-rw-rw-rw-   0        0        0       91 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/main.py
+-rw-rw-rw-   0        0        0     1855 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_adb.py
+-rw-rw-rw-   0        0        0     2624 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_check_image_recognition.py
+-rw-rw-rw-   0        0        0     2383 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_crop_screenshot.py
+-rw-rw-rw-   0        0        0     2712 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_default_tap.py
+-rw-rw-rw-   0        0        0     1835 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_generate_example.py
+-rw-rw-rw-   0        0        0     1673 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_image_recognition.py
+-rw-rw-rw-   0        0        0     2205 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_metis_log.py
+-rw-rw-rw-   0        0        0     1777 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_metis_path.py
+-rw-rw-rw-   0        0        0     3034 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_metisse_class.py
+-rw-rw-rw-   0        0        0     3058 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_save_screenshot_compression.py
+-rw-rw-rw-   0        0        0     1422 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_ui_client.py
+-rw-rw-rw-   0        0        0     1508 2023-06-08 09:03:19.000000 metisse-0.0.7/pytest_metisse/test_wdaclient.py
+-rw-rw-rw-   0        0        0       42 2023-06-08 12:05:05.967091 metisse-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1123 2023-06-08 12:04:20.000000 metisse-0.0.7/setup.py
```

### Comparing `metisse-0.0.6/PKG-INFO` & `metisse-0.0.7/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: metisse
-Version: 0.0.6
-Summary: A versatile and automated testing framework for games and apps on Android and iOS platforms
-Author: Henry Chen
-Author-email: weekand7@gmail.com
-License: Apache License 2.0
-Keywords: automation,automated-test,game,android,ios
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Metisse
 
 Metisse is a powerful image recognition and automation package designed to facilitate the development of scripts for mobile devices. It provides an extensive set of tools for image recognition, screenshot manipulation, and user interaction, such as tapping, swiping, and pressing.
 
 ## Features
 
 ![image](./demo.gif)
@@ -96,22 +82,38 @@
 ```bash
 from metisse.metisse import MetisseClass
 import metisse.example.generate_example as ex
 if __name__ == '__main__':
 
     ex.create_example_py_file()
 ```
-
-
+This is a script structure diagram.
+```bash
+your project
+│   script_example.py
+│
+├───ui
+├───icon
+│   └───script_example
+└───01234567(test_uid)
+    ├───backup
+    ├───log
+    ├───storage
+    │   └───script_example
+    └───temp_image
+```
 For more detailed information about the available methods and their usage, please refer to the MetisseClass Methods documentation.
+You can also use this tool for rapid development of automation scripts: [AndroidScreenCaptureTool](https://github.com/weekanda7/AndroidScreenCaptureTool).
+
+![image](./demo2.png)
 
 ## Contributing
 We welcome contributions to Metisse! If you'd like to contribute, please follow these steps:
 - Fork the repository
 - Create a new branch for your changes
 - Make your changes and test them thoroughly
 - Commit your changes and push them to your forked repository
 - Create a pull request with a detailed description of your changes
 - Please make sure to follow the code style and conventions used in the project.
 
 ## License
-Metisse is licensed under the Apache License 2.0.
+Metisse is licensed under the Apache License 2.0.
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `metisse-0.0.6/metisse/clients/android/adb.py` & `metisse-0.0.7/metisse/clients/android/adb.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/clients/client.py` & `metisse-0.0.7/metisse/clients/client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/clients/ios/wda.py` & `metisse-0.0.7/metisse/clients/ios/wda.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/icon/example_template_face.png` & `metisse-0.0.7/metisse/example/example_data/icon/example_template_face.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/icon/example_template_hand.png` & `metisse-0.0.7/metisse/example/example_data/icon/example_template_hand.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/temp_image/tmp0.png` & `metisse-0.0.7/metisse/example/example_data/temp_image/tmp0.png`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/script_gui.py` & `metisse-0.0.7/metisse/example/example_data/ui/script_gui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main.ui` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_main.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_main_ui.py` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_main_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub.ui` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2.ui` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub2.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub2_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3.ui` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub3.ui`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub3_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/example_data/ui/universal_script_gui_sub_ui.py` & `metisse-0.0.7/metisse/example/example_data/ui/universal_script_gui_sub_ui.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/example/generate_example.py` & `metisse-0.0.7/metisse/example/generate_example.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,15 +40,16 @@
 
 def example():
     print(get_current_path())
 
 
 def create_example_py_file():
     _path = get_current_path()
-    MetisseClass('01234567(test_uid)', _path, None, 'android')
+    _tmp = MetisseClass('01234567(test_uid)', _path, None, 'android')
+    _tmp._logger.close()
     _curPath = os.path.abspath(os.path.dirname(__file__))
 
     source_folder = os.path.join(_curPath, "example_data", 'icon')
     destination_folder = os.path.join(_path, 'icon', 'script_example')
     copy_images(source_folder, destination_folder)
 
     source_folder = os.path.join(_curPath, "example_data", 'temp_image')
@@ -60,81 +61,74 @@
     copy_ui(source_folder, destination_folder)
 
     content = '''import os
 import sys
 sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), "..")))
 from metisse.metisse import MetisseClass
 from metisse.params import ImageRecognitionParams , SaveParams
-
-class CustomImage(ImageRecognitionParams):
-
-    def __init__(self, *args, template_image_secondary_dir='script_example', **kwargs):
-        super().__init__(*args, template_image_secondary_dir=template_image_secondary_dir, **kwargs)
-
-
-class CustomSave(SaveParams):
-
-    def __init__(self, *args, save_image_secondary_dir='script_example', **kwargs):
-        super().__init__(*args, save_image_secondary_dir=save_image_secondary_dir, **kwargs)
+TEMPLATE = {'template_image_secondary_dir' : 'script_example'}
+SAVE = {'save_image_secondary_dir' : 'script_example'}
 
 class script_example(MetisseClass):
 
     def __init__(self, device_id='', relatively_path='', pyqt6_ui_label={}, os_environment=''):
         MetisseClass.__init__(
             self,
             device_id=device_id,
             relatively_path=relatively_path,
             pyqt6_ui_label=pyqt6_ui_label,
             os_environment=os_environment,
         )
 
     def __call__(self, *args, **kwargs):
         self.check_image_recognition(
-            CustomImage(screen_image_name='tmp0',
+            ImageRecognitionParams(screen_image_name='tmp0',
                                    template_image_name='example_template_hand',
-                                   is_refresh_screenshot=False))  # simulate image recognition hand icon
+                                   is_refresh_screenshot=False,**TEMPLATE))  # simulate image recognition hand icon
         print(f'hand pos = {self._img_recog_result.coordinate}')
 
         self.execute_time_sleep(1)  # wait 1 second
 
         self.default_tap(
             ImageRecognitionParams(screen_image_name='tmp0',
                                    template_image_name='example_template_face',
                                    template_image_secondary_dir='script_example',
                                    is_refresh_screenshot=False))  # simulate image recognition face icon and tap face pos
         self.default_tap(
-            CustomImage(screen_image_name='tmp0',
+            ImageRecognitionParams(screen_image_name='tmp0',
                                    template_image_name='example_template_face',
-                                   is_refresh_screenshot=False))  # simulate image recognition face icon and tap face pos
+                                   is_refresh_screenshot=False,**TEMPLATE))  # simulate image recognition face icon and tap face pos
 
         self.save_screenshot_compression( SaveParams(
                        save_image_name='save_image',
                        save_image_primary_dir='storage',
                        save_image_secondary_dir='script_example',
                        compression=0.5,
                        screenshot_wait_time=1,
                        is_save_image_name_add_time=True,
                        is_refresh_screenshot=False,
                        ))
-        self.save_screenshot_compression( CustomSave(
+        self.save_screenshot_compression( SaveParams(
                        save_image_name='save_image',
                        save_image_primary_dir='storage',
                        compression=0.5,
                        screenshot_wait_time=1,
                        is_save_image_name_add_time=True,
                        is_refresh_screenshot=False,
+                       **SAVE,
                        ))
-        self.save_screenshot_compression( CustomSave(
+        self.save_screenshot_compression( SaveParams(
                        save_image_name='save_image',
                        save_image_primary_dir='storage',
                        save_image_subdirs = ['third','forth'],
                        compression=0.5,
                        screenshot_wait_time=1,
                        is_save_image_name_add_time=True,
                        is_refresh_screenshot=False,
+                       **SAVE,
                        ))
         self.crop_screenshot((288, 260), (340, 294),
                              SaveParams(load_image_primary_dir='temp_image',
                                         save_image_primary_dir='storage',
                                         save_image_name='eyes',
                                         load_image_name='tmp0',
                                         is_refresh_screenshot=False))
```

### Comparing `metisse-0.0.6/metisse/metisse.py` & `metisse-0.0.7/metisse/metisse.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,28 +93,26 @@
             return ' -s ' + self._device_id
         return ''
 
     def check_gamelog(self, params: ImageRecognitionParams):
         params.template_image_name = 'log_button'
         try:
             _screen_image_path = self._script_path.get_screen_image_path(params)
+            if not os.path.isfile(_screen_image_path):
+                self.screenshot()
             _template_image_path = self._script_path.get_template_image_path(params)
+            if not os.path.isfile(_template_image_path):
+                raise FileNotFoundError(f"FileNotFoundError: {_template_image_path}")
             self.opencv_utils = Opencv_utils(_screen_image_path, _template_image_path)
             self._img_recog_result = image_recognition.match_template(self.opencv_utils.screen_image_mat,
                                                                       self.opencv_utils.template_image_mat, params.accuracy_val)
         except FileNotFoundError as error_msg:
             self._logger.info("FileNotFoundError: %s", error_msg)
-        except ValueError as error_msg:
-            self._logger.info("ValueError: %s", error_msg)
-            self.screenshot()
-            _screen_image_path = self._script_path.get_screen_image_path(params)
-            _template_image_path = self._script_path.get_template_image_path(params)
-            self.opencv_utils = Opencv_utils(_screen_image_path, _template_image_path)
-            self._img_recog_result = image_recognition.match_template(self.opencv_utils.screen_image_mat,
-                                                                      self.opencv_utils.template_image_mat, params.accuracy_val)
+        except Exception as error:
+            self._logger.error("An unexpected error occurred: %s", error)
 
         if self._img_recog_result.is_recognized:
             self._logger.info("match_template method : template_name=%s prob=%.4f accuracy_val=%.4f %s",
                               params.template_image_name, self._img_recog_result.recognition_threshold, params.accuracy_val,
                               self._img_recog_result.is_recognized)
             self._ui_client.send_image_path_to_ui(_image_path=_template_image_path)
             self._ui_client.send_log_to_ui(
@@ -202,15 +200,15 @@
 
             for _num in range(params.compare_times_counter):
                 for _temp_screen_image_name in _screen_image_name_list:
 
                     self.screenshot(_temp_screen_image_name, params.screen_image_primary_dir, params.screen_image_secondary_dir)
                 for _temp_screen_image_name in _screen_image_name_list:
                     _screen_image_path = self._script_path.get_screen_image_path(params)
-
+                    params.screen_image_name = _temp_screen_image_name
                     self.opencv_utils = Opencv_utils(_screen_image_path, _template_image_path)
                     self._img_recog_result = image_recognition.match_template(self.opencv_utils.screen_image_mat,
                                                                               self.opencv_utils.template_image_mat,
                                                                               params.accuracy_val)
                     self._logger.info("match_template method : template_name=%s  prob=%.4f accuracy_val=%.4f %s",
                                       params.template_image_name, self._img_recog_result.recognition_threshold,
                                       params.accuracy_val, self._img_recog_result.is_recognized)
```

### Comparing `metisse-0.0.6/metisse/params.py` & `metisse-0.0.7/metisse/params.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/template_metis.py` & `metisse-0.0.7/metisse/template_metis.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/utils/image_recognition.py` & `metisse-0.0.7/metisse/utils/image_recognition.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/utils/metisse_log.py` & `metisse-0.0.7/metisse/utils/metisse_log.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/utils/metisse_path.py` & `metisse-0.0.7/metisse/utils/metisse_path.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/utils/opencv_utils.py` & `metisse-0.0.7/metisse/utils/opencv_utils.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse/utils/ui_client.py` & `metisse-0.0.7/metisse/utils/ui_client.py`

 * *Files identical despite different names*

### Comparing `metisse-0.0.6/metisse.egg-info/SOURCES.txt` & `metisse-0.0.7/metisse.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE
 README.md
 setup.py
 metisse/__init__.py
 metisse/metisse.py
 metisse/params.py
 metisse/settings.py
 metisse/template_metis.py
@@ -33,8 +32,22 @@
 metisse/example/example_data/ui/universal_script_gui_sub3_ui.py
 metisse/example/example_data/ui/universal_script_gui_sub_ui.py
 metisse/utils/__init__.py
 metisse/utils/image_recognition.py
 metisse/utils/metisse_log.py
 metisse/utils/metisse_path.py
 metisse/utils/opencv_utils.py
-metisse/utils/ui_client.py
+metisse/utils/ui_client.py
+pytest_metisse/__init__.py
+pytest_metisse/main.py
+pytest_metisse/test_adb.py
+pytest_metisse/test_check_image_recognition.py
+pytest_metisse/test_crop_screenshot.py
+pytest_metisse/test_default_tap.py
+pytest_metisse/test_generate_example.py
+pytest_metisse/test_image_recognition.py
+pytest_metisse/test_metis_log.py
+pytest_metisse/test_metis_path.py
+pytest_metisse/test_metisse_class.py
+pytest_metisse/test_save_screenshot_compression.py
+pytest_metisse/test_ui_client.py
+pytest_metisse/test_wdaclient.py
```

### Comparing `metisse-0.0.6/setup.py` & `metisse-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name='metisse',
-    version="0.0.6",
+    version="0.0.7",
     description="A versatile and automated testing framework for games and apps on Android and iOS platforms",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Henry Chen',
     author_email='weekand7@gmail.com',
     license='Apache License 2.0',
     keywords=['automation', 'automated-test', 'game', 'android', 'ios'],
@@ -25,8 +25,8 @@
         'tidevice>=0.9.12',
     ],
     classifiers=[
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
     ],
-)
+)
```

