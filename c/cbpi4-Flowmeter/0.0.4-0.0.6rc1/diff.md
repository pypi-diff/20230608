# Comparing `tmp/cbpi4-Flowmeter-0.0.4.tar.gz` & `tmp/cbpi4-Flowmeter-0.0.6rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cbpi4-Flowmeter-0.0.4.tar", last modified: Wed May 11 05:03:54 2022, max compression
+gzip compressed data, was "cbpi4-Flowmeter-0.0.6rc1.tar", last modified: Thu Jun  8 11:02:51 2023, max compression
```

## Comparing `cbpi4-Flowmeter-0.0.4.tar` & `cbpi4-Flowmeter-0.0.6rc1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2022-05-11 05:03:54.239961 cbpi4-Flowmeter-0.0.4/
--rw-rw-rw-   0        0        0    35149 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       78 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     3209 2022-05-11 05:03:54.238963 cbpi4-Flowmeter-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     2874 2022-05-11 05:03:16.000000 cbpi4-Flowmeter-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2022-05-11 05:03:54.202968 cbpi4-Flowmeter-0.0.4/cbpi4-Flowmeter/
--rw-rw-rw-   0        0        0    11741 2022-05-10 16:23:32.000000 cbpi4-Flowmeter-0.0.4/cbpi4-Flowmeter/__init__.py
--rw-rw-rw-   0        0        0       32 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.4/cbpi4-Flowmeter/config.yaml
-drwxrwxrwx   0        0        0        0 2022-05-11 05:03:54.236960 cbpi4-Flowmeter-0.0.4/cbpi4_Flowmeter.egg-info/
--rw-rw-rw-   0        0        0     3209 2022-05-11 05:03:54.000000 cbpi4-Flowmeter-0.0.4/cbpi4_Flowmeter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      250 2022-05-11 05:03:54.000000 cbpi4-Flowmeter-0.0.4/cbpi4_Flowmeter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-05-11 05:03:54.000000 cbpi4-Flowmeter-0.0.4/cbpi4_Flowmeter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2022-05-11 05:03:54.000000 cbpi4-Flowmeter-0.0.4/cbpi4_Flowmeter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-05-11 05:03:54.239961 cbpi4-Flowmeter-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0      855 2022-05-11 05:03:31.000000 cbpi4-Flowmeter-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.037570 cbpi4-Flowmeter-0.0.6rc1/
+-rw-rw-rw-   0        0        0    35149 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6rc1/LICENSE
+-rw-rw-rw-   0        0        0       78 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6rc1/MANIFEST.in
+-rw-rw-rw-   0        0        0     4317 2023-06-08 11:02:51.036568 cbpi4-Flowmeter-0.0.6rc1/PKG-INFO
+-rw-rw-rw-   0        0        0     3953 2023-06-02 15:22:20.000000 cbpi4-Flowmeter-0.0.6rc1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:50.994571 cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/
+-rw-rw-rw-   0        0        0    16141 2023-06-02 15:20:10.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/__init__.py
+-rw-rw-rw-   0        0        0       32 2021-09-25 10:05:32.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/config.yaml
+drwxrwxrwx   0        0        0        0 2023-06-08 11:02:51.033568 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/
+-rw-rw-rw-   0        0        0     4317 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      288 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 11:02:50.000000 cbpi4-Flowmeter-0.0.6rc1/cbpi4_Flowmeter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:02:51.038567 cbpi4-Flowmeter-0.0.6rc1/setup.cfg
+-rw-rw-rw-   0        0        0      982 2023-06-02 15:22:12.000000 cbpi4-Flowmeter-0.0.6rc1/setup.py
```

### Comparing `cbpi4-Flowmeter-0.0.4/LICENSE` & `cbpi4-Flowmeter-0.0.6rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cbpi4-Flowmeter-0.0.4/PKG-INFO` & `cbpi4-Flowmeter-0.0.6rc1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,25 @@
-Metadata-Version: 2.1
-Name: cbpi4-Flowmeter
-Version: 0.0.4
-Summary: CraftBeerPi4 Flowsensor / Step Plugin 
-Home-page: https://github.com/avollkopf/cbpi4-Flowmeter
-Author: Alexander Vollkopf
-Author-email: avollkopf@web.de
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # CraftBeerPi4 FLowmeter Sensor / Step Plugin
 
