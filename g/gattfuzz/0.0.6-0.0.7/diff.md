# Comparing `tmp/gattfuzz-0.0.6.tar.gz` & `tmp/gattfuzz-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattfuzz-0.0.6.tar", last modified: Thu Jun  8 11:19:53 2023, max compression
+gzip compressed data, was "gattfuzz-0.0.7.tar", last modified: Thu Jun  8 11:26:10 2023, max compression
```

## Comparing `gattfuzz-0.0.6.tar` & `gattfuzz-0.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.741737 gattfuzz-0.0.6/
--rw-rw-rw-   0        0        0     1257 2023-06-08 11:19:53.741737 gattfuzz-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.721741 gattfuzz-0.0.6/gattfuzz/
--rw-rw-rw-   0        0        0     3680 2023-06-07 12:16:32.000000 gattfuzz-0.0.6/gattfuzz/GattFuzz.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.739739 gattfuzz-0.0.6/gattfuzz/lib/
--rw-rw-rw-   0        0        0    15069 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/BLEControl.py
--rw-rw-rw-   0        0        0     1862 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/Logger.py
--rw-rw-rw-   0        0        0     3930 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/PcapProcessor.py
--rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/StringMutator.py
--rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/ValueLCS.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.730737 gattfuzz-0.0.6/gattfuzz.egg-info/
--rw-rw-rw-   0        0        0     1257 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 11:19:53.741737 gattfuzz-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-06-08 11:13:57.000000 gattfuzz-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.516725 gattfuzz-0.0.7/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 11:26:10.515733 gattfuzz-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.487721 gattfuzz-0.0.7/gattfuzz/
+-rw-rw-rw-   0        0        0     3806 2023-06-08 11:20:44.000000 gattfuzz-0.0.7/gattfuzz/GattFuzz.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.511723 gattfuzz-0.0.7/gattfuzz/lib/
+-rw-rw-rw-   0        0        0    15534 2023-06-08 11:20:44.000000 gattfuzz-0.0.7/gattfuzz/lib/BLEControl.py
+-rw-rw-rw-   0        0        0     1852 2023-06-08 11:20:44.000000 gattfuzz-0.0.7/gattfuzz/lib/Logger.py
+-rw-rw-rw-   0        0        0     3930 2023-06-08 11:23:41.000000 gattfuzz-0.0.7/gattfuzz/lib/PcapProcessor.py
+-rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/lib/StringMutator.py
+-rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/lib/ValueLCS.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.500720 gattfuzz-0.0.7/gattfuzz.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:26:10.516725 gattfuzz-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-08 11:22:46.000000 gattfuzz-0.0.7/setup.py
```

### Comparing `gattfuzz-0.0.6/PKG-INFO` & `gattfuzz-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.6/README.md` & `gattfuzz-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.6/gattfuzz/GattFuzz.py` & `gattfuzz-0.0.7/gattfuzz/GattFuzz.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,113 +1,114 @@
-from gattfuzz.lib.ValueLCS import ValueLCS
-from gattfuzz.lib.PcapProcessor import PcapProcessor
-from gattfuzz.lib.BLEControl import BLEControl
-from scapy.all import *
-import argparse
-
-from gattfuzz.lib.Logger import Logger
-logger = Logger(loggername='Main').get_logger()
-
-
-val = ValueLCS()
-
-'''
-2023.2.8 补充 空pyload
-7.21 一个问题（已解决）
-基于pcap的变异覆盖率
-
-7.21 一个问题
-多次连接才能连上
-'''
-def fuzz_with_pcap(pcap_path,tar_mac):
-    
-    latest_dic = {}
-    #提取数据包 static          
-    logger.info("--开始处理pcap文件--")
-    pcap_processor = PcapProcessor(pcap_path)
-
-    pcap_handles = []
-    han_val_dic = {}
-
-    pcap_handles, han_val_dic = pcap_processor.process_pcap()          # 返回handle列表和{handle：[value]}字典
-    logger.info("--处理pcap文件结束--")
-    # print("pcap handles:", pcap_handles)                # pcap中的handles
-    # print("all_value:", han_val_dic)
-                                      
-
-    # connect device and logger.info chars
-    # logger.info("#"*30+ "设备扫描"+ '#'*30)
-    ble = BLEControl()                 
-    ble.tar_con(tar_mac)
-    bulepy_handles = ble.print_char()                      # 建立连接打印read，并打开所有notification
-    logger.info("bluepy handles:{}".format(str(bulepy_handles)))
-
-    # 存在部分handle不通信的情况，pcap中没有数据，补充这部分
-    for handle in bulepy_handles:
-        # logger.info("handle:{}".format(str(handle))
-        if handle not in pcap_handles:
-            latest_dic[handle] = []
-        else:
-            latest_dic[handle] = han_val_dic[handle]
-    # print("latest pcap dic:", latest_dic)
-    
-    logger.info("--开始变异--")
-    after_Muta_dic = val.pro_dict(latest_dic)              # 进行规则标记、变异，返回变异后字典
-    # TODO add thread
-    
-    # logger.info(after_Muta_dic)
-    # ble.tar_con(tar_mac)
-    # # TODO +判断连接状态
-    ble.write_to_csv(after_Muta_dic)                        # write过程写入csv并写到目标设备handle
-
-def fuzz_without_pcap(tar_mac):
-
-    # just write
-    ble = BLEControl()
-    ble.tar_con(tar_mac)
-    handles = ble.print_char()
-    # print("handles:", handles)
-
-    # 随机变异十次
-    n = 0
-    after_dic = {}
-    while n<100:
-        logger.info("--开始随机变异--")
-        after_dic = val.var_no_pcap(handles)   # 一次变异
-        logger.info("--随机变异结束--")
-        # print("after_dic:", after_dic)
-        n += 1
-
-        time.sleep(10.0)
-        print(ble._conn)
-        logger.info("--开始变异结果写入--")
-        # ble.tar_con(tar_mac)
-        ble.write_to_csv(after_dic)
-        logger.info("--一次Fuzz结束--")
-    
-
-def main():
-    print("""
-       ###     #     #####   #####   ######
-  #   #    #       #       #     #
- #        ###      #       #     #       #    #  #####   #####
- #  ###   # #      #       #     ####    #    #     #       #
- #    #  #####     #       #     #       #    #    #       #
-  #   #  #   #     #       #     #       #   ##   #       #
-   #### ##   ##    #       #     #        ### #  #####   #####
-
-    """)
-    parser = argparse.ArgumentParser()
-    parser.add_argument('-f', '--file', help='input pcap file',required=False)
-    parser.add_argument('-m', '--mac', help='mac address of target', required=True)
-    args = parser.parse_args()
-    
-    pcap_path = args.file
-    target_mac = args.mac
-    # try:
-    if not pcap_path:
-        fuzz_without_pcap(target_mac.lower())
-    else:
-        fuzz_with_pcap(pcap_path, target_mac.lower())
-    # except Exception as e:
-    #     logger.error('[-] fuzz error : {}'.format(e))
-
+from gattfuzz.lib.ValueLCS import ValueLCS
+from gattfuzz.lib.PcapProcessor import PcapProcessor
+from gattfuzz.lib.BLEControl import BLEControl
+from scapy.all import *
+import argparse
+import time
+
+from gattfuzz.lib.Logger import Logger
+logger = Logger(loggername='Main').get_logger()
+
+
+val = ValueLCS()
+
+'''
+2023.2.8 补充 空pyload
+7.21 一个问题（已解决）
+基于pcap的变异覆盖率
+
+7.21 一个问题
+多次连接才能连上
+'''
+def fuzz_with_pcap(pcap_path,tar_mac):
+    
+    latest_dic = {}
+    #提取数据包 static          
+    logger.info("--开始处理pcap文件--")
+    pcap_processor = PcapProcessor(pcap_path)
+
+    pcap_handles = []
+    han_val_dic = {}
+
+    pcap_handles, han_val_dic = pcap_processor.process_pcap()          # 返回handle列表和{handle：[value]}字典
+    logger.info("--处理pcap文件结束--")
+    # print("pcap handles:", pcap_handles)                # pcap中的handles
+    # print("all_value:", han_val_dic)
+                                      
+
+    # connect device and logger.info chars
+    # logger.info("#"*30+ "设备扫描"+ '#'*30)
+    ble = BLEControl()                 
+    ble.tar_con(tar_mac)
+    bulepy_handles = ble.print_char()                      # 建立连接打印read，并打开所有notification
+    logger.info("bluepy handles:{}".format(str(bulepy_handles)))
+
+    # 存在部分handle不通信的情况，pcap中没有数据，补充这部分
+    for handle in bulepy_handles:
+        # logger.info("handle:{}".format(str(handle))
+        if handle not in pcap_handles:
+            latest_dic[handle] = []
+        else:
+            latest_dic[handle] = han_val_dic[handle]
+    # print("latest pcap dic:", latest_dic)
+    
+    logger.info("--开始变异--")
+    after_Muta_dic = val.pro_dict(latest_dic)              # 进行规则标记、变异，返回变异后字典
+    # TODO add thread
+    
+    # logger.info(after_Muta_dic)
+    # ble.tar_con(tar_mac)
+    # # TODO +判断连接状态
+    ble.write_to_csv(after_Muta_dic)                        # write过程写入csv并写到目标设备handle
+
+def fuzz_without_pcap(tar_mac):
+
+    # just write
+    ble = BLEControl()
+    ble.tar_con(tar_mac)
+    handles = ble.print_char()
+    # print("handles:", handles)
+
+    # 随机变异十次
+    n = 0
+    after_dic = {}
+    while n<100:
+        logger.info("--开始随机变异--")
+        after_dic = val.var_no_pcap(handles)   # 一次变异
+        logger.info("--随机变异结束--")
+        # print("after_dic:", after_dic)
+        n += 1
+
+        time.sleep(10.0)
+        print(ble._conn)
+        logger.info("--开始变异结果写入--")
+        # ble.tar_con(tar_mac)
+        ble.write_to_csv(after_dic)
+        logger.info("--一次Fuzz结束--")
+    
+
+def main():
+    print("""
+       ###     #     #####   #####   ######
+  #   #    #       #       #     #
+ #        ###      #       #     #       #    #  #####   #####
+ #  ###   # #      #       #     ####    #    #     #       #
+ #    #  #####     #       #     #       #    #    #       #
+  #   #  #   #     #       #     #       #   ##   #       #
+   #### ##   ##    #       #     #        ### #  #####   #####
+
+    """)
+    parser = argparse.ArgumentParser()
+    parser.add_argument('-f', '--file', help='input pcap file',required=False)
+    parser.add_argument('-m', '--mac', help='mac address of target', required=True)
+    args = parser.parse_args()
+    
+    pcap_path = args.file
+    target_mac = args.mac
+    # try:
+    if not pcap_path:
+        fuzz_without_pcap(target_mac.lower())
+    else:
+        fuzz_with_pcap(pcap_path, target_mac.lower())
+    # except Exception as e:
+    #     logger.error('[-] fuzz error : {}'.format(e))
+
```

### Comparing `gattfuzz-0.0.6/gattfuzz/lib/BLEControl.py` & `gattfuzz-0.0.7/gattfuzz/lib/BLEControl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 from cgitb import enable
-import csv
-import threading
 from bluepy import btle
 from bluepy.btle import Peripheral,UUID,DefaultDelegate,Scanner
 from bluepy.btle import BTLEException
