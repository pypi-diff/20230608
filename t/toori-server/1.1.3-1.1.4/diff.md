# Comparing `tmp/toori-server-1.1.3.tar.gz` & `tmp/toori-server-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/toori-server-1.1.3.tar", last modified: Mon Jan 30 12:27:48 2023, max compression
+gzip compressed data, was "dist/toori-server-1.1.4.tar", last modified: Thu Jun  8 05:04:09 2023, max compression
```

## Comparing `toori-server-1.1.3.tar` & `toori-server-1.1.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:27:48.000000 toori-server-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-30 12:27:48.000000 toori-server-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-01-30 12:27:36.000000 toori-server-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:27:48.000000 toori-server-1.1.3/iro/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-01-30 12:27:36.000000 toori-server-1.1.3/iro/console.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-01-30 12:27:36.000000 toori-server-1.1.3/iro/main.cpp
--rw-r--r--   0 runner    (1001) docker     (123)     5248 2023-01-30 12:27:36.000000 toori-server-1.1.3/iro/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-01-30 12:27:36.000000 toori-server-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-30 12:27:48.000000 toori-server-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-01-30 12:27:36.000000 toori-server-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1642 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-01-30 12:27:48.000000 toori-server-1.1.3/toori_server.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:04:09.000000 toori-server-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 05:04:09.000000 toori-server-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-06-08 05:03:54.000000 toori-server-1.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:04:09.000000 toori-server-1.1.4/iro/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-06-08 05:03:54.000000 toori-server-1.1.4/iro/console.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-08 05:03:54.000000 toori-server-1.1.4/iro/main.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-08 05:03:54.000000 toori-server-1.1.4/iro/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 05:03:54.000000 toori-server-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 05:04:09.000000 toori-server-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-06-08 05:03:54.000000 toori-server-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2666 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-08 05:04:09.000000 toori-server-1.1.4/toori_server.egg-info/top_level.txt
```

### Comparing `toori-server-1.1.3/PKG-INFO` & `toori-server-1.1.4/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,77 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.3
+Version: 1.1.4
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
-        [![PyPI Release](https://github.com/kokseen1/Iro/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/Iro/actions/workflows/release.yml)
+        [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
+        [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
         [![PyPI Version](https://img.shields.io/pypi/v/toori-server.svg)](https://pypi.python.org/pypi/toori-server/)
         
         Server for a minimal layer 3 tunnel over http(s).
         
-        ## Prerequisites
+        ## Deploying with Docker
         
-        - [Libtins](http://libtins.github.io/download/) (optional, will fallback to Scapy (slow) if not installed)
+        Instead of installing toori-server on the host, it can be deployed as a Docker container with much convenience.
         
-        ### RST Packets
+        Pull from GHCR:
         
-        Because the Linux kernel sends a `RST` to connections it did not establish, use the following command to ensure that outgoing packets are sent successfully:
+        ```shell
+        sudo docker pull ghcr.io/kokseen1/toori-server:latest
+        ```
+        
+        Run the container:
         
         ```shell
-        sudo iptables -A OUTPUT -p tcp --tcp-flags RST RST -s <local address> -j DROP
+        sudo docker run -d --cap-add=NET_ADMIN -p 80:80 ghcr.io/kokseen1/toori-server
         ```
         
-        [See here](https://stackoverflow.com/questions/9058052/unwanted-rst-tcp-packet-with-scapy) for more information.
+        #### HTTPS
+        
+        To deploy with HTTPS, run the container with a bind mount and pass the port and certs directory as arguments:
+        
+        ```shell
+        sudo docker run -d -v /etc/letsencrypt:/etc/letsencrypt --cap-add=NET_ADMIN -p 443:443 ghcr.io/kokseen1/toori-server 443 /etc/letsencrypt/live/toori.server/
+        ```
         
         ## Installation
         
         ```shell
         pip3 install toori-server --no-binary :all:
         ```
         
+        ## Prerequisites
+        
+        - [Libtins](http://libtins.github.io/download/) (optional, will fallback to Scapy (slow) if not installed)
+        
+        ### RST Packets
+        
+        Because the Linux kernel sends a `RST` to connections it did not establish, use the following command to ensure that outgoing packets are sent successfully:
+        
+        ```shell
+        sudo iptables -A OUTPUT -p tcp --tcp-flags RST RST -s <local address> -j DROP
+        ```
+        
+        [See here](https://stackoverflow.com/questions/9058052/unwanted-rst-tcp-packet-with-scapy) for more information.
+        
         ## Usage
         
         Run with root permissions:
         
         ```shell
         iro <port>
         ```
         
         Example with HTTPS:
         
         ```shell
         iro 443 -c "/etc/letsencrypt/live/toori.server/"
         ```
         
+        
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `toori-server-1.1.3/iro/main.py` & `toori-server-1.1.4/iro/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,19 +8,21 @@
     conf,
     IP,
     TCP,
     UDP,
 )
 import asyncio
 from sanic import Sanic
+import urllib.request
 
 from engineio.payload import Payload
 
 Payload.max_decode_packets = 2500000
 
+PUBLIC_IP = urllib.request.urlopen('https://checkip.amazonaws.com').read().decode('utf8')
 LOCAL_IP = get_if_addr(conf.iface)
 conf.layers.filter([IP, TCP, UDP])
 
 app = Sanic("Iro")
 app.config["CORS_SUPPORTS_CREDENTIALS"] = True
 
 sio = socketio.AsyncServer(async_mode="sanic", cors_allowed_origins=[])
@@ -70,14 +72,17 @@
         pkt.src = virtual_ip_map.get((pkt.src, sid))
         pkt.dst, target_sid = vtarget
         await sio.emit("in", bytes(pkt), to=target_sid)
         return
 
     if pkt.haslayer(TCP) or pkt.haslayer(UDP):
 
+        if pkt.dst == PUBLIC_IP:
+            pkt.dst = LOCAL_IP
+
         # Check if existing mapping exists
         # For O(1) lookup for existing connections instead of using the loop below
         fake_sport = forward_nat.get((pkt.sport, sid, pkt.dst, pkt.dport))
 
         if fake_sport is None:
             decrement = False
             # New first-time connection
```

### Comparing `toori-server-1.1.3/setup.py` & `toori-server-1.1.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Available at setup time due to pyproject.toml
 from pybind11.setup_helpers import Pybind11Extension, build_ext
 from setuptools import setup
 import pathlib
 import subprocess
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
 
 # The main interface is through Pybind11Extension.
 # * You can add cxx_std=11/14/17, and then build_ext can be removed.
 # * You can set include_pybind11=false to add the include directory yourself,
 #   say from a submodule.
 #
 # Note:
```

### Comparing `toori-server-1.1.3/toori_server.egg-info/PKG-INFO` & `toori-server-1.1.4/toori_server.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,50 +1,77 @@
 Metadata-Version: 2.1
 Name: toori-server
-Version: 1.1.3
+Version: 1.1.4
 Summary: Server for a minimal layer 3 tunnel over http(s).
 Home-page: https://github.com/kokseen1/Iro
 License: UNKNOWN
 Description: # Iro 
         
-        [![PyPI Release](https://github.com/kokseen1/Iro/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/Iro/actions/workflows/release.yml)
+        [![GHCR](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/ghcr.yml)
+        [![PyPI Release](https://github.com/kokseen1/toori-server/actions/workflows/release.yml/badge.svg)](https://github.com/kokseen1/toori-server/actions/workflows/release.yml)
         [![PyPI Version](https://img.shields.io/pypi/v/toori-server.svg)](https://pypi.python.org/pypi/toori-server/)
         
         Server for a minimal layer 3 tunnel over http(s).
         
-        ## Prerequisites
+        ## Deploying with Docker
         
-        - [Libtins](http://libtins.github.io/download/) (optional, will fallback to Scapy (slow) if not installed)
+        Instead of installing toori-server on the host, it can be deployed as a Docker container with much convenience.
         
-        ### RST Packets
+        Pull from GHCR:
         
-        Because the Linux kernel sends a `RST` to connections it did not establish, use the following command to ensure that outgoing packets are sent successfully:
+        ```shell
+        sudo docker pull ghcr.io/kokseen1/toori-server:latest
+        ```
+        
+        Run the container:
         
         ```shell
-        sudo iptables -A OUTPUT -p tcp --tcp-flags RST RST -s <local address> -j DROP
+        sudo docker run -d --cap-add=NET_ADMIN -p 80:80 ghcr.io/kokseen1/toori-server
         ```
         
-        [See here](https://stackoverflow.com/questions/9058052/unwanted-rst-tcp-packet-with-scapy) for more information.
+        #### HTTPS
+        
+        To deploy with HTTPS, run the container with a bind mount and pass the port and certs directory as arguments:
+        
+        ```shell
+        sudo docker run -d -v /etc/letsencrypt:/etc/letsencrypt --cap-add=NET_ADMIN -p 443:443 ghcr.io/kokseen1/toori-server 443 /etc/letsencrypt/live/toori.server/
+        ```
         
         ## Installation
         
         ```shell
         pip3 install toori-server --no-binary :all:
         ```
         
+        ## Prerequisites
+        
+        - [Libtins](http://libtins.github.io/download/) (optional, will fallback to Scapy (slow) if not installed)
+        
+        ### RST Packets
+        
+        Because the Linux kernel sends a `RST` to connections it did not establish, use the following command to ensure that outgoing packets are sent successfully:
+        
+        ```shell
+        sudo iptables -A OUTPUT -p tcp --tcp-flags RST RST -s <local address> -j DROP
+        ```
+        
+        [See here](https://stackoverflow.com/questions/9058052/unwanted-rst-tcp-packet-with-scapy) for more information.
+        
         ## Usage
         
         Run with root permissions:
         
         ```shell
         iro <port>
         ```
         
         Example with HTTPS:
         
         ```shell
         iro 443 -c "/etc/letsencrypt/live/toori.server/"
         ```
         
+        
+        
 Platform: UNKNOWN
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

