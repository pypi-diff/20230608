# Comparing `tmp/dl_myo-0.1.0.tar.gz` & `tmp/dl_myo-0.1.1.tar.gz`

## Comparing `dl_myo-0.1.0.tar` & `dl_myo-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 dl_myo-0.1.0/.github/workflows/build.yml
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 dl_myo-0.1.0/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0     3175 2020-02-02 00:00:00.000000 dl_myo-0.1.0/examples/driver.py
--rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 dl_myo-0.1.0/myo/__init__.py
--rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dl_myo-0.1.0/myo/commands.py
--rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 dl_myo-0.1.0/myo/device.py
--rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dl_myo-0.1.0/myo/handle.py
--rw-r--r--   0        0        0     5913 2020-02-02 00:00:00.000000 dl_myo-0.1.0/myo/types.py
--rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dl_myo-0.1.0/.gitignore
--rw-r--r--   0        0        0    35131 2020-02-02 00:00:00.000000 dl_myo-0.1.0/LICENSE
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 dl_myo-0.1.0/README.md
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 dl_myo-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1964 2020-02-02 00:00:00.000000 dl_myo-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      440 2020-02-02 00:00:00.000000 dl_myo-0.1.1/Dockerfile
+-rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 dl_myo-0.1.1/docker-compose.yml
+-rw-r--r--   0        0        0     1433 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.github/workflows/build.yml
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0     1559 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.github/workflows/release-package.yml
+-rw-r--r--   0        0        0     3201 2020-02-02 00:00:00.000000 dl_myo-0.1.1/examples/sample.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 dl_myo-0.1.1/examples/ws_client.py
+-rw-r--r--   0        0        0     5494 2020-02-02 00:00:00.000000 dl_myo-0.1.1/examples/ws_server.py
+-rw-r--r--   0        0        0      455 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/__init__.py
+-rw-r--r--   0        0        0     3141 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/commands.py
+-rw-r--r--   0        0        0     6772 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/device.py
+-rw-r--r--   0        0        0     5519 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/handle.py
+-rw-r--r--   0        0        0     5967 2020-02-02 00:00:00.000000 dl_myo-0.1.1/myo/types.py
+-rw-r--r--   0        0        0     2741 2020-02-02 00:00:00.000000 dl_myo-0.1.1/.gitignore
+-rw-r--r--   0        0        0    35131 2020-02-02 00:00:00.000000 dl_myo-0.1.1/LICENSE
+-rw-r--r--   0        0        0     2249 2020-02-02 00:00:00.000000 dl_myo-0.1.1/README.md
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 dl_myo-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3080 2020-02-02 00:00:00.000000 dl_myo-0.1.1/PKG-INFO
```

### Comparing `dl_myo-0.1.0/.github/workflows/build.yml` & `dl_myo-0.1.1/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/.github/workflows/python-publish.yml` & `dl_myo-0.1.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/examples/driver.py` & `dl_myo-0.1.1/examples/sample.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+
 import argparse
 import asyncio
 import logging
 
 from bleak import BleakClient
 from bleak.backends.characteristic import BleakGATTCharacteristic
 
@@ -49,17 +52,15 @@
         await client.start_notify(Handle.EMG2_DATA.value, callback)  # pyright: ignore
         await client.start_notify(Handle.EMG3_DATA.value, callback)  # pyright: ignore
         await client.start_notify(Handle.IMU_DATA.value, callback)  # pyright: ignore
 
         await m.vibrate(client, VibrationType.MEDIUM)
 
         # enable emg and imu
-        await m.set_mode(
-            client, EMGMode.SEND_EMG, IMUMode.SEND_ALL, ClassifierMode.DISABLED
-        )
+        await m.set_mode(client, EMGMode.SEND_EMG, IMUMode.SEND_ALL, ClassifierMode.DISABLED)
 
         logging.info("sleep 1")
         await asyncio.sleep(0.5)
 
         # disable emg and imu
         await m.set_mode(client, EMGMode.NONE, IMUMode.NONE, ClassifierMode.DISABLED)
```

### Comparing `dl_myo-0.1.0/myo/commands.py` & `dl_myo-0.1.1/myo/commands.py`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/myo/device.py` & `dl_myo-0.1.1/myo/device.py`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/myo/handle.py` & `dl_myo-0.1.1/myo/handle.py`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/myo/types.py` & `dl_myo-0.1.1/myo/types.py`

 * *Files 5% similar despite different names*

