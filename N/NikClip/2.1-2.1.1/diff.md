# Comparing `tmp/NikClip-2.1.tar.gz` & `tmp/NikClip-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NikClip-2.1.tar", last modified: Wed Jun  7 04:11:00 2023, max compression
+gzip compressed data, was "NikClip-2.1.1.tar", last modified: Thu Jun  8 01:33:06 2023, max compression
```

## Comparing `NikClip-2.1.tar` & `NikClip-2.1.1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 04:11:00.768787 NikClip-2.1/
--rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikClip-2.1/LICENSE
-drwxrwxrwx   0        0        0        0 2023-06-07 04:11:00.753711 NikClip-2.1/NikClip.egg-info/
--rw-rw-rw-   0        0        0     2545 2023-06-07 04:11:00.000000 NikClip-2.1/NikClip.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-07 04:11:00.000000 NikClip-2.1/NikClip.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:11:00.000000 NikClip-2.1/NikClip.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 04:11:00.000000 NikClip-2.1/NikClip.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2545 2023-06-07 04:11:00.769797 NikClip-2.1/PKG-INFO
--rw-rw-rw-   0        0        0     2063 2023-05-24 05:11:07.000000 NikClip-2.1/README.md
--rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikClip-2.1/pyproject.toml
--rw-rw-rw-   0        0        0      584 2023-06-07 04:11:00.785377 NikClip-2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 01:33:06.583158 NikClip-2.1.1/
+-rw-rw-rw-   0        0        0     1094 2023-05-19 05:37:20.000000 NikClip-2.1.1/LICENSE
+drwxrwxrwx   0        0        0        0 2023-06-08 01:33:06.517800 NikClip-2.1.1/NikClip/
+-rw-rw-rw-   0        0        0     3777 2023-06-08 01:31:18.000000 NikClip-2.1.1/NikClip/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 01:33:06.566053 NikClip-2.1.1/NikClip.egg-info/
+-rw-rw-rw-   0        0        0     2547 2023-06-08 01:33:06.000000 NikClip-2.1.1/NikClip.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      186 2023-06-08 01:33:06.000000 NikClip-2.1.1/NikClip.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 01:33:06.000000 NikClip-2.1.1/NikClip.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2023-06-08 01:33:06.000000 NikClip-2.1.1/NikClip.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2547 2023-06-08 01:33:06.584168 NikClip-2.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2063 2023-05-24 05:11:07.000000 NikClip-2.1.1/README.md
+-rw-rw-rw-   0        0        0      100 2023-05-21 16:11:11.000000 NikClip-2.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0      586 2023-06-08 01:33:06.599422 NikClip-2.1.1/setup.cfg
```

### Comparing `NikClip-2.1/LICENSE` & `NikClip-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NikClip-2.1/NikClip.egg-info/PKG-INFO` & `NikClip-2.1.1/NikClip.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikClip
-Version: 2.1
+Version: 2.1.1
 Summary: A full fledged media-player and media-downloader
 Home-page: https://github.com/Nikhilodeon1/NikClip
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikClip-2.1/PKG-INFO` & `NikClip-2.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: NikClip
-Version: 2.1
+Version: 2.1.1
 Summary: A full fledged media-player and media-downloader
 Home-page: https://github.com/Nikhilodeon1/NikClip
 Author: Nikhil Tamvada (Nikhilodeon1)
 Author-email: nikhiltamvada@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `NikClip-2.1/README.md` & `NikClip-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `NikClip-2.1/setup.cfg` & `NikClip-2.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 204e 696b 436c 6970 0d0a 7665 7273   = NikClip..vers
