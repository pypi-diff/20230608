# Comparing `tmp/gattfuzz-0.0.5.tar.gz` & `tmp/gattfuzz-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gattfuzz-0.0.5.tar", last modified: Wed Jun  7 12:41:53 2023, max compression
+gzip compressed data, was "gattfuzz-0.0.6.tar", last modified: Thu Jun  8 11:19:53 2023, max compression
```

## Comparing `gattfuzz-0.0.5.tar` & `gattfuzz-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 12:41:53.682284 gattfuzz-0.0.5/
--rw-rw-rw-   0        0        0     1257 2023-06-07 12:41:53.682284 gattfuzz-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-06-07 12:41:53.666649 gattfuzz-0.0.5/gattfuzz/
--rw-rw-rw-   0        0        0     3680 2023-06-07 12:16:32.000000 gattfuzz-0.0.5/gattfuzz/GattFuzz.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:41:53.666649 gattfuzz-0.0.5/gattfuzz/lib/
--rw-rw-rw-   0        0        0    15069 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/lib/BLEControl.py
--rw-rw-rw-   0        0        0     1862 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/lib/Logger.py
--rw-rw-rw-   0        0        0     3930 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/lib/PcapProcessor.py
--rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/lib/StringMutator.py
--rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/lib/ValueLCS.py
--rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.5/gattfuzz/lib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 12:41:53.666649 gattfuzz-0.0.5/gattfuzz.egg-info/
--rw-rw-rw-   0        0        0     1257 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      445 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       27 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-06-07 12:41:53.000000 gattfuzz-0.0.5/gattfuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-07 12:41:53.682284 gattfuzz-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      557 2023-06-07 12:36:53.000000 gattfuzz-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.741737 gattfuzz-0.0.6/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 11:19:53.741737 gattfuzz-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1138 2023-06-07 12:36:00.000000 gattfuzz-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.721741 gattfuzz-0.0.6/gattfuzz/
+-rw-rw-rw-   0        0        0     3680 2023-06-07 12:16:32.000000 gattfuzz-0.0.6/gattfuzz/GattFuzz.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.739739 gattfuzz-0.0.6/gattfuzz/lib/
+-rw-rw-rw-   0        0        0    15069 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/BLEControl.py
+-rw-rw-rw-   0        0        0     1862 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/Logger.py
+-rw-rw-rw-   0        0        0     3930 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/PcapProcessor.py
+-rw-rw-rw-   0        0        0     6805 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/StringMutator.py
+-rw-rw-rw-   0        0        0    17716 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/ValueLCS.py
+-rw-rw-rw-   0        0        0        0 2023-06-07 12:32:32.000000 gattfuzz-0.0.6/gattfuzz/lib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 11:19:53.730737 gattfuzz-0.0.6/gattfuzz.egg-info/
+-rw-rw-rw-   0        0        0     1257 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      445 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       27 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-06-08 11:19:53.000000 gattfuzz-0.0.6/gattfuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 11:19:53.741737 gattfuzz-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      557 2023-06-08 11:13:57.000000 gattfuzz-0.0.6/setup.py
```

### Comparing `gattfuzz-0.0.5/PKG-INFO` & `gattfuzz-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.5/README.md` & `gattfuzz-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz/GattFuzz.py` & `gattfuzz-0.0.6/gattfuzz/GattFuzz.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz/lib/BLEControl.py` & `gattfuzz-0.0.6/gattfuzz/lib/BLEControl.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz/lib/Logger.py` & `gattfuzz-0.0.6/gattfuzz/lib/Logger.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz/lib/PcapProcessor.py` & `gattfuzz-0.0.6/gattfuzz/lib/PcapProcessor.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz/lib/StringMutator.py` & `gattfuzz-0.0.6/gattfuzz/lib/StringMutator.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz/lib/ValueLCS.py` & `gattfuzz-0.0.6/gattfuzz/lib/ValueLCS.py`

 * *Files identical despite different names*

### Comparing `gattfuzz-0.0.5/gattfuzz.egg-info/PKG-INFO` & `gattfuzz-0.0.6/gattfuzz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gattfuzz
-Version: 0.0.5
+Version: 0.0.6
 Summary: A tool for fuzzing BLE GATT
 Requires-Python: >=3.6
 
 # GattFuzz
 GattFuzz 是一款针对BLE Gatt的模糊测试工具。
 
 ### 环境
```

### Comparing `gattfuzz-0.0.5/setup.py` & `gattfuzz-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fp:
     description = fp.read()
 
 setup(
     name='gattfuzz',
-    version='0.0.5',
+    version='0.0.6',
     description= "A tool for fuzzing BLE GATT",
     long_description=description,
     packages=find_packages(),
     #packages=['gattfuzz'],
     zip_safe=False,
     install_requires=[
         'bluepy==1.3.0',
```

