# Comparing `tmp/lumimqtt-1.0.8.tar.gz` & `tmp/lumimqtt-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lumimqtt-1.0.8.tar", last modified: Sun Jan 24 12:09:37 2021, max compression
+gzip compressed data, was "dist/lumimqtt-1.0.9.tar", last modified: Thu Jan 28 22:17:06 2021, max compression
```

## Comparing `lumimqtt-1.0.8.tar` & `lumimqtt-1.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 belokobylskiy   (501) staff       (20)        0 2021-01-24 12:09:37.368652 lumimqtt-1.0.8/
--rw-r--r--   0 belokobylskiy   (501) staff       (20)      197 2020-10-20 08:10:38.000000 lumimqtt-1.0.8/CHANGELOG.md
--rw-r--r--   0 belokobylskiy   (501) staff       (20)    35149 2020-10-17 10:19:29.000000 lumimqtt-1.0.8/LICENSE
--rw-r--r--   0 belokobylskiy   (501) staff       (20)       55 2020-10-17 10:19:29.000000 lumimqtt-1.0.8/MANIFEST.in
--rw-r--r--   0 belokobylskiy   (501) staff       (20)     4145 2021-01-24 12:09:37.368817 lumimqtt-1.0.8/PKG-INFO
--rw-r--r--   0 belokobylskiy   (501) staff       (20)     2613 2021-01-23 09:12:48.000000 lumimqtt-1.0.8/README.md
-drwxr-xr-x   0 belokobylskiy   (501) staff       (20)        0 2021-01-24 12:09:37.366118 lumimqtt-1.0.8/lumimqtt/
--rw-r--r--   0 belokobylskiy   (501) staff       (20)        0 2020-12-22 17:42:53.000000 lumimqtt-1.0.8/lumimqtt/__init__.py
--rw-r--r--   0 belokobylskiy   (501) staff       (20)     2988 2021-01-17 07:40:41.000000 lumimqtt-1.0.8/lumimqtt/__main__.py
--rw-r--r--   0 belokobylskiy   (501) staff       (20)       18 2021-01-24 12:08:37.000000 lumimqtt-1.0.8/lumimqtt/__version__.py
--rw-r--r--   0 belokobylskiy   (501) staff       (20)    18484 2021-01-24 12:08:28.000000 lumimqtt-1.0.8/lumimqtt/lumimqtt.py
-drwxr-xr-x   0 belokobylskiy   (501) staff       (20)        0 2021-01-24 12:09:37.368429 lumimqtt-1.0.8/lumimqtt.egg-info/
--rw-r--r--   0 belokobylskiy   (501) staff       (20)     4145 2021-01-24 12:09:37.000000 lumimqtt-1.0.8/lumimqtt.egg-info/PKG-INFO
--rw-r--r--   0 belokobylskiy   (501) staff       (20)      351 2021-01-24 12:09:37.000000 lumimqtt-1.0.8/lumimqtt.egg-info/SOURCES.txt
--rw-r--r--   0 belokobylskiy   (501) staff       (20)        1 2021-01-24 12:09:37.000000 lumimqtt-1.0.8/lumimqtt.egg-info/dependency_links.txt
--rw-r--r--   0 belokobylskiy   (501) staff       (20)       53 2021-01-24 12:09:37.000000 lumimqtt-1.0.8/lumimqtt.egg-info/entry_points.txt
--rw-r--r--   0 belokobylskiy   (501) staff       (20)       29 2021-01-24 12:09:37.000000 lumimqtt-1.0.8/lumimqtt.egg-info/requires.txt
--rw-r--r--   0 belokobylskiy   (501) staff       (20)        9 2021-01-24 12:09:37.000000 lumimqtt-1.0.8/lumimqtt.egg-info/top_level.txt
--rw-r--r--   0 belokobylskiy   (501) staff       (20)       88 2021-01-24 12:09:37.369358 lumimqtt-1.0.8/setup.cfg
--rw-r--r--   0 belokobylskiy   (501) staff       (20)      991 2020-12-23 12:50:37.000000 lumimqtt-1.0.8/setup.py
+drwxr-xr-x   0 belokobylskiy   (501) staff       (20)        0 2021-01-28 22:17:06.938554 lumimqtt-1.0.9/
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)      197 2020-10-20 08:10:38.000000 lumimqtt-1.0.9/CHANGELOG.md
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)    35149 2020-10-17 10:19:29.000000 lumimqtt-1.0.9/LICENSE
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)       55 2020-10-17 10:19:29.000000 lumimqtt-1.0.9/MANIFEST.in
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)     4145 2021-01-28 22:17:06.939043 lumimqtt-1.0.9/PKG-INFO
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)     2613 2021-01-23 09:12:48.000000 lumimqtt-1.0.9/README.md
+drwxr-xr-x   0 belokobylskiy   (501) staff       (20)        0 2021-01-28 22:17:06.934470 lumimqtt-1.0.9/lumimqtt/
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)        0 2020-12-22 17:42:53.000000 lumimqtt-1.0.9/lumimqtt/__init__.py
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)     3372 2021-01-28 18:05:25.000000 lumimqtt-1.0.9/lumimqtt/__main__.py
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)       18 2021-01-28 22:16:24.000000 lumimqtt-1.0.9/lumimqtt/__version__.py
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)    18672 2021-01-28 18:04:18.000000 lumimqtt-1.0.9/lumimqtt/lumimqtt.py
+drwxr-xr-x   0 belokobylskiy   (501) staff       (20)        0 2021-01-28 22:17:06.938136 lumimqtt-1.0.9/lumimqtt.egg-info/
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)     4145 2021-01-28 22:17:06.000000 lumimqtt-1.0.9/lumimqtt.egg-info/PKG-INFO
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)      351 2021-01-28 22:17:06.000000 lumimqtt-1.0.9/lumimqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)        1 2021-01-28 22:17:06.000000 lumimqtt-1.0.9/lumimqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)       53 2021-01-28 22:17:06.000000 lumimqtt-1.0.9/lumimqtt.egg-info/entry_points.txt
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)       29 2021-01-28 22:17:06.000000 lumimqtt-1.0.9/lumimqtt.egg-info/requires.txt
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)        9 2021-01-28 22:17:06.000000 lumimqtt-1.0.9/lumimqtt.egg-info/top_level.txt
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)       88 2021-01-28 22:17:06.939888 lumimqtt-1.0.9/setup.cfg
+-rw-r--r--   0 belokobylskiy   (501) staff       (20)      991 2020-12-23 12:50:37.000000 lumimqtt-1.0.9/setup.py
```

### Comparing `lumimqtt-1.0.8/LICENSE` & `lumimqtt-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `lumimqtt-1.0.8/PKG-INFO` & `lumimqtt-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumimqtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Xiaomi Lumi Gateway MQTT integration
 Home-page: https://github.com/openlumi/lumimqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
 License: UNKNOWN
 Description: # MQTT agent for Xiaomi Lumi gateway
```

