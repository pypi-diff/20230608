# Comparing `tmp/cbpi4-PCF8574-GPIO-0.0.4.tar.gz` & `tmp/cbpi4-PCF8574-GPIO-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-PCF8574-GPIO-0.0.4.tar", last modified: Tue May 10 17:51:15 2022, max compression
+gzip compressed data, was "cbpi4-PCF8574-GPIO-0.0.6rc1.tar", last modified: Thu Jun  8 11:04:17 2023, max compression
```

## Comparing `cbpi4-PCF8574-GPIO-0.0.4.tar` & `cbpi4-PCF8574-GPIO-0.0.6rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-10 17:51:15.277140 cbpi4-PCF8574-GPIO-0.0.4/
--rw-rw-rw-   0        0        0    35149 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       84 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     2036 2022-05-10 17:51:15.276134 cbpi4-PCF8574-GPIO-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     1665 2022-05-10 15:31:33.000000 cbpi4-PCF8574-GPIO-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-05-10 17:51:15.240145 cbpi4-PCF8574-GPIO-0.0.4/cbpi4-PCF8574-GPIO/
--rw-rw-rw-   0        0        0     5004 2021-12-09 18:05:34.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4-PCF8574-GPIO/__init__.py
--rw-rw-rw-   0        0        0       35 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4-PCF8574-GPIO/config.yaml
-drwxrwxrwx   0        0        0        0 2022-05-10 17:51:15.274161 cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/
--rw-rw-rw-   0        0        0     2036 2022-05-10 17:51:15.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      309 2022-05-10 17:51:15.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-10 17:51:15.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2022-05-10 17:51:15.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2022-05-10 17:51:15.000000 cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-10 17:51:15.277140 cbpi4-PCF8574-GPIO-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      932 2022-05-10 15:31:14.000000 cbpi4-PCF8574-GPIO-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:17.115646 cbpi4-PCF8574-GPIO-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35149 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       84 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2243 2023-06-08 11:04:17.114643 cbpi4-PCF8574-GPIO-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     1841 2023-06-02 15:13:11.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:17.079641 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/
+-rw-rw-rw-   0        0        0     6519 2023-04-07 15:05:20.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/__init__.py
+-rw-rw-rw-   0        0        0       35 2021-12-08 16:22:47.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:04:17.112640 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/
+-rw-rw-rw-   0        0        0     2243 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      309 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-08 11:04:16.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:04:17.115646 cbpi4-PCF8574-GPIO-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0      996 2023-06-02 15:12:44.000000 cbpi4-PCF8574-GPIO-0.0.6rc1/setup.py
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.4/LICENSE` & `cbpi4-PCF8574-GPIO-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-PCF8574-GPIO-0.0.4/PKG-INFO` & `cbpi4-PCF8574-GPIO-0.0.6rc1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: cbpi4-PCF8574-GPIO
-Version: 0.0.4
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 PCF8574 Actor Plugin
-Home-page: https://github.com/avollkopf/cbpi4-PCF8574-GPIO
+Home-page: https://github.com/PiBrewing/cbpi4-PCF8574-GPIO
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CraftBeerPi4 PCF8574 IO Actor Plugin 
 
 ### PCF8574 based Actor
 
 Plugin will add an PCF8574Actor which has to possibility to define up 8 additional actors to your pi. The board needs to be connected via I2C
 Theoretically, multiple boards (up to 8) could be connected with different addresses to make up to 64 IO ports available. However, the pulgin supports one board.
 
 ### Installation: 
 - sudo pip3 install cbpi4-PCF8574-GPIO
 - or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-PCF8574-GPIO/archive/main.zip
