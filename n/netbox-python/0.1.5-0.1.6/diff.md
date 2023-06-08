# Comparing `tmp/netbox_python-0.1.5.tar.gz` & `tmp/netbox_python-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_python-0.1.5.tar", last modified: Tue Mar 28 16:52:56 2023, max compression
+gzip compressed data, was "netbox_python-0.1.6.tar", last modified: Thu Jun  8 19:17:33 2023, max compression
```

## Comparing `netbox_python-0.1.5.tar` & `netbox_python-0.1.6.tar`

### file list

```diff
@@ -1,43 +1,55 @@
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.191800 netbox_python-0.1.5/
--rw-r--r--   0 ahanson    (502) staff       (20)     3929 2023-02-27 17:19:35.000000 netbox_python-0.1.5/CONTRIBUTING.rst
--rw-r--r--   0 ahanson    (502) staff       (20)      584 2023-02-27 16:58:50.000000 netbox_python-0.1.5/LICENSE
--rw-r--r--   0 ahanson    (502) staff       (20)      262 2023-02-27 18:27:55.000000 netbox_python-0.1.5/MANIFEST.in
--rw-r--r--   0 ahanson    (502) staff       (20)     6476 2023-03-28 16:52:56.191874 netbox_python-0.1.5/PKG-INFO
--rw-r--r--   0 ahanson    (502) staff       (20)     5673 2023-03-17 17:23:36.000000 netbox_python-0.1.5/README.md
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.183148 netbox_python-0.1.5/docs/
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.184976 netbox_python-0.1.5/docs/images/
--rw-r--r--   0 ahanson    (502) staff       (20)     6347 2023-03-03 17:12:55.000000 netbox_python-0.1.5/docs/images/screenshot.png
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.187346 netbox_python-0.1.5/netbox_python/
--rw-r--r--   0 ahanson    (502) staff       (20)      274 2023-03-03 19:32:40.000000 netbox_python-0.1.5/netbox_python/__init__.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.191125 netbox_python-0.1.5/netbox_python/api/
--rw-r--r--   0 ahanson    (502) staff       (20)      454 2023-03-03 19:40:30.000000 netbox_python-0.1.5/netbox_python/api/__init__.py
--rw-r--r--   0 ahanson    (502) staff       (20)      822 2023-03-03 19:28:32.000000 netbox_python-0.1.5/netbox_python/api/circuits.py
--rw-r--r--   0 ahanson    (502) staff       (20)      372 2023-03-03 19:28:38.000000 netbox_python-0.1.5/netbox_python/api/core.py
--rw-r--r--   0 ahanson    (502) staff       (20)     5957 2023-03-03 19:28:44.000000 netbox_python-0.1.5/netbox_python/api/dcim.py
--rw-r--r--   0 ahanson    (502) staff       (20)     2105 2023-03-03 19:28:48.000000 netbox_python-0.1.5/netbox_python/api/extras.py
--rw-r--r--   0 ahanson    (502) staff       (20)     2175 2023-03-03 19:28:52.000000 netbox_python-0.1.5/netbox_python/api/ipam.py
--rw-r--r--   0 ahanson    (502) staff       (20)      275 2023-03-03 19:28:56.000000 netbox_python-0.1.5/netbox_python/api/plugins.py
--rw-r--r--   0 ahanson    (502) staff       (20)      928 2023-03-03 19:29:00.000000 netbox_python-0.1.5/netbox_python/api/tenancy.py
--rw-r--r--   0 ahanson    (502) staff       (20)      674 2023-03-03 19:29:05.000000 netbox_python-0.1.5/netbox_python/api/users.py
--rw-r--r--   0 ahanson    (502) staff       (20)      833 2023-03-03 19:29:09.000000 netbox_python-0.1.5/netbox_python/api/virtualization.py
--rw-r--r--   0 ahanson    (502) staff       (20)      565 2023-03-03 19:29:12.000000 netbox_python-0.1.5/netbox_python/api/wireless.py
--rw-r--r--   0 ahanson    (502) staff       (20)     2260 2023-03-28 16:50:47.000000 netbox_python-0.1.5/netbox_python/baseapi.py
--rw-r--r--   0 ahanson    (502) staff       (20)       82 2023-03-02 19:10:28.000000 netbox_python-0.1.5/netbox_python/exceptions.py
--rw-r--r--   0 ahanson    (502) staff       (20)     1763 2023-03-03 19:32:40.000000 netbox_python-0.1.5/netbox_python/netbox.py
--rw-r--r--   0 ahanson    (502) staff       (20)     3614 2023-03-28 16:50:47.000000 netbox_python-0.1.5/netbox_python/rest.py
--rw-r--r--   0 ahanson    (502) staff       (20)     2564 2023-03-17 20:46:43.000000 netbox_python-0.1.5/netbox_python/test_full.py
--rw-r--r--   0 ahanson    (502) staff       (20)      368 2023-03-24 18:13:57.000000 netbox_python-0.1.5/netbox_python/testit.py
--rw-r--r--   0 ahanson    (502) staff       (20)      973 2023-03-21 14:36:18.000000 netbox_python-0.1.5/netbox_python/testit2.py
--rw-r--r--   0 ahanson    (502) staff       (20)     1161 2023-03-24 18:13:57.000000 netbox_python-0.1.5/netbox_python/testit3.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.188474 netbox_python-0.1.5/netbox_python.egg-info/
--rw-r--r--   0 ahanson    (502) staff       (20)     6476 2023-03-28 16:52:56.000000 netbox_python-0.1.5/netbox_python.egg-info/PKG-INFO
--rw-r--r--   0 ahanson    (502) staff       (20)      901 2023-03-28 16:52:56.000000 netbox_python-0.1.5/netbox_python.egg-info/SOURCES.txt
--rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-03-28 16:52:56.000000 netbox_python-0.1.5/netbox_python.egg-info/dependency_links.txt
--rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-03-03 19:00:30.000000 netbox_python-0.1.5/netbox_python.egg-info/not-zip-safe
--rw-r--r--   0 ahanson    (502) staff       (20)       22 2023-03-28 16:52:56.000000 netbox_python-0.1.5/netbox_python.egg-info/requires.txt
--rw-r--r--   0 ahanson    (502) staff       (20)       14 2023-03-28 16:52:56.000000 netbox_python-0.1.5/netbox_python.egg-info/top_level.txt
--rw-r--r--   0 ahanson    (502) staff       (20)      430 2023-03-28 16:52:56.192206 netbox_python-0.1.5/setup.cfg
--rw-r--r--   0 ahanson    (502) staff       (20)     1352 2023-03-28 16:50:47.000000 netbox_python-0.1.5/setup.py
-drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-03-28 16:52:56.191556 netbox_python-0.1.5/tests/
--rw-r--r--   0 ahanson    (502) staff       (20)       43 2023-02-27 18:27:55.000000 netbox_python-0.1.5/tests/__init__.py
--rw-r--r--   0 ahanson    (502) staff       (20)      570 2023-03-02 19:40:41.000000 netbox_python-0.1.5/tests/test_netbox_python.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.462731 netbox_python-0.1.6/
+-rw-r--r--   0 ahanson    (502) staff       (20)     3929 2023-02-27 17:19:35.000000 netbox_python-0.1.6/CONTRIBUTING.rst
+-rw-r--r--   0 ahanson    (502) staff       (20)      584 2023-02-27 16:58:50.000000 netbox_python-0.1.6/LICENSE
+-rw-r--r--   0 ahanson    (502) staff       (20)      262 2023-02-27 18:27:55.000000 netbox_python-0.1.6/MANIFEST.in
+-rw-r--r--   0 ahanson    (502) staff       (20)     6476 2023-06-08 19:17:33.462815 netbox_python-0.1.6/PKG-INFO
+-rw-r--r--   0 ahanson    (502) staff       (20)     5673 2023-03-17 17:23:36.000000 netbox_python-0.1.6/README.md
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.451694 netbox_python-0.1.6/docs/
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.453453 netbox_python-0.1.6/docs/images/
+-rw-r--r--   0 ahanson    (502) staff       (20)     6347 2023-03-03 17:12:55.000000 netbox_python-0.1.6/docs/images/screenshot.png
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.457594 netbox_python-0.1.6/netbox_python/
+-rw-r--r--   0 ahanson    (502) staff       (20)      274 2023-03-03 19:32:40.000000 netbox_python-0.1.6/netbox_python/__init__.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.461587 netbox_python-0.1.6/netbox_python/api/
+-rw-r--r--   0 ahanson    (502) staff       (20)      648 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/api/__init__.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      295 2023-04-12 23:14:00.000000 netbox_python-0.1.6/netbox_python/api/asn_range.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      822 2023-03-03 19:28:32.000000 netbox_python-0.1.6/netbox_python/api/circuits.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      372 2023-03-03 19:28:38.000000 netbox_python-0.1.6/netbox_python/api/core.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     6178 2023-06-07 17:33:27.000000 netbox_python-0.1.6/netbox_python/api/dcim.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     2289 2023-06-07 20:30:24.000000 netbox_python-0.1.6/netbox_python/api/extras.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      289 2023-04-12 23:14:00.000000 netbox_python-0.1.6/netbox_python/api/ip_range.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     2581 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/api/ipam.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      275 2023-03-03 19:28:56.000000 netbox_python-0.1.6/netbox_python/api/plugins.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      462 2023-04-12 23:14:00.000000 netbox_python-0.1.6/netbox_python/api/prefix.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      928 2023-03-03 19:29:00.000000 netbox_python-0.1.6/netbox_python/api/tenancy.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      674 2023-03-03 19:29:05.000000 netbox_python-0.1.6/netbox_python/api/users.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      833 2023-03-03 19:29:09.000000 netbox_python-0.1.6/netbox_python/api/virtualization.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      301 2023-04-12 23:14:00.000000 netbox_python-0.1.6/netbox_python/api/vlan_group.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      565 2023-03-03 19:29:12.000000 netbox_python-0.1.6/netbox_python/api/wireless.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     3040 2023-04-12 23:14:00.000000 netbox_python-0.1.6/netbox_python/baseapi.py
+-rw-r--r--   0 ahanson    (502) staff       (20)       82 2023-03-02 19:10:28.000000 netbox_python-0.1.6/netbox_python/exceptions.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     1763 2023-03-03 19:32:40.000000 netbox_python-0.1.6/netbox_python/netbox.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     3614 2023-03-28 16:50:47.000000 netbox_python-0.1.6/netbox_python/rest.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     2564 2023-03-17 20:46:43.000000 netbox_python-0.1.6/netbox_python/test_full.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      479 2023-06-08 19:12:57.000000 netbox_python-0.1.6/netbox_python/testhackathon.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     1007 2023-06-08 19:12:57.000000 netbox_python-0.1.6/netbox_python/testit.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      339 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/testit11091.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      590 2023-04-19 18:38:18.000000 netbox_python-0.1.6/netbox_python/testit11432.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      597 2023-06-08 19:13:02.000000 netbox_python-0.1.6/netbox_python/testit11513.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      364 2023-06-08 19:12:58.000000 netbox_python-0.1.6/netbox_python/testit11607.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      471 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/testit11729.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      331 2023-06-08 19:12:58.000000 netbox_python-0.1.6/netbox_python/testit12281.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      974 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/testit2.py
+-rw-r--r--   0 ahanson    (502) staff       (20)     1161 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/testit3.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      585 2023-04-12 23:14:02.000000 netbox_python-0.1.6/netbox_python/testit7503.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.458462 netbox_python-0.1.6/netbox_python.egg-info/
+-rw-r--r--   0 ahanson    (502) staff       (20)     6476 2023-06-08 19:17:33.000000 netbox_python-0.1.6/netbox_python.egg-info/PKG-INFO
+-rw-r--r--   0 ahanson    (502) staff       (20)     1255 2023-06-08 19:17:33.000000 netbox_python-0.1.6/netbox_python.egg-info/SOURCES.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-06-08 19:17:33.000000 netbox_python-0.1.6/netbox_python.egg-info/dependency_links.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)        1 2023-03-03 19:00:30.000000 netbox_python-0.1.6/netbox_python.egg-info/not-zip-safe
+-rw-r--r--   0 ahanson    (502) staff       (20)       22 2023-06-08 19:17:33.000000 netbox_python-0.1.6/netbox_python.egg-info/requires.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)       14 2023-06-08 19:17:33.000000 netbox_python-0.1.6/netbox_python.egg-info/top_level.txt
+-rw-r--r--   0 ahanson    (502) staff       (20)      430 2023-06-08 19:17:33.463199 netbox_python-0.1.6/setup.cfg
+-rw-r--r--   0 ahanson    (502) staff       (20)     1352 2023-06-08 18:44:50.000000 netbox_python-0.1.6/setup.py
+drwxr-xr-x   0 ahanson    (502) staff       (20)        0 2023-06-08 19:17:33.462498 netbox_python-0.1.6/tests/
+-rw-r--r--   0 ahanson    (502) staff       (20)       43 2023-02-27 18:27:55.000000 netbox_python-0.1.6/tests/__init__.py
+-rw-r--r--   0 ahanson    (502) staff       (20)      570 2023-03-02 19:40:41.000000 netbox_python-0.1.6/tests/test_netbox_python.py
```

### Comparing `netbox_python-0.1.5/CONTRIBUTING.rst` & `netbox_python-0.1.6/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/LICENSE` & `netbox_python-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/PKG-INFO` & `netbox_python-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox_python
-Version: 0.1.5
+Version: 0.1.6
 Summary: NetBox Python API Client
 Home-page: https://github.com/netbox-community/netbox_python
 Author: Arthur Hanson
 Author-email: ahanson@netboxlabs.com
 License: Apache Software License 2.0
 Keywords: netbox_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `netbox_python-0.1.5/README.md` & `netbox_python-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/docs/images/screenshot.png` & `netbox_python-0.1.6/docs/images/screenshot.png`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/api/circuits.py` & `netbox_python-0.1.6/netbox_python/api/circuits.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/api/dcim.py` & `netbox_python-0.1.6/netbox_python/api/dcim.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-from netbox_python.baseapi import APIResource
