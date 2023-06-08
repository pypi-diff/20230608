# Comparing `tmp/cbpi4-PushOver-0.0.7.tar.gz` & `tmp/cbpi4-PushOver-0.0.8rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-PushOver-0.0.7.tar", last modified: Tue May 10 20:05:11 2022, max compression
+gzip compressed data, was "cbpi4-PushOver-0.0.8rc1.tar", last modified: Thu Jun  8 10:58:03 2023, max compression
```

## Comparing `cbpi4-PushOver-0.0.7.tar` & `cbpi4-PushOver-0.0.8rc1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-10 20:05:11.954290 cbpi4-PushOver-0.0.7/
--rw-rw-rw-   0        0        0    35149 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.7/LICENSE
--rw-rw-rw-   0        0        0       76 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     1059 2022-05-10 20:05:11.953290 cbpi4-PushOver-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0      663 2022-05-10 20:04:47.000000 cbpi4-PushOver-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2022-05-10 20:05:11.922291 cbpi4-PushOver-0.0.7/cbpi4-PushOver/
--rw-rw-rw-   0        0        0     2702 2021-04-17 11:12:15.000000 cbpi4-PushOver-0.0.7/cbpi4-PushOver/__init__.py
--rw-rw-rw-   0        0        0       31 2021-04-17 11:12:15.000000 cbpi4-PushOver-0.0.7/cbpi4-PushOver/config.yaml
-drwxrwxrwx   0        0        0        0 2022-05-10 20:05:11.950294 cbpi4-PushOver-0.0.7/cbpi4_PushOver.egg-info/
--rw-rw-rw-   0        0        0     1059 2022-05-10 20:05:11.000000 cbpi4-PushOver-0.0.7/cbpi4_PushOver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      244 2022-05-10 20:05:11.000000 cbpi4-PushOver-0.0.7/cbpi4_PushOver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-10 20:05:11.000000 cbpi4-PushOver-0.0.7/cbpi4_PushOver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2022-05-10 20:05:11.000000 cbpi4-PushOver-0.0.7/cbpi4_PushOver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-10 20:05:11.954290 cbpi4-PushOver-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      912 2022-05-10 20:04:23.000000 cbpi4-PushOver-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 10:58:03.070863 cbpi4-PushOver-0.0.8rc1/
+-rw-rw-rw-   0        0        0    35149 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.8rc1/LICENSE
+-rw-rw-rw-   0        0        0       76 2021-04-17 11:12:14.000000 cbpi4-PushOver-0.0.8rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1210 2023-06-08 10:58:03.068868 cbpi4-PushOver-0.0.8rc1/PKG-INFO
+-rw-rw-rw-   0        0        0      783 2023-06-02 15:25:09.000000 cbpi4-PushOver-0.0.8rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 10:58:03.023871 cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/
+-rw-rw-rw-   0        0        0     4286 2023-04-05 17:22:51.000000 cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/__init__.py
+-rw-rw-rw-   0        0        0       31 2021-04-17 11:12:15.000000 cbpi4-PushOver-0.0.8rc1/cbpi4-PushOver/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 10:58:03.066866 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/
+-rw-rw-rw-   0        0        0     1210 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      281 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-06-08 10:58:02.000000 cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 10:58:03.070863 cbpi4-PushOver-0.0.8rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1013 2023-06-02 15:25:11.000000 cbpi4-PushOver-0.0.8rc1/setup.py
```

### Comparing `cbpi4-PushOver-0.0.7/LICENSE` & `cbpi4-PushOver-0.0.8rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-PushOver-0.0.7/PKG-INFO` & `cbpi4-PushOver-0.0.8rc1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: cbpi4-PushOver
-Version: 0.0.7
+Version: 0.0.8rc1
 Summary: CraftBeerPi4 Plugin to forward Notifications to Pushover Push Notifications