-- cbpi add cbpi4-PCF8574-GPIO
 	
 ### Usage:
 
 - Configure the PCF8574 I2C Address in the cbpi global settings. 
 
 ![PCF8574 I2C address Settings](https://github.com/avollkopf/cbpi4-PCF8574-GPIO/blob/main/PCF8574_Address_Settings.png?raw=true)
 
@@ -37,13 +37,16 @@
 
 Some information can be found here: https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/
 Connect the device to 5 Volt, GND and your I2C bus. Check the Address ans set it to a different address if required
 According to the datasheet, the pins can handle up to 25 mA. If you want to trigger an SSR or a relais, it is recommended to add a darlington array like the ULN2308
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) Added cbpi4 version requirement
+- 07.04.23: (0.0.6.a1) Added fucntions for plugins settings selection branches of server and ui
+- 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 10.12.21: (0.0.3) Updated README
 - 09.12.21: (0.0.2) Bug Fix for power
 - 09-12-21: (0.0.1) Initial release
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.4/README.md` & `cbpi4-PCF8574-GPIO-0.0.6rc1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 Plugin will add an PCF8574Actor which has to possibility to define up 8 additional actors to your pi. The board needs to be connected via I2C
 Theoretically, multiple boards (up to 8) could be connected with different addresses to make up to 64 IO ports available. However, the pulgin supports one board.
 
 ### Installation: 
 - sudo pip3 install cbpi4-PCF8574-GPIO
 - or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-PCF8574-GPIO/archive/main.zip
-- cbpi add cbpi4-PCF8574-GPIO
 	
 ### Usage:
 
 - Configure the PCF8574 I2C Address in the cbpi global settings. 
 
 ![PCF8574 I2C address Settings](https://github.com/avollkopf/cbpi4-PCF8574-GPIO/blob/main/PCF8574_Address_Settings.png?raw=true)
 
@@ -25,11 +24,14 @@
 
 Some information can be found here: https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/
 Connect the device to 5 Volt, GND and your I2C bus. Check the Address ans set it to a different address if required
 According to the datasheet, the pins can handle up to 25 mA. If you want to trigger an SSR or a relais, it is recommended to add a darlington array like the ULN2308
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) Added cbpi4 version requirement
+- 07.04.23: (0.0.6.a1) Added fucntions for plugins settings selection branches of server and ui
+- 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 10.12.21: (0.0.3) Updated README
 - 09.12.21: (0.0.2) Bug Fix for power
 - 09-12-21: (0.0.1) Initial release
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.4/cbpi4-PCF8574-GPIO/__init__.py` & `cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4-PCF8574-GPIO/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -47,23 +47,51 @@
         logger.info("Checked PCF Address")
         PCF8574_Address = self.cbpi.config.get("PCF8574_Address", "0x20")
         address=int(PCF8574_Address,16)
         PCFActor(address)
 
     async def PCF8574_Address(self): 
         global PCF8574_address
+        plugin = await self.cbpi.plugin.load_plugin_list("cbpi4-PCF8574-GPIO")
+        self.version=plugin[0].get("Version","0.0.0")
+        self.name=plugin[0].get("Name","cbpi4-PCF8574-GPIO")
+
+        self.PCF8574_update = self.cbpi.config.get(self.name+"_update", None)
+
+
         PCF8574_Address = self.cbpi.config.get("PCF8574_Address", None)
         if PCF8574_Address is None:
             logger.info("INIT PCF8574_Address")
             try:
-                await self.cbpi.config.add('PCF8574_Address', '0x20', ConfigType.STRING, 'PCF8574 I2C Bus address (e.g. 0x20). Change requires reboot')
+                await self.cbpi.config.add('PCF8574_Address', '0x20', type=ConfigType.STRING, 
+                                           description='PCF8574 I2C Bus address (e.g. 0x20). Change requires reboot',
+                                           source=self.name)
                 PCF8574_Address = self.cbpi.config.get("PCF8574_Address", None)
