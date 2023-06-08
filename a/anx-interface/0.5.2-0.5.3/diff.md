# Comparing `tmp/anx_interface-0.5.2.tar.gz` & `tmp/anx_interface-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anx_interface-0.5.2.tar", max compression
+gzip compressed data, was "anx_interface-0.5.3.tar", max compression
```

## Comparing `anx_interface-0.5.2.tar` & `anx_interface-0.5.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      437 2023-03-24 10:07:57.450653 anx_interface-0.5.2/README.md
--rw-r--r--   0        0        0      105 2023-03-24 10:07:57.450902 anx_interface-0.5.2/anx_interface/__init__.py
--rw-r--r--   0        0        0    14048 2023-06-01 06:26:15.933105 anx_interface-0.5.2/anx_interface/anx_interface.py
--rw-r--r--   0        0        0        0 2023-02-18 08:58:29.850329 anx_interface-0.5.2/anx_interface/assets/__init__.py
--rw-r--r--   0        0        0     2012 2023-05-15 13:22:58.745801 anx_interface-0.5.2/anx_interface/assets/device_camera.py
--rw-r--r--   0        0        0     1529 2023-03-24 10:07:57.451316 anx_interface-0.5.2/anx_interface/assets/device_gnss.py
--rw-r--r--   0        0        0     1519 2023-03-24 10:07:57.451416 anx_interface-0.5.2/anx_interface/assets/device_imu.py
--rw-r--r--   0        0        0        0 2023-02-18 08:58:29.851022 anx_interface-0.5.2/anx_interface/tests/__init__.py
--rwxr-xr-x   0        0        0     1133 2023-05-15 13:24:41.280464 anx_interface-0.5.2/anx_interface/tests/test_device_camera.py
--rwxr-xr-x   0        0        0      315 2023-03-24 10:07:57.451655 anx_interface-0.5.2/anx_interface/tests/test_listen_device_camera.py
--rw-r--r--   0        0        0     6526 2023-04-05 10:49:46.421341 anx_interface-0.5.2/anx_interface/tflite_interface.py
--rw-r--r--   0        0        0        0 2023-03-24 10:07:57.451811 anx_interface-0.5.2/anx_interface/tools/__init__.py
--rw-r--r--   0        0        0     6141 2023-06-01 10:00:47.155562 anx_interface-0.5.2/anx_interface/tools/anx.py
--rw-r--r--   0        0        0        0 2023-04-22 06:41:14.576033 anx_interface-0.5.2/anx_interface/utils/__init__.py
--rw-r--r--   0        0        0      928 2023-04-26 13:15:20.161175 anx_interface-0.5.2/anx_interface/utils/fifo.py
--rw-r--r--   0        0        0        0 2023-03-24 10:07:57.451957 anx_interface-0.5.2/anx_logging/__init__.py
--rwxr-xr-x   0        0        0     5038 2023-04-03 11:05:06.101471 anx_interface-0.5.2/anx_logging/perf_logger.py
--rw-r--r--   0        0        0        0 2023-02-18 08:58:29.851977 anx_interface-0.5.2/anx_mock/__init__.py
--rwxr-xr-x   0        0        0     7194 2023-03-24 10:07:57.452183 anx_interface-0.5.2/anx_mock/anx_mock.py
--rw-r--r--   0        0        0        0 2023-02-18 08:58:29.852394 anx_interface-0.5.2/anx_mock/assets/__init__.py
--rw-r--r--   0        0        0     2810 2023-03-24 10:07:57.452293 anx_interface-0.5.2/anx_mock/assets/device_camera.py
--rw-r--r--   0        0        0     1263 2023-03-24 10:07:57.452396 anx_interface-0.5.2/anx_mock/assets/device_gnss.py
--rw-r--r--   0        0        0     2325 2023-03-24 10:07:57.452484 anx_interface-0.5.2/anx_mock/assets/device_imu.py
--rw-r--r--   0        0        0      337 2023-02-18 08:58:29.853096 anx_interface-0.5.2/anx_mock/utils.py
--rw-r--r--   0        0        0     6148 2023-05-18 07:09:39.954752 anx_interface-0.5.2/anx_proto/.DS_Store
--rw-r--r--   0        0        0        0 2023-05-20 12:41:32.754638 anx_interface-0.5.2/anx_proto/__init__.py
--rw-r--r--   0        0        0        0 2023-05-20 12:41:32.754566 anx_interface-0.5.2/anx_proto/python/__init__.py
--rw-r--r--   0        0        0    22855 2023-05-20 12:41:32.755103 anx_interface-0.5.2/anx_proto/python/assets_pb2.py
--rw-r--r--   0        0        0    10046 2023-05-20 12:41:32.755366 anx_interface-0.5.2/anx_proto/python/common_pb2.py
--rw-r--r--   0        0        0    10457 2023-05-20 12:41:32.754839 anx_interface-0.5.2/anx_proto/python/device_pb2.py
--rw-r--r--   0        0        0     4288 2023-05-20 12:41:32.755211 anx_interface-0.5.2/anx_proto/python/model_pb2.py
--rw-r--r--   0        0        0      684 2023-06-01 10:31:34.039384 anx_interface-0.5.2/pyproject.toml
--rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 anx_interface-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0      437 2023-06-01 11:07:19.797446 anx_interface-0.5.3/README.md
+-rw-r--r--   0        0        0      105 2023-06-01 11:07:19.797776 anx_interface-0.5.3/anx_interface/__init__.py
+-rw-r--r--   0        0        0    14048 2023-06-06 13:09:31.416299 anx_interface-0.5.3/anx_interface/anx_interface.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:07:19.800785 anx_interface-0.5.3/anx_interface/assets/__init__.py
+-rw-r--r--   0        0        0     2024 2023-06-08 08:39:55.176391 anx_interface-0.5.3/anx_interface/assets/device_camera.py
+-rw-r--r--   0        0        0     1529 2023-06-01 11:07:19.801161 anx_interface-0.5.3/anx_interface/assets/device_gnss.py
+-rw-r--r--   0        0        0     1519 2023-06-01 11:07:19.801230 anx_interface-0.5.3/anx_interface/assets/device_imu.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:07:19.801297 anx_interface-0.5.3/anx_interface/tests/__init__.py
+-rwxr-xr-x   0        0        0     1133 2023-06-01 11:07:19.801537 anx_interface-0.5.3/anx_interface/tests/test_device_camera.py
+-rwxr-xr-x   0        0        0      315 2023-06-01 11:07:19.801608 anx_interface-0.5.3/anx_interface/tests/test_listen_device_camera.py
+-rw-r--r--   0        0        0     6530 2023-06-01 11:07:42.036552 anx_interface-0.5.3/anx_interface/tflite_interface.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:07:19.801858 anx_interface-0.5.3/anx_interface/tools/__init__.py
+-rw-r--r--   0        0        0     6324 2023-06-06 13:09:36.412833 anx_interface-0.5.3/anx_interface/tools/anx.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:07:19.802136 anx_interface-0.5.3/anx_interface/utils/__init__.py
+-rw-r--r--   0        0        0      928 2023-06-01 11:07:19.802366 anx_interface-0.5.3/anx_interface/utils/fifo.py
+-rw-r--r--   0        0        0       36 2023-06-01 11:07:42.037173 anx_interface-0.5.3/anx_logging/__init__.py
+-rwxr-xr-x   0        0        0     5023 2023-06-08 06:00:46.050001 anx_interface-0.5.3/anx_logging/perf_logger.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:07:19.802751 anx_interface-0.5.3/anx_mock/__init__.py
+-rwxr-xr-x   0        0        0     7194 2023-06-01 11:07:19.802865 anx_interface-0.5.3/anx_mock/anx_mock.py
+-rw-r--r--   0        0        0        0 2023-06-01 11:07:19.802943 anx_interface-0.5.3/anx_mock/assets/__init__.py
+-rw-r--r--   0        0        0     2810 2023-06-01 11:07:19.803037 anx_interface-0.5.3/anx_mock/assets/device_camera.py
+-rw-r--r--   0        0        0     1263 2023-06-01 11:07:19.803107 anx_interface-0.5.3/anx_mock/assets/device_gnss.py
+-rw-r--r--   0        0        0     2325 2023-06-01 11:07:19.803164 anx_interface-0.5.3/anx_mock/assets/device_imu.py
+-rw-r--r--   0        0        0      337 2023-06-01 11:07:19.803242 anx_interface-0.5.3/anx_mock/utils.py
+-rw-r--r--   0        0        0     6148 2023-05-18 07:09:39.954752 anx_interface-0.5.3/anx_proto/.DS_Store
+-rw-r--r--   0        0        0        0 2023-06-06 13:07:54.022995 anx_interface-0.5.3/anx_proto/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-06 13:07:54.022748 anx_interface-0.5.3/anx_proto/python/__init__.py
+-rw-r--r--   0        0        0    22855 2023-06-06 13:07:54.023966 anx_interface-0.5.3/anx_proto/python/assets_pb2.py
+-rw-r--r--   0        0        0    10046 2023-06-06 13:07:54.024314 anx_interface-0.5.3/anx_proto/python/common_pb2.py
+-rw-r--r--   0        0        0    10457 2023-06-06 13:07:54.023630 anx_interface-0.5.3/anx_proto/python/device_pb2.py
+-rw-r--r--   0        0        0     4288 2023-06-06 13:07:54.024106 anx_interface-0.5.3/anx_proto/python/model_pb2.py
+-rw-r--r--   0        0        0      684 2023-06-08 08:41:18.132474 anx_interface-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0     1221 1970-01-01 00:00:00.000000 anx_interface-0.5.3/PKG-INFO
```

### Comparing `anx_interface-0.5.2/anx_interface/anx_interface.py` & `anx_interface-0.5.3/anx_interface/anx_interface.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_interface/assets/device_camera.py` & `anx_interface-0.5.3/anx_interface/assets/device_camera.py`

 * *Files 4% similar despite different names*

```diff
@@ -63,12 +63,12 @@
     def _data_thread(self):
         while self._active:
             events = self._poller.poll(100)
             if events:
                 msg_bytes = self._socket.recv()
                 msg = assets_pb2.CameraData()
                 msg.ParseFromString(msg_bytes)
