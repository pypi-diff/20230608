# Comparing `tmp/minidevice-1.0.6.tar.gz` & `tmp/minidevice-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minidevice-1.0.6.tar", last modified: Mon Jun  5 08:23:41 2023, max compression
+gzip compressed data, was "minidevice-1.0.7.tar", last modified: Wed Jun  7 14:57:10 2023, max compression
```

## Comparing `minidevice-1.0.6.tar` & `minidevice-1.0.7.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.168431 minidevice-1.0.6/
--rw-rw-rw-   0        0        0     1394 2023-06-05 08:23:41.166478 minidevice-1.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.017789 minidevice-1.0.6/minidevice/
--rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.6/minidevice/__init__.py
--rw-rw-rw-   0        0        0     3583 2023-06-02 05:28:24.000000 minidevice-1.0.6/minidevice/adb.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.157651 minidevice-1.0.6/minidevice/bin/
--rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.6/minidevice/bin/AdbWinApi.dll
--rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.6/minidevice/bin/AdbWinUsbApi.dll
--rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.6/minidevice/bin/adb.exe
--rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.6/minidevice/config.py
--rw-rw-rw-   0        0        0     2775 2023-06-05 08:21:57.000000 minidevice-1.0.6/minidevice/device.py
--rw-rw-rw-   0        0        0     2267 2023-06-01 01:26:18.000000 minidevice-1.0.6/minidevice/minicap.py
--rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.6/minidevice/minitouch.py
--rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.6/minidevice/utils.py
-drwxrwxrwx   0        0        0        0 2023-06-05 08:23:41.049750 minidevice-1.0.6/minidevice.egg-info/
--rw-rw-rw-   0        0        0     1394 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      420 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       90 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-05 08:23:40.000000 minidevice-1.0.6/minidevice.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-05 08:23:41.168431 minidevice-1.0.6/setup.cfg
--rw-rw-rw-   0        0        0      944 2023-06-05 08:22:12.000000 minidevice-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:57:10.892970 minidevice-1.0.7/
+-rw-rw-rw-   0        0        0     1394 2023-06-07 14:57:10.892970 minidevice-1.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     1090 2023-06-01 04:04:50.000000 minidevice-1.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-06-07 14:57:10.781672 minidevice-1.0.7/minidevice/
+-rw-rw-rw-   0        0        0       30 2023-06-01 03:24:16.000000 minidevice-1.0.7/minidevice/__init__.py
+-rw-rw-rw-   0        0        0     3583 2023-06-02 05:28:24.000000 minidevice-1.0.7/minidevice/adb.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:57:10.879749 minidevice-1.0.7/minidevice/bin/
+-rw-rw-rw-   0        0        0    97792 2023-03-12 01:13:21.000000 minidevice-1.0.7/minidevice/bin/AdbWinApi.dll
+-rw-rw-rw-   0        0        0    62976 2023-03-12 01:13:21.000000 minidevice-1.0.7/minidevice/bin/AdbWinUsbApi.dll
+-rwxrwxrwx   0        0        0  6021632 2023-03-12 01:13:21.000000 minidevice-1.0.7/minidevice/bin/adb.exe
+-rw-rw-rw-   0        0        0      285 2023-06-01 04:18:26.000000 minidevice-1.0.7/minidevice/config.py
+-rw-rw-rw-   0        0        0     2775 2023-06-05 08:21:57.000000 minidevice-1.0.7/minidevice/device.py
+-rw-rw-rw-   0        0        0     2266 2023-06-07 14:54:13.000000 minidevice-1.0.7/minidevice/minicap.py
+-rw-rw-rw-   0        0        0      483 2023-06-01 01:14:25.000000 minidevice-1.0.7/minidevice/minitouch.py
+-rw-rw-rw-   0        0        0      261 2023-05-31 10:21:47.000000 minidevice-1.0.7/minidevice/utils.py
+drwxrwxrwx   0        0        0        0 2023-06-07 14:57:10.810866 minidevice-1.0.7/minidevice.egg-info/
+-rw-rw-rw-   0        0        0     1394 2023-06-07 14:57:10.000000 minidevice-1.0.7/minidevice.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      420 2023-06-07 14:57:10.000000 minidevice-1.0.7/minidevice.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 14:57:10.000000 minidevice-1.0.7/minidevice.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       90 2023-06-07 14:57:10.000000 minidevice-1.0.7/minidevice.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-07 14:57:10.000000 minidevice-1.0.7/minidevice.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-07 14:57:10.893947 minidevice-1.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      944 2023-06-07 14:54:33.000000 minidevice-1.0.7/setup.py
```

### Comparing `minidevice-1.0.6/PKG-INFO` & `minidevice-1.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.6
+Version: 1.0.7
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
```

### Comparing `minidevice-1.0.6/README.md` & `minidevice-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.6/minidevice/adb.py` & `minidevice-1.0.7/minidevice/adb.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.6/minidevice/bin/AdbWinApi.dll` & `minidevice-1.0.7/minidevice/bin/AdbWinApi.dll`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.6/minidevice/bin/AdbWinUsbApi.dll` & `minidevice-1.0.7/minidevice/bin/AdbWinUsbApi.dll`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.6/minidevice/bin/adb.exe` & `minidevice-1.0.7/minidevice/bin/adb.exe`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.6/minidevice/device.py` & `minidevice-1.0.7/minidevice/device.py`

 * *Files identical despite different names*

### Comparing `minidevice-1.0.6/minidevice/minicap.py` & `minidevice-1.0.7/minidevice/minicap.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,17 +24,17 @@
 
 def minicap_install(device, sdk, abi):
     """minicap
 
     Args:
         device (_type_): _description_
     """
-
-    if sdk >= 32 and abi == "x86_64":
-        raise Exception("Don't use minicap on x86_64 and Android 12L")
+    #在x86_64上运行32位minicap可正常运行
+    if sdk >= 31 and abi == "x86_64":
+        abi = "x86"
 
 
     MNC_HOME = "/data/local/tmp/minicap"
     MNC_SO_HOME = "/data/local/tmp/minicap.so"
 
     subprocess.run([
         ADB_PATH, "-s", device, "push",
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `minidevice-1.0.6/minidevice.egg-info/PKG-INFO` & `minidevice-1.0.7/minidevice.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minidevice
-Version: 1.0.6
+Version: 1.0.7
 Summary: Android Auto Pypi
 Home-page: https://github.com/NakanoSanku
 Author: KateTseng
 Author-email: Kate.TsengK@outlook.com
 License: MIT
 Keywords: game
 Platform: UNKNOWN
```

### Comparing `minidevice-1.0.6/setup.py` & `minidevice-1.0.7/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import find_packages, setup
 
 with open('README.md', 'r', encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(name='minidevice',
-      version='1.0.6',
+      version='1.0.7',
       description='Android Auto Pypi',
       author='KateTseng',
       author_email='Kate.TsengK@outlook.com',
       long_description=long_description,
       long_description_content_type="text/markdown",
       url='https://github.com/NakanoSanku',
       license='MIT',
```

