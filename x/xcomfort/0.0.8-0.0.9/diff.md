# Comparing `tmp/xcomfort-0.0.8.tar.gz` & `tmp/xcomfort-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/xcomfort-0.0.8.tar", last modified: Mon Jul  6 18:32:16 2020, max compression
+gzip compressed data, was "dist/xcomfort-0.0.9.tar", last modified: Fri Jul 17 10:58:18 2020, max compression
```

## Comparing `xcomfort-0.0.8.tar` & `xcomfort-0.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-06 18:32:16.107048 xcomfort-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-06 18:32:16.107048 xcomfort-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      709 2020-07-06 18:32:00.000000 xcomfort-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-06 18:32:16.107048 xcomfort-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      712 2020-07-06 18:32:00.000000 xcomfort-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-06 18:32:16.107048 xcomfort-0.0.8/xcomfort/
--rw-r--r--   0 runner    (1001) docker     (116)       54 2020-07-06 18:32:00.000000 xcomfort-0.0.8/xcomfort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3915 2020-07-06 18:32:00.000000 xcomfort-0.0.8/xcomfort/bridge.py
--rw-r--r--   0 runner    (1001) docker     (116)     7266 2020-07-06 18:32:00.000000 xcomfort-0.0.8/xcomfort/connection.py
--rw-r--r--   0 runner    (1001) docker     (116)      921 2020-07-06 18:32:00.000000 xcomfort-0.0.8/xcomfort/devices.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-06 18:32:16.107048 xcomfort-0.0.8/xcomfort.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-06 18:32:15.000000 xcomfort-0.0.8/xcomfort.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      229 2020-07-06 18:32:16.000000 xcomfort-0.0.8/xcomfort.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-06 18:32:15.000000 xcomfort-0.0.8/xcomfort.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)        9 2020-07-06 18:32:15.000000 xcomfort-0.0.8/xcomfort.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 10:58:18.565326 xcomfort-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-17 10:58:18.565326 xcomfort-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      709 2020-07-17 10:58:09.000000 xcomfort-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2020-07-17 10:58:18.565326 xcomfort-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      712 2020-07-17 10:58:09.000000 xcomfort-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 10:58:18.565326 xcomfort-0.0.9/xcomfort/
+-rw-r--r--   0 runner    (1001) docker     (116)       54 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3915 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/bridge.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7322 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/connection.py
+-rw-r--r--   0 runner    (1001) docker     (116)      921 2020-07-17 10:58:09.000000 xcomfort-0.0.9/xcomfort/devices.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-07-17 10:58:18.565326 xcomfort-0.0.9/xcomfort.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1480 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      229 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        9 2020-07-17 10:58:18.000000 xcomfort-0.0.9/xcomfort.egg-info/top_level.txt
```

### Comparing `xcomfort-0.0.8/PKG-INFO` & `xcomfort-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcomfort
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration with Eaton xComfort Bridge
 Home-page: https://github.com/jankrib/xcomfort-python
 Author: Jan Kristian Bjerke
 Author-email: jan.bjerke@gmail.com
 License: UNKNOWN
 Description: # xcomfort-python
         Unofficial python package for communicating with Eaton xComfort Bridge
```

### Comparing `xcomfort-0.0.8/README.md` & `xcomfort-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `xcomfort-0.0.8/setup.py` & `xcomfort-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="xcomfort",
-    version="0.0.8",
+    version="0.0.9",
     author="Jan Kristian Bjerke",
     author_email="jan.bjerke@gmail.com",
     description="Integration with Eaton xComfort Bridge",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jankrib/xcomfort-python",
     packages=setuptools.find_packages(),
```

### Comparing `xcomfort-0.0.8/xcomfort/bridge.py` & `xcomfort-0.0.9/xcomfort/bridge.py`

 * *Files identical despite different names*

### Comparing `xcomfort-0.0.8/xcomfort/connection.py` & `xcomfort-0.0.9/xcomfort/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         secret = b64encode(cipher.encrypt((key.hex() + ":::" + iv.hex()).encode()))
         print(f"secret: {secret}")
         secret = secret.decode()
         print(f"secret: {secret}")
 
         await __send(ws, {"type_int":16,"mc":-1,"payload":{"secret": secret}})
 
-        connection = SecureBridgeConnection(ws, key, iv)
+        connection = SecureBridgeConnection(ws, key, iv, deviceId)
 
         # Start LOGIN
 
         msg = await connection.receive()
         
         if msg['type_int'] != 17:
             raise Exception('Failed to establish secure connection')
@@ -118,18 +118,19 @@
 
         return connection
     except:
         await ws.close()
         raise
 
 class SecureBridgeConnection:
-    def __init__(self, websocket, key, iv):
+    def __init__(self, websocket, key, iv, device_id):
         self.websocket = websocket
         self.key = key
         self.iv = iv
+        self.device_id = device_id
 
         self.state = ConnectionState.Initial
         self._messageSubject = rx.subject.Subject()
         self.mc = 0
 
         self.messages = self._messageSubject.pipe(
             ops.as_observable()
```

### Comparing `xcomfort-0.0.8/xcomfort/devices.py` & `xcomfort-0.0.9/xcomfort/devices.py`

 * *Files identical despite different names*

### Comparing `xcomfort-0.0.8/xcomfort.egg-info/PKG-INFO` & `xcomfort-0.0.9/xcomfort.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xcomfort
-Version: 0.0.8
+Version: 0.0.9
 Summary: Integration with Eaton xComfort Bridge
 Home-page: https://github.com/jankrib/xcomfort-python
 Author: Jan Kristian Bjerke
 Author-email: jan.bjerke@gmail.com
 License: UNKNOWN
 Description: # xcomfort-python
         Unofficial python package for communicating with Eaton xComfort Bridge
```

