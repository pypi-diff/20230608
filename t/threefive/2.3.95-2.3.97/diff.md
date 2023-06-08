# Comparing `tmp/threefive-2.3.95.tar.gz` & `tmp/threefive-2.3.97.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "threefive-2.3.95.tar", last modified: Thu Jun  1 23:43:37 2023, max compression
+gzip compressed data, was "threefive-2.3.97.tar", last modified: Thu Jun  8 10:08:53 2023, max compression
```

## Comparing `threefive-2.3.95.tar` & `threefive-2.3.97.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.213339 threefive-2.3.95/
--rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.95/LICENSE
--rw-r--r--   0 a         (1000) a         (1000)    13225 2023-06-01 23:43:37.213339 threefive-2.3.95/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)    12654 2023-06-01 23:43:28.000000 threefive-2.3.95/README.md
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.209338 threefive-2.3.95/bin/
--rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.95/bin/threefive
--rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-01 23:43:37.213339 threefive-2.3.95/setup.cfg
--rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.95/setup.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.213339 threefive-2.3.95/threefive/
--rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/__init__.py
--rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/base.py
--rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/bitn.py
--rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/commands.py
--rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/crc.py
--rw-r--r--   0 a         (1000) a         (1000)    10691 2023-06-01 23:43:28.000000 threefive-2.3.95/threefive/cue.py
--rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/decode.py
--rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/descriptors.py
--rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/encode.py
--rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/packetdata.py
--rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/section.py
--rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/segment.py
--rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/segmentation.py
--rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/smoketest.py
--rw-r--r--   0 a         (1000) a         (1000)    18046 2023-05-16 17:14:07.000000 threefive-2.3.95/threefive/stream.py
--rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/stuff.py
--rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.95/threefive/upids.py
--rw-r--r--   0 a         (1000) a         (1000)       43 2023-06-01 23:43:28.000000 threefive-2.3.95/threefive/version.py
-drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-01 23:43:37.213339 threefive-2.3.95/threefive.egg-info/
--rw-r--r--   0 a         (1000) a         (1000)    13225 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/PKG-INFO
--rw-r--r--   0 a         (1000) a         (1000)      577 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/SOURCES.txt
--rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/dependency_links.txt
--rw-r--r--   0 a         (1000) a         (1000)       24 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/requires.txt
--rw-r--r--   0 a         (1000) a         (1000)       10 2023-06-01 23:43:37.000000 threefive-2.3.95/threefive.egg-info/top_level.txt
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.534958 threefive-2.3.97/
+-rw-r--r--   0 a         (1000) a         (1000)     1074 2023-05-16 15:18:26.000000 threefive-2.3.97/LICENSE
+-rw-r--r--   0 a         (1000) a         (1000)    13338 2023-06-08 10:08:53.534958 threefive-2.3.97/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)    12767 2023-06-08 10:08:46.000000 threefive-2.3.97/README.md
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.530961 threefive-2.3.97/bin/
+-rwxr-xr-x   0 a         (1000) a         (1000)      667 2023-05-16 15:18:26.000000 threefive-2.3.97/bin/threefive
+-rw-r--r--   0 a         (1000) a         (1000)       38 2023-06-08 10:08:53.534958 threefive-2.3.97/setup.cfg
+-rw-r--r--   0 a         (1000) a         (1000)     1026 2023-05-16 15:18:26.000000 threefive-2.3.97/setup.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.534958 threefive-2.3.97/threefive/
+-rw-r--r--   0 a         (1000) a         (1000)      628 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/__init__.py
+-rw-r--r--   0 a         (1000) a         (1000)     2873 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/base.py
+-rw-r--r--   0 a         (1000) a         (1000)     4811 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/bitn.py
+-rw-r--r--   0 a         (1000) a         (1000)    11730 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/commands.py
+-rw-r--r--   0 a         (1000) a         (1000)      846 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/crc.py
+-rw-r--r--   0 a         (1000) a         (1000)    10691 2023-06-01 23:43:28.000000 threefive-2.3.97/threefive/cue.py
+-rw-r--r--   0 a         (1000) a         (1000)     1837 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/decode.py
+-rw-r--r--   0 a         (1000) a         (1000)    13788 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/descriptors.py
+-rw-r--r--   0 a         (1000) a         (1000)     2719 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/encode.py
+-rw-r--r--   0 a         (1000) a         (1000)     1038 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/packetdata.py
+-rw-r--r--   0 a         (1000) a         (1000)     5709 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/section.py
+-rw-r--r--   0 a         (1000) a         (1000)     2972 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/segment.py
+-rw-r--r--   0 a         (1000) a         (1000)     1970 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/segmentation.py
+-rw-r--r--   0 a         (1000) a         (1000)     1660 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/smoketest.py
+-rw-r--r--   0 a         (1000) a         (1000)    18089 2023-06-08 10:05:54.000000 threefive-2.3.97/threefive/stream.py
+-rw-r--r--   0 a         (1000) a         (1000)      199 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/stuff.py
+-rw-r--r--   0 a         (1000) a         (1000)     6607 2023-05-16 15:18:26.000000 threefive-2.3.97/threefive/upids.py
+-rw-r--r--   0 a         (1000) a         (1000)       43 2023-06-08 10:05:54.000000 threefive-2.3.97/threefive/version.py
+drwxr-xr-x   0 a         (1000) a         (1000)        0 2023-06-08 10:08:53.534958 threefive-2.3.97/threefive.egg-info/
+-rw-r--r--   0 a         (1000) a         (1000)    13338 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/PKG-INFO
+-rw-r--r--   0 a         (1000) a         (1000)      577 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/SOURCES.txt
+-rw-r--r--   0 a         (1000) a         (1000)        1 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/dependency_links.txt
+-rw-r--r--   0 a         (1000) a         (1000)       24 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/requires.txt
+-rw-r--r--   0 a         (1000) a         (1000)       10 2023-06-08 10:08:53.000000 threefive-2.3.97/threefive.egg-info/top_level.txt
```

### Comparing `threefive-2.3.95/LICENSE` & `threefive-2.3.97/LICENSE`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/PKG-INFO` & `threefive-2.3.97/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.3.95
+Version: 2.3.97
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.95</b><i> (fix for me breaking base64 decoding)</i> </summary>
+<details><summary><b>Latest Version is 2.3.97</b><i> (fix for me breaking parsing for payloads without PTS in the Stream class)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
 
@@ -490,24 +490,25 @@
 '扢湬灤桰䑮Ȃ菁ʥ\x00'
 ```
 
 </details>
 
 ### Powered by threefive
 