-                self.data = np.array(Image.open(BytesIO(msg.image)))
+                self.data = np.array(Image.open(BytesIO(msg.image)).rotate(180))
                 self._is_read = False
                 if self._cb is not None:
                     self._cb(self.data)
```

### Comparing `anx_interface-0.5.2/anx_interface/assets/device_gnss.py` & `anx_interface-0.5.3/anx_interface/assets/device_gnss.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_interface/assets/device_imu.py` & `anx_interface-0.5.3/anx_interface/assets/device_imu.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_interface/tests/test_device_camera.py` & `anx_interface-0.5.3/anx_interface/tests/test_device_camera.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_interface/tflite_interface.py` & `anx_interface-0.5.3/anx_interface/tflite_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,17 +116,17 @@
             rep = common_pb2.StdResponse()
             rep_bytes = self.socket.recv()
             rep.ParseFromString(rep_bytes)
             if rep.success:
                 self.model_loaded = False
                 self.model = None
 
-                self.input_tensor = []
+                self.input_tensors = []
 
-                self.output_tensor = []
+                self.output_tensors = []
                 return True
             else:
                 print(rep.message)
         return False
 
     def set_inputs(self, inputs):
         """
@@ -143,19 +143,19 @@
         # Check if input length is equal to self.input_sensor len
         if not len(inputs) == len(self.input_tensors):
             print("Expected inputs of length {len(self.input_tensors)}, but got {len(inputs)}")
             return False
 
         for index, input_ in enumerate(inputs):
             if not input_.shape == self.input_tensors[index].shape:
-                print(f"Input{index} shape should be {self.input_tensor.shape}")
+                print(f"Input{index} shape should be {self.input_tensors.shape}")
                 return False
 
             if not input_.dtype == self.input_tensors[index].dtype:
-                print(f"Input{index} dtype should be {self.input_tensor.dtype}")
+                print(f"Input{index} dtype should be {self.input_tensors.dtype}")
                 return False
 
             self.input_tensors[index].tensor = input_
 
         return True
 
     def invoke(self):
```

### Comparing `anx_interface-0.5.2/anx_interface/tools/anx.py` & `anx_interface-0.5.3/anx_interface/tools/anx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python3
 
 import click
 import time
 import numpy as np
 from anx_interface import Anx
+from anx_logging import PerfLogger
 
 class HzObserver:
     def __init__(self, N):
         self.N = N
         self.timestamps = []
 
     def ping(self):
@@ -189,27 +190,33 @@
 def reset_fs():
     response = anx.reset_fs()
     if response[0]:
         print(response[1])
     else:
         print(f"Error in resettig file system : {response[1]}")
 
+@click.command(name="perf_logger")
+def perf_logger():
+    perflogger = PerfLogger()
+    perflogger.logger_thread()
 
 @click.group()
 def cli():
     pass
 
 anx = None
-# hz_observer = None
+hz_observer = None
 
 def main():
     global anx
     anx = Anx()
+
     global hz_observer
     hz_observer = HzObserver(10)
+
     cli.add_command(get_gnss_config)
     cli.add_command(stream_gnss)
     cli.add_command(get_imu_config)
     cli.add_command(stream_imu)
     cli.add_command(get_camera_config)
     cli.add_command(stream_camera)
     cli.add_command(get_imei_numbers)
@@ -224,8 +231,9 @@
     cli.add_command(get_floos_version)
     cli.add_command(start_android_logs)
     cli.add_command(stop_android_logs)
     cli.add_command(wifi_stats)
     cli.add_command(hotspot_stats)
     cli.add_command(cellular_stats)
     cli.add_command(reset_fs)
+    cli.add_command(perf_logger)
     cli()
```

### Comparing `anx_interface-0.5.2/anx_interface/utils/fifo.py` & `anx_interface-0.5.3/anx_interface/utils/fifo.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_logging/perf_logger.py` & `anx_interface-0.5.3/anx_logging/perf_logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,24 +7,15 @@
 import psutil
 import numpy as np
 
 class PerfLogger:
     def __init__(self):
         signal.signal(signal.SIGINT, self.signal_handler)
 
-        self.thermal_zones = {
-                "cpu0-silver-usr": "thermal_zone11",
-                "cpu1-silver-usr": "thermal_zone22",
-                "cpu2-silver-usr": "thermal_zone33",
-                "cpu3-silver-usr": "thermal_zone44",
-                "cpu0-gold-usr": "thermal_zone71",
-                "cpu1-gold-usr": "thermal_zone72",
-                "cpu2-gold-usr": "thermal_zone73",
-                "cpu3-gold-usr": "thermal_zone1"
-        }
+        self.thermal_zones = {}
 
         self.filepath = "/root/.logs/"
         self.filename = f"{datetime.now().strftime('%d-%m-%Y-%H-%M-%S')}.csv"
 
         self.ok = True
 
         self.thermals = []
@@ -32,14 +23,15 @@
         self.ram = 0
         self.cpu_percentage = 0
         self.gpu_percentage = 0
         self.V = 0
         self.I = 0
 
         self.init_logfile()
+        self._populate_thermal_zones()
 
     def signal_handler(self, sig, frame):
         self.ok = False
 
     def init_logfile(self):
         if not os.path.exists(self.filepath):
             os.makedirs(self.filepath)
@@ -118,14 +110,21 @@
                 silver_core_avg_freq = "{:.2f}".format(np.array(self.core_freq[:4]).sum()/4)
                 gold_core_avg_freq = "{:.2f}".format(np.array(self.core_freq[4:8]).sum()/4)
                 print(f"Ts: {silver_core_avg_temp}°C, Tg: {gold_core_avg_temp}°C, Fs: {silver_core_avg_freq}MHz, Fg: {gold_core_avg_freq}MHz, ram: {self.ram}MB, cpu%: {self.cpu_percentage}, gpu%: {self.gpu_percentage}, V: {self.V}mV, I: {self.I}mA")
 
     def read(self, path):
         with open(path, 'r') as fd:
             return fd.read().strip()
+        
+    def _populate_thermal_zones(self):
+        for thermal_zone in os.listdir("/sys/devices/virtual/thermal"):
+            if not thermal_zone.startswith("thermal_zone"):
+                continue
+            with open(os.path.join("/sys/devices/virtual/thermal", thermal_zone, "type")) as f:
+                self.thermal_zones[f.read().strip()] = thermal_zone
 
 def main():
     perflogger = PerfLogger()
     perflogger.logger_thread()
 
 if __name__ == "__main__":
     main()
```

### Comparing `anx_interface-0.5.2/anx_mock/anx_mock.py` & `anx_interface-0.5.3/anx_mock/anx_mock.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_mock/assets/device_camera.py` & `anx_interface-0.5.3/anx_mock/assets/device_camera.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_mock/assets/device_gnss.py` & `anx_interface-0.5.3/anx_mock/assets/device_gnss.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_mock/assets/device_imu.py` & `anx_interface-0.5.3/anx_mock/assets/device_imu.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_proto/.DS_Store` & `anx_interface-0.5.3/anx_proto/.DS_Store`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_proto/python/assets_pb2.py` & `anx_interface-0.5.3/anx_proto/python/assets_pb2.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_proto/python/common_pb2.py` & `anx_interface-0.5.3/anx_proto/python/common_pb2.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_proto/python/device_pb2.py` & `anx_interface-0.5.3/anx_proto/python/device_pb2.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/anx_proto/python/model_pb2.py` & `anx_interface-0.5.3/anx_proto/python/model_pb2.py`

 * *Files identical despite different names*

### Comparing `anx_interface-0.5.2/pyproject.toml` & `anx_interface-0.5.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "anx-interface"
-version = "0.5.2"
+version = "0.5.3"
 description = "Implements anx_api"
 authors = ["Tech FloMobility <tech@flomobility.com>"]
 readme = "README.md"
 include = ["anx_proto/python/*", "anx_proto/*"]
 packages = [
   {include = "anx_interface"},
   {include = "anx_mock"},
```

### Comparing `anx_interface-0.5.2/PKG-INFO` & `anx_interface-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anx-interface
-Version: 0.5.2
+Version: 0.5.3
 Summary: Implements anx_api
 Author: Tech FloMobility
 Author-email: tech@flomobility.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

