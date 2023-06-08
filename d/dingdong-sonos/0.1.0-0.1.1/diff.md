# Comparing `tmp/dingdong_sonos-0.1.0.tar.gz` & `tmp/dingdong_sonos-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dingdong_sonos-0.1.0.tar", last modified: Thu Jun  8 13:41:25 2023, max compression
+gzip compressed data, was "dingdong_sonos-0.1.1.tar", last modified: Thu Jun  8 14:15:15 2023, max compression
```

## Comparing `dingdong_sonos-0.1.0.tar` & `dingdong_sonos-0.1.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 13:41:25.631973 dingdong_sonos-0.1.0/
--rw-r--r--   0 tim        (501) staff       (20)       30 2023-06-08 13:35:24.000000 dingdong_sonos-0.1.0/MANIFEST.in
--rw-r--r--   0 tim        (501) staff       (20)      668 2023-06-08 13:41:25.631411 dingdong_sonos-0.1.0/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)       10 2023-06-08 13:41:12.000000 dingdong_sonos-0.1.0/README.md
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 13:41:25.622091 dingdong_sonos-0.1.0/dingdong_sonos/
--rw-r--r--   0 tim        (501) staff       (20)        0 2023-06-08 13:27:50.000000 dingdong_sonos-0.1.0/dingdong_sonos/__init__.py
--rw-r--r--   0 tim        (501) staff       (20)     2117 2023-06-08 13:28:02.000000 dingdong_sonos-0.1.0/dingdong_sonos/main.py
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 13:41:25.628933 dingdong_sonos-0.1.0/dingdong_sonos/media/
--rw-r--r--   0 tim        (501) staff       (20)    49210 2023-06-08 13:07:14.000000 dingdong_sonos-0.1.0/dingdong_sonos/media/school-bell-sound.mov
--rw-r--r--   0 tim        (501) staff       (20)    81465 2023-06-08 13:08:24.000000 dingdong_sonos-0.1.0/dingdong_sonos/media/school-bell-sound.mp3
-drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 13:41:25.626389 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/
--rw-r--r--   0 tim        (501) staff       (20)      668 2023-06-08 13:41:25.000000 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/PKG-INFO
--rw-r--r--   0 tim        (501) staff       (20)      402 2023-06-08 13:41:25.000000 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/SOURCES.txt
--rw-r--r--   0 tim        (501) staff       (20)        1 2023-06-08 13:41:25.000000 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/dependency_links.txt
--rw-r--r--   0 tim        (501) staff       (20)       54 2023-06-08 13:41:25.000000 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/entry_points.txt
--rw-r--r--   0 tim        (501) staff       (20)       47 2023-06-08 13:41:25.000000 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/requires.txt
--rw-r--r--   0 tim        (501) staff       (20)       15 2023-06-08 13:41:25.000000 dingdong_sonos-0.1.0/dingdong_sonos.egg-info/top_level.txt
--rw-r--r--   0 tim        (501) staff       (20)     1110 2023-06-08 13:41:02.000000 dingdong_sonos-0.1.0/pyproject.toml
--rw-r--r--   0 tim        (501) staff       (20)       38 2023-06-08 13:41:25.632103 dingdong_sonos-0.1.0/setup.cfg
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 14:15:15.935455 dingdong_sonos-0.1.1/
+-rw-r--r--   0 tim        (501) staff       (20)       30 2023-06-08 13:35:24.000000 dingdong_sonos-0.1.1/MANIFEST.in
+-rw-r--r--   0 tim        (501) staff       (20)     1051 2023-06-08 14:15:15.934704 dingdong_sonos-0.1.1/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)      393 2023-06-08 14:11:53.000000 dingdong_sonos-0.1.1/README.md
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 14:15:15.915725 dingdong_sonos-0.1.1/dingdong_sonos/
+-rw-r--r--   0 tim        (501) staff       (20)        0 2023-06-08 13:27:50.000000 dingdong_sonos-0.1.1/dingdong_sonos/__init__.py
+-rw-r--r--   0 tim        (501) staff       (20)     2733 2023-06-08 14:14:09.000000 dingdong_sonos-0.1.1/dingdong_sonos/main.py
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 14:15:15.932814 dingdong_sonos-0.1.1/dingdong_sonos/media/
+-rw-r--r--   0 tim        (501) staff       (20)    49210 2023-06-08 13:07:14.000000 dingdong_sonos-0.1.1/dingdong_sonos/media/school-bell-sound.mov
+-rw-r--r--   0 tim        (501) staff       (20)    81465 2023-06-08 13:08:24.000000 dingdong_sonos-0.1.1/dingdong_sonos/media/school-bell-sound.mp3
+drwxr-xr-x   0 tim        (501) staff       (20)        0 2023-06-08 14:15:15.928625 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/
+-rw-r--r--   0 tim        (501) staff       (20)     1051 2023-06-08 14:15:15.000000 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/PKG-INFO
+-rw-r--r--   0 tim        (501) staff       (20)      402 2023-06-08 14:15:15.000000 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/SOURCES.txt
+-rw-r--r--   0 tim        (501) staff       (20)        1 2023-06-08 14:15:15.000000 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/dependency_links.txt
+-rw-r--r--   0 tim        (501) staff       (20)       54 2023-06-08 14:15:15.000000 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/entry_points.txt
+-rw-r--r--   0 tim        (501) staff       (20)       47 2023-06-08 14:15:15.000000 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/requires.txt
+-rw-r--r--   0 tim        (501) staff       (20)       15 2023-06-08 14:15:15.000000 dingdong_sonos-0.1.1/dingdong_sonos.egg-info/top_level.txt
+-rw-r--r--   0 tim        (501) staff       (20)     1110 2023-06-08 14:14:59.000000 dingdong_sonos-0.1.1/pyproject.toml
+-rw-r--r--   0 tim        (501) staff       (20)       38 2023-06-08 14:15:15.936524 dingdong_sonos-0.1.1/setup.cfg
```

### Comparing `dingdong_sonos-0.1.0/dingdong_sonos/main.py` & `dingdong_sonos-0.1.1/dingdong_sonos/main.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
-import click
 import os
