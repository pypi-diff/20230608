# Comparing `tmp/gattfuzz-0.0.8.tar.gz` & `tmp/gattfuzz-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattfuzz-0.0.8.tar", last modified: Thu Jun  8 11:58:09 2023, max compression
+gzip compressed data, was "gattfuzz-0.0.9.tar", last modified: Thu Jun  8 12:04:48 2023, max compression
```

## Comparing `gattfuzz-0.0.8.tar` & `gattfuzz-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.036239 gattfuzz-0.0.8/
--rw-rw-rw-   0        0        0     1257 2023-06-08 11:58:09.035239 gattfuzz-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.018240 gattfuzz-0.0.8/gattfuzz/
--rw-rw-rw-   0        0        0     3807 2023-06-08 11:45:19.000000 gattfuzz-0.0.8/gattfuzz/GattFuzz.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.034240 gattfuzz-0.0.8/gattfuzz/lib/
--rw-rw-rw-   0        0        0    15846 2023-06-08 11:55:52.000000 gattfuzz-0.0.8/gattfuzz/lib/BLEControl.py
--rw-rw-rw-   0        0        0     1852 2023-06-08 11:20:44.000000 gattfuzz-0.0.8/gattfuzz/lib/Logger.py
--rw-rw-rw-   0        0        0     3930 2023-06-08 11:23:41.000000 gattfuzz-0.0.8/gattfuzz/lib/PcapProcessor.py
--rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/lib/StringMutator.py
--rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/lib/ValueLCS.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.027237 gattfuzz-0.0.8/gattfuzz.egg-info/
--rw-rw-rw-   0        0        0     1257 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 11:58:09.036239 gattfuzz-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-08 11:57:34.000000 gattfuzz-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:04:48.813068 gattfuzz-0.0.9/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 12:04:48.812069 gattfuzz-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 12:04:48.793070 gattfuzz-0.0.9/gattfuzz/
+-rw-rw-rw-   0        0        0     3794 2023-06-08 12:04:11.000000 gattfuzz-0.0.9/gattfuzz/GattFuzz.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.9/gattfuzz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:04:48.811072 gattfuzz-0.0.9/gattfuzz/lib/
+-rw-rw-rw-   0        0        0    15830 2023-06-08 12:04:02.000000 gattfuzz-0.0.9/gattfuzz/lib/BLEControl.py
+-rw-rw-rw-   0        0        0     1852 2023-06-08 11:20:44.000000 gattfuzz-0.0.9/gattfuzz/lib/Logger.py
+-rw-rw-rw-   0        0        0     3930 2023-06-08 11:23:41.000000 gattfuzz-0.0.9/gattfuzz/lib/PcapProcessor.py
+-rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.9/gattfuzz/lib/StringMutator.py
+-rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.9/gattfuzz/lib/ValueLCS.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.9/gattfuzz/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 12:04:48.802069 gattfuzz-0.0.9/gattfuzz.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 12:04:48.000000 gattfuzz-0.0.9/gattfuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-06-08 12:04:48.000000 gattfuzz-0.0.9/gattfuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 12:04:48.000000 gattfuzz-0.0.9/gattfuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-08 12:04:48.000000 gattfuzz-0.0.9/gattfuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 11:58:08.000000 gattfuzz-0.0.9/gattfuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-06-08 12:04:48.000000 gattfuzz-0.0.9/gattfuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 12:04:48.000000 gattfuzz-0.0.9/gattfuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 12:04:48.813068 gattfuzz-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-08 12:04:37.000000 gattfuzz-0.0.9/setup.py
```

### Comparing `gattfuzz-0.0.8/PKG-INFO` & `gattfuzz-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.8/README.md` & `gattfuzz-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.8/gattfuzz/GattFuzz.py` & `gattfuzz-0.0.9/gattfuzz/GattFuzz.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from gattfuzz.lib.ValueLCS import ValueLCS
 from gattfuzz.lib.PcapProcessor import PcapProcessor
 from gattfuzz.lib.BLEControl import BLEControl
 from scapy.all import *
 import argparse
-import time
 
 from gattfuzz.lib.Logger import Logger
 logger = Logger(loggername='Main').get_logger()
 
 
 val = ValueLCS()
 
 '''
 2023.2.8 补充 空pyload
 7.21 一个问题（已解决）
 基于pcap的变异覆盖率
 
 7.21 一个问题
-多次连接才能连上
+多次连接才能连上g
 '''
 def fuzz_with_pcap(pcap_path,tar_mac):
     
     latest_dic = {}
     #提取数据包 static          
     logger.info("--开始处理pcap文件--")
     pcap_processor = PcapProcessor(pcap_path)
@@ -33,16 +32,16 @@
     logger.info("--处理pcap文件结束--")
     # print("pcap handles:", pcap_handles)                # pcap中的handles
     # print("all_value:", han_val_dic)
                                       
 
     # connect device and logger.info chars
     # logger.info("#"*30+ "设备扫描"+ '#'*30)
