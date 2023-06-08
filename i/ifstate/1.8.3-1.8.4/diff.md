# Comparing `tmp/ifstate-1.8.3.tar.gz` & `tmp/ifstate-1.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ifstate-1.8.3.tar", last modified: Wed Apr 12 20:37:32 2023, max compression
+gzip compressed data, was "ifstate-1.8.4.tar", last modified: Thu Jun  8 12:57:02 2023, max compression
```

## Comparing `ifstate-1.8.3.tar` & `ifstate-1.8.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-12 20:37:24.000000 ifstate-1.8.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-12 20:37:32.707270 ifstate-1.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-04-12 20:37:24.000000 ifstate-1.8.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/ifstate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:24.000000 ifstate-1.8.3/ifstate/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6391 2023-04-12 20:37:24.000000 ifstate-1.8.3/ifstate/ifstate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-04-12 20:37:24.000000 ifstate-1.8.3/ifstate/shell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/ifstate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-12 20:37:32.000000 ifstate-1.8.3/ifstate.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/address/
--rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/address/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/bpf/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/bpf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/bpf/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/bpf/map.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/brport/
--rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/brport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/link/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/physical.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/tun.py
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/link/veth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/neighbour/
--rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/neighbour/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/libifstate/parser/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/parser/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/parser/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/routing/
--rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/routing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/sysctl/
--rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/sysctl/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/tc/
--rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/tc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/wireguard/
--rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/wireguard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.707270 ifstate-1.8.3/libifstate/xdp/
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-04-12 20:37:24.000000 ifstate-1.8.3/libifstate/xdp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 20:37:32.703270 ifstate-1.8.3/schema/
--rw-r--r--   0 runner    (1001) docker     (123)   178382 2023-04-12 20:37:24.000000 ifstate-1.8.3/schema/ifstate.conf.schema.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 20:37:32.707270 ifstate-1.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-04-12 20:37:24.000000 ifstate-1.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.773380 ifstate-1.8.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-08 12:56:45.000000 ifstate-1.8.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-08 12:57:02.769379 ifstate-1.8.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-08 12:56:45.000000 ifstate-1.8.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.765380 ifstate-1.8.4/ifstate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 12:56:45.000000 ifstate-1.8.4/ifstate/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6391 2023-06-08 12:56:45.000000 ifstate-1.8.4/ifstate/ifstate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-06-08 12:56:45.000000 ifstate-1.8.4/ifstate/shell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.765380 ifstate-1.8.4/ifstate.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 12:57:02.000000 ifstate-1.8.4/ifstate.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/
+-rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/address/
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/address/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/bpf/
+-rw-r--r--   0 runner    (1001) docker     (123)     6818 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/bpf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/bpf/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10818 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/bpf/map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/brport/
+-rw-r--r--   0 runner    (1001) docker     (123)     2868 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/brport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22110 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/physical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/tun.py
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/link/veth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3264 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/neighbour/
+-rw-r--r--   0 runner    (1001) docker     (123)     2577 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/neighbour/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/parser/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3686 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/parser/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/parser/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/routing/
+-rw-r--r--   0 runner    (1001) docker     (123)    17006 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/routing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/sysctl/
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/sysctl/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/tc/
+-rw-r--r--   0 runner    (1001) docker     (123)    11188 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/tc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/wireguard/
+-rw-r--r--   0 runner    (1001) docker     (123)     5207 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/wireguard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/libifstate/xdp/
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-06-08 12:56:45.000000 ifstate-1.8.4/libifstate/xdp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 12:57:02.769379 ifstate-1.8.4/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)   178382 2023-06-08 12:56:45.000000 ifstate-1.8.4/schema/ifstate.conf.schema.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 12:57:02.773380 ifstate-1.8.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-06-08 12:56:45.000000 ifstate-1.8.4/setup.py
```

### Comparing `ifstate-1.8.3/LICENSE` & `ifstate-1.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/PKG-INFO` & `ifstate-1.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.3
+Version: 1.8.4
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.3/README.md` & `ifstate-1.8.4/README.md`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/ifstate/ifstate.py` & `ifstate-1.8.4/ifstate/ifstate.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/ifstate/shell.py` & `ifstate-1.8.4/ifstate/shell.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/ifstate.egg-info/PKG-INFO` & `ifstate-1.8.4/ifstate.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ifstate
-Version: 1.8.3
+Version: 1.8.4
 Summary: Manage host interface settings in a declarative manner
 Home-page: https://ifstate.net/
 Author: Thomas Liske
 Author-email: thomas@fiasko-nw.net
 License: GPL3+
 Description-Content-Type: text/markdown
 Provides-Extra: shell
```