-from soco import SoCo
-from soco.data_structures import DidlMusicTrack, DidlResource
-import subprocess
 import socket
+import subprocess
+import sys
 import time
 
+import click
+import soco
+from soco import SoCo
+from soco.data_structures import DidlMusicTrack, DidlResource
+
 
 def get_local_ip():
     s = socket.socket(socket.AF_INET, socket.SOCK_DGRAM)
     try:
         # doesn't need to be reachable, this just gets the IP of the preferred outbound socket
         s.connect(("8.8.8.8", 80))
         local_ip = s.getsockname()[0]
@@ -17,37 +20,61 @@
         s.close()
     return local_ip
 
 
 def start_http_server(port="8001"):
     media_folder = os.path.join(os.path.dirname(__file__), "media")
     httpserver = subprocess.Popen(
-        ["python", "-m", "http.server", str(port)], cwd=media_folder
+        [sys.executable, "-m", "http.server", str(port)], cwd=media_folder
     )
     return httpserver
 
 
+def group_all_sonos():
+    # Discover all Sonos speakers
+    speakers = list(soco.discover())
+
+    # Get the first speaker as the coordinator
+    coordinator = speakers[0]
+
+    # Join all other speakers to the coordinator
+    for speaker in speakers[1:]:
+        speaker.join(coordinator)
+
+    # Print the group information
+    print("Sonos speakers grouped successfully.")
+
+
 @click.command()
-@click.argument("sonos_ip")
+@click.option(
+    "--sonos_ip",
+    default=None,
+    help="IP address of the Sonos speaker, default is to us ALL speakers",
+)
 @click.option("--port", default="8001", help="Port to run the HTTP server on")
-@click.option("--volume", default=5, help="Volume to play the sound at")
+@click.option("--volume", default=60, help="Volume to play the sound at")
 def main(sonos_ip, port, volume):
     # Get the IP of this machine in the local network
     host_address = f"{get_local_ip()}:{port}"
 
     # Specify the path to the MP3 file on your computer
     path_to_mp3 = f"http://{host_address}/school-bell-sound.mp3"
 
     # Specify the IP address of the Sonos speaker
 
     # Start the HTTP server
     httpserver = start_http_server(port)
 
-    # Create a SoCo instance
-    sonos = SoCo(sonos_ip)
+    if sonos_ip:
+        sonos = SoCo(sonos_ip)
+        sonos.volume = volume
+    else:
+        group_all_sonos()
+        sonos = list(soco.discover())[0]
+        sonos.group.volume = volume
 
     # Create a Resource object for the MP3 file
     mp3_resource = DidlResource(
         uri=path_to_mp3, protocol_info="http-get:*:audio/mpeg:*"
     )
 
     # Create a DidlMusicTrack object for the MP3 file
@@ -60,15 +87,14 @@
 
     # Clear the queue
     sonos.clear_queue()
 
     # Add the MP3 file to the Sonos speaker's queue
     sonos.add_to_queue(mp3_item)
 
-    sonos.volume = volume
     # Play the queue (i.e., the MP3 file we just added)
     sonos.play_from_queue(0)
 
     # wait 3 seconds
     time.sleep(3)
 
     # Stop the HTTP server
```

### Comparing `dingdong_sonos-0.1.0/dingdong_sonos/media/school-bell-sound.mov` & `dingdong_sonos-0.1.1/dingdong_sonos/media/school-bell-sound.mov`

 * *Files identical despite different names*

### Comparing `dingdong_sonos-0.1.0/dingdong_sonos/media/school-bell-sound.mp3` & `dingdong_sonos-0.1.1/dingdong_sonos/media/school-bell-sound.mp3`

 * *Files identical despite different names*

### Comparing `dingdong_sonos-0.1.0/pyproject.toml` & `dingdong_sonos-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 
 [project]
 name = "dingdong_sonos"
-version = "0.1.0"
+version = "0.1.1"
 description = "Ring the Gong"
 readme = "README.md"
 authors = [{name = "Tim Rohner", email = "info@timrohner.ch"}]
 keywords = ["dingdong_sonos"]
 # homepage = "https://github.com/leokster/dingdong_sonos"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
```

