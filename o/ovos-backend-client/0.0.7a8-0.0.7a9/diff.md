# Comparing `tmp/ovos-backend-client-0.0.7a8.tar.gz` & `tmp/ovos-backend-client-0.0.7a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.0.7a8.tar", last modified: Wed Jun  7 10:49:24 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.0.7a9.tar", last modified: Wed Jun  7 23:45:02 2023, max compression
```

## Comparing `ovos-backend-client-0.0.7a8.tar` & `ovos-backend-client-0.0.7a9.tar`

### file list

```diff
@@ -1,29 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5375 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.038743 ovos-backend-client-0.0.7a8/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21426 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     3549 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16318 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)     8991 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/ovos.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/backends/selene.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    12079 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 10:49:24.038743 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 10:49:24.000000 ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 10:49:24.042743 ovos-backend-client-0.0.7a8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 10:49:23.000000 ovos-backend-client-0.0.7a8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20820 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/setup.py
```

### Comparing `ovos-backend-client-0.0.7a8/README.md` & `ovos-backend-client-0.0.7a9/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,41 +1,34 @@
 # OVOS Backend Client
 
 Python client library for interaction with several supported backends under a single unified interface
 
 - Personal backend - [self hosted](https://github.com/OpenVoiceOS/OVOS-local-backend)
-- Selene - https://api.mycroft.ai
-- OpenVoiceOS API Service - https://api.openvoiceos.com
 - Offline - support for setting your own api keys and query services directly
 
 ## Backend Overview
 
-| API       | Offline | Personal | Selene | OVOS    | 
-|-----------|---------|----------|--------|---------|
-| Admin     | yes [1] | yes      | no     | no      | 
-| Device    | yes [2] | yes      | yes    | yes [4] | 
-| Metrics   | yes [2] | yes      | yes    | yes [4] | 
-| Dataset   | yes [2] | yes      | yes    | yes [4] | 
-| OAuth     | yes [2] | yes      | yes    | yes [4] |
-| Wolfram   | yes [3] | yes      | yes    | yes     | 
-| Geolocate | yes     | yes      | yes    | yes     |
-| STT       | yes [3] | yes      | yes    | yes     | 
-| Weather   | yes [3] | yes      | yes    | yes     | 
-| Email     | yes [3] | yes      | yes    | yes     |
+| API       | Offline | Personal |
+|-----------|---------|----------|
+| Admin     | yes [1] | yes      |
+| Device    | yes     | yes      |
+| Metrics   | yes     | yes      |
+| Dataset   | yes     | yes      |
+| OAuth     | yes     | yes      |
+| Wolfram   | yes [2] | yes      |
+| Geolocate | yes     | yes      |
+| STT       | yes [2] | yes      |
+| Weather   | yes [2] | yes      |
+| Email     | yes [2] | yes      |
 
     [1] will update user level mycroft.conf
-    [2] shared json database with personal backend for UI compat
-    [3] needs additional configuration (eg. credentials)
-    [4] uses offline_backend functionality
+    [2] needs additional configuration (eg. credentials)
+    [3] uses offline_backend functionality
 
 
-## STT
-
-a companion stt plugin is available - [ovos-stt-plugin-selene](https://github.com/OpenVoiceOS/ovos-stt-plugin-selene)
-
 ## Geolocation
 
 ```python
 from ovos_backend_client.api import GeolocationApi
 
 geo = GeolocationApi()
 data = geo.get_geolocation("Lisbon Portugal")
@@ -52,27 +45,36 @@
 from ovos_backend_client.api import OpenWeatherMapApi
 
 owm = OpenWeatherMapApi()
 data = owm.get_weather()
 # dict - see api docs from owm onecall api
 ```
 
+DEPRECATED - weather skill now uses open meteo
+
 ## Wolfram Alpha proxy
 
 ```python
 from ovos_backend_client.api import WolframAlphaApi
 
 wolf = WolframAlphaApi()
 answer = wolf.spoken("what is the speed of light")
 # The speed of light has a value of about 300 million meters per second
 
 data = wolf.full_results("2+2")
 # dict - see api docs from wolfram
 ```
 
+## STT
+
+a companion stt plugin is available - [ovos-stt-plugin-selene](https://github.com/OpenVoiceOS/ovos-stt-plugin-selene)
+
+DEPRECATED - use https://github.com/OpenVoiceOS/ovos-stt-plugin-server with a public server instead
+
+
 ## Remote Settings
 
 To interact with skill settings on selene
 
 ```python
 from ovos_backend_client.settings import RemoteSkillSettings
```

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/api.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,22 @@
 from ovos_utils import timed_lru_cache
 from ovos_utils.log import LOG
 
-from ovos_backend_client.backends import OfflineBackend, OVOSAPIBackend, \
-    SeleneBackend, PersonalBackend, BackendType, get_backend_config, API_REGISTRY
+from ovos_backend_client.backends import OfflineBackend, PersonalBackend, \
+    BackendType, get_backend_config, API_REGISTRY
 
 
 class BaseApi:
     def __init__(self, url=None, version="v1", identity_file=None, backend_type=None, credentials=None):
         url, version, identity_file, backend_type = get_backend_config(url, version,
                                                                        identity_file, backend_type)
         self.url = url
         self.credentials = credentials or {}
-        if backend_type == BackendType.SELENE:
-            self.backend = SeleneBackend(url, version, identity_file)
-        elif backend_type == BackendType.PERSONAL:
+        if backend_type == BackendType.PERSONAL:
             self.backend = PersonalBackend(url, version, identity_file)
-        elif backend_type == BackendType.OVOS_API:
-            self.backend = OVOSAPIBackend(url, version, identity_file)
         else:  # if backend_type == BackendType.OFFLINE:
             self.backend = OfflineBackend(url, version, identity_file)
         self.validate_backend_type()
 
     def validate_backend_type(self):
         pass
 
@@ -328,17 +324,15 @@
 
     def __init__(self, url=None, version="v1", identity_file=None, backend_type=None):
         super().__init__(url, version, identity_file, backend_type)
 
     def validate_backend_type(self):
         if not API_REGISTRY[self.backend_type]["geolocate"]:
             raise ValueError(f"{self.__class__.__name__} not available for {self.backend_type}")
-        if self.backend_type == BackendType.OVOS_API:
-            self.url = f"{self.backend_url}/geolocate"
-        elif self.backend_type == BackendType.OFFLINE:
+        if self.backend_type == BackendType.OFFLINE:
             self.url = "https://nominatim.openstreetmap.org"
         else:
             self.url = f"{self.backend_url}/{self.backend_version}/geolocation"
 
     def get_geolocation(self, location):
         """Call the geolocation endpoint.
 
@@ -381,17 +375,15 @@
 
     def validate_backend_type(self):
         if not API_REGISTRY[self.backend_type]["wolfram"]:
             raise ValueError(f"{self.__class__.__name__} not available for {self.backend_type}")
         if self.backend_type == BackendType.OFFLINE and not self.credentials["wolfram"]:
             raise ValueError("WolframAlpha api key not set!")
 
-        if self.backend_type == BackendType.OVOS_API:
-            self.url = f"{self.backend_url}/wolframalpha"
-        elif self.backend_type == BackendType.OFFLINE:
+        if self.backend_type == BackendType.OFFLINE:
             self.url = "https://api.wolframalpha.com"
         else:
             self.url = f"{self.backend_url}/{self.backend_version}/wolframAlpha"
 
     # cached to save api calls, wolfram answer wont change often
     @timed_lru_cache(seconds=60 * 30)
     def spoken(self, query, units="metric", lat_lon=None, optional_params=None):
@@ -419,17 +411,15 @@
         super().__init__(url, version, identity_file, backend_type, credentials={"owm": key})
 
     def validate_backend_type(self):
         if not API_REGISTRY[self.backend_type]["owm"]:
             raise ValueError(f"{self.__class__.__name__} not available for {self.backend_type}")
         if self.backend_type == BackendType.OFFLINE and not self.backend.credentials["owm"]:
             raise ValueError("OWM api key not set!")
-        if self.backend_type == BackendType.OVOS_API:
-            self.url = f"{self.backend_url}/weather"
-        elif self.backend_type == BackendType.OFFLINE:
+        if self.backend_type == BackendType.OFFLINE:
             self.url = "https://api.openweathermap.org/data/2.5"
         else:
             self.url = f"{self.backend_url}/{self.backend_version}/owm"
 
     def owm_language(self, lang: str):
         """
         OWM supports 31 languages, see https://openweathermap.org/current#multi
```

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/base.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/backends/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,14 @@
 except ImportError:
     TimezoneFinder = None
 
 
 class BackendType(str, Enum):
     OFFLINE = "offline"
     PERSONAL = "personal"
-    SELENE = "selene"
-    OVOS_API = "ovos_api"
 
 
 class AbstractBackend:
 
     def __init__(self, url, version="v1", identity_file=None, backend_type=BackendType.OFFLINE, credentials=None):
         self.backend_url = url
         self.backend_type = backend_type
```

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/offline.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/backends/offline.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/backends/personal.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/backends/personal.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/cloud.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/config.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/database.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/database.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/identity.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/pairing.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/pairing.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,20 +7,18 @@
 from ovos_utils.log import LOG
 from ovos_utils.messagebus import Message, FakeBus
 from ovos_utils.network_utils import is_connected
 
 from ovos_backend_client.api import DeviceApi, BackendType
 from ovos_backend_client.exceptions import BackendDown, InternetDown, HTTPError
 from ovos_backend_client.identity import IdentityManager
-from ovos_backend_client.backends.selene import SELENE_API_URL
 from ovos_backend_client.backends import BackendType, get_backend_type
 
 
-PAIRING_BACKENDS = [BackendType.PERSONAL,
-                    BackendType.SELENE]
+PAIRING_BACKENDS = [BackendType.PERSONAL]
 
 
 def is_backend_disabled():
     config = Configuration()
     if not config.get("server"):
         # missing server block implies disabling backend
         return True
@@ -121,16 +119,16 @@
                  enclosure=None,
                  code_callback=None,
                  error_callback=None,
                  success_callback=None,
                  start_callback=None,
                  restart_callback=None,
                  end_callback=None,
-                 pairing_url="home.mycroft.ai",
-                 api_url=SELENE_API_URL,
+                 pairing_url="0.0.0.0;6712",
+                 api_url="0.0.0.0;6712",
                  version="v1",
                  identity_file=None,
                  backend_type=None):
         if enclosure:
             LOG.warning("enclosure argument has been deprecated, it is no longer used")
         self.pairing_url = pairing_url
         self.api_url = api_url
@@ -150,15 +148,15 @@
         self.activator = None
         self.activator_lock = Lock()
         self.activator_cancelled = False
         self.counter_lock = Lock()
         self.count = -1  # for repeating pairing code. -1 = not running
         self.num_failed_codes = 0
 
-    def set_api_url(self, url,  version="v1", identity_file=None, backend_type=BackendType.SELENE):
+    def set_api_url(self, url,  version="v1", identity_file=None, backend_type=BackendType.PERSONAL):
         if not url.startswith("http"):
             url = f"http://{url}"
         self.api_url = url
         self.api = DeviceApi(url, version=version,
                              identity_file=identity_file,
                              backend_type=backend_type)
```

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client/settings.py` & `ovos-backend-client-0.0.7a9/ovos_backend_client/settings.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a8/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,10 +14,8 @@
 ovos_backend_client.egg-info/SOURCES.txt
 ovos_backend_client.egg-info/dependency_links.txt
 ovos_backend_client.egg-info/requires.txt
 ovos_backend_client.egg-info/top_level.txt
 ovos_backend_client/backends/__init__.py
 ovos_backend_client/backends/base.py
 ovos_backend_client/backends/offline.py
-ovos_backend_client/backends/ovos.py
-ovos_backend_client/backends/personal.py
-ovos_backend_client/backends/selene.py
+ovos_backend_client/backends/personal.py
```

### Comparing `ovos-backend-client-0.0.7a8/setup.py` & `ovos-backend-client-0.0.7a9/setup.py`

 * *Files identical despite different names*