-import _thread
-import time
+
 from gattfuzz.lib.Logger import Logger
 logger = Logger(loggername='Gatt_Write').get_logger()
 
 '''
 connect to target device
 
 #TODO 监听所有notification接口，所有indications属性
@@ -139,99 +136,104 @@
     # hold connect            
     def con_hold(self):
         self.tar_con(self._mac)
         self.open_notify()       # 打开notify
 
     def print_char(self):
         # Get service & characteristic
-        wriList = {}
-        services = self._conn.getServices()
-        han_list = []
-        for svc in services:
-            print("[+]        Service: ", svc.uuid)
-            for n in range(0,10):
-                try:
-                    characteristics = svc.getCharacteristics()
-                    break
-                except:
-                    if n < 10:
-                        continue
-                    else:
-                        logger.warning("Service {} char get error.")
-                        continue
-            for charac in characteristics:
-                uu = charac.uuid
-                Properties = charac.propertiesToString()
-                print("    Characteristic: ", uu)
-                print("        Properties: ", Properties)
-                print("            handle: ", charac.getHandle())
-            
-                # listen notification
-                #     try:
-                #         handl = charac.getHandle()
-                #         notify = threading.Thread(target=self.wait_noti, name=str(handl), args=(handl, ))
-                #         notify.start()                    
-                #     except BTLEException:
-                #         # print(uu + "notify failed!!")
-                #         continue
-
-                # if Properties.find('INDICATE'):
-                #     try:
-                #         handl = charac.getHandle()
-                #         indicate = threading.Thread(target=self.wait_indications, name=str(handl), args=(handl, ))
-                #         indicate.start()                   
-                #     except BTLEException:
-                #         # print(uu + "notify failed!!")
-                #         continue
-
-                # write
-
-                # print(Properties)
-                if 'WRITE' in Properties.replace(" ",""):
-                    # print("write dadian")
-                    han = charac.getHandle()
-                    wriList[svc.uuid]= uu                   #保存service uuid和characteristic uuid 
-                    if han not in han_list:      
-                        han_list.append(han)
-
-                if str(Properties).find('NOTIFY'):
-                    handle = charac.getHandle()
-                    try:
-                        self._conn.writeCharacteristic(handle, b'\x01\x00')  #\x01\x00 for notify
-                    except BTLEException:
-                        logger.warning("Open handle :{} notification error.".format(str(handle)))
-                        continue
-                # listen INDICATE
-                if str(Properties).find('INDICATE'):
-                    handle = charac.getHandle()
+        if self._conn:
+            wriList = {}
+            services = self._conn.getServices()
+            han_list = []
+            for svc in services:
+                print("[+]        Service: ", svc.uuid)
+                for n in range(0,10):
                     try:
-                        self._conn.writeCharacteristic(handle, b'\x02\x00')
-                        # handl = charac.getHandle()
-                        # indicate = threading.Thread(target=self.wait_indications, name=str(handl), args=(handl, ))
-                        # indicate.start()                   
-                    except BTLEException:
-                        # print(uu + "notify failed!!")
-                        logger.warning("Open handle :{} INDICATE error.".format(str(handle)))
-                        continue
+                        characteristics = svc.getCharacteristics()
+                        break
+                    except:
+                        if n < 10:
+                            continue
+                        else:
+                            logger.warning("Service {} char get error.")
+                            continue
+                for charac in characteristics:
+                    uu = charac.uuid
+                    Properties = charac.propertiesToString()
+                    print("    Characteristic: ", uu)
+                    print("        Properties: ", Properties)
+                    print("            handle: ", charac.getHandle())
                 
-                # 很神奇，read操作会影响write属性的判断
-                # read
-                if charac.supportsRead():
-                    try:
-                        value = charac.read()
-                        print("             Value: ", value)
-                        print("            charac: ", charac)
-                    except BTLEException:
-                        # print(uu+" read failed!!")
-                        continue 
+                    # listen notification
+                    #     try:
+                    #         handl = charac.getHandle()
+                    #         notify = threading.Thread(target=self.wait_noti, name=str(handl), args=(handl, ))
+                    #         notify.start()                    
+                    #     except BTLEException:
+                    #         # print(uu + "notify failed!!")
+                    #         continue
+
+                    # if Properties.find('INDICATE'):
+                    #     try:
+                    #         handl = charac.getHandle()
+                    #         indicate = threading.Thread(target=self.wait_indications, name=str(handl), args=(handl, ))
+                    #         indicate.start()                   
+                    #     except BTLEException:
+                    #         # print(uu + "notify failed!!")
+                    #         continue
+
+                    # write
+
+                    # print(Properties)
+                    if 'WRITE' in Properties.replace(" ",""):
+                        # print("write dadian")
+                        han = charac.getHandle()
+                        wriList[svc.uuid]= uu                   #保存service uuid和characteristic uuid 
+                        if han not in han_list:      
+                            han_list.append(han)
+
+                    if str(Properties).find('NOTIFY'):
+                        handle = charac.getHandle()
+                        try:
+                            self._conn.writeCharacteristic(handle, b'\x01\x00')  #\x01\x00 for notify
+                        except BTLEException:
+                            logger.warning("Open handle :{} notification error.".format(str(handle)))
+                            continue
+                    # listen INDICATE
+                    if str(Properties).find('INDICATE'):
+                        handle = charac.getHandle()
+                        try:
+                            self._conn.writeCharacteristic(handle, b'\x02\x00')
+                            # handl = charac.getHandle()
+                            # indicate = threading.Thread(target=self.wait_indications, name=str(handl), args=(handl, ))
+                            # indicate.start()                   
+                        except BTLEException:
+                            # print(uu + "notify failed!!")
+                            logger.warning("Open handle :{} INDICATE error.".format(str(handle)))
+                            continue
+                    
+                    # 很神奇，read操作会影响write属性的判断
+                    # read
+                    if charac.supportsRead():
+                        try:
+                            value = charac.read()
+                            print("             Value: ", value)
+                            print("            charac: ", charac)
+                        except BTLEException:
+                            # print(uu+" read failed!!")
+                            continue 
 
-                
-            print(60*'-')
-        # self._conn.disconnect()
-        return han_list                     # 遍历pher设备handler，防止pcap包不全
+                    
+                print(60*'-')
+            # self._conn.disconnect()
+            return han_list                     # 遍历pher设备handler，防止pcap包不全
+        else:
+            logger.info("连接断开，尝试重连...")
+            self.con_hold()
+            self.print_char()
 
     def wri_value(self, handle, val):
 
         if type(val) != bytes:
             val = val.encode()
         try:
             respon = self._conn.writeCharacteristic(handle, val, withResponse=True)                  ## python3.*  type(val)=byte
@@ -239,15 +241,17 @@
             self._conn.waitForNotifications(2.0)                                                     # 监听notify
         except BTLEException  as ex:
             logger.info("GATT write no response.")                                                  
 
     def open_notify(self):
         wriList = {}
         services = self._conn.getServices()
+        
         for svc in services:
+            characteristics = []
             for n in range(0,5):
                 try:
                     characteristics = svc.getCharacteristics()
                     break
                 except:
                     if n < 5:
                         continue
```

### Comparing `gattfuzz-0.0.6/gattfuzz/lib/Logger.py` & `gattfuzz-0.0.7/gattfuzz/lib/Logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import logging
 from colorama import Fore,Style
-import sys
+
 
 class Logger():
     def __init__(self, loglevel=logging.INFO, loggername=None):
         self.logger = logging.getLogger(loggername)
         self.logger.setLevel(loglevel)
 
         formatter = logging.Formatter('%(asctime)s %(filename)s[line:%(lineno)d] %(levelname)s %(message)s')
```

### Comparing `gattfuzz-0.0.6/gattfuzz/lib/PcapProcessor.py` & `gattfuzz-0.0.7/gattfuzz/lib/PcapProcessor.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.6/gattfuzz/lib/StringMutator.py` & `gattfuzz-0.0.7/gattfuzz/lib/StringMutator.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.6/gattfuzz/lib/ValueLCS.py` & `gattfuzz-0.0.7/gattfuzz/lib/ValueLCS.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.6/gattfuzz.egg-info/PKG-INFO` & `gattfuzz-0.0.7/gattfuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.6
+Version: 0.0.7
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.6/setup.py` & `gattfuzz-0.0.7/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from setuptools import setup, find_packages
-
-with open("README.md", "r", encoding="utf-8") as fp:
-    description = fp.read()
-
-setup(
-    name='gattfuzz',
-    version='0.0.6',
-    description= "A tool for fuzzing BLE GATT",
-    long_description=description,
-    packages=find_packages(),
-    #packages=['gattfuzz'],
-    zip_safe=False,
-    install_requires=[
-        'bluepy==1.3.0',
-        'scapy==2.4.5',
-    ],
-    python_requires=">=3.6",
-    entry_points={
-        'console_scripts': [
-            'gattfuzz=gattfuzz.GattFuzz:main',
-        ]
-    }
-)
+from setuptools import setup, find_packages
+
+with open("README.md", "r", encoding="utf-8") as fp:
+    description = fp.read()
+
+setup(
+    name='gattfuzz',
+    version='0.0.7',
+    description= "A tool for fuzzing BLE GATT",
+    long_description=description,
+    packages=find_packages(),
+    #packages=['gattfuzz'],
+    zip_safe=False,
+    install_requires=[
+        'bluepy==1.3.0',
+        'scapy==2.4.5',
+    ],
+    python_requires=">=3.6",
+    entry_points={
+        'console_scripts': [
+            'gattfuzz=gattfuzz.GattFuzz:main',
+        ]
+    }
+)
```

