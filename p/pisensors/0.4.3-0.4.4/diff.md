# Comparing `tmp/pisensors-0.4.3.tar.gz` & `tmp/pisensors-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pisensors-0.4.3.tar", last modified: Tue Jun  6 13:15:56 2023, max compression
+gzip compressed data, was "pisensors-0.4.4.tar", last modified: Thu Jun  8 18:23:26 2023, max compression
```

## Comparing `pisensors-0.4.3.tar` & `pisensors-0.4.4.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:15:56.068860 pisensors-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 13:15:56.068860 pisensors-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-06 13:15:41.000000 pisensors-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:15:56.064860 pisensors-0.4.3/pisensors/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-06 13:15:41.000000 pisensors-0.4.3/pisensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-06 13:15:41.000000 pisensors-0.4.3/pisensors/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-06-06 13:15:41.000000 pisensors-0.4.3/pisensors/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 13:15:56.068860 pisensors-0.4.3/pisensors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-06 13:15:56.000000 pisensors-0.4.3/pisensors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-06 13:15:55.000000 pisensors-0.4.3/pisensors.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-06 13:15:56.068860 pisensors-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-06 13:15:41.000000 pisensors-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:26.473185 pisensors-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-08 18:23:26.473185 pisensors-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-08 18:23:16.000000 pisensors-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:26.469185 pisensors-0.4.4/pisensors/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2527 2023-06-08 18:23:16.000000 pisensors-0.4.4/pisensors/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:23:26.473185 pisensors-0.4.4/pisensors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:23:26.000000 pisensors-0.4.4/pisensors.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:23:26.473185 pisensors-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-06-08 18:23:16.000000 pisensors-0.4.4/setup.py
```

### Comparing `pisensors-0.4.3/PKG-INFO` & `pisensors-0.4.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.3
+Version: 0.4.4
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.3/pisensors/sensors.py` & `pisensors-0.4.4/pisensors/sensors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 """ Read DHT22 sensors """
 import os
 from pathlib import Path
+import logging
+
 from influxdb_wrapper import influxdb_factory
-from log_mgr import Logger
 from config_yml import Config
 
 
 class Sensors():
     """Read inputs from DHT22 sensors (temperature & humidity) and write it to influx database"""
 
     def __init__(self, template_config_path: str = None, dry_run: bool = False):
-        self.logger = Logger(self.get_class_name(), 'sensors')
+        self.logger = logging.getLogger()
 
         if dry_run:
             dry_run_abs_path = ""
         else:
             dry_run_abs_path = None
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
-        self.config = Config(package_name=self.get_class_name(),
+        self.config = Config(package_name=self.class_name(),
                              template_path=template_config_path,
                              config_file_name="config.yml",
                              dry_run=True,
                              dry_run_abs_path=dry_run_abs_path)
 
         influx_conn_type = self.config['influxdbconn'].get('type', 'influx')
         self.conn = influxdb_factory(influx_conn_type)
         self.conn.open_conn(self.config['influxdbconn'])
 
     @classmethod
-    def get_class_name(cls):
+    def class_name(cls):
         """ Class name """
         return "sensors"
 
     def sensor_read(self):
         """
         Read sensors information
         """
@@ -50,29 +51,25 @@
             have_readings = True
         except (ModuleNotFoundError, NameError):
             self.logger.warning("No adafruit supported: returning default values.")
             humidity = 50
             temp_c = 25
             have_readings = True
         except RuntimeError as ex:
-            self.logger.error(f"Error reading sensor DHT22: {ex}")
+            self.logger.error("Error reading sensor DHT22: %s", ex)
 
         if have_readings:
             try:
                 points = [
                     {
                         "tags": {"sensorid": self.config["id"]},
                         "fields": {"temp": float(temp_c), "humidity": float(humidity)},
                     }
                 ]
                 self.conn.insert("DHT22", points)
 
-                self.logger.info(f"Temp: {temp_c} | Humid: {humidity}")
+                self.logger.info("Temp: %s | Humid: %s", temp_c, humidity)
 
             except RuntimeError as ex:
-                self.logger.error(f"RuntimeError: {ex}")
-                self.logger.error(f"influxDB conn={self.config['influxdbconn']}")
-
+                self.logger.error("RuntimeError: %s", ex)
+                self.logger.error("influxDB conn = %s", self.config['influxdbconn'])
 
-if __name__ == "__main__":
-    sensors_instance = Sensors()
-    sensors_instance.sensor_read()
```

### Comparing `pisensors-0.4.3/pisensors.egg-info/PKG-INFO` & `pisensors-0.4.4/pisensors.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pisensors
-Version: 0.4.3
+Version: 0.4.4
 Summary: Raspberry Pi Sensors script for Temperature & Humidity
 Home-page: https://github.com/Phornee/pisensors
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # pisensors
         Raspberry Pi Sensors script for Temperature & Humidity.
```

### Comparing `pisensors-0.4.3/setup.py` & `pisensors-0.4.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pisensors",
-    version="0.4.3",
+    version="0.4.4",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Raspberry Pi Sensors script for Temperature & Humidity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/pisensors",
     packages=setuptools.find_packages(),
@@ -21,13 +21,13 @@
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX :: Linux",
         "Topic :: Home Automation"
     ],
     install_requires=[
         'config_yml>=0.3.1',
-        'log_mgr>=0.0.2',
+        'log_mgr>=0.1.1',
         'influxdb_wrapper>=0.0.5',
         'adafruit-circuitpython-dht>=3.5.1'
     ],
     python_requires='>=3.6',
 )
```

