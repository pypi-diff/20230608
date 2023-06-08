# Comparing `tmp/wpcsys-2.1.2.tar.gz` & `tmp/wpcsys-2.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wpcsys-2.1.2.tar", last modified: Mon Jun  5 06:51:42 2023, max compression
+gzip compressed data, was "wpcsys-2.1.4.tar", last modified: Thu Jun  8 05:37:00 2023, max compression
```

## Comparing `wpcsys-2.1.2.tar` & `wpcsys-2.1.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 06:51:42.462447 wpcsys-2.1.2/
--rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.2/LICENSE
--rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0     9924 2023-06-05 06:51:42.455429 wpcsys-2.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     8863 2023-06-05 06:31:04.000000 wpcsys-2.1.2/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-05 06:51:42.463430 wpcsys-2.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-05 06:51:42.403247 wpcsys-2.1.2/wpcsys/
--rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.2/wpcsys/__init__.py
--rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.2/wpcsys/libusb-1.0.dll
--rw-rw-rw-   0        0        0  6996992 2023-06-05 06:49:32.000000 wpcsys-2.1.2/wpcsys/pywpc.cp310-win_amd64.pyd
--rw-rw-rw-   0        0        0  7545344 2023-06-05 06:50:46.000000 wpcsys-2.1.2/wpcsys/pywpc.cp38-win_amd64.pyd
--rw-rw-rw-   0        0        0  7555072 2023-06-05 06:50:13.000000 wpcsys-2.1.2/wpcsys/pywpc.cp39-win_amd64.pyd
-drwxrwxrwx   0        0        0        0 2023-06-05 06:51:42.452429 wpcsys-2.1.2/wpcsys.egg-info/
--rw-rw-rw-   0        0        0     9924 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      326 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      152 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-05 06:51:42.000000 wpcsys-2.1.2/wpcsys.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 05:37:00.902944 wpcsys-2.1.4/
+-rw-rw-rw-   0        0        0     1091 2022-10-03 09:42:47.000000 wpcsys-2.1.4/LICENSE
+-rw-rw-rw-   0        0        0       64 2022-11-04 05:05:00.000000 wpcsys-2.1.4/MANIFEST.in
+-rw-rw-rw-   0        0        0    10325 2023-06-08 05:37:00.893920 wpcsys-2.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     9264 2023-06-08 05:31:19.000000 wpcsys-2.1.4/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-08 05:37:00.902944 wpcsys-2.1.4/setup.cfg
+-rw-rw-rw-   0        0        0     1985 2022-11-23 08:57:09.000000 wpcsys-2.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 05:37:00.839378 wpcsys-2.1.4/wpcsys/
+-rw-rw-rw-   0        0        0        0 2022-10-06 03:03:31.000000 wpcsys-2.1.4/wpcsys/__init__.py
+-rw-rw-rw-   0        0        0  1292959 2023-02-08 04:26:34.000000 wpcsys-2.1.4/wpcsys/libusb-1.0.dll
+-rw-rw-rw-   0        0        0  7016448 2023-06-08 05:33:58.000000 wpcsys-2.1.4/wpcsys/pywpc.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0  7566336 2023-06-08 05:36:18.000000 wpcsys-2.1.4/wpcsys/pywpc.cp38-win_amd64.pyd
+-rw-rw-rw-   0        0        0  7575552 2023-06-08 05:34:38.000000 wpcsys-2.1.4/wpcsys/pywpc.cp39-win_amd64.pyd
+drwxrwxrwx   0        0        0        0 2023-06-08 05:37:00.892032 wpcsys-2.1.4/wpcsys.egg-info/
+-rw-rw-rw-   0        0        0    10325 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      326 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      152 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-08 05:37:00.000000 wpcsys-2.1.4/wpcsys.egg-info/top_level.txt
```

### Comparing `wpcsys-2.1.2/LICENSE` & `wpcsys-2.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.2/PKG-INFO` & `wpcsys-2.1.4/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.2
+Version: 2.1.4
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.0.0>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.4>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -88,15 +88,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -154,21 +154,23 @@
 
 - USB-DAQ-F1-AOD (Digital + AI + AO)
 
 Wifi based DAQ card
 
 - Wifi-DAQ-E3-A
 
-I/O Function Table
-------------------
+- Wifi-DAQ-F4-A
+
+I/O port function table
+-----------------------
 
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| STEM           |1,3,4|1,3,4|0~7 |0~7 |    |     |     |     |    |   |      |
+| STEM           |1,2,4|1,2,4|0~7 |0~7 |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
@@ -188,14 +190,19 @@
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Wifi-DAQ-F4-A  |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+
+In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
+Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
```

### Comparing `wpcsys-2.1.2/README.rst` & `wpcsys-2.1.4/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.0.0>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.4>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -64,15 +64,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -130,21 +130,23 @@
 
 - USB-DAQ-F1-AOD (Digital + AI + AO)
 
 Wifi based DAQ card
 
 - Wifi-DAQ-E3-A
 