+from netbox_python.baseapi import APIResource, CreateableAPIResource
+from netbox_python.rest import Result
 
 
 class dcim:
     def __init__(self, client):
         self.cable_terminations = self._cable_terminations(client)
         self.cables = self._cables(client)
         self.connected_devices = self._connected_devices(client)
@@ -79,14 +80,17 @@
 
     class _device_types(APIResource):
         path = "dcim/device-types/"
 
     class _devices(APIResource):
         path = "dcim/devices/"
 
+        def render_config(self, id: str | int, *args, **kwargs) -> Result:
+            return self._create(f"{self.path}{id}/render-config/", *args, **kwargs)
+
     class _front_port_templates(APIResource):
         path = "dcim/front-port-templates/"
 
     class _front_ports(APIResource):
         path = "dcim/front-ports/"
 
     class _interface_templates(APIResource):
```

### Comparing `netbox_python-0.1.5/netbox_python/api/extras.py` & `netbox_python-0.1.6/netbox_python/api/extras.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from netbox_python.baseapi import APIResource
+from netbox_python.rest import Result
 
 
 class extras:
     def __init__(self, client):
         self.config_contexts = self._config_contexts(client)
         self.config_templates = self._config_templates(client)
         self.content_types = self._content_types(client)
@@ -22,14 +23,17 @@
 
     class _config_contexts(APIResource):
         path = "extras/config-contexts/"
 
     class _config_templates(APIResource):
         path = "extras/config-templates/"
 
