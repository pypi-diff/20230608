# Comparing `tmp/ariston-0.13.1.tar.gz` & `tmp/ariston-0.13.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ariston-0.13.1.tar", last modified: Fri Apr 14 17:56:55 2023, max compression
+gzip compressed data, was "ariston-0.13.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ariston-0.13.1.tar` & `ariston-0.13.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1063 2023-04-14 17:56:45.872999 ariston-0.13.1/LICENSE
--rw-r--r--   0        0        0     3495 2023-04-14 17:56:45.872999 ariston-0.13.1/README.md
--rw-r--r--   0        0        0     5933 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/__init__.py
--rw-r--r--   0        0        0    23504 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/ariston_api.py
--rw-r--r--   0        0        0    13991 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/const.py
--rw-r--r--   0        0        0    12513 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/device.py
--rw-r--r--   0        0        0     3766 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/evo_device.py
--rw-r--r--   0        0        0     1090 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/evo_lydos_device.py
--rw-r--r--   0        0        0    30516 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/galevo_device.py
--rw-r--r--   0        0        0     1487 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/lux_device.py
--rw-r--r--   0        0        0     3172 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/lydos_hybrid_device.py
--rw-r--r--   0        0        0     9836 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/nuos_split_device.py
--rw-r--r--   0        0        0     7118 2023-04-14 17:56:45.872999 ariston-0.13.1/ariston/velis_device.py
--rw-r--r--   0        0        0      361 2023-04-14 17:56:45.872999 ariston-0.13.1/pyproject.toml
--rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.1/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-06-08 10:17:11.741925 ariston-0.13.2/LICENSE
+-rw-r--r--   0        0        0     3495 2023-06-08 10:17:11.741925 ariston-0.13.2/README.md
+-rw-r--r--   0        0        0     5933 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/__init__.py
+-rw-r--r--   0        0        0    23552 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/ariston_api.py
+-rw-r--r--   0        0        0    13991 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/const.py
+-rw-r--r--   0        0        0    12513 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/device.py
+-rw-r--r--   0        0        0     3766 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/evo_device.py
+-rw-r--r--   0        0        0     1090 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/evo_lydos_device.py
+-rw-r--r--   0        0        0    30516 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/galevo_device.py
+-rw-r--r--   0        0        0     1487 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/lux_device.py
+-rw-r--r--   0        0        0     3172 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/lydos_hybrid_device.py
+-rw-r--r--   0        0        0     9836 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/nuos_split_device.py
+-rw-r--r--   0        0        0     7118 2023-06-08 10:17:11.741925 ariston-0.13.2/ariston/velis_device.py
+-rw-r--r--   0        0        0      361 2023-06-08 10:17:11.741925 ariston-0.13.2/pyproject.toml
+-rw-r--r--   0        0        0     3732 1970-01-01 00:00:00.000000 ariston-0.13.2/PKG-INFO
```

### Comparing `ariston-0.13.1/LICENSE` & `ariston-0.13.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/README.md` & `ariston-0.13.2/README.md`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/__init__.py` & `ariston-0.13.2/ariston/__init__.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/ariston_api.py` & `ariston-0.13.2/ariston/ariston_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,25 +173,25 @@
         )
         if properties is not None:
             return properties
         return dict()
 
     def get_velis_plant_data(self, plant_data: PlantData, gw_id: str) -> dict[str, Any]:
         """Get Velis properties"""
-        data = self._get(f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}")
+        data = self._get(f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}")
         if data is not None:
             return data
         return dict()
 
     def get_velis_plant_settings(
         self, plant_data: PlantData, gw_id: str
     ) -> dict[str, Any]:
         """Get Velis settings"""
         settings = self._get(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}/plantSettings"
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}/plantSettings"
         )
         if settings is not None:
             return settings
         return dict()
 
     def set_property(
         self,
@@ -289,29 +289,29 @@
             f"{ARISTON_API_URL}{ARISTON_VELIS}/{PlantData.Med}/{gw_id}/switchEco",
             eco_mode,
         )
 
     def set_velis_power(self, plant_data: PlantData, gw_id: str, power: bool) -> None:
         """Set Velis power"""
         self._post(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}/switch",
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}/switch",
             power,
         )
 
     def set_velis_plant_setting(
         self,
         plant_data: PlantData,
         gw_id: str,
         setting: str,
         value: float,
         old_value: float,
     ) -> None:
         """Set Velis plant setting"""
         self._post(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}/plantSettings",
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}/plantSettings",
             {setting: {"new": value, "old": old_value}},
         )
 
     def get_thermostat_time_progs(
         self, gw_id: str, zone: int, umsys: str
     ) -> dict[str, Any]:
         """Get thermostat time programs"""
@@ -496,26 +496,26 @@
         return dict()
 
     async def async_get_velis_plant_data(
         self, plant_data: PlantData, gw_id: str
     ) -> dict[str, Any]:
         """Async get Velis properties"""
         med_plant_data = await self._async_get(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}"
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}"
         )
         if med_plant_data is not None:
             return med_plant_data
         return dict()
 
     async def async_get_velis_plant_settings(
         self, plant_data: PlantData, gw_id: str
     ) -> dict[str, Any]:
         """Async get Velis settings"""
         med_plant_settings = await self._async_get(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}/plantSettings"
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}/plantSettings"
         )
         if med_plant_settings is not None:
             return med_plant_settings
         return dict()
 
     async def async_set_property(
         self,
@@ -619,29 +619,29 @@
         )
 
     async def async_set_velis_power(
         self, plant_data: PlantData, gw_id: str, power: bool
     ) -> None:
         """Async set Velis power"""
         await self._async_post(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}/switch",
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}/switch",
             power,
         )
 
     async def async_set_velis_plant_setting(
         self,
         plant_data: PlantData,
         gw_id: str,
         setting: str,
         value: float,
         old_value: float,
     ) -> None:
         """Async set Velis Evo plant setting"""
         await self._async_post(
-            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data}/{gw_id}/plantSettings",
+            f"{ARISTON_API_URL}{ARISTON_VELIS}/{plant_data.value}/{gw_id}/plantSettings",
             {setting: {"new": value, "old": old_value}},
         )
 
     async def async_get_thermostat_time_progs(
         self, gw_id: str, zone: int, umsys: str
     ) -> Optional[dict[str, Any]]:
         """Async get thermostat time programs"""
```

### Comparing `ariston-0.13.1/ariston/const.py` & `ariston-0.13.2/ariston/const.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/device.py` & `ariston-0.13.2/ariston/device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/evo_device.py` & `ariston-0.13.2/ariston/evo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/evo_lydos_device.py` & `ariston-0.13.2/ariston/evo_lydos_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/galevo_device.py` & `ariston-0.13.2/ariston/galevo_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/lux_device.py` & `ariston-0.13.2/ariston/lux_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/lydos_hybrid_device.py` & `ariston-0.13.2/ariston/lydos_hybrid_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/nuos_split_device.py` & `ariston-0.13.2/ariston/nuos_split_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/ariston/velis_device.py` & `ariston-0.13.2/ariston/velis_device.py`

 * *Files identical despite different names*

### Comparing `ariston-0.13.1/PKG-INFO` & `ariston-0.13.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ariston
-Version: 0.13.1
+Version: 0.13.2
 Summary: Ariston module
 Author-email: Tamás Füstös <fustom@gmail.com>
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: aiohttp
 Requires-Dist: requests
```

