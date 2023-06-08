# Comparing `tmp/pyvoyis-1.0.2.tar.gz` & `tmp/pyvoyis-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoyis-1.0.2.tar", last modified: Thu Jun  1 16:01:15 2023, max compression
+gzip compressed data, was "pyvoyis-1.0.3.tar", last modified: Thu Jun  8 15:05:38 2023, max compression
```

## Comparing `pyvoyis-1.0.2.tar` & `pyvoyis-1.0.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:01:15.254876 pyvoyis-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-01 16:01:15.254876 pyvoyis-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 16:01:15.254876 pyvoyis-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:01:15.250875 pyvoyis-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:01:15.250875 pyvoyis-1.0.2/src/pyvoyis/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38878 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:01:15.254876 pyvoyis-1.0.2/src/pyvoyis/api500/
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/api500/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5819 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/api500/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/api500/command.py
--rw-r--r--   0 runner    (1001) docker     (123)    56612 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/api500/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/commander.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/messages.py
--rw-r--r--   0 runner    (1001) docker     (123)     2572 2023-06-01 16:01:06.000000 pyvoyis-1.0.2/src/pyvoyis/state_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 16:01:15.250875 pyvoyis-1.0.2/src/pyvoyis.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4043 2023-06-01 16:01:15.000000 pyvoyis-1.0.2/src/pyvoyis.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-01 16:01:15.000000 pyvoyis-1.0.2/src/pyvoyis.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 16:01:15.000000 pyvoyis-1.0.2/src/pyvoyis.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-01 16:01:15.000000 pyvoyis-1.0.2/src/pyvoyis.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-01 16:01:15.000000 pyvoyis-1.0.2/src/pyvoyis.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-01 16:01:15.000000 pyvoyis-1.0.2/src/pyvoyis.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/pyvoyis/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42832 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/pyvoyis/api500/
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      953 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57923 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/api500/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/commander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8111 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15669 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/messages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2600 2023-06-08 15:05:29.000000 pyvoyis-1.0.3/src/pyvoyis/state_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 15:05:38.779862 pyvoyis-1.0.3/src/pyvoyis.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2763 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-08 15:05:38.000000 pyvoyis-1.0.3/src/pyvoyis.egg-info/top_level.txt
```

### Comparing `pyvoyis-1.0.2/LICENSE` & `pyvoyis-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.2/setup.py` & `pyvoyis-1.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 # read the contents of README file
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="pyvoyis",
-    version="1.0.2",
+    version="1.0.3",
     description="Voyis Recon LS python driver",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Miquel Massot",
     author_email="miquel.massot@gmail.com",
     maintainer="Miquel Massot",
     maintainer_email="miquel.massot@gmail.com",
```

### Comparing `pyvoyis-1.0.2/src/pyvoyis/__init__.py` & `pyvoyis-1.0.3/src/pyvoyis/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.2/src/pyvoyis/api.py` & `pyvoyis-1.0.3/src/pyvoyis/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,26 +9,28 @@
 import logging
 import threading
 import time
 from pathlib import Path
 
 import nest_asyncio
 
+from pyvoyis.tools.custom_logger import setup_logging
 from pyvoyis.api500 import API500Client
 from pyvoyis.api500.defs import (
     API_PARAM_STILLS_IMAGE_SAVE_ORIGINAL,
     API_PARAM_STILLS_IMAGE_UNDISTORT,
     API_PARAM_STILLS_PROCESSED_IMAGE_FORMAT,
     ENDPOINT_ID_LOG,
     ENDPOINT_ID_SENSOR_LASER,
     ENDPOINT_ID_SENSOR_STILLS_PROCESSED,
     ENDPOINT_ID_SENSOR_STILLS_RAW,
     ENDPOINT_ID_STREAM,
     ENDPOINT_ID_XYZ_LASER,
     NAVPROTO_PSONNAV,
+    SCANNER_NOT_READY,
     SCANNER_CONNECTED_TO_THIS_API,
     SCANNER_PARAM_INDEX_OF_REFRACTION,
     SCANNER_PARAM_LASER_FREQ,
     SCANNER_PARAM_LASER_MAX_RANGE,
     SCANNER_PARAM_LASER_MIN_RANGE,
     SCANNER_PARAM_LASER_OUTPUT_GAIN,
     SCANNER_PARAM_LED_PANEL_INTENSITY,
@@ -60,14 +62,16 @@
     SCANNER_STATUS_STILLS_CAMERA_CONNECTED,
     SCANNER_STATUS_STILLS_CAMERA_READY,
     SOURCE_TCP_CLIENT,
     SOURCE_TCP_SERVER,
     VALUE_TYPE_BOOL,
     VALUE_TYPE_UINT,
     scanner_connection_to_str,
+    str_to_navproto,
+    str_to_network_source,
 )
 from pyvoyis.commander import VoyisCommander
 from pyvoyis.messages import (
     AckRsp,
     APIConfiguration,
     APIConfigurationNot,
     APIStatus,
@@ -84,49 +88,62 @@
     ScannerParameter,
     ScannerParametersNot,
     ScannerStatus,
     ScannerStatusNot,
 )
 from pyvoyis.state_machine import VoyisAPIStateMachine
 from pyvoyis.tools.bool2str import bool2str