### Comparing `lumimqtt-1.0.8/README.md` & `lumimqtt-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `lumimqtt-1.0.8/lumimqtt/__main__.py` & `lumimqtt-1.0.9/lumimqtt/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,25 +2,29 @@
 import json
 import logging
 import os
 from uuid import getnode as get_mac
 
 from evdev import ecodes  # noqa
 
-from .lumimqtt import LumiMqtt, BinarySensor, IlluminanceSensor, Button, Light
 from .__version__ import VERSION
+from .lumimqtt import BinarySensor, Button, IlluminanceSensor, Light, LumiMqtt
 
 logger = logging.getLogger(__name__)
 
 
 illuminance_dev = '/sys/bus/iio/devices/iio:device0/in_voltage5_raw'
 button_dev = '/dev/input/event0'
-led_r = '/sys/class/backlight/lumi_r/brightness'
-led_g = '/sys/class/backlight/lumi_g/brightness'
-led_b = '/sys/class/backlight/lumi_b/brightness'
+led_r = '/sys/class/leds/red/brightness'
+led_g = '/sys/class/leds/green/brightness'
+led_b = '/sys/class/leds/blue/brightness'
+
+led_r_legacy = '/sys/class/backlight/lumi_r/brightness'
+led_g_legacy = '/sys/class/backlight/lumi_g/brightness'
+led_b_legacy = '/sys/class/backlight/lumi_b/brightness'
 
 SUBTOPIC_BTN = 'btn0'
 SUBTOPIC_ILLUMINANCE = 'illuminance'
 SUBTOPIC_LIGHT = 'light'
 
 
 def main():
@@ -42,14 +46,24 @@
         'mqtt_host': 'localhost',
         'mqtt_port': 1883,
         'sensor_threshold': 50,  # 5% of illuminance sensor
         'sensor_debounce_period': 60,  # 1 minute
         **config,
     }
 
