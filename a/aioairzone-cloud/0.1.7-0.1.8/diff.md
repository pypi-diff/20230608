# Comparing `tmp/aioairzone-cloud-0.1.7.tar.gz` & `tmp/aioairzone-cloud-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioairzone-cloud-0.1.7.tar", last modified: Wed May 31 18:00:15 2023, max compression
+gzip compressed data, was "aioairzone-cloud-0.1.8.tar", last modified: Thu Jun  8 08:02:58 2023, max compression
```

## Comparing `aioairzone-cloud-0.1.7.tar` & `aioairzone-cloud-0.1.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/
--rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.7/LICENSE
--rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.7/MANIFEST.in
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/README.md
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/aioairzone_cloud/
--rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/__init__.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/aidoo.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    18280 2023-05-31 17:41:58.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/cloudapi.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/common.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     6843 2023-05-31 17:41:58.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/const.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4293 2023-05-31 17:51:01.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/device.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/exceptions.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)    16988 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/hvac.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/installation.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/py.typed
--rw-r--r--   0 noltari   (1000) noltari   (1000)      976 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/system.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     4140 2023-05-31 17:58:06.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/webserver.py
--rw-r--r--   0 noltari   (1000) noltari   (1000)     2231 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.7/aioairzone_cloud/zone.py
-drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/not-zip-safe
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/requires.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-05-31 18:00:15.000000 aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/top_level.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-05-31 17:59:14.000000 aioairzone-cloud-0.1.7/pyproject.toml
--rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.7/requirements.txt
--rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-05-31 18:00:15.290126 aioairzone-cloud-0.1.7/setup.cfg
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-08 08:02:58.580407 aioairzone-cloud-0.1.8/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    11357 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.8/LICENSE
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       59 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.8/MANIFEST.in
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-08 08:02:58.580407 aioairzone-cloud-0.1.8/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      746 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/README.md
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-08 08:02:58.580407 aioairzone-cloud-0.1.8/aioairzone_cloud/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       33 2022-04-06 08:19:16.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/__init__.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      156 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/aidoo.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    18516 2023-06-08 07:52:33.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/cloudapi.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1527 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/common.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     6843 2023-05-31 17:41:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/const.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     4321 2023-06-08 07:47:36.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/device.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      806 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/exceptions.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)    17522 2023-06-08 07:46:59.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/hvac.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1181 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/installation.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        0 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/py.typed
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      976 2023-05-31 16:54:53.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/system.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     5101 2023-06-08 07:39:37.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/webserver.py
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     2243 2023-06-08 07:48:35.000000 aioairzone-cloud-0.1.8/aioairzone_cloud/zone.py
+drwxr-xr-x   0 noltari   (1000) noltari   (1000)        0 2023-06-08 08:02:58.580407 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1528 2023-06-08 08:02:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/PKG-INFO
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      670 2023-06-08 08:02:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/SOURCES.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-08 08:02:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/dependency_links.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        1 2023-06-08 08:02:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/not-zip-safe
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2023-06-08 08:02:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/requires.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)       17 2023-06-08 08:02:58.000000 aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/top_level.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)     1029 2023-06-08 07:59:11.000000 aioairzone-cloud-0.1.8/pyproject.toml
+-rw-r--r--   0 noltari   (1000) noltari   (1000)        8 2022-03-21 14:52:35.000000 aioairzone-cloud-0.1.8/requirements.txt
+-rw-r--r--   0 noltari   (1000) noltari   (1000)      296 2023-06-08 08:02:58.580407 aioairzone-cloud-0.1.8/setup.cfg
```

### Comparing `aioairzone-cloud-0.1.7/LICENSE` & `aioairzone-cloud-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/PKG-INFO` & `aioairzone-cloud-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.7/README.md` & `aioairzone-cloud-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/cloudapi.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/cloudapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     async def api_request(
         self, method: str, path: str, json: Any | None = None
     ) -> dict[str, Any]:
         """Airzone Cloud API request."""
         _LOGGER.debug("aiohttp request: /%s (params=%s)", path, json)
 
         headers: dict[str, str] = {}