+from pyvoyis.tools.str2bool import str2bool
 from pyvoyis.tools.rate import Rate
 from pyvoyis.tools.safe_get import safe_get
 
 nest_asyncio.apply()
 
 
 class VoyisAPI:
     def __init__(self, config):
         """Class to handle the Voyis API"""
         self.config = config
+        setup_logging(config.log_path)
+
+        print(self.config)
+
         self.ip = config.ip_address
         self.port = config.port
         self.log = logging.getLogger("VoyisAPI")
         self.event = threading.Event()
         self.task_set = set()
-        self.loop = asyncio.get_event_loop()
+
+        # Handle RuntimeError: There is no current event loop in thread 'Thread-1'.
+        try:
+            self.loop = asyncio.get_event_loop()
+        except RuntimeError as e:
+            if str(e).startswith('There is no current event loop in thread'):
+                self.loop = asyncio.new_event_loop()
+                asyncio.set_event_loop(self.loop)
+            else:
+                raise
+
         self.client = API500Client(self.ip, self.port, self.loop, self.task_set)
         self.state = VoyisAPIStateMachine()
         self.cmd = VoyisCommander()
 
+        self.last_connection_state = 0
+
         self.api_status_not_dict = {}
         self.scanner_list_not_dict = {}
         self.scanner_parameters_not_dict = {}
         self.scanner_status_not_dict = {}
         self.api_configuration_not_dict = {}
         self.endpoint_configuration_not_dict = {}
 
         self.api_version_not_list = []
         self.api_status_list = []
         self.connection_change_not_list = []
-        self.scanner_status_list = []
         self.leak_detection_not_list = []
-        self.scanner_parameter_list = []
-        self.api_configuration_list = []
-        self.endpoint_configuration_list = []
         self.correction_model_load_not_list = []
         self.correction_model_list_not_list = []
         self.pending_cmd_status_not_list = []
         self.ack_rsp_list = []
 
         self._request_acquisition = False
         self._request_stop = False
@@ -135,31 +152,35 @@
         """Request acquisition"""
         self._request_acquisition = True
 
     def request_stop(self):
         """Request stop"""
         self._request_stop = True
 
-    def send_message(self, cmd, timeout_s=6.0):
+    def send_message(self, cmd, timeout_s=10.0, retries=2, expect_ack=True):
         """Sends a message to the API500Client
 
         Parameters
         ----------
         cmd : API500Command
             Command to send
         timeout_s : float, optional
             Timeout in seconds to wait for the AckRsp, by default 6.0
 
         Returns
         -------
         bool
             True if the command was accepted, False otherwise
         """
+        if retries <= 0:
+            return False
         len_ack_before = len(self.ack_rsp_list)
         self.loop.run_until_complete(self.client.send_message(cmd.to_str()))
+        if not expect_ack: 
+            return True
         # Wait for AckRsp to be received
         timeout_start = time.time()
         while time.time() < timeout_start + timeout_s:
             if len(self.ack_rsp_list) == len_ack_before + 1:
                 break
             time.sleep(0.1)
         if len(self.ack_rsp_list) > 0:
@@ -170,14 +191,15 @@
                         cmd.command, ack_rsp.nack_error_string
                     )
                 )
             elif ack_rsp.accepted:
                 self.log.info("Command {} accepted!".format(cmd.command))
             return ack_rsp.accepted
         else:
