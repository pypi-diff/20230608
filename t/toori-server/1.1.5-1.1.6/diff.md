# Comparing `tmp/toori-server-1.1.5.tar.gz` & `tmp/toori-server-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toori-server-1.1.5.tar", last modified: Thu Jun  8 05:15:15 2023, max compression
+gzip compressed data, was "dist/toori-server-1.1.6.tar", last modified: Thu Jun  8 07:23:07 2023, max compression
```

## Comparing `toori-server-1.1.5.tar` & `toori-server-1.1.6.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:15:15.000000 toori-server-1.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 05:15:15.000000 toori-server-1.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-08 05:15:05.000000 toori-server-1.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:15:15.000000 toori-server-1.1.5/iro/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 05:15:05.000000 toori-server-1.1.5/iro/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 05:15:05.000000 toori-server-1.1.5/iro/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5433 2023-06-08 05:15:05.000000 toori-server-1.1.5/iro/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 05:15:05.000000 toori-server-1.1.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 05:15:15.000000 toori-server-1.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 05:15:05.000000 toori-server-1.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 05:15:15.000000 toori-server-1.1.5/toori_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:23:07.000000 toori-server-1.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 07:23:07.000000 toori-server-1.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-08 07:22:56.000000 toori-server-1.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:23:07.000000 toori-server-1.1.6/iro/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 07:22:56.000000 toori-server-1.1.6/iro/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 07:22:56.000000 toori-server-1.1.6/iro/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5702 2023-06-08 07:22:56.000000 toori-server-1.1.6/iro/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 07:22:56.000000 toori-server-1.1.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 07:23:07.000000 toori-server-1.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 07:22:56.000000 toori-server-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 07:23:07.000000 toori-server-1.1.6/toori_server.egg-info/top_level.txt
```

### Comparing `toori-server-1.1.5/PKG-INFO` & `toori-server-1.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.5
+Version: 1.1.6
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
         [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
         [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
```

### Comparing `toori-server-1.1.5/README.md` & `toori-server-1.1.6/README.md`

 * *Files identical despite different names*

### Comparing `toori-server-1.1.5/iro/main.py` & `toori-server-1.1.6/iro/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,22 +8,33 @@
     conf,
     IP,
     TCP,
     UDP,
 )
 import asyncio
 from sanic import Sanic
+
 import urllib.request
+import netifaces as ni
 
 from engineio.payload import Payload
 
 Payload.max_decode_packets = 2500000
 
 PUBLIC_IP = urllib.request.urlopen('https://checkip.amazonaws.com').read().decode('utf8').strip()
 LOCAL_IP = get_if_addr(conf.iface)
+
+if PUBLIC_IP == LOCAL_IP:
+    default_interface = ni.gateways()["default"][ni.AF_INET][1]
+    addrs = {d['addr'] for d in ni.ifaddresses(default_interface)[ni.AF_INET]}
+    addrs.remove(PUBLIC_IP)
+
+    if addrs:
+        LOCAL_IP = addrs.pop()
+
 conf.layers.filter([IP, TCP, UDP])
 
 app = Sanic("Iro")
 app.config["CORS_SUPPORTS_CREDENTIALS"] = True
 
 sio = socketio.AsyncServer(async_mode="sanic", cors_allowed_origins=[])
 sio.attach(app)
```

### Comparing `toori-server-1.1.5/setup.py` & `toori-server-1.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 import pathlib
 import subprocess
 
-__version__ = "1.1.5"
+__version__ = "1.1.6"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `toori-server-1.1.5/toori_server.egg-info/PKG-INFO` & `toori-server-1.1.6/toori_server.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.5
+Version: 1.1.6
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
         [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
         [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
```