+        def render(self, id: str | int, *args, **kwargs) -> Result:
+            return self._create(f"{self.path}{id}/render/", *args, **kwargs)
+
     class _content_types(APIResource):
         path = "extras/content-types/"
 
     class _custom_fields(APIResource):
         path = "extras/custom-fields/"
 
     class _custom_links(APIResource):
```

### Comparing `netbox_python-0.1.5/netbox_python/api/tenancy.py` & `netbox_python-0.1.6/netbox_python/api/tenancy.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/api/users.py` & `netbox_python-0.1.6/netbox_python/api/users.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/api/virtualization.py` & `netbox_python-0.1.6/netbox_python/api/virtualization.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/api/wireless.py` & `netbox_python-0.1.6/netbox_python/api/wireless.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/baseapi.py` & `netbox_python-0.1.6/netbox_python/baseapi.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,19 @@
 class baseapi:
     def __init__(self, client):
         self.client = client
         super().__init__()
 
 
 class CreateableAPIResource:
+    def _create(self, path, *args, **kwargs) -> Result:
+        return self.client.post(path, json=args[0] if args else kwargs)
+
     def create(self, *args, **kwargs) -> Result:
-        return self.client.post(self.path, json=args[0] if args else kwargs)
+        return self._create(self.path, *args, **kwargs)
 
 
 class DeletableAPIResource:
     def delete(self, obj: List[Any] | str | int) -> Result:
         if isinstance(obj, list):
             return self.client.delete(self.path, json=obj)
 
