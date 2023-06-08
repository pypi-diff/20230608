# Comparing `tmp/duplocloud-client-0.0.8.tar.gz` & `tmp/duplocloud-client-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "duplocloud-client-0.0.8.tar", last modified: Tue May  9 17:24:38 2023, max compression
+gzip compressed data, was "duplocloud-client-0.0.9.tar", last modified: Thu Jun  8 17:55:20 2023, max compression
```

## Comparing `duplocloud-client-0.0.8.tar` & `duplocloud-client-0.0.9.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.238013 duplocloud-client-0.0.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)      857 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/dev-requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.238013 duplocloud-client-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/src/duplo_resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/tenant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplo_resource/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/src/duplocloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-09 17:24:02.000000 duplocloud-client-0.0.8/src/duplocloud/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-09 17:24:38.242013 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      695 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      715 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-09 17:24:38.000000 duplocloud-client-0.0.8/src/duplocloud_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.339079 duplocloud-client-0.0.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)      857 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/dev-requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.339079 duplocloud-client-0.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/src/duplo_resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplo_resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2102 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplo_resource/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplo_resource/tenant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplo_resource/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/src/duplocloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplocloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplocloud/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplocloud/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplocloud/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplocloud/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 17:54:38.000000 duplocloud-client-0.0.9/src/duplocloud/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 17:55:20.343079 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      695 2023-06-08 17:55:20.000000 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      715 2023-06-08 17:55:20.000000 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 17:55:20.000000 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-08 17:55:20.000000 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 17:55:20.000000 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-08 17:55:20.000000 duplocloud-client-0.0.9/src/duplocloud_client.egg-info/top_level.txt
```

### Comparing `duplocloud-client-0.0.8/.github/workflows/publish.yaml` & `duplocloud-client-0.0.9/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/.github/workflows/test.yml` & `duplocloud-client-0.0.9/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/CONTRIBUTING.md` & `duplocloud-client-0.0.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/PKG-INFO` & `duplocloud-client-0.0.9/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.8/setup.cfg` & `duplocloud-client-0.0.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/src/duplo_resource/service.py` & `duplocloud-client-0.0.9/src/duplo_resource/service.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/src/duplo_resource/tenant.py` & `duplocloud-client-0.0.9/src/duplo_resource/tenant.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/src/duplo_resource/user.py` & `duplocloud-client-0.0.9/src/duplo_resource/user.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/src/duplocloud/cli.py` & `duplocloud-client-0.0.9/src/duplocloud/cli.py`

 * *Files identical despite different names*

### Comparing `duplocloud-client-0.0.8/src/duplocloud/client.py` & `duplocloud-client-0.0.9/src/duplocloud/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 
 import requests
+import json
 from cachetools import cached, TTLCache
 from importlib.metadata import entry_points
 
 ENTRYPOINT="duplocloud.net"
 
 class DuploClient():
   """Duplo Client
@@ -84,8 +85,18 @@
     Returns:
       The instantiated service with a reference to this client.
     """
     eps = entry_points()[ENTRYPOINT]
     # e = entry_points(group=group, name=kind)
     e = [ep for ep in eps if ep.name == name][0]
     svc = e.load() 
-    return svc(self)
+    return svc(self)
+  
+  def json(self, data):
+    """Convert data to JSON.
+    
+    Args:
+      data: The data to convert.
+    Returns:
+      The data as a JSON object.
+    """
+    return json.dumps(data)
```

### Comparing `duplocloud-client-0.0.8/src/duplocloud/resource.py` & `duplocloud-client-0.0.9/src/duplocloud/resource.py`

 * *Files 26% similar despite different names*

```diff
@@ -13,10 +13,16 @@
       self.tenant = self.tenant_svc.find(self.duplo.tenant_name)
     return self.tenant
   
   def exec(self, subcmd, args=[]):
     if not (func := getattr(self, subcmd, None)):
       raise ValueError(f"Invalid subcommand: {subcmd}")
     try:
-      return print(func(*args))
+      res = func(*args)
+      # if res is a dict or list, turn it into json
+      if isinstance(res, (dict, list)):
+        res = self.duplo.json(res)
+      return print(res)
     except Exception as e:
       raise DuploError(f"Error executing subcommand: {subcmd}") from e
+    
+
```

### Comparing `duplocloud-client-0.0.8/src/duplocloud_client.egg-info/PKG-INFO` & `duplocloud-client-0.0.9/src/duplocloud_client.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: duplocloud-client
-Version: 0.0.8
+Version: 0.0.9
 Summary: Generic DuploClient for Python apps.
 Home-page: https://github.com/duplocloud/py-client
 Author: Kelly Ferrone
 Author-email: kelly@duplocloud.net
 Project-URL: Bug Tracker, https://github.com/duplocloud/py-client/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `duplocloud-client-0.0.8/src/duplocloud_client.egg-info/SOURCES.txt` & `duplocloud-client-0.0.9/src/duplocloud_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

