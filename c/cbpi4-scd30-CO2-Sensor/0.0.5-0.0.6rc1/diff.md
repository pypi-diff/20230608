# Comparing `tmp/cbpi4-scd30_CO2_Sensor-0.0.5.tar.gz` & `tmp/cbpi4-scd30-CO2-Sensor-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-scd30_CO2_Sensor-0.0.5.tar", last modified: Tue May 10 19:58:15 2022, max compression
+gzip compressed data, was "cbpi4-scd30-CO2-Sensor-0.0.6rc1.tar", last modified: Thu Jun  8 11:02:07 2023, max compression
```

## Comparing `cbpi4-scd30_CO2_Sensor-0.0.5.tar` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-10 19:58:15.358731 cbpi4-scd30_CO2_Sensor-0.0.5/
--rw-rw-rw-   0        0        0    35149 2021-11-29 14:48:50.000000 cbpi4-scd30_CO2_Sensor-0.0.5/LICENSE
--rw-rw-rw-   0        0        0       92 2021-11-29 14:48:50.000000 cbpi4-scd30_CO2_Sensor-0.0.5/MANIFEST.in
--rw-rw-rw-   0        0        0     2299 2022-05-10 19:58:15.356728 cbpi4-scd30_CO2_Sensor-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1902 2022-05-10 19:57:28.000000 cbpi4-scd30_CO2_Sensor-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2022-05-10 19:58:15.317733 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4-scd30_CO2_Sensor/
--rw-rw-rw-   0        0        0     5758 2022-01-14 15:45:17.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4-scd30_CO2_Sensor/__init__.py
--rw-rw-rw-   0        0        0       39 2021-11-29 14:48:50.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4-scd30_CO2_Sensor/config.yaml
-drwxrwxrwx   0        0        0        0 2022-05-10 19:58:15.353724 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/
--rw-rw-rw-   0        0        0     2299 2022-05-10 19:58:15.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      337 2022-05-10 19:58:15.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-10 19:58:15.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2022-05-10 19:58:15.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2022-05-10 19:58:15.000000 cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-10 19:58:15.358731 cbpi4-scd30_CO2_Sensor-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      979 2022-05-10 19:57:11.000000 cbpi4-scd30_CO2_Sensor-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:07.926223 cbpi4-scd30-CO2-Sensor-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35149 2021-11-29 14:48:50.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       92 2023-04-08 13:04:58.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2501 2023-06-08 11:02:07.925168 cbpi4-scd30-CO2-Sensor-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     2072 2023-06-02 15:19:03.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:07.874807 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/
+-rw-rw-rw-   0        0        0     8172 2023-04-16 15:20:12.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/__init__.py
+-rw-rw-rw-   0        0        0       39 2023-04-08 13:05:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:07.922487 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/
+-rw-rw-rw-   0        0        0     2501 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      337 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2023-06-08 11:02:07.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:02:07.926223 cbpi4-scd30-CO2-Sensor-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0     1044 2023-06-02 15:19:08.000000 cbpi4-scd30-CO2-Sensor-0.0.6rc1/setup.py
```

### Comparing `cbpi4-scd30_CO2_Sensor-0.0.5/LICENSE` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-scd30_CO2_Sensor-0.0.5/PKG-INFO` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
-Name: cbpi4-scd30_CO2_Sensor
-Version: 0.0.5
+Name: cbpi4-scd30-CO2-Sensor
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Plugin for SCD30 based CO2 Sensor
-Home-page: https://github.com/avollkopf/cbpi4-scd30-co2-sensor
+Home-page: https://github.com/PiBrewing/cbpi4-scd30-co2-sensor
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CraftBeerPi4 SCD30 based CO2 Sensor Plugin
 
 ### Sensors	
@@ -44,13 +45,16 @@
 
 Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
 
 The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
+- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
 - 10.05.22: (0.0.4) Removed cbpi requirement
 - 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.2) Reduction of mqtt traffic
 - 23.07.21: (0.0.1) Initial commit
```

### Comparing `cbpi4-scd30_CO2_Sensor-0.0.5/README.md` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -32,11 +32,14 @@
 
 Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
 
 The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
+- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
 - 10.05.22: (0.0.4) Removed cbpi requirement
 - 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.2) Reduction of mqtt traffic
 - 23.07.21: (0.0.1) Initial commit
```

### Comparing `cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4-scd30_CO2_Sensor/__init__.py` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4-scd30-CO2-Sensor/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,14 +19,20 @@
 class SCD30_Config(CBPiExtension):
 
     def __init__(self,cbpi):
         self.cbpi = cbpi
         self._task = asyncio.create_task(self.init_sensor())
 
     async def init_sensor(self):
+        plugin = await self.cbpi.plugin.load_plugin_list("cbpi4-scd30-CO2-Sensor")
+        self.version=plugin[0].get("Version","0.0.0")
+        self.name=plugin[0].get("Name","cbpi4-scd30-CO2-Sensor")
+
+        self.scd30_update = self.cbpi.config.get(self.name+"_update", None)
+
         global SCD30_Active
         SCD30_Active=False
         await self.scd30_interval()
         self.scd30 = SCD30()
         self.Interval = self.cbpi.config.get("scd30_interval", 5)
         retries = 30
         logging.info("Probing SCD30 sensor...")