@@ -29,29 +32,35 @@
         while next_token:
             result = self.client.get(
                 self.path, url_override=next_token, params=result.params
             )
             yield result
             next_token = result.pagination["next"]
 
+    def _list(self, path, **kwargs) -> Result:
+        return self.client.get(path, params=kwargs)
+
     def list(self, **kwargs) -> Result:
-        return self.client.get(self.path, params=kwargs)
+        return self._list(self.path, **kwargs)
 
-    def all(self, **kwargs):
+    def _all(self, path, **kwargs):
         result = None
-        for page in self.paginate(self.client.get(self.path, params=kwargs)):
+        for page in self.paginate(self._list(path, **kwargs)):
             if not result:
                 result = page
             else:
                 result.data.extend(page.data)
 
         result.pagination["next"] = None
         result.pagination["previous"] = None
         return result
 
+    def all(self, **kwargs):
+        return self._all(self.path, **kwargs)
+
 
 class RetrievableAPIResource:
     def get(self, id: str | int) -> Result:
         return self.client.get(f"{self.path}{id}/")
 
 
 class RetrievableRootAPIResource:
@@ -82,7 +91,25 @@
     baseapi,
     DeletableAPIResource,
     ListableAPIResource,
     RetrievableAPIResource,
     UpdateableAPIResource,
 ):
     pass