-            except:
-                logger.warning('Unable to update database')
-
+            except Exception as e:
+                    logger.warning('Unable to update config')
+                    logger.warning(e)
+        else:
+            if self.PCF8574_update == None or self.PCF8574_update != self.version:
+                try:
+                    await self.cbpi.config.add('PCF8574_Address', PCF8574_Address, type=ConfigType.STRING, 
+                                           description='PCF8574 I2C Bus address (e.g. 0x20). Change requires reboot',
+                                           source=self.name)
+                except Exception as e:
+                    logger.warning('Unable to update config')
+                    logger.warning(e)
+                    
+        if self.PCF8574_update == None or self.PCF8574_update != self.version:
+            try:
+                await self.cbpi.config.add(self.name+"_update", self.version, type=ConfigType.STRING,
+                                           description="PCF8574 Plugin Version",
+                                           source='hidden')
+            except Exception as e:
+                logger.warning('Unable to update config')
+                logger.warning(e)
+            pass                
 
 @parameters([Property.Select(label="GPIO", options=["p0","p1","p2","p3","p4","p5","p6","p7"]),
              Property.Select(label="Inverted", options=["Yes", "No"],description="No: Active on high; Yes: Active on low"),
              Property.Select(label="SamplingTime", options=[2,5],description="Time in seconds for power base interval (Default:5)")])
 class PCF8574Actor(CBPiActor):
     # Custom property which can be configured by the user
     @action("Set Power", parameters=[Property.Number(label="Power", configurable=True,description="Power Setting [0-100]")])
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.4/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO` & `cbpi4-PCF8574-GPIO-0.0.6rc1/cbpi4_PCF8574_GPIO.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: cbpi4-PCF8574-GPIO
-Version: 0.0.4
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 PCF8574 Actor Plugin
-Home-page: https://github.com/avollkopf/cbpi4-PCF8574-GPIO
+Home-page: https://github.com/PiBrewing/cbpi4-PCF8574-GPIO
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CraftBeerPi4 PCF8574 IO Actor Plugin 
 
 ### PCF8574 based Actor
 
 Plugin will add an PCF8574Actor which has to possibility to define up 8 additional actors to your pi. The board needs to be connected via I2C
 Theoretically, multiple boards (up to 8) could be connected with different addresses to make up to 64 IO ports available. However, the pulgin supports one board.
 
 ### Installation: 
 - sudo pip3 install cbpi4-PCF8574-GPIO
 - or install from repo: sudo pip3 install https://github.com/avollkopf/cbpi4-PCF8574-GPIO/archive/main.zip
-- cbpi add cbpi4-PCF8574-GPIO
 	
 ### Usage:
 
 - Configure the PCF8574 I2C Address in the cbpi global settings. 
 
 ![PCF8574 I2C address Settings](https://github.com/avollkopf/cbpi4-PCF8574-GPIO/blob/main/PCF8574_Address_Settings.png?raw=true)
 
@@ -37,13 +37,16 @@
 
 Some information can be found here: https://www.instructables.com/PCF8574-GPIO-Extender-With-Arduino-and-NodeMCU/
 Connect the device to 5 Volt, GND and your I2C bus. Check the Address ans set it to a different address if required
 According to the datasheet, the pins can handle up to 25 mA. If you want to trigger an SSR or a relais, it is recommended to add a darlington array like the ULN2308
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) Added cbpi4 version requirement
+- 07.04.23: (0.0.6.a1) Added fucntions for plugins settings selection branches of server and ui
+- 11.05.22: (0.0.5) Updated README (removed cbpi add)
 - 10.05.22: (0.0.4) Removed cbpi dependency
 - 10.12.21: (0.0.3) Updated README
 - 09.12.21: (0.0.2) Bug Fix for power
 - 09-12-21: (0.0.1) Initial release
```

### Comparing `cbpi4-PCF8574-GPIO-0.0.4/setup.py` & `cbpi4-PCF8574-GPIO-0.0.6rc1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='cbpi4-PCF8574-GPIO',
-      version='0.0.4',
+      version='0.0.6.rc1',
       description='CraftBeerPi4 PCF8574 Actor Plugin',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
-      url='https://github.com/avollkopf/cbpi4-PCF8574-GPIO',
+      url='https://github.com/PiBrewing/cbpi4-PCF8574-GPIO',
       include_package_data=True,
+      keywords='globalsettings',
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-PCF8574-GPIO': ['*','*.txt', '*.rst', '*.yaml']},
       packages=['cbpi4-PCF8574-GPIO'],
       install_requires=[
       'smbus2',
-      'pcf8574-io'
+      'pcf8574-io',
+      'cbpi4>=4.1.10.rc2'
       ],
       long_description=long_description,
       long_description_content_type='text/markdown'
      )
```

