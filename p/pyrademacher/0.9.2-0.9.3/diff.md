# Comparing `tmp/pyrademacher-0.9.2.tar.gz` & `tmp/pyrademacher-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrademacher-0.9.2.tar", last modified: Sun Feb 19 21:51:31 2023, max compression
+gzip compressed data, was "pyrademacher-0.9.3.tar", last modified: Wed Jun  7 23:48:28 2023, max compression
```

## Comparing `pyrademacher-0.9.2.tar` & `pyrademacher-0.9.3.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:51:31.076869 pyrademacher-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-02-19 21:51:31.076869 pyrademacher-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:51:31.072868 pyrademacher-0.9.2/homepilot/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/actuator.py
--rw-r--r--   0 runner    (1001) docker     (123)    14640 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3827 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/homepilot/thermostat.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:51:31.076869 pyrademacher-0.9.2/pyrademacher.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-02-19 21:51:31.000000 pyrademacher-0.9.2/pyrademacher.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-02-19 21:51:31.000000 pyrademacher-0.9.2/pyrademacher.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-19 21:51:31.000000 pyrademacher-0.9.2/pyrademacher.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-19 21:51:31.000000 pyrademacher-0.9.2/pyrademacher.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-02-19 21:51:31.000000 pyrademacher-0.9.2/pyrademacher.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-19 21:51:31.076869 pyrademacher-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-19 21:51:31.076869 pyrademacher-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_cover.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_hub.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-02-19 21:51:20.000000 pyrademacher-0.9.2/tests/test_thermostat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:48:28.061985 pyrademacher-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 23:48:28.061985 pyrademacher-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:48:28.057985 pyrademacher-0.9.3/homepilot/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/actuator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15019 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7834 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8540 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11620 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/homepilot/thermostat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:48:28.061985 pyrademacher-0.9.3/pyrademacher.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-06-07 23:48:28.000000 pyrademacher-0.9.3/pyrademacher.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-07 23:48:28.000000 pyrademacher-0.9.3/pyrademacher.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:48:28.000000 pyrademacher-0.9.3/pyrademacher.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-07 23:48:28.000000 pyrademacher-0.9.3/pyrademacher.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-07 23:48:28.000000 pyrademacher-0.9.3/pyrademacher.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 23:48:28.061985 pyrademacher-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1113 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:48:28.061985 pyrademacher-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13931 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_cover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_hub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3293 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-06-07 23:48:17.000000 pyrademacher-0.9.3/tests/test_thermostat.py
```

### Comparing `pyrademacher-0.9.2/LICENSE` & `pyrademacher-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/PKG-INFO` & `pyrademacher-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrademacher
-Version: 0.9.2
+Version: 0.9.3
 Summary: Control devices connected to your Rademacher Homepilot (or Start2Smart) hub
 Home-page: https://github.com/peribeir/pyrademacher
 Author: Pedro Ribeiro
 Author-email: pedroeusebio@gmail.com
 Project-URL: Bug Tracker, https://github.com/peribeir/pyrademacher/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrademacher-0.9.2/README.md` & `pyrademacher-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/actuator.py` & `pyrademacher-0.9.3/homepilot/actuator.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/api.py` & `pyrademacher-0.9.3/homepilot/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,23 @@
         async with aiohttp.ClientSession(cookie_jar=self.cookie_jar) as session:
             async with session.get(
                 f"http://{self.host}/service/system-update-image/status"
             ) as response:
                 response = await response.json()
                 return response
 
+    async def async_get_interfaces(self):
+        await self.authenticate()
+        async with aiohttp.ClientSession(cookie_jar=self.cookie_jar) as session:
+            async with session.get(
+                f"http://{self.host}service/system/networkmgr/v1/interfaces"
+            ) as response:
+                response = await response.json()
+                return response
+
     async def async_get_fw_version(self):
         await self.authenticate()
         async with aiohttp.ClientSession(cookie_jar=self.cookie_jar) as session:
             async with session.get(
                 f"http://{self.host}/service/system-update-image/version"
             ) as response:
                 response = await response.json()
```

### Comparing `pyrademacher-0.9.2/homepilot/const.py` & `pyrademacher-0.9.3/homepilot/const.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/cover.py` & `pyrademacher-0.9.3/homepilot/cover.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/device.py` & `pyrademacher-0.9.3/homepilot/device.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/hub.py` & `pyrademacher-0.9.3/homepilot/hub.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/manager.py` & `pyrademacher-0.9.3/homepilot/manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,14 +50,21 @@
             return await HomePilotActuator.async_build_from_api(api, id_type["did"])
         if id_type["type"] == "5":
             return await HomePilotThermostat.async_build_from_api(api, id_type["did"])
         if id_type["type"] == "8":
             return await HomePilotCover.async_build_from_api(api, id_type["did"])
         return None
 
+    async def get_hub_macaddress(self):
+        interfaces = await self.api.async_get_interfaces()["interfaces"]
+        for k in interfaces:
+            if interfaces[k]["enabled"] == True:
+                return interfaces[k]["address"]
+        return None
+
     async def get_hub_state(self):
         return {
             "status": await self.api.async_get_fw_status(),
             "version": await self.api.async_get_fw_version(),
             "led": await self.api.async_get_led_status(),
         }
```

### Comparing `pyrademacher-0.9.2/homepilot/sensor.py` & `pyrademacher-0.9.3/homepilot/sensor.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/switch.py` & `pyrademacher-0.9.3/homepilot/switch.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/homepilot/thermostat.py` & `pyrademacher-0.9.3/homepilot/thermostat.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/pyrademacher.egg-info/PKG-INFO` & `pyrademacher-0.9.3/pyrademacher.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrademacher
-Version: 0.9.2
+Version: 0.9.3
 Summary: Control devices connected to your Rademacher Homepilot (or Start2Smart) hub
 Home-page: https://github.com/peribeir/pyrademacher
 Author: Pedro Ribeiro
 Author-email: pedroeusebio@gmail.com
 Project-URL: Bug Tracker, https://github.com/peribeir/pyrademacher/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `pyrademacher-0.9.2/pyrademacher.egg-info/SOURCES.txt` & `pyrademacher-0.9.3/pyrademacher.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/setup.py` & `pyrademacher-0.9.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyrademacher",
-    version="0.9.2",
+    version="0.9.3",
     author="Pedro Ribeiro",
     author_email="pedroeusebio@gmail.com",
     description="Control devices connected to your Rademacher Homepilot "
     "(or Start2Smart) hub",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/peribeir/pyrademacher",
```

### Comparing `pyrademacher-0.9.2/tests/test_api.py` & `pyrademacher-0.9.3/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/tests/test_cover.py` & `pyrademacher-0.9.3/tests/test_cover.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/tests/test_hub.py` & `pyrademacher-0.9.3/tests/test_hub.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/tests/test_manager.py` & `pyrademacher-0.9.3/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/tests/test_sensor.py` & `pyrademacher-0.9.3/tests/test_sensor.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/tests/test_switch.py` & `pyrademacher-0.9.3/tests/test_switch.py`

 * *Files identical despite different names*

### Comparing `pyrademacher-0.9.2/tests/test_thermostat.py` & `pyrademacher-0.9.3/tests/test_thermostat.py`

 * *Files identical despite different names*

