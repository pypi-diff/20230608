# Comparing `tmp/gattfuzz-0.0.7.tar.gz` & `tmp/gattfuzz-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattfuzz-0.0.7.tar", last modified: Thu Jun  8 11:26:10 2023, max compression
+gzip compressed data, was "gattfuzz-0.0.8.tar", last modified: Thu Jun  8 11:58:09 2023, max compression
```

## Comparing `gattfuzz-0.0.7.tar` & `gattfuzz-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.516725 gattfuzz-0.0.7/
--rw-rw-rw-   0        0        0     1257 2023-06-08 11:26:10.515733 gattfuzz-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.487721 gattfuzz-0.0.7/gattfuzz/
--rw-rw-rw-   0        0        0     3806 2023-06-08 11:20:44.000000 gattfuzz-0.0.7/gattfuzz/GattFuzz.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.511723 gattfuzz-0.0.7/gattfuzz/lib/
--rw-rw-rw-   0        0        0    15534 2023-06-08 11:20:44.000000 gattfuzz-0.0.7/gattfuzz/lib/BLEControl.py
--rw-rw-rw-   0        0        0     1852 2023-06-08 11:20:44.000000 gattfuzz-0.0.7/gattfuzz/lib/Logger.py
--rw-rw-rw-   0        0        0     3930 2023-06-08 11:23:41.000000 gattfuzz-0.0.7/gattfuzz/lib/PcapProcessor.py
--rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/lib/StringMutator.py
--rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/lib/ValueLCS.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.7/gattfuzz/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-08 11:26:10.500720 gattfuzz-0.0.7/gattfuzz.egg-info/
--rw-rw-rw-   0        0        0     1257 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 11:26:10.000000 gattfuzz-0.0.7/gattfuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-08 11:26:10.516725 gattfuzz-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      581 2023-06-08 11:22:46.000000 gattfuzz-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.036239 gattfuzz-0.0.8/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 11:58:09.035239 gattfuzz-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.018240 gattfuzz-0.0.8/gattfuzz/
+-rw-rw-rw-   0        0        0     3807 2023-06-08 11:45:19.000000 gattfuzz-0.0.8/gattfuzz/GattFuzz.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.034240 gattfuzz-0.0.8/gattfuzz/lib/
+-rw-rw-rw-   0        0        0    15846 2023-06-08 11:55:52.000000 gattfuzz-0.0.8/gattfuzz/lib/BLEControl.py
+-rw-rw-rw-   0        0        0     1852 2023-06-08 11:20:44.000000 gattfuzz-0.0.8/gattfuzz/lib/Logger.py
+-rw-rw-rw-   0        0        0     3930 2023-06-08 11:23:41.000000 gattfuzz-0.0.8/gattfuzz/lib/PcapProcessor.py
+-rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/lib/StringMutator.py
+-rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/lib/ValueLCS.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.8/gattfuzz/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:58:09.027237 gattfuzz-0.0.8/gattfuzz.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 11:58:08.000000 gattfuzz-0.0.8/gattfuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:58:09.036239 gattfuzz-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      581 2023-06-08 11:57:34.000000 gattfuzz-0.0.8/setup.py
```

### Comparing `gattfuzz-0.0.7/PKG-INFO` & `gattfuzz-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.7/README.md` & `gattfuzz-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.7/gattfuzz/GattFuzz.py` & `gattfuzz-0.0.8/gattfuzz/GattFuzz.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         logger.info("--开始随机变异--")
         after_dic = val.var_no_pcap(handles)   # 一次变异
         logger.info("--随机变异结束--")
         # print("after_dic:", after_dic)
         n += 1
 
         time.sleep(10.0)
-        print(ble._conn)
+        #print(ble._conn)
         logger.info("--开始变异结果写入--")
         # ble.tar_con(tar_mac)
         ble.write_to_csv(after_dic)
         logger.info("--一次Fuzz结束--")
     
 
 def main():
```

### Comparing `gattfuzz-0.0.7/gattfuzz/lib/BLEControl.py` & `gattfuzz-0.0.8/gattfuzz/lib/BLEControl.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,17 +19,25 @@
     
     def handleNotification(self, cHandle, data):
         logger.error("Recevied handle: {}  nofity  ----> {} ".format(str(cHandle), str(data)))
 
 
 
 class BLEControl():
- 
+
+    def __init__(self, custom_logger=None):
+        self._conn = None
+        if custom_logger:
+            self.logger = custom_logger
+        else:
+            self.logger = logger
+    
     # connect to target mac
     def tar_con(self, tar_mac):
+        logger = self.logger
         logger.info("Begin sacn")
         n = 1
         scanner = Scanner()
         devices = scanner.scan(timeout=10)
         logger.info("发现 %d 个设备", len(devices))          
         for dev in devices:    
             if dev.addr==tar_mac:
@@ -135,14 +143,15 @@
     
     # hold connect            
     def con_hold(self):
         self.tar_con(self._mac)
         self.open_notify()       # 打开notify
 
     def print_char(self):
+        logger = self.logger
         # Get service & characteristic
         if self._conn:
             wriList = {}
             services = self._conn.getServices()
             han_list = []
             for svc in services:
                 print("[+]        Service: ", svc.uuid)
@@ -239,14 +248,15 @@
             respon = self._conn.writeCharacteristic(handle, val, withResponse=True)                  ## python3.*  type(val)=byte
             logger.error("Write: {} to: {}  response: {}".format(str(val),str(handle),respon))       # 监听返回值
             self._conn.waitForNotifications(2.0)                                                     # 监听notify
         except BTLEException  as ex:
             logger.info("GATT write no response.")                                                  
 
     def open_notify(self):
+        logger = self.logger
         wriList = {}
         services = self._conn.getServices()
         
         for svc in services:
             characteristics = []
             for n in range(0,5):
                 try:
@@ -280,15 +290,15 @@
                         # indicate.start()                   
                     except BTLEException:
                         # print(uu + "notify failed!!")
                         logger.warning("Open handle :{} INDICATE error.".format(str(handle)))
                         continue
 
     def write_to_csv(self, after_Muta_dic):
-
+        logger = self.logger
         for handle in after_Muta_dic.keys():
             # self.path = './'+ str(handle) +'.csv'                               #把变异数据写入./fuzz_data.csv 
             
 
             # with open(self.path, 'w+', newline='') as f:
             #     csv_doc = csv.writer(f)
```

### Comparing `gattfuzz-0.0.7/gattfuzz/lib/Logger.py` & `gattfuzz-0.0.8/gattfuzz/lib/Logger.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.7/gattfuzz/lib/PcapProcessor.py` & `gattfuzz-0.0.8/gattfuzz/lib/PcapProcessor.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.7/gattfuzz/lib/StringMutator.py` & `gattfuzz-0.0.8/gattfuzz/lib/StringMutator.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.7/gattfuzz/lib/ValueLCS.py` & `gattfuzz-0.0.8/gattfuzz/lib/ValueLCS.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.7/gattfuzz.egg-info/PKG-INFO` & `gattfuzz-0.0.8/gattfuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.7
+Version: 0.0.8
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.7/setup.py` & `gattfuzz-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fp:
     description = fp.read()
 
 setup(
     name='gattfuzz',
-    version='0.0.7',
+    version='0.0.8',
     description= "A tool for fuzzing BLE GATT",
     long_description=description,
     packages=find_packages(),
     #packages=['gattfuzz'],
     zip_safe=False,
     install_requires=[
         'bluepy==1.3.0',
```

