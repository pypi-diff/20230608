# Comparing `tmp/ovos-backend-client-0.0.7a9.tar.gz` & `tmp/ovos-backend-client-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-backend-client-0.0.7a9.tar", last modified: Wed Jun  7 23:45:02 2023, max compression
+gzip compressed data, was "ovos-backend-client-0.1.0a2.tar", last modified: Thu Jun  8 00:08:22 2023, max compression
```

## Comparing `ovos-backend-client-0.0.7a9.tar` & `ovos-backend-client-0.1.0a2.tar`

### file list

```diff
@@ -1,27 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/ovos_backend_client/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20820 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16270 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    24024 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/offline.py
--rw-r--r--   0 runner    (1001) docker     (123)    18134 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/backends/personal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4593 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/identity.py
--rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/pairing.py
--rw-r--r--   0 runner    (1001) docker     (123)    15623 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/ovos_backend_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 23:45:02.000000 ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 23:45:02.063004 ovos-backend-client-0.0.7a9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-07 23:45:01.000000 ovos-backend-client-0.0.7a9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.487462 ovos-backend-client-0.1.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     4011 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/ovos_backend_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33404 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26658 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40613 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/offline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37782 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/backends/personal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3276 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15926 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11975 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/pairing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16512 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/ovos_backend_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 00:08:22.483462 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-08 00:08:22.000000 ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 00:08:22.487462 ovos-backend-client-0.1.0a2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-08 00:08:21.000000 ovos-backend-client-0.1.0a2/setup.py
```

### Comparing `ovos-backend-client-0.0.7a9/README.md` & `ovos-backend-client-0.1.0a2/README.md`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client/backends/__init__.py` & `ovos-backend-client-0.1.0a2/ovos_backend_client/backends/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,35 +3,39 @@
 from ovos_backend_client.backends.base import BackendType
 from ovos_backend_client.backends.offline import OfflineBackend
 from ovos_backend_client.backends.personal import PersonalBackend
 
 API_REGISTRY = {
     BackendType.OFFLINE: {
         "admin": True,  # updates mycroft.conf if used
-        "device": True,  # shared database with local backend for UI compat
-        "dataset": True,  # shared database with local backend for ww tagger UI compat
-        "metrics": True,  # shared database with local backend for metrics UI compat
+        "database": True,  # manages local files only
+        "device": True,  # manages local files only
+        "skill_settings": True,  # manages local files only
+        "dataset": True,  # manages local files only
+        "metrics": True,  # manages local files only
         "wolfram": True,  # key needs to be set
         "geolocate": True,  # nominatim - no key needed
         "stt": True,  # uses OPM and reads from mycroft.conf
         "owm": True,  # key needs to be set
         "email": True,  # smtp config needs to be set
-        "oauth": True  # use local backend UI on same device to register apps
+        "oauth": True  # oauth PHAL plugin to register apps
     },
     BackendType.PERSONAL: {
         "admin": True,
+        "database": True,  # requires ovos-personal-backend>=0.2.0
         "device": True,
+        "skill_settings": True,
         "dataset": True,
         "metrics": True,
         "wolfram": True,
         "geolocate": True,
         "stt": True,
         "owm": True,
         "email": True,
-        "oauth": True  # can use local backend UI to register apps
+        "oauth": True  # can use personal-backend-manager to register apps
     }
 }
 
 
 def get_backend_type(conf=None):
     conf = conf or Configuration()
     if "server" in conf:
```

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client/cloud.py` & `ovos-backend-client-0.1.0a2/ovos_backend_client/cloud.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client/config.py` & `ovos-backend-client-0.1.0a2/ovos_backend_client/config.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client/identity.py` & `ovos-backend-client-0.1.0a2/ovos_backend_client/identity.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client/pairing.py` & `ovos-backend-client-0.1.0a2/ovos_backend_client/pairing.py`

 * *Files identical despite different names*

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client/settings.py` & `ovos-backend-client-0.1.0a2/ovos_backend_client/settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,25 +5,48 @@
 from os import makedirs
 from os.path import dirname, expanduser, join, isfile, isdir
 
 from json_database import JsonStorage
 from ovos_config import Configuration
 from ovos_utils import camel_case_split
 from ovos_utils.configuration import get_xdg_config_save_path, get_xdg_data_save_path, get_xdg_data_dirs
-
-from ovos_backend_client.api import DeviceApi
+from ovos_backend_client.database import SkillSettingsModel
+import ovos_backend_client.api as _api
 
 
 def get_display_name(skill_name: str):
     """Splits camelcase and removes leading/trailing "skill"."""
     skill_name = skill_name.replace("_", " ").replace("-", " ")
     skill_name = re.sub(r'(^[Ss]kill|[Ss]kill$)', '', skill_name)
     return camel_case_split(skill_name).title().strip()
 
 
+def get_local_settings():
+    settings_path = f"{get_xdg_config_save_path()}/skills"
+    if not isdir(settings_path):
+        return []
+    settings = {}
+    meta = {}
+    all_settings = []
+    for skill_id in os.listdir(settings_path):
+        s = f"{settings_path}/{skill_id}/settings.json"
+        if isfile(s):
+            with open(s) as f:
+                settings = json.load(f)
+        s = f"{settings_path}/{skill_id}/settingsmeta.json"
+        if isfile(s):
+            meta = json.load(f)
+
+        display_name = skill_id.split(".")[-1].replace("_", "").replace("-", "").title()
+        s = SkillSettingsModel(skill_id=skill_id, meta=meta,
+                               skill_settings=settings, display_name=display_name)
+        all_settings.append(s)
+    return all_settings
+
+
 class RemoteSkillSettings:
     """ WARNING: selene backend does not use proper skill_id, if you have
     skills with same name but different author settings will overwrite each
     other on the backend, THIS CLASS IS NOT 100% SAFE in mycroft-core
 
     mycroft-core uses msm to generate weird metadata, removes author and munges github branch names into id
     see: https://github.com/MycroftAI/mycroft-skills-manager/blob/master/msm/skill_entry.py#L145
@@ -33,15 +56,15 @@
 
     you can define arbitrary strings as skill_id to use this as a datastore
 
     skill matching is currently done by checking "if {skill_id} in string"
     """
 
     def __init__(self, skill_id, settings=None, meta=None, url=None, version="v1", remote_id=None):
-        self.api = DeviceApi(url, version)
+        self.api = _api.DeviceApi(url, version)
         self.skill_id = skill_id
         self.identifier = remote_id or \
                           self.selene_gid if not skill_id.startswith("@") else skill_id
         self.settings = settings or {}
         self.meta = meta or {}
         self.local_path = join(get_xdg_config_save_path(), 'skills', self.skill_id, 'settings.json')
         if not self.settings:
@@ -154,15 +177,15 @@
                     return self.deserialize(sets)
 
         s = match_settings(data, self.identifier) or \
             match_settings(data, self.skill_id)
 
         if s:
             self.meta = s.meta
-            self.settings = s.settings
+            self.settings = s.skill_settings
             # update actual identifier from selene
             self.identifier = s.identifier
 
     def upload(self):
         data = self.serialize()
         return self.api.put_skill_settings_v1(data)
 
@@ -268,15 +291,15 @@
 
     def __init__(self, api=None):
         path = os.path.join(get_xdg_data_save_path(), 'skills.json')
         super().__init__(path, disable_lock=True)
         if "skills" not in self:
             self["skills"] = []
             self.store()
-        self.api = api or DeviceApi()
+        self.api = api or _api.DeviceApi()
 
     @staticmethod
     def _get_default_skills_directory(conf=None):
         """ return default directory to scan for skills
 
         users can define the data directory in mycroft.conf
         the skills folder name (relative to data_dir) can also be defined there
@@ -407,19 +430,19 @@
 
 
 if __name__ == "__main__":
     s = RemoteSkillSettings("mycroft-date-time")
     print(s.api.get_skill_settings_v1())
     s.download()
     print(s)
-    s.settings["not"] = "yes"  # ignored, not in meta
-    s.settings["show_time"] = True
+    s.skill_settings["not"] = "yes"  # ignored, not in meta
+    s.skill_settings["show_time"] = True
     s.upload()
     s.download()
     print(s)
-    s.settings["not"] = "yes"
+    s.skill_settings["not"] = "yes"
     s.generate_meta()  # now in meta
-    s.settings["not"] = "no"
-    s.settings["show_time"] = False
+    s.skill_settings["not"] = "no"
+    s.skill_settings["show_time"] = False
     s.upload()
     s.download()
     print(s)
```

### Comparing `ovos-backend-client-0.0.7a9/ovos_backend_client.egg-info/SOURCES.txt` & `ovos-backend-client-0.1.0a2/ovos_backend_client.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+CHANGELOG.md
+MANIFEST.in
 README.md
 setup.py
 ovos_backend_client/__init__.py
 ovos_backend_client/api.py
 ovos_backend_client/cloud.py
 ovos_backend_client/config.py
 ovos_backend_client/database.py
```

### Comparing `ovos-backend-client-0.0.7a9/setup.py` & `ovos-backend-client-0.1.0a2/setup.py`

 * *Files identical despite different names*