-    ble = BLEControl()                 
-    ble.tar_con(tar_mac)
+    ble = BLEControl(tar_mac)                 
+    ble.tar_con()
     bulepy_handles = ble.print_char()                      # 建立连接打印read，并打开所有notification
     logger.info("bluepy handles:{}".format(str(bulepy_handles)))
 
     # 存在部分handle不通信的情况，pcap中没有数据，补充这部分
     for handle in bulepy_handles:
         # logger.info("handle:{}".format(str(handle))
         if handle not in pcap_handles:
@@ -59,31 +58,31 @@
     # ble.tar_con(tar_mac)
     # # TODO +判断连接状态
     ble.write_to_csv(after_Muta_dic)                        # write过程写入csv并写到目标设备handle
 
 def fuzz_without_pcap(tar_mac):
 
     # just write
-    ble = BLEControl()
-    ble.tar_con(tar_mac)
+    ble = BLEControl(tar_mac)
+    ble.tar_con()
     handles = ble.print_char()
     # print("handles:", handles)
 
     # 随机变异十次
     n = 0
     after_dic = {}
     while n<100:
         logger.info("--开始随机变异--")
         after_dic = val.var_no_pcap(handles)   # 一次变异
         logger.info("--随机变异结束--")
         # print("after_dic:", after_dic)
         n += 1
 
         time.sleep(10.0)
-        #print(ble._conn)
+        print(ble._conn)
         logger.info("--开始变异结果写入--")
         # ble.tar_con(tar_mac)
         ble.write_to_csv(after_dic)
         logger.info("--一次Fuzz结束--")
     
 
 def main():
```

### Comparing `gattfuzz-0.0.8/gattfuzz/lib/BLEControl.py` & `gattfuzz-0.0.9/gattfuzz/lib/BLEControl.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,32 +20,33 @@
     def handleNotification(self, cHandle, data):
         logger.error("Recevied handle: {}  nofity  ----> {} ".format(str(cHandle), str(data)))
 
 
 
 class BLEControl():
 
-    def __init__(self, custom_logger=None):
+    def __init__(self, mac, custom_logger=None):
         self._conn = None
+        self._mac = mac
         if custom_logger:
             self.logger = custom_logger
         else:
             self.logger = logger
     
     # connect to target mac
-    def tar_con(self, tar_mac):
+    def tar_con(self):
         logger = self.logger
         logger.info("Begin sacn")
         n = 1
         scanner = Scanner()
         devices = scanner.scan(timeout=10)
         logger.info("发现 %d 个设备", len(devices))          
         for dev in devices:    
-            if dev.addr==tar_mac:
-                logger.info("Find target device::"+ tar_mac)
+            if dev.addr==self._mac:
+                logger.info("Find target device::"+ self._mac)
                 # logger.info("\n")
                 logger.info("              ————————————广播信息————————————                    ")
                 logger.info("|                                                      |")
                 for (adtype, desc, value) in dev.getScanData():
                     logger.info("    %s = %s" % (desc, value))
                 logger.info("|                                                      |")
                 logger.info("              ————————————广播信息————————————                    ")
@@ -59,15 +60,14 @@
                         if i<10:
                             continue
                         else:
                             logger.info('\n')
                             logger.error("The device connection failed, check the device status or previous pyload and try again.")
                             # sys.exit()
                 if self._conn:
-                    self._mac = tar_mac
                     self._conn.setDelegate(ReceiveDelegate())
                     self._conn.setMTU(500)
                     # self.print_char()
                 
                 else: 
                     if n < len(devices):
                         n = n+1
```

### Comparing `gattfuzz-0.0.8/gattfuzz/lib/Logger.py` & `gattfuzz-0.0.9/gattfuzz/lib/Logger.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.8/gattfuzz/lib/PcapProcessor.py` & `gattfuzz-0.0.9/gattfuzz/lib/PcapProcessor.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.8/gattfuzz/lib/StringMutator.py` & `gattfuzz-0.0.9/gattfuzz/lib/StringMutator.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.8/gattfuzz/lib/ValueLCS.py` & `gattfuzz-0.0.9/gattfuzz/lib/ValueLCS.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.8/gattfuzz.egg-info/PKG-INFO` & `gattfuzz-0.0.9/gattfuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.8
+Version: 0.0.9
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.8/setup.py` & `gattfuzz-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fp:
     description = fp.read()
 
 setup(
     name='gattfuzz',
-    version='0.0.8',
+    version='0.0.9',
     description= "A tool for fuzzing BLE GATT",
     long_description=description,
     packages=find_packages(),
     #packages=['gattfuzz'],
     zip_safe=False,
     install_requires=[
         'bluepy==1.3.0',
```