-I/O Function Table
-------------------
+- Wifi-DAQ-F4-A
+
+I/O port function table
+-----------------------
 
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| STEM           |1,3,4|1,3,4|0~7 |0~7 |    |     |     |     |    |   |      |
+| STEM           |1,2,4|1,2,4|0~7 |0~7 |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
@@ -164,14 +166,19 @@
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Wifi-DAQ-F4-A  |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+
+In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
+Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
```

### Comparing `wpcsys-2.1.2/setup.py` & `wpcsys-2.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.2/wpcsys/libusb-1.0.dll` & `wpcsys-2.1.4/wpcsys/libusb-1.0.dll`

 * *Files identical despite different names*

### Comparing `wpcsys-2.1.2/wpcsys.egg-info/PKG-INFO` & `wpcsys-2.1.4/wpcsys.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wpcsys
-Version: 2.1.2
+Version: 2.1.4
 Summary: WPC Python driver APIs, the easiest way to Control & Data Acquisition (DAQ)
 Home-page: https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release
 Author: chunglee_people, Chieh-An Lin
 Author-email: wu@wpc.com.tw
 License: MIT
 Keywords: wpc,daq,driver,usb,ethernet,wifi,data acquisition
 Classifier: Development Status :: 5 - Production/Stable
@@ -34,15 +34,15 @@
 
 Asynchronous mode means that processes run independently of each other and don't wait for the completion of the previous process. Instead, each process runs on its own, without blocking the execution of other processes.
 
 In general, synchronous mode is easier to understand and debug, while asynchronous mode is more scalable and allows for greater concurrency.
 
 Some API functions in the `pywpc` package may not compatible with earlier versions of WPC DAQ firmware.
 To update device firmware to the latest version, please use WPC Device Manager and `LabVIEW Run-time engine <https://drive.google.com/file/d/1Uj6r65KhNxvuApiqrMkZp-NWyq-Eek-k/view>`_.
-You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.0.0>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
+You can download WPC Device Manager by `latest release <https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release/releases/tag/v2.1.4>`_ or visit `WPC Systems Ltd. official website <http://www.wpc.com.tw/>`_.
 
 +-------------------+-----------------------------------------------------------------------------------+
 |                   | Link                                                                              |
 +===================+===================================================================================+
 | WPC official site | http://www.wpc.com.tw/                                                            |
 +-------------------+-----------------------------------------------------------------------------------+
 | GitHub            | https://github.com/WPC-Systems-Ltd/WPC_Python_driver_release                      |
@@ -88,15 +88,15 @@
 -----------
 **Easy, fast, and just works!**
 
    >>> from wpcsys import pywpc
    >>> pywpc.PKG_NAME
    pywpc
    >>> pywpc.HANDLE_LIST
-   ['DeviceFinder', 'WifiDAQE3A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
+   ['DeviceFinder', 'WifiDAQE3A', 'WifiDAQF4A', 'STEM', 'EMotion', 'EthanA', 'EthanD', 'EthanL', 'EthanO', 'USBDAQF1D', 'USBDAQF1DSNK', 'USBDAQF1AD', 'USBDAQF1AOD', 'USBDAQF1TD', 'USBDAQF1RD', 'USBDAQF1CD']
 
 Install and Upgrade
 -------------------
 
 - Install
 
 .. code-block:: shell
@@ -154,21 +154,23 @@
 
 - USB-DAQ-F1-AOD (Digital + AI + AO)
 
 Wifi based DAQ card
 
 - Wifi-DAQ-E3-A
 
-I/O Function Table
-------------------
+- Wifi-DAQ-F4-A
+
+I/O port function table
+-----------------------
 
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Model          |AI   |AO   |DI  |DO  |CAN |UART |SPI  |I2C  |RTD |TC |Motion|
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
-| STEM           |1,3,4|1,3,4|0~7 |0~7 |    |     |     |     |    |   |      |
+| STEM           |1,2,4|1,2,4|0~7 |0~7 |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Emotion        |     |     |    |    |    |     |     |     |    |   |0     |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Ethan-A        |0    |     |    |    |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Ethan-D        |     |     |1   |0   |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
@@ -188,14 +190,19 @@
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | USB-DAQ-F1-CD  |     |     |0~3 |0~3 |1   |1, 2 |2    |1, 2 |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | USB-DAQ-F1-AOD |0    |0    |0~3 |0~3 |    |1, 2 |     |1, 2 |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
 | Wifi-DAQ-E3-A  |0    |     |    |    |    |     |     |     |    |   |      |
 +----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+| Wifi-DAQ-F4-A  |0    |     |    |    |    |     |     |     |    |   |      |
++----------------+-----+-----+----+----+----+-----+-----+-----+----+---+------+
+
+In the `STEM` product, the values 1, 2, and 4 are used to represent the slots in the AIO.
+Additionally, the DIO ports 0 to 1 are assigned to slot 1, while ports 2 to 3 are assigned to slot 2.
 
 Remark: `TC` stands for `Thermocouple`
 
 Take `USB-DAQ-F1-AOD` for example:
 
 - Port 0 is available for AI
```