+            self.send_message(cmd, timeout_s=timeout_s, retries=retries-1)
             return False
 
     def get_received_messages(self):
         """Get the received messages from the API500Client
 
         Returns
         -------
@@ -245,38 +267,46 @@
             success = self.perform_system_checks()
             if not success:
                 self.log.error("Could not perform system checks or some checks failed")
                 return
             success = self.stop_scanning_if_running()
             if not success:
                 self.log.error("Could not stop scanning")
-            """
             success = self.configure_time_source()
             if not success:
-                self.log.error('Could not configure time source')
+                self.log.error('Could not configure time source. Check that the IP address provided for time sync is accessible from the Voyis API PC network.')
                 return
-            """
-            """
             success = self.configure_nav()
             if not success:
-                self.log.error('Could not configure nav')
+                self.log.error('Could not configure nav. Check that the IP address provided for nav updates is accessible from the Voyis PC network.')
                 return
-            """
             success = self.set_scan_parameters()
             if not success:
                 self.log.error("Could not set scan parameters")
                 return
             success = self.check_laser_is_armed()
             if not success:
                 self.log.error("Could not check laser is armed")
                 return
             success = self.check_temperatures()
             if not success:
                 self.log.error("Could not check temperatures")
                 return
+            
+            """
+            # Do a network time sync
+            self.cmd.network_time_sync.payload = {
+                "microseconds_since_epoch": int(time.time()*1e6)
+            }
+            success = self.send_message(self.cmd.network_time_sync)
+            if not success:
+                self.log.error("Could not sync network time")
+                return
+            """
+
             self.state.ready()
         if self.state.is_readying and self._request_acquisition:
             self._request_acquisition = False
             self.state.request_acquisition()
         elif self.state.is_requesting_acquisition:
             success = self.start_scanning()
             if not success:
@@ -299,15 +329,15 @@
         elif self.state.is_stopping:
             self.state.disconnect()
         elif self.state.is_disconnecting:
             success = self.disconnect()
             if not success:
                 self.log.error("Could not disconnect")
                 return
-            self.state.idle()
+            self.state.idling()
 
     def run(self):
         """Main function to run the API client"""
         self.asyncio_thread = threading.Thread(target=self.asyncio_thread_fn)
         self.asyncio_thread.start()
 
         # Prepare a background thread to listen to the API and keep it alive
@@ -355,23 +385,51 @@
 
         Returns
         -------
         bool
             True if the connection was successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Connecting to scanner...")
+        success = self.send_message(self.cmd.list_scanners)
+        if not success:
+            self.log.warn("Command list_scanners was not successful")
+            return False
+        
         self.cmd.check_for_scanner.payload = {"ip_address": self.ip}
         success = self.send_message(self.cmd.check_for_scanner)
 
         if not success:
+            self.log.warn("Command check_for_scanner was not successful")
             return False
 
-        if not self.is_scanner_connected():
+        while not self.is_scanner_connected():
             self.cmd.connect_scanner.payload = {"ip_address": self.ip}
-            return self.send_message(self.cmd.connect_scanner)
+            success =  self.send_message(self.cmd.connect_scanner)
+            if not success:
+                self.log.warn("Command connect_scanner was not successful")
+                return False
+            if self.last_connection_state == 5:
+                break
+            self.log.info("Waiting 5 seconds before requesting for a connection")
+            time.sleep(5)
+
+        """
+        scanner_connected = False
+        retries = 0
+        while not scanner_connected and retries < 5:
+            if SCANNER_STATUS_CONNECTED in self.scanner_status_not_dict:
+                scanner_connected = str2bool(self.scanner_status_not_dict[SCANNER_STATUS_CONNECTED].value.get())
+            retries += 1
+            time.sleep(1)
+        
+        if not scanner_connected:
+            self.log.warn("The state SCANNER_STATUS_CONNECTED was never set.")
+
+        return scanner_connected
+        """
         return True
 
     def check_connection_status(self):
         """Check connection status
 
         Returns
         -------