@@ -69,24 +75,48 @@
 
     async def scd30_interval(self):
         global scd30_interval
         scd30_interval = self.cbpi.config.get("scd30_interval", None)
         if scd30_interval is None:
             logger.info("INIT scd30_intervall")
             try:
-                await self.cbpi.config.add("scd30_interval", 5, ConfigType.SELECT, "SCD30 Readout Interval", [{"label": "2s","value": 2},
+                await self.cbpi.config.add("scd30_interval", 5, type=ConfigType.SELECT, description="SCD30 Readout Interval",
+                                                                                                    source=self.name,
+                                                                                                    options= [{"label": "2s","value": 2},
                                                                                                             {"label": "5s", "value": 5},
                                                                                                             {"label": "10s", "value": 10},
                                                                                                             {"label": "15s", "value": 15},
                                                                                                             {"label": "30s", "value": 30},
                                                                                                             {"label": "60s", "value": 60}])
+                                                                                                            
                 scd30_interval = self.cbpi.config.get("scd30_interval", None)
             except:
                 logger.warning('Unable to update database')
+        else:
+            if self.scd30_update == None or self.scd30_update != self.version:
+                try:
+                    await self.cbpi.config.add("scd30_interval", scd30_interval, type=ConfigType.SELECT, description="SCD30 Readout Interval",
+                                                                                                    source=self.name,
+                                                                                                    options= [{"label": "2s","value": 2},
+                                                                                                            {"label": "5s", "value": 5},
+                                                                                                            {"label": "10s", "value": 10},
+                                                                                                            {"label": "15s", "value": 15},
+                                                                                                            {"label": "30s", "value": 30},
+                                                                                                            {"label": "60s", "value": 60}])
+                                                                                                            
+
+                except:
+                    logger.warning('Unable to update database')
 
+        if self.scd30_update == None or self.scd30_update != self.version:
+            try:
+                 await self.cbpi.config.add(self.name+"_update", self.version,type=ConfigType.STRING, description='SCD30 Version update', source='hidden')
+            except Exception as e:
+                logger.warning('Unable to update database')
+                logger.warning(e)
 
     async def ReadSensor(self):
         logging.info("Starting scd30 ReadSensor Loop")
         global cache
         while True:
             if self.scd30.get_data_ready():
                 measurement = self.scd30.read_measurement()
```

### Comparing `cbpi4-scd30_CO2_Sensor-0.0.5/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/cbpi4_scd30_CO2_Sensor.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: cbpi4-scd30-CO2-Sensor
-Version: 0.0.5
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Plugin for SCD30 based CO2 Sensor
-Home-page: https://github.com/avollkopf/cbpi4-scd30-co2-sensor
+Home-page: https://github.com/PiBrewing/cbpi4-scd30-co2-sensor
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: GPLv3
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CraftBeerPi4 SCD30 based CO2 Sensor Plugin
 
 ### Sensors	
@@ -44,13 +45,16 @@
 
 Information on how read from then sensor is documented here: https://cdn.sparkfun.com/assets/d/c/0/7/2/SCD30_Interface_Description.pdf
 
 The sensor is connected via I2C and has the address 0x61. The user just needs to activate I2C in the raspi config and connect the sensor to the I2C bus. The supply voltage (VDD) can be 5V, but the I2C bus has to be at 3.3V
 
 ### Changelog:
 
+- 02.06.23: (0.0.6.rc1) added cbpi4 requirement
+- 16.04.23: (0.0.6.a6) fixed bug in parameter generation
+- 04.04.23: (0.0.6.a5) test for plugin settings selection branch
 - 10.05.22: (0.0.4) Removed cbpi requirement
 - 16.01.22: (0.0.3) adaption for cbpi 4.0.1.2
 - 12.01.22: (0.0.2) Reduction of mqtt traffic
 - 23.07.21: (0.0.1) Initial commit
```

### Comparing `cbpi4-scd30_CO2_Sensor-0.0.5/setup.py` & `cbpi4-scd30-CO2-Sensor-0.0.6rc1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,28 +2,30 @@
 
 # read the contents of your README file
 from os import path
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
-setup(name='cbpi4-scd30_CO2_Sensor',
-      version='0.0.5',
+setup(name='cbpi4-scd30-CO2-Sensor',
+      version='0.0.6.rc1',
       description='CraftBeerPi4 Plugin for SCD30 based CO2 Sensor',
       author='Alexander Vollkopf',
       author_email='avollkopf@web.de',
-      url='https://github.com/avollkopf/cbpi4-scd30-co2-sensor',
+      url='https://github.com/PiBrewing/cbpi4-scd30-co2-sensor',
       license='GPLv3',
       include_package_data=True,
+      keywords='globalsettings',
       package_data={
         # If any package contains *.txt or *.rst files, include them:
       '': ['*.txt', '*.rst', '*.yaml'],
       'cbpi4-scd30_CO2_Sensor': ['*','*.txt', '*.rst', '*.yaml']},
-      packages=['cbpi4-scd30_CO2_Sensor'],
+      packages=['cbpi4-scd30-CO2-Sensor'],
         install_requires=[
         'smbus2',
         'scd30_i2c',
+        'cbpi4>=4.1.10.rc2'
   ],
   long_description=long_description,
   long_description_content_type='text/markdown'
 
      )
```

