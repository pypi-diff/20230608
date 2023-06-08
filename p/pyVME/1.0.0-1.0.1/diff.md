# Comparing `tmp/pyVME-1.0.0.tar.gz` & `tmp/pyVME-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyVME-1.0.0.tar", last modified: Thu May 11 16:44:04 2023, max compression
+gzip compressed data, was "pyVME-1.0.1.tar", last modified: Thu Jun  8 18:04:52 2023, max compression
```

## Comparing `pyVME-1.0.0.tar` & `pyVME-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-05-11 16:44:04.570455 pyVME-1.0.0/
--rw-r--r--   0 schuechter  (2198) users      (100)    31962 2023-05-11 16:24:21.000000 pyVME-1.0.0/LICENSE
--rw-r--r--   0 schuechter  (2198) users      (100)       60 2023-05-03 16:08:39.000000 pyVME-1.0.0/MANIFEST.in
--rw-r--r--   0 schuechter  (2198) users      (100)     4692 2023-05-11 16:44:04.566455 pyVME-1.0.0/PKG-INFO
--rw-r--r--   0 schuechter  (2198) users      (100)     4111 2023-05-11 16:24:37.000000 pyVME-1.0.0/README.md
--rw-r--r--   0 schuechter  (2198) users      (100)      709 2023-05-11 16:40:59.000000 pyVME-1.0.0/pyproject.toml
--rw-r--r--   0 schuechter  (2198) users      (100)       38 2023-05-11 16:44:04.570455 pyVME-1.0.0/setup.cfg
-drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-05-11 16:44:04.402449 pyVME-1.0.0/src/
-drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-05-11 16:44:04.443451 pyVME-1.0.0/src/pyVME/
--rw-r--r--   0 schuechter  (2198) users      (100)       80 2023-04-04 12:16:21.000000 pyVME-1.0.0/src/pyVME/__init__.py
--rw-r--r--   0 schuechter  (2198) users      (100)     4325 2023-05-11 16:23:56.000000 pyVME-1.0.0/src/pyVME/client.py
--rw-r--r--   0 schuechter  (2198) users      (100)     2568 2023-05-11 16:24:01.000000 pyVME-1.0.0/src/pyVME/fpga.py
--rw-r--r--   0 schuechter  (2198) users      (100)     7045 2023-05-11 16:24:08.000000 pyVME-1.0.0/src/pyVME/server.py
--rwxr-xr-x   0 schuechter  (2198) users      (100) 10929728 2023-05-11 16:36:41.000000 pyVME-1.0.0/src/pyVME/vme_fpga_py.cpython-39-x86_64-linux-gnu.so
-drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-05-11 16:44:04.561454 pyVME-1.0.0/src/pyVME.egg-info/
--rw-r--r--   0 schuechter  (2198) users      (100)     4692 2023-05-11 16:44:04.000000 pyVME-1.0.0/src/pyVME.egg-info/PKG-INFO
--rw-r--r--   0 schuechter  (2198) users      (100)      309 2023-05-11 16:44:04.000000 pyVME-1.0.0/src/pyVME.egg-info/SOURCES.txt
--rw-r--r--   0 schuechter  (2198) users      (100)        1 2023-05-11 16:44:04.000000 pyVME-1.0.0/src/pyVME.egg-info/dependency_links.txt
--rw-r--r--   0 schuechter  (2198) users      (100)        6 2023-05-11 16:44:04.000000 pyVME-1.0.0/src/pyVME.egg-info/top_level.txt
+drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-06-08 18:04:52.544862 pyVME-1.0.1/
+-rw-r--r--   0 schuechter  (2198) users      (100)    31962 2023-06-08 17:51:34.000000 pyVME-1.0.1/LICENSE
+-rw-r--r--   0 schuechter  (2198) users      (100)       60 2023-06-08 17:51:34.000000 pyVME-1.0.1/MANIFEST.in
+-rw-r--r--   0 schuechter  (2198) users      (100)     4680 2023-06-08 18:04:52.543862 pyVME-1.0.1/PKG-INFO
+-rw-r--r--   0 schuechter  (2198) users      (100)     4098 2023-06-08 17:51:34.000000 pyVME-1.0.1/README.md
+-rw-r--r--   0 schuechter  (2198) users      (100)      709 2023-06-08 18:04:42.000000 pyVME-1.0.1/pyproject.toml
+-rw-r--r--   0 schuechter  (2198) users      (100)       38 2023-06-08 18:04:52.544862 pyVME-1.0.1/setup.cfg
+drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-06-08 18:04:52.393857 pyVME-1.0.1/src/
+drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-06-08 18:04:52.417858 pyVME-1.0.1/src/pyVME/
+-rw-r--r--   0 schuechter  (2198) users      (100)       80 2023-06-08 17:51:34.000000 pyVME-1.0.1/src/pyVME/__init__.py
+-rw-r--r--   0 schuechter  (2198) users      (100)     4325 2023-06-08 17:51:34.000000 pyVME-1.0.1/src/pyVME/client.py
+-rw-r--r--   0 schuechter  (2198) users      (100)     2568 2023-06-08 17:51:34.000000 pyVME-1.0.1/src/pyVME/fpga.py
+-rw-r--r--   0 schuechter  (2198) users      (100)     7043 2023-06-08 17:51:34.000000 pyVME-1.0.1/src/pyVME/server.py
+-rwxr-xr-x   0 schuechter  (2198) users      (100) 10929728 2023-06-08 17:53:29.000000 pyVME-1.0.1/src/pyVME/vme_fpga_py.cpython-39-x86_64-linux-gnu.so
+drwxr-xr-x   0 schuechter  (2198) users      (100)        0 2023-06-08 18:04:52.534862 pyVME-1.0.1/src/pyVME.egg-info/
+-rw-r--r--   0 schuechter  (2198) users      (100)     4680 2023-06-08 18:04:52.000000 pyVME-1.0.1/src/pyVME.egg-info/PKG-INFO
+-rw-r--r--   0 schuechter  (2198) users      (100)      309 2023-06-08 18:04:52.000000 pyVME-1.0.1/src/pyVME.egg-info/SOURCES.txt
+-rw-r--r--   0 schuechter  (2198) users      (100)        1 2023-06-08 18:04:52.000000 pyVME-1.0.1/src/pyVME.egg-info/dependency_links.txt
+-rw-r--r--   0 schuechter  (2198) users      (100)        6 2023-06-08 18:04:52.000000 pyVME-1.0.1/src/pyVME.egg-info/top_level.txt
```

### Comparing `pyVME-1.0.0/LICENSE` & `pyVME-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyVME-1.0.0/PKG-INFO` & `pyVME-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVME
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small python VME integration, that uses an exposed cpp vme library to interact with a FPGA and can act as a user<->server system
 Author-email: Dominic Schüchter <schuechter@hiskp.uni-bonn.de>
 Project-URL: Homepage, https://github.com/dschuechter/pyVME
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
@@ -24,21 +24,21 @@
 2. [Installation](#Installation)
 3. [Building from source](#Building-from-source)
    
 ## Requierements:
 This package needs to be run on a Linux 64bit machine with python >= 3.9 installed
 
 ## Installation
-This package is available via [```pipy```](https://pypi.org) and can be simply installed by running:
+This package is available via [```pypi```](https://pypi.org) and can be simply installed by running:
 
     pip install pyVME
 
 ## Features
-After installation (e.g. pip install pyVME) you can import this package into your projects via, returns ```
-```import pyVME````
+After installation (e.g. pip install pyVME) you can import this package into your projects via ```import pyVME```.
+
 This gives you access to the three classes that come within this package, returns ```
 1. ```pyVME.fpga(baseaddr)```: Allows you to instantiate one FPGA that is directly connected to the CPU your python program is running on
 2. ```pyVME.server(int server_port)```: Allows you to run a server on a remote machine that is connected with one or more FPGAs. It will instantiate for each FPGA defined by the client a new instance.  
 3. ```pyVME.remoteFPGA(int baseaddr, string server_ip, int server_port)```: Allows you to connect to a running server and call functions of the remote FPGA instances.
 
 Every class has the same set of functions that act differently in the background without the user having to change anything.
 
@@ -94,15 +94,15 @@
 ```
 No other packages are requiered. You can simply build this package by running:
 ```
 python3 -m build
 ```
 in the root directory of this repository.
 
-It will automatically generate a ```dist```folder with the contents ```pyVME-X.X.X-py3-none-any.whl``` and ```pyVME-1.0.0.tar.gz```.
+It will automatically generate a ```dist```folder with the contents ```pyVME-X.X.X-py3-none-any.whl``` and ```pyVME-X.X.X.tar.gz```.
 
 You can install the build package by running 
 ```
 pip install ./dist/pyVME-X.X.X-py3-none-any.whl
 ```
 or
```

### Comparing `pyVME-1.0.0/README.md` & `pyVME-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -11,21 +11,21 @@
 2. [Installation](#Installation)
 3. [Building from source](#Building-from-source)
    
 ## Requierements:
 This package needs to be run on a Linux 64bit machine with python >= 3.9 installed
 
 ## Installation
-This package is available via [```pipy```](https://pypi.org) and can be simply installed by running:
+This package is available via [```pypi```](https://pypi.org) and can be simply installed by running:
 
     pip install pyVME
 
 ## Features
-After installation (e.g. pip install pyVME) you can import this package into your projects via, returns ```
-```import pyVME````
+After installation (e.g. pip install pyVME) you can import this package into your projects via ```import pyVME```.
+
 This gives you access to the three classes that come within this package, returns ```
 1. ```pyVME.fpga(baseaddr)```: Allows you to instantiate one FPGA that is directly connected to the CPU your python program is running on
 2. ```pyVME.server(int server_port)```: Allows you to run a server on a remote machine that is connected with one or more FPGAs. It will instantiate for each FPGA defined by the client a new instance.  
 3. ```pyVME.remoteFPGA(int baseaddr, string server_ip, int server_port)```: Allows you to connect to a running server and call functions of the remote FPGA instances.
 
 Every class has the same set of functions that act differently in the background without the user having to change anything.
 
@@ -81,18 +81,18 @@
 ```
 No other packages are requiered. You can simply build this package by running:
 ```
 python3 -m build
 ```
 in the root directory of this repository.
 
-It will automatically generate a ```dist```folder with the contents ```pyVME-X.X.X-py3-none-any.whl``` and ```pyVME-1.0.0.tar.gz```.
+It will automatically generate a ```dist```folder with the contents ```pyVME-X.X.X-py3-none-any.whl``` and ```pyVME-X.X.X.tar.gz```.
 
 You can install the build package by running 
 ```
 pip install ./dist/pyVME-X.X.X-py3-none-any.whl
 ```
 or
 
 ```
 pip install ./dist/pyVME-X.X.X.tar.gz   
-```
+```
```

### Comparing `pyVME-1.0.0/pyproject.toml` & `pyVME-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyVME"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="Dominic Schüchter", email="schuechter@hiskp.uni-bonn.de" },
 ]
 description = "A small python VME integration, that uses an exposed cpp vme library to interact with a FPGA and can act as a user<->server system"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `pyVME-1.0.0/src/pyVME/client.py` & `pyVME-1.0.1/src/pyVME/client.py`

 * *Files identical despite different names*

### Comparing `pyVME-1.0.0/src/pyVME/fpga.py` & `pyVME-1.0.1/src/pyVME/fpga.py`

 * *Files identical despite different names*

### Comparing `pyVME-1.0.0/src/pyVME/server.py` & `pyVME-1.0.1/src/pyVME/server.py`

 * *Files 1% similar despite different names*

```diff
@@ -146,15 +146,15 @@
             return read_fpgaDone
 
         if command == 'wait_on_fpga_done':
             read_wait_on_fpga_done = FPGA.wait_on_fpga_done()
             if self.debug_messages: print("Get wait on fpga done: ", read_wait_on_fpga_done)
             return read_wait_on_fpga_done       
 
-    def input(self):
+    def run(self):
             self.info()
             with socket.socket(socket.AF_INET, socket.SOCK_STREAM) as s:
                 s.bind((self.server_ip, self.server_port))
                 s.listen()
                 while True:
                     conn, addr = s.accept()
```

### Comparing `pyVME-1.0.0/src/pyVME/vme_fpga_py.cpython-39-x86_64-linux-gnu.so` & `pyVME-1.0.1/src/pyVME/vme_fpga_py.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyVME-1.0.0/src/pyVME.egg-info/PKG-INFO` & `pyVME-1.0.1/src/pyVME.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyVME
-Version: 1.0.0
+Version: 1.0.1
 Summary: A small python VME integration, that uses an exposed cpp vme library to interact with a FPGA and can act as a user<->server system
 Author-email: Dominic Schüchter <schuechter@hiskp.uni-bonn.de>
 Project-URL: Homepage, https://github.com/dschuechter/pyVME
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Requires-Python: >=3.9
@@ -24,21 +24,21 @@
 2. [Installation](#Installation)
 3. [Building from source](#Building-from-source)
    
 ## Requierements:
 This package needs to be run on a Linux 64bit machine with python >= 3.9 installed
 
 ## Installation
-This package is available via [```pipy```](https://pypi.org) and can be simply installed by running:
+This package is available via [```pypi```](https://pypi.org) and can be simply installed by running:
 
     pip install pyVME
 
 ## Features
-After installation (e.g. pip install pyVME) you can import this package into your projects via, returns ```
-```import pyVME````
+After installation (e.g. pip install pyVME) you can import this package into your projects via ```import pyVME```.
+
 This gives you access to the three classes that come within this package, returns ```
 1. ```pyVME.fpga(baseaddr)```: Allows you to instantiate one FPGA that is directly connected to the CPU your python program is running on
 2. ```pyVME.server(int server_port)```: Allows you to run a server on a remote machine that is connected with one or more FPGAs. It will instantiate for each FPGA defined by the client a new instance.  
 3. ```pyVME.remoteFPGA(int baseaddr, string server_ip, int server_port)```: Allows you to connect to a running server and call functions of the remote FPGA instances.
 
 Every class has the same set of functions that act differently in the background without the user having to change anything.
 
@@ -94,15 +94,15 @@
 ```
 No other packages are requiered. You can simply build this package by running:
 ```
 python3 -m build
 ```
 in the root directory of this repository.
 
-It will automatically generate a ```dist```folder with the contents ```pyVME-X.X.X-py3-none-any.whl``` and ```pyVME-1.0.0.tar.gz```.
+It will automatically generate a ```dist```folder with the contents ```pyVME-X.X.X-py3-none-any.whl``` and ```pyVME-X.X.X.tar.gz```.
 
 You can install the build package by running 
 ```
 pip install ./dist/pyVME-X.X.X-py3-none-any.whl
 ```
 or
```