```diff
@@ -68,15 +68,18 @@
         self.sample1 = u[:8]
         self.sample2 = u[8:]
 
     def __str__(self):
         return str(self.sample1 + self.sample2)
 
     def json(self):
-        return json.dumps({"sample1": self.sample1, "sample2": self.sample2})
+        return json.dumps(self.to_dict())
+
+    def to_dict(self):
+        return {"sample1": self.sample1, "sample2": self.sample2}
 
 
 # -> myohw_emg_mode_t
 class EMGMode(aenum.Enum):
     NONE = 0x00
     SEND_EMG = 0x02
     SEND_RAW = 0x03
```

### Comparing `dl_myo-0.1.0/.gitignore` & `dl_myo-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/LICENSE` & `dl_myo-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dl_myo-0.1.0/pyproject.toml` & `dl_myo-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "dl-myo"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
   { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
 ]
 maintainers = [
   { name="Iori Mizutani", email="iori.mizutani@gmail.com" },
 ]
 description = "A replacement middleware to MyoConnect for Myo Armband"
```

### Comparing `dl_myo-0.1.0/PKG-INFO` & `dl_myo-0.1.1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dl-myo
-Version: 0.1.0
+Version: 0.1.1
 Summary: A replacement middleware to MyoConnect for Myo Armband
 Project-URL: Homepage, https://github.com/iomz/dl-myo
 Project-URL: Bug Tracker, https://github.com/iomz/dl-myo/issues
 Author-email: Iori Mizutani <iori.mizutani@gmail.com>
 Maintainer-email: Iori Mizutani <iori.mizutani@gmail.com>
 License-File: LICENSE
 Classifier: Framework :: AsyncIO
@@ -17,33 +17,60 @@
 Requires-Python: >=3.11
 Requires-Dist: aenum
 Requires-Dist: bleak
 Description-Content-Type: text/markdown
 
 # dl-myo (Dongle-less Myo)
 
-[![PyPI Version](https://badge.fury.io/py/dl-myo.svg)](https://badge.fury.io/py/dl-myo)
 [![Build Status](https://github.com/iomz/dl-myo/workflows/Build/badge.svg)](https://github.com/iomz/dl-myo/actions?query=workflow%3ABuild)
+[![Release Package](https://github.com/iomz/dl-myo/actions/workflows/release-package.yml/badge.svg)](https://github.com/iomz/dl-myo/actions/workflows/release-package.yml)
+[![Image Size](https://ghcr-badge.egpl.dev/iomz/dl-myo/size?label=Image%20Size)](https://github.com/iomz/dl-myo/pkgs/container/dl-myo)
+[![PyPI Version](https://badge.fury.io/py/dl-myo.svg)](https://badge.fury.io/py/dl-myo)
 
 dl-myo is a replacement to MyoConnect for Myo Armband without an official Myo dongle.
 
 If you are fed up with the dongle and still need to use Myo anyway this is the right stuff to grab.
 
-This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91] and enhanced by [@MyrikLD]) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
+This project is a reimplementation of [Dongleless-myo](https://github.com/iomz/Dongleless-myo) (originally created by [@mamo91](https://github.com/mamo91) and enhanced by [@MyrikLD](https://github.com/MyrikLD)) using [Bleak](https://github.com/hbldh/bleak) instead of [bluepy](https://github.com/IanHarvey/bluepy), and therefore supports asyncio on multiple platforms.
+
+The GATT service naming convention reflects the official BLE specification for Myo (i.e., [myohw.h](https://github.com/iomz/myo-bluetooth/blob/master/myohw.h)); however, some services and characteristics differ for a uniform naming.
+
+See [`myo/handle.py`](https://github.com/iomz/dl-myo/blob/main/myo/handle.py) for more detail.
 
 ## Platform Support
 
-|       Linux        |    Raspberry Pi    |       macOS        |      Windows       |
-| :----------------: | :----------------: | :----------------: | :----------------: |
-| :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: | :heavy_check_mark: |
+| Linux | Raspberry Pi | macOS | Windows |
+| :---: | :----------: | :---: | :-----: |
+|  ✅   |      ✅      |  ✅   |   ✅    |
 
 ## Install
 
 ```bash
 pip install dl-myo
 ```
 
 ## Example
 
+The script scans a Myo device, connect, set LED colors, vibrates, collect EMG/IMU data for a moment, and then read the avaialable services/characteristics from the device.
+
+Any Myo Armband should have the service UUID `d5060001-a904-deb9-4748-2c7f4a124842`.
+
 ```bash
 python examples/sample.py
 ```
+
+Otherwise, you can also bind to a specific MAC address. For example,
+
+```bash
+python examples/sample.py --mac D2:3B:85:94:32:8E
+```
+
+### Try the example with Docker
+
+```bash
+docker compose pull
+docker compose run --rm dl-myo
+```
+
+## Author
+
+[@iomz](https://github.com/iomz) (Iori Mizutani)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

