# Comparing `tmp/cbpi4-system-0.0.8.tar.gz` & `tmp/cbpi4-system-0.0.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-system-0.0.8.tar", last modified: Sun Jan  8 16:14:19 2023, max compression
+gzip compressed data, was "cbpi4-system-0.0.9rc1.tar", last modified: Thu Jun  8 11:03:36 2023, max compression
```

## Comparing `cbpi4-system-0.0.8.tar` & `cbpi4-system-0.0.9rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-01-08 16:14:19.689113 cbpi4-system-0.0.8/
--rw-rw-rw-   0        0        0    35149 2022-01-12 21:11:50.000000 cbpi4-system-0.0.8/LICENSE
--rw-rw-rw-   0        0        0       72 2022-01-12 21:11:50.000000 cbpi4-system-0.0.8/MANIFEST.in
--rw-rw-rw-   0        0        0     1925 2023-01-08 16:14:19.688097 cbpi4-system-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1556 2023-01-08 16:13:30.000000 cbpi4-system-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-08 16:14:19.651090 cbpi4-system-0.0.8/cbpi4-system/
--rw-rw-rw-   0        0        0     7598 2022-01-14 15:47:44.000000 cbpi4-system-0.0.8/cbpi4-system/__init__.py
--rw-rw-rw-   0        0        0       29 2022-01-12 21:11:50.000000 cbpi4-system-0.0.8/cbpi4-system/config.yaml
-drwxrwxrwx   0        0        0        0 2023-01-08 16:14:19.685089 cbpi4-system-0.0.8/cbpi4_system.egg-info/
--rw-rw-rw-   0        0        0     1925 2023-01-08 16:14:19.000000 cbpi4-system-0.0.8/cbpi4_system.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      267 2023-01-08 16:14:19.000000 cbpi4-system-0.0.8/cbpi4_system.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-08 16:14:19.000000 cbpi4-system-0.0.8/cbpi4_system.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-01-08 16:14:19.000000 cbpi4-system-0.0.8/cbpi4_system.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-01-08 16:14:19.000000 cbpi4-system-0.0.8/cbpi4_system.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-08 16:14:19.690094 cbpi4-system-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      962 2023-01-08 16:12:25.000000 cbpi4-system-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:03:36.217127 cbpi4-system-0.0.9rc1/
+-rw-rw-rw-   0        0        0    35149 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9rc1/LICENSE
+-rw-rw-rw-   0        0        0       72 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2145 2023-06-08 11:03:36.216126 cbpi4-system-0.0.9rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1744 2023-06-02 15:17:20.000000 cbpi4-system-0.0.9rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:03:36.178124 cbpi4-system-0.0.9rc1/cbpi4-system/
+-rw-rw-rw-   0        0        0    13312 2023-04-16 15:17:45.000000 cbpi4-system-0.0.9rc1/cbpi4-system/__init__.py
+-rw-rw-rw-   0        0        0       29 2022-01-12 21:11:50.000000 cbpi4-system-0.0.9rc1/cbpi4-system/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:03:36.214129 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/
+-rw-rw-rw-   0        0        0     2145 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      267 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-06-08 11:03:36.000000 cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:03:36.218123 cbpi4-system-0.0.9rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2023-06-02 15:16:49.000000 cbpi4-system-0.0.9rc1/setup.py
```

### Comparing `cbpi4-system-0.0.8/LICENSE` & `cbpi4-system-0.0.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-system-0.0.8/PKG-INFO` & `cbpi4-system-0.0.9rc1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,41 @@
-Metadata-Version: 2.1
-Name: cbpi4-system
-Version: 0.0.8
-Summary: CraftBeerPi4 Plugin for system fucntions
-Home-page: https://github.com/avollkopf/cbpi4-system
-Author: Alexander Vollkopf
-Author-email: avollkopf@web.de
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# CraftBeerPi4 System Functions Plugin
-
-### Functions:
-
-- Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
-
-![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
-
-### Sensors	
-
-Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
-	
-- CPU Load: 		CPU load in % (psutil: cpu_perc)
-- Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
-- Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
-- CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
-
-Each parameter has to be added as individual sensor.
-	
-![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
-
-### Installation: 
-- sudo pip3 install cbpi4-system
-- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
-	
-### Usage:
-
-- Add Hardware under Sensor and choose SystemSensor as Type
-- Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
-
-### Changelog:
-
-- 08.01.23: (0.0.8) updated requirements
-- 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
-- 12.01.22: (0.0.4) Reduced amount of mqtt traffic
-- 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
-- 02.09.21: (0.0.2) Remove Actor to reboot / shutdown system. Add automatic reboot and add system sensors
-- 18.06.21: (0.0.1) Initial commit with Actor to shutdown/reboot system
-
-
+# CraftBeerPi4 System Functions Plugin
+
+### Functions:
+
+- Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
+
+![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
+
+### Sensors	
+
+Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
+	
+- CPU Load: 		CPU load in % (psutil: cpu_perc)
+- Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
+- Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
+- CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
+
+Each parameter has to be added as individual sensor.
+	
+![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
+
+### Installation: 
+- sudo pip3 install cbpi4-system
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
+	
+### Usage:
+
+- Add Hardware under Sensor and choose SystemSensor as Type
+- Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
+
+### Changelog:
+
+- 02.06.23: (0.0.9.rc1) add cbpi4 version requirements
+- 16.04.23: (0.0.9.a6) fixed bug with creation of parameters
+- 05.04.23: (0.0.9.a5) test for gloabl plugin settings selection branch
+- 08.01.23: (0.0.8) updated requirements
+- 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
+- 12.01.22: (0.0.4) Reduced amount of mqtt traffic
+- 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
+- 02.09.21: (0.0.2) Remove Actor to reboot / shutdown system. Add automatic reboot and add system sensors
+- 18.06.21: (0.0.1) Initial commit with Actor to shutdown/reboot system
```

### Comparing `cbpi4-system-0.0.8/README.md` & `cbpi4-system-0.0.9rc1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,56 @@
-# CraftBeerPi4 System Functions Plugin
-
-### Functions:
-
-- Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
-
-![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
-
-### Sensors	
-
-Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
-	
-- CPU Load: 		CPU load in % (psutil: cpu_perc)
-- Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
-- Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
-- CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
-
-Each parameter has to be added as individual sensor.
-	
-![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
-
-### Installation: 
-- sudo pip3 install cbpi4-system
-- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
-	
-### Usage:
-
-- Add Hardware under Sensor and choose SystemSensor as Type
-- Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
-
-### Changelog:
-
-- 08.01.23: (0.0.8) updated requirements
-- 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
-- 12.01.22: (0.0.4) Reduced amount of mqtt traffic
-- 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
-- 02.09.21: (0.0.2) Remove Actor to reboot / shutdown system. Add automatic reboot and add system sensors
-- 18.06.21: (0.0.1) Initial commit with Actor to shutdown/reboot system
+Metadata-Version: 2.1
+Name: cbpi4-system
+Version: 0.0.9rc1
+Summary: CraftBeerPi4 Plugin for system fucntions
+Home-page: https://github.com/PiBrewing/cbpi4-system
+Author: Alexander Vollkopf
+Author-email: avollkopf@web.de
+License: UNKNOWN
+Keywords: globalsettings
+Platform: UNKNOWN
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# CraftBeerPi4 System Functions Plugin
+
+### Functions:
+
+- Plugin has capability to reboot Pi every day at a time that can be specified in the settings.
+
+![Auto Reboot](https://github.com/avollkopf/cbpi4-system/blob/main/AutoReboot.png?raw=true)
+
+### Sensors	
+
+Plugin will add system 'sensors' to monitor some system parameters. The psutil package is currently used for that purpose:
+	
+- CPU Load: 		CPU load in % (psutil: cpu_perc)
+- Available Memory:	Available system memory in Mb (psutil: vitrual_memory -> available)
+- Used memory:		Used memory in percent (psutil: vitrual_memory -> percent)
+- CPU Temp:		CPU temperature (psutil: sensors_temperatures -> cpu_thermal)
+
+Each parameter has to be added as individual sensor.
+	
+![Sensor Config](https://github.com/avollkopf/cbpi4-system/blob/main/SystemSensor.png?raw=true)
+
+### Installation: 
+- sudo pip3 install cbpi4-system
+- or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-system/archive/main.zip
+	
+### Usage:
+
+- Add Hardware under Sensor and choose SystemSensor as Type
+- Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
+
+### Changelog:
+
+- 02.06.23: (0.0.9.rc1) add cbpi4 version requirements
+- 16.04.23: (0.0.9.a6) fixed bug with creation of parameters
+- 05.04.23: (0.0.9.a5) test for gloabl plugin settings selection branch
+- 08.01.23: (0.0.8) updated requirements
+- 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
+- 12.01.22: (0.0.4) Reduced amount of mqtt traffic
+- 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
+- 02.09.21: (0.0.2) Remove Actor to reboot / shutdown system. Add automatic reboot and add system sensors
+- 18.06.21: (0.0.1) Initial commit with Actor to shutdown/reboot system
+
+
```

### Comparing `cbpi4-system-0.0.8/cbpi4_system.egg-info/PKG-INFO` & `cbpi4-system-0.0.9rc1/cbpi4_system.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cbpi4-system
-Version: 0.0.8
+Version: 0.0.9rc1
 Summary: CraftBeerPi4 Plugin for system fucntions
-Home-page: https://github.com/avollkopf/cbpi4-system
+Home-page: https://github.com/PiBrewing/cbpi4-system
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CraftBeerPi4 System Functions Plugin
 
 ### Functions:
@@ -38,14 +39,17 @@
 ### Usage:
 
 - Add Hardware under Sensor and choose SystemSensor as Type
 - Configure Autoreboot in settings (Default is 'No') and specify time of day (0-23 -> Full hour)
 
 ### Changelog:
 
+- 02.06.23: (0.0.9.rc1) add cbpi4 version requirements
+- 16.04.23: (0.0.9.a6) fixed bug with creation of parameters
+- 05.04.23: (0.0.9.a5) test for gloabl plugin settings selection branch
 - 08.01.23: (0.0.8) updated requirements
 - 16.01.22: (0.0.5) Adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.4) Reduced amount of mqtt traffic
 - 27.11.21: (0.0.3) New Readme file and link to plugin included in setup.py
 - 02.09.21: (0.0.2) Remove Actor to reboot / shutdown system. Add automatic reboot and add system sensors
 - 18.06.21: (0.0.1) Initial commit with Actor to shutdown/reboot system
```

### Comparing `cbpi4-system-0.0.8/setup.py` & `cbpi4-system-0.0.9rc1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,28 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-system',
-      version='0.0.8',
+      version='0.0.9.rc1',
       description='CraftBeerPi4 Plugin for system fucntions',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
-      url='https://github.com/avollkopf/cbpi4-system',
+      url='https://github.com/PiBrewing/cbpi4-system',
       include_package_data=True,
+      keywords='globalsettings',
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-system': ['*','*.txt', '*.rst', '*.yaml']},
       packages=['cbpi4-system'],
 
       install_requires=[
             'psutil>=5.9.0',
             'gpiozero',
+            'cbpi4>=4.1.10.rc2'
       ],
       long_description=long_description,
       long_description_content_type='text/markdown'
      )
```