@@ -396,55 +454,55 @@
 
         self.cmd.set_endpoints.payload = [
             {
                 "endpoint_id": ENDPOINT_ID_LOG,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoind_id.log,
+                "file_name": self.config.endpoint_id.log,
                 "file_max_bytes": 1024 * 1024 * 1024,
             },
             {
                 "endpoint_id": ENDPOINT_ID_STREAM,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoind_id.stream,
+                "file_name": self.config.endpoint_id.stream,
                 "file_max_bytes": 1024 * 1024 * 1024,
             },
             {
                 "endpoint_id": ENDPOINT_ID_XYZ_LASER,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoind_id.xyz_laser,
+                "file_name": self.config.endpoint_id.xyz_laser,
                 "file_max_bytes": 1024 * 1024 * 1024,
             },
             {
                 "endpoint_id": ENDPOINT_ID_SENSOR_LASER,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoind_id.sensor_laser,
+                "file_name": self.config.endpoint_id.sensor_laser,
                 "file_max_bytes": 0,
             },
             {
                 "endpoint_id": ENDPOINT_ID_SENSOR_STILLS_RAW,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoind_id.sensor_stills_raw,
+                "file_name": self.config.endpoint_id.sensor_stills_raw,
                 "file_max_bytes": 0,
             },
             {
                 "endpoint_id": ENDPOINT_ID_SENSOR_STILLS_PROCESSED,
                 "net_enabled": False,
                 "net_connection": "",
                 "file_enabled": True,
-                "file_name": self.config.endpoind_id.sensor_stills_processed,
+                "file_name": self.config.endpoint_id.sensor_stills_processed,
                 "file_max_bytes": 0,
             },
         ]
 
         success = self.send_message(self.cmd.set_endpoints)
         if not success:
             return False
@@ -460,58 +518,79 @@
         respectively.
 
         Returns
         -------
         bool
             True if the scanner is connected to this API, False otherwise
         """
-        self.send_message(self.cmd.list_scanners)
+        #self.send_message(self.cmd.list_scanners)
 
-        self.cmd.check_for_scanner.payload = {"ip_address": self.ip}
-        self.send_message(self.cmd.check_for_scanner)
+        #self.cmd.check_for_scanner.payload = {"ip_address": self.ip}
+        #self.send_message(self.cmd.check_for_scanner)
 
         while len(self.scanner_list_not_dict) == 0:
             time.sleep(1)
             self.log.info("Waiting for ScannerListNot")
             if not self.client.connected:
                 return False
-
-        scanner_connection_state = safe_get(self.scanner_list_not_dict, self.ip)
+            
+        scanner_connection_state = int(safe_get(self.scanner_list_not_dict, self.ip))
         if scanner_connection_state is None:
             self.log.warning("Scanner not found in ScannerListNot")
             return False
 
-        self.log.info("[VoyisAPI]: Scanner found in ScannerListNot")
+        self.log.debug("[VoyisAPI]: Scanner found in ScannerListNot")
         self.log.info(
             "[VoyisAPI]: Scanner connection state: {}".format(
                 scanner_connection_to_str(scanner_connection_state)
             )
         )
 
+        if scanner_connection_state < SCANNER_NOT_READY:
+            self.log.warn("Scanner is not ready, resetting comms...")
+            self.state.reset()
+
         return scanner_connection_state == SCANNER_CONNECTED_TO_THIS_API
+    
+    def wait_for_scanning_status(self, expected_value):
+        status_achieved = False
+        while not status_achieved:
+            success = self.get_scanner_status()
+            if SCANNER_STATUS_SCAN_IN_PROGRESS not in self.scanner_status_not_dict:
+                continue
+            res = str2bool(self.scanner_status_not_dict[SCANNER_STATUS_SCAN_IN_PROGRESS].value.get())
+            if res == expected_value:
+                break
+            self.log.info("Waiting for SCANNER_STATUS_SCAN_IN_PROGRESS to become {}".format(expected_value))
+            time.sleep(5)
 
     def stop_scanning_if_running(self):
         """Helper function to stop scanning if it is running
 
         Returns
         -------
         bool
             True if the scanner was stopped, False otherwise
         """
-        success = False
-        if SCANNER_STATUS_SCAN_IN_PROGRESS not in self.scanner_status_not_dict:
-            self.log.debug("Assumed scanner is not scanning...")
-            return True
+        success = self.stop_scanning()
+        self.wait_for_scanning_status(False)
+        """
+        while not success:
+            if SCANNER_STATUS_SCAN_IN_PROGRESS in self.scanner_status_not_dict:
+                break
+            time.sleep(1)
 
         while self.scanner_status_not_dict[SCANNER_STATUS_SCAN_IN_PROGRESS].value:
             self.log.info("Scan in progress, trying to stop it...")
             success = self.stop_scanning()
             if success:
                 break
             time.sleep(5)