-00000020: 696f 6e20 3d20 322e 310d 0a61 7574 686f  ion = 2.1..autho
-00000030: 7220 3d20 4e69 6b68 696c 2054 616d 7661  r = Nikhil Tamva
-00000040: 6461 2028 4e69 6b68 696c 6f64 656f 6e31  da (Nikhilodeon1
-00000050: 290d 0a61 7574 686f 725f 656d 6169 6c20  )..author_email 
-00000060: 3d20 6e69 6b68 696c 7461 6d76 6164 6140  = nikhiltamvada@
-00000070: 676d 6169 6c2e 636f 6d0d 0a64 6573 6372  gmail.com..descr
-00000080: 6970 7469 6f6e 203d 2041 2066 756c 6c20  iption = A full 
-00000090: 666c 6564 6765 6420 6d65 6469 612d 706c  fledged media-pl
-000000a0: 6179 6572 2061 6e64 206d 6564 6961 2d64  ayer and media-d
-000000b0: 6f77 6e6c 6f61 6465 720d 0a6c 6f6e 675f  ownloader..long_
-000000c0: 6465 7363 7269 7074 696f 6e20 3d20 6669  description = fi
-000000d0: 6c65 3a20 5245 4144 4d45 2e6d 640d 0a6c  le: README.md..l
-000000e0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-000000f0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-00000100: 6578 742f 6d61 726b 646f 776e 0d0a 686f  ext/markdown..ho
-00000110: 6d65 5f70 6167 6520 3d20 6874 7470 733a  me_page = https:
-00000120: 2f2f 6769 7468 7562 2e63 6f6d 2f4e 696b  //github.com/Nik
-00000130: 6869 6c6f 6465 6f6e 312f 4e69 6b43 6c69  hilodeon1/NikCli
-00000140: 700d 0a63 6c61 7373 6966 6965 7273 203d  p..classifiers =
-00000150: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
-00000160: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
-00000170: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
-00000180: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
-00000190: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
-000001a0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
-000001b0: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
-000001c0: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
-000001d0: 735d 0d0a 7061 636b 6167 6573 203d 2066  s]..packages = f
-000001e0: 696e 643a 0d0a 7079 7468 6f6e 5f72 6571  ind:..python_req
-000001f0: 7569 7265 7320 3d20 3e3d 332e 380d 0a69  uires = >=3.8..i
-00000200: 6e63 6c75 6465 5f70 6163 6b61 6765 5f64  nclude_package_d
-00000210: 6174 6120 3d20 5472 7565 0d0a 0d0a 5b65  ata = True....[e
-00000220: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
-00000230: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
-00000240: 203d 2030 0d0a 0d0a                       = 0....
+00000020: 696f 6e20 3d20 322e 312e 310d 0a61 7574  ion = 2.1.1..aut
+00000030: 686f 7220 3d20 4e69 6b68 696c 2054 616d  hor = Nikhil Tam
+00000040: 7661 6461 2028 4e69 6b68 696c 6f64 656f  vada (Nikhilodeo
+00000050: 6e31 290d 0a61 7574 686f 725f 656d 6169  n1)..author_emai
+00000060: 6c20 3d20 6e69 6b68 696c 7461 6d76 6164  l = nikhiltamvad
+00000070: 6140 676d 6169 6c2e 636f 6d0d 0a64 6573  a@gmail.com..des
+00000080: 6372 6970 7469 6f6e 203d 2041 2066 756c  cription = A ful
+00000090: 6c20 666c 6564 6765 6420 6d65 6469 612d  l fledged media-
+000000a0: 706c 6179 6572 2061 6e64 206d 6564 6961  player and media
+000000b0: 2d64 6f77 6e6c 6f61 6465 720d 0a6c 6f6e  -downloader..lon
+000000c0: 675f 6465 7363 7269 7074 696f 6e20 3d20  g_description = 
+000000d0: 6669 6c65 3a20 5245 4144 4d45 2e6d 640d  file: README.md.
+000000e0: 0a6c 6f6e 675f 6465 7363 7269 7074 696f  .long_descriptio
+000000f0: 6e5f 636f 6e74 656e 745f 7479 7065 203d  n_content_type =
+00000100: 2074 6578 742f 6d61 726b 646f 776e 0d0a   text/markdown..
+00000110: 686f 6d65 5f70 6167 6520 3d20 6874 7470  home_page = http
+00000120: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f4e  s://github.com/N
+00000130: 696b 6869 6c6f 6465 6f6e 312f 4e69 6b43  ikhilodeon1/NikC
+00000140: 6c69 700d 0a63 6c61 7373 6966 6965 7273  lip..classifiers
+00000150: 203d 200d 0a09 5072 6f67 7261 6d6d 696e   = ...Programmin
+00000160: 6720 4c61 6e67 7561 6765 203a 3a20 5079  g Language :: Py
+00000170: 7468 6f6e 203a 3a20 330d 0a09 4c69 6365  thon :: 3...Lice
+00000180: 6e73 6520 3a3a 204f 5349 2041 7070 726f  nse :: OSI Appro
+00000190: 7665 6420 3a3a 204d 4954 204c 6963 656e  ved :: MIT Licen
+000001a0: 7365 0d0a 094f 7065 7261 7469 6e67 2053  se...Operating S
+000001b0: 7973 7465 6d20 3a3a 204f 5320 496e 6465  ystem :: OS Inde
+000001c0: 7065 6e64 656e 740d 0a0d 0a5b 6f70 7469  pendent....[opti
+000001d0: 6f6e 735d 0d0a 7061 636b 6167 6573 203d  ons]..packages =
+000001e0: 2066 696e 643a 0d0a 7079 7468 6f6e 5f72   find:..python_r
+000001f0: 6571 7569 7265 7320 3d20 3e3d 332e 380d  equires = >=3.8.
+00000200: 0a69 6e63 6c75 6465 5f70 6163 6b61 6765  .include_package
+00000210: 5f64 6174 6120 3d20 5472 7565 0d0a 0d0a  _data = True....
+00000220: 5b65 6767 5f69 6e66 6f5d 0d0a 7461 675f  [egg_info]..tag_
+00000230: 6275 696c 6420 3d20 0d0a 7461 675f 6461  build = ..tag_da
+00000240: 7465 203d 2030 0d0a 0d0a                 te = 0....
```