-
+  * [POIS Server](https://github.com/scunning1987/pois_reference_server) is Super Cool.
+ 
   * [x9k3](https://github.com/futzu/x9k3): SCTE-35 HLS Segmenter and Cue Inserter.
 
   * [m3ufu](https://github.com/futzu/m3ufu): SCTE-35 m3u8 Parser.
 
   * [six2scte35](https://github.com/futzu/six2scte35): ffmpeg changes SCTE-35 stream type to 0x06 bin data, six2scte35 changes it back.
 
   * [SuperKabuki](https://github.com/futzu/SuperKabuki): SCTE-35 Packet Injection.
 
 ### other threefive stuff
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
-  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue. I am NOT the SCTE-35 Support Hotline. Do your own damn homework*
+  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue or "what is the meaning of life?" type of question.*
```

### Comparing `threefive-2.3.95/README.md` & `threefive-2.3.97/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.95</b><i> (fix for me breaking base64 decoding)</i> </summary>
+<details><summary><b>Latest Version is 2.3.97</b><i> (fix for me breaking parsing for payloads without PTS in the Stream class)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
 
@@ -474,24 +474,25 @@
 '扢湬灤桰䑮Ȃ菁ʥ\x00'
 ```
 
 </details>
 
 ### Powered by threefive
 
-
+  * [POIS Server](https://github.com/scunning1987/pois_reference_server) is Super Cool.
+ 
   * [x9k3](https://github.com/futzu/x9k3): SCTE-35 HLS Segmenter and Cue Inserter.
 
   * [m3ufu](https://github.com/futzu/m3ufu): SCTE-35 m3u8 Parser.
 
   * [six2scte35](https://github.com/futzu/six2scte35): ffmpeg changes SCTE-35 stream type to 0x06 bin data, six2scte35 changes it back.
 
   * [SuperKabuki](https://github.com/futzu/SuperKabuki): SCTE-35 Packet Injection.
 
 ### other threefive stuff
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
-  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue. I am NOT the SCTE-35 Support Hotline. Do your own damn homework*
+  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue or "what is the meaning of life?" type of question.*
```

### Comparing `threefive-2.3.95/bin/threefive` & `threefive-2.3.97/bin/threefive`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/setup.py` & `threefive-2.3.97/setup.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/__init__.py` & `threefive-2.3.97/threefive/__init__.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/base.py` & `threefive-2.3.97/threefive/base.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/bitn.py` & `threefive-2.3.97/threefive/bitn.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/commands.py` & `threefive-2.3.97/threefive/commands.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/crc.py` & `threefive-2.3.97/threefive/crc.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/cue.py` & `threefive-2.3.97/threefive/cue.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/decode.py` & `threefive-2.3.97/threefive/decode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/descriptors.py` & `threefive-2.3.97/threefive/descriptors.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/encode.py` & `threefive-2.3.97/threefive/encode.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/packetdata.py` & `threefive-2.3.97/threefive/packetdata.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/section.py` & `threefive-2.3.97/threefive/section.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/segment.py` & `threefive-2.3.97/threefive/segment.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/segmentation.py` & `threefive-2.3.97/threefive/segmentation.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/smoketest.py` & `threefive-2.3.97/threefive/smoketest.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive/stream.py` & `threefive-2.3.97/threefive/stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -392,27 +392,28 @@
         self.maps.pid_cc[pid] = c_c
 
     def _parse_pts(self, pkt, pid):
         """
         parse pts and store by program key
         in the dict Stream._pid_pts
         """
-        # if len(payload) > 13:
+
         if self._pusi_flag(pkt):
             payload = self._parse_payload(pkt)
-            if self._pts_flag(payload):
-                pts = (payload[9] & 14) << 29
-                pts |= payload[10] << 22
-                pts |= (payload[11] >> 1) << 15
-                pts |= payload[12] << 7
-                pts |= payload[13] >> 1
-                prgm = self.pid2prgm(pid)
-                self.maps.prgm_pts[prgm] = pts
-                if prgm not in self.start:
-                    self.start[prgm] = pts
+            if len(payload) > 13:
+                if self._pts_flag(payload):
+                    pts = (payload[9] & 14) << 29
+                    pts |= payload[10] << 22
+                    pts |= (payload[11] >> 1) << 15
+                    pts |= payload[12] << 7
+                    pts |= payload[13] >> 1
+                    prgm = self.pid2prgm(pid)
+                    self.maps.prgm_pts[prgm] = pts
+                    if prgm not in self.start:
+                        self.start[prgm] = pts
 
     def _parse_payload(self, pkt):
         """
         _parse_payload returns the packet payload
         """
         head_size = 4
         if self._afc_flag(pkt[3]):
```

### Comparing `threefive-2.3.95/threefive/upids.py` & `threefive-2.3.97/threefive/upids.py`

 * *Files identical despite different names*

### Comparing `threefive-2.3.95/threefive.egg-info/PKG-INFO` & `threefive-2.3.97/threefive.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: threefive
-Version: 2.3.95
+Version: 2.3.97
 Summary: Pythonic SCTE35
 Home-page: https://github.com/futzu/threefive
 Author: Adrian and a Cast of Thousands.
 Author-email: spam@iodisco.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![image](https://github.com/futzu/scte35-threefive/assets/52701496/8bfacebe-1cf9-4cc5-82f5-84efa5dbe1c2)
 
-<details><summary><b>Latest Version is 2.3.95</b><i> (fix for me breaking base64 decoding)</i> </summary>
+<details><summary><b>Latest Version is 2.3.97</b><i> (fix for me breaking parsing for payloads without PTS in the Stream class)</i> </summary>
 
  * __Removed__ The rogue file cmd.py.
 
 </details>
  
  <details><summary><b>Installation and Getting Started</b></summary>
 
@@ -490,24 +490,25 @@
 '扢湬灤桰䑮Ȃ菁ʥ\x00'
 ```
 
 </details>
 
 ### Powered by threefive
 
-
+  * [POIS Server](https://github.com/scunning1987/pois_reference_server) is Super Cool.
+ 
   * [x9k3](https://github.com/futzu/x9k3): SCTE-35 HLS Segmenter and Cue Inserter.
 
   * [m3ufu](https://github.com/futzu/m3ufu): SCTE-35 m3u8 Parser.
 
   * [six2scte35](https://github.com/futzu/six2scte35): ffmpeg changes SCTE-35 stream type to 0x06 bin data, six2scte35 changes it back.
 
   * [SuperKabuki](https://github.com/futzu/SuperKabuki): SCTE-35 Packet Injection.
 
 ### other threefive stuff
 
   * [Diagram](https://github.com/futzu/threefive/blob/master/cue.md) of a threefive SCTE-35 Cue.
 
   * [ffmpeg and threefive](https://github.com/futzu/SCTE35-threefive/blob/master/threefive-ffmpeg.md) and SCTE35 and Stream Type 0x6 bin data.
 
-  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue. I am NOT the SCTE-35 Support Hotline. Do your own damn homework*
+  * [Issues and Bugs and Feature Requests](https://github.com/futzu/scte35-threefive/issues) *No forms man, just open an issue and tell me what you need. It needs to be a threefive related issue or "what is the meaning of life?" type of question.*
```

### Comparing `threefive-2.3.95/threefive.egg-info/SOURCES.txt` & `threefive-2.3.97/threefive.egg-info/SOURCES.txt`

 * *Files identical despite different names*