+
+
+class AvailableAPIResource(
+    baseapi,
+    CreateableAPIResource,
+    ListableAPIResource,
+):
+    def create(self, id: str | int, *args, **kwargs) -> Result:
+        path = self.path.format(id=id)
+        return self._create(path, *args, **kwargs)
+
+    def list(self, id: str | int, **kwargs) -> Result:
+        path = self.path.format(id=id)
+        return self._list(path, **kwargs)
+
+    def all(self, id: str | int, **kwargs):
+        path = self.path.format(id=id)
+        return self._all(path, **kwargs)
```

### Comparing `netbox_python-0.1.5/netbox_python/netbox.py` & `netbox_python-0.1.6/netbox_python/netbox.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/rest.py` & `netbox_python-0.1.6/netbox_python/rest.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/test_full.py` & `netbox_python-0.1.6/netbox_python/test_full.py`

 * *Files identical despite different names*

### Comparing `netbox_python-0.1.5/netbox_python/testit2.py` & `netbox_python-0.1.6/netbox_python/testit2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import json
+
 from netbox import NetBoxClient
 
 nb = NetBoxClient(
     base_url="http://127.0.0.1:8000/", token="1dc6fa5bfcef8390dd83a261c36ed8f1551b2d6b"
 )
 
 # 1. List (paginated)