-Home-page: https://github.com/avollkopf/cbpi4-PushOver
+Home-page: https://github.com/PiBrewing/cbpi4-PushOver
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Craftbeerpi4 PushOver Notifications Plugin
 
 ## Plugin to forward Craftbeerpi4 Notifications to Pushover Push Notification service
 
 - Installation:
 
-	- Plugin requires cbpi >= 4.0.0.33
+	- Plugin requires cbpi >= 4.1.10.rc2
 	- sudo pip3 install cbpi4-PushOver
 	- or installation from github
 
 
 - Usage:
 
 	- First Installation will add parameters to settings.
@@ -30,13 +31,15 @@
 - Parameters:
 
 	- pushover_token: your token for this service
 	- pushover_user: your user for this service
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 05.04.23: (0.0.8.a2) test for plugin settings selection test branch
 - 10.05.22: (0.0.7) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 02.04.21:  Minor changes
 - 15.03.21: Initial Release.
```

### Comparing `cbpi4-PushOver-0.0.7/README.md` & `cbpi4-PushOver-0.0.8rc1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Craftbeerpi4 PushOver Notifications Plugin
 
 ## Plugin to forward Craftbeerpi4 Notifications to Pushover Push Notification service
 
 - Installation:
 
-	- Plugin requires cbpi >= 4.0.0.33
+	- Plugin requires cbpi >= 4.1.10.rc2
 	- sudo pip3 install cbpi4-PushOver
 	- or installation from github
 
 
 - Usage:
 
 	- First Installation will add parameters to settings.
@@ -18,11 +18,13 @@
 - Parameters:
 
 	- pushover_token: your token for this service
 	- pushover_user: your user for this service
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 05.04.23: (0.0.8.a2) test for plugin settings selection test branch
 - 10.05.22: (0.0.7) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 02.04.21:  Minor changes
 - 15.03.21: Initial Release.
```

### Comparing `cbpi4-PushOver-0.0.7/cbpi4_PushOver.egg-info/PKG-INFO` & `cbpi4-PushOver-0.0.8rc1/cbpi4_PushOver.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: cbpi4-PushOver
-Version: 0.0.7
+Version: 0.0.8rc1
 Summary: CraftBeerPi4 Plugin to forward Notifications to Pushover Push Notifications
-Home-page: https://github.com/avollkopf/cbpi4-PushOver
+Home-page: https://github.com/PiBrewing/cbpi4-PushOver
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Craftbeerpi4 PushOver Notifications Plugin
 
 ## Plugin to forward Craftbeerpi4 Notifications to Pushover Push Notification service
 
 - Installation:
 
-	- Plugin requires cbpi >= 4.0.0.33
+	- Plugin requires cbpi >= 4.1.10.rc2
 	- sudo pip3 install cbpi4-PushOver
 	- or installation from github
 
 
 - Usage:
 
 	- First Installation will add parameters to settings.
@@ -30,13 +31,15 @@
 - Parameters:
 
 	- pushover_token: your token for this service
 	- pushover_user: your user for this service
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 05.04.23: (0.0.8.a2) test for plugin settings selection test branch
 - 10.05.22: (0.0.7) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 02.04.21:  Minor changes
 - 15.03.21: Initial Release.
```

### Comparing `cbpi4-PushOver-0.0.7/setup.py` & `cbpi4-PushOver-0.0.8rc1/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,22 +3,26 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-PushOver',
-      version='0.0.7',
+      version='0.0.8.rc1',
       description='CraftBeerPi4 Plugin to forward Notifications to Pushover Push Notifications',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
-      url='https://github.com/avollkopf/cbpi4-PushOver',
+      url='https://github.com/PiBrewing/cbpi4-PushOver',
       license='GPLv3',
       include_package_data=True,
+      keywords='globalsettings',
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-PushOver': ['*','*.txt', '*.rst', '*.yaml']},
       packages=['cbpi4-PushOver'],
+      install_requires=[
+          'cbpi4>=4.1.10.rc2'
+      ],
       long_description=long_description,
       long_description_content_type='text/markdown'
      )
```

