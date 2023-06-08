# Comparing `tmp/sessypy-0.0.8.tar.gz` & `tmp/sessypy-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sessypy-0.0.8.tar", last modified: Sat May 13 19:08:21 2023, max compression
+gzip compressed data, was "sessypy-0.0.9.tar", last modified: Fri Jun  2 21:02:28 2023, max compression
```

## Comparing `sessypy-0.0.8.tar` & `sessypy-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:08:21.697957 sessypy-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-05-13 19:08:05.000000 sessypy-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-13 19:08:21.697957 sessypy-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-13 19:08:05.000000 sessypy-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-13 19:08:05.000000 sessypy-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-13 19:08:21.697957 sessypy-0.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:08:21.693957 sessypy-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:08:21.693957 sessypy-0.0.8/src/sessypy/
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-13 19:08:05.000000 sessypy-0.0.8/src/sessypy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-13 19:08:05.000000 sessypy-0.0.8/src/sessypy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2179 2023-05-13 19:08:05.000000 sessypy-0.0.8/src/sessypy/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-13 19:08:05.000000 sessypy-0.0.8/src/sessypy/devices.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-05-13 19:08:05.000000 sessypy-0.0.8/src/sessypy/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 19:08:21.697957 sessypy-0.0.8/src/sessypy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-13 19:08:21.000000 sessypy-0.0.8/src/sessypy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-05-13 19:08:21.000000 sessypy-0.0.8/src/sessypy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 19:08:21.000000 sessypy-0.0.8/src/sessypy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-13 19:08:21.000000 sessypy-0.0.8/src/sessypy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-13 19:08:21.000000 sessypy-0.0.8/src/sessypy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.013666 sessypy-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-02 21:02:14.000000 sessypy-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-02 21:02:28.013666 sessypy-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-06-02 21:02:14.000000 sessypy-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-06-02 21:02:14.000000 sessypy-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-02 21:02:28.013666 sessypy-0.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.005665 sessypy-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.009666 sessypy-0.0.9/src/sessypy/
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3301 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-02 21:02:14.000000 sessypy-0.0.9/src/sessypy/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 21:02:28.013666 sessypy-0.0.9/src/sessypy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-06-02 21:02:28.000000 sessypy-0.0.9/src/sessypy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 21:02:27.000000 sessypy-0.0.9/src/sessypy.egg-info/top_level.txt
```

### Comparing `sessypy-0.0.8/LICENSE` & `sessypy-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sessypy-0.0.8/PKG-INFO` & `sessypy-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `sessypy-0.0.8/src/sessypy/api.py` & `sessypy-0.0.9/src/sessypy/api.py`

 * *Files identical despite different names*

### Comparing `sessypy-0.0.8/src/sessypy/const.py` & `sessypy-0.0.9/src/sessypy/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from enum import Enum
 
 API_VERSION_1 = "api/v1"
 
 class SessyApiCommand(str, Enum):
+    NETWORK_SCAN = f"{API_VERSION_1}/network/scan"
     NETWORK_STATUS = f"{API_VERSION_1}/network/status"
     OTA_CHECK = f"{API_VERSION_1}/ota/check"
     OTA_START = f"{API_VERSION_1}/ota/start"
     OTA_STATUS = f"{API_VERSION_1}/ota/status"
     
     POWER_SETPOINT = f"{API_VERSION_1}/power/setpoint"
     POWER_STATUS = f"{API_VERSION_1}/power/status"
```

### Comparing `sessypy-0.0.8/src/sessypy/devices.py` & `sessypy-0.0.9/src/sessypy/devices.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
     
     async def check_ota(self):
         return await self.api.get(SessyApiCommand.OTA_CHECK)
     
     async def install_ota(self, target: SessyOtaTarget):
         return await self.api.post(SessyApiCommand.OTA_START, {"target": target.value})
     
+    async def get_network_scan(self):
+        return await self.api.get(SessyApiCommand.NETWORK_SCAN)
+    
     async def get_network_status(self):
         return await self.api.get(SessyApiCommand.NETWORK_STATUS)
 
     async def set_wifi_credentials(self, ssid: str, password: str):
         return await self.api.post(SessyApiCommand.WIFI_STA_CREDENTIALS, {"ssid":ssid, "pass":password})
 
     async def close(self):
```

### Comparing `sessypy-0.0.8/src/sessypy.egg-info/PKG-INFO` & `sessypy-0.0.9/src/sessypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sessypy
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python wrapper for Sessy REST API
 Home-page: https://github.com/PimDoos/sessypy
 Author: PimDoos
 License: GNU GPLv3
 Project-URL: Homepage, https://github.com/PimDoos/sessypy
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