+        self.wait_for_scanning_status(False)
+        """
         return success
 
     def perform_system_checks(self):
         """Perform system checks
 
         Returns
         -------
@@ -573,67 +652,64 @@
         led_panel_ready = safe_get(
             self.scanner_status_not_dict, SCANNER_STATUS_LED_PANEL_READY
         )
 
         self.log.info("[VoyisAPI]: Device status:")
         self.log.info(
             "  * API: {} {}".format(
-                "Connected" if api_connected else "NOT Connected",
-                "Ready" if api_ready else "NOT Ready",
+                "Connected" if str2bool(api_connected.value.get()) else "NOT Connected",
+                "Ready" if str2bool(api_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * Stills camera: {} {}".format(
-                "Connected" if stills_cam_connected else "NOT Connected",
-                "Ready" if stills_cam_ready else "NOT Ready",
+                "Connected" if str2bool(stills_cam_connected.value.get()) else "NOT Connected",
+                "Ready" if str2bool(stills_cam_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * Laser camera: {} {}".format(
-                "Connected" if laser_cam_connected else "NOT Connected",
-                "Ready" if laser_cam_ready else "NOT Ready",
+                "Connected" if str2bool(laser_cam_connected.value.get()) else "NOT Connected",
+                "Ready" if str2bool(laser_cam_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * Laser: {} {}".format(
-                "Connected" if laser_connected else "NOT Connected",
-                "Ready" if laser_ready else "NOT Ready",
+                "Connected" if str2bool(laser_connected.value.get()) else "NOT Connected",
+                "Ready" if str2bool(laser_ready.value.get()) else "NOT Ready",
             )
         )
         self.log.info(
             "  * LED panel: {} {}".format(
-                "Connected" if led_panel_connected else "NOT Connected",
-                "Ready" if led_panel_ready else "NOT Ready",
+                "Connected" if str2bool(led_panel_connected.value.get()) else "NOT Connected",
+                "Ready" if str2bool(led_panel_ready.value.get()) else "NOT Ready",
             )
         )
 
-        """
         return (
             api_ready
             and stills_cam_ready
             and laser_cam_ready
             and laser_ready
             and led_panel_ready
         )
-        """
-        return True
 
     def configure_time_source(self):
         """Sends command to configure time source
 
         Returns
         -------
         bool
             True if the command was successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Configuring time source...")
 
         self.cmd.set_time_tag_source.payload = {
-            "network": SOURCE_TCP_CLIENT,
-            "connection": "4010",
+            "network": str_to_network_source(self.config.pps_input.mode),
+            "connection": self.config.pps_input.ip_address,
         }
 
         return self.send_message(self.cmd.set_time_tag_source)
 
     def configure_nav(self):
         """Sends command to configure the navigation source
 
@@ -641,44 +717,44 @@
         -------
         bool
             True if the command was successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Configuring nav...")
 
         self.cmd.set_nav_data_source.payload = {
-            "network": SOURCE_TCP_SERVER,
-            "protocol": NAVPROTO_PSONNAV,
-            "connection": "192.168.179.10:4003",
+            "network": str_to_network_source(self.config.navigation_input.mode),
+            "protocol": str_to_navproto(self.config.navigation_input.driver),
+            "connection": self.config.navigation_input.ip_address,
         }
         return self.send_message(self.cmd.set_nav_data_source)
 
     def set_scan_parameters(self):
         """Sets the scan parameters
 
         Returns
         -------
         bool
             True if the command was successful, False otherwise
         """
         self.log.info("[VoyisAPI]: Setting scan parameters...")
-        cfg = self.config.scanner_param.s
+        cfg = self.config.scanner_param
         self.cmd.set_local_scanner_parameters.payload = [
             {
                 "parameter_id": SCANNER_PARAM_PROFILE_STILLS_EXP,
-                "value": str(cfg.scanner_param.stills_exp_us),
+                "value": str(cfg.stills_exp_us),
                 "type": VALUE_TYPE_UINT,
             },
             {
                 "parameter_id": SCANNER_PARAM_LASER_FREQ,
-                "value": str(int(cfg.scanner_param.laser_freq_hz * 1000)),
+                "value": str(int(cfg.laser_freq_hz * 1000)),
                 "type": VALUE_TYPE_UINT,
             },
             {
                 "parameter_id": SCANNER_PARAM_STILL_FREQ,
-                "value": str(int(cfg.scanner_param.stills_freq_hz * 1000)),
+                "value": str(int(cfg.stills_freq_hz * 1000)),
                 "type": VALUE_TYPE_UINT,
             },
             {  # If true, laser freq is 1 Hz
                 "parameter_id": SCANNER_PARAM_OUTPUT_LASER_DATA,
                 "value": bool2str(cfg.save_laser_images),
                 "type": VALUE_TYPE_BOOL,
             },
@@ -722,33 +798,48 @@
         success = self.send_message(self.cmd.set_local_scanner_parameters)
         if not success:
             return False
 
         success = self.send_message(self.cmd.apply_local_scanner_parameters)
         if not success:
             return False
+        
+        """
+        success = self.send_message(self.cmd.query_api_configuration)
+        if not success:
+            return False
 
+        cfg = self.config.api_param_stills
         self.cmd.set_api_configuration.payload = [
             {
                 "parameter_id": API_PARAM_STILLS_IMAGE_UNDISTORT,
-                "value": bool2str(cfg.undistort_images, "1", "0"),
+                "value": bool2str(cfg.undistort, "1", "0"),
                 "type": VALUE_TYPE_UINT,
             },
             {
                 "parameter_id": API_PARAM_STILLS_IMAGE_SAVE_ORIGINAL,
                 "value": bool2str(cfg.save_original, "1", "0"),
                 "type": VALUE_TYPE_BOOL,
             },
             {
                 "parameter_id": API_PARAM_STILLS_PROCESSED_IMAGE_FORMAT,
-                "value": bool2str(cfg.processed_image_format, "1", "0"),
+                "value": cfg.processed_image_format_uint,
                 "type": VALUE_TYPE_UINT,
             },
         ]
-        return self.send_message(self.cmd.set_api_configuration)
+        success =  self.send_message(self.cmd.set_api_configuration, expect_ack=False)
+        if not success:
+            return False
+    
+        success = self.send_message(self.cmd.query_api_configuration)
+        if not success:
+            return False
+        """
+        
+        return True
 
     def check_laser_is_armed(self):
         """Helper function to check if the laser is armed
 
         Returns
         -------
         bool
@@ -853,15 +944,15 @@
         if internal_temp_stills_sensor is not None:
             self.log.info(
                 "  * internal_temp_stills_sensor: {} C".format(
                     internal_temp_stills_sensor.value.get()
                 )
             )
         if internal_temp_ch is not None:
-            return internal_temp_ch.value.get() < 60
+            return int(internal_temp_ch.value.get()) < 60
         else:
             return True
 
     def start_scanning(self):
         """Sends the command to start scanning
 
         Returns
@@ -966,14 +1057,15 @@
                     f.write(val.to_yaml())
         elif message == "ScannerListNot":
             msg_class = ScannerListNot(data)
             for idx in range(msg_class.size()):
                 self.scanner_list_not_dict[
                     msg_class.ip_addresses[idx]
                 ] = msg_class.connection_states[idx]
+            self.last_connection_state = int(safe_get(self.scanner_list_not_dict, self.ip))
         elif message == "ConnectionChangeNot":
             msg_class = ConnectionChangeNot(data)
             self.connection_change_not_list.append(msg_class)
         elif message == "ScannerStatus":
             msg_class = ScannerStatus(data)
             self.scanner_status_list.append(msg_class)
         elif message == "ScannerStatusNot":
```

### Comparing `pyvoyis-1.0.2/src/pyvoyis/api500/client.py` & `pyvoyis-1.0.3/src/pyvoyis/api500/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 See LICENSE.md file in the project root for full license information.
 """
 
 import asyncio
 import json
 import logging
 import sys
+import copy
 
 if sys.version_info[:2] >= (3, 7):
     pass
 else:
     pass
 
 
@@ -24,23 +25,24 @@
         self._ready = asyncio.Event()
         self.loop = loop
         self.task = self.loop.create_task(self._process_queue_loop())
         # Store received messages here
         self.received = []
         self.lock = asyncio.Lock()
         self.connected = False
+        self.data = ""
 
     async def _process_queue_loop(self):
         """Send messages to the server as they become available."""
         await self._ready.wait()
         self.log.info("API500 client ready!")
         while True:
             message = await self.queue.get()
             self.transport.write(message.encode("utf-8"))
-            self.log.debug("Message sent: \n{}".format(message))
+            self.log.warn("Message sent: \n{}".format(message))
             await asyncio.sleep(0.1)
 
     def connection_made(self, transport):
         """Upon connection send the message to the
         server
 
         A message has to have the following items:
@@ -78,33 +80,45 @@
         back from the server
 
         The return message consist of three fields:
             type:           subscribe/unsubscribe
             channel:        the name of the channel
             channel_count:  the amount of channels subscribed to
         """
-        data = data.decode("utf-8")
-        # self.log.debug('Received: \n{}'.format(data))
-
+        chunk = data.decode("utf-8")
+        whole_data = ""
+        # self.log.debug('Received raw chunk: {}'.format(data))
+        if chunk.endswith("\n}"):
+            self.data += chunk
+            whole_data = copy.deepcopy(self.data)
+            self.data = ""
+            self.log.debug("Whole chunk ready")
+        else:
+            self.log.debug("Adding chunk to message")
+            self.data += chunk
+            return
+        
         # Split data into JSON strings if "}{" is found
-        objects = data.split("}{")
+        objects = whole_data.split("}{")
 
         # Add back the missing brackets
         if len(objects) > 1:
             objects[0] = objects[0] + "}"
             objects[-1] = "{" + objects[-1]
             for idx in range(1, len(objects) - 1):
                 objects[idx] = "{" + objects[idx] + "}"
 
         # Process each object
         for idx, obj in enumerate(objects):
-            self.log.debug(
-                "Received split object {}: {}".format(idx, json.dumps(json.loads(obj)))
-            )
-            asyncio.ensure_future(self.process_data(obj))
+            try:
+                self.log.warn(
+                    "Received split object {}: {}".format(idx, json.dumps(json.loads(obj))))
+                asyncio.ensure_future(self.process_data(obj))
+            except json.decoder.JSONDecodeError as e:
+                self.log.warn("Could not decode: {}".format(obj))
 
     def connection_lost(self, error):
         if error:
             self.log.error("ERROR: {}".format(error))
         else:
             self.log.warning("The server closed the connection")
         self.connected = False
```

### Comparing `pyvoyis-1.0.2/src/pyvoyis/api500/command.py` & `pyvoyis-1.0.3/src/pyvoyis/api500/command.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.2/src/pyvoyis/api500/defs.py` & `pyvoyis-1.0.3/src/pyvoyis/api500/defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,15 +342,21 @@
     elif value == API_PARAM_STILLS_ADVANCED_BRIGHTNESS:
         return "API_PARAM_STILLS_ADVANCED_BRIGHTNESS"
     elif value == API_PARAM_STILLS_ADVANCED_CONTRAST:
         return "API_PARAM_STILLS_ADVANCED_CONTRAST"
     elif value == API_PARAM_STILLS_ADVANCED_WHITE_BALANCE:
         return "API_PARAM_STILLS_ADVANCED_WHITE_BALANCE"
     elif value == API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING:
-        return "API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING"
+        return "API_PARAM_STILLS_ADVANCED_ADAPTIVE_LIGHTING" 
+    elif value == API_PARAM_DUMMY_0:
+        return "API_PARAM_DUMMY_0"
+    elif value == API_PARAM_DUMMY_1:
+        return "API_PARAM_DUMMY_1"
+    elif value == API_PARAM_ENABLE_RAM_BUFF_MONITOR:
+        return "API_PARAM_ENABLE_RAM_BUFF_MONITOR"
     else:
         print("Unknown API parameter:", value)
         return "Unknown"
 
 
 """ Scanner status """
 SCANNER_STATUS_CONNECTED = 0
@@ -1200,14 +1206,26 @@
 
 SOURCE_COM = 0
 SOURCE_UDP = 1
 SOURCE_TCP_CLIENT = 2
 SOURCE_TCP_SERVER = 3
 SOURCE_MULTICAST = 4
 
+def str_to_network_source(value:str):
+    if value.lower() == "com":
+        return SOURCE_COM
+    elif value.lower() == "udp":
+        return SOURCE_UDP
+    elif value.lower() == "tcp_client":
+        return SOURCE_TCP_CLIENT
+    elif value.lower() == "tcp_server":
+        return SOURCE_TCP_SERVER
+    elif value.lower() == "multicast":
+        return SOURCE_MULTICAST
+
 
 def source_to_str(value):
     if value == SOURCE_COM:
         return "SOURCE_COM"
     elif value == SOURCE_UDP:
         return "SOURCE_UDP"
     elif value == SOURCE_TCP_CLIENT:
@@ -1236,14 +1254,37 @@
 NAVPROTO_ROVINS = 50  # ROVINS INS format
 NAVPROTO_NAVLAB = 60  # NAVLAB format
 NAVPROTO_IXBLUESTD = 70  # IXBlue Std format
 NAVPROTO_PHINSSTD = 80  # PHINS Std format supports range
 NAVPROTO_PSONNAV = 1  # Sonardyne PSONNAV format
 
 
+def str_to_navproto(value:str):
+    if value.lower() == "raw":
+        return NAVPROTO_RAW
+    if value.lower() == "lnav":
+        return NAVPROTO_LNAV
+    if value.lower() == "delphins":
+        return NAVPROTO_DELPHINS
+    if value.lower() == "ise":
+        return NAVPROTO_ISE
+    if value.lower() == "kongsberg":
+        return NAVPROTO_KONGSBERG
+    if value.lower() == "rovins":
+        return NAVPROTO_ROVINS
+    if value.lower() == "navlab":
+        return NAVPROTO_NAVLAB
+    if value.lower() == "ixbluestd":
+        return NAVPROTO_IXBLUESTD
+    if value.lower() == "phinsstd":
+        return NAVPROTO_PHINSSTD
+    if value.lower() == "psonnav":
+        return NAVPROTO_PSONNAV
+
+
 def navproto_to_str(value):
     if value == NAVPROTO_RAW:
         return "NAVPROTO_RAW"
     elif value == NAVPROTO_LNAV:
         return "NAVPROTO_LNAV"
     elif value == NAVPROTO_DELPHINS:
         return "NAVPROTO_DELPHINS"
```

### Comparing `pyvoyis-1.0.2/src/pyvoyis/cli.py` & `pyvoyis-1.0.3/src/pyvoyis/cli.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,18 +4,17 @@
 Copyright (c) 2023, Miquel Massot
 All rights reserved.
 Licensed under the GPLv3 License.
 See LICENSE.md file in the project root for full license information.
 """
 
 import argparse
-import logging
 
 from pyvoyis import Configuration, VoyisAPI
-from pyvoyis.tools.custom_logger import setup_logging
+
 
 
 def main():
     parser = argparse.ArgumentParser(
         description="Run a TCP client to send messages to Voyis API"
     )
     parser.add_argument("--ip", type=str, help="IP address of the Voyis API")
@@ -27,23 +26,22 @@
     args = parser.parse_args()
 
     config = Configuration(args.config)
 
     if args.log_path:
         config.log_path = args.log_path
 
-    setup_logging(config.log_path)
-    log = logging.getLogger("VoyisROS")
-    log.info("Starting Voyis API client")
+    
+    print("Starting Voyis API client")
 
     if args.ip:
-        log.info("Using provided IP address: %s", args.ip)
+        print("Using provided IP address: %s", args.ip)
         config.ip_address = args.ip
     if args.port:
-        log.info("Using provided port: %s", args.port)
+        print("Using provided port: %s", args.port)
         config.port = args.port
 
     api = VoyisAPI(config)
     api.request_acquisition()
     api.run()
```

### Comparing `pyvoyis-1.0.2/src/pyvoyis/commander.py` & `pyvoyis-1.0.3/src/pyvoyis/commander.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.2/src/pyvoyis/messages.py` & `pyvoyis-1.0.3/src/pyvoyis/messages.py`

 * *Files identical despite different names*

### Comparing `pyvoyis-1.0.2/src/pyvoyis/state_machine.py` & `pyvoyis-1.0.3/src/pyvoyis/state_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
         | configuring.to(idling)
         | readying.to(idling)
         | requesting_acquisition.to(idling)
         | acquiring.to(idling)
         | requesting_stop.to(idling)
         | stopping.to(idling)
         | disconnecting.to(idling)
+        | idling.to(idling)
     )
 
     def before_cycle(self, event: str, source: State, target: State, message: str = ""):
         message = ". " + message if message else ""
         return f"Running {event} from {source.id} to {target.id}{message}"
 
     @property
```

### Comparing `pyvoyis-1.0.2/src/pyvoyis.egg-info/SOURCES.txt` & `pyvoyis-1.0.3/src/pyvoyis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

