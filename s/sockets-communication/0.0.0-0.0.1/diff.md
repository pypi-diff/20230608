# Comparing `tmp/sockets-communication-0.0.0.tar.gz` & `tmp/sockets-communication-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sockets-communication-0.0.0.tar", last modified: Fri Apr 21 18:16:56 2023, max compression
+gzip compressed data, was "sockets-communication-0.0.1.tar", last modified: Thu Jun  8 09:59:31 2023, max compression
```

## Comparing `sockets-communication-0.0.0.tar` & `sockets-communication-0.0.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 18:16:56.229807 sockets-communication-0.0.0/
--rw-rw-rw-   0        0        0       68 2023-04-21 18:16:56.000000 sockets-communication-0.0.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2107 2023-04-21 18:16:56.229807 sockets-communication-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-0.0.0/README.md
--rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 sockets-communication-0.0.0/build.py
--rw-rw-rw-   0        0        0      708 2023-04-21 18:15:57.000000 sockets-communication-0.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-0.0.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 18:16:56.230807 sockets-communication-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1643 2023-04-21 18:09:13.000000 sockets-communication-0.0.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:16:56.222797 sockets-communication-0.0.0/sockets_communication/
--rw-rw-rw-   0        0        0     8199 2023-04-21 18:16:30.000000 sockets-communication-0.0.0/sockets_communication/base.py
--rw-rw-rw-   0        0        0      405 2023-04-21 18:07:48.000000 sockets-communication-0.0.0/sockets_communication/document.py
--rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-0.0.0/sockets_communication/exceptions.py
--rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-0.0.0/sockets_communication/process.py
--rw-rw-rw-   0        0        0    19196 2023-04-21 18:06:50.000000 sockets-communication-0.0.0/sockets_communication/sockets.py
-drwxrwxrwx   0        0        0        0 2023-04-21 18:16:56.228806 sockets-communication-0.0.0/sockets_communication.egg-info/
--rw-rw-rw-   0        0        0     2107 2023-04-21 18:16:56.000000 sockets-communication-0.0.0/sockets_communication.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      461 2023-04-21 18:16:56.000000 sockets-communication-0.0.0/sockets_communication.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 18:16:56.000000 sockets-communication-0.0.0/sockets_communication.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-21 18:16:56.000000 sockets-communication-0.0.0/sockets_communication.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-04-21 18:16:56.000000 sockets-communication-0.0.0/sockets_communication.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 09:59:31.163750 sockets-communication-0.0.1/
+-rw-rw-rw-   0        0        0       68 2023-06-08 09:59:30.000000 sockets-communication-0.0.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     2107 2023-06-08 09:59:31.162750 sockets-communication-0.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1223 2023-04-21 18:12:49.000000 sockets-communication-0.0.1/README.md
+-rw-rw-rw-   0        0        0    12920 2023-03-17 11:14:12.000000 sockets-communication-0.0.1/build.py
+-rw-rw-rw-   0        0        0      708 2023-06-08 09:59:30.000000 sockets-communication-0.0.1/pyproject.toml
+-rw-rw-rw-   0        0        0       29 2023-04-21 18:06:22.000000 sockets-communication-0.0.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-06-08 09:59:31.163750 sockets-communication-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1643 2023-06-08 09:59:26.000000 sockets-communication-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:59:31.147750 sockets-communication-0.0.1/sockets_communication/
+-rw-rw-rw-   0        0        0     8199 2023-04-21 18:16:30.000000 sockets-communication-0.0.1/sockets_communication/base.py
+-rw-rw-rw-   0        0        0      405 2023-04-21 18:07:48.000000 sockets-communication-0.0.1/sockets_communication/document.py
+-rw-rw-rw-   0        0        0     1566 2023-04-12 14:12:33.000000 sockets-communication-0.0.1/sockets_communication/exceptions.py
+-rw-rw-rw-   0        0        0     1604 2023-04-21 18:07:17.000000 sockets-communication-0.0.1/sockets_communication/process.py
+-rw-rw-rw-   0        0        0    19347 2023-06-08 09:57:10.000000 sockets-communication-0.0.1/sockets_communication/sockets.py
+drwxrwxrwx   0        0        0        0 2023-06-08 09:59:31.162750 sockets-communication-0.0.1/sockets_communication.egg-info/
+-rw-rw-rw-   0        0        0     2107 2023-06-08 09:59:31.000000 sockets-communication-0.0.1/sockets_communication.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      461 2023-06-08 09:59:31.000000 sockets-communication-0.0.1/sockets_communication.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 09:59:31.000000 sockets-communication-0.0.1/sockets_communication.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-06-08 09:59:31.000000 sockets-communication-0.0.1/sockets_communication.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-06-08 09:59:31.000000 sockets-communication-0.0.1/sockets_communication.egg-info/top_level.txt
```

### Comparing `sockets-communication-0.0.0/PKG-INFO` & `sockets-communication-0.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 0.0.0
+Version: 0.0.1
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sockets-communication-0.0.0/README.md` & `sockets-communication-0.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sockets-communication-0.0.0/build.py` & `sockets-communication-0.0.1/build.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-0.0.0/pyproject.toml` & `sockets-communication-0.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'sockets-communication'
-version = '0.0.0'
+version = '0.0.1'
 description = 'This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.'
 classifiers = [
 	'Intended Audience :: Developers',
 	'License :: OSI Approved :: MIT License',
 	'Programming Language :: Python',
 	'Programming Language :: Python :: 3',
 	'Programming Language :: Python :: 3.8',
```

### Comparing `sockets-communication-0.0.0/setup.py` & `sockets-communication-0.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         exclude=[
             "__pycache__",
             "*.pyc"
         ],
         requirements="requirements.txt",
         dev_requirements="requirements-dev.txt",
         name='sockets-communication',
-        version='0.0.0',
+        version='0.0.1',
         description=(
             "This module provides a wrapper for the built-in "
             "socket module in python. The program provides server and. "
             "client classes, with the communication methods."
         ),
         license='MIT',
         author="Shahaf Frank-Shapir",
```

### Comparing `sockets-communication-0.0.0/sockets_communication/base.py` & `sockets-communication-0.0.1/sockets_communication/base.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-0.0.0/sockets_communication/exceptions.py` & `sockets-communication-0.0.1/sockets_communication/exceptions.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-0.0.0/sockets_communication/process.py` & `sockets-communication-0.0.1/sockets_communication/process.py`

 * *Files identical despite different names*

### Comparing `sockets-communication-0.0.0/sockets_communication/sockets.py` & `sockets-communication-0.0.1/sockets_communication/sockets.py`

 * *Files 1% similar despite different names*

```diff
@@ -346,15 +346,15 @@
     def created(self) -> bool:
         """
         Checks if the service was created.
 
         :return: The value for the service being created.
         """
 
-        return self.listening_process is not None
+        return isinstance(self.listening_process, threading.Thread)
     # end created
 
     def blocked(self) -> bool:
         """
         Returns the value of te execution being blocked by the service loop.
 
         :return: The blocking value.
@@ -568,15 +568,19 @@
     def terminate(self) -> None:
         """Pauses the process of service."""
 
         if not self.running():
             return
         # end if
 
-        terminate_thread(self.listening_process)
+        if isinstance(self.listening_process, threading.Thread):
+            terminate_thread(self.listening_process)
+
+            self.listening_process = None
+        # end if
     # end terminate
 
     def send_message_to_client(self, message: bytes, connection: Socket) -> None:
         """
         Sends a message to the client by its connection.
 
         :param message: The message to send to the client.
```

### Comparing `sockets-communication-0.0.0/sockets_communication.egg-info/PKG-INFO` & `sockets-communication-0.0.1/sockets_communication.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sockets-communication
-Version: 0.0.0
+Version: 0.0.1
 Summary: This module provides a wrapper for the built-in socket module in python. The program provides server and. client classes, with the communication methods.
 Home-page: https://github.com/Shahaf-F-S/sockets-communication
 Author: Shahaf Frank-Shapir
 Author-email: shahaffrs@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