+*For recently added VolumeSensor functionality scroll down*
+
 This plugin has been ported from the craftbeerpi3 plugin version (https://github.com/nanab/Flowmeter)
 
 The plugin includes sensor with action to reset the sensor and a custom step.
 Use a 10k ohm resistor on sensors signal pin to protect your Pi or connect the hall type flow sensor to your Craftbeerpi extension board at the flowmeter ports.
 
 Wire the sensor to the pi:
 Red -> 5v.
 Black -> GND.
 Yellow -> 10k ohm resistor -> GPIO pin. (or data on the extension board. No extra resistor required here)
 
 - Installation: 
-    - sudo pip3 install cbpi4-Flowmeter
-    --> or install from Repo
-    - sudo pip3 install https://github.com/avollkopf/cbpi4-Flowmeter/archive/main.zip
+    - pypi release: sudo pip3 install cbpi4-Flowmeter
+    - PiBrewing release: sudo pip3 install https://github.com/avollkopf/cbpi4-Flowmeter/archive/main.zip
+	- prash3r VolumeSensor testing branch: sudo pip3 install https://github.com/prash3r/cbpi4-Flowmeter/archive/VolumeSensor.zip
 
 - Sensor Usage:
     - On the settings page, choose a unit for the Volume (e.g. L, qt, gal, ...)
     - Add Sensor under Hardware and choose Flowmeter as Type
     - Several parameters can be set:
         - GPIO defines the GPIO that is used for the signal of the sensor (connected to the yellow cable)
         - Display defines if the total volume or the flow per second is displayed
@@ -55,17 +45,32 @@
     - An actor has to be defined that triggers the start and stop of the flow (e.g. magnetic valve)
     - You need to enter the volume that should flow while the step is active
     - When the step starts, the sensor will be set to 0.
     - You can select if the sensor should be set to 0 once the step is completed.
 
 ![Flowstep](https://github.com/avollkopf/cbpi4-Flowmeter/blob/main/FlowStep.png?raw=true)
 
+## VolumeSensor functionality
 
-## Changelog:
+The recently added *very simple* VolumeSensor functionality can be used like this:
+
+Parameters:
+ - GPIO: The GPIO Pin number in BCM numbering
+ - impulsesPerVolumeUnit: the amount of impulses that should be displaying the volume of 1 of whatever Unit. This is unit agnostic. Just use the same unit in your FlowStep if you use it.
+
+The VolumeSensor does nothing more then to count impulses and calculate the volume the number of impulses represent.
+
+Actions:
+ - Reset Sensor: resets the countet impulses and volume to 0
+ - Fake Impulse: fakes the detection of an impulse (i used this for testing because i dont have a flow sensor)
 
+
+
+## Changelog:
+- 14.05.23: (0.0.6.rc1) added simple VolumeSensor and cbpi4 requirement
+- 14.04.23: (0.0.5.a2) fixed bug in parameter generation
+- 08.04.23: (0.0.5.a1) added test support for plugin settings selection branch
 - 11.05.22: (0.0.4) Updated README (removed cbpi add)
 - 10.05.22: (0.0.3) removed cbpi dependency
 - 27.04.22: (0.0.2) Added MQTT based flowsensor with reset topic
 - 02.10.21: (0.0.1) Initial Release
 
-
-
```

### Comparing `cbpi4-Flowmeter-0.0.4/cbpi4-Flowmeter/__init__.py` & `cbpi4-Flowmeter-0.0.6rc1/cbpi4-Flowmeter/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -36,25 +36,57 @@
 class Flowmeter_Config(CBPiExtension):
 
     def __init__(self,cbpi):
         self.cbpi = cbpi
         self._task = asyncio.create_task(self.init_sensor())
 
     async def init_sensor(self):
+        plugin = await self.cbpi.plugin.load_plugin_list("cbpi4-Flowmeter")
+        self.version=plugin[0].get("Version","0.0.0")
+        self.name=plugin[0].get("Name","cbpi4-Flowmeter")
+
+        self.flowmeter_update = self.cbpi.config.get(self.name+"_update", None)
+
         unit = self.cbpi.config.get("flowunit", None)
         if unit is None:
             logging.info("INIT FLOW SENSOR CONFIG")
             try:
-                await self.cbpi.config.add("flowunit", "L", ConfigType.SELECT, "Flowmeter unit", [{"label": "L", "value": "L"},
+                await self.cbpi.config.add("flowunit", "L", type=ConfigType.SELECT, description="Flowmeter unit", 
+                                                                                    source=self.name,
+                                                                                    options=[{"label": "L", "value": "L"},
+                                                                                            {"label": "gal(us)", "value": "gal(us)"},
+                                                                                            {"label": "gal(uk)", "value": "gal(uk)"},
+                                                                                            {"label": "qt", "value": "qt"}])
+                                                                                            
+            except Exception as e:
+                    logger.warning('Unable to update config')
+                    logger.warning(e)
+        else:
+            if self.flowmeter_update == None or self.flowmeter_update != self.version:
+                try:
+                    await self.cbpi.config.add("flowunit", unit , type=ConfigType.SELECT, description="Flowmeter unit", 
+                                                                                    source=self.name,
+                                                                                    options=[{"label": "L", "value": "L"},
                                                                                             {"label": "gal(us)", "value": "gal(us)"},
                                                                                             {"label": "gal(uk)", "value": "gal(uk)"},
                                                                                             {"label": "qt", "value": "qt"}])
-            except:
-                logging.info("Flowmeter Error, Unable to update database.")
+                                                                                            
+                except Exception as e:
+                    logger.warning('Unable to update config')
+                    logger.warning(e)
 
+        if self.flowmeter_update == None or self.flowmeter_update != self.version:
+            try:
+                await self.cbpi.config.add(self.name+"_update", self.version, type=ConfigType.STRING,
+                                           description="Flowmeter Plugin Version",
+                                           source='hidden')
+            except Exception as e:
+                logger.warning('Unable to update config')
+                logger.warning(e)
+            pass         
 
 
 class FlowMeterData():
     SECONDS_IN_A_MINUTE = 60
     MS_IN_A_SECOND = 1000.0
     enabled = True
     clicks = 0
@@ -228,14 +260,70 @@
         logging.info("Reset Flowsensor")
         self.fms[int(self.gpio)].clear()
         return "Ok"
     
     def get_state(self):
         return dict(value=self.value)
 
+##########
+
+@parameters([Property.Select(label="GPIO", options=[0, 1, 2, 3, 4, 5, 6, 7, 8, 9, 10, 11, 12, 13, 14, 15, 16, 17, 18, 19, 20, 21, 22, 23, 24, 25, 26, 27],description="GPIO that is used by the Flowsensor"),
+            Property.Number(label="impulsesPerVolumeUnit", configurable=True, description="Here you need to configure how many impulses per Unit of measurement the sensor is sending. ")])
+
+class VolumeSensor(CBPiSensor):
+    
+    def __init__(self, cbpi, id, props):
+        super(VolumeSensor, self).__init__(cbpi, id, props)
+        self.value = 0
+        self.impulses = 0
+        self.liter = 0
+        self.gpio = self.props.get("GPIO",0)
+        self.IperL = self.props.get("impulsesPerVolumeUnit", 450)
+        self.LperI = float(1.0) / float(self.IperL)
+
+        try:
+            GPIO.setup(int(self.gpio),GPIO.IN, pull_up_down = GPIO.PUD_UP)
+            GPIO.remove_event_detect(int(self.gpio))
+            GPIO.add_event_detect(int(self.gpio), GPIO.RISING, callback=self.impulseDetected, bouncetime=20)
+        except Exception as e:
+            print(e)
+
+    @action(key="Reset Sensor", parameters=[])
+    async def Reset(self, **kwargs):
+        self.reset()
+
+    @action(key="Fake Impulse", parameters=[])
+    async def fakeImpulse(self, **kwargs):
+        self.impulseDetected("fake")
+
+    def impulseDetected(self, channel):
+        logging.debug("impulse detected on")
+        self.impulses = self.impulses + 1
+        self.liter = round(self.LperI * self.impulses,3)
+        self.value = self.liter
+
+    async def run(self):
+        while self.running is True:
+            self.log_data(self.value)
+            self.push_update(self.value)
+            await asyncio.sleep(1)
+
+    def reset(self):
+        logging.info(f'reset VolumeSensor from {self.liter} to 0.')
+        self.impulses = 0
+        self.liter = 0
+        self.value = 0
+        self.push_update(self.value)        
+        return "Ok"
+    
+    def get_state(self):
+        return dict(value=self.value)
+
+###########################################
+
 
 @parameters([Property.Number(label="Volume", description="Volume limit for this step", configurable=True),
              Property.Actor(label="Actor",description="Actor to switch media flow on and off"),
              Property.Sensor(label="Sensor"),
              Property.Select(label="Reset", options=["Yes","No"],description="Reset Flowmeter when done")])
 
 class FlowStep(CBPiStep):
@@ -300,12 +388,13 @@
             await asyncio.sleep(0.2)
 
         return StepResult.DONE
 
 
 def setup(cbpi):
     cbpi.plugin.register("FlowStep", FlowStep)
+    cbpi.plugin.register("VolumeSensor", VolumeSensor)
     cbpi.plugin.register("FlowSensor", FlowSensor)
     cbpi.plugin.register("Flowmeter_Config", Flowmeter_Config)
     if str(cbpi.static_config.get("mqtt", False)).lower() == "true":
         cbpi.plugin.register("MQTTFLowSensor", MQTTFlowSensor)
     pass
```

### Comparing `cbpi4-Flowmeter-0.0.4/cbpi4_Flowmeter.egg-info/PKG-INFO` & `cbpi4-Flowmeter-0.0.6rc1/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 Metadata-Version: 2.1
 Name: cbpi4-Flowmeter
-Version: 0.0.4
+Version: 0.0.6rc1
 Summary: CraftBeerPi4 Flowsensor / Step Plugin 
-Home-page: https://github.com/avollkopf/cbpi4-Flowmeter
+Home-page: https://github.com/PiBrewing/cbpi4-Flowmeter
 Author: Alexander Vollkopf
 Author-email: avollkopf@web.de
 License: UNKNOWN
+Keywords: globalsettings
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # CraftBeerPi4 FLowmeter Sensor / Step Plugin
 
+*For recently added VolumeSensor functionality scroll down*
+
 This plugin has been ported from the craftbeerpi3 plugin version (https://github.com/nanab/Flowmeter)
 
 The plugin includes sensor with action to reset the sensor and a custom step.
 Use a 10k ohm resistor on sensors signal pin to protect your Pi or connect the hall type flow sensor to your Craftbeerpi extension board at the flowmeter ports.
 
 Wire the sensor to the pi:
 Red -> 5v.
 Black -> GND.
 Yellow -> 10k ohm resistor -> GPIO pin. (or data on the extension board. No extra resistor required here)
 
 - Installation: 
-    - sudo pip3 install cbpi4-Flowmeter
-    --> or install from Repo
-    - sudo pip3 install https://github.com/avollkopf/cbpi4-Flowmeter/archive/main.zip
+    - pypi release: sudo pip3 install cbpi4-Flowmeter
+    - PiBrewing release: sudo pip3 install https://github.com/avollkopf/cbpi4-Flowmeter/archive/main.zip
+	- prash3r VolumeSensor testing branch: sudo pip3 install https://github.com/prash3r/cbpi4-Flowmeter/archive/VolumeSensor.zip
 
 - Sensor Usage:
     - On the settings page, choose a unit for the Volume (e.g. L, qt, gal, ...)
     - Add Sensor under Hardware and choose Flowmeter as Type
     - Several parameters can be set:
         - GPIO defines the GPIO that is used for the signal of the sensor (connected to the yellow cable)
         - Display defines if the total volume or the flow per second is displayed
@@ -55,17 +58,34 @@
     - An actor has to be defined that triggers the start and stop of the flow (e.g. magnetic valve)
     - You need to enter the volume that should flow while the step is active
     - When the step starts, the sensor will be set to 0.
     - You can select if the sensor should be set to 0 once the step is completed.
 
 ![Flowstep](https://github.com/avollkopf/cbpi4-Flowmeter/blob/main/FlowStep.png?raw=true)
 
+## VolumeSensor functionality
 
-## Changelog:
+The recently added *very simple* VolumeSensor functionality can be used like this:
+
+Parameters:
+ - GPIO: The GPIO Pin number in BCM numbering
+ - impulsesPerVolumeUnit: the amount of impulses that should be displaying the volume of 1 of whatever Unit. This is unit agnostic. Just use the same unit in your FlowStep if you use it.
+
+The VolumeSensor does nothing more then to count impulses and calculate the volume the number of impulses represent.
 
+Actions:
+ - Reset Sensor: resets the countet impulses and volume to 0
+ - Fake Impulse: fakes the detection of an impulse (i used this for testing because i dont have a flow sensor)
+
+
+
+## Changelog:
+- 14.05.23: (0.0.6.rc1) added simple VolumeSensor and cbpi4 requirement
+- 14.04.23: (0.0.5.a2) fixed bug in parameter generation
+- 08.04.23: (0.0.5.a1) added test support for plugin settings selection branch
 - 11.05.22: (0.0.4) Updated README (removed cbpi add)
 - 10.05.22: (0.0.3) removed cbpi dependency
 - 27.04.22: (0.0.2) Added MQTT based flowsensor with reset topic
 - 02.10.21: (0.0.1) Initial Release
```

### Comparing `cbpi4-Flowmeter-0.0.4/setup.py` & `cbpi4-Flowmeter-0.0.6rc1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,27 @@
-from setuptools import setup
-
-# read the contents of your README file
-from os import path
-this_directory = path.abspath(path.dirname(__file__))
-with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
-    long_description = f.read()
-
-setup(name='cbpi4-Flowmeter',
-      version='0.0.4',
-      description='CraftBeerPi4 Flowsensor / Step Plugin ',
-      author='Alexander Vollkopf',
-      author_email='avollkopf@web.de',
-      url='https://github.com/avollkopf/cbpi4-Flowmeter',
-      include_package_data=True,
-      package_data={
-        # If any package contains *.txt or *.rst files, include them:
-      '': ['*.txt', '*.rst', '*.yaml'],
-      'cbpi4-Flowmeter': ['*','*.txt', '*.rst', '*.yaml']},
-      packages=['cbpi4-Flowmeter'],
-      long_description=long_description,
-      long_description_content_type='text/markdown'
+from setuptools import setup
+
+# read the contents of your README file
+from os import path
+this_directory = path.abspath(path.dirname(__file__))
+with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
+    long_description = f.read()
+
+setup(name='cbpi4-Flowmeter',
+      version='0.0.6.rc1',
+      description='CraftBeerPi4 Flowsensor / Step Plugin ',
+      author='Alexander Vollkopf',
+      author_email='avollkopf@web.de',
+      url='https://github.com/PiBrewing/cbpi4-Flowmeter',
+      include_package_data=True,
+      keywords='globalsettings',
+      package_data={
+        # If any package contains *.txt or *.rst files, include them:
+      '': ['*.txt', '*.rst', '*.yaml'],
+      'cbpi4-Flowmeter': ['*','*.txt', '*.rst', '*.yaml']},
+      packages=['cbpi4-Flowmeter'],
+      install_requires=[
+          'cbpi4>=4.1.10.rc2'
+      ],
+      long_description=long_description,
+      long_description_content_type='text/markdown'
      )
```