+    if os.path.exists(led_r_legacy):
+        light = {
+            'r': led_r_legacy,
+            'g': led_g_legacy,
+            'b': led_b_legacy,
+            'pwm_max': 100,
+        }
+    else:
+        light = {'r': led_r, 'g': led_g, 'b': led_b, 'pwm_max': 255}
+
     server = LumiMqtt(
         reconnection_interval=10,
         loop=loop,
         dev_id=dev_id,
         topic_root=config['topic_root'].replace('{MAC}', dev_id),
         host=config['mqtt_host'],
         port=config['mqtt_port'],
@@ -67,24 +81,24 @@
     server.register(Button(
         device=button_dev,
         name='btn0',
         topic=SUBTOPIC_BTN,
         scancodes=[ecodes.BTN_0],
     ))
     server.register(Light(
-        device={'r': led_r, 'g': led_g, 'b': led_b},
+        device=light,
         name='light',
         topic=SUBTOPIC_LIGHT,
     ))
     if config.get('binary_sensors'):
         for sensor, sensor_options in config['binary_sensors'].items():
             sensor_config = {
                 'name': sensor,
                 'topic': sensor,
-                **sensor_options
+                **sensor_options,
             }
             if 'gpio' in sensor_config:
                 server.register(BinarySensor(**sensor_config))
             else:
                 logger.error(f'GPIO number is not set for {sensor} sensor!')
 
     try:
```

### Comparing `lumimqtt-1.0.8/lumimqtt/lumimqtt.py` & `lumimqtt-1.0.9/lumimqtt/lumimqtt.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,14 +60,15 @@
     BRIGHTNESS = True
 
     def __init__(self, device: dict, name, topic):
         super().__init__(device, name, topic)
         self.led_r = self.device['r']
         self.led_g = self.device['g']
         self.led_b = self.device['b']
+        self.pwm_max = int(self.device['pwm_max'])
         self.state = {
             'state': 'OFF',
             'brightness': 255,
             'color': {
                 'r': 255,
                 'g': 255,
                 'b': 255,
@@ -84,18 +85,19 @@
         brightness = value.get('brightness', self.state['brightness'])
 
         for c, file in [
             ('r', self.led_r),
             ('g', self.led_g),
             ('b', self.led_b),
         ]:
-            pwm_value = int((color[c] * 100 / 255) * brightness / 255)
+            pwm_value = \
+                int((color[c] * self.pwm_max / 255) * brightness / 255)
             if state.lower() == 'off':
                 pwm_value = 0
-            if not (0 <= pwm_value <= 100):
+            if not (0 <= pwm_value <= self.pwm_max):
                 pwm_value = 0
             with open(file, 'w+') as f:
                 f.write(str(pwm_value))
                 f.write('\n')
 
         self.state = {
             'state': state,
@@ -183,15 +185,18 @@
 
         self._sensor_retain = sensor_retain
         self._sensor_threshold = sensor_threshold
         self._sensor_debounce_period = sensor_debounce_period
 
         self._reconnection_interval = reconnection_interval
         self._loop = loop or aio.get_event_loop()
-        self._client = aio_mqtt.Client(loop=self._loop)
+        self._client = aio_mqtt.Client(
+            loop=self._loop,
+            client_id_prefix='lumimqtt_',
+        )
         self._tasks = []
 
         self.sensors: ty.List[Sensor] = []
         self.lights: ty.List[Light] = []
         self.buttons: ty.List[Button] = []
 
         self._debounce_sensors: ty.Dict[Sensor, DebounceSensor] = {}
@@ -483,18 +488,18 @@
         while True:
             try:
                 connect_result = await self._client.connect(
                     host=self._mqtt_host,
                     port=self._mqtt_port,
                     username=self._mqtt_user,
                     password=self._mqtt_password,
-                    client_id=self.dev_id,
+                    client_id=f'lumimqtt_{self.dev_id}',
                     will_message=self._will_message,
                 )
-                logger.info("Connected")
+                logger.info(f"Connected to {self._mqtt_host}")
 
                 await self._client.publish(
                     aio_mqtt.PublishableMessage(
                         topic_name=self._topic_lwt,
                         payload='online',
                         qos=aio_mqtt.QOSLevel.QOS_1,
                         retain=True,
```

### Comparing `lumimqtt-1.0.8/lumimqtt.egg-info/PKG-INFO` & `lumimqtt-1.0.9/lumimqtt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumimqtt
-Version: 1.0.8
+Version: 1.0.9
 Summary: Xiaomi Lumi Gateway MQTT integration
 Home-page: https://github.com/openlumi/lumimqtt/
 Author: Ivan Belokobylskiy
 Author-email: belokobylskij@gmail.com
 License: UNKNOWN
 Description: # MQTT agent for Xiaomi Lumi gateway
```

### Comparing `lumimqtt-1.0.8/setup.py` & `lumimqtt-1.0.9/setup.py`

 * *Files identical despite different names*

