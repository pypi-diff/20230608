# Comparing `tmp/python-selve-new-2.2.8.tar.gz` & `tmp/python-selve-new-2.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-selve-new-2.2.8.tar", last modified: Mon Jun  5 09:29:53 2023, max compression
+gzip compressed data, was "python-selve-new-2.2.9.tar", last modified: Mon Jun  5 09:30:51 2023, max compression
```

## Comparing `python-selve-new-2.2.8.tar` & `python-selve-new-2.2.9.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:53.350376 python-selve-new-2.2.8/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-05 09:29:53.350376 python-selve-new-2.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:53.346376 python-selve-new-2.2.8/python_selve_new.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-05 09:29:53.000000 python-selve-new-2.2.8/python_selve_new.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-05 09:29:53.000000 python-selve-new-2.2.8/python_selve_new.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:29:53.000000 python-selve-new-2.2.8/python_selve_new.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 09:29:53.000000 python-selve-new-2.2.8/python_selve_new.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 09:29:53.000000 python-selve-new-2.2.8/python_selve_new.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:53.346376 python-selve-new-2.2.8/selve/
--rw-r--r--   0 runner    (1001) docker     (123)    66558 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:53.350376 python-selve-new-2.2.8/selve/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/device.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/param.py
--rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/commands/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/device.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/gateway.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/group.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/iveo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/senSim.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/sender.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:29:53.350376 python-selve-new-2.2.8/selve/util/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/selve/util/protocol.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:29:53.350376 python-selve-new-2.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-05 09:29:48.000000 python-selve-new-2.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/python_selve_new.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-06-05 09:30:51.000000 python-selve-new-2.2.9/python_selve_new.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-06-05 09:30:51.000000 python-selve-new-2.2.9/python_selve_new.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 09:30:51.000000 python-selve-new-2.2.9/python_selve_new.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-05 09:30:51.000000 python-selve-new-2.2.9/python_selve_new.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-05 09:30:51.000000 python-selve-new-2.2.9/python_selve_new.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/selve/
+-rw-r--r--   0 runner    (1001) docker     (123)    66557 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/selve/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6658 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4550 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/param.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5956 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3801 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/commands/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/iveo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/senSim.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/selve/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/selve/util/protocol.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-05 09:30:51.749959 python-selve-new-2.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3163 2023-06-05 09:30:46.000000 python-selve-new-2.2.9/setup.py
```

### Comparing `python-selve-new-2.2.8/LICENSE` & `python-selve-new-2.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/PKG-INFO` & `python-selve-new-2.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.2.8/python_selve_new.egg-info/PKG-INFO` & `python-selve-new-2.2.9/python_selve_new.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-selve-new
-Version: 2.2.8
+Version: 2.2.9
 Summary: Python library for interfacing with selve devices using the USB-RF controller. Written completely new.
 Home-page: https://github.com/Kannix2005/python-selve-new
 Author: Stefan Altheimer
 Author-email: me@stefan-altheimer.de
 Keywords: selve blind awning shutter usb rf
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Information Technology
```

### Comparing `python-selve-new-2.2.8/python_selve_new.egg-info/SOURCES.txt` & `python-selve-new-2.2.9/python_selve_new.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/__init__.py` & `python-selve-new-2.2.9/selve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                                     await self.processResponse(msg)
 
                                     # if msg.rstrip() == b' ':
                                     self._LOGGER.debug(f'(Selve Worker): Worker received: {msg}')
                 if self._stopThread.is_set():
                     self._LOGGER.debug("(Selve Worker): " + 'Exiting worker loop...')
                     break
-                await asyncio.sleep(0.01)
+                await asyncio.sleep(0.5)
             return True
         # serial port exceptions, all of these notify that we are in some
         # serious trouble
         except serial.SerialException:
             # log message
             self._LOGGER.error("(Selve Worker): " + 'Serial Port RX error')
```

### Comparing `python-selve-new-2.2.8/selve/commands/command.py` & `python-selve-new-2.2.9/selve/commands/command.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/device.py` & `python-selve-new-2.2.9/selve/commands/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/event.py` & `python-selve-new-2.2.9/selve/commands/event.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/group.py` & `python-selve-new-2.2.9/selve/commands/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/iveo.py` & `python-selve-new-2.2.9/selve/commands/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/param.py` & `python-selve-new-2.2.9/selve/commands/param.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/senSim.py` & `python-selve-new-2.2.9/selve/commands/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/sender.py` & `python-selve-new-2.2.9/selve/commands/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/sensor.py` & `python-selve-new-2.2.9/selve/commands/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/commands/service.py` & `python-selve-new-2.2.9/selve/commands/service.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/device.py` & `python-selve-new-2.2.9/selve/device.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/group.py` & `python-selve-new-2.2.9/selve/group.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/iveo.py` & `python-selve-new-2.2.9/selve/iveo.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/senSim.py` & `python-selve-new-2.2.9/selve/senSim.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/sender.py` & `python-selve-new-2.2.9/selve/sender.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/sensor.py` & `python-selve-new-2.2.9/selve/sensor.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/util/__init__.py` & `python-selve-new-2.2.9/selve/util/__init__.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/util/errors.py` & `python-selve-new-2.2.9/selve/util/errors.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/selve/util/protocol.py` & `python-selve-new-2.2.9/selve/util/protocol.py`

 * *Files identical despite different names*

### Comparing `python-selve-new-2.2.8/setup.py` & `python-selve-new-2.2.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 
 setup(
     
     name='python-selve-new',  # Required    
-    version='2.2.8',  # Required
+    version='2.2.9',  # Required
     description='Python library for interfacing with selve devices using the USB-RF controller. Written completely new.',  # Required   
     long_description=long_description,  # Optional 
     long_description_content_type="text/markdown",   
     url='https://github.com/Kannix2005/python-selve-new',  # Optional
     author='Stefan Altheimer',  # Optional
    
     author_email='me@stefan-altheimer.de',  # Optional
```

