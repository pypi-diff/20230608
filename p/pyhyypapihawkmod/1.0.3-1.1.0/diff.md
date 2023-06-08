# Comparing `tmp/pyhyypapihawkmod-1.0.3.tar.gz` & `tmp/pyhyypapihawkmod-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhyypapihawkmod-1.0.3.tar", last modified: Fri Jun  2 16:41:27 2023, max compression
+gzip compressed data, was "pyhyypapihawkmod-1.1.0.tar", last modified: Thu Jun  8 13:20:32 2023, max compression
```

## Comparing `pyhyypapihawkmod-1.0.3.tar` & `pyhyypapihawkmod-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 16:41:27.223935 pyhyypapihawkmod-1.0.3/
--rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/LICENSE.md
--rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/MANIFEST.in
--rw-rw-rw-   0        0        0      517 2023-06-02 16:41:27.223392 pyhyypapihawkmod-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1609 2023-06-02 16:39:00.000000 pyhyypapihawkmod-1.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 16:41:27.213476 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/
--rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/__init__.py
--rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/__main__.py
--rw-rw-rw-   0        0        0     5760 2023-06-02 16:34:38.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/alarm_info.py
--rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/android_checkin_pb2.py
--rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/checkin_pb2.py
--rw-rw-rw-   0        0        0    27687 2023-06-02 10:07:05.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/client.py
--rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/constants.py
--rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/exceptions.py
--rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/mcs_pb2.py
--rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/push_receiver.py
-drwxrwxrwx   0        0        0        0 2023-06-02 16:41:27.221829 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/
--rw-rw-rw-   0        0        0      517 2023-06-02 16:41:27.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      551 2023-06-02 16:41:27.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 16:41:27.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-02 16:41:27.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2023-06-02 16:41:27.000000 pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-02 16:41:27.223935 pyhyypapihawkmod-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      921 2023-06-02 16:39:07.000000 pyhyypapihawkmod-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:20:32.863070 pyhyypapihawkmod-1.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/LICENSE.md
+-rw-rw-rw-   0        0        0       20 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      517 2023-06-08 13:20:32.862558 pyhyypapihawkmod-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1679 2023-06-08 12:51:40.000000 pyhyypapihawkmod-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 13:20:32.849773 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/
+-rw-rw-rw-   0        0        0      429 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/__init__.py
+-rw-rw-rw-   0        0        0      151 2023-05-24 18:38:52.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/__main__.py
+-rw-rw-rw-   0        0        0     7431 2023-06-08 12:47:29.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/alarm_info.py
+-rw-rw-rw-   0        0        0     2815 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/android_checkin_pb2.py
+-rw-rw-rw-   0        0        0     2857 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/checkin_pb2.py
+-rw-rw-rw-   0        0        0    27687 2023-06-08 12:19:08.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/client.py
+-rw-rw-rw-   0        0        0     4005 2023-05-28 09:35:32.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/constants.py
+-rw-rw-rw-   0        0        0      248 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/exceptions.py
+-rw-rw-rw-   0        0        0     7557 2023-05-23 06:11:42.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/mcs_pb2.py
+-rw-rw-rw-   0        0        0    16227 2023-05-27 21:24:48.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/push_receiver.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:20:32.860527 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/
+-rw-rw-rw-   0        0        0      517 2023-06-08 13:20:32.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      551 2023-06-08 13:20:32.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 13:20:32.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-06-08 13:20:32.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2023-06-08 13:20:32.000000 pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 13:20:32.863070 pyhyypapihawkmod-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      921 2023-06-08 12:52:02.000000 pyhyypapihawkmod-1.1.0/setup.py
```

### Comparing `pyhyypapihawkmod-1.0.3/LICENSE.md` & `pyhyypapihawkmod-1.1.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/PKG-INFO` & `pyhyypapihawkmod-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.0.3
+Version: 1.1.0
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.0.3/README.md` & `pyhyypapihawkmod-1.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 - CLI usage. (GCF client is there, just needs some more automation.)
 - Capture panic api...for obvious reasons.
 - What zone caused arm/arm stay not to work. - Looks like GCM/Firebase push messages. Added GCM client...just run main program and register GCF code in function called register gcf. It works.
 
 
 Changelog 
 
+1.1.0
+- Added feature to detect which zones triggered an alarm.
+
+
 1.0.3
 - Fixed a bug where stay profiles would mostly go to false even though stay profiles were armed.
 
 1.0.2
 - Fixed a bug where the parameters for certain items were swapped
 
 1.0.1