### Comparing `ifstate-1.8.3/ifstate.egg-info/SOURCES.txt` & `ifstate-1.8.4/ifstate.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/__init__.py` & `ifstate-1.8.4/libifstate/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 import os
 import pkgutil
 import re
 import json
 import errno
 import logging
 
-__version__ = "1.8.3"
+__version__ = "1.8.4"
 
 
 class IfState():
     def __init__(self):
         logger.debug('IfState {}'.format(__version__))
         self.links = {}
         self.addresses = {}
```

### Comparing `ifstate-1.8.3/libifstate/address/__init__.py` & `ifstate-1.8.4/libifstate/address/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/bpf/__init__.py` & `ifstate-1.8.4/libifstate/bpf/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/bpf/ctypes.py` & `ifstate-1.8.4/libifstate/bpf/ctypes.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/bpf/map.py` & `ifstate-1.8.4/libifstate/bpf/map.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/brport/__init__.py` & `ifstate-1.8.4/libifstate/brport/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/exception.py` & `ifstate-1.8.4/libifstate/exception.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/link/base.py` & `ifstate-1.8.4/libifstate/link/base.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/link/physical.py` & `ifstate-1.8.4/libifstate/link/physical.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/link/tun.py` & `ifstate-1.8.4/libifstate/link/tun.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/link/veth.py` & `ifstate-1.8.4/libifstate/link/veth.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/log.py` & `ifstate-1.8.4/libifstate/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,20 +3,15 @@
 import os
 import queue
 import sys
 
 logger = logging.getLogger('ifstate')
 logger.propagate = False
 
-formatter = logging.Formatter('%(bol)s%(prefix)s%(style)s%(message)s%(eol)s', defaults={
-    'bol': '',
-    'eol': '',
-    'prefix': '',
-})
-
+formatter = logging.Formatter('%(bol)s%(prefix)s%(style)s%(message)s%(eol)s')
 
 class IfStateLogFilter(logging.Filter):
     def __init__(self, is_terminal):
         super().__init__()
         self.is_terminal = is_terminal
 
     def filter(self, record):
```

### Comparing `ifstate-1.8.3/libifstate/neighbour/__init__.py` & `ifstate-1.8.4/libifstate/neighbour/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/parser/base.py` & `ifstate-1.8.4/libifstate/parser/base.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/parser/yaml.py` & `ifstate-1.8.4/libifstate/parser/yaml.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/routing/__init__.py` & `ifstate-1.8.4/libifstate/routing/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/sysctl/__init__.py` & `ifstate-1.8.4/libifstate/sysctl/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/tc/__init__.py` & `ifstate-1.8.4/libifstate/tc/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/util.py` & `ifstate-1.8.4/libifstate/util.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/wireguard/__init__.py` & `ifstate-1.8.4/libifstate/wireguard/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/libifstate/xdp/__init__.py` & `ifstate-1.8.4/libifstate/xdp/__init__.py`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/schema/ifstate.conf.schema.json` & `ifstate-1.8.4/schema/ifstate.conf.schema.json`

 * *Files identical despite different names*

### Comparing `ifstate-1.8.3/setup.py` & `ifstate-1.8.4/setup.py`

 * *Files identical despite different names*