```

### Comparing `netbox_python-0.1.5/netbox_python/testit3.py` & `netbox_python-0.1.6/netbox_python/testit3.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 
-from netbox import NetBoxClient
 import pynetbox
+from netbox import NetBoxClient
 
 nb = NetBoxClient(
     base_url="http://127.0.0.1:8000/", token="1dc6fa5bfcef8390dd83a261c36ed8f1551b2d6b"
 )
 
 pynb = pynetbox.api(
     "http://127.0.0.1:8000/", token="1dc6fa5bfcef8390dd83a261c36ed8f1551b2d6b"
```

### Comparing `netbox_python-0.1.5/netbox_python.egg-info/PKG-INFO` & `netbox_python-0.1.6/netbox_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-python
-Version: 0.1.5
+Version: 0.1.6
 Summary: NetBox Python API Client
 Home-page: https://github.com/netbox-community/netbox_python
 Author: Arthur Hanson
 Author-email: ahanson@netboxlabs.com
 License: Apache Software License 2.0
 Keywords: netbox_python
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `netbox_python-0.1.5/netbox_python.egg-info/SOURCES.txt` & `netbox_python-0.1.6/netbox_python.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -7,29 +7,41 @@
 docs/images/screenshot.png
 netbox_python/__init__.py
 netbox_python/baseapi.py
 netbox_python/exceptions.py
 netbox_python/netbox.py
 netbox_python/rest.py
 netbox_python/test_full.py
+netbox_python/testhackathon.py
 netbox_python/testit.py
+netbox_python/testit11091.py
+netbox_python/testit11432.py
+netbox_python/testit11513.py
+netbox_python/testit11607.py
+netbox_python/testit11729.py
+netbox_python/testit12281.py
 netbox_python/testit2.py
 netbox_python/testit3.py
+netbox_python/testit7503.py
 netbox_python.egg-info/PKG-INFO
 netbox_python.egg-info/SOURCES.txt
 netbox_python.egg-info/dependency_links.txt
 netbox_python.egg-info/not-zip-safe
 netbox_python.egg-info/requires.txt
 netbox_python.egg-info/top_level.txt
 netbox_python/api/__init__.py
+netbox_python/api/asn_range.py
 netbox_python/api/circuits.py
 netbox_python/api/core.py
 netbox_python/api/dcim.py
 netbox_python/api/extras.py
+netbox_python/api/ip_range.py
 netbox_python/api/ipam.py
 netbox_python/api/plugins.py
+netbox_python/api/prefix.py
 netbox_python/api/tenancy.py
 netbox_python/api/users.py
 netbox_python/api/virtualization.py
+netbox_python/api/vlan_group.py
 netbox_python/api/wireless.py
 tests/__init__.py
 tests/test_netbox_python.py
```

### Comparing `netbox_python-0.1.5/setup.py` & `netbox_python-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,10 +38,10 @@
     include_package_data=True,
     keywords="netbox_python",
     name="netbox_python",
     packages=find_packages(include=["netbox_python", "netbox_python.*"]),
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/netbox-community/netbox_python",
-    version="0.1.5",
+    version="0.1.6",
     zip_safe=False,
 )
```

### Comparing `netbox_python-0.1.5/tests/test_netbox_python.py` & `netbox_python-0.1.6/tests/test_netbox_python.py`

 * *Files identical despite different names*