-        if self.token:
+        if self.token is not None:
             headers[HEADER_AUTHORIZATION] = f"{HEADER_BEARER} {self.token}"
 
         try:
             resp: ClientResponse = await self.aiohttp_session.request(
                 method,
                 f"{API_URL}/{path}",
                 headers=headers,
@@ -226,15 +226,15 @@
         )
         self._api_raw_data[RAW_WEBSERVERS][ws_id] = res
 
         return res
 
     async def login(self) -> None:
         """Perform Airzone Cloud API login."""
-        if self.token:
+        if self.token is not None:
             await self.logout()
         resp = await self.api_request(
             "POST",
             f"{API_V1}/{API_AUTH_LOGIN}",
             {
                 API_EMAIL: self.options.username,
                 API_PASSWORD: self.options.password,
@@ -246,29 +246,29 @@
         self.refresh_time = datetime.now()
         self.refresh_token = resp[API_REFRESH_TOKEN]
         self.token = resp[API_TOKEN]
 
     async def logout(self) -> None:
         """Perform Airzone Cloud API logout."""
         try:
-            if self.token:
+            if self.token is not None:
                 await self.api_request(
                     "GET",
                     f"{API_V1}/{API_USER_LOGOUT}",
                 )
         except AirzoneCloudError:
             pass
         finally:
             self.refresh_time = None
             self.refresh_token = None
             self.token = None
 
     async def token_refresh(self) -> None:
         """Perform Airzone Cloud API token refresh."""
-        if self.token and self.refresh_token:
+        if self.token is not None and self.refresh_token is not None:
             refresh_token = urllib.parse.quote(self.refresh_token)
             resp = await self.api_request(
                 "GET",
                 f"{API_V1}/{API_AUTH_REFRESH_TOKEN}/{refresh_token}",
             )
             _LOGGER.debug("refresh resp: %s", resp)
             if resp.keys() < {API_TOKEN, API_REFRESH_TOKEN}:
@@ -281,39 +281,39 @@
         """Return raw Airzone Cloud API data."""
         return self._api_raw_data
 
     def data(self) -> dict[str, Any]:
         """Return Airzone Cloud data."""
         data: dict[str, Any] = {}
 
-        if len(self.aidoos):
+        if len(self.aidoos) > 0:
             aidoos: dict[str, Any] = {}
             for key, aidoo in self.aidoos.items():
                 aidoos[key] = aidoo.data()
             data[AZD_AIDOOS] = aidoos
 
-        if len(self.installations):
+        if len(self.installations) > 0:
             installations: dict[str, Any] = {}
             for key, installation in self.installations.items():
                 installations[key] = installation.data()
             data[AZD_INSTALLATIONS] = installations
 
-        if len(self.systems):
+        if len(self.systems) > 0:
             systems: dict[str, Any] = {}
             for key, system in self.systems.items():
                 systems[key] = system.data()
             data[AZD_SYSTEMS] = systems
 
-        if len(self.webservers):
+        if len(self.webservers) > 0:
             webservers: dict[str, Any] = {}
             for key, webserver in self.webservers.items():
                 webservers[key] = webserver.data()
             data[AZD_WEBSERVERS] = webservers
 
-        if len(self.zones):
+        if len(self.zones) > 0:
             zones: dict[str, Any] = {}
             for key, zone in self.zones.items():
                 zones[key] = zone.data()
             data[AZD_ZONES] = zones
 
         return data
 
@@ -349,15 +349,15 @@
 
     def select_installation(self, inst: Installation) -> None:
         """Select single Airzone Cloud installation."""
         self.installations = {
             inst.get_id(): inst,
         }
         for ws_id in inst.get_webservers():
-            if not self.get_webserver_id(ws_id):
+            if self.get_webserver_id(ws_id) is None:
                 self.webservers[ws_id] = WebServer(inst.get_id(), ws_id)
 
     def set_system_zones_data(self, system: System) -> None:
         """Set slave zones modes from master zone."""
         modes = system.get_modes()
         installation_id = system.get_installation()
         system_id = system.get_id()
@@ -389,55 +389,55 @@
 
     async def update_installation(self, inst: Installation) -> None:
         """Update Airzone Cloud installation from API."""
         installation_data = await self.api_get_installation(inst)
         for group in installation_data[API_GROUPS]:
             for device_data in group[API_DEVICES]:
                 if API_AZ_ZONE == device_data[API_TYPE]:
-                    if not self.get_zone_id(device_data[API_DEVICE_ID]):
+                    if self.get_zone_id(device_data[API_DEVICE_ID]) is None:
                         zone = Zone(inst.get_id(), device_data[API_WS_ID], device_data)
-                        if zone:
+                        if zone is not None:
                             self.zones[zone.get_id()] = zone
                 elif API_AZ_SYSTEM == device_data[API_TYPE]:
-                    if not self.get_system_id(device_data[API_DEVICE_ID]):
+                    if self.get_system_id(device_data[API_DEVICE_ID]) is None:
                         system = System(
                             inst.get_id(), device_data[API_WS_ID], device_data
                         )
-                        if system:
+                        if system is not None:
                             self.systems[system.get_id()] = system
                 elif API_AZ_AIDOO == device_data[API_TYPE]:
-                    if not self.get_aidoo_id(device_data[API_DEVICE_ID]):
+                    if self.get_aidoo_id(device_data[API_DEVICE_ID]) is None:
                         aidoo = Aidoo(
                             inst.get_id(), device_data[API_WS_ID], device_data
                         )
-                        if aidoo:
+                        if aidoo is not None:
                             self.aidoos[aidoo.get_id()] = aidoo
 
     async def update_installations(self) -> None:
         """Update Airzone Cloud installations from API."""
         installations_data = await self.api_get_installations()
         for installation_data in installations_data[API_INSTALLATIONS]:
-            if not self.get_installation_id(installation_data[API_INSTALLATION_ID]):
+            if self.get_installation_id(installation_data[API_INSTALLATION_ID]) is None:
                 installation = Installation(installation_data)
-                if installation:
+                if installation is not None:
                     self.installations[installation.get_id()] = installation
                     for ws_id in installation.get_webservers():
-                        if not self.get_webserver_id(ws_id):
+                        if self.get_webserver_id(ws_id) is None:
                             ws = WebServer(installation.get_id(), ws_id)
                             self.webservers[ws_id] = ws
 
     async def update_system(self, system: System) -> None:
         """Update Airzone Cloud System from API."""
         device_data = await self.api_get_device_status(system)
         system.update(device_data)
 
     async def update_system_id(self, sys_id: str) -> None:
         """Update Airzone Cloud System by ID."""
         system = self.get_system_id(sys_id)
-        if system:
+        if system is not None:
             await self.update_system(system)
 
     async def update_systems(self) -> None:
         """Update all Airzone Cloud Systems."""
         tasks = []
 
         for system in self.systems.values():
@@ -448,33 +448,33 @@
     async def update_webserver(self, ws: WebServer, devices: bool) -> None:
         """Update Airzone Cloud WebServer from API."""
         ws_data = await self.api_get_webserver(ws, devices)
         ws.update(ws_data)
         if devices:
             for device_data in ws_data[API_DEVICES]:
                 if API_AZ_ZONE == device_data[API_DEVICE_TYPE]:
-                    if not self.get_zone_id(device_data[API_DEVICE_ID]):
+                    if self.get_zone_id(device_data[API_DEVICE_ID]) is None:
                         zone = Zone(ws.get_installation(), ws.get_id(), device_data)
-                        if zone:
+                        if zone is not None:
                             self.zones[zone.get_id()] = zone
                 elif API_AZ_SYSTEM == device_data[API_DEVICE_TYPE]:
-                    if not self.get_system_id(device_data[API_DEVICE_ID]):
+                    if self.get_system_id(device_data[API_DEVICE_ID]) is None:
                         system = System(ws.get_installation(), ws.get_id(), device_data)
-                        if system:
+                        if system is not None:
                             self.systems[system.get_id()] = system
                 elif API_AZ_AIDOO == device_data[API_DEVICE_TYPE]:
-                    if not self.get_aidoo_id(device_data[API_DEVICE_ID]):
+                    if self.get_aidoo_id(device_data[API_DEVICE_ID]) is None:
                         aidoo = Aidoo(ws.get_installation(), ws.get_id(), device_data)
-                        if aidoo:
+                        if aidoo is not None:
                             self.aidoos[aidoo.get_id()] = aidoo
 
     async def update_webserver_id(self, ws_id: str, devices: bool) -> None:
         """Update Airzone Cloud WebServer by ID."""
         ws = self.get_webserver_id(ws_id)
-        if ws:
+        if ws is not None:
             await self.update_webserver(ws, devices)
 
     async def update_webservers(self, devices: bool) -> None:
         """Update all Airzone Cloud WebServers."""
         tasks = []
 
         for ws in self.webservers.values():
@@ -486,15 +486,15 @@
         """Update Airzone Cloud Zone from API."""
         device_data = await self.api_get_device_status(zone)
         zone.update(device_data)
 
     async def update_zone_id(self, zone_id: str) -> None:
         """Update Airzone Cloud Zone by ID."""
         zone = self.get_zone_id(zone_id)
-        if zone:
+        if zone is not None:
             await self.update_zone(zone)
 
     async def update_zones(self) -> None:
         """Update all Airzone Cloud Zones."""
         tasks = []
 
         for zone in self.zones.values():
```

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/common.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/common.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/const.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/const.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/device.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/device.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         if API_IS_CONNECTED in device_data:
             self.is_connected = bool(device_data[API_IS_CONNECTED])
         else:
             self.is_connected = True
 
     def data(self) -> dict[str, Any]:
         """Return Device data."""
-        data = {
+        data: dict[str, Any] = {
             AZD_AVAILABLE: self.get_available(),
             AZD_ID: self.get_id(),
             AZD_INSTALLATION: self.get_installation(),
             AZD_IS_CONNECTED: self.get_is_connected(),
             AZD_MODE: self.get_mode(),
             AZD_NAME: self.get_name(),
             AZD_PROBLEMS: self.get_problems(),
@@ -63,15 +63,15 @@
         }
 
         errors = self.get_errors()
         if len(errors) > 0:
             data[AZD_ERRORS] = errors
 
         modes = self.get_modes()
-        if modes:
+        if modes is not None:
             data[AZD_MODES] = modes
 
         warnings = self.get_warnings()
         if len(warnings) > 0:
             data[AZD_WARNINGS] = warnings
 
         return data
```

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/exceptions.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/hvac.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/hvac.py`

 * *Files 13% similar despite different names*

```diff
@@ -86,142 +86,145 @@
         self.temp: float | None = None
         self.temp_step: float | None = None
 
     def data(self) -> dict[str, Any]:
         """Return HVAC device data."""
         data = super().data()
 
-        data[AZD_HUMIDITY] = self.get_humidity()
         data[AZD_POWER] = self.get_power()
         data[AZD_TEMP] = self.get_temperature()
         data[AZD_TEMP_STEP] = self.get_temp_step()
 
+        humidity = self.get_humidity()
+        if humidity is not None:
+            data[AZD_HUMIDITY] = humidity
+
         temp_set_max = self.get_temp_set_max()
-        if temp_set_max:
+        if temp_set_max is not None:
             data[AZD_TEMP_SET_MAX] = temp_set_max
         temp_set_max_cool_air = self.get_temp_set_max_cool_air()
-        if temp_set_max_cool_air:
+        if temp_set_max_cool_air is not None:
             data[AZD_TEMP_SET_MAX_COOL_AIR] = temp_set_max_cool_air
         temp_set_max_dry_air = self.get_temp_set_max_dry_air()
-        if temp_set_max_dry_air:
+        if temp_set_max_dry_air is not None:
             data[AZD_TEMP_SET_MAX_DRY_AIR] = temp_set_max_dry_air
         temp_set_max_emerheat_air = self.get_temp_set_max_emerheat_air()
-        if temp_set_max_emerheat_air:
+        if temp_set_max_emerheat_air is not None:
             data[AZD_TEMP_SET_MAX_EMERHEAT_AIR] = temp_set_max_emerheat_air
         temp_set_max_hot_air = self.get_temp_set_max_hot_air()
-        if temp_set_max_hot_air:
+        if temp_set_max_hot_air is not None:
             data[AZD_TEMP_SET_MAX_HOT_AIR] = temp_set_max_hot_air
         temp_set_max_stop_air = self.get_temp_set_max_stop_air()
-        if temp_set_max_stop_air:
+        if temp_set_max_stop_air is not None:
             data[AZD_TEMP_SET_MAX_STOP_AIR] = temp_set_max_stop_air
         temp_set_max_vent_air = self.get_temp_set_max_vent_air()
-        if temp_set_max_vent_air:
+        if temp_set_max_vent_air is not None:
             data[AZD_TEMP_SET_MAX_VENT_AIR] = temp_set_max_vent_air
 
         temp_set_min = self.get_temp_set_min()
-        if temp_set_min:
+        if temp_set_min is not None:
             data[AZD_TEMP_SET_MIN] = temp_set_min
         temp_set_min_cool_air = self.get_temp_set_min_cool_air()
-        if temp_set_min_cool_air:
+        if temp_set_min_cool_air is not None:
             data[AZD_TEMP_SET_MIN_COOL_AIR] = temp_set_min_cool_air
         temp_set_min_dry_air = self.get_temp_set_min_dry_air()
-        if temp_set_min_dry_air:
+        if temp_set_min_dry_air is not None:
             data[AZD_TEMP_SET_MIN_DRY_AIR] = temp_set_min_dry_air
         temp_set_min_emerheat_air = self.get_temp_set_min_emerheat_air()
-        if temp_set_min_emerheat_air:
+        if temp_set_min_emerheat_air is not None:
             data[AZD_TEMP_SET_MIN_EMERHEAT_AIR] = temp_set_min_emerheat_air
         temp_set_min_hot_air = self.get_temp_set_min_hot_air()
-        if temp_set_min_hot_air:
+        if temp_set_min_hot_air is not None:
             data[AZD_TEMP_SET_MIN_HOT_AIR] = temp_set_min_hot_air
         temp_set_min_stop_air = self.get_temp_set_min_stop_air()
-        if temp_set_min_stop_air:
+        if temp_set_min_stop_air is not None:
             data[AZD_TEMP_SET_MIN_STOP_AIR] = temp_set_min_stop_air
         temp_set_min_vent_air = self.get_temp_set_min_vent_air()
-        if temp_set_min_vent_air:
+        if temp_set_min_vent_air is not None:
             data[AZD_TEMP_SET_MIN_VENT_AIR] = temp_set_min_vent_air
 
         temp_set = self.get_temp_set()
-        if temp_set:
+        if temp_set is not None:
             data[AZD_TEMP_SET] = temp_set
         temp_set_cool_air = self.get_temp_set_cool_air()
-        if temp_set_cool_air:
+        if temp_set_cool_air is not None:
             data[AZD_TEMP_SET_COOL_AIR] = temp_set_cool_air
         temp_set_dry_air = self.get_temp_set_dry_air()
-        if temp_set_dry_air:
+        if temp_set_dry_air is not None:
             data[AZD_TEMP_SET_DRY_AIR] = temp_set_dry_air
         temp_set_hot_air = self.get_temp_set_hot_air()
-        if temp_set_hot_air:
+        if temp_set_hot_air is not None:
             data[AZD_TEMP_SET_HOT_AIR] = temp_set_hot_air
         temp_set_stop_air = self.get_temp_set_stop_air()
-        if temp_set_stop_air:
+        if temp_set_stop_air is not None:
             data[AZD_TEMP_SET_STOP_AIR] = temp_set_stop_air
         temp_set_vent_air = self.get_temp_set_vent_air()
-        if temp_set_vent_air:
+        if temp_set_vent_air is not None:
             data[AZD_TEMP_SET_VENT_AIR] = temp_set_vent_air
 
         return data
 
     def get_humidity(self) -> int | None:
         """Return HVAC device humidity."""
         return self.humidity
 
     def get_power(self) -> bool | None:
         """Return HVAC device power."""
         return self.power
 
     def get_temperature(self) -> float | None:
         """Return HVAC device temperature."""
-        if self.temp:
+        if self.temp is not None:
             return round(self.temp, 1)
         return None
 
     def get_temp_set(self) -> float | None:
         """Return HVAC device temperature setpoint."""
         temp_set: float | None = None
         mode = self.get_mode()
-        if mode:
+        if mode is not None:
             if mode.is_cool():
                 temp_set = self.get_temp_set_cool_air()
             elif mode.is_dry():
                 temp_set = self.get_temp_set_dry_air()
             elif mode.is_heat():
                 temp_set = self.get_temp_set_hot_air()
             elif mode.is_stop():
                 temp_set = self.get_temp_set_stop_air()
             elif mode.is_vent():
                 temp_set = self.get_temp_set_vent_air()
         return temp_set
 
     def get_temp_set_cool_air(self) -> float | None:
         """Return HVAC device setpoint for Cool Air."""
-        if self.temp_set_cool_air:
+        if self.temp_set_cool_air is not None:
             return round(self.temp_set_cool_air, 1)
         return None
 
     def get_temp_set_dry_air(self) -> float | None:
         """Return HVAC device setpoint for Dry Air."""
-        if self.temp_set_dry_air:
+        if self.temp_set_dry_air is not None:
             return round(self.temp_set_dry_air, 1)
         return None
 
     def get_temp_set_hot_air(self) -> float | None:
         """Return HVAC device setpoint for Heat Air."""
-        if self.temp_set_hot_air:
+        if self.temp_set_hot_air is not None:
             return round(self.temp_set_hot_air, 1)
         return None
 
     def get_temp_set_stop_air(self) -> float | None:
         """Return HVAC device setpoint for Stop Air."""
-        if self.temp_set_stop_air:
+        if self.temp_set_stop_air is not None:
             return round(self.temp_set_stop_air, 1)
         return None
 
     def get_temp_set_vent_air(self) -> float | None:
         """Return HVAC device setpoint for Ventilation Air."""
-        if self.temp_set_vent_air:
+        if self.temp_set_vent_air is not None:
             return round(self.temp_set_vent_air, 1)
         return None
 
     def get_temp_set_max(self) -> float | None:
         """Return HVAC device max setpoint."""
         max_temp: float | None = None
         temps = [
@@ -236,45 +239,45 @@
             if temp is not None:
                 if max_temp is None or temp > max_temp:
                     max_temp = temp
         return max_temp
 
     def get_temp_set_max_cool_air(self) -> float | None:
         """Return HVAC device max setpoint for Cool Air."""
-        if self.temp_set_max_cool_air:
+        if self.temp_set_max_cool_air is not None:
             return round(self.temp_set_max_cool_air, 1)
         return None
 
     def get_temp_set_max_dry_air(self) -> float | None:
         """Return HVAC device max setpoint for Dry Air."""
-        if self.temp_set_max_dry_air:
+        if self.temp_set_max_dry_air is not None:
             return round(self.temp_set_max_dry_air, 1)
         return None
 
     def get_temp_set_max_emerheat_air(self) -> float | None:
         """Return HVAC device max setpoint for Emergency Heat Air."""
-        if self.temp_set_max_emerheat_air:
+        if self.temp_set_max_emerheat_air is not None:
             return round(self.temp_set_max_emerheat_air, 1)
         return None
 
     def get_temp_set_max_hot_air(self) -> float | None:
         """Return HVAC device max setpoint for Heat Air."""
-        if self.temp_set_max_hot_air:
+        if self.temp_set_max_hot_air is not None:
             return round(self.temp_set_max_hot_air, 1)
         return None
 
     def get_temp_set_max_stop_air(self) -> float | None:
         """Return HVAC device max setpoint for Stop Air."""
-        if self.temp_set_max_stop_air:
+        if self.temp_set_max_stop_air is not None:
             return round(self.temp_set_max_stop_air, 1)
         return None
 
     def get_temp_set_max_vent_air(self) -> float | None:
         """Return HVAC device max setpoint for Ventilation Air."""
-        if self.temp_set_max_vent_air:
+        if self.temp_set_max_vent_air is not None:
             return round(self.temp_set_max_vent_air, 1)
         return None
 
     def get_temp_set_min(self) -> float | None:
         """Return HVAC device min setpoint."""
         min_temp: float | None = None
         temps = [
@@ -295,45 +298,45 @@
         """Return HVAC device min setpoint for Cool Air."""
         if self.temp_set_min_cool_air:
             return round(self.temp_set_min_cool_air, 1)
         return None
 
     def get_temp_set_min_dry_air(self) -> float | None:
         """Return HVAC device min setpoint for Dry Air."""
-        if self.temp_set_min_dry_air:
+        if self.temp_set_min_dry_air is not None:
             return round(self.temp_set_min_dry_air, 1)
         return None
 
     def get_temp_set_min_emerheat_air(self) -> float | None:
         """Return HVAC device min setpoint for Emergency Heat Air."""
-        if self.temp_set_min_emerheat_air:
+        if self.temp_set_min_emerheat_air is not None:
             return round(self.temp_set_min_emerheat_air, 1)
         return None
 
     def get_temp_set_min_hot_air(self) -> float | None:
         """Return HVAC device min setpoint for Hot Air."""
-        if self.temp_set_min_hot_air:
+        if self.temp_set_min_hot_air is not None:
             return round(self.temp_set_min_hot_air, 1)
         return None
 
     def get_temp_set_min_stop_air(self) -> float | None:
         """Return HVAC device min setpoint for Stop Air."""
-        if self.temp_set_min_stop_air:
+        if self.temp_set_min_stop_air is not None:
             return round(self.temp_set_min_stop_air, 1)
         return None
 
     def get_temp_set_min_vent_air(self) -> float | None:
         """Return HVAC device min setpoint for Ventilation Air."""
-        if self.temp_set_min_vent_air:
+        if self.temp_set_min_vent_air is not None:
             return round(self.temp_set_min_vent_air, 1)
         return None
 
     def get_temp_step(self) -> float | None:
         """Return HVAC device temperature step."""
-        if self.temp_step:
+        if self.temp_step is not None:
             return round(self.temp_step, 1)
         return API_DEFAULT_TEMP_STEP
 
     def update(self, data: dict[str, Any]) -> None:
         """Update HVAC device data."""
         super().update(data)
```

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/installation.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/installation.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/system.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/system.py`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud/zone.py` & `aioairzone-cloud-0.1.8/aioairzone_cloud/zone.py`

 * *Files 3% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         data = super().data()
 
         data[AZD_MASTER] = self.get_master()
         data[AZD_SYSTEM] = self.get_system()
         data[AZD_ZONE] = self.get_zone()
 
         system_id = self.get_system_id()
-        if system_id:
+        if system_id is not None:
             data[AZD_SYSTEM_ID] = system_id
 
         return data
 
     def get_master(self) -> bool | None:
         """Return Zone device master/slave."""
         return self.master
```

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/PKG-INFO` & `aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioairzone-cloud
-Version: 0.1.7
+Version: 0.1.8
 Summary: Library to control Airzone Cloud devices
 Author-email: Álvaro Fernández Rojas <noltari@gmail.com>
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/Noltari/aioairzone-cloud
 Project-URL: Bug Tracker, https://github.com/Noltari/aioairzone-cloud/issues
 Keywords: airzone,cloud,hvac,home
 Platform: any
```

### Comparing `aioairzone-cloud-0.1.7/aioairzone_cloud.egg-info/SOURCES.txt` & `aioairzone-cloud-0.1.8/aioairzone_cloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioairzone-cloud-0.1.7/pyproject.toml` & `aioairzone-cloud-0.1.8/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "aioairzone-cloud"
-version = "0.1.7"
+version = "0.1.8"
 description = "Library to control Airzone Cloud devices"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {text = "Apache-2.0"}
 keywords = ["airzone", "cloud", "hvac", "home"] 
 authors = [
   {name = "Álvaro Fernández Rojas", email = "noltari@gmail.com" }
```

