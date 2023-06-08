# Comparing `tmp/sbc_gpio-1.0.1.tar.gz` & `tmp/sbc_gpio-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbc_gpio-1.0.1.tar", last modified: Thu Jun  8 03:32:07 2023, max compression
+gzip compressed data, was "sbc_gpio-1.0.2.tar", last modified: Thu Jun  8 06:00:47 2023, max compression
```

## Comparing `sbc_gpio-1.0.1.tar` & `sbc_gpio-1.0.2.tar`

### file list

```diff
@@ -1,40 +1,41 @@
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1095 2023-05-01 17:06:12.000000 sbc_gpio-1.0.1/LICENSE
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      690 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      969 2023-06-08 03:31:55.000000 sbc_gpio-1.0.1/pyproject.toml
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/setup.cfg
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.310818 sbc_gpio-1.0.1/src/
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.314151 sbc_gpio-1.0.1/src/sbc_gpio/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       61 2023-05-01 16:10:15.000000 sbc_gpio-1.0.1/src/sbc_gpio/DIR.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      105 2023-05-01 16:10:24.000000 sbc_gpio-1.0.1/src/sbc_gpio/EVENT.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       77 2023-05-01 16:10:30.000000 sbc_gpio-1.0.1/src/sbc_gpio/PULL.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    22714 2023-06-08 03:24:26.000000 sbc_gpio-1.0.1/src/sbc_gpio/__init__.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    11470 2023-05-01 06:08:01.000000 sbc_gpio-1.0.1/src/sbc_gpio/__main__.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6497 2023-05-01 17:05:09.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/_test_base.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3843 2023-04-24 05:33:29.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/bmx_spi.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2390 2023-04-24 05:41:03.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/button_gpiod.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4556 2023-04-21 05:07:35.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/dht_spi.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3910 2023-04-21 05:05:08.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/i2c_display.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    15093 2023-05-11 06:04:40.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/ir.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3381 2023-04-21 05:27:04.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/led_gpiod.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     7952 2023-04-30 05:51:05.000000 sbc_gpio-1.0.1/src/sbc_gpio/device_tests/uart.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4514 2023-06-08 03:25:52.000000 sbc_gpio-1.0.1/src/sbc_gpio/dynamic_dts.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2759 2023-06-06 02:23:36.000000 sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/_generic_gpio.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6439 2023-05-11 06:05:12.000000 sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/gpiod.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4391 2023-05-11 06:05:12.000000 sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/rpi_gpio.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/src/sbc_gpio/platforms/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1589 2023-06-06 21:44:28.000000 sbc_gpio-1.0.1/src/sbc_gpio/platforms/_generic.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      810 2023-06-06 02:32:08.000000 sbc_gpio-1.0.1/src/sbc_gpio/platforms/pi4b.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     5251 2023-06-08 03:23:57.000000 sbc_gpio-1.0.1/src/sbc_gpio/platforms/rock5b.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/src/sbc_gpio/tests/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     9523 2023-05-11 06:05:12.000000 sbc_gpio-1.0.1/src/sbc_gpio/tests/devtester_test.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      230 2023-06-06 21:23:52.000000 sbc_gpio-1.0.1/src/sbc_gpio/tests/quick.py
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2212 2023-06-06 21:00:20.000000 sbc_gpio-1.0.1/src/sbc_gpio/tests/sbc_test.py
-drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 03:32:07.317484 sbc_gpio-1.0.1/src/sbc_gpio.egg-info/
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      690 2023-06-08 03:32:07.000000 sbc_gpio-1.0.1/src/sbc_gpio.egg-info/PKG-INFO
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      950 2023-06-08 03:32:07.000000 sbc_gpio-1.0.1/src/sbc_gpio.egg-info/SOURCES.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-06-08 03:32:07.000000 sbc_gpio-1.0.1/src/sbc_gpio.egg-info/dependency_links.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       71 2023-06-08 03:32:07.000000 sbc_gpio-1.0.1/src/sbc_gpio.egg-info/entry_points.txt
--rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        9 2023-06-08 03:32:07.000000 sbc_gpio-1.0.1/src/sbc_gpio.egg-info/top_level.txt
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1095 2023-05-01 17:06:12.000000 sbc_gpio-1.0.2/LICENSE
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      690 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      984 2023-06-08 05:42:09.000000 sbc_gpio-1.0.2/pyproject.toml
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       38 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/setup.cfg
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.010483 sbc_gpio-1.0.2/src/
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       62 2023-06-08 03:34:57.000000 sbc_gpio-1.0.2/src/sbc_gpio/DIR.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      105 2023-05-01 16:10:24.000000 sbc_gpio-1.0.2/src/sbc_gpio/EVENT.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       77 2023-05-01 16:10:30.000000 sbc_gpio-1.0.2/src/sbc_gpio/PULL.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    22859 2023-06-08 03:56:52.000000 sbc_gpio-1.0.2/src/sbc_gpio/__init__.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    11583 2023-06-08 03:59:36.000000 sbc_gpio-1.0.2/src/sbc_gpio/__main__.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6497 2023-05-01 17:05:09.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/_test_base.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3843 2023-04-24 05:33:29.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/bmx_spi.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2390 2023-04-24 05:41:03.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/button_gpiod.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4556 2023-04-21 05:07:35.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/dht_spi.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3910 2023-04-21 05:05:08.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/i2c_display.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)    15093 2023-05-11 06:04:40.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/ir.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     3381 2023-04-21 05:27:04.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/led_gpiod.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     7952 2023-04-30 05:51:05.000000 sbc_gpio-1.0.2/src/sbc_gpio/device_tests/uart.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6449 2023-06-08 05:39:56.000000 sbc_gpio-1.0.2/src/sbc_gpio/dynamic_dts.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     2759 2023-06-06 02:23:36.000000 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/_generic_gpio.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     6439 2023-05-11 06:05:12.000000 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/gpiod.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     4391 2023-05-11 06:05:12.000000 sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/rpi_gpio.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/src/sbc_gpio/platforms/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1589 2023-06-08 05:46:58.000000 sbc_gpio-1.0.2/src/sbc_gpio/platforms/_generic.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1355 2023-06-08 03:52:31.000000 sbc_gpio-1.0.2/src/sbc_gpio/platforms/pi4b.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     5453 2023-06-08 03:49:47.000000 sbc_gpio-1.0.2/src/sbc_gpio/platforms/rock5b.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      609 2023-06-08 05:41:51.000000 sbc_gpio-1.0.2/src/sbc_gpio/scripts.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.017150 sbc_gpio-1.0.2/src/sbc_gpio/tests/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     9523 2023-05-11 06:05:12.000000 sbc_gpio-1.0.2/src/sbc_gpio/tests/devtester_test.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)     1861 2023-06-08 04:00:27.000000 sbc_gpio-1.0.2/src/sbc_gpio/tests/sbc_test.py
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      230 2023-06-06 21:23:52.000000 sbc_gpio-1.0.2/src/sbc_gpio/tests/test_dynamic_overlay.py
+drwxr-xr-x   0 tdunteman (10001117) groupthomas (10003129)        0 2023-06-08 06:00:47.013816 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      690 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/PKG-INFO
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)      989 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/SOURCES.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        1 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/dependency_links.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)       86 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/entry_points.txt
+-rw-r--r--   0 tdunteman (10001117) groupthomas (10003129)        9 2023-06-08 06:00:47.000000 sbc_gpio-1.0.2/src/sbc_gpio.egg-info/top_level.txt
```

### Comparing `sbc_gpio-1.0.1/LICENSE` & `sbc_gpio-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/pyproject.toml` & `sbc_gpio-1.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "sbc_gpio"
-version = "1.0.1"
+version = "1.0.2"
 description = "Python Library for abstraction GPIO and for SBC testing"
 authors = [{name = "Thomas Dunteman", email= "git@learningtopi.com"}]
 keywords = ["sbc", "gpio"]
 readme = "README.md"
 requires-python =">=3.8"
 classifiers = [
     "Topic :: System :: Logging",
@@ -21,8 +21,8 @@
 
 [build-system]
 requires = ["setuptools>=61", "gpiod", "bmx280-spi", "dht11-spi", "Jinja2", "lirc",
             "logging-handler", "pyserial", "RPLCD", "smbus2", "spidev"]
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
-"update_dynamic_overlay.py"="sbc_gpio.dynamic_dts:run"
+"update_dynamic_overlay.py"="sbc_gpio.scripts:update_dynamic_overlay"
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/__init__.py` & `sbc_gpio-1.0.2/src/sbc_gpio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 from logging_handler import create_logger, INFO
 from . import DIR, EVENT, PULL
 from .gpio_libs._generic_gpio import GpioIn, GpioOut
 from .dynamic_dts import DynamicOverlay
 
 PLATFORM_BASE_DIR = os.path.join(os.path.dirname(__file__), 'platforms')
 
-PLATFORM_INFO = namedtuple('PLATFORM_INFO', ('model', 'description', 'gpio_valid_values', 
+PLATFORM_INFO = namedtuple('PLATFORM_INFO', ('model', 'description', 'gpio_valid_values',
                                              'dynamic_overlay_dir', 'dynamic_overlays', 'config_file',
                                              'update_extlinux_script', 'extlinux_conf', 'local'))
 
 class SBCPlatform:
     ''' Class to handle platform specific commands on SBC '''
     def __init__(self, log_level=INFO):
         self._platform = None
@@ -171,53 +171,52 @@
                 self.convert_gpio_tuple = mod.convert_gpio_tuple
             self._platform_write_dynamic_overlay = mod.write_dynamic_overlay if 'write_dynamic_overlay' in dir(mod) else None
             self._compile_dtbo = mod.compile_dtbo if 'compile_dtbo' in dir(mod) else None
             self._GpioIn_Class = mod.GpioIn
             self._GpioOut_Class = mod.GpioOut
             self._logger.info(f"{self.info_str}: Platform identified as {self._platform.model} ({self.description})")
         else:
-            raise ValueError(f"Unable to identify platform.  Supported devices are: {','.join(self.supported_platforms)}")            
+            raise ValueError(f"Unable to identify platform.  Supported devices are: {','.join(self.supported_platforms)}")
 
     def __str__(self):
         return self.model
 
-    def __del__(self):
-        self.close()
-
-    def close(self):
-        pass
-
     @property
     def model(self):
+        ''' Return the model of the device as a string '''
         if isinstance(self._platform, PLATFORM_INFO):
             return self._platform.model
         return ''
-        
+
     @property
     def description(self):
+        ''' Return a description of the platform as a string '''
         if isinstance(self._platform, PLATFORM_INFO):
             return self._platform.description
         return ''
-        
+
     @property
     def gpio_valid_values(self):
+        ''' Return a list of valid GPIO values as a list '''
         if isinstance(self._platform, PLATFORM_INFO):
             return self._platform.gpio_valid_values
         return []
-        
+
     @property
     def _local(self):
+        ''' Return the platform local settings '''
         if isinstance(self._platform, PLATFORM_INFO):
             return self._platform.local
+        return None
 
-    def convert_gpio(self, *args) -> int:
+    def convert_gpio(self, *args) -> int: # pylint: disable=E0202
         ''' function placeholder - replaced with platform specific function, otherwise returns first parameter '''
         return args[0]
-    
-    def convert_gpio_tuple(self, *args) -> tuple:
+
+    def convert_gpio_tuple(self, *args) -> tuple: # pylint: disable=E0202
         ''' function placeholder - replaced with platform specific function, otherwise returns chip 0 and the first parameter as a tuple '''
         return 0, args[0]
 
     def gpio_is_valid(self, gpio_id) -> bool:
         ''' Checks if a passed value is a valid GPIO for the platform '''
         if isinstance(gpio_id, int) and gpio_id in self.gpio_valid_values:
             return True
@@ -233,15 +232,15 @@
         elif isinstance(gpio_id, str):
             gpio_tuple = self.convert_gpio_tuple(gpio_id)
         elif isinstance(gpio_id, tuple) and len(gpio_id) == 2:
             gpio_tuple = gpio_id
         else:
             raise ValueError('"gpio_id" must be an integer for a pin, or a tuple containing the gpio chip and gpio pin (chip, pin)')
         return self._GpioOut_Class(gpio_tuple[1], gpio_tuple[0], name=name, pull=pull, log_level=log_level, initial_state=initial_state)
-    
+
     def get_gpio_in(self, gpio_id, name=None, pull=PULL.DOWN, event=EVENT.BOTH, debounce_ms=100, callback=None, log_level=INFO, start_polling=True) -> GpioIn:
         ''' Get a gpio in pin.  Gpio_id can be a string (passed to convert), an int, or a tuple (chip, pin) '''
         gpio_tuple = tuple()
         if isinstance(gpio_id, int):
             gpio_tuple = (0, gpio_id)
         elif isinstance(gpio_id, str):
             gpio_tuple = self.convert_gpio_tuple(gpio_id)
@@ -301,15 +300,15 @@
     def write_dynamic_overlays(self):
         ''' Read any dynamic overlays from the config file and write dts and dtbo files'''
         # check that dynamic DTS is supported
         if self._platform is None or not isinstance(self._platform.dynamic_overlay_dir, str) or not isinstance(self._platform.dynamic_overlays, dict) or len(self._platform.dynamic_overlays) == 0:
             self._logger.warning(f"{self.info_str}: Platform does not support dynamic overlay configuration.")
             self._logger.info(f"{self.info_str}: Dynamic overlay configuration aborted.")
             return
-        
+
         # create dynamic_overlay folder
         try:
             os.makedirs(self._platform.dynamic_overlay_dir, mode=0o755, exist_ok=True)
 
             # Delete any existing dynamic overlay files (will recreate ones that still exist in the config)
             dynamic_overlay_files = os.listdir(self._platform.dynamic_overlay_dir)
             dynamic_overlay_files = [f for f in dynamic_overlay_files if os.path.isfile(self._platform.dynamic_overlay_dir+'/'+f)]
@@ -317,15 +316,15 @@
             for file in dynamic_overlay_files:
                 self._logger.debug(f"{self.info_str}: Deleting file {file}")
                 os.remove(os.path.join(self._platform.dynamic_overlay_dir, file))
         except PermissionError:
             self._logger.error(f"{self.info_str}: Insufficient permisions to write to {self._platform.dynamic_overlay_dir}. Check permissions or run with sudo!")
             self._logger.info(f"{self.info_str}: Dynamic overlay configuration aborted.")
             return
-    
+
         # Read all dynamic overlays from the config file
         dynamic_overlays = {}
         try:
             with open(self._platform.config_file, 'r', encoding='utf-8') as input_file:
                 config_lines = input_file.readlines()
             for config_line in config_lines:
                 dynamic_dts_re = re.search(r'^dynamic_overlay=(?P<driver>[^\s,]*),*(?P<options>[^\s]*)', config_line)
@@ -358,15 +357,15 @@
             # verify that all configured dynamic overlays have all required configurations
             for key, item in dynamic_overlays.items():
                 if not item.ok:
                     self._logger.error(f"{self.info_str}: Overlay {key} is missing required parameters: {item.missing_params}")
                     for missing_param in item.missing_params:
                         self._logger.info(f"    Param {missing_param} help: {item.get_param(missing_param).param_help}")
                     continue
-            
+
                 # write the DTS file
                 if self._platform_write_dynamic_overlay is not None:
                     self._logger.info(f"{self.info_str}: Writing dynamic overlay " + os.path.join(self._platform.dynamic_overlay_dir, f"{item.name}-{item.get_param('gpio').set_value}.dts"))
                     self._platform_write_dynamic_overlay(item)
                 else:
                     self._logger.error(f"{self.info_str}: Unable to write overlay {key}.  Missing required platform function.")
 
@@ -406,12 +405,10 @@
                         for fdtoverlays_line in fdtoverlays_lines:
                             self._logger.debug(f"{self.info_str}: adding dynamic overlay to existng fdtoverlays in extlinux.conf")
                             extlinux_conf[extlinux_conf.index(fdtoverlays_line)] = extlinux_conf[extlinux_conf.index(fdtoverlays_line)].rstrip() + f" {dtbo_file}\n"
 
                     self._logger.info(f"{self.info_str}: Writing updated extlinux configuration file {self._platform.extlinux_conf}")
                     with open(self._platform.extlinux_conf, 'w', encoding='utf-8') as output_file:
                         output_file.writelines(extlinux_conf)
-        
+
         except Exception as e:
             self._logger.error(f"{self.info_str}: Error creating dynamic overlays: {e}")
-
-
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/__main__.py` & `sbc_gpio-1.0.2/src/sbc_gpio/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,32 +79,33 @@
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 SOFTWARE.
 '''
-from . import SBCPlatform
 import argparse
 import os
 import json
 import sys
 from time import sleep
 from logging_handler import create_logger, INFO, WARNING
 from sbc_gpio.device_tests.led_gpiod import DevTest_LED
 from sbc_gpio.device_tests.button_gpiod import DevTest_Button
 from sbc_gpio.device_tests.i2c_display import DevTest_I2CDisp
 from sbc_gpio.device_tests.ir import DevTest_IR
 from sbc_gpio.device_tests.dht_spi import DevTest_DHT
 from sbc_gpio.device_tests.bmx_spi import DevTest_BMX
 from sbc_gpio.device_tests.uart import DevTest_UART
+from . import SBCPlatform
 
 
 def run_test(run_secs=60, led=None, btn=None, dht=None, ir=None, dht_spi=None, dht22=False, bmx=None, bmx_spi=None, i2c=None, log_level=INFO,
              uart_dev=None, usb_dev=None):
+    ''' Run a basic set of tests on the specified devices.  All tests are run in parallel for a number of seconds.'''
     logger = create_logger(console_level=log_level, name='SBC_Tester')
 
     # loop through and start each test
     platform = SBCPlatform()
     # only run a test if passed values are not None or empty string
     tests = []
     if led is not None and led != '':
@@ -175,15 +176,15 @@
     parser.add_argument('--log-level', dest='log_level', required=False, type=str, default='INFO', help='(INFO) Specify the logging level for the console (DEBUG, INFO, WARN, CRITICAL)')
 
     args = vars(parser.parse_args())
 
     if args.get('write_config', False) and args.get('config') is None:
         sys.tracebacklimit=0
         raise ValueError('Parameter "write-config" requires parameter "config"')
-    
+
     if args.get('write_config', False):
         sample_config = {
             'led': '3A7',
             'btn': '3B6',
             'dht': '1D7',
             'dht22': True,
             'dht_spi': 0,
@@ -216,8 +217,7 @@
     print('#' * 35)
     print('SBC Model:       ', platform.model)
     print('SBC Description: ', platform.description)
     print('SBC Serial:      ', platform.serial)
     print('SPI Buses:       ', ', '.join([str(x) for x in platform.spi_buses()]))
     print('I2C Buses:       ', ', '.join([str(x) for x in platform.i2c_buses()]))
     print('#' * 35)
-
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/_test_base.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/_test_base.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/bmx_spi.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/bmx_spi.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/button_gpiod.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/button_gpiod.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/dht_spi.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/dht_spi.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/i2c_display.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/i2c_display.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/ir.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/ir.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/led_gpiod.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/led_gpiod.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/device_tests/uart.py` & `sbc_gpio-1.0.2/src/sbc_gpio/device_tests/uart.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/_generic_gpio.py` & `sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/_generic_gpio.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/gpiod.py` & `sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/gpiod.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/gpio_libs/rpi_gpio.py` & `sbc_gpio-1.0.2/src/sbc_gpio/gpio_libs/rpi_gpio.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/platforms/_generic.py` & `sbc_gpio-1.0.2/src/sbc_gpio/platforms/_generic.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,9 +34,9 @@
 
 def set_gpio_flags(*args) -> int:
     ''' Return an integer based on the flags sent.'''
     ret_value = 0
     for arg in args:
         if arg.upper() not in FLAGS.keys():
             raise ValueError(f'Value {arg} not in list of supported flags: {FLAGS}')
-        ret_value = ret_value & (FLAGS[arg.upper()].get('value', 0b0) << FLAGS[arg.upper()].get('offset', 0))
+        ret_value = ret_value | (FLAGS[arg.upper()].get('value', 0b0) << FLAGS[arg.upper()].get('offset', 0))
     return ret_value
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/platforms/rock5b.py` & `sbc_gpio-1.0.2/src/sbc_gpio/platforms/rock5b.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,21 @@
+'''
+Platform specific file for the Radxa Rock 5B.  This system uses extlinux for boot and supports
+dynamic overlays.  GPIO's are provided in the format <chip><bank><number> (i.e. "0A3", "3B3").
+'''
 import os
 import re
 from collections import namedtuple
 import jinja2
 from sbc_gpio import PLATFORM_INFO
-from sbc_gpio.dynamic_dts import DynamicOverlay, OverlayParam
+from sbc_gpio.dynamic_dts import DynamicOverlay
 from ._generic import set_gpio_flags
 
 # select the gpio library for the platform
-from sbc_gpio.gpio_libs.gpiod import GpioIn, GpioOut
+from sbc_gpio.gpio_libs.gpiod import GpioIn, GpioOut #pylint: disable=W0611,C0411
 
 MODEL_IDENTIFIER = [
     {
         'type': 'file', 'file': '/sys/firmware/devicetree/base/model', 'contents': 'Radxa ROCK 5B'
     }
 ]
 
@@ -35,15 +39,15 @@
             {
                 "name": "pull",
                 "param_type": "str",
                 "values": ["high", "low", "none"],
                 "param_help": "Set internal pull-up/pull-down or no bias [high|low|none]",
                 "default_value": "none"
             }
-        ], 
+        ],
         "template": "gpio-basic.dts"
     },
     "gpio-ir-recv": {}
 }
 
 SERIAL_NUMBER = '/sys/firmware/devicetree/base/serial-number'
 PLATFORM_LOCAL = namedtuple('PLATFORM_LOCAL', ('gpio_re_format', 'serial_path', 'gpio_prefix'))
@@ -105,9 +109,7 @@
 
     with open(os.path.join(PLATFORM_SPECIFIC.dynamic_overlay_dir, f"{overlay.name}-{overlay.get_param('gpio').set_value}.dts"), 'w', encoding='utf-8') as output_file:
         output_file.write(template.render(driver=overlay.name,
                                           gpio_number=convert_gpio(str(overlay.get_param('gpio').set_value)),
                                           gpio_chip=convert_gpio_tuple(str(overlay.get_param('gpio').set_value))[0],
                                           gpio_pin=convert_gpio_tuple(str(overlay.get_param('gpio').set_value))[1],
                                           gpio_pin_ctrl=set_gpio_flags(*gpio_flags)))
-        
-
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/tests/devtester_test.py` & `sbc_gpio-1.0.2/src/sbc_gpio/tests/devtester_test.py`

 * *Files identical despite different names*

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio/tests/sbc_test.py` & `sbc_gpio-1.0.2/src/sbc_gpio/tests/sbc_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,15 +42,7 @@
             sleep(.5)
             gpio_out.set_low()
             sleep(.5)
         self.assertGreaterEqual(gpio_in_events, 5)
         gpio_in.stop()
         del gpio_in
         del gpio_out
-
-    def dynamic_overlay(self):
-        logger.info('===================================== %s', self._testMethodName)
-        platform = sbc_gpio.SBCPlatform(DEBUG)
-        logger.info(f"Device Platform: {platform}")
-        self.assertTrue(isinstance(platform, sbc_gpio.SBCPlatform))
-        platform.write_dynamic_overlays()
-        print('test123')
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio.egg-info/PKG-INFO` & `sbc_gpio-1.0.2/src/sbc_gpio.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbc-gpio
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python Library for abstraction GPIO and for SBC testing
 Author-email: Thomas Dunteman <git@learningtopi.com>
 Project-URL: Homepage, https://www.learningtopi.com/python-modules-applications/sbc_gpio/
 Project-URL: Bug Tracker, https://github.com/LearningToPi/sbc_gpio/issues
 Project-URL: Source Code, https://github.com/LearningToPi/sbc_gpio
 Keywords: sbc,gpio
 Classifier: Topic :: System :: Logging
```

### Comparing `sbc_gpio-1.0.1/src/sbc_gpio.egg-info/SOURCES.txt` & `sbc_gpio-1.0.2/src/sbc_gpio.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 pyproject.toml
 src/sbc_gpio/DIR.py
 src/sbc_gpio/EVENT.py
 src/sbc_gpio/PULL.py
 src/sbc_gpio/__init__.py
 src/sbc_gpio/__main__.py
 src/sbc_gpio/dynamic_dts.py
+src/sbc_gpio/scripts.py
 src/sbc_gpio.egg-info/PKG-INFO
 src/sbc_gpio.egg-info/SOURCES.txt
 src/sbc_gpio.egg-info/dependency_links.txt
 src/sbc_gpio.egg-info/entry_points.txt
 src/sbc_gpio.egg-info/top_level.txt
 src/sbc_gpio/device_tests/_test_base.py
 src/sbc_gpio/device_tests/bmx_spi.py
@@ -22,9 +23,9 @@
 src/sbc_gpio/gpio_libs/_generic_gpio.py
 src/sbc_gpio/gpio_libs/gpiod.py
 src/sbc_gpio/gpio_libs/rpi_gpio.py
 src/sbc_gpio/platforms/_generic.py
 src/sbc_gpio/platforms/pi4b.py
 src/sbc_gpio/platforms/rock5b.py
 src/sbc_gpio/tests/devtester_test.py
-src/sbc_gpio/tests/quick.py
-src/sbc_gpio/tests/sbc_test.py
+src/sbc_gpio/tests/sbc_test.py
+src/sbc_gpio/tests/test_dynamic_overlay.py
```