```

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/alarm_info.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/alarm_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -41,14 +41,56 @@
             _response = {
                 "lastNoticeTime": _last_event_datetime,
                 "lastNoticeName": EventNumber[str(_last_event)],
             }
 
         return _response
 
+
+
+    def _new_notifications(self, site_id: int) -> Any:
+
+        global _last_notification_check_timestamp   
+        _response = []
+
+        _notifications = self._client.site_notifications(
+            site_id=site_id)
+                
+        _current_timestamp = round(datetime.now().timestamp())
+            
+        for x in _notifications:
+            
+            _notification_timestamp = round(x['timestamp']/1000)
+            if _current_timestamp - _notification_timestamp > 120:
+                continue
+            if _notification_timestamp <= (_last_notification_check_timestamp-30):
+                continue
+            _response.append(x)
+        
+        _last_notification_check_timestamp = _current_timestamp
+ 
+        return _response
+
+
+    def _triggered_zones(self, site_id: int) -> Any:
+           
+        triggeredZoneIds = []
+        _new_notifications = self._new_notifications(site_id=site_id)
+        
+        for _notification in _new_notifications:
+            if _notification['eventNumber'] != 5:
+                continue
+            triggeredZoneIds.append(_notification['zoneId'])  
+                 
+        _response = triggeredZoneIds
+        
+        return _response
+     
+
+     
     def _format_data(self) -> dict[Any, Any]:
         """Format data for Hass."""
 
         # The API returns data from site level.
         # Partitions are used as entity that actions are performed on.
 
         site_ids = {site["id"]: site for site in self._sync_info["sites"]}
@@ -62,14 +104,16 @@
         }
         
         trigger_ids = {
             trigger["id"]: trigger for trigger in self._sync_info["triggers"]
         }
         
         for site in site_ids:
+            
+            triggered_zones = self._triggered_zones(site_id=site)
 
             # Add last site notification.
             _last_notice = self._last_notice(site_id=site)
             site_ids[site]["lastNoticeTime"] = _last_notice["lastNoticeTime"]
             site_ids[site]["lastNoticeName"] = _last_notice["lastNoticeName"]
 
             # Add triggers (PGM / Automations in APP)
@@ -102,14 +146,21 @@
 
                 # Add zone bypass info to zone.
                 for zone in site_ids[site]["partitions"][partition]["zones"]:
                     site_ids[site]["partitions"][partition]["zones"][zone][
                         "bypassed"
                     ] = bool(zone in self._state_info["bypassedZoneIds"])
 
+                # Add zone trigger info to zone (Zone triggered alarm).
+                for zone in site_ids[site]["partitions"][partition]["zones"]:
+                    site_ids[site]["partitions"][partition]["zones"][zone][
+                        "triggered"
+                    ] = bool(zone in triggered_zones)
+
+
                 # Add stay profile info.
                 site_ids[site]["partitions"][partition]["stayProfiles"] = {
                     key: value
                     for (key, value) in stay_ids.items()
                     if key in site_ids[site]["partitions"][partition]["stayProfileIds"]
                 }
```

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/android_checkin_pb2.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/android_checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/checkin_pb2.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/checkin_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/client.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/client.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/constants.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/constants.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/mcs_pb2.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/mcs_pb2.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod/push_receiver.py` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod/push_receiver.py`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/PKG-INFO` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhyypapihawkmod
-Version: 1.0.3
+Version: 1.1.0
 Summary: IDS Hyyp/ADT Secure Home API
 Home-page: https://github.com/hawky358/pyHyypApi
 Author: hawky358 (Original code by Renier Moorcroft)
 Author-email: hawky358@users.github.com
 License: Apache Software License 2.0
 Requires-Python: >=3.6
 License-File: LICENSE.md
```

### Comparing `pyhyypapihawkmod-1.0.3/pyhyypapihawkmod.egg-info/SOURCES.txt` & `pyhyypapihawkmod-1.1.0/pyhyypapihawkmod.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhyypapihawkmod-1.0.3/setup.py` & `pyhyypapihawkmod-1.1.0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='pyhyypapihawkmod',
-    version="1.0.3",
+    version="1.1.0",
     license='Apache Software License 2.0',
     author='hawky358 (Original code by Renier Moorcroft)',
     author_email='hawky358@users.github.com',
     description='IDS Hyyp/ADT Secure Home API',
     long_description="API for accessing IDS Hyyp. This is used by ADT Home Connect and possibly others. Please view readme on github (Based on 0.0.0.8 by Renier Moorcroft with updated protobuf files) ",
     url='https://github.com/hawky358/pyHyypApi',
     packages=setuptools.find_packages(),
```

