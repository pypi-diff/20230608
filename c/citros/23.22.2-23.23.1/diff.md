# Comparing `tmp/citros-23.22.2.tar.gz` & `tmp/citros-23.23.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "citros-23.22.2.tar", last modified: Tue May 30 10:47:03 2023, max compression
+gzip compressed data, was "citros-23.23.1.tar", last modified: Thu Jun  8 14:53:45 2023, max compression
```

## Comparing `citros-23.22.2.tar` & `citros-23.23.1.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-30 10:46:45.000000 citros-23.22.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-30 10:47:03.120994 citros-23.22.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8003 2023-05-30 10:46:45.000000 citros-23.22.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.116994 citros-23.22.2/bin/
--rw-r--r--   0 runner    (1001) docker     (123)    15347 2023-05-30 10:46:45.000000 citros-23.22.2/bin/citros
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-30 10:46:45.000000 citros-23.22.2/citros/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14142 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros.py
--rw-r--r--   0 runner    (1001) docker     (123)    13838 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_bag.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_batch.py
--rw-r--r--   0 runner    (1001) docker     (123)     7597 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_events.py
--rw-r--r--   0 runner    (1001) docker     (123)     9274 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-05-30 10:46:45.000000 citros-23.22.2/citros/citros_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/launches/
--rw-r--r--   0 runner    (1001) docker     (123)      972 2023-05-30 10:46:45.000000 citros-23.22.2/citros/launches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-30 10:46:45.000000 citros-23.22.2/citros/launches/launch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-05-30 10:46:45.000000 citros-23.22.2/citros/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-05-30 10:46:45.000000 citros-23.22.2/citros/logger/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-05-30 10:46:45.000000 citros-23.22.2/citros/logger/logger_pg_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/parsers/
--rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-05-30 10:46:45.000000 citros-23.22.2/citros/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 10:46:45.000000 citros-23.22.2/citros/parsers/parser_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    18298 2023-05-30 10:46:45.000000 citros-23.22.2/citros/parsers/parser_ros2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros/rosbag/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/reader_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/reader_mcap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-05-30 10:46:45.000000 citros-23.22.2/citros/rosbag/reader_sqlite.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/citros.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8290 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      785 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-30 10:47:03.000000 citros-23.22.2/citros.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-05-30 10:46:45.000000 citros-23.22.2/citros_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-30 10:47:03.120994 citros-23.22.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2043 2023-05-30 10:46:45.000000 citros-23.22.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-30 10:47:03.120994 citros-23.22.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:46:45.000000 citros-23.22.2/tests/test_parse_ros_project.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-30 10:46:45.000000 citros-23.22.2/tests/test_uplosd_to_server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-08 14:53:26.000000 citros-23.23.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 14:53:45.167378 citros-23.23.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8896 2023-06-08 14:53:26.000000 citros-23.23.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)    17335 2023-06-08 14:53:26.000000 citros-23.23.1/bin/citros
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-06-08 14:53:26.000000 citros-23.23.1/citros/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19208 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12122 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_bag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2178 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_batch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1390 2023-06-08 14:53:26.000000 citros-23.23.1/citros/citros_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros/launches/
+-rw-r--r--   0 runner    (1001) docker     (123)      972 2023-06-08 14:53:26.000000 citros-23.23.1/citros/launches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-08 14:53:26.000000 citros-23.23.1/citros/launches/launch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-06-08 14:53:26.000000 citros-23.23.1/citros/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3200 2023-06-08 14:53:26.000000 citros-23.23.1/citros/logger/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-08 14:53:26.000000 citros-23.23.1/citros/logger/logger_pg_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/citros/parsers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-08 14:53:26.000000 citros-23.23.1/citros/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 14:53:26.000000 citros-23.23.1/citros/parsers/parser_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20601 2023-06-08 14:53:26.000000 citros-23.23.1/citros/parsers/parser_ros2.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/citros/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/reader_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/reader_mcap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-06-08 14:53:26.000000 citros-23.23.1/citros/rosbag/reader_sqlite.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.163378 citros-23.23.1/citros.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9183 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-08 14:53:45.000000 citros-23.23.1/citros.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-08 14:53:26.000000 citros-23.23.1/citros_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 14:53:45.167378 citros-23.23.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-06-08 14:53:26.000000 citros-23.23.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 14:53:45.167378 citros-23.23.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3595 2023-06-08 14:53:26.000000 citros-23.23.1/tests/test_parse_makefile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2248 2023-06-08 14:53:26.000000 citros-23.23.1/tests/test_parse_setup_py.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-06-08 14:53:26.000000 citros-23.23.1/tests/test_parse_xml.py
```

### Comparing `citros-23.22.2/LICENSE` & `citros-23.23.1/LICENSE`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/PKG-INFO` & `citros-23.23.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,519 +1,556 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6369 7472  : 2.1.Name: citr
-00000020: 6f73 0a56 6572 7369 6f6e 3a20 3233 2e32  os.Version: 23.2
-00000030: 322e 320a 5375 6d6d 6172 793a 2041 2063  2.2.Summary: A c
-00000040: 6c69 2065 6e74 7279 706f 696e 7420 666f  li entrypoint fo
-00000050: 7220 7468 6520 6369 7472 6f73 2073 7973  r the citros sys
-00000060: 7465 6d2e 0a48 6f6d 652d 7061 6765 3a20  tem..Home-page: 
-00000070: 6874 7470 3a2f 2f70 7970 692e 7079 7468  http://pypi.pyth
-00000080: 6f6e 2e6f 7267 2f70 7970 692f 6369 7472  on.org/pypi/citr
-00000090: 6f73 5f63 6c69 2f0a 4175 7468 6f72 3a20  os_cli/.Author: 
-000000a0: 766f 7661 636f 6f70 6572 0a41 7574 686f  vovacooper.Autho
-000000b0: 722d 656d 6169 6c3a 2076 6f76 6140 6c75  r-email: vova@lu
-000000c0: 6c61 762e 7370 6163 650a 4c69 6365 6e73  lav.space.Licens
-000000d0: 653a 204c 4943 454e 5345 2e74 7874 0a44  e: LICENSE.txt.D
-000000e0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
-000000f0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
-00000100: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
-00000110: 696c 653a 204c 4943 454e 5345 0a0a 6060  ile: LICENSE..``
-00000120: 6070 7974 686f 6e0a 2320 3d3d 3d3d 3d3d  `python.# ======
-00000130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000150: 3d3d 3d3d 3d3d 3d3d 0a23 2020 20e2 9688  ========.#   ...
-00000160: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00000170: 9597 e296 88e2 9688 e295 97e2 9688 e296  ................
-00000180: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
-00000190: e296 88e2 9597 e296 88e2 9688 e296 88e2  ................
-000001a0: 9688 e296 88e2 9688 e295 9720 20e2 9688  ...........  ...
-000001b0: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-000001c0: 9597 20e2 9688 e296 88e2 9688 e296 88e2  .. .............
-000001d0: 9688 e296 88e2 9688 e295 970a 2320 20e2  ............#  .
-000001e0: 9688 e296 88e2 9594 e295 90e2 9590 e295  ................
-000001f0: 90e2 9590 e295 9de2 9688 e296 88e2 9591  ................
-00000200: e295 9ae2 9590 e295 90e2 9688 e296 88e2  ................
-00000210: 9594 e295 90e2 9590 e295 9de2 9688 e296  ................
-00000220: 88e2 9594 e295 90e2 9590 e296 88e2 9688  ................
-00000230: e295 97e2 9688 e296 88e2 9594 e295 90e2  ................
-00000240: 9590 e295 90e2 9688 e296 88e2 9597 e296  ................
-00000250: 88e2 9688 e295 94e2 9590 e295 90e2 9590  ................
-00000260: e295 90e2 959d 0a23 2020 e296 88e2 9688  .......#  ......
-00000270: e295 9120 2020 2020 e296 88e2 9688 e295  ...     ........
-00000280: 9120 2020 e296 88e2 9688 e295 9120 2020  .   .........   
-00000290: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-000002a0: 9688 e295 94e2 959d e296 88e2 9688 e295  ................
-000002b0: 9120 2020 e296 88e2 9688 e295 91e2 9688  .   ............
-000002c0: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-000002d0: 9688 e295 970a 2320 20e2 9688 e296 88e2  ......#  .......
-000002e0: 9591 2020 2020 20e2 9688 e296 88e2 9591  ..     .........
-000002f0: 2020 20e2 9688 e296 88e2 9591 2020 20e2     .........   .
-00000300: 9688 e296 88e2 9594 e295 90e2 9590 e296  ................
-00000310: 88e2 9688 e295 97e2 9688 e296 88e2 9591  ................
-00000320: 2020 20e2 9688 e296 88e2 9591 e295 9ae2     .............
-00000330: 9590 e295 90e2 9590 e295 90e2 9688 e296  ................
-00000340: 88e2 9591 0a23 2020 e295 9ae2 9688 e296  .....#  ........
-00000350: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
-00000360: e296 88e2 9688 e295 9120 2020 e296 88e2  .........   ....
-00000370: 9688 e295 9120 2020 e296 88e2 9688 e295  .....   ........
-00000380: 9120 20e2 9688 e296 88e2 9591 e295 9ae2  .  .............
-00000390: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-000003a0: 88e2 9594 e295 9de2 9688 e296 88e2 9688  ................
-000003b0: e296 88e2 9688 e296 88e2 9688 e295 910a  ................
-000003c0: 2320 2020 e295 9ae2 9590 e295 90e2 9590  #   ............
-000003d0: e295 90e2 9590 e295 9de2 959a e295 90e2  ................
-000003e0: 959d 2020 20e2 959a e295 90e2 959d 2020  ..   .........  
-000003f0: 20e2 959a e295 90e2 959d 2020 e295 9ae2   .........  ....
-00000400: 9590 e295 9d20 e295 9ae2 9590 e295 90e2  ..... ..........
-00000410: 9590 e295 90e2 9590 e295 9d20 e295 9ae2  ........... ....
-00000420: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
-00000430: 90e2 959d 2020 2020 2020 2020 2020 2020  ....            
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 2020 2020 2020 2020 2020 2020 0a23 203d              .# =
-00000460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 6060  =============.``
-00000490: 600a 2320 4349 5452 4f53 2043 4c49 0a0a  `.# CITROS CLI..
-000004a0: 5b21 5b50 7562 6c69 7368 2043 4954 524f  [![Publish CITRO
-000004b0: 535f 434c 4920 746f 2050 7950 4920 2f20  S_CLI to PyPI / 
-000004c0: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
-000004d0: 6769 7468 7562 2e63 6f6d 2f6c 756c 6176  github.com/lulav
-000004e0: 2f63 6974 726f 735f 636c 692f 6163 7469  /citros_cli/acti
-000004f0: 6f6e 732f 776f 726b 666c 6f77 732f 7265  ons/workflows/re
-00000500: 6c65 6173 655f 746f 5f70 7970 692e 7961  lease_to_pypi.ya
-00000510: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
-00000520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000530: 6d2f 6c75 6c61 762f 6369 7472 6f73 5f63  m/lulav/citros_c
-00000540: 6c69 2f61 6374 696f 6e73 2f77 6f72 6b66  li/actions/workf
-00000550: 6c6f 7773 2f72 656c 6561 7365 5f74 6f5f  lows/release_to_
-00000560: 7079 7069 2e79 616d 6c29 0a0a 2320 4465  pypi.yaml)..# De
-00000570: 7363 7269 7074 696f 6e0a 0a54 6869 7320  scription..This 
-00000580: 7265 706f 7369 746f 7279 2069 7320 6120  repository is a 
-00000590: 7079 7468 6f6e 2070 6163 6b61 6765 2074  python package t
-000005a0: 6861 7420 696d 706c 656d 656e 7473 2074  hat implements t
-000005b0: 6865 2043 4954 524f 5320 434c 4920 4150  he CITROS CLI AP
-000005c0: 492e 0a49 7420 6973 2072 756e 2062 7920  I..It is run by 
-000005d0: 7468 6520 7573 6572 2069 6e73 6964 6520  the user inside 
-000005e0: 7468 6520 524f 5320 7072 6f6a 6563 7420  the ROS project 
-000005f0: 666f 6c64 6572 2e20 0a0a 2320 5072 6572  folder. ..# Prer
-00000600: 6571 7569 7369 7465 730a 0a2d 205b 7673  equisites..- [vs
-00000610: 636f 6465 5d28 6874 7470 733a 2f2f 636f  code](https://co
-00000620: 6465 2e76 6973 7561 6c73 7475 6469 6f2e  de.visualstudio.
-00000630: 636f 6d2f 646f 776e 6c6f 6164 290a 2d20  com/download).- 
-00000640: 5b44 6f63 6b65 725d 2868 7474 7073 3a2f  [Docker](https:/
-00000650: 2f77 7777 2e64 6f63 6b65 722e 636f 6d2f  /www.docker.com/
-00000660: 290a 2d20 5b50 7974 686f 6e33 5d28 6874  ).- [Python3](ht
-00000670: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
-00000680: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
-00000690: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
-000006a0: 0a0a 312e 2063 6c6f 6e65 2074 6865 2072  ..1. clone the r
-000006b0: 6570 6f3a 0a20 2020 200a 2020 2020 2020  epo:.    .      
-000006c0: 2020 6769 7420 636c 6f6e 6520 6769 7440    git clone git@
-000006d0: 6769 7468 7562 2e63 6f6d 3a6c 756c 6176  github.com:lulav
-000006e0: 2f63 6974 726f 735f 636c 692e 6769 740a  /citros_cli.git.
-000006f0: 0a32 2e20 5769 7468 696e 2074 6865 2063  .2. Within the c
-00000700: 6c6f 6e65 6420 6063 6974 726f 735f 636c  loned `citros_cl
-00000710: 6960 2066 6f6c 6465 722c 206f 7065 6e20  i` folder, open 
-00000720: 5653 436f 6465 3a0a 2020 2020 0a20 2020  VSCode:.    .   
-00000730: 2020 2020 2063 6f64 6520 2e0a 0a20 2020       code ...   
-00000740: 2061 6e64 2072 656f 7065 6e20 7468 6520   and reopen the 
-00000750: 666f 6c64 6572 2069 6e73 6964 6520 6120  folder inside a 
-00000760: 4465 7620 436f 6e74 6169 6e65 722e 0a0a  Dev Container...
-00000770: 332e 2049 6e73 7461 6c6c 2074 6865 2070  3. Install the p
-00000780: 6163 6b61 6765 2066 726f 6d20 7468 6520  ackage from the 
-00000790: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
-000007a0: 792c 2077 6974 6820 736f 6674 206c 696e  y, with soft lin
-000007b0: 6b73 2074 6f20 6465 7620 656e 7669 726f  ks to dev enviro
-000007c0: 6e6d 656e 7420 0a0a 2020 2020 2020 2020  nment ..        
-000007d0: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
-000007e0: 6e73 7461 6c6c 202d 6520 2e0a 0a20 2020  nstall -e ...   
-000007f0: 2028 7265 636f 6d6d 656e 6465 6420 6475   (recommended du
-00000800: 7269 6e67 2064 6576 656c 6f70 6d65 6e74  ring development
-00000810: 292c 0a0a 2020 2020 6f72 200a 0a20 2020  ),..    or ..   
-00000820: 2049 6e73 7461 6c6c 2074 6865 2070 6163   Install the pac
-00000830: 6b61 6765 2066 726f 6d20 7468 6520 6375  kage from the cu
-00000840: 7272 656e 7420 6469 7265 6374 6f72 792c  rrent directory,
-00000850: 2064 6972 6563 746c 7920 746f 2061 2067   directly to a g
-00000860: 6c6f 6261 6c20 6269 6e20 666f 6c64 6572  lobal bin folder
-00000870: 200a 0a20 2020 2020 2020 2070 7974 686f   ..        pytho
-00000880: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
-00000890: 6c20 2e0a 2020 2020 0a20 2020 2028 7368  l ..    .    (sh
-000008a0: 6f75 6c64 2062 6520 646f 6e65 2062 6566  ould be done bef
-000008b0: 6f72 6520 7570 6c6f 6164 696e 6720 746f  ore uploading to
-000008c0: 2050 7950 492c 2074 6f20 6d61 6b65 2073   PyPI, to make s
-000008d0: 7572 6520 7468 6520 696e 7374 616c 6c61  ure the installa
-000008e0: 7469 6f6e 2069 7320 776f 726b 696e 6720  tion is working 
-000008f0: 7072 6f70 6572 6c79 292e 0a0a 2320 434c  properly)...# CL
-00000900: 4920 4150 4920 636f 6d6d 616e 6473 3a0a  I API commands:.
-00000910: 0a23 2320 6c6f 6769 6e0a 4c6f 6769 6e20  .## login.Login 
-00000920: 746f 2043 4954 524f 532e 0a0a 4166 7465  to CITROS...Afte
-00000930: 7220 656e 7465 7269 6e67 2074 6865 2063  r entering the c
-00000940: 6f6d 6d61 6e64 2c20 796f 7520 7769 6c6c  ommand, you will
-00000950: 2062 6520 7072 6f6d 7074 6564 2066 6f72   be prompted for
-00000960: 2079 6f75 7220 656d 6169 6c20 2874 6865   your email (the
-00000970: 2075 7365 726e 616d 6529 2061 6e64 2070   username) and p
-00000980: 6173 7377 6f72 642e 0a0a 6578 616d 706c  assword...exampl
-00000990: 653a 0a0a 2020 2020 726f 7340 7368 616c  e:..    ros@shal
-000009a0: 6576 2d49 6e73 7069 726f 6e2d 3135 2d35  ev-Inspiron-15-5
-000009b0: 3531 303a 2f77 6f72 6b73 7061 6365 732f  510:/workspaces/
-000009c0: 6361 6e6e 6f6e 2420 6369 7472 6f73 206c  cannon$ citros l
-000009d0: 6f67 696e 0a20 2020 2065 6d61 696c 3a20  ogin.    email: 
-000009e0: 7368 616c 6576 406c 756c 6176 2e73 7061  shalev@lulav.spa
-000009f0: 6365 0a20 2020 2050 6173 7377 6f72 643a  ce.    Password:
-00000a00: 200a 2020 2020 5573 6572 206c 6f67 6765   .    User logge
-00000a10: 6420 696e 2e0a 2020 2020 5b32 3032 332d  d in..    [2023-
-00000a20: 3035 2d31 3120 3038 3a31 323a 3138 2c30  05-11 08:12:18,0
-00000a30: 3635 5d20 5b63 6974 726f 732e 6369 7472  65] [citros.citr
-00000a40: 6f73 2d4e 6f6e 652d 4e6f 6e65 2e6c 6f67  os-None-None.log
-00000a50: 696e 3a32 3638 5d20 5b49 4e46 4f5d 3a20  in:268] [INFO]: 
-00000a60: 4175 7468 656e 7469 6361 7465 6421 0a0a  Authenticated!..
-00000a70: 2323 2061 7574 6865 6e74 6963 6174 650a  ## authenticate.
-00000a80: 4175 7468 656e 7469 6361 7465 2079 6f75  Authenticate you
-00000a90: 7273 656c 6620 746f 2043 4954 524f 5320  rself to CITROS 
-00000aa0: 7768 656e 2061 206c 6f67 696e 2069 7320  when a login is 
-00000ab0: 6e6f 7420 706f 7373 6962 6c65 2c20 652e  not possible, e.
-00000ac0: 672e 2077 6865 6e20 7275 6e6e 696e 6720  g. when running 
-00000ad0: 696e 2074 6865 2063 6c6f 7564 206f 7220  in the cloud or 
-00000ae0: 7065 7266 6f72 6d69 6e67 2061 7574 6f6d  performing autom
-00000af0: 6174 6564 2074 6573 7473 2e0a 0a46 6972  ated tests...Fir
-00000b00: 7374 2c20 696e 206f 7264 6572 2074 6f20  st, in order to 
-00000b10: 6f62 7461 696e 2061 2076 616c 6964 2061  obtain a valid a
-00000b20: 7574 6865 6e74 6963 6174 696f 6e20 6b65  uthentication ke
-00000b30: 792c 206c 6f67 696e 2074 6f20 5b63 6974  y, login to [cit
-00000b40: 726f 735d 2868 7474 703a 2f2f 6369 7472  ros](http://citr
-00000b50: 6f73 2e69 6f2f 2920 616e 6420 636c 6963  os.io/) and clic
-00000b60: 6b20 7468 6520 6041 6464 2050 726f 6a65  k the `Add Proje
-00000b70: 6374 6020 6275 7474 6f6e 2069 6e20 7468  ct` button in th
-00000b80: 6520 746f 7020 7269 6768 7420 636f 726e  e top right corn
-00000b90: 6572 3a0a 215b 6164 645f 7072 6f6a 5d28  er:.![add_proj](
-00000ba0: 696d 672f 6164 645f 7072 6f6a 2e70 6e67  img/add_proj.png
-00000bb0: 2022 6164 6420 7072 6f6a 6563 7422 290a   "add project").
-00000bc0: 0a43 6f70 7920 7468 6520 6c69 6e65 2060  .Copy the line `
-00000bd0: 6369 7472 6f73 2061 7574 6865 6e74 6963  citros authentic
-00000be0: 6174 6520 3c79 6f75 7220 6b65 793e 603a  ate <your key>`:
-00000bf0: 0a21 5b61 7574 685f 6b65 795d 2869 6d67  .![auth_key](img
-00000c00: 2f61 7574 685f 6b65 792e 706e 6720 2261  /auth_key.png "a
-00000c10: 7574 6865 6e74 6963 6174 696f 6e20 6b65  uthentication ke
-00000c20: 7922 290a 0a20 616e 6420 7061 7374 6520  y").. and paste 
-00000c30: 6974 2069 6e20 7468 6520 636f 6d6d 616e  it in the comman
-00000c40: 6420 6c69 6e65 2e0a 0a65 7861 6d70 6c65  d line...example
-00000c50: 3a0a 0a20 2020 2072 6f73 4073 6861 6c65  :..    ros@shale
-00000c60: 762d 496e 7370 6972 6f6e 2d31 352d 3535  v-Inspiron-15-55
-00000c70: 3130 3a2f 776f 726b 7370 6163 6573 2f63  10:/workspaces/c
-00000c80: 616e 6e6f 6e24 2063 6974 726f 7320 6175  annon$ citros au
-00000c90: 7468 656e 7469 6361 7465 2065 794a 6862  thenticate eyJhb
-00000ca0: 4763 694f 694a 4955 7a49 314e 6949 7349  GciOiJIUzI1NiIsI
-00000cb0: 6e52 3563 4349 3649 6b70 5856 434a 392e  nR5cCI6IkpXVCJ9.
-00000cc0: 6579 4a79 6232 786c 496a 6f69 5932 6c30  eyJyb2xlIjoiY2l0
-00000cd0: 636d 397a 5832 466b 6257 6c75 4969 7769  cm9zX2FkbWluIiwi
-00000ce0: 6458 4e6c 636c 3970 5a43 4936 496a 4535  dXNlcl9pZCI6IjE5
-00000cf0: 4e7a 686a 4f44 5534 4c54 526a 596d 4574  NzhjODU4LTRjYmEt
-00000d00: 4e44 5979 4e53 3034 4e6a 646c 4c54 5577  NDYyNS04NjdlLTUw
-00000d10: 4d6a 4d32 5a6d 526a 4e6d 5135 4d53 4973  MjM2ZmRjNmQ5MSIs
-00000d20: 496e 567a 5a58 4a66 626d 4674 5a53 4936  InVzZXJfbmFtZSI6
-00000d30: 496e 4e6f 5957 786c 6469 4973 496d 4e70  InNoYWxldiIsImNp
-00000d40: 6448 4a76 6331 3979 6232 786c 496a 6f69  dHJvc19yb2xlIjoi
-00000d50: 6458 4e6c 6369 4973 496d 3979 5a32 4675  dXNlciIsIm9yZ2Fu
-00000d60: 6158 7068 6447 6c76 626c 3970 5a43 4936  aXphdGlvbl9pZCI6
-00000d70: 496d 5535 4d54 566b 4e6a 4d35 4c54 597a  ImU5MTVkNjM5LTYz
-00000d80: 4e7a 4974 4e44 566c 4e43 3034 4e54 566b  NzItNDVlNC04NTVk
-00000d90: 4c57 4534 597a 6c69 4e32 5132 5957 4977  LWE4YzliN2Q2YWIw
-00000da0: 4d69 4973 496d 3979 5a32 4675 6158 7068  MiIsIm9yZ2FuaXph
-00000db0: 6447 6c76 626c 3930 6558 426c 496a 6f69  dGlvbl90eXBlIjoi
-00000dc0: 5455 464f 5155 6446 4969 7769 5a47 3974  TUFOQUdFIiwiZG9t
-00000dd0: 5957 6c75 5833 4279 5a57 5a70 6543 4936  YWluX3ByZWZpeCI6
-00000de0: 496d 7831 6247 4632 4969 7769 5a58 6877  Imx1bGF2IiwiZXhw
-00000df0: 496a 6f78 4e6a 677a 4e7a 4131 4f54 557a  IjoxNjgzNzA1OTUz
-00000e00: 4c43 4a70 5958 5169 4f6a 4532 4f44 4d32  LCJpYXQiOjE2ODM2
-00000e10: 4d54 6b31 4e54 4d73 496d 4631 5a43 4936  MTk1NTMsImF1ZCI6
-00000e20: 496e 4276 6333 526e 636d 4677 6147 6c73  InBvc3RncmFwaGls
-00000e30: 5a53 4973 496d 6c7a 6379 4936 496e 4276  ZSIsImlzcyI6InBv
-00000e40: 6333 526e 636d 4677 6147 6c73 5a53 4a39  c3RncmFwaGlsZSJ9
-00000e50: 2e68 4b67 7832 596c 444d 6848 3233 7047  .hKgx2YlDMhH23pG
-00000e60: 435a 4768 3359 7161 6158 3377 5469 6b6a  CZGh3YqaaX3wTikj
-00000e70: 4242 7970 4972 5f64 4d38 7467 0a20 2020  BBypIr_dM8tg.   
-00000e80: 2041 7574 6865 6e74 6963 6174 6564 210a   Authenticated!.
-00000e90: 2020 2020 5b32 3032 332d 3035 2d31 3120      [2023-05-11 
-00000ea0: 3038 3a35 373a 3131 2c30 3030 5d20 5b63  08:57:11,000] [c
-00000eb0: 6974 726f 732e 6369 7472 6f73 2d4e 6f6e  itros.citros-Non
-00000ec0: 652d 4e6f 6e65 2e61 7574 6865 6e74 6963  e-None.authentic
-00000ed0: 6174 655f 7769 7468 5f6b 6579 3a32 3139  ate_with_key:219
-00000ee0: 5d20 5b49 4e46 4f5d 3a20 4175 7468 656e  ] [INFO]: Authen
-00000ef0: 7469 6361 7465 6421 0a4e 6f74 653a 2074  ticated!.Note: t
-00000f00: 6865 206b 6579 2069 7320 7661 6c69 6420  he key is valid 
-00000f10: 666f 7220 7477 6f20 6461 7973 2c20 6166  for two days, af
-00000f20: 7465 7220 7768 6963 6820 6120 6e65 7720  ter which a new 
-00000f30: 6b65 7920 6e65 6564 7320 746f 2062 6520  key needs to be 
-00000f40: 6765 6e65 7261 7465 642e 2020 0a0a 2323  generated.  ..##
-00000f50: 206c 6f67 6f75 740a 4c6f 676f 7574 206f   logout.Logout o
-00000f60: 6620 4349 5452 4f53 2e0a 0a65 7861 6d70  f CITROS...examp
-00000f70: 6c65 3a0a 0a20 2020 2072 6f73 4073 6861  le:..    ros@sha
-00000f80: 6c65 762d 496e 7370 6972 6f6e 2d31 352d  lev-Inspiron-15-
-00000f90: 3535 3130 3a2f 776f 726b 7370 6163 6573  5510:/workspaces
-00000fa0: 2f63 616e 6e6f 6e24 2063 6974 726f 7320  /cannon$ citros 
-00000fb0: 6c6f 676f 7574 0a20 2020 2055 7365 7220  logout.    User 
-00000fc0: 6c6f 6767 6564 206f 7574 2e0a 2323 2073  logged out..## s
-00000fd0: 796e 630a 5379 6e63 2074 6865 2072 6f73  ync.Sync the ros
-00000fe0: 2070 726f 6a65 6374 2074 6f20 6369 7472   project to citr
-00000ff0: 6f73 2e0a 0a54 6869 7320 636f 6d6d 616e  os...This comman
-00001000: 6420 7769 6c6c 2070 6172 7365 2079 6f75  d will parse you
-00001010: 7220 524f 5332 2070 726f 6a65 6374 2c20  r ROS2 project, 
-00001020: 6578 7472 6163 7420 7468 6520 6e61 6d65  extract the name
-00001030: 7320 6f66 2061 6c6c 2074 6865 2070 6163  s of all the pac
-00001040: 6b61 6765 732c 200a 6e6f 6465 732c 2070  kages, .nodes, p
-00001050: 6172 616d 6574 6572 7320 616e 6420 6c61  arameters and la
-00001060: 756e 6368 2066 696c 6573 2028 616e 6420  unch files (and 
-00001070: 736f 6d65 206f 7468 6572 206d 6574 6164  some other metad
-00001080: 6174 6129 2c20 0a61 7373 6967 6e20 6561  ata), .assign ea
-00001090: 6368 206f 6620 7468 656d 2061 2055 4944  ch of them a UID
-000010a0: 2061 6e64 2075 706c 6f61 6420 7468 656d   and upload them
-000010b0: 2074 6f20 7468 6520 6369 7472 6f73 2064   to the citros d
-000010c0: 6174 6162 6173 652e 0a0a 6578 616d 706c  atabase...exampl
-000010d0: 653a 0a20 2020 200a 2020 2020 726f 7340  e:.    .    ros@
-000010e0: 7368 616c 6576 2d49 6e73 7069 726f 6e2d  shalev-Inspiron-
-000010f0: 3135 2d35 3531 303a 2f77 6f72 6b73 7061  15-5510:/workspa
-00001100: 6365 732f 6d61 7373 5f73 7072 696e 675f  ces/mass_spring_
-00001110: 6475 6d70 6572 2420 6369 7472 6f73 2073  dumper$ citros s
-00001120: 796e 630a 2020 2020 2d2d 2d2d 2d2d 2d2d  ync.    --------
-00001130: 2d2d 2d2d 2d2d 2d2d 2d2d 2d73 796e 635f  -----------sync_
-00001140: 7072 6f6a 6563 742d 2d2d 2d2d 2d2d 2d2d  project---------
-00001150: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 202e  ----------.    .
-00001160: 2e2e 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  ...    ---------
-00001170: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d44 4f4e  -------------DON
-00001180: 452d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  E---------------
-00001190: 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 6620 7468  ---------..If th
-000011a0: 6572 6520 7765 7265 206e 6f20 6368 616e  ere were no chan
-000011b0: 6765 7320 7369 6e63 6520 7468 6520 6c61  ges since the la
-000011c0: 7374 2073 796e 632c 2074 6865 2073 796e  st sync, the syn
-000011d0: 6320 6973 2075 6e6e 6563 6573 7361 7279  c is unnecessary
-000011e0: 3a0a 0a20 2020 2072 6f73 4073 6861 6c65  :..    ros@shale
-000011f0: 762d 496e 7370 6972 6f6e 2d31 352d 3535  v-Inspiron-15-55
-00001200: 3130 3a2f 776f 726b 7370 6163 6573 2f6d  10:/workspaces/m
-00001210: 6173 735f 7370 7269 6e67 5f64 756d 7065  ass_spring_dumpe
-00001220: 7224 2063 6974 726f 7320 7379 6e63 0a20  r$ citros sync. 
-00001230: 2020 2070 726f 6a65 6374 2061 6c72 6561     project alrea
-00001240: 6479 2073 796e 6368 6564 2e0a 0a49 6620  dy synched...If 
-00001250: 7468 6973 2077 6173 2079 6f75 7220 6669  this was your fi
-00001260: 7273 7420 7469 6d65 2072 756e 6e69 6e67  rst time running
-00001270: 2073 796e 6320 6f6e 2074 6869 7320 7072   sync on this pr
-00001280: 6f6a 6563 742c 2079 6f75 2063 616e 206f  oject, you can o
-00001290: 7065 6e20 796f 7572 2066 6176 6f72 6974  pen your favorit
-000012a0: 6520 6272 6f77 7365 7220 616e 6420 6e61  e browser and na
-000012b0: 7669 6761 7465 2074 6f20 5b63 6974 726f  vigate to [citro
-000012c0: 732e 696f 5d28 6369 7472 6f73 2e69 6f29  s.io](citros.io)
-000012d0: 2061 6e64 206c 6f67 2069 6e2c 2061 6e64   and log in, and
-000012e0: 2075 6e64 6572 2074 6865 2070 726f 6a65   under the proje
-000012f0: 6374 206c 6973 7420 796f 7527 6c6c 2073  ct list you'll s
-00001300: 6565 2061 206e 6577 2069 7465 6d20 666f  ee a new item fo
-00001310: 7220 796f 7572 2070 726f 6a65 6374 2068  r your project h
-00001320: 6173 2062 6565 6e20 6164 6465 6420 746f  as been added to
-00001330: 2074 6865 206c 6973 743a 0a21 5b70 726f   the list:.![pro
-00001340: 6a65 6374 206c 6973 745d 2869 6d67 2f70  ject list](img/p
-00001350: 726f 6a5f 6c69 7374 2e70 6e67 2022 7072  roj_list.png "pr
-00001360: 6f6a 6563 7420 6c69 7374 2229 0a0a 0a23  oject list")...#
-00001370: 2323 2070 6172 616d 6574 6572 733a 0a70  ## parameters:.p
-00001380: 6172 616d 6574 6572 7c64 6573 6372 6970  arameter|descrip
-00001390: 7469 6f6e 0a7c 2d2d 7c2d 2d7c 0a7c 602d  tion.|--|--|.|`-
-000013a0: 6469 7260 203c 666f 6c64 6572 5f6e 616d  dir` <folder_nam
-000013b0: 653e 207c 2054 6865 2077 6f72 6b69 6e67  e> | The working
-000013c0: 2064 6972 6563 746f 7279 206f 6620 7468   directory of th
-000013d0: 6520 7072 6f6a 6563 742e 2044 6566 6175  e project. Defau
-000013e0: 6c74 7320 746f 2022 2e22 2e7c 0a7c 602d  lts to ".".|.|`-
-000013f0: 6e61 6d65 6020 3c70 726f 6a5f 6e61 6d65  name` <proj_name
-00001400: 3e20 7c20 5468 6520 6e61 6d65 206f 6620  > | The name of 
-00001410: 7468 6520 7072 6f6a 6563 742e 2044 6566  the project. Def
-00001420: 6175 6c74 7320 746f 2074 6865 206c 6173  aults to the las
-00001430: 7420 666f 6c64 6572 2069 6e20 7468 6520  t folder in the 
-00001440: 7061 7468 206f 6620 2a64 6972 2a7c 0a7c  path of *dir*|.|
-00001450: 602d 7760 2c20 602d 7773 6020 3c77 6f72  `-w`, `-ws` <wor
-00001460: 6b73 7061 6365 5f6e 616d 653e 207c 2054  kspace_name> | T
-00001470: 6865 206e 616d 6520 6f66 2061 2077 6f72  he name of a wor
-00001480: 6b73 7061 6365 2069 6e73 6964 6520 7468  kspace inside th
-00001490: 6520 7072 6f6a 6563 7420 6469 7265 6374  e project direct
-000014a0: 6f72 792e 204d 6179 2062 6520 7573 6564  ory. May be used
-000014b0: 206d 756c 7469 706c 6520 7469 6d65 7320   multiple times 
-000014c0: 666f 7220 6d75 6c74 6970 6c65 2077 6f72  for multiple wor
-000014d0: 6b73 7061 6365 732e 2044 6566 6175 6c74  kspaces. Default
-000014e0: 7320 746f 2022 2220 286e 616d 656c 792c  s to "" (namely,
-000014f0: 206e 6f20 776f 726b 7370 6163 652c 2070   no workspace, p
-00001500: 6163 6b61 6765 2066 6f6c 6465 7273 2061  ackage folders a
-00001510: 7265 2064 6972 6563 746c 7920 756e 6465  re directly unde
-00001520: 7220 7468 6520 7072 6f6a 6563 7420 666f  r the project fo
-00001530: 6c64 6572 2e20 4465 6661 756c 7420 6973  lder. Default is
-00001540: 2075 7365 6420 7768 6574 6865 7220 7468   used whether th
-00001550: 6973 2070 6172 616d 6574 6572 2069 7320  is parameter is 
-00001560: 7370 6563 6966 6965 6420 6f72 206e 6f74  specified or not
-00001570: 202d 2061 6464 6974 696f 6e61 6c20 6e61   - additional na
-00001580: 6d65 7370 6163 6573 2061 7265 2061 6464  mespaces are add
-00001590: 6564 2c20 6275 7420 646f 206e 6f74 206f  ed, but do not o
-000015a0: 7665 7277 7269 7465 2069 7429 2e20 7c0a  verwrite it). |.
-000015b0: 0a23 2320 7061 7261 6d73 0a65 7870 6572  .## params.exper
-000015c0: 696d 656e 7461 6c2e 0a0a 6765 6e65 7261  imental...genera
-000015d0: 7465 2070 6172 616d 6574 6572 7320 666f  te parameters fo
-000015e0: 7220 7468 6520 7072 6f6a 6563 740a 2323  r the project.##
-000015f0: 2072 756e 5f73 696d 756c 6174 696f 6e0a   run_simulation.
-00001600: 4372 6561 7465 2061 206e 6577 2062 6174  Create a new bat
-00001610: 6368 206f 6620 7369 6d75 6c61 7469 6f6e  ch of simulation
-00001620: 2072 756e 7320 666f 7220 796f 7572 2070   runs for your p
-00001630: 726f 6a65 6374 2061 6e64 2072 756e 2069  roject and run i
-00001640: 7420 6c6f 6361 6c6c 792e 0a0a 2323 2320  t locally...### 
-00001650: 7072 6572 6571 7569 7369 7465 733a 0a54  prerequisites:.T
-00001660: 6865 2070 726f 6a65 6374 2068 6173 2062  he project has b
-00001670: 6565 6e20 6275 696c 742c 2073 6f75 7263  een built, sourc
-00001680: 6564 2061 6e64 2060 7379 6e63 6065 6420  ed and `sync`ed 
-00001690: 7769 7468 2063 6974 726f 732c 2065 2e67  with citros, e.g
-000016a0: 2e3a 0a20 2020 200a 2020 2020 636f 6c63  .:.    .    colc
-000016b0: 6f6e 2062 7569 6c64 0a20 2020 2073 6f75  on build.    sou
-000016c0: 7263 6520 696e 7374 616c 6c2f 6c6f 6361  rce install/loca
-000016d0: 6c5f 7365 7475 702e 6261 7368 0a20 2020  l_setup.bash.   
-000016e0: 2063 6974 726f 7320 7379 6e63 0a0a 496e   citros sync..In
-000016f0: 2074 6865 2063 6974 726f 7320 6775 692c   the citros gui,
-00001700: 206e 6176 6967 6174 6520 746f 2079 6f75   navigate to you
-00001710: 7220 7072 6f6a 6563 7420 6279 2063 6c69  r project by cli
-00001720: 636b 696e 6720 7468 6520 7468 7265 6520  cking the three 
-00001730: 7665 7274 6963 616c 2064 6f74 7320 6f6e  vertical dots on
-00001740: 2074 6865 2072 6967 6874 2073 6964 6520   the right side 
-00001750: 6f66 206f 6620 796f 7572 2070 726f 6a65  of of your proje
-00001760: 6374 2773 2072 6f77 2069 6e20 7468 6520  ct's row in the 
-00001770: 7072 6f6a 6563 7420 6c69 7374 2061 6e64  project list and
-00001780: 2073 656c 6563 7420 606e 6176 6967 6174   select `navigat
-00001790: 6560 3a20 0a21 5b6e 6176 5f70 726f 6a5d  e`: .![nav_proj]
-000017a0: 2869 6d67 2f6e 6176 5f70 726f 6a2e 706e  (img/nav_proj.pn
-000017b0: 6720 226e 6176 6967 6174 6520 746f 2070  g "navigate to p
-000017c0: 726f 6a65 6374 2229 200a 0a77 6869 6368  roject") ..which
-000017d0: 2077 696c 6c20 7461 6b65 2079 6f75 2074   will take you t
-000017e0: 6f20 7468 6520 7072 6f6a 6563 7427 7320  o the project's 
-000017f0: 4465 7461 696c 7320 7061 6765 2e20 0a0a  Details page. ..
-00001800: 5468 6572 652c 2063 6c69 636b 2074 6865  There, click the
-00001810: 2060 5369 6d75 6c61 7469 6f6e 2053 6574   `Simulation Set
-00001820: 7570 6020 7461 623a 0a21 5b73 696d 5f73  up` tab:.![sim_s
-00001830: 6574 7570 5d28 696d 672f 7369 6d5f 7365  etup](img/sim_se
-00001840: 7475 702e 706e 6720 2273 696d 756c 6174  tup.png "simulat
-00001850: 696f 6e20 7365 7475 7022 290a 0a61 6e64  ion setup")..and
-00001860: 2063 6c69 636b 206f 6e20 606e 6577 602e   click on `new`.
-00001870: 0a0a 4669 6c6c 2069 6e20 616e 7920 7265  ..Fill in any re
-00001880: 6c65 7661 6e74 2064 6574 6169 6c73 2066  levant details f
-00001890: 6f72 2074 6865 206e 6577 2073 696d 756c  or the new simul
-000018a0: 6174 696f 6e20 616e 6420 7361 7665 3a0a  ation and save:.
-000018b0: 215b 7361 7665 5f6e 6577 5f73 696d 5d28  ![save_new_sim](
-000018c0: 696d 672f 7361 7665 5f6e 6577 5f73 696d  img/save_new_sim
-000018d0: 2e70 6e67 2022 7361 7665 206e 6577 2073  .png "save new s
-000018e0: 696d 756c 6174 696f 6e22 290a 0a4e 6f77  imulation")..Now
-000018f0: 2063 6c69 636b 206f 6e20 6052 756e 2053   click on `Run S
-00001900: 696d 756c 6174 696f 6e20 4c6f 6361 6c6c  imulation Locall
-00001910: 7960 3a0a 215b 7275 6e5f 7369 6d5f 6c6f  y`:.![run_sim_lo
-00001920: 635d 2869 6d67 2f72 756e 5f73 696d 5f6c  c](img/run_sim_l
-00001930: 6f63 2e70 6e67 2022 7275 6e20 7369 6d75  oc.png "run simu
-00001940: 6c61 7469 6f6e 206c 6f63 616c 6c79 2229  lation locally")
-00001950: 0a0a 616e 6420 696e 2074 6865 2070 6f70  ..and in the pop
-00001960: 2d75 7020 7468 6174 2063 6f6d 6573 2075  -up that comes u
-00001970: 702c 2063 6f70 7920 7468 6520 7369 6d75  p, copy the simu
-00001980: 6c61 7469 6f6e 2069 6420 7468 6174 2077  lation id that w
-00001990: 6173 2067 656e 6572 6174 6564 3a0a 215b  as generated:.![
-000019a0: 636f 7079 5f73 696d 5f69 645d 2869 6d67  copy_sim_id](img
-000019b0: 2f63 6f70 795f 7369 6d5f 6964 2e70 6e67  /copy_sim_id.png
-000019c0: 2022 636f 7079 2074 6865 2073 696d 756c   "copy the simul
-000019d0: 6174 696f 6e20 6964 2229 0a0a 616e 6420  ation id")..and 
-000019e0: 6e6f 772c 2066 696e 616c 6c79 2c20 696e  now, finally, in
-000019f0: 2074 6865 2063 6f6d 6d61 6e64 2d6c 696e   the command-lin
-00001a00: 652c 2072 756e 0a0a 2020 2020 6369 7472  e, run..    citr
-00001a10: 6f73 2072 756e 5f73 696d 756c 6174 696f  os run_simulatio
-00001a20: 6e20 3c73 696d 2069 643e 203c 7265 7065  n <sim id> <repe
-00001a30: 7469 7469 6f6e 733e 0a77 6865 7265 2060  titions>.where `
-00001a40: 3c73 696d 5f69 643e 6020 6973 2074 6865  <sim_id>` is the
-00001a50: 2069 6420 796f 7520 6a75 7374 2063 6f70   id you just cop
-00001a60: 6965 642c 2061 6e64 2060 3c72 6570 6574  ied, and `<repet
-00001a70: 6974 696f 6e73 3e60 2069 7320 6e75 6d62  itions>` is numb
-00001a80: 6572 206f 6620 7369 6d75 6c61 7469 6f6e  er of simulation
-00001a90: 2072 756e 7320 7468 6174 2077 696c 6c20   runs that will 
-00001aa0: 7275 6e2e 2045 7861 6d70 6c65 3a0a 2020  run. Example:.  
-00001ab0: 2020 0a20 2020 2063 6974 726f 7320 7275    .    citros ru
-00001ac0: 6e5f 7369 6d75 6c61 7469 6f6e 2063 6631  n_simulation cf1
-00001ad0: 6234 3636 332d 6136 6533 2d34 3962 642d  b4663-a6e3-49bd-
-00001ae0: 3936 6535 2d62 6334 3763 6235 6435 3332  96e5-bc47cb5d532
-00001af0: 3620 310a 2020 2020 2e2e 2e0a 2020 2020  6 1.    ....    
-00001b00: 2d20 2d20 4669 6e69 7368 6564 2073 696d  - - Finished sim
-00001b10: 756c 6174 696f 6e20 7369 6420 3d20 5b30  ulation sid = [0
-00001b20: 5d20 7769 7468 2072 6574 7572 6e20 636f  ] with return co
-00001b30: 6465 205b 315d 2e0a 2020 2020 2d20 4669  de [1]..    - Fi
-00001b40: 6e69 7368 6564 205b 6137 6231 3838 6464  nished [a7b188dd
-00001b50: 2d37 3462 622d 3464 6539 2d62 3338 362d  -74bb-4de9-b386-
-00001b60: 3961 3330 3438 3936 3532 6362 5d20 6261  9a30489652cb] ba
-00001b70: 7463 682e 0a0a 2323 2072 756e 0a52 756e  tch...## run.Run
-00001b80: 2061 2070 7265 7669 6f75 736c 7920 6372   a previously cr
-00001b90: 6561 7465 6420 6261 7463 6820 6c6f 6361  eated batch loca
-00001ba0: 6c6c 792e 2054 6869 7320 636f 6d6d 616e  lly. This comman
-00001bb0: 6420 6973 2075 7365 6675 6c20 7768 656e  d is useful when
-00001bc0: 2079 6f75 2764 206c 696b 6520 746f 206c   you'd like to l
-00001bd0: 6f63 616c 6c79 2072 6572 756e 2061 2062  ocally rerun a b
-00001be0: 6174 6368 2074 6861 7420 7761 7320 616c  atch that was al
-00001bf0: 7265 6164 7920 7275 6e20 2865 6974 6865  ready run (eithe
-00001c00: 7220 6c6f 6361 6c6c 7920 6f72 206f 6e20  r locally or on 
-00001c10: 7468 6520 636c 7573 7465 7229 2e0a 0a41  the cluster)...A
-00001c20: 6674 6572 2079 6f75 2776 6520 6c6f 6767  fter you've logg
-00001c30: 6564 2069 6e74 6f20 5b63 6974 726f 732e  ed into [citros.
-00001c40: 696f 5d28 6369 7472 6f73 2e69 6f29 2c20  io](citros.io), 
-00001c50: 636c 6963 6b20 7468 6520 6053 696d 756c  click the `Simul
-00001c60: 6174 696f 6e20 5275 6e73 6020 7461 623a  ation Runs` tab:
-00001c70: 0a21 5b73 696d 5f72 756e 735d 2869 6d67  .![sim_runs](img
-00001c80: 2f73 696d 5f72 756e 732e 706e 6720 2253  /sim_runs.png "S
-00001c90: 696d 756c 6174 696f 6e20 5275 6e73 2229  imulation Runs")
-00001ca0: 2020 0a0a 616e 6420 6f6e 2074 6865 206c    ..and on the l
-00001cb0: 6973 7420 6974 656d 2063 6f72 7265 7370  ist item corresp
-00001cc0: 6f6e 6469 6e67 2074 6f20 7468 6520 6261  onding to the ba
-00001cd0: 7463 6820 796f 7527 6420 6c69 6b65 2074  tch you'd like t
-00001ce0: 6f20 7275 6e2c 2063 6c69 636b 2074 6865  o run, click the
-00001cf0: 2074 6872 6565 2076 6572 7469 6361 6c20   three vertical 
-00001d00: 646f 7473 206f 6e20 7468 6520 7269 6768  dots on the righ
-00001d10: 7420 616e 6420 7468 656e 2063 6c69 636b  t and then click
-00001d20: 206e 6176 6967 6174 6520 6f6e 2074 6865   navigate on the
-00001d30: 2073 6d61 6c6c 2063 6f6e 7465 7874 206d   small context m
-00001d40: 656e 7520 7468 6174 206f 7065 6e73 2e20  enu that opens. 
-00001d50: 5468 6973 2077 696c 6c20 7461 6b65 2079  This will take y
-00001d60: 6f75 2074 6f20 7468 6520 6c69 7374 206f  ou to the list o
-00001d70: 6620 7369 6d75 6c61 7469 6f6e 2072 756e  f simulation run
-00001d80: 7320 666f 7220 7468 6520 6261 7463 6820  s for the batch 
-00001d90: 796f 7520 7365 6c65 6374 6564 3a0a 215b  you selected:.![
-00001da0: 6261 7463 685f 7275 6e73 5d28 696d 672f  batch_runs](img/
-00001db0: 6261 7463 685f 7275 6e73 2e70 6e67 2022  batch_runs.png "
-00001dc0: 4261 7463 6820 5275 6e73 2229 0a0a 756e  Batch Runs")..un
-00001dd0: 6465 7220 7468 6520 6053 696d 756c 6174  der the `Simulat
-00001de0: 696f 6e20 5275 6e73 6020 6865 6164 696e  ion Runs` headin
-00001df0: 672c 2079 6f75 2061 7265 2070 7265 7365  g, you are prese
-00001e00: 6e74 6564 2077 6974 6820 736f 6d65 206d  nted with some m
-00001e10: 6574 6164 6174 6120 666f 7220 7468 6973  etadata for this
-00001e20: 2062 6174 6368 2069 6e20 7468 6520 666f   batch in the fo
-00001e30: 6c6c 6f77 696e 6720 666f 726d 6174 3a0a  llowing format:.
-00001e40: 0a20 2020 2044 6173 6862 6f61 7264 202d  .    Dashboard -
-00001e50: 2050 726f 6a65 6374 4c69 7374 202d 203c   ProjectList - <
-00001e60: 7072 6f6a 6563 745f 6e61 6d65 3e20 2d20  project_name> - 
-00001e70: 3c73 696d 756c 6174 696f 6e5f 6964 3e20  <simulation_id> 
-00001e80: 2d20 3c62 6174 6368 5f69 643e 0a0a 636f  - <batch_id>..co
-00001e90: 7079 2074 6865 2074 6865 2062 6174 6368  py the the batch
-00001ea0: 2069 642c 2061 6e64 2069 6e20 7468 6520   id, and in the 
-00001eb0: 636f 6d6d 616e 642d 6c69 6e65 3a0a 0a20  command-line:.. 
-00001ec0: 2020 2063 6974 726f 7320 7275 6e20 3c62     citros run <b
-00001ed0: 6174 6368 5f69 643e 203c 7369 6d5f 7275  atch_id> <sim_ru
-00001ee0: 6e5f 6964 3e0a 0a77 6865 7265 2060 3c73  n_id>..where `<s
-00001ef0: 696d 5f72 756e 5f69 643e 6020 6973 2074  im_run_id>` is t
-00001f00: 6865 2028 7a65 726f 2d62 6173 6564 2920  he (zero-based) 
-00001f10: 7275 6e20 696e 6465 7820 286e 6f74 2074  run index (not t
-00001f20: 6f20 6265 2063 6f6e 6675 7365 6420 7769  o be confused wi
-00001f30: 7468 2060 7369 6d75 6c61 7469 6f6e 5f69  th `simulation_i
-00001f40: 6460 292e 2049 6620 6974 2069 7320 6e6f  d`). If it is no
-00001f50: 7420 7370 6563 6966 6965 642c 2074 6865  t specified, the
-00001f60: 2065 6e74 6972 6520 6261 7463 6820 6973   entire batch is
-00001f70: 2065 7865 6375 7465 642e 2045 7861 6d70   executed. Examp
-00001f80: 6c65 3a0a 0a20 2020 2063 6974 726f 7320  le:..    citros 
-00001f90: 7275 6e20 6264 3137 3561 3933 2d34 3233  run bd175a93-423
-00001fa0: 342d 3432 3434 2d39 3432 642d 3062 3261  4-4244-942d-0b2a
-00001fb0: 3938 3263 3436 3566 2030 0a0a 2323 2075  982c465f 0..## u
-00001fc0: 706c 6f61 645f 6261 670a 6578 7065 7269  pload_bag.experi
-00001fd0: 6d65 6e74 616c 2e0a 0a75 706c 6f61 6420  mental...upload 
-00001fe0: 6261 6720 746f 2063 6974 726f 732e 0a23  bag to citros..#
-00001ff0: 2320 7374 7265 7373 0a65 7870 6572 696d  # stress.experim
-00002000: 656e 7461 6c2e 0a0a 7374 7265 7373 2074  ental...stress t
-00002010: 6573 7420 7468 6520 7379 7374 656d 2e0a  est the system..
-00002020: 2323 2064 6f63 6b65 722d 6c6f 6769 6e0a  ## docker-login.
-00002030: 6c6f 6769 6e20 746f 2064 6f63 6b65 722d  login to docker-
-00002040: 6875 620a 2323 2064 6f63 6b65 720a 4275  hub.## docker.Bu
-00002050: 696c 6473 2074 6865 2070 726f 6a65 6374  ilds the project
-00002060: 2e0a                                     ..
+00000000: 6060 6070 7974 686f 6e0a 2320 3d3d 3d3d  ```python.# ====
+00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 0a23 2020 20e2  ==========.#   .
+00000040: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+00000050: 88e2 9597 e296 88e2 9688 e295 97e2 9688  ................
+00000060: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000070: 9688 e296 88e2 9597 e296 88e2 9688 e296  ................
+00000080: 88e2 9688 e296 88e2 9688 e295 9720 20e2  .............  .
+00000090: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+000000a0: 88e2 9597 20e2 9688 e296 88e2 9688 e296  .... ...........
+000000b0: 88e2 9688 e296 88e2 9688 e295 970a 2320  ..............# 
+000000c0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
+000000d0: e295 90e2 9590 e295 9de2 9688 e296 88e2  ................
+000000e0: 9591 e295 9ae2 9590 e295 90e2 9688 e296  ................
+000000f0: 88e2 9594 e295 90e2 9590 e295 9de2 9688  ................
+00000100: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
+00000110: 9688 e295 97e2 9688 e296 88e2 9594 e295  ................
+00000120: 90e2 9590 e295 90e2 9688 e296 88e2 9597  ................
+00000130: e296 88e2 9688 e295 94e2 9590 e295 90e2  ................
+00000140: 9590 e295 90e2 959d 0a23 2020 e296 88e2  .........#  ....
+00000150: 9688 e295 9120 2020 2020 e296 88e2 9688  .....     ......
+00000160: e295 9120 2020 e296 88e2 9688 e295 9120  ...   ......... 
+00000170: 2020 e296 88e2 9688 e296 88e2 9688 e296    ..............
+00000180: 88e2 9688 e295 94e2 959d e296 88e2 9688  ................
+00000190: e295 9120 2020 e296 88e2 9688 e295 91e2  ...   ..........
+000001a0: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+000001b0: 88e2 9688 e295 970a 2320 20e2 9688 e296  ........#  .....
+000001c0: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
+000001d0: 9591 2020 20e2 9688 e296 88e2 9591 2020  ..   .........  
+000001e0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
+000001f0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
+00000200: 9591 2020 20e2 9688 e296 88e2 9591 e295  ..   ...........
+00000210: 9ae2 9590 e295 90e2 9590 e295 90e2 9688  ................
+00000220: e296 88e2 9591 0a23 2020 e295 9ae2 9688  .......#  ......
+00000230: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000240: 9597 e296 88e2 9688 e295 9120 2020 e296  ...........   ..
+00000250: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
+00000260: e295 9120 20e2 9688 e296 88e2 9591 e295  ...  ...........
+00000270: 9ae2 9688 e296 88e2 9688 e296 88e2 9688  ................
+00000280: e296 88e2 9594 e295 9de2 9688 e296 88e2  ................
+00000290: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
+000002a0: 910a 2320 2020 e295 9ae2 9590 e295 90e2  ..#   ..........
+000002b0: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
+000002c0: 90e2 959d 2020 20e2 959a e295 90e2 959d  ....   .........
+000002d0: 2020 20e2 959a e295 90e2 959d 2020 e295     .........  ..
+000002e0: 9ae2 9590 e295 9d20 e295 9ae2 9590 e295  ....... ........
+000002f0: 90e2 9590 e295 90e2 9590 e295 9d20 e295  ............. ..
+00000300: 9ae2 9590 e295 90e2 9590 e295 90e2 9590  ................
+00000310: e295 90e2 959d 2020 2020 2020 2020 2020  ......          
+00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000330: 2020 2020 2020 2020 2020 2020 2020 0a23                .#
+00000340: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
+00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
+00000370: 6060 600a 2320 4349 5452 4f53 2043 4c49  ```.# CITROS CLI
+00000380: 0a0a 5b21 5b50 7562 6c69 7368 2043 4954  ..[![Publish CIT
+00000390: 524f 535f 434c 4920 746f 2050 7950 4920  ROS_CLI to PyPI 
+000003a0: 2f20 4769 7448 7562 5d28 6874 7470 733a  / GitHub](https:
+000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 756c  //github.com/lul
+000003c0: 6176 2f63 6974 726f 735f 636c 692f 6163  av/citros_cli/ac
+000003d0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
+000003e0: 7265 6c65 6173 655f 746f 5f70 7970 692e  release_to_pypi.
+000003f0: 7961 6d6c 2f62 6164 6765 2e73 7667 295d  yaml/badge.svg)]
+00000400: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00000410: 636f 6d2f 6c75 6c61 762f 6369 7472 6f73  com/lulav/citros
+00000420: 5f63 6c69 2f61 6374 696f 6e73 2f77 6f72  _cli/actions/wor
+00000430: 6b66 6c6f 7773 2f72 656c 6561 7365 5f74  kflows/release_t
+00000440: 6f5f 7079 7069 2e79 616d 6c29 0a0a 2320  o_pypi.yaml)..# 
+00000450: 4465 7363 7269 7074 696f 6e0a 0a54 6869  Description..Thi
+00000460: 7320 7265 706f 7369 746f 7279 2069 7320  s repository is 
+00000470: 6120 7079 7468 6f6e 2070 6163 6b61 6765  a python package
+00000480: 2074 6861 7420 696d 706c 656d 656e 7473   that implements
+00000490: 2074 6865 2043 4954 524f 5320 434c 4920   the CITROS CLI 
+000004a0: 4150 492e 0a49 7420 6973 2072 756e 2062  API..It is run b
+000004b0: 7920 7468 6520 7573 6572 2069 6e73 6964  y the user insid
+000004c0: 6520 7468 6520 524f 5320 7072 6f6a 6563  e the ROS projec
+000004d0: 7420 666f 6c64 6572 2e20 0a0a 2320 5072  t folder. ..# Pr
+000004e0: 6572 6571 7569 7369 7465 730a 0a2d 205b  erequisites..- [
+000004f0: 7673 636f 6465 5d28 6874 7470 733a 2f2f  vscode](https://
+00000500: 636f 6465 2e76 6973 7561 6c73 7475 6469  code.visualstudi
+00000510: 6f2e 636f 6d2f 646f 776e 6c6f 6164 290a  o.com/download).
+00000520: 2d20 5b44 6f63 6b65 725d 2868 7474 7073  - [Docker](https
+00000530: 3a2f 2f77 7777 2e64 6f63 6b65 722e 636f  ://www.docker.co
+00000540: 6d2f 290a 2d20 5b50 7974 686f 6e33 5d28  m/).- [Python3](
+00000550: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
+00000560: 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61 6473  on.org/downloads
+00000570: 2f29 0a0a 2320 496e 7374 616c 6c61 7469  /)..# Installati
+00000580: 6f6e 0a0a 312e 2063 6c6f 6e65 2074 6865  on..1. clone the
+00000590: 2072 6570 6f3a 0a20 2020 200a 2020 2020   repo:.    .    
+000005a0: 2020 2020 6769 7420 636c 6f6e 6520 6769      git clone gi
+000005b0: 7440 6769 7468 7562 2e63 6f6d 3a6c 756c  t@github.com:lul
+000005c0: 6176 2f63 6974 726f 735f 636c 692e 6769  av/citros_cli.gi
+000005d0: 740a 0a32 2e20 5769 7468 696e 2074 6865  t..2. Within the
+000005e0: 2063 6c6f 6e65 6420 6063 6974 726f 735f   cloned `citros_
+000005f0: 636c 6960 2066 6f6c 6465 722c 206f 7065  cli` folder, ope
+00000600: 6e20 5653 436f 6465 3a0a 2020 2020 0a20  n VSCode:.    . 
+00000610: 2020 2020 2020 2063 6f64 6520 2e0a 0a20         code ... 
+00000620: 2020 2061 6e64 2072 656f 7065 6e20 7468     and reopen th
+00000630: 6520 666f 6c64 6572 2069 6e73 6964 6520  e folder inside 
+00000640: 6120 4465 7620 436f 6e74 6169 6e65 722e  a Dev Container.
+00000650: 0a0a 332e 2049 6e73 7461 6c6c 2074 6865  ..3. Install the
+00000660: 2070 6163 6b61 6765 2066 726f 6d20 7468   package from th
+00000670: 6520 6375 7272 656e 7420 6469 7265 6374  e current direct
+00000680: 6f72 792c 2077 6974 6820 736f 6674 206c  ory, with soft l
+00000690: 696e 6b73 2074 6f20 6465 7620 656e 7669  inks to dev envi
+000006a0: 726f 6e6d 656e 7420 0a0a 2020 2020 2020  ronment ..      
+000006b0: 2020 7079 7468 6f6e 3320 2d6d 2070 6970    python3 -m pip
+000006c0: 2069 6e73 7461 6c6c 202d 6520 2e0a 0a20   install -e ... 
+000006d0: 2020 2028 7265 636f 6d6d 656e 6465 6420     (recommended 
+000006e0: 6475 7269 6e67 2064 6576 656c 6f70 6d65  during developme
+000006f0: 6e74 292c 0a0a 2020 2020 6f72 200a 0a20  nt),..    or .. 
+00000700: 2020 2049 6e73 7461 6c6c 2074 6865 2070     Install the p
+00000710: 6163 6b61 6765 2066 726f 6d20 7468 6520  ackage from the 
+00000720: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
+00000730: 792c 2064 6972 6563 746c 7920 746f 2061  y, directly to a
+00000740: 2067 6c6f 6261 6c20 6269 6e20 666f 6c64   global bin fold
+00000750: 6572 200a 0a20 2020 2020 2020 2070 7974  er ..        pyt
+00000760: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
+00000770: 616c 6c20 2e0a 2020 2020 0a20 2020 2028  all ..    .    (
+00000780: 7368 6f75 6c64 2062 6520 646f 6e65 2062  should be done b
+00000790: 6566 6f72 6520 7570 6c6f 6164 696e 6720  efore uploading 
+000007a0: 746f 2050 7950 492c 2074 6f20 6d61 6b65  to PyPI, to make
+000007b0: 2073 7572 6520 7468 6520 696e 7374 616c   sure the instal
+000007c0: 6c61 7469 6f6e 2069 7320 776f 726b 696e  lation is workin
+000007d0: 6720 7072 6f70 6572 6c79 292e 0a0a 342e  g properly)...4.
+000007e0: 2045 6e76 0a0a 7c20 454e 5620 7c20 4465   Env..| ENV | De
+000007f0: 7363 7269 7074 696f 6e20 7c20 7573 6564  scription | used
+00000800: 2069 6e20 7c0a 7c20 2d2d 2d20 7c20 2d2d   in |.| --- | --
+00000810: 2d20 7c20 2d2d 2d20 7c0a 7c20 6043 4954  - | --- |.| `CIT
+00000820: 524f 535f 444f 4d41 494e 6020 7c20 7468  ROS_DOMAIN` | th
+00000830: 6520 6d61 696e 2064 6f6d 6169 6e2c 2064  e main domain, d
+00000840: 6566 6175 6c74 2069 7320 6063 6974 726f  efault is `citro
+00000850: 732e 696f 6020 7c20 616c 6c20 7061 636b  s.io` | all pack
+00000860: 6167 6573 207c 0a7c 2060 4349 5452 4f53  ages |.| `CITROS
+00000870: 5f44 4154 415f 484f 5354 6020 7c20 686f  _DATA_HOST` | ho
+00000880: 7374 206f 6620 7468 6520 706c 6179 6772  st of the playgr
+00000890: 6f75 6e64 2050 4744 422c 2064 6566 6175  ound PGDB, defau
+000008a0: 6c74 2063 6f6d 6573 2066 726f 6d20 7369  lt comes from si
+000008b0: 6d75 6c61 7469 6f6e 206a 6f62 2065 6e76  mulation job env
+000008c0: 2028 6369 7472 6f73 5f77 6f72 6b65 7229   (citros_worker)
+000008d0: 2061 6e64 2069 733a 2060 7368 6172 6564   and is: `shared
+000008e0: 2d70 6c61 7967 726f 756e 642d 706f 7374  -playground-post
+000008f0: 6772 6573 716c 2e6e 732d 6369 7472 6f73  gresql.ns-citros
+00000900: 2d73 6861 7265 6460 2e20 7573 6564 2066  -shared`. used f
+00000910: 6f72 2075 706c 6f61 6469 6e67 2042 4147  or uploading BAG
+00000920: 2e20 7c20 6369 7472 6f73 5f62 6167 207c  . | citros_bag |
+00000930: 0a7c 2060 4349 5452 4f53 5f44 4154 415f  .| `CITROS_DATA_
+00000940: 504f 5254 6020 7c20 7468 6520 706f 7274  PORT` | the port
+00000950: 206f 6620 5047 4442 2c20 6465 6661 756c   of PGDB, defaul
+00000960: 7420 6035 3433 3260 207c 2063 6974 726f  t `5432` | citro
+00000970: 735f 6261 6720 7c0a 7c20 6043 4954 524f  s_bag |.| `CITRO
+00000980: 535f 4441 5441 5f44 4154 4142 4153 4560  S_DATA_DATABASE`
+00000990: 207c 2074 6865 2064 6174 6162 6173 6520   | the database 
+000009a0: 746f 2061 6363 6573 7320 696e 7369 6465  to access inside
+000009b0: 2050 4744 422e 2064 6566 6175 6c74 2063   PGDB. default c
+000009c0: 6f6d 6573 2066 726f 6d20 7369 6d75 6c61  omes from simula
+000009d0: 7469 6f6e 206a 6f62 2065 6e76 2028 6369  tion job env (ci
+000009e0: 7472 6f73 5f77 6f72 6b65 7229 2061 6e64  tros_worker) and
+000009f0: 2069 733a 2060 646f 6d61 696e 5f70 7265   is: `domain_pre
+00000a00: 6669 7860 2e20 7573 6564 2066 6f72 2075  fix`. used for u
+00000a10: 706c 6f61 6469 6e67 2042 4147 2e20 7c20  ploading BAG. | 
+00000a20: 6369 7472 6f73 5f62 6167 207c 0a7c 2060  citros_bag |.| `
+00000a30: 4349 5452 4f53 5f44 4154 415f 5553 4552  CITROS_DATA_USER
+00000a40: 4e41 4d45 6020 7c20 7468 6520 7573 6572  NAME` | the user
+00000a50: 6e61 6d65 2074 6f20 6163 6365 7373 2050  name to access P
+00000a60: 4744 422c 2064 6566 6175 6c74 2060 6369  GDB, default `ci
+00000a70: 7472 6f73 5f61 6e6f 6e79 6d6f 7573 602e  tros_anonymous`.
+00000a80: 2074 6865 2075 7365 726e 616d 6520 6973   the username is
+00000a90: 2074 6865 2075 7365 726e 616d 6520 6672   the username fr
+00000aa0: 6f6d 2063 6974 726f 732e 2020 7c20 6369  om citros.  | ci
+00000ab0: 7472 6f73 5f62 6167 207c 0a7c 2060 4349  tros_bag |.| `CI
+00000ac0: 5452 4f53 5f44 4154 415f 5041 5353 574f  TROS_DATA_PASSWO
+00000ad0: 5244 6020 7c20 7468 6520 7061 7373 776f  RD` | the passwo
+00000ae0: 7264 2074 6f20 6163 6365 7373 2050 4744  rd to access PGD
+00000af0: 422c 2064 6566 6175 6c74 2060 6369 7472  B, default `citr
+00000b00: 6f73 5f61 6e6f 6e79 6d6f 7573 602e 2074  os_anonymous`. t
+00000b10: 6865 2070 6173 7377 6f72 6420 6973 2074  he password is t
+00000b20: 6865 2069 6420 6f66 2074 6865 2075 7365  he id of the use
+00000b30: 7220 696e 2060 6369 7472 6f73 2e75 7365  r in `citros.use
+00000b40: 7260 2074 6162 6c65 2e20 207c 2063 6974  r` table.  | cit
+00000b50: 726f 735f 6261 6720 7c0a 0a23 2043 4c49  ros_bag |..# CLI
+00000b60: 2041 5049 2063 6f6d 6d61 6e64 733a 0a0a   API commands:..
+00000b70: 2323 206c 6f67 696e 0a4c 6f67 696e 2074  ## login.Login t
+00000b80: 6f20 4349 5452 4f53 2e0a 0a41 6674 6572  o CITROS...After
+00000b90: 2065 6e74 6572 696e 6720 7468 6520 636f   entering the co
+00000ba0: 6d6d 616e 642c 2079 6f75 2077 696c 6c20  mmand, you will 
+00000bb0: 6265 2070 726f 6d70 7465 6420 666f 7220  be prompted for 
+00000bc0: 796f 7572 2065 6d61 696c 2028 7468 6520  your email (the 
+00000bd0: 7573 6572 6e61 6d65 2920 616e 6420 7061  username) and pa
+00000be0: 7373 776f 7264 2e0a 0a65 7861 6d70 6c65  ssword...example
+00000bf0: 3a0a 0a20 2020 2072 6f73 4073 6861 6c65  :..    ros@shale
+00000c00: 762d 496e 7370 6972 6f6e 2d31 352d 3535  v-Inspiron-15-55
+00000c10: 3130 3a2f 776f 726b 7370 6163 6573 2f63  10:/workspaces/c
+00000c20: 616e 6e6f 6e24 2063 6974 726f 7320 6c6f  annon$ citros lo
+00000c30: 6769 6e0a 2020 2020 656d 6169 6c3a 2073  gin.    email: s
+00000c40: 6861 6c65 7640 6c75 6c61 762e 7370 6163  halev@lulav.spac
+00000c50: 650a 2020 2020 5061 7373 776f 7264 3a20  e.    Password: 
+00000c60: 0a20 2020 2055 7365 7220 6c6f 6767 6564  .    User logged
+00000c70: 2069 6e2e 0a20 2020 205b 3230 3233 2d30   in..    [2023-0
+00000c80: 352d 3131 2030 383a 3132 3a31 382c 3036  5-11 08:12:18,06
+00000c90: 355d 205b 6369 7472 6f73 2e63 6974 726f  5] [citros.citro
+00000ca0: 732d 4e6f 6e65 2d4e 6f6e 652e 6c6f 6769  s-None-None.logi
+00000cb0: 6e3a 3236 385d 205b 494e 464f 5d3a 2041  n:268] [INFO]: A
+00000cc0: 7574 6865 6e74 6963 6174 6564 210a 0a23  uthenticated!..#
+00000cd0: 2320 6175 7468 656e 7469 6361 7465 0a41  # authenticate.A
+00000ce0: 7574 6865 6e74 6963 6174 6520 796f 7572  uthenticate your
+00000cf0: 7365 6c66 2074 6f20 4349 5452 4f53 2077  self to CITROS w
+00000d00: 6865 6e20 6120 6c6f 6769 6e20 6973 206e  hen a login is n
+00000d10: 6f74 2070 6f73 7369 626c 652c 2065 2e67  ot possible, e.g
+00000d20: 2e20 7768 656e 2072 756e 6e69 6e67 2069  . when running i
+00000d30: 6e20 7468 6520 636c 6f75 6420 6f72 2070  n the cloud or p
+00000d40: 6572 666f 726d 696e 6720 6175 746f 6d61  erforming automa
+00000d50: 7465 6420 7465 7374 732e 0a0a 4669 7273  ted tests...Firs
+00000d60: 742c 2069 6e20 6f72 6465 7220 746f 206f  t, in order to o
+00000d70: 6274 6169 6e20 6120 7661 6c69 6420 6175  btain a valid au
+00000d80: 7468 656e 7469 6361 7469 6f6e 206b 6579  thentication key
+00000d90: 2c20 6c6f 6769 6e20 746f 205b 6369 7472  , login to [citr
+00000da0: 6f73 5d28 6874 7470 3a2f 2f63 6974 726f  os](http://citro
+00000db0: 732e 696f 2f29 2061 6e64 2063 6c69 636b  s.io/) and click
+00000dc0: 2074 6865 2060 4164 6420 5072 6f6a 6563   the `Add Projec
+00000dd0: 7460 2062 7574 746f 6e20 696e 2074 6865  t` button in the
+00000de0: 2074 6f70 2072 6967 6874 2063 6f72 6e65   top right corne
+00000df0: 723a 0a21 5b61 6464 5f70 726f 6a5d 2869  r:.![add_proj](i
+00000e00: 6d67 2f61 6464 5f70 726f 6a2e 706e 6720  mg/add_proj.png 
+00000e10: 2261 6464 2070 726f 6a65 6374 2229 0a0a  "add project")..
+00000e20: 436f 7079 2074 6865 206c 696e 6520 6063  Copy the line `c
+00000e30: 6974 726f 7320 6175 7468 656e 7469 6361  itros authentica
+00000e40: 7465 203c 796f 7572 206b 6579 3e60 3a0a  te <your key>`:.
+00000e50: 215b 6175 7468 5f6b 6579 5d28 696d 672f  ![auth_key](img/
+00000e60: 6175 7468 5f6b 6579 2e70 6e67 2022 6175  auth_key.png "au
+00000e70: 7468 656e 7469 6361 7469 6f6e 206b 6579  thentication key
+00000e80: 2229 0a0a 2061 6e64 2070 6173 7465 2069  ").. and paste i
+00000e90: 7420 696e 2074 6865 2063 6f6d 6d61 6e64  t in the command
+00000ea0: 206c 696e 652e 0a0a 6578 616d 706c 653a   line...example:
+00000eb0: 0a0a 2020 2020 726f 7340 7368 616c 6576  ..    ros@shalev
+00000ec0: 2d49 6e73 7069 726f 6e2d 3135 2d35 3531  -Inspiron-15-551
+00000ed0: 303a 2f77 6f72 6b73 7061 6365 732f 6361  0:/workspaces/ca
+00000ee0: 6e6e 6f6e 2420 6369 7472 6f73 2061 7574  nnon$ citros aut
+00000ef0: 6865 6e74 6963 6174 6520 6579 4a68 6247  henticate eyJhbG
+00000f00: 6369 4f69 4a49 557a 4931 4e69 4973 496e  ciOiJIUzI1NiIsIn
+00000f10: 5235 6343 4936 496b 7058 5643 4a39 2e65  R5cCI6IkpXVCJ9.e
+00000f20: 794a 7962 3278 6c49 6a6f 6959 326c 3063  yJyb2xlIjoiY2l0c
+00000f30: 6d39 7a58 3246 6b62 576c 7549 6977 6964  m9zX2FkbWluIiwid
+00000f40: 584e 6c63 6c39 705a 4349 3649 6a45 354e  XNlcl9pZCI6IjE5N
+00000f50: 7a68 6a4f 4455 344c 5452 6a59 6d45 744e  zhjODU4LTRjYmEtN
+00000f60: 4459 794e 5330 344e 6a64 6c4c 5455 774d  DYyNS04NjdlLTUwM
+00000f70: 6a4d 325a 6d52 6a4e 6d51 354d 5349 7349  jM2ZmRjNmQ5MSIsI
+00000f80: 6e56 7a5a 584a 6662 6d46 745a 5349 3649  nVzZXJfbmFtZSI6I
+00000f90: 6e4e 6f59 5778 6c64 6949 7349 6d4e 7064  nNoYWxldiIsImNpd
+00000fa0: 484a 7663 3139 7962 3278 6c49 6a6f 6964  HJvc19yb2xlIjoid
+00000fb0: 584e 6c63 6949 7349 6d39 795a 3246 7561  XNlciIsIm9yZ2Fua
+00000fc0: 5870 6864 476c 7662 6c39 705a 4349 3649  XphdGlvbl9pZCI6I
+00000fd0: 6d55 354d 5456 6b4e 6a4d 354c 5459 7a4e  mU5MTVkNjM5LTYzN
+00000fe0: 7a49 744e 4456 6c4e 4330 344e 5456 6b4c  zItNDVlNC04NTVkL
+00000ff0: 5745 3459 7a6c 694e 3251 3259 5749 774d  WE4YzliN2Q2YWIwM
+00001000: 6949 7349 6d39 795a 3246 7561 5870 6864  iIsIm9yZ2FuaXphd
+00001010: 476c 7662 6c39 3065 5842 6c49 6a6f 6954  Glvbl90eXBlIjoiT
+00001020: 5546 4f51 5564 4649 6977 695a 4739 7459  UFOQUdFIiwiZG9tY
+00001030: 576c 7558 3342 795a 575a 7065 4349 3649  WluX3ByZWZpeCI6I
+00001040: 6d78 3162 4746 3249 6977 695a 5868 7749  mx1bGF2IiwiZXhwI
+00001050: 6a6f 784e 6a67 7a4e 7a41 314f 5455 7a4c  joxNjgzNzA1OTUzL
+00001060: 434a 7059 5851 694f 6a45 324f 444d 324d  CJpYXQiOjE2ODM2M
+00001070: 546b 314e 544d 7349 6d46 315a 4349 3649  Tk1NTMsImF1ZCI6I
+00001080: 6e42 7663 3352 6e63 6d46 7761 476c 735a  nBvc3RncmFwaGlsZ
+00001090: 5349 7349 6d6c 7a63 7949 3649 6e42 7663  SIsImlzcyI6InBvc
+000010a0: 3352 6e63 6d46 7761 476c 735a 534a 392e  3RncmFwaGlsZSJ9.
+000010b0: 684b 6778 3259 6c44 4d68 4832 3370 4743  hKgx2YlDMhH23pGC
+000010c0: 5a47 6833 5971 6161 5833 7754 696b 6a42  ZGh3YqaaX3wTikjB
+000010d0: 4279 7049 725f 644d 3874 670a 2020 2020  BypIr_dM8tg.    
+000010e0: 4175 7468 656e 7469 6361 7465 6421 0a20  Authenticated!. 
+000010f0: 2020 205b 3230 3233 2d30 352d 3131 2030     [2023-05-11 0
+00001100: 383a 3537 3a31 312c 3030 305d 205b 6369  8:57:11,000] [ci
+00001110: 7472 6f73 2e63 6974 726f 732d 4e6f 6e65  tros.citros-None
+00001120: 2d4e 6f6e 652e 6175 7468 656e 7469 6361  -None.authentica
+00001130: 7465 5f77 6974 685f 6b65 793a 3231 395d  te_with_key:219]
+00001140: 205b 494e 464f 5d3a 2041 7574 6865 6e74   [INFO]: Authent
+00001150: 6963 6174 6564 210a 4e6f 7465 3a20 7468  icated!.Note: th
+00001160: 6520 6b65 7920 6973 2076 616c 6964 2066  e key is valid f
+00001170: 6f72 2074 776f 2064 6179 732c 2061 6674  or two days, aft
+00001180: 6572 2077 6869 6368 2061 206e 6577 206b  er which a new k
+00001190: 6579 206e 6565 6473 2074 6f20 6265 2067  ey needs to be g
+000011a0: 656e 6572 6174 6564 2e20 200a 0a23 2320  enerated.  ..## 
+000011b0: 6c6f 676f 7574 0a4c 6f67 6f75 7420 6f66  logout.Logout of
+000011c0: 2043 4954 524f 532e 0a0a 6578 616d 706c   CITROS...exampl
+000011d0: 653a 0a0a 2020 2020 726f 7340 7368 616c  e:..    ros@shal
+000011e0: 6576 2d49 6e73 7069 726f 6e2d 3135 2d35  ev-Inspiron-15-5
+000011f0: 3531 303a 2f77 6f72 6b73 7061 6365 732f  510:/workspaces/
+00001200: 6361 6e6e 6f6e 2420 6369 7472 6f73 206c  cannon$ citros l
+00001210: 6f67 6f75 740a 2020 2020 5573 6572 206c  ogout.    User l
+00001220: 6f67 6765 6420 6f75 742e 0a23 2320 7379  ogged out..## sy
+00001230: 6e63 0a53 796e 6320 7468 6520 726f 7320  nc.Sync the ros 
+00001240: 7072 6f6a 6563 7420 746f 2063 6974 726f  project to citro
+00001250: 732e 0a0a 5468 6973 2063 6f6d 6d61 6e64  s...This command
+00001260: 2077 696c 6c20 7061 7273 6520 796f 7572   will parse your
+00001270: 2052 4f53 3220 7072 6f6a 6563 742c 2065   ROS2 project, e
+00001280: 7874 7261 6374 2074 6865 206e 616d 6573  xtract the names
+00001290: 206f 6620 616c 6c20 7468 6520 7061 636b   of all the pack
+000012a0: 6167 6573 2c20 0a6e 6f64 6573 2c20 7061  ages, .nodes, pa
+000012b0: 7261 6d65 7465 7273 2061 6e64 206c 6175  rameters and lau
+000012c0: 6e63 6820 6669 6c65 7320 2861 6e64 2073  nch files (and s
+000012d0: 6f6d 6520 6f74 6865 7220 6d65 7461 6461  ome other metada
+000012e0: 7461 292c 200a 6173 7369 676e 2065 6163  ta), .assign eac
+000012f0: 6820 6f66 2074 6865 6d20 6120 5549 4420  h of them a UID 
+00001300: 616e 6420 7570 6c6f 6164 2074 6865 6d20  and upload them 
+00001310: 746f 2074 6865 2063 6974 726f 7320 6461  to the citros da
+00001320: 7461 6261 7365 2e0a 0a65 7861 6d70 6c65  tabase...example
+00001330: 3a0a 2020 2020 0a20 2020 2072 6f73 4073  :.    .    ros@s
+00001340: 6861 6c65 762d 496e 7370 6972 6f6e 2d31  halev-Inspiron-1
+00001350: 352d 3535 3130 3a2f 776f 726b 7370 6163  5-5510:/workspac
+00001360: 6573 2f6d 6173 735f 7370 7269 6e67 5f64  es/mass_spring_d
+00001370: 756d 7065 7224 2063 6974 726f 7320 7379  umper$ citros sy
+00001380: 6e63 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  nc.    ---------
+00001390: 2d2d 2d2d 2d2d 2d2d 2d2d 7379 6e63 5f70  ----------sync_p
+000013a0: 726f 6a65 6374 2d2d 2d2d 2d2d 2d2d 2d2d  roject----------
+000013b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e  ---------.    ..
+000013c0: 2e0a 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d  ..    ----------
+000013d0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 444f 4e45  ------------DONE
+000013e0: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+000013f0: 2d2d 2d2d 2d2d 2d2d 0a0a 4966 2074 6865  --------..If the
+00001400: 7265 2077 6572 6520 6e6f 2063 6861 6e67  re were no chang
+00001410: 6573 2073 696e 6365 2074 6865 206c 6173  es since the las
+00001420: 7420 7379 6e63 2c20 7468 6520 7379 6e63  t sync, the sync
+00001430: 2069 7320 756e 6e65 6365 7373 6172 793a   is unnecessary:
+00001440: 0a0a 2020 2020 726f 7340 7368 616c 6576  ..    ros@shalev
+00001450: 2d49 6e73 7069 726f 6e2d 3135 2d35 3531  -Inspiron-15-551
+00001460: 303a 2f77 6f72 6b73 7061 6365 732f 6d61  0:/workspaces/ma
+00001470: 7373 5f73 7072 696e 675f 6475 6d70 6572  ss_spring_dumper
+00001480: 2420 6369 7472 6f73 2073 796e 630a 2020  $ citros sync.  
+00001490: 2020 7072 6f6a 6563 7420 616c 7265 6164    project alread
+000014a0: 7920 7379 6e63 6865 642e 0a0a 4966 2074  y synched...If t
+000014b0: 6869 7320 7761 7320 796f 7572 2066 6972  his was your fir
+000014c0: 7374 2074 696d 6520 7275 6e6e 696e 6720  st time running 
+000014d0: 7379 6e63 206f 6e20 7468 6973 2070 726f  sync on this pro
+000014e0: 6a65 6374 2c20 796f 7520 6361 6e20 6f70  ject, you can op
+000014f0: 656e 2079 6f75 7220 6661 766f 7269 7465  en your favorite
+00001500: 2062 726f 7773 6572 2061 6e64 206e 6176   browser and nav
+00001510: 6967 6174 6520 746f 205b 6369 7472 6f73  igate to [citros
+00001520: 2e69 6f5d 2863 6974 726f 732e 696f 2920  .io](citros.io) 
+00001530: 616e 6420 6c6f 6720 696e 2c20 616e 6420  and log in, and 
+00001540: 756e 6465 7220 7468 6520 7072 6f6a 6563  under the projec
+00001550: 7420 6c69 7374 2079 6f75 276c 6c20 7365  t list you'll se
+00001560: 6520 6120 6e65 7720 6974 656d 2066 6f72  e a new item for
+00001570: 2079 6f75 7220 7072 6f6a 6563 7420 6861   your project ha
+00001580: 7320 6265 656e 2061 6464 6564 2074 6f20  s been added to 
+00001590: 7468 6520 6c69 7374 3a0a 215b 7072 6f6a  the list:.![proj
+000015a0: 6563 7420 6c69 7374 5d28 696d 672f 7072  ect list](img/pr
+000015b0: 6f6a 5f6c 6973 742e 706e 6720 2270 726f  oj_list.png "pro
+000015c0: 6a65 6374 206c 6973 7422 290a 0a0a 2323  ject list")...##
+000015d0: 2320 7061 7261 6d65 7465 7273 3a0a 7061  # parameters:.pa
+000015e0: 7261 6d65 7465 727c 6465 7363 7269 7074  rameter|descript
+000015f0: 696f 6e0a 7c2d 2d7c 2d2d 7c0a 7c60 2d64  ion.|--|--|.|`-d
+00001600: 6972 6020 3c66 6f6c 6465 725f 6e61 6d65  ir` <folder_name
+00001610: 3e20 7c20 5468 6520 776f 726b 696e 6720  > | The working 
+00001620: 6469 7265 6374 6f72 7920 6f66 2074 6865  directory of the
+00001630: 2070 726f 6a65 6374 2e20 4465 6661 756c   project. Defaul
+00001640: 7473 2074 6f20 222e 222e 7c0a 7c60 2d6e  ts to ".".|.|`-n
+00001650: 616d 6560 203c 7072 6f6a 5f6e 616d 653e  ame` <proj_name>
+00001660: 207c 2054 6865 206e 616d 6520 6f66 2074   | The name of t
+00001670: 6865 2070 726f 6a65 6374 2e20 4465 6661  he project. Defa
+00001680: 756c 7473 2074 6f20 7468 6520 6c61 7374  ults to the last
+00001690: 2066 6f6c 6465 7220 696e 2074 6865 2070   folder in the p
+000016a0: 6174 6820 6f66 202a 6469 722a 7c0a 7c60  ath of *dir*|.|`
+000016b0: 2d77 602c 2060 2d77 7360 203c 776f 726b  -w`, `-ws` <work
+000016c0: 7370 6163 655f 6e61 6d65 3e20 7c20 5468  space_name> | Th
+000016d0: 6520 6e61 6d65 206f 6620 6120 776f 726b  e name of a work
+000016e0: 7370 6163 6520 696e 7369 6465 2074 6865  space inside the
+000016f0: 2070 726f 6a65 6374 2064 6972 6563 746f   project directo
+00001700: 7279 2e20 4d61 7920 6265 2075 7365 6420  ry. May be used 
+00001710: 6d75 6c74 6970 6c65 2074 696d 6573 2066  multiple times f
+00001720: 6f72 206d 756c 7469 706c 6520 776f 726b  or multiple work
+00001730: 7370 6163 6573 2e20 4465 6661 756c 7473  spaces. Defaults
+00001740: 2074 6f20 2222 2028 6e61 6d65 6c79 2c20   to "" (namely, 
+00001750: 6e6f 2077 6f72 6b73 7061 6365 2c20 7061  no workspace, pa
+00001760: 636b 6167 6520 666f 6c64 6572 7320 6172  ckage folders ar
+00001770: 6520 6469 7265 6374 6c79 2075 6e64 6572  e directly under
+00001780: 2074 6865 2070 726f 6a65 6374 2066 6f6c   the project fol
+00001790: 6465 722e 2044 6566 6175 6c74 2069 7320  der. Default is 
+000017a0: 7573 6564 2077 6865 7468 6572 2074 6869  used whether thi
+000017b0: 7320 7061 7261 6d65 7465 7220 6973 2073  s parameter is s
+000017c0: 7065 6369 6669 6564 206f 7220 6e6f 7420  pecified or not 
+000017d0: 2d20 6164 6469 7469 6f6e 616c 206e 616d  - additional nam
+000017e0: 6573 7061 6365 7320 6172 6520 6164 6465  espaces are adde
+000017f0: 642c 2062 7574 2064 6f20 6e6f 7420 6f76  d, but do not ov
+00001800: 6572 7772 6974 6520 6974 292e 207c 0a0a  erwrite it). |..
+00001810: 2323 2070 6172 616d 730a 6578 7065 7269  ## params.experi
+00001820: 6d65 6e74 616c 2e0a 0a67 656e 6572 6174  mental...generat
+00001830: 6520 7061 7261 6d65 7465 7273 2066 6f72  e parameters for
+00001840: 2074 6865 2070 726f 6a65 6374 0a23 2320   the project.## 
+00001850: 7275 6e5f 7369 6d75 6c61 7469 6f6e 0a43  run_simulation.C
+00001860: 7265 6174 6520 6120 6e65 7720 6261 7463  reate a new batc
+00001870: 6820 6f66 2073 696d 756c 6174 696f 6e20  h of simulation 
+00001880: 7275 6e73 2066 6f72 2079 6f75 7220 7072  runs for your pr
+00001890: 6f6a 6563 7420 616e 6420 7275 6e20 6974  oject and run it
+000018a0: 206c 6f63 616c 6c79 2e0a 0a23 2323 2070   locally...### p
+000018b0: 7265 7265 7175 6973 6974 6573 3a0a 5468  rerequisites:.Th
+000018c0: 6520 7072 6f6a 6563 7420 6861 7320 6265  e project has be
+000018d0: 656e 2062 7569 6c74 2c20 736f 7572 6365  en built, source
+000018e0: 6420 616e 6420 6073 796e 6360 6564 2077  d and `sync`ed w
+000018f0: 6974 6820 6369 7472 6f73 2c20 652e 672e  ith citros, e.g.
+00001900: 3a0a 2020 2020 0a20 2020 2063 6f6c 636f  :.    .    colco
+00001910: 6e20 6275 696c 640a 2020 2020 736f 7572  n build.    sour
+00001920: 6365 2069 6e73 7461 6c6c 2f6c 6f63 616c  ce install/local
+00001930: 5f73 6574 7570 2e62 6173 680a 2020 2020  _setup.bash.    
+00001940: 6369 7472 6f73 2073 796e 630a 0a49 6e20  citros sync..In 
+00001950: 7468 6520 6369 7472 6f73 2067 7569 2c20  the citros gui, 
+00001960: 6e61 7669 6761 7465 2074 6f20 796f 7572  navigate to your
+00001970: 2070 726f 6a65 6374 2062 7920 636c 6963   project by clic
+00001980: 6b69 6e67 2074 6865 2074 6872 6565 2076  king the three v
+00001990: 6572 7469 6361 6c20 646f 7473 206f 6e20  ertical dots on 
+000019a0: 7468 6520 7269 6768 7420 7369 6465 206f  the right side o
+000019b0: 6620 6f66 2079 6f75 7220 7072 6f6a 6563  f of your projec
+000019c0: 7427 7320 726f 7720 696e 2074 6865 2070  t's row in the p
+000019d0: 726f 6a65 6374 206c 6973 7420 616e 6420  roject list and 
+000019e0: 7365 6c65 6374 2060 6e61 7669 6761 7465  select `navigate
+000019f0: 603a 200a 215b 6e61 765f 7072 6f6a 5d28  `: .![nav_proj](
+00001a00: 696d 672f 6e61 765f 7072 6f6a 2e70 6e67  img/nav_proj.png
+00001a10: 2022 6e61 7669 6761 7465 2074 6f20 7072   "navigate to pr
+00001a20: 6f6a 6563 7422 2920 0a0a 7768 6963 6820  oject") ..which 
+00001a30: 7769 6c6c 2074 616b 6520 796f 7520 746f  will take you to
+00001a40: 2074 6865 2070 726f 6a65 6374 2773 2044   the project's D
+00001a50: 6574 6169 6c73 2070 6167 652e 200a 0a54  etails page. ..T
+00001a60: 6865 7265 2c20 636c 6963 6b20 7468 6520  here, click the 
+00001a70: 6053 696d 756c 6174 696f 6e20 5365 7475  `Simulation Setu
+00001a80: 7060 2074 6162 3a0a 215b 7369 6d5f 7365  p` tab:.![sim_se
+00001a90: 7475 705d 2869 6d67 2f73 696d 5f73 6574  tup](img/sim_set
+00001aa0: 7570 2e70 6e67 2022 7369 6d75 6c61 7469  up.png "simulati
+00001ab0: 6f6e 2073 6574 7570 2229 0a0a 616e 6420  on setup")..and 
+00001ac0: 636c 6963 6b20 6f6e 2060 6e65 7760 2e0a  click on `new`..
+00001ad0: 0a46 696c 6c20 696e 2061 6e79 2072 656c  .Fill in any rel
+00001ae0: 6576 616e 7420 6465 7461 696c 7320 666f  evant details fo
+00001af0: 7220 7468 6520 6e65 7720 7369 6d75 6c61  r the new simula
+00001b00: 7469 6f6e 2061 6e64 2073 6176 653a 0a21  tion and save:.!
+00001b10: 5b73 6176 655f 6e65 775f 7369 6d5d 2869  [save_new_sim](i
+00001b20: 6d67 2f73 6176 655f 6e65 775f 7369 6d2e  mg/save_new_sim.
+00001b30: 706e 6720 2273 6176 6520 6e65 7720 7369  png "save new si
+00001b40: 6d75 6c61 7469 6f6e 2229 0a0a 4e6f 7720  mulation")..Now 
+00001b50: 636c 6963 6b20 6f6e 2060 5275 6e20 5369  click on `Run Si
+00001b60: 6d75 6c61 7469 6f6e 204c 6f63 616c 6c79  mulation Locally
+00001b70: 603a 0a21 5b72 756e 5f73 696d 5f6c 6f63  `:.![run_sim_loc
+00001b80: 5d28 696d 672f 7275 6e5f 7369 6d5f 6c6f  ](img/run_sim_lo
+00001b90: 632e 706e 6720 2272 756e 2073 696d 756c  c.png "run simul
+00001ba0: 6174 696f 6e20 6c6f 6361 6c6c 7922 290a  ation locally").
+00001bb0: 0a61 6e64 2069 6e20 7468 6520 706f 702d  .and in the pop-
+00001bc0: 7570 2074 6861 7420 636f 6d65 7320 7570  up that comes up
+00001bd0: 2c20 636f 7079 2074 6865 2073 696d 756c  , copy the simul
+00001be0: 6174 696f 6e20 6964 2074 6861 7420 7761  ation id that wa
+00001bf0: 7320 6765 6e65 7261 7465 643a 0a21 5b63  s generated:.![c
+00001c00: 6f70 795f 7369 6d5f 6964 5d28 696d 672f  opy_sim_id](img/
+00001c10: 636f 7079 5f73 696d 5f69 642e 706e 6720  copy_sim_id.png 
+00001c20: 2263 6f70 7920 7468 6520 7369 6d75 6c61  "copy the simula
+00001c30: 7469 6f6e 2069 6422 290a 0a61 6e64 206e  tion id")..and n
+00001c40: 6f77 2c20 6669 6e61 6c6c 792c 2069 6e20  ow, finally, in 
+00001c50: 7468 6520 636f 6d6d 616e 642d 6c69 6e65  the command-line
+00001c60: 2c20 7275 6e0a 0a20 2020 2063 6974 726f  , run..    citro
+00001c70: 7320 7275 6e5f 7369 6d75 6c61 7469 6f6e  s run_simulation
+00001c80: 203c 7369 6d20 6964 3e20 3c72 6570 6574   <sim id> <repet
+00001c90: 6974 696f 6e73 3e0a 7768 6572 6520 603c  itions>.where `<
+00001ca0: 7369 6d5f 6964 3e60 2069 7320 7468 6520  sim_id>` is the 
+00001cb0: 6964 2079 6f75 206a 7573 7420 636f 7069  id you just copi
+00001cc0: 6564 2c20 616e 6420 603c 7265 7065 7469  ed, and `<repeti
+00001cd0: 7469 6f6e 733e 6020 6973 206e 756d 6265  tions>` is numbe
+00001ce0: 7220 6f66 2073 696d 756c 6174 696f 6e20  r of simulation 
+00001cf0: 7275 6e73 2074 6861 7420 7769 6c6c 2072  runs that will r
+00001d00: 756e 2e20 4578 616d 706c 653a 0a20 2020  un. Example:.   
+00001d10: 200a 2020 2020 6369 7472 6f73 2072 756e   .    citros run
+00001d20: 5f73 696d 756c 6174 696f 6e20 6366 3162  _simulation cf1b
+00001d30: 3436 3633 2d61 3665 332d 3439 6264 2d39  4663-a6e3-49bd-9
+00001d40: 3665 352d 6263 3437 6362 3564 3533 3236  6e5-bc47cb5d5326
+00001d50: 2031 0a20 2020 202e 2e2e 0a20 2020 202d   1.    ....    -
+00001d60: 202d 2046 696e 6973 6865 6420 7369 6d75   - Finished simu
+00001d70: 6c61 7469 6f6e 2073 6964 203d 205b 305d  lation sid = [0]
+00001d80: 2077 6974 6820 7265 7475 726e 2063 6f64   with return cod
+00001d90: 6520 5b31 5d2e 0a20 2020 202d 2046 696e  e [1]..    - Fin
+00001da0: 6973 6865 6420 5b61 3762 3138 3864 642d  ished [a7b188dd-
+00001db0: 3734 6262 2d34 6465 392d 6233 3836 2d39  74bb-4de9-b386-9
+00001dc0: 6133 3034 3839 3635 3263 625d 2062 6174  a30489652cb] bat
+00001dd0: 6368 2e0a 0a23 2320 7275 6e0a 5275 6e20  ch...## run.Run 
+00001de0: 6120 7072 6576 696f 7573 6c79 2063 7265  a previously cre
+00001df0: 6174 6564 2062 6174 6368 206c 6f63 616c  ated batch local
+00001e00: 6c79 2e20 5468 6973 2063 6f6d 6d61 6e64  ly. This command
+00001e10: 2069 7320 7573 6566 756c 2077 6865 6e20   is useful when 
+00001e20: 796f 7527 6420 6c69 6b65 2074 6f20 6c6f  you'd like to lo
+00001e30: 6361 6c6c 7920 7265 7275 6e20 6120 6261  cally rerun a ba
+00001e40: 7463 6820 7468 6174 2077 6173 2061 6c72  tch that was alr
+00001e50: 6561 6479 2072 756e 2028 6569 7468 6572  eady run (either
+00001e60: 206c 6f63 616c 6c79 206f 7220 6f6e 2074   locally or on t
+00001e70: 6865 2063 6c75 7374 6572 292e 0a0a 4166  he cluster)...Af
+00001e80: 7465 7220 796f 7527 7665 206c 6f67 6765  ter you've logge
+00001e90: 6420 696e 746f 205b 6369 7472 6f73 2e69  d into [citros.i
+00001ea0: 6f5d 2863 6974 726f 732e 696f 292c 2063  o](citros.io), c
+00001eb0: 6c69 636b 2074 6865 2060 5369 6d75 6c61  lick the `Simula
+00001ec0: 7469 6f6e 2052 756e 7360 2074 6162 3a0a  tion Runs` tab:.
+00001ed0: 215b 7369 6d5f 7275 6e73 5d28 696d 672f  ![sim_runs](img/
+00001ee0: 7369 6d5f 7275 6e73 2e70 6e67 2022 5369  sim_runs.png "Si
+00001ef0: 6d75 6c61 7469 6f6e 2052 756e 7322 2920  mulation Runs") 
+00001f00: 200a 0a61 6e64 206f 6e20 7468 6520 6c69   ..and on the li
+00001f10: 7374 2069 7465 6d20 636f 7272 6573 706f  st item correspo
+00001f20: 6e64 696e 6720 746f 2074 6865 2062 6174  nding to the bat
+00001f30: 6368 2079 6f75 2764 206c 696b 6520 746f  ch you'd like to
+00001f40: 2072 756e 2c20 636c 6963 6b20 7468 6520   run, click the 
+00001f50: 7468 7265 6520 7665 7274 6963 616c 2064  three vertical d
+00001f60: 6f74 7320 6f6e 2074 6865 2072 6967 6874  ots on the right
+00001f70: 2061 6e64 2074 6865 6e20 636c 6963 6b20   and then click 
+00001f80: 6e61 7669 6761 7465 206f 6e20 7468 6520  navigate on the 
+00001f90: 736d 616c 6c20 636f 6e74 6578 7420 6d65  small context me
+00001fa0: 6e75 2074 6861 7420 6f70 656e 732e 2054  nu that opens. T
+00001fb0: 6869 7320 7769 6c6c 2074 616b 6520 796f  his will take yo
+00001fc0: 7520 746f 2074 6865 206c 6973 7420 6f66  u to the list of
+00001fd0: 2073 696d 756c 6174 696f 6e20 7275 6e73   simulation runs
+00001fe0: 2066 6f72 2074 6865 2062 6174 6368 2079   for the batch y
+00001ff0: 6f75 2073 656c 6563 7465 643a 0a21 5b62  ou selected:.![b
+00002000: 6174 6368 5f72 756e 735d 2869 6d67 2f62  atch_runs](img/b
+00002010: 6174 6368 5f72 756e 732e 706e 6720 2242  atch_runs.png "B
+00002020: 6174 6368 2052 756e 7322 290a 0a75 6e64  atch Runs")..und
+00002030: 6572 2074 6865 2060 5369 6d75 6c61 7469  er the `Simulati
+00002040: 6f6e 2052 756e 7360 2068 6561 6469 6e67  on Runs` heading
+00002050: 2c20 796f 7520 6172 6520 7072 6573 656e  , you are presen
+00002060: 7465 6420 7769 7468 2073 6f6d 6520 6d65  ted with some me
+00002070: 7461 6461 7461 2066 6f72 2074 6869 7320  tadata for this 
+00002080: 6261 7463 6820 696e 2074 6865 2066 6f6c  batch in the fol
+00002090: 6c6f 7769 6e67 2066 6f72 6d61 743a 0a0a  lowing format:..
+000020a0: 2020 2020 4461 7368 626f 6172 6420 2d20      Dashboard - 
+000020b0: 5072 6f6a 6563 744c 6973 7420 2d20 3c70  ProjectList - <p
+000020c0: 726f 6a65 6374 5f6e 616d 653e 202d 203c  roject_name> - <
+000020d0: 7369 6d75 6c61 7469 6f6e 5f69 643e 202d  simulation_id> -
+000020e0: 203c 6261 7463 685f 6964 3e0a 0a63 6f70   <batch_id>..cop
+000020f0: 7920 7468 6520 7468 6520 6261 7463 6820  y the the batch 
+00002100: 6964 2c20 616e 6420 696e 2074 6865 2063  id, and in the c
+00002110: 6f6d 6d61 6e64 2d6c 696e 653a 0a0a 2020  ommand-line:..  
+00002120: 2020 6369 7472 6f73 2072 756e 203c 6261    citros run <ba
+00002130: 7463 685f 6964 3e20 3c73 696d 5f72 756e  tch_id> <sim_run
+00002140: 5f69 643e 0a0a 7768 6572 6520 603c 7369  _id>..where `<si
+00002150: 6d5f 7275 6e5f 6964 3e60 2069 7320 7468  m_run_id>` is th
+00002160: 6520 287a 6572 6f2d 6261 7365 6429 2072  e (zero-based) r
+00002170: 756e 2069 6e64 6578 2028 6e6f 7420 746f  un index (not to
+00002180: 2062 6520 636f 6e66 7573 6564 2077 6974   be confused wit
+00002190: 6820 6073 696d 756c 6174 696f 6e5f 6964  h `simulation_id
+000021a0: 6029 2e20 4966 2069 7420 6973 206e 6f74  `). If it is not
+000021b0: 2073 7065 6369 6669 6564 2c20 7468 6520   specified, the 
+000021c0: 656e 7469 7265 2062 6174 6368 2069 7320  entire batch is 
+000021d0: 6578 6563 7574 6564 2e20 4578 616d 706c  executed. Exampl
+000021e0: 653a 0a0a 2020 2020 6369 7472 6f73 2072  e:..    citros r
+000021f0: 756e 2062 6431 3735 6139 332d 3432 3334  un bd175a93-4234
+00002200: 2d34 3234 342d 3934 3264 2d30 6232 6139  -4244-942d-0b2a9
+00002210: 3832 6334 3635 6620 300a 0a23 2320 7570  82c465f 0..## up
+00002220: 6c6f 6164 5f62 6167 0a65 7870 6572 696d  load_bag.experim
+00002230: 656e 7461 6c2e 0a0a 7570 6c6f 6164 2062  ental...upload b
+00002240: 6167 2074 6f20 6369 7472 6f73 2e0a 2323  ag to citros..##
+00002250: 2073 7472 6573 730a 6578 7065 7269 6d65   stress.experime
+00002260: 6e74 616c 2e0a 0a73 7472 6573 7320 7465  ntal...stress te
+00002270: 7374 2074 6865 2073 7973 7465 6d2e 0a23  st the system..#
+00002280: 2320 646f 636b 6572 2d6c 6f67 696e 0a6c  # docker-login.l
+00002290: 6f67 696e 2074 6f20 646f 636b 6572 2d68  ogin to docker-h
+000022a0: 7562 0a23 2320 646f 636b 6572 0a42 7569  ub.## docker.Bui
+000022b0: 6c64 7320 7468 6520 7072 6f6a 6563 742e  lds the project.
```

### Comparing `citros-23.22.2/README.md` & `citros-23.23.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,501 +1,574 @@
-00000000: 6060 6070 7974 686f 6e0a 2320 3d3d 3d3d  ```python.# ====
-00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000030: 3d3d 3d3d 3d3d 3d3d 3d3d 0a23 2020 20e2  ==========.#   .
-00000040: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-00000050: 88e2 9597 e296 88e2 9688 e295 97e2 9688  ................
-00000060: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00000070: 9688 e296 88e2 9597 e296 88e2 9688 e296  ................
-00000080: 88e2 9688 e296 88e2 9688 e295 9720 20e2  .............  .
-00000090: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-000000a0: 88e2 9597 20e2 9688 e296 88e2 9688 e296  .... ...........
-000000b0: 88e2 9688 e296 88e2 9688 e295 970a 2320  ..............# 
-000000c0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
-000000d0: e295 90e2 9590 e295 9de2 9688 e296 88e2  ................
-000000e0: 9591 e295 9ae2 9590 e295 90e2 9688 e296  ................
-000000f0: 88e2 9594 e295 90e2 9590 e295 9de2 9688  ................
-00000100: e296 88e2 9594 e295 90e2 9590 e296 88e2  ................
-00000110: 9688 e295 97e2 9688 e296 88e2 9594 e295  ................
-00000120: 90e2 9590 e295 90e2 9688 e296 88e2 9597  ................
-00000130: e296 88e2 9688 e295 94e2 9590 e295 90e2  ................
-00000140: 9590 e295 90e2 959d 0a23 2020 e296 88e2  .........#  ....
-00000150: 9688 e295 9120 2020 2020 e296 88e2 9688  .....     ......
-00000160: e295 9120 2020 e296 88e2 9688 e295 9120  ...   ......... 
-00000170: 2020 e296 88e2 9688 e296 88e2 9688 e296    ..............
-00000180: 88e2 9688 e295 94e2 959d e296 88e2 9688  ................
-00000190: e295 9120 2020 e296 88e2 9688 e295 91e2  ...   ..........
-000001a0: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
-000001b0: 88e2 9688 e295 970a 2320 20e2 9688 e296  ........#  .....
-000001c0: 88e2 9591 2020 2020 20e2 9688 e296 88e2  ....     .......
-000001d0: 9591 2020 20e2 9688 e296 88e2 9591 2020  ..   .........  
-000001e0: 20e2 9688 e296 88e2 9594 e295 90e2 9590   ...............
-000001f0: e296 88e2 9688 e295 97e2 9688 e296 88e2  ................
-00000200: 9591 2020 20e2 9688 e296 88e2 9591 e295  ..   ...........
-00000210: 9ae2 9590 e295 90e2 9590 e295 90e2 9688  ................
-00000220: e296 88e2 9591 0a23 2020 e295 9ae2 9688  .......#  ......
-00000230: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
-00000240: 9597 e296 88e2 9688 e295 9120 2020 e296  ...........   ..
-00000250: 88e2 9688 e295 9120 2020 e296 88e2 9688  .......   ......
-00000260: e295 9120 20e2 9688 e296 88e2 9591 e295  ...  ...........
-00000270: 9ae2 9688 e296 88e2 9688 e296 88e2 9688  ................
-00000280: e296 88e2 9594 e295 9de2 9688 e296 88e2  ................
-00000290: 9688 e296 88e2 9688 e296 88e2 9688 e295  ................
-000002a0: 910a 2320 2020 e295 9ae2 9590 e295 90e2  ..#   ..........
-000002b0: 9590 e295 90e2 9590 e295 9de2 959a e295  ................
-000002c0: 90e2 959d 2020 20e2 959a e295 90e2 959d  ....   .........
-000002d0: 2020 20e2 959a e295 90e2 959d 2020 e295     .........  ..
-000002e0: 9ae2 9590 e295 9d20 e295 9ae2 9590 e295  ....... ........
-000002f0: 90e2 9590 e295 90e2 9590 e295 9d20 e295  ............. ..
-00000300: 9ae2 9590 e295 90e2 9590 e295 90e2 9590  ................
-00000310: e295 90e2 959d 2020 2020 2020 2020 2020  ......          
-00000320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000330: 2020 2020 2020 2020 2020 2020 2020 0a23                .#
-00000340: 203d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d   ===============
-00000350: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000360: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
-00000370: 6060 600a 2320 4349 5452 4f53 2043 4c49  ```.# CITROS CLI
-00000380: 0a0a 5b21 5b50 7562 6c69 7368 2043 4954  ..[![Publish CIT
-00000390: 524f 535f 434c 4920 746f 2050 7950 4920  ROS_CLI to PyPI 
-000003a0: 2f20 4769 7448 7562 5d28 6874 7470 733a  / GitHub](https:
-000003b0: 2f2f 6769 7468 7562 2e63 6f6d 2f6c 756c  //github.com/lul
-000003c0: 6176 2f63 6974 726f 735f 636c 692f 6163  av/citros_cli/ac
-000003d0: 7469 6f6e 732f 776f 726b 666c 6f77 732f  tions/workflows/
-000003e0: 7265 6c65 6173 655f 746f 5f70 7970 692e  release_to_pypi.
-000003f0: 7961 6d6c 2f62 6164 6765 2e73 7667 295d  yaml/badge.svg)]
-00000400: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-00000410: 636f 6d2f 6c75 6c61 762f 6369 7472 6f73  com/lulav/citros
-00000420: 5f63 6c69 2f61 6374 696f 6e73 2f77 6f72  _cli/actions/wor
-00000430: 6b66 6c6f 7773 2f72 656c 6561 7365 5f74  kflows/release_t
-00000440: 6f5f 7079 7069 2e79 616d 6c29 0a0a 2320  o_pypi.yaml)..# 
-00000450: 4465 7363 7269 7074 696f 6e0a 0a54 6869  Description..Thi
-00000460: 7320 7265 706f 7369 746f 7279 2069 7320  s repository is 
-00000470: 6120 7079 7468 6f6e 2070 6163 6b61 6765  a python package
-00000480: 2074 6861 7420 696d 706c 656d 656e 7473   that implements
-00000490: 2074 6865 2043 4954 524f 5320 434c 4920   the CITROS CLI 
-000004a0: 4150 492e 0a49 7420 6973 2072 756e 2062  API..It is run b
-000004b0: 7920 7468 6520 7573 6572 2069 6e73 6964  y the user insid
-000004c0: 6520 7468 6520 524f 5320 7072 6f6a 6563  e the ROS projec
-000004d0: 7420 666f 6c64 6572 2e20 0a0a 2320 5072  t folder. ..# Pr
-000004e0: 6572 6571 7569 7369 7465 730a 0a2d 205b  erequisites..- [
-000004f0: 7673 636f 6465 5d28 6874 7470 733a 2f2f  vscode](https://
-00000500: 636f 6465 2e76 6973 7561 6c73 7475 6469  code.visualstudi
-00000510: 6f2e 636f 6d2f 646f 776e 6c6f 6164 290a  o.com/download).
-00000520: 2d20 5b44 6f63 6b65 725d 2868 7474 7073  - [Docker](https
-00000530: 3a2f 2f77 7777 2e64 6f63 6b65 722e 636f  ://www.docker.co
-00000540: 6d2f 290a 2d20 5b50 7974 686f 6e33 5d28  m/).- [Python3](
-00000550: 6874 7470 733a 2f2f 7777 772e 7079 7468  https://www.pyth
-00000560: 6f6e 2e6f 7267 2f64 6f77 6e6c 6f61 6473  on.org/downloads
-00000570: 2f29 0a0a 2320 496e 7374 616c 6c61 7469  /)..# Installati
-00000580: 6f6e 0a0a 312e 2063 6c6f 6e65 2074 6865  on..1. clone the
-00000590: 2072 6570 6f3a 0a20 2020 200a 2020 2020   repo:.    .    
-000005a0: 2020 2020 6769 7420 636c 6f6e 6520 6769      git clone gi
-000005b0: 7440 6769 7468 7562 2e63 6f6d 3a6c 756c  t@github.com:lul
-000005c0: 6176 2f63 6974 726f 735f 636c 692e 6769  av/citros_cli.gi
-000005d0: 740a 0a32 2e20 5769 7468 696e 2074 6865  t..2. Within the
-000005e0: 2063 6c6f 6e65 6420 6063 6974 726f 735f   cloned `citros_
-000005f0: 636c 6960 2066 6f6c 6465 722c 206f 7065  cli` folder, ope
-00000600: 6e20 5653 436f 6465 3a0a 2020 2020 0a20  n VSCode:.    . 
-00000610: 2020 2020 2020 2063 6f64 6520 2e0a 0a20         code ... 
-00000620: 2020 2061 6e64 2072 656f 7065 6e20 7468     and reopen th
-00000630: 6520 666f 6c64 6572 2069 6e73 6964 6520  e folder inside 
-00000640: 6120 4465 7620 436f 6e74 6169 6e65 722e  a Dev Container.
-00000650: 0a0a 332e 2049 6e73 7461 6c6c 2074 6865  ..3. Install the
-00000660: 2070 6163 6b61 6765 2066 726f 6d20 7468   package from th
-00000670: 6520 6375 7272 656e 7420 6469 7265 6374  e current direct
-00000680: 6f72 792c 2077 6974 6820 736f 6674 206c  ory, with soft l
-00000690: 696e 6b73 2074 6f20 6465 7620 656e 7669  inks to dev envi
-000006a0: 726f 6e6d 656e 7420 0a0a 2020 2020 2020  ronment ..      
-000006b0: 2020 7079 7468 6f6e 3320 2d6d 2070 6970    python3 -m pip
-000006c0: 2069 6e73 7461 6c6c 202d 6520 2e0a 0a20   install -e ... 
-000006d0: 2020 2028 7265 636f 6d6d 656e 6465 6420     (recommended 
-000006e0: 6475 7269 6e67 2064 6576 656c 6f70 6d65  during developme
-000006f0: 6e74 292c 0a0a 2020 2020 6f72 200a 0a20  nt),..    or .. 
-00000700: 2020 2049 6e73 7461 6c6c 2074 6865 2070     Install the p
-00000710: 6163 6b61 6765 2066 726f 6d20 7468 6520  ackage from the 
-00000720: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
-00000730: 792c 2064 6972 6563 746c 7920 746f 2061  y, directly to a
-00000740: 2067 6c6f 6261 6c20 6269 6e20 666f 6c64   global bin fold
-00000750: 6572 200a 0a20 2020 2020 2020 2070 7974  er ..        pyt
-00000760: 686f 6e33 202d 6d20 7069 7020 696e 7374  hon3 -m pip inst
-00000770: 616c 6c20 2e0a 2020 2020 0a20 2020 2028  all ..    .    (
-00000780: 7368 6f75 6c64 2062 6520 646f 6e65 2062  should be done b
-00000790: 6566 6f72 6520 7570 6c6f 6164 696e 6720  efore uploading 
-000007a0: 746f 2050 7950 492c 2074 6f20 6d61 6b65  to PyPI, to make
-000007b0: 2073 7572 6520 7468 6520 696e 7374 616c   sure the instal
-000007c0: 6c61 7469 6f6e 2069 7320 776f 726b 696e  lation is workin
-000007d0: 6720 7072 6f70 6572 6c79 292e 0a0a 2320  g properly)...# 
-000007e0: 434c 4920 4150 4920 636f 6d6d 616e 6473  CLI API commands
-000007f0: 3a0a 0a23 2320 6c6f 6769 6e0a 4c6f 6769  :..## login.Logi
-00000800: 6e20 746f 2043 4954 524f 532e 0a0a 4166  n to CITROS...Af
-00000810: 7465 7220 656e 7465 7269 6e67 2074 6865  ter entering the
-00000820: 2063 6f6d 6d61 6e64 2c20 796f 7520 7769   command, you wi
-00000830: 6c6c 2062 6520 7072 6f6d 7074 6564 2066  ll be prompted f
-00000840: 6f72 2079 6f75 7220 656d 6169 6c20 2874  or your email (t
-00000850: 6865 2075 7365 726e 616d 6529 2061 6e64  he username) and
-00000860: 2070 6173 7377 6f72 642e 0a0a 6578 616d   password...exam
-00000870: 706c 653a 0a0a 2020 2020 726f 7340 7368  ple:..    ros@sh
-00000880: 616c 6576 2d49 6e73 7069 726f 6e2d 3135  alev-Inspiron-15
-00000890: 2d35 3531 303a 2f77 6f72 6b73 7061 6365  -5510:/workspace
-000008a0: 732f 6361 6e6e 6f6e 2420 6369 7472 6f73  s/cannon$ citros
-000008b0: 206c 6f67 696e 0a20 2020 2065 6d61 696c   login.    email
-000008c0: 3a20 7368 616c 6576 406c 756c 6176 2e73  : shalev@lulav.s
-000008d0: 7061 6365 0a20 2020 2050 6173 7377 6f72  pace.    Passwor
-000008e0: 643a 200a 2020 2020 5573 6572 206c 6f67  d: .    User log
-000008f0: 6765 6420 696e 2e0a 2020 2020 5b32 3032  ged in..    [202
-00000900: 332d 3035 2d31 3120 3038 3a31 323a 3138  3-05-11 08:12:18
-00000910: 2c30 3635 5d20 5b63 6974 726f 732e 6369  ,065] [citros.ci
-00000920: 7472 6f73 2d4e 6f6e 652d 4e6f 6e65 2e6c  tros-None-None.l
-00000930: 6f67 696e 3a32 3638 5d20 5b49 4e46 4f5d  ogin:268] [INFO]
-00000940: 3a20 4175 7468 656e 7469 6361 7465 6421  : Authenticated!
-00000950: 0a0a 2323 2061 7574 6865 6e74 6963 6174  ..## authenticat
-00000960: 650a 4175 7468 656e 7469 6361 7465 2079  e.Authenticate y
-00000970: 6f75 7273 656c 6620 746f 2043 4954 524f  ourself to CITRO
-00000980: 5320 7768 656e 2061 206c 6f67 696e 2069  S when a login i
-00000990: 7320 6e6f 7420 706f 7373 6962 6c65 2c20  s not possible, 
-000009a0: 652e 672e 2077 6865 6e20 7275 6e6e 696e  e.g. when runnin
-000009b0: 6720 696e 2074 6865 2063 6c6f 7564 206f  g in the cloud o
-000009c0: 7220 7065 7266 6f72 6d69 6e67 2061 7574  r performing aut
-000009d0: 6f6d 6174 6564 2074 6573 7473 2e0a 0a46  omated tests...F
-000009e0: 6972 7374 2c20 696e 206f 7264 6572 2074  irst, in order t
-000009f0: 6f20 6f62 7461 696e 2061 2076 616c 6964  o obtain a valid
-00000a00: 2061 7574 6865 6e74 6963 6174 696f 6e20   authentication 
-00000a10: 6b65 792c 206c 6f67 696e 2074 6f20 5b63  key, login to [c
-00000a20: 6974 726f 735d 2868 7474 703a 2f2f 6369  itros](http://ci
-00000a30: 7472 6f73 2e69 6f2f 2920 616e 6420 636c  tros.io/) and cl
-00000a40: 6963 6b20 7468 6520 6041 6464 2050 726f  ick the `Add Pro
-00000a50: 6a65 6374 6020 6275 7474 6f6e 2069 6e20  ject` button in 
-00000a60: 7468 6520 746f 7020 7269 6768 7420 636f  the top right co
-00000a70: 726e 6572 3a0a 215b 6164 645f 7072 6f6a  rner:.![add_proj
-00000a80: 5d28 696d 672f 6164 645f 7072 6f6a 2e70  ](img/add_proj.p
-00000a90: 6e67 2022 6164 6420 7072 6f6a 6563 7422  ng "add project"
-00000aa0: 290a 0a43 6f70 7920 7468 6520 6c69 6e65  )..Copy the line
-00000ab0: 2060 6369 7472 6f73 2061 7574 6865 6e74   `citros authent
-00000ac0: 6963 6174 6520 3c79 6f75 7220 6b65 793e  icate <your key>
-00000ad0: 603a 0a21 5b61 7574 685f 6b65 795d 2869  `:.![auth_key](i
-00000ae0: 6d67 2f61 7574 685f 6b65 792e 706e 6720  mg/auth_key.png 
-00000af0: 2261 7574 6865 6e74 6963 6174 696f 6e20  "authentication 
-00000b00: 6b65 7922 290a 0a20 616e 6420 7061 7374  key").. and past
-00000b10: 6520 6974 2069 6e20 7468 6520 636f 6d6d  e it in the comm
-00000b20: 616e 6420 6c69 6e65 2e0a 0a65 7861 6d70  and line...examp
-00000b30: 6c65 3a0a 0a20 2020 2072 6f73 4073 6861  le:..    ros@sha
-00000b40: 6c65 762d 496e 7370 6972 6f6e 2d31 352d  lev-Inspiron-15-
-00000b50: 3535 3130 3a2f 776f 726b 7370 6163 6573  5510:/workspaces
-00000b60: 2f63 616e 6e6f 6e24 2063 6974 726f 7320  /cannon$ citros 
-00000b70: 6175 7468 656e 7469 6361 7465 2065 794a  authenticate eyJ
-00000b80: 6862 4763 694f 694a 4955 7a49 314e 6949  hbGciOiJIUzI1NiI
-00000b90: 7349 6e52 3563 4349 3649 6b70 5856 434a  sInR5cCI6IkpXVCJ
-00000ba0: 392e 6579 4a79 6232 786c 496a 6f69 5932  9.eyJyb2xlIjoiY2
-00000bb0: 6c30 636d 397a 5832 466b 6257 6c75 4969  l0cm9zX2FkbWluIi
-00000bc0: 7769 6458 4e6c 636c 3970 5a43 4936 496a  widXNlcl9pZCI6Ij
-00000bd0: 4535 4e7a 686a 4f44 5534 4c54 526a 596d  E5NzhjODU4LTRjYm
-00000be0: 4574 4e44 5979 4e53 3034 4e6a 646c 4c54  EtNDYyNS04NjdlLT
-00000bf0: 5577 4d6a 4d32 5a6d 526a 4e6d 5135 4d53  UwMjM2ZmRjNmQ5MS
-00000c00: 4973 496e 567a 5a58 4a66 626d 4674 5a53  IsInVzZXJfbmFtZS
-00000c10: 4936 496e 4e6f 5957 786c 6469 4973 496d  I6InNoYWxldiIsIm
-00000c20: 4e70 6448 4a76 6331 3979 6232 786c 496a  NpdHJvc19yb2xlIj
-00000c30: 6f69 6458 4e6c 6369 4973 496d 3979 5a32  oidXNlciIsIm9yZ2
-00000c40: 4675 6158 7068 6447 6c76 626c 3970 5a43  FuaXphdGlvbl9pZC
-00000c50: 4936 496d 5535 4d54 566b 4e6a 4d35 4c54  I6ImU5MTVkNjM5LT
-00000c60: 597a 4e7a 4974 4e44 566c 4e43 3034 4e54  YzNzItNDVlNC04NT
-00000c70: 566b 4c57 4534 597a 6c69 4e32 5132 5957  VkLWE4YzliN2Q2YW
-00000c80: 4977 4d69 4973 496d 3979 5a32 4675 6158  IwMiIsIm9yZ2FuaX
-00000c90: 7068 6447 6c76 626c 3930 6558 426c 496a  phdGlvbl90eXBlIj
-00000ca0: 6f69 5455 464f 5155 6446 4969 7769 5a47  oiTUFOQUdFIiwiZG
-00000cb0: 3974 5957 6c75 5833 4279 5a57 5a70 6543  9tYWluX3ByZWZpeC
-00000cc0: 4936 496d 7831 6247 4632 4969 7769 5a58  I6Imx1bGF2IiwiZX
-00000cd0: 6877 496a 6f78 4e6a 677a 4e7a 4131 4f54  hwIjoxNjgzNzA1OT
-00000ce0: 557a 4c43 4a70 5958 5169 4f6a 4532 4f44  UzLCJpYXQiOjE2OD
-00000cf0: 4d32 4d54 6b31 4e54 4d73 496d 4631 5a43  M2MTk1NTMsImF1ZC
-00000d00: 4936 496e 4276 6333 526e 636d 4677 6147  I6InBvc3RncmFwaG
-00000d10: 6c73 5a53 4973 496d 6c7a 6379 4936 496e  lsZSIsImlzcyI6In
-00000d20: 4276 6333 526e 636d 4677 6147 6c73 5a53  Bvc3RncmFwaGlsZS
-00000d30: 4a39 2e68 4b67 7832 596c 444d 6848 3233  J9.hKgx2YlDMhH23
-00000d40: 7047 435a 4768 3359 7161 6158 3377 5469  pGCZGh3YqaaX3wTi
-00000d50: 6b6a 4242 7970 4972 5f64 4d38 7467 0a20  kjBBypIr_dM8tg. 
-00000d60: 2020 2041 7574 6865 6e74 6963 6174 6564     Authenticated
-00000d70: 210a 2020 2020 5b32 3032 332d 3035 2d31  !.    [2023-05-1
-00000d80: 3120 3038 3a35 373a 3131 2c30 3030 5d20  1 08:57:11,000] 
-00000d90: 5b63 6974 726f 732e 6369 7472 6f73 2d4e  [citros.citros-N
-00000da0: 6f6e 652d 4e6f 6e65 2e61 7574 6865 6e74  one-None.authent
-00000db0: 6963 6174 655f 7769 7468 5f6b 6579 3a32  icate_with_key:2
-00000dc0: 3139 5d20 5b49 4e46 4f5d 3a20 4175 7468  19] [INFO]: Auth
-00000dd0: 656e 7469 6361 7465 6421 0a4e 6f74 653a  enticated!.Note:
-00000de0: 2074 6865 206b 6579 2069 7320 7661 6c69   the key is vali
-00000df0: 6420 666f 7220 7477 6f20 6461 7973 2c20  d for two days, 
-00000e00: 6166 7465 7220 7768 6963 6820 6120 6e65  after which a ne
-00000e10: 7720 6b65 7920 6e65 6564 7320 746f 2062  w key needs to b
-00000e20: 6520 6765 6e65 7261 7465 642e 2020 0a0a  e generated.  ..
-00000e30: 2323 206c 6f67 6f75 740a 4c6f 676f 7574  ## logout.Logout
-00000e40: 206f 6620 4349 5452 4f53 2e0a 0a65 7861   of CITROS...exa
-00000e50: 6d70 6c65 3a0a 0a20 2020 2072 6f73 4073  mple:..    ros@s
-00000e60: 6861 6c65 762d 496e 7370 6972 6f6e 2d31  halev-Inspiron-1
-00000e70: 352d 3535 3130 3a2f 776f 726b 7370 6163  5-5510:/workspac
-00000e80: 6573 2f63 616e 6e6f 6e24 2063 6974 726f  es/cannon$ citro
-00000e90: 7320 6c6f 676f 7574 0a20 2020 2055 7365  s logout.    Use
-00000ea0: 7220 6c6f 6767 6564 206f 7574 2e0a 2323  r logged out..##
-00000eb0: 2073 796e 630a 5379 6e63 2074 6865 2072   sync.Sync the r
-00000ec0: 6f73 2070 726f 6a65 6374 2074 6f20 6369  os project to ci
-00000ed0: 7472 6f73 2e0a 0a54 6869 7320 636f 6d6d  tros...This comm
-00000ee0: 616e 6420 7769 6c6c 2070 6172 7365 2079  and will parse y
-00000ef0: 6f75 7220 524f 5332 2070 726f 6a65 6374  our ROS2 project
-00000f00: 2c20 6578 7472 6163 7420 7468 6520 6e61  , extract the na
-00000f10: 6d65 7320 6f66 2061 6c6c 2074 6865 2070  mes of all the p
-00000f20: 6163 6b61 6765 732c 200a 6e6f 6465 732c  ackages, .nodes,
-00000f30: 2070 6172 616d 6574 6572 7320 616e 6420   parameters and 
-00000f40: 6c61 756e 6368 2066 696c 6573 2028 616e  launch files (an
-00000f50: 6420 736f 6d65 206f 7468 6572 206d 6574  d some other met
-00000f60: 6164 6174 6129 2c20 0a61 7373 6967 6e20  adata), .assign 
-00000f70: 6561 6368 206f 6620 7468 656d 2061 2055  each of them a U
-00000f80: 4944 2061 6e64 2075 706c 6f61 6420 7468  ID and upload th
-00000f90: 656d 2074 6f20 7468 6520 6369 7472 6f73  em to the citros
-00000fa0: 2064 6174 6162 6173 652e 0a0a 6578 616d   database...exam
-00000fb0: 706c 653a 0a20 2020 200a 2020 2020 726f  ple:.    .    ro
-00000fc0: 7340 7368 616c 6576 2d49 6e73 7069 726f  s@shalev-Inspiro
-00000fd0: 6e2d 3135 2d35 3531 303a 2f77 6f72 6b73  n-15-5510:/works
-00000fe0: 7061 6365 732f 6d61 7373 5f73 7072 696e  paces/mass_sprin
-00000ff0: 675f 6475 6d70 6572 2420 6369 7472 6f73  g_dumper$ citros
-00001000: 2073 796e 630a 2020 2020 2d2d 2d2d 2d2d   sync.    ------
-00001010: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d73 796e  -------------syn
-00001020: 635f 7072 6f6a 6563 742d 2d2d 2d2d 2d2d  c_project-------
-00001030: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020  ------------.   
-00001040: 202e 2e2e 0a20 2020 202d 2d2d 2d2d 2d2d   ....    -------
-00001050: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d44  ---------------D
-00001060: 4f4e 452d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ONE-------------
-00001070: 2d2d 2d2d 2d2d 2d2d 2d2d 2d0a 0a49 6620  -----------..If 
-00001080: 7468 6572 6520 7765 7265 206e 6f20 6368  there were no ch
-00001090: 616e 6765 7320 7369 6e63 6520 7468 6520  anges since the 
-000010a0: 6c61 7374 2073 796e 632c 2074 6865 2073  last sync, the s
-000010b0: 796e 6320 6973 2075 6e6e 6563 6573 7361  ync is unnecessa
-000010c0: 7279 3a0a 0a20 2020 2072 6f73 4073 6861  ry:..    ros@sha
-000010d0: 6c65 762d 496e 7370 6972 6f6e 2d31 352d  lev-Inspiron-15-
-000010e0: 3535 3130 3a2f 776f 726b 7370 6163 6573  5510:/workspaces
-000010f0: 2f6d 6173 735f 7370 7269 6e67 5f64 756d  /mass_spring_dum
-00001100: 7065 7224 2063 6974 726f 7320 7379 6e63  per$ citros sync
-00001110: 0a20 2020 2070 726f 6a65 6374 2061 6c72  .    project alr
-00001120: 6561 6479 2073 796e 6368 6564 2e0a 0a49  eady synched...I
-00001130: 6620 7468 6973 2077 6173 2079 6f75 7220  f this was your 
-00001140: 6669 7273 7420 7469 6d65 2072 756e 6e69  first time runni
-00001150: 6e67 2073 796e 6320 6f6e 2074 6869 7320  ng sync on this 
-00001160: 7072 6f6a 6563 742c 2079 6f75 2063 616e  project, you can
-00001170: 206f 7065 6e20 796f 7572 2066 6176 6f72   open your favor
-00001180: 6974 6520 6272 6f77 7365 7220 616e 6420  ite browser and 
-00001190: 6e61 7669 6761 7465 2074 6f20 5b63 6974  navigate to [cit
-000011a0: 726f 732e 696f 5d28 6369 7472 6f73 2e69  ros.io](citros.i
-000011b0: 6f29 2061 6e64 206c 6f67 2069 6e2c 2061  o) and log in, a
-000011c0: 6e64 2075 6e64 6572 2074 6865 2070 726f  nd under the pro
-000011d0: 6a65 6374 206c 6973 7420 796f 7527 6c6c  ject list you'll
-000011e0: 2073 6565 2061 206e 6577 2069 7465 6d20   see a new item 
-000011f0: 666f 7220 796f 7572 2070 726f 6a65 6374  for your project
-00001200: 2068 6173 2062 6565 6e20 6164 6465 6420   has been added 
-00001210: 746f 2074 6865 206c 6973 743a 0a21 5b70  to the list:.![p
-00001220: 726f 6a65 6374 206c 6973 745d 2869 6d67  roject list](img
-00001230: 2f70 726f 6a5f 6c69 7374 2e70 6e67 2022  /proj_list.png "
-00001240: 7072 6f6a 6563 7420 6c69 7374 2229 0a0a  project list")..
-00001250: 0a23 2323 2070 6172 616d 6574 6572 733a  .### parameters:
-00001260: 0a70 6172 616d 6574 6572 7c64 6573 6372  .parameter|descr
-00001270: 6970 7469 6f6e 0a7c 2d2d 7c2d 2d7c 0a7c  iption.|--|--|.|
-00001280: 602d 6469 7260 203c 666f 6c64 6572 5f6e  `-dir` <folder_n
-00001290: 616d 653e 207c 2054 6865 2077 6f72 6b69  ame> | The worki
-000012a0: 6e67 2064 6972 6563 746f 7279 206f 6620  ng directory of 
-000012b0: 7468 6520 7072 6f6a 6563 742e 2044 6566  the project. Def
-000012c0: 6175 6c74 7320 746f 2022 2e22 2e7c 0a7c  aults to ".".|.|
-000012d0: 602d 6e61 6d65 6020 3c70 726f 6a5f 6e61  `-name` <proj_na
-000012e0: 6d65 3e20 7c20 5468 6520 6e61 6d65 206f  me> | The name o
-000012f0: 6620 7468 6520 7072 6f6a 6563 742e 2044  f the project. D
-00001300: 6566 6175 6c74 7320 746f 2074 6865 206c  efaults to the l
-00001310: 6173 7420 666f 6c64 6572 2069 6e20 7468  ast folder in th
-00001320: 6520 7061 7468 206f 6620 2a64 6972 2a7c  e path of *dir*|
-00001330: 0a7c 602d 7760 2c20 602d 7773 6020 3c77  .|`-w`, `-ws` <w
-00001340: 6f72 6b73 7061 6365 5f6e 616d 653e 207c  orkspace_name> |
-00001350: 2054 6865 206e 616d 6520 6f66 2061 2077   The name of a w
-00001360: 6f72 6b73 7061 6365 2069 6e73 6964 6520  orkspace inside 
-00001370: 7468 6520 7072 6f6a 6563 7420 6469 7265  the project dire
-00001380: 6374 6f72 792e 204d 6179 2062 6520 7573  ctory. May be us
-00001390: 6564 206d 756c 7469 706c 6520 7469 6d65  ed multiple time
-000013a0: 7320 666f 7220 6d75 6c74 6970 6c65 2077  s for multiple w
-000013b0: 6f72 6b73 7061 6365 732e 2044 6566 6175  orkspaces. Defau
-000013c0: 6c74 7320 746f 2022 2220 286e 616d 656c  lts to "" (namel
-000013d0: 792c 206e 6f20 776f 726b 7370 6163 652c  y, no workspace,
-000013e0: 2070 6163 6b61 6765 2066 6f6c 6465 7273   package folders
-000013f0: 2061 7265 2064 6972 6563 746c 7920 756e   are directly un
-00001400: 6465 7220 7468 6520 7072 6f6a 6563 7420  der the project 
-00001410: 666f 6c64 6572 2e20 4465 6661 756c 7420  folder. Default 
-00001420: 6973 2075 7365 6420 7768 6574 6865 7220  is used whether 
-00001430: 7468 6973 2070 6172 616d 6574 6572 2069  this parameter i
-00001440: 7320 7370 6563 6966 6965 6420 6f72 206e  s specified or n
-00001450: 6f74 202d 2061 6464 6974 696f 6e61 6c20  ot - additional 
-00001460: 6e61 6d65 7370 6163 6573 2061 7265 2061  namespaces are a
-00001470: 6464 6564 2c20 6275 7420 646f 206e 6f74  dded, but do not
-00001480: 206f 7665 7277 7269 7465 2069 7429 2e20   overwrite it). 
-00001490: 7c0a 0a23 2320 7061 7261 6d73 0a65 7870  |..## params.exp
-000014a0: 6572 696d 656e 7461 6c2e 0a0a 6765 6e65  erimental...gene
-000014b0: 7261 7465 2070 6172 616d 6574 6572 7320  rate parameters 
-000014c0: 666f 7220 7468 6520 7072 6f6a 6563 740a  for the project.
-000014d0: 2323 2072 756e 5f73 696d 756c 6174 696f  ## run_simulatio
-000014e0: 6e0a 4372 6561 7465 2061 206e 6577 2062  n.Create a new b
-000014f0: 6174 6368 206f 6620 7369 6d75 6c61 7469  atch of simulati
-00001500: 6f6e 2072 756e 7320 666f 7220 796f 7572  on runs for your
-00001510: 2070 726f 6a65 6374 2061 6e64 2072 756e   project and run
-00001520: 2069 7420 6c6f 6361 6c6c 792e 0a0a 2323   it locally...##
-00001530: 2320 7072 6572 6571 7569 7369 7465 733a  # prerequisites:
-00001540: 0a54 6865 2070 726f 6a65 6374 2068 6173  .The project has
-00001550: 2062 6565 6e20 6275 696c 742c 2073 6f75   been built, sou
-00001560: 7263 6564 2061 6e64 2060 7379 6e63 6065  rced and `sync`e
-00001570: 6420 7769 7468 2063 6974 726f 732c 2065  d with citros, e
-00001580: 2e67 2e3a 0a20 2020 200a 2020 2020 636f  .g.:.    .    co
-00001590: 6c63 6f6e 2062 7569 6c64 0a20 2020 2073  lcon build.    s
-000015a0: 6f75 7263 6520 696e 7374 616c 6c2f 6c6f  ource install/lo
-000015b0: 6361 6c5f 7365 7475 702e 6261 7368 0a20  cal_setup.bash. 
-000015c0: 2020 2063 6974 726f 7320 7379 6e63 0a0a     citros sync..
-000015d0: 496e 2074 6865 2063 6974 726f 7320 6775  In the citros gu
-000015e0: 692c 206e 6176 6967 6174 6520 746f 2079  i, navigate to y
-000015f0: 6f75 7220 7072 6f6a 6563 7420 6279 2063  our project by c
-00001600: 6c69 636b 696e 6720 7468 6520 7468 7265  licking the thre
-00001610: 6520 7665 7274 6963 616c 2064 6f74 7320  e vertical dots 
-00001620: 6f6e 2074 6865 2072 6967 6874 2073 6964  on the right sid
-00001630: 6520 6f66 206f 6620 796f 7572 2070 726f  e of of your pro
-00001640: 6a65 6374 2773 2072 6f77 2069 6e20 7468  ject's row in th
-00001650: 6520 7072 6f6a 6563 7420 6c69 7374 2061  e project list a
-00001660: 6e64 2073 656c 6563 7420 606e 6176 6967  nd select `navig
-00001670: 6174 6560 3a20 0a21 5b6e 6176 5f70 726f  ate`: .![nav_pro
-00001680: 6a5d 2869 6d67 2f6e 6176 5f70 726f 6a2e  j](img/nav_proj.
-00001690: 706e 6720 226e 6176 6967 6174 6520 746f  png "navigate to
-000016a0: 2070 726f 6a65 6374 2229 200a 0a77 6869   project") ..whi
-000016b0: 6368 2077 696c 6c20 7461 6b65 2079 6f75  ch will take you
-000016c0: 2074 6f20 7468 6520 7072 6f6a 6563 7427   to the project'
-000016d0: 7320 4465 7461 696c 7320 7061 6765 2e20  s Details page. 
-000016e0: 0a0a 5468 6572 652c 2063 6c69 636b 2074  ..There, click t
-000016f0: 6865 2060 5369 6d75 6c61 7469 6f6e 2053  he `Simulation S
-00001700: 6574 7570 6020 7461 623a 0a21 5b73 696d  etup` tab:.![sim
-00001710: 5f73 6574 7570 5d28 696d 672f 7369 6d5f  _setup](img/sim_
-00001720: 7365 7475 702e 706e 6720 2273 696d 756c  setup.png "simul
-00001730: 6174 696f 6e20 7365 7475 7022 290a 0a61  ation setup")..a
-00001740: 6e64 2063 6c69 636b 206f 6e20 606e 6577  nd click on `new
-00001750: 602e 0a0a 4669 6c6c 2069 6e20 616e 7920  `...Fill in any 
-00001760: 7265 6c65 7661 6e74 2064 6574 6169 6c73  relevant details
-00001770: 2066 6f72 2074 6865 206e 6577 2073 696d   for the new sim
-00001780: 756c 6174 696f 6e20 616e 6420 7361 7665  ulation and save
-00001790: 3a0a 215b 7361 7665 5f6e 6577 5f73 696d  :.![save_new_sim
-000017a0: 5d28 696d 672f 7361 7665 5f6e 6577 5f73  ](img/save_new_s
-000017b0: 696d 2e70 6e67 2022 7361 7665 206e 6577  im.png "save new
-000017c0: 2073 696d 756c 6174 696f 6e22 290a 0a4e   simulation")..N
-000017d0: 6f77 2063 6c69 636b 206f 6e20 6052 756e  ow click on `Run
-000017e0: 2053 696d 756c 6174 696f 6e20 4c6f 6361   Simulation Loca
-000017f0: 6c6c 7960 3a0a 215b 7275 6e5f 7369 6d5f  lly`:.![run_sim_
-00001800: 6c6f 635d 2869 6d67 2f72 756e 5f73 696d  loc](img/run_sim
-00001810: 5f6c 6f63 2e70 6e67 2022 7275 6e20 7369  _loc.png "run si
-00001820: 6d75 6c61 7469 6f6e 206c 6f63 616c 6c79  mulation locally
-00001830: 2229 0a0a 616e 6420 696e 2074 6865 2070  ")..and in the p
-00001840: 6f70 2d75 7020 7468 6174 2063 6f6d 6573  op-up that comes
-00001850: 2075 702c 2063 6f70 7920 7468 6520 7369   up, copy the si
-00001860: 6d75 6c61 7469 6f6e 2069 6420 7468 6174  mulation id that
-00001870: 2077 6173 2067 656e 6572 6174 6564 3a0a   was generated:.
-00001880: 215b 636f 7079 5f73 696d 5f69 645d 2869  ![copy_sim_id](i
-00001890: 6d67 2f63 6f70 795f 7369 6d5f 6964 2e70  mg/copy_sim_id.p
-000018a0: 6e67 2022 636f 7079 2074 6865 2073 696d  ng "copy the sim
-000018b0: 756c 6174 696f 6e20 6964 2229 0a0a 616e  ulation id")..an
-000018c0: 6420 6e6f 772c 2066 696e 616c 6c79 2c20  d now, finally, 
-000018d0: 696e 2074 6865 2063 6f6d 6d61 6e64 2d6c  in the command-l
-000018e0: 696e 652c 2072 756e 0a0a 2020 2020 6369  ine, run..    ci
-000018f0: 7472 6f73 2072 756e 5f73 696d 756c 6174  tros run_simulat
-00001900: 696f 6e20 3c73 696d 2069 643e 203c 7265  ion <sim id> <re
-00001910: 7065 7469 7469 6f6e 733e 0a77 6865 7265  petitions>.where
-00001920: 2060 3c73 696d 5f69 643e 6020 6973 2074   `<sim_id>` is t
-00001930: 6865 2069 6420 796f 7520 6a75 7374 2063  he id you just c
-00001940: 6f70 6965 642c 2061 6e64 2060 3c72 6570  opied, and `<rep
-00001950: 6574 6974 696f 6e73 3e60 2069 7320 6e75  etitions>` is nu
-00001960: 6d62 6572 206f 6620 7369 6d75 6c61 7469  mber of simulati
-00001970: 6f6e 2072 756e 7320 7468 6174 2077 696c  on runs that wil
-00001980: 6c20 7275 6e2e 2045 7861 6d70 6c65 3a0a  l run. Example:.
-00001990: 2020 2020 0a20 2020 2063 6974 726f 7320      .    citros 
-000019a0: 7275 6e5f 7369 6d75 6c61 7469 6f6e 2063  run_simulation c
-000019b0: 6631 6234 3636 332d 6136 6533 2d34 3962  f1b4663-a6e3-49b
-000019c0: 642d 3936 6535 2d62 6334 3763 6235 6435  d-96e5-bc47cb5d5
-000019d0: 3332 3620 310a 2020 2020 2e2e 2e0a 2020  326 1.    ....  
-000019e0: 2020 2d20 2d20 4669 6e69 7368 6564 2073    - - Finished s
-000019f0: 696d 756c 6174 696f 6e20 7369 6420 3d20  imulation sid = 
-00001a00: 5b30 5d20 7769 7468 2072 6574 7572 6e20  [0] with return 
-00001a10: 636f 6465 205b 315d 2e0a 2020 2020 2d20  code [1]..    - 
-00001a20: 4669 6e69 7368 6564 205b 6137 6231 3838  Finished [a7b188
-00001a30: 6464 2d37 3462 622d 3464 6539 2d62 3338  dd-74bb-4de9-b38
-00001a40: 362d 3961 3330 3438 3936 3532 6362 5d20  6-9a30489652cb] 
-00001a50: 6261 7463 682e 0a0a 2323 2072 756e 0a52  batch...## run.R
-00001a60: 756e 2061 2070 7265 7669 6f75 736c 7920  un a previously 
-00001a70: 6372 6561 7465 6420 6261 7463 6820 6c6f  created batch lo
-00001a80: 6361 6c6c 792e 2054 6869 7320 636f 6d6d  cally. This comm
-00001a90: 616e 6420 6973 2075 7365 6675 6c20 7768  and is useful wh
-00001aa0: 656e 2079 6f75 2764 206c 696b 6520 746f  en you'd like to
-00001ab0: 206c 6f63 616c 6c79 2072 6572 756e 2061   locally rerun a
-00001ac0: 2062 6174 6368 2074 6861 7420 7761 7320   batch that was 
-00001ad0: 616c 7265 6164 7920 7275 6e20 2865 6974  already run (eit
-00001ae0: 6865 7220 6c6f 6361 6c6c 7920 6f72 206f  her locally or o
-00001af0: 6e20 7468 6520 636c 7573 7465 7229 2e0a  n the cluster)..
-00001b00: 0a41 6674 6572 2079 6f75 2776 6520 6c6f  .After you've lo
-00001b10: 6767 6564 2069 6e74 6f20 5b63 6974 726f  gged into [citro
-00001b20: 732e 696f 5d28 6369 7472 6f73 2e69 6f29  s.io](citros.io)
-00001b30: 2c20 636c 6963 6b20 7468 6520 6053 696d  , click the `Sim
-00001b40: 756c 6174 696f 6e20 5275 6e73 6020 7461  ulation Runs` ta
-00001b50: 623a 0a21 5b73 696d 5f72 756e 735d 2869  b:.![sim_runs](i
-00001b60: 6d67 2f73 696d 5f72 756e 732e 706e 6720  mg/sim_runs.png 
-00001b70: 2253 696d 756c 6174 696f 6e20 5275 6e73  "Simulation Runs
-00001b80: 2229 2020 0a0a 616e 6420 6f6e 2074 6865  ")  ..and on the
-00001b90: 206c 6973 7420 6974 656d 2063 6f72 7265   list item corre
-00001ba0: 7370 6f6e 6469 6e67 2074 6f20 7468 6520  sponding to the 
-00001bb0: 6261 7463 6820 796f 7527 6420 6c69 6b65  batch you'd like
-00001bc0: 2074 6f20 7275 6e2c 2063 6c69 636b 2074   to run, click t
-00001bd0: 6865 2074 6872 6565 2076 6572 7469 6361  he three vertica
-00001be0: 6c20 646f 7473 206f 6e20 7468 6520 7269  l dots on the ri
-00001bf0: 6768 7420 616e 6420 7468 656e 2063 6c69  ght and then cli
-00001c00: 636b 206e 6176 6967 6174 6520 6f6e 2074  ck navigate on t
-00001c10: 6865 2073 6d61 6c6c 2063 6f6e 7465 7874  he small context
-00001c20: 206d 656e 7520 7468 6174 206f 7065 6e73   menu that opens
-00001c30: 2e20 5468 6973 2077 696c 6c20 7461 6b65  . This will take
-00001c40: 2079 6f75 2074 6f20 7468 6520 6c69 7374   you to the list
-00001c50: 206f 6620 7369 6d75 6c61 7469 6f6e 2072   of simulation r
-00001c60: 756e 7320 666f 7220 7468 6520 6261 7463  uns for the batc
-00001c70: 6820 796f 7520 7365 6c65 6374 6564 3a0a  h you selected:.
-00001c80: 215b 6261 7463 685f 7275 6e73 5d28 696d  ![batch_runs](im
-00001c90: 672f 6261 7463 685f 7275 6e73 2e70 6e67  g/batch_runs.png
-00001ca0: 2022 4261 7463 6820 5275 6e73 2229 0a0a   "Batch Runs")..
-00001cb0: 756e 6465 7220 7468 6520 6053 696d 756c  under the `Simul
-00001cc0: 6174 696f 6e20 5275 6e73 6020 6865 6164  ation Runs` head
-00001cd0: 696e 672c 2079 6f75 2061 7265 2070 7265  ing, you are pre
-00001ce0: 7365 6e74 6564 2077 6974 6820 736f 6d65  sented with some
-00001cf0: 206d 6574 6164 6174 6120 666f 7220 7468   metadata for th
-00001d00: 6973 2062 6174 6368 2069 6e20 7468 6520  is batch in the 
-00001d10: 666f 6c6c 6f77 696e 6720 666f 726d 6174  following format
-00001d20: 3a0a 0a20 2020 2044 6173 6862 6f61 7264  :..    Dashboard
-00001d30: 202d 2050 726f 6a65 6374 4c69 7374 202d   - ProjectList -
-00001d40: 203c 7072 6f6a 6563 745f 6e61 6d65 3e20   <project_name> 
-00001d50: 2d20 3c73 696d 756c 6174 696f 6e5f 6964  - <simulation_id
-00001d60: 3e20 2d20 3c62 6174 6368 5f69 643e 0a0a  > - <batch_id>..
-00001d70: 636f 7079 2074 6865 2074 6865 2062 6174  copy the the bat
-00001d80: 6368 2069 642c 2061 6e64 2069 6e20 7468  ch id, and in th
-00001d90: 6520 636f 6d6d 616e 642d 6c69 6e65 3a0a  e command-line:.
-00001da0: 0a20 2020 2063 6974 726f 7320 7275 6e20  .    citros run 
-00001db0: 3c62 6174 6368 5f69 643e 203c 7369 6d5f  <batch_id> <sim_
-00001dc0: 7275 6e5f 6964 3e0a 0a77 6865 7265 2060  run_id>..where `
-00001dd0: 3c73 696d 5f72 756e 5f69 643e 6020 6973  <sim_run_id>` is
-00001de0: 2074 6865 2028 7a65 726f 2d62 6173 6564   the (zero-based
-00001df0: 2920 7275 6e20 696e 6465 7820 286e 6f74  ) run index (not
-00001e00: 2074 6f20 6265 2063 6f6e 6675 7365 6420   to be confused 
-00001e10: 7769 7468 2060 7369 6d75 6c61 7469 6f6e  with `simulation
-00001e20: 5f69 6460 292e 2049 6620 6974 2069 7320  _id`). If it is 
-00001e30: 6e6f 7420 7370 6563 6966 6965 642c 2074  not specified, t
-00001e40: 6865 2065 6e74 6972 6520 6261 7463 6820  he entire batch 
-00001e50: 6973 2065 7865 6375 7465 642e 2045 7861  is executed. Exa
-00001e60: 6d70 6c65 3a0a 0a20 2020 2063 6974 726f  mple:..    citro
-00001e70: 7320 7275 6e20 6264 3137 3561 3933 2d34  s run bd175a93-4
-00001e80: 3233 342d 3432 3434 2d39 3432 642d 3062  234-4244-942d-0b
-00001e90: 3261 3938 3263 3436 3566 2030 0a0a 2323  2a982c465f 0..##
-00001ea0: 2075 706c 6f61 645f 6261 670a 6578 7065   upload_bag.expe
-00001eb0: 7269 6d65 6e74 616c 2e0a 0a75 706c 6f61  rimental...uploa
-00001ec0: 6420 6261 6720 746f 2063 6974 726f 732e  d bag to citros.
-00001ed0: 0a23 2320 7374 7265 7373 0a65 7870 6572  .## stress.exper
-00001ee0: 696d 656e 7461 6c2e 0a0a 7374 7265 7373  imental...stress
-00001ef0: 2074 6573 7420 7468 6520 7379 7374 656d   test the system
-00001f00: 2e0a 2323 2064 6f63 6b65 722d 6c6f 6769  ..## docker-logi
-00001f10: 6e0a 6c6f 6769 6e20 746f 2064 6f63 6b65  n.login to docke
-00001f20: 722d 6875 620a 2323 2064 6f63 6b65 720a  r-hub.## docker.
-00001f30: 4275 696c 6473 2074 6865 2070 726f 6a65  Builds the proje
-00001f40: 6374 2e                                  ct.
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6369 7472  : 2.1.Name: citr
+00000020: 6f73 0a56 6572 7369 6f6e 3a20 3233 2e32  os.Version: 23.2
+00000030: 332e 310a 5375 6d6d 6172 793a 2041 2063  3.1.Summary: A c
+00000040: 6c69 2065 6e74 7279 706f 696e 7420 666f  li entrypoint fo
+00000050: 7220 7468 6520 6369 7472 6f73 2073 7973  r the citros sys
+00000060: 7465 6d2e 0a48 6f6d 652d 7061 6765 3a20  tem..Home-page: 
+00000070: 6874 7470 3a2f 2f70 7970 692e 7079 7468  http://pypi.pyth
+00000080: 6f6e 2e6f 7267 2f70 7970 692f 6369 7472  on.org/pypi/citr
+00000090: 6f73 5f63 6c69 2f0a 4175 7468 6f72 3a20  os_cli/.Author: 
+000000a0: 766f 7661 636f 6f70 6572 0a41 7574 686f  vovacooper.Autho
+000000b0: 722d 656d 6169 6c3a 2076 6f76 6140 6c75  r-email: vova@lu
+000000c0: 6c61 762e 7370 6163 650a 4c69 6365 6e73  lav.space.Licens
+000000d0: 653a 204c 4943 454e 5345 2e74 7874 0a44  e: LICENSE.txt.D
+000000e0: 6573 6372 6970 7469 6f6e 2d43 6f6e 7465  escription-Conte
+000000f0: 6e74 2d54 7970 653a 2074 6578 742f 6d61  nt-Type: text/ma
+00000100: 726b 646f 776e 0a4c 6963 656e 7365 2d46  rkdown.License-F
+00000110: 696c 653a 204c 4943 454e 5345 0a0a 6060  ile: LICENSE..``
+00000120: 6070 7974 686f 6e0a 2320 3d3d 3d3d 3d3d  `python.# ======
+00000130: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000140: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000150: 3d3d 3d3d 3d3d 3d3d 0a23 2020 20e2 9688  ========.#   ...
+00000160: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+00000170: 9597 e296 88e2 9688 e295 97e2 9688 e296  ................
+00000180: 88e2 9688 e296 88e2 9688 e296 88e2 9688  ................
+00000190: e296 88e2 9597 e296 88e2 9688 e296 88e2  ................
+000001a0: 9688 e296 88e2 9688 e295 9720 20e2 9688  ...........  ...
+000001b0: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+000001c0: 9597 20e2 9688 e296 88e2 9688 e296 88e2  .. .............
+000001d0: 9688 e296 88e2 9688 e295 970a 2320 20e2  ............#  .
+000001e0: 9688 e296 88e2 9594 e295 90e2 9590 e295  ................
+000001f0: 90e2 9590 e295 9de2 9688 e296 88e2 9591  ................
+00000200: e295 9ae2 9590 e295 90e2 9688 e296 88e2  ................
+00000210: 9594 e295 90e2 9590 e295 9de2 9688 e296  ................
+00000220: 88e2 9594 e295 90e2 9590 e296 88e2 9688  ................
+00000230: e295 97e2 9688 e296 88e2 9594 e295 90e2  ................
+00000240: 9590 e295 90e2 9688 e296 88e2 9597 e296  ................
+00000250: 88e2 9688 e295 94e2 9590 e295 90e2 9590  ................
+00000260: e295 90e2 959d 0a23 2020 e296 88e2 9688  .......#  ......
+00000270: e295 9120 2020 2020 e296 88e2 9688 e295  ...     ........
+00000280: 9120 2020 e296 88e2 9688 e295 9120 2020  .   .........   
+00000290: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+000002a0: 9688 e295 94e2 959d e296 88e2 9688 e295  ................
+000002b0: 9120 2020 e296 88e2 9688 e295 91e2 9688  .   ............
+000002c0: e296 88e2 9688 e296 88e2 9688 e296 88e2  ................
+000002d0: 9688 e295 970a 2320 20e2 9688 e296 88e2  ......#  .......
+000002e0: 9591 2020 2020 20e2 9688 e296 88e2 9591  ..     .........
+000002f0: 2020 20e2 9688 e296 88e2 9591 2020 20e2     .........   .
+00000300: 9688 e296 88e2 9594 e295 90e2 9590 e296  ................
+00000310: 88e2 9688 e295 97e2 9688 e296 88e2 9591  ................
+00000320: 2020 20e2 9688 e296 88e2 9591 e295 9ae2     .............
+00000330: 9590 e295 90e2 9590 e295 90e2 9688 e296  ................
+00000340: 88e2 9591 0a23 2020 e295 9ae2 9688 e296  .....#  ........
+00000350: 88e2 9688 e296 88e2 9688 e296 88e2 9597  ................
+00000360: e296 88e2 9688 e295 9120 2020 e296 88e2  .........   ....
+00000370: 9688 e295 9120 2020 e296 88e2 9688 e295  .....   ........
+00000380: 9120 20e2 9688 e296 88e2 9591 e295 9ae2  .  .............
+00000390: 9688 e296 88e2 9688 e296 88e2 9688 e296  ................
+000003a0: 88e2 9594 e295 9de2 9688 e296 88e2 9688  ................
+000003b0: e296 88e2 9688 e296 88e2 9688 e295 910a  ................
+000003c0: 2320 2020 e295 9ae2 9590 e295 90e2 9590  #   ............
+000003d0: e295 90e2 9590 e295 9de2 959a e295 90e2  ................
+000003e0: 959d 2020 20e2 959a e295 90e2 959d 2020  ..   .........  
+000003f0: 20e2 959a e295 90e2 959d 2020 e295 9ae2   .........  ....
+00000400: 9590 e295 9d20 e295 9ae2 9590 e295 90e2  ..... ..........
+00000410: 9590 e295 90e2 9590 e295 9d20 e295 9ae2  ........... ....
+00000420: 9590 e295 90e2 9590 e295 90e2 9590 e295  ................
+00000430: 90e2 959d 2020 2020 2020 2020 2020 2020  ....            
+00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000450: 2020 2020 2020 2020 2020 2020 0a23 203d              .# =
+00000460: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000470: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
+00000480: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 6060  =============.``
+00000490: 600a 2320 4349 5452 4f53 2043 4c49 0a0a  `.# CITROS CLI..
+000004a0: 5b21 5b50 7562 6c69 7368 2043 4954 524f  [![Publish CITRO
+000004b0: 535f 434c 4920 746f 2050 7950 4920 2f20  S_CLI to PyPI / 
+000004c0: 4769 7448 7562 5d28 6874 7470 733a 2f2f  GitHub](https://
+000004d0: 6769 7468 7562 2e63 6f6d 2f6c 756c 6176  github.com/lulav
+000004e0: 2f63 6974 726f 735f 636c 692f 6163 7469  /citros_cli/acti
+000004f0: 6f6e 732f 776f 726b 666c 6f77 732f 7265  ons/workflows/re
+00000500: 6c65 6173 655f 746f 5f70 7970 692e 7961  lease_to_pypi.ya
+00000510: 6d6c 2f62 6164 6765 2e73 7667 295d 2868  ml/badge.svg)](h
+00000520: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000530: 6d2f 6c75 6c61 762f 6369 7472 6f73 5f63  m/lulav/citros_c
+00000540: 6c69 2f61 6374 696f 6e73 2f77 6f72 6b66  li/actions/workf
+00000550: 6c6f 7773 2f72 656c 6561 7365 5f74 6f5f  lows/release_to_
+00000560: 7079 7069 2e79 616d 6c29 0a0a 2320 4465  pypi.yaml)..# De
+00000570: 7363 7269 7074 696f 6e0a 0a54 6869 7320  scription..This 
+00000580: 7265 706f 7369 746f 7279 2069 7320 6120  repository is a 
+00000590: 7079 7468 6f6e 2070 6163 6b61 6765 2074  python package t
+000005a0: 6861 7420 696d 706c 656d 656e 7473 2074  hat implements t
+000005b0: 6865 2043 4954 524f 5320 434c 4920 4150  he CITROS CLI AP
+000005c0: 492e 0a49 7420 6973 2072 756e 2062 7920  I..It is run by 
+000005d0: 7468 6520 7573 6572 2069 6e73 6964 6520  the user inside 
+000005e0: 7468 6520 524f 5320 7072 6f6a 6563 7420  the ROS project 
+000005f0: 666f 6c64 6572 2e20 0a0a 2320 5072 6572  folder. ..# Prer
+00000600: 6571 7569 7369 7465 730a 0a2d 205b 7673  equisites..- [vs
+00000610: 636f 6465 5d28 6874 7470 733a 2f2f 636f  code](https://co
+00000620: 6465 2e76 6973 7561 6c73 7475 6469 6f2e  de.visualstudio.
+00000630: 636f 6d2f 646f 776e 6c6f 6164 290a 2d20  com/download).- 
+00000640: 5b44 6f63 6b65 725d 2868 7474 7073 3a2f  [Docker](https:/
+00000650: 2f77 7777 2e64 6f63 6b65 722e 636f 6d2f  /www.docker.com/
+00000660: 290a 2d20 5b50 7974 686f 6e33 5d28 6874  ).- [Python3](ht
+00000670: 7470 733a 2f2f 7777 772e 7079 7468 6f6e  tps://www.python
+00000680: 2e6f 7267 2f64 6f77 6e6c 6f61 6473 2f29  .org/downloads/)
+00000690: 0a0a 2320 496e 7374 616c 6c61 7469 6f6e  ..# Installation
+000006a0: 0a0a 312e 2063 6c6f 6e65 2074 6865 2072  ..1. clone the r
+000006b0: 6570 6f3a 0a20 2020 200a 2020 2020 2020  epo:.    .      
+000006c0: 2020 6769 7420 636c 6f6e 6520 6769 7440    git clone git@
+000006d0: 6769 7468 7562 2e63 6f6d 3a6c 756c 6176  github.com:lulav
+000006e0: 2f63 6974 726f 735f 636c 692e 6769 740a  /citros_cli.git.
+000006f0: 0a32 2e20 5769 7468 696e 2074 6865 2063  .2. Within the c
+00000700: 6c6f 6e65 6420 6063 6974 726f 735f 636c  loned `citros_cl
+00000710: 6960 2066 6f6c 6465 722c 206f 7065 6e20  i` folder, open 
+00000720: 5653 436f 6465 3a0a 2020 2020 0a20 2020  VSCode:.    .   
+00000730: 2020 2020 2063 6f64 6520 2e0a 0a20 2020       code ...   
+00000740: 2061 6e64 2072 656f 7065 6e20 7468 6520   and reopen the 
+00000750: 666f 6c64 6572 2069 6e73 6964 6520 6120  folder inside a 
+00000760: 4465 7620 436f 6e74 6169 6e65 722e 0a0a  Dev Container...
+00000770: 332e 2049 6e73 7461 6c6c 2074 6865 2070  3. Install the p
+00000780: 6163 6b61 6765 2066 726f 6d20 7468 6520  ackage from the 
+00000790: 6375 7272 656e 7420 6469 7265 6374 6f72  current director
+000007a0: 792c 2077 6974 6820 736f 6674 206c 696e  y, with soft lin
+000007b0: 6b73 2074 6f20 6465 7620 656e 7669 726f  ks to dev enviro
+000007c0: 6e6d 656e 7420 0a0a 2020 2020 2020 2020  nment ..        
+000007d0: 7079 7468 6f6e 3320 2d6d 2070 6970 2069  python3 -m pip i
+000007e0: 6e73 7461 6c6c 202d 6520 2e0a 0a20 2020  nstall -e ...   
+000007f0: 2028 7265 636f 6d6d 656e 6465 6420 6475   (recommended du
+00000800: 7269 6e67 2064 6576 656c 6f70 6d65 6e74  ring development
+00000810: 292c 0a0a 2020 2020 6f72 200a 0a20 2020  ),..    or ..   
+00000820: 2049 6e73 7461 6c6c 2074 6865 2070 6163   Install the pac
+00000830: 6b61 6765 2066 726f 6d20 7468 6520 6375  kage from the cu
+00000840: 7272 656e 7420 6469 7265 6374 6f72 792c  rrent directory,
+00000850: 2064 6972 6563 746c 7920 746f 2061 2067   directly to a g
+00000860: 6c6f 6261 6c20 6269 6e20 666f 6c64 6572  lobal bin folder
+00000870: 200a 0a20 2020 2020 2020 2070 7974 686f   ..        pytho
+00000880: 6e33 202d 6d20 7069 7020 696e 7374 616c  n3 -m pip instal
+00000890: 6c20 2e0a 2020 2020 0a20 2020 2028 7368  l ..    .    (sh
+000008a0: 6f75 6c64 2062 6520 646f 6e65 2062 6566  ould be done bef
+000008b0: 6f72 6520 7570 6c6f 6164 696e 6720 746f  ore uploading to
+000008c0: 2050 7950 492c 2074 6f20 6d61 6b65 2073   PyPI, to make s
+000008d0: 7572 6520 7468 6520 696e 7374 616c 6c61  ure the installa
+000008e0: 7469 6f6e 2069 7320 776f 726b 696e 6720  tion is working 
+000008f0: 7072 6f70 6572 6c79 292e 0a0a 342e 2045  properly)...4. E
+00000900: 6e76 0a0a 7c20 454e 5620 7c20 4465 7363  nv..| ENV | Desc
+00000910: 7269 7074 696f 6e20 7c20 7573 6564 2069  ription | used i
+00000920: 6e20 7c0a 7c20 2d2d 2d20 7c20 2d2d 2d20  n |.| --- | --- 
+00000930: 7c20 2d2d 2d20 7c0a 7c20 6043 4954 524f  | --- |.| `CITRO
+00000940: 535f 444f 4d41 494e 6020 7c20 7468 6520  S_DOMAIN` | the 
+00000950: 6d61 696e 2064 6f6d 6169 6e2c 2064 6566  main domain, def
+00000960: 6175 6c74 2069 7320 6063 6974 726f 732e  ault is `citros.
+00000970: 696f 6020 7c20 616c 6c20 7061 636b 6167  io` | all packag
+00000980: 6573 207c 0a7c 2060 4349 5452 4f53 5f44  es |.| `CITROS_D
+00000990: 4154 415f 484f 5354 6020 7c20 686f 7374  ATA_HOST` | host
+000009a0: 206f 6620 7468 6520 706c 6179 6772 6f75   of the playgrou
+000009b0: 6e64 2050 4744 422c 2064 6566 6175 6c74  nd PGDB, default
+000009c0: 2063 6f6d 6573 2066 726f 6d20 7369 6d75   comes from simu
+000009d0: 6c61 7469 6f6e 206a 6f62 2065 6e76 2028  lation job env (
+000009e0: 6369 7472 6f73 5f77 6f72 6b65 7229 2061  citros_worker) a
+000009f0: 6e64 2069 733a 2060 7368 6172 6564 2d70  nd is: `shared-p
+00000a00: 6c61 7967 726f 756e 642d 706f 7374 6772  layground-postgr
+00000a10: 6573 716c 2e6e 732d 6369 7472 6f73 2d73  esql.ns-citros-s
+00000a20: 6861 7265 6460 2e20 7573 6564 2066 6f72  hared`. used for
+00000a30: 2075 706c 6f61 6469 6e67 2042 4147 2e20   uploading BAG. 
+00000a40: 7c20 6369 7472 6f73 5f62 6167 207c 0a7c  | citros_bag |.|
+00000a50: 2060 4349 5452 4f53 5f44 4154 415f 504f   `CITROS_DATA_PO
+00000a60: 5254 6020 7c20 7468 6520 706f 7274 206f  RT` | the port o
+00000a70: 6620 5047 4442 2c20 6465 6661 756c 7420  f PGDB, default 
+00000a80: 6035 3433 3260 207c 2063 6974 726f 735f  `5432` | citros_
+00000a90: 6261 6720 7c0a 7c20 6043 4954 524f 535f  bag |.| `CITROS_
+00000aa0: 4441 5441 5f44 4154 4142 4153 4560 207c  DATA_DATABASE` |
+00000ab0: 2074 6865 2064 6174 6162 6173 6520 746f   the database to
+00000ac0: 2061 6363 6573 7320 696e 7369 6465 2050   access inside P
+00000ad0: 4744 422e 2064 6566 6175 6c74 2063 6f6d  GDB. default com
+00000ae0: 6573 2066 726f 6d20 7369 6d75 6c61 7469  es from simulati
+00000af0: 6f6e 206a 6f62 2065 6e76 2028 6369 7472  on job env (citr
+00000b00: 6f73 5f77 6f72 6b65 7229 2061 6e64 2069  os_worker) and i
+00000b10: 733a 2060 646f 6d61 696e 5f70 7265 6669  s: `domain_prefi
+00000b20: 7860 2e20 7573 6564 2066 6f72 2075 706c  x`. used for upl
+00000b30: 6f61 6469 6e67 2042 4147 2e20 7c20 6369  oading BAG. | ci
+00000b40: 7472 6f73 5f62 6167 207c 0a7c 2060 4349  tros_bag |.| `CI
+00000b50: 5452 4f53 5f44 4154 415f 5553 4552 4e41  TROS_DATA_USERNA
+00000b60: 4d45 6020 7c20 7468 6520 7573 6572 6e61  ME` | the userna
+00000b70: 6d65 2074 6f20 6163 6365 7373 2050 4744  me to access PGD
+00000b80: 422c 2064 6566 6175 6c74 2060 6369 7472  B, default `citr
+00000b90: 6f73 5f61 6e6f 6e79 6d6f 7573 602e 2074  os_anonymous`. t
+00000ba0: 6865 2075 7365 726e 616d 6520 6973 2074  he username is t
+00000bb0: 6865 2075 7365 726e 616d 6520 6672 6f6d  he username from
+00000bc0: 2063 6974 726f 732e 2020 7c20 6369 7472   citros.  | citr
+00000bd0: 6f73 5f62 6167 207c 0a7c 2060 4349 5452  os_bag |.| `CITR
+00000be0: 4f53 5f44 4154 415f 5041 5353 574f 5244  OS_DATA_PASSWORD
+00000bf0: 6020 7c20 7468 6520 7061 7373 776f 7264  ` | the password
+00000c00: 2074 6f20 6163 6365 7373 2050 4744 422c   to access PGDB,
+00000c10: 2064 6566 6175 6c74 2060 6369 7472 6f73   default `citros
+00000c20: 5f61 6e6f 6e79 6d6f 7573 602e 2074 6865  _anonymous`. the
+00000c30: 2070 6173 7377 6f72 6420 6973 2074 6865   password is the
+00000c40: 2069 6420 6f66 2074 6865 2075 7365 7220   id of the user 
+00000c50: 696e 2060 6369 7472 6f73 2e75 7365 7260  in `citros.user`
+00000c60: 2074 6162 6c65 2e20 207c 2063 6974 726f   table.  | citro
+00000c70: 735f 6261 6720 7c0a 0a23 2043 4c49 2041  s_bag |..# CLI A
+00000c80: 5049 2063 6f6d 6d61 6e64 733a 0a0a 2323  PI commands:..##
+00000c90: 206c 6f67 696e 0a4c 6f67 696e 2074 6f20   login.Login to 
+00000ca0: 4349 5452 4f53 2e0a 0a41 6674 6572 2065  CITROS...After e
+00000cb0: 6e74 6572 696e 6720 7468 6520 636f 6d6d  ntering the comm
+00000cc0: 616e 642c 2079 6f75 2077 696c 6c20 6265  and, you will be
+00000cd0: 2070 726f 6d70 7465 6420 666f 7220 796f   prompted for yo
+00000ce0: 7572 2065 6d61 696c 2028 7468 6520 7573  ur email (the us
+00000cf0: 6572 6e61 6d65 2920 616e 6420 7061 7373  ername) and pass
+00000d00: 776f 7264 2e0a 0a65 7861 6d70 6c65 3a0a  word...example:.
+00000d10: 0a20 2020 2072 6f73 4073 6861 6c65 762d  .    ros@shalev-
+00000d20: 496e 7370 6972 6f6e 2d31 352d 3535 3130  Inspiron-15-5510
+00000d30: 3a2f 776f 726b 7370 6163 6573 2f63 616e  :/workspaces/can
+00000d40: 6e6f 6e24 2063 6974 726f 7320 6c6f 6769  non$ citros logi
+00000d50: 6e0a 2020 2020 656d 6169 6c3a 2073 6861  n.    email: sha
+00000d60: 6c65 7640 6c75 6c61 762e 7370 6163 650a  lev@lulav.space.
+00000d70: 2020 2020 5061 7373 776f 7264 3a20 0a20      Password: . 
+00000d80: 2020 2055 7365 7220 6c6f 6767 6564 2069     User logged i
+00000d90: 6e2e 0a20 2020 205b 3230 3233 2d30 352d  n..    [2023-05-
+00000da0: 3131 2030 383a 3132 3a31 382c 3036 355d  11 08:12:18,065]
+00000db0: 205b 6369 7472 6f73 2e63 6974 726f 732d   [citros.citros-
+00000dc0: 4e6f 6e65 2d4e 6f6e 652e 6c6f 6769 6e3a  None-None.login:
+00000dd0: 3236 385d 205b 494e 464f 5d3a 2041 7574  268] [INFO]: Aut
+00000de0: 6865 6e74 6963 6174 6564 210a 0a23 2320  henticated!..## 
+00000df0: 6175 7468 656e 7469 6361 7465 0a41 7574  authenticate.Aut
+00000e00: 6865 6e74 6963 6174 6520 796f 7572 7365  henticate yourse
+00000e10: 6c66 2074 6f20 4349 5452 4f53 2077 6865  lf to CITROS whe
+00000e20: 6e20 6120 6c6f 6769 6e20 6973 206e 6f74  n a login is not
+00000e30: 2070 6f73 7369 626c 652c 2065 2e67 2e20   possible, e.g. 
+00000e40: 7768 656e 2072 756e 6e69 6e67 2069 6e20  when running in 
+00000e50: 7468 6520 636c 6f75 6420 6f72 2070 6572  the cloud or per
+00000e60: 666f 726d 696e 6720 6175 746f 6d61 7465  forming automate
+00000e70: 6420 7465 7374 732e 0a0a 4669 7273 742c  d tests...First,
+00000e80: 2069 6e20 6f72 6465 7220 746f 206f 6274   in order to obt
+00000e90: 6169 6e20 6120 7661 6c69 6420 6175 7468  ain a valid auth
+00000ea0: 656e 7469 6361 7469 6f6e 206b 6579 2c20  entication key, 
+00000eb0: 6c6f 6769 6e20 746f 205b 6369 7472 6f73  login to [citros
+00000ec0: 5d28 6874 7470 3a2f 2f63 6974 726f 732e  ](http://citros.
+00000ed0: 696f 2f29 2061 6e64 2063 6c69 636b 2074  io/) and click t
+00000ee0: 6865 2060 4164 6420 5072 6f6a 6563 7460  he `Add Project`
+00000ef0: 2062 7574 746f 6e20 696e 2074 6865 2074   button in the t
+00000f00: 6f70 2072 6967 6874 2063 6f72 6e65 723a  op right corner:
+00000f10: 0a21 5b61 6464 5f70 726f 6a5d 2869 6d67  .![add_proj](img
+00000f20: 2f61 6464 5f70 726f 6a2e 706e 6720 2261  /add_proj.png "a
+00000f30: 6464 2070 726f 6a65 6374 2229 0a0a 436f  dd project")..Co
+00000f40: 7079 2074 6865 206c 696e 6520 6063 6974  py the line `cit
+00000f50: 726f 7320 6175 7468 656e 7469 6361 7465  ros authenticate
+00000f60: 203c 796f 7572 206b 6579 3e60 3a0a 215b   <your key>`:.![
+00000f70: 6175 7468 5f6b 6579 5d28 696d 672f 6175  auth_key](img/au
+00000f80: 7468 5f6b 6579 2e70 6e67 2022 6175 7468  th_key.png "auth
+00000f90: 656e 7469 6361 7469 6f6e 206b 6579 2229  entication key")
+00000fa0: 0a0a 2061 6e64 2070 6173 7465 2069 7420  .. and paste it 
+00000fb0: 696e 2074 6865 2063 6f6d 6d61 6e64 206c  in the command l
+00000fc0: 696e 652e 0a0a 6578 616d 706c 653a 0a0a  ine...example:..
+00000fd0: 2020 2020 726f 7340 7368 616c 6576 2d49      ros@shalev-I
+00000fe0: 6e73 7069 726f 6e2d 3135 2d35 3531 303a  nspiron-15-5510:
+00000ff0: 2f77 6f72 6b73 7061 6365 732f 6361 6e6e  /workspaces/cann
+00001000: 6f6e 2420 6369 7472 6f73 2061 7574 6865  on$ citros authe
+00001010: 6e74 6963 6174 6520 6579 4a68 6247 6369  nticate eyJhbGci
+00001020: 4f69 4a49 557a 4931 4e69 4973 496e 5235  OiJIUzI1NiIsInR5
+00001030: 6343 4936 496b 7058 5643 4a39 2e65 794a  cCI6IkpXVCJ9.eyJ
+00001040: 7962 3278 6c49 6a6f 6959 326c 3063 6d39  yb2xlIjoiY2l0cm9
+00001050: 7a58 3246 6b62 576c 7549 6977 6964 584e  zX2FkbWluIiwidXN
+00001060: 6c63 6c39 705a 4349 3649 6a45 354e 7a68  lcl9pZCI6IjE5Nzh
+00001070: 6a4f 4455 344c 5452 6a59 6d45 744e 4459  jODU4LTRjYmEtNDY
+00001080: 794e 5330 344e 6a64 6c4c 5455 774d 6a4d  yNS04NjdlLTUwMjM
+00001090: 325a 6d52 6a4e 6d51 354d 5349 7349 6e56  2ZmRjNmQ5MSIsInV
+000010a0: 7a5a 584a 6662 6d46 745a 5349 3649 6e4e  zZXJfbmFtZSI6InN
+000010b0: 6f59 5778 6c64 6949 7349 6d4e 7064 484a  oYWxldiIsImNpdHJ
+000010c0: 7663 3139 7962 3278 6c49 6a6f 6964 584e  vc19yb2xlIjoidXN
+000010d0: 6c63 6949 7349 6d39 795a 3246 7561 5870  lciIsIm9yZ2FuaXp
+000010e0: 6864 476c 7662 6c39 705a 4349 3649 6d55  hdGlvbl9pZCI6ImU
+000010f0: 354d 5456 6b4e 6a4d 354c 5459 7a4e 7a49  5MTVkNjM5LTYzNzI
+00001100: 744e 4456 6c4e 4330 344e 5456 6b4c 5745  tNDVlNC04NTVkLWE
+00001110: 3459 7a6c 694e 3251 3259 5749 774d 6949  4YzliN2Q2YWIwMiI
+00001120: 7349 6d39 795a 3246 7561 5870 6864 476c  sIm9yZ2FuaXphdGl
+00001130: 7662 6c39 3065 5842 6c49 6a6f 6954 5546  vbl90eXBlIjoiTUF
+00001140: 4f51 5564 4649 6977 695a 4739 7459 576c  OQUdFIiwiZG9tYWl
+00001150: 7558 3342 795a 575a 7065 4349 3649 6d78  uX3ByZWZpeCI6Imx
+00001160: 3162 4746 3249 6977 695a 5868 7749 6a6f  1bGF2IiwiZXhwIjo
+00001170: 784e 6a67 7a4e 7a41 314f 5455 7a4c 434a  xNjgzNzA1OTUzLCJ
+00001180: 7059 5851 694f 6a45 324f 444d 324d 546b  pYXQiOjE2ODM2MTk
+00001190: 314e 544d 7349 6d46 315a 4349 3649 6e42  1NTMsImF1ZCI6InB
+000011a0: 7663 3352 6e63 6d46 7761 476c 735a 5349  vc3RncmFwaGlsZSI
+000011b0: 7349 6d6c 7a63 7949 3649 6e42 7663 3352  sImlzcyI6InBvc3R
+000011c0: 6e63 6d46 7761 476c 735a 534a 392e 684b  ncmFwaGlsZSJ9.hK
+000011d0: 6778 3259 6c44 4d68 4832 3370 4743 5a47  gx2YlDMhH23pGCZG
+000011e0: 6833 5971 6161 5833 7754 696b 6a42 4279  h3YqaaX3wTikjBBy
+000011f0: 7049 725f 644d 3874 670a 2020 2020 4175  pIr_dM8tg.    Au
+00001200: 7468 656e 7469 6361 7465 6421 0a20 2020  thenticated!.   
+00001210: 205b 3230 3233 2d30 352d 3131 2030 383a   [2023-05-11 08:
+00001220: 3537 3a31 312c 3030 305d 205b 6369 7472  57:11,000] [citr
+00001230: 6f73 2e63 6974 726f 732d 4e6f 6e65 2d4e  os.citros-None-N
+00001240: 6f6e 652e 6175 7468 656e 7469 6361 7465  one.authenticate
+00001250: 5f77 6974 685f 6b65 793a 3231 395d 205b  _with_key:219] [
+00001260: 494e 464f 5d3a 2041 7574 6865 6e74 6963  INFO]: Authentic
+00001270: 6174 6564 210a 4e6f 7465 3a20 7468 6520  ated!.Note: the 
+00001280: 6b65 7920 6973 2076 616c 6964 2066 6f72  key is valid for
+00001290: 2074 776f 2064 6179 732c 2061 6674 6572   two days, after
+000012a0: 2077 6869 6368 2061 206e 6577 206b 6579   which a new key
+000012b0: 206e 6565 6473 2074 6f20 6265 2067 656e   needs to be gen
+000012c0: 6572 6174 6564 2e20 200a 0a23 2320 6c6f  erated.  ..## lo
+000012d0: 676f 7574 0a4c 6f67 6f75 7420 6f66 2043  gout.Logout of C
+000012e0: 4954 524f 532e 0a0a 6578 616d 706c 653a  ITROS...example:
+000012f0: 0a0a 2020 2020 726f 7340 7368 616c 6576  ..    ros@shalev
+00001300: 2d49 6e73 7069 726f 6e2d 3135 2d35 3531  -Inspiron-15-551
+00001310: 303a 2f77 6f72 6b73 7061 6365 732f 6361  0:/workspaces/ca
+00001320: 6e6e 6f6e 2420 6369 7472 6f73 206c 6f67  nnon$ citros log
+00001330: 6f75 740a 2020 2020 5573 6572 206c 6f67  out.    User log
+00001340: 6765 6420 6f75 742e 0a23 2320 7379 6e63  ged out..## sync
+00001350: 0a53 796e 6320 7468 6520 726f 7320 7072  .Sync the ros pr
+00001360: 6f6a 6563 7420 746f 2063 6974 726f 732e  oject to citros.
+00001370: 0a0a 5468 6973 2063 6f6d 6d61 6e64 2077  ..This command w
+00001380: 696c 6c20 7061 7273 6520 796f 7572 2052  ill parse your R
+00001390: 4f53 3220 7072 6f6a 6563 742c 2065 7874  OS2 project, ext
+000013a0: 7261 6374 2074 6865 206e 616d 6573 206f  ract the names o
+000013b0: 6620 616c 6c20 7468 6520 7061 636b 6167  f all the packag
+000013c0: 6573 2c20 0a6e 6f64 6573 2c20 7061 7261  es, .nodes, para
+000013d0: 6d65 7465 7273 2061 6e64 206c 6175 6e63  meters and launc
+000013e0: 6820 6669 6c65 7320 2861 6e64 2073 6f6d  h files (and som
+000013f0: 6520 6f74 6865 7220 6d65 7461 6461 7461  e other metadata
+00001400: 292c 200a 6173 7369 676e 2065 6163 6820  ), .assign each 
+00001410: 6f66 2074 6865 6d20 6120 5549 4420 616e  of them a UID an
+00001420: 6420 7570 6c6f 6164 2074 6865 6d20 746f  d upload them to
+00001430: 2074 6865 2063 6974 726f 7320 6461 7461   the citros data
+00001440: 6261 7365 2e0a 0a65 7861 6d70 6c65 3a0a  base...example:.
+00001450: 2020 2020 0a20 2020 2072 6f73 4073 6861      .    ros@sha
+00001460: 6c65 762d 496e 7370 6972 6f6e 2d31 352d  lev-Inspiron-15-
+00001470: 3535 3130 3a2f 776f 726b 7370 6163 6573  5510:/workspaces
+00001480: 2f6d 6173 735f 7370 7269 6e67 5f64 756d  /mass_spring_dum
+00001490: 7065 7224 2063 6974 726f 7320 7379 6e63  per$ citros sync
+000014a0: 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d 2d2d  .    -----------
+000014b0: 2d2d 2d2d 2d2d 2d2d 7379 6e63 5f70 726f  --------sync_pro
+000014c0: 6a65 6374 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ject------------
+000014d0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2e2e 2e0a  -------.    ....
+000014e0: 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d      ------------
+000014f0: 2d2d 2d2d 2d2d 2d2d 2d2d 444f 4e45 2d2d  ----------DONE--
+00001500: 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d 2d2d  ----------------
+00001510: 2d2d 2d2d 2d2d 0a0a 4966 2074 6865 7265  ------..If there
+00001520: 2077 6572 6520 6e6f 2063 6861 6e67 6573   were no changes
+00001530: 2073 696e 6365 2074 6865 206c 6173 7420   since the last 
+00001540: 7379 6e63 2c20 7468 6520 7379 6e63 2069  sync, the sync i
+00001550: 7320 756e 6e65 6365 7373 6172 793a 0a0a  s unnecessary:..
+00001560: 2020 2020 726f 7340 7368 616c 6576 2d49      ros@shalev-I
+00001570: 6e73 7069 726f 6e2d 3135 2d35 3531 303a  nspiron-15-5510:
+00001580: 2f77 6f72 6b73 7061 6365 732f 6d61 7373  /workspaces/mass
+00001590: 5f73 7072 696e 675f 6475 6d70 6572 2420  _spring_dumper$ 
+000015a0: 6369 7472 6f73 2073 796e 630a 2020 2020  citros sync.    
+000015b0: 7072 6f6a 6563 7420 616c 7265 6164 7920  project already 
+000015c0: 7379 6e63 6865 642e 0a0a 4966 2074 6869  synched...If thi
+000015d0: 7320 7761 7320 796f 7572 2066 6972 7374  s was your first
+000015e0: 2074 696d 6520 7275 6e6e 696e 6720 7379   time running sy
+000015f0: 6e63 206f 6e20 7468 6973 2070 726f 6a65  nc on this proje
+00001600: 6374 2c20 796f 7520 6361 6e20 6f70 656e  ct, you can open
+00001610: 2079 6f75 7220 6661 766f 7269 7465 2062   your favorite b
+00001620: 726f 7773 6572 2061 6e64 206e 6176 6967  rowser and navig
+00001630: 6174 6520 746f 205b 6369 7472 6f73 2e69  ate to [citros.i
+00001640: 6f5d 2863 6974 726f 732e 696f 2920 616e  o](citros.io) an
+00001650: 6420 6c6f 6720 696e 2c20 616e 6420 756e  d log in, and un
+00001660: 6465 7220 7468 6520 7072 6f6a 6563 7420  der the project 
+00001670: 6c69 7374 2079 6f75 276c 6c20 7365 6520  list you'll see 
+00001680: 6120 6e65 7720 6974 656d 2066 6f72 2079  a new item for y
+00001690: 6f75 7220 7072 6f6a 6563 7420 6861 7320  our project has 
+000016a0: 6265 656e 2061 6464 6564 2074 6f20 7468  been added to th
+000016b0: 6520 6c69 7374 3a0a 215b 7072 6f6a 6563  e list:.![projec
+000016c0: 7420 6c69 7374 5d28 696d 672f 7072 6f6a  t list](img/proj
+000016d0: 5f6c 6973 742e 706e 6720 2270 726f 6a65  _list.png "proje
+000016e0: 6374 206c 6973 7422 290a 0a0a 2323 2320  ct list")...### 
+000016f0: 7061 7261 6d65 7465 7273 3a0a 7061 7261  parameters:.para
+00001700: 6d65 7465 727c 6465 7363 7269 7074 696f  meter|descriptio
+00001710: 6e0a 7c2d 2d7c 2d2d 7c0a 7c60 2d64 6972  n.|--|--|.|`-dir
+00001720: 6020 3c66 6f6c 6465 725f 6e61 6d65 3e20  ` <folder_name> 
+00001730: 7c20 5468 6520 776f 726b 696e 6720 6469  | The working di
+00001740: 7265 6374 6f72 7920 6f66 2074 6865 2070  rectory of the p
+00001750: 726f 6a65 6374 2e20 4465 6661 756c 7473  roject. Defaults
+00001760: 2074 6f20 222e 222e 7c0a 7c60 2d6e 616d   to ".".|.|`-nam
+00001770: 6560 203c 7072 6f6a 5f6e 616d 653e 207c  e` <proj_name> |
+00001780: 2054 6865 206e 616d 6520 6f66 2074 6865   The name of the
+00001790: 2070 726f 6a65 6374 2e20 4465 6661 756c   project. Defaul
+000017a0: 7473 2074 6f20 7468 6520 6c61 7374 2066  ts to the last f
+000017b0: 6f6c 6465 7220 696e 2074 6865 2070 6174  older in the pat
+000017c0: 6820 6f66 202a 6469 722a 7c0a 7c60 2d77  h of *dir*|.|`-w
+000017d0: 602c 2060 2d77 7360 203c 776f 726b 7370  `, `-ws` <worksp
+000017e0: 6163 655f 6e61 6d65 3e20 7c20 5468 6520  ace_name> | The 
+000017f0: 6e61 6d65 206f 6620 6120 776f 726b 7370  name of a worksp
+00001800: 6163 6520 696e 7369 6465 2074 6865 2070  ace inside the p
+00001810: 726f 6a65 6374 2064 6972 6563 746f 7279  roject directory
+00001820: 2e20 4d61 7920 6265 2075 7365 6420 6d75  . May be used mu
+00001830: 6c74 6970 6c65 2074 696d 6573 2066 6f72  ltiple times for
+00001840: 206d 756c 7469 706c 6520 776f 726b 7370   multiple worksp
+00001850: 6163 6573 2e20 4465 6661 756c 7473 2074  aces. Defaults t
+00001860: 6f20 2222 2028 6e61 6d65 6c79 2c20 6e6f  o "" (namely, no
+00001870: 2077 6f72 6b73 7061 6365 2c20 7061 636b   workspace, pack
+00001880: 6167 6520 666f 6c64 6572 7320 6172 6520  age folders are 
+00001890: 6469 7265 6374 6c79 2075 6e64 6572 2074  directly under t
+000018a0: 6865 2070 726f 6a65 6374 2066 6f6c 6465  he project folde
+000018b0: 722e 2044 6566 6175 6c74 2069 7320 7573  r. Default is us
+000018c0: 6564 2077 6865 7468 6572 2074 6869 7320  ed whether this 
+000018d0: 7061 7261 6d65 7465 7220 6973 2073 7065  parameter is spe
+000018e0: 6369 6669 6564 206f 7220 6e6f 7420 2d20  cified or not - 
+000018f0: 6164 6469 7469 6f6e 616c 206e 616d 6573  additional names
+00001900: 7061 6365 7320 6172 6520 6164 6465 642c  paces are added,
+00001910: 2062 7574 2064 6f20 6e6f 7420 6f76 6572   but do not over
+00001920: 7772 6974 6520 6974 292e 207c 0a0a 2323  write it). |..##
+00001930: 2070 6172 616d 730a 6578 7065 7269 6d65   params.experime
+00001940: 6e74 616c 2e0a 0a67 656e 6572 6174 6520  ntal...generate 
+00001950: 7061 7261 6d65 7465 7273 2066 6f72 2074  parameters for t
+00001960: 6865 2070 726f 6a65 6374 0a23 2320 7275  he project.## ru
+00001970: 6e5f 7369 6d75 6c61 7469 6f6e 0a43 7265  n_simulation.Cre
+00001980: 6174 6520 6120 6e65 7720 6261 7463 6820  ate a new batch 
+00001990: 6f66 2073 696d 756c 6174 696f 6e20 7275  of simulation ru
+000019a0: 6e73 2066 6f72 2079 6f75 7220 7072 6f6a  ns for your proj
+000019b0: 6563 7420 616e 6420 7275 6e20 6974 206c  ect and run it l
+000019c0: 6f63 616c 6c79 2e0a 0a23 2323 2070 7265  ocally...### pre
+000019d0: 7265 7175 6973 6974 6573 3a0a 5468 6520  requisites:.The 
+000019e0: 7072 6f6a 6563 7420 6861 7320 6265 656e  project has been
+000019f0: 2062 7569 6c74 2c20 736f 7572 6365 6420   built, sourced 
+00001a00: 616e 6420 6073 796e 6360 6564 2077 6974  and `sync`ed wit
+00001a10: 6820 6369 7472 6f73 2c20 652e 672e 3a0a  h citros, e.g.:.
+00001a20: 2020 2020 0a20 2020 2063 6f6c 636f 6e20      .    colcon 
+00001a30: 6275 696c 640a 2020 2020 736f 7572 6365  build.    source
+00001a40: 2069 6e73 7461 6c6c 2f6c 6f63 616c 5f73   install/local_s
+00001a50: 6574 7570 2e62 6173 680a 2020 2020 6369  etup.bash.    ci
+00001a60: 7472 6f73 2073 796e 630a 0a49 6e20 7468  tros sync..In th
+00001a70: 6520 6369 7472 6f73 2067 7569 2c20 6e61  e citros gui, na
+00001a80: 7669 6761 7465 2074 6f20 796f 7572 2070  vigate to your p
+00001a90: 726f 6a65 6374 2062 7920 636c 6963 6b69  roject by clicki
+00001aa0: 6e67 2074 6865 2074 6872 6565 2076 6572  ng the three ver
+00001ab0: 7469 6361 6c20 646f 7473 206f 6e20 7468  tical dots on th
+00001ac0: 6520 7269 6768 7420 7369 6465 206f 6620  e right side of 
+00001ad0: 6f66 2079 6f75 7220 7072 6f6a 6563 7427  of your project'
+00001ae0: 7320 726f 7720 696e 2074 6865 2070 726f  s row in the pro
+00001af0: 6a65 6374 206c 6973 7420 616e 6420 7365  ject list and se
+00001b00: 6c65 6374 2060 6e61 7669 6761 7465 603a  lect `navigate`:
+00001b10: 200a 215b 6e61 765f 7072 6f6a 5d28 696d   .![nav_proj](im
+00001b20: 672f 6e61 765f 7072 6f6a 2e70 6e67 2022  g/nav_proj.png "
+00001b30: 6e61 7669 6761 7465 2074 6f20 7072 6f6a  navigate to proj
+00001b40: 6563 7422 2920 0a0a 7768 6963 6820 7769  ect") ..which wi
+00001b50: 6c6c 2074 616b 6520 796f 7520 746f 2074  ll take you to t
+00001b60: 6865 2070 726f 6a65 6374 2773 2044 6574  he project's Det
+00001b70: 6169 6c73 2070 6167 652e 200a 0a54 6865  ails page. ..The
+00001b80: 7265 2c20 636c 6963 6b20 7468 6520 6053  re, click the `S
+00001b90: 696d 756c 6174 696f 6e20 5365 7475 7060  imulation Setup`
+00001ba0: 2074 6162 3a0a 215b 7369 6d5f 7365 7475   tab:.![sim_setu
+00001bb0: 705d 2869 6d67 2f73 696d 5f73 6574 7570  p](img/sim_setup
+00001bc0: 2e70 6e67 2022 7369 6d75 6c61 7469 6f6e  .png "simulation
+00001bd0: 2073 6574 7570 2229 0a0a 616e 6420 636c   setup")..and cl
+00001be0: 6963 6b20 6f6e 2060 6e65 7760 2e0a 0a46  ick on `new`...F
+00001bf0: 696c 6c20 696e 2061 6e79 2072 656c 6576  ill in any relev
+00001c00: 616e 7420 6465 7461 696c 7320 666f 7220  ant details for 
+00001c10: 7468 6520 6e65 7720 7369 6d75 6c61 7469  the new simulati
+00001c20: 6f6e 2061 6e64 2073 6176 653a 0a21 5b73  on and save:.![s
+00001c30: 6176 655f 6e65 775f 7369 6d5d 2869 6d67  ave_new_sim](img
+00001c40: 2f73 6176 655f 6e65 775f 7369 6d2e 706e  /save_new_sim.pn
+00001c50: 6720 2273 6176 6520 6e65 7720 7369 6d75  g "save new simu
+00001c60: 6c61 7469 6f6e 2229 0a0a 4e6f 7720 636c  lation")..Now cl
+00001c70: 6963 6b20 6f6e 2060 5275 6e20 5369 6d75  ick on `Run Simu
+00001c80: 6c61 7469 6f6e 204c 6f63 616c 6c79 603a  lation Locally`:
+00001c90: 0a21 5b72 756e 5f73 696d 5f6c 6f63 5d28  .![run_sim_loc](
+00001ca0: 696d 672f 7275 6e5f 7369 6d5f 6c6f 632e  img/run_sim_loc.
+00001cb0: 706e 6720 2272 756e 2073 696d 756c 6174  png "run simulat
+00001cc0: 696f 6e20 6c6f 6361 6c6c 7922 290a 0a61  ion locally")..a
+00001cd0: 6e64 2069 6e20 7468 6520 706f 702d 7570  nd in the pop-up
+00001ce0: 2074 6861 7420 636f 6d65 7320 7570 2c20   that comes up, 
+00001cf0: 636f 7079 2074 6865 2073 696d 756c 6174  copy the simulat
+00001d00: 696f 6e20 6964 2074 6861 7420 7761 7320  ion id that was 
+00001d10: 6765 6e65 7261 7465 643a 0a21 5b63 6f70  generated:.![cop
+00001d20: 795f 7369 6d5f 6964 5d28 696d 672f 636f  y_sim_id](img/co
+00001d30: 7079 5f73 696d 5f69 642e 706e 6720 2263  py_sim_id.png "c
+00001d40: 6f70 7920 7468 6520 7369 6d75 6c61 7469  opy the simulati
+00001d50: 6f6e 2069 6422 290a 0a61 6e64 206e 6f77  on id")..and now
+00001d60: 2c20 6669 6e61 6c6c 792c 2069 6e20 7468  , finally, in th
+00001d70: 6520 636f 6d6d 616e 642d 6c69 6e65 2c20  e command-line, 
+00001d80: 7275 6e0a 0a20 2020 2063 6974 726f 7320  run..    citros 
+00001d90: 7275 6e5f 7369 6d75 6c61 7469 6f6e 203c  run_simulation <
+00001da0: 7369 6d20 6964 3e20 3c72 6570 6574 6974  sim id> <repetit
+00001db0: 696f 6e73 3e0a 7768 6572 6520 603c 7369  ions>.where `<si
+00001dc0: 6d5f 6964 3e60 2069 7320 7468 6520 6964  m_id>` is the id
+00001dd0: 2079 6f75 206a 7573 7420 636f 7069 6564   you just copied
+00001de0: 2c20 616e 6420 603c 7265 7065 7469 7469  , and `<repetiti
+00001df0: 6f6e 733e 6020 6973 206e 756d 6265 7220  ons>` is number 
+00001e00: 6f66 2073 696d 756c 6174 696f 6e20 7275  of simulation ru
+00001e10: 6e73 2074 6861 7420 7769 6c6c 2072 756e  ns that will run
+00001e20: 2e20 4578 616d 706c 653a 0a20 2020 200a  . Example:.    .
+00001e30: 2020 2020 6369 7472 6f73 2072 756e 5f73      citros run_s
+00001e40: 696d 756c 6174 696f 6e20 6366 3162 3436  imulation cf1b46
+00001e50: 3633 2d61 3665 332d 3439 6264 2d39 3665  63-a6e3-49bd-96e
+00001e60: 352d 6263 3437 6362 3564 3533 3236 2031  5-bc47cb5d5326 1
+00001e70: 0a20 2020 202e 2e2e 0a20 2020 202d 202d  .    ....    - -
+00001e80: 2046 696e 6973 6865 6420 7369 6d75 6c61   Finished simula
+00001e90: 7469 6f6e 2073 6964 203d 205b 305d 2077  tion sid = [0] w
+00001ea0: 6974 6820 7265 7475 726e 2063 6f64 6520  ith return code 
+00001eb0: 5b31 5d2e 0a20 2020 202d 2046 696e 6973  [1]..    - Finis
+00001ec0: 6865 6420 5b61 3762 3138 3864 642d 3734  hed [a7b188dd-74
+00001ed0: 6262 2d34 6465 392d 6233 3836 2d39 6133  bb-4de9-b386-9a3
+00001ee0: 3034 3839 3635 3263 625d 2062 6174 6368  0489652cb] batch
+00001ef0: 2e0a 0a23 2320 7275 6e0a 5275 6e20 6120  ...## run.Run a 
+00001f00: 7072 6576 696f 7573 6c79 2063 7265 6174  previously creat
+00001f10: 6564 2062 6174 6368 206c 6f63 616c 6c79  ed batch locally
+00001f20: 2e20 5468 6973 2063 6f6d 6d61 6e64 2069  . This command i
+00001f30: 7320 7573 6566 756c 2077 6865 6e20 796f  s useful when yo
+00001f40: 7527 6420 6c69 6b65 2074 6f20 6c6f 6361  u'd like to loca
+00001f50: 6c6c 7920 7265 7275 6e20 6120 6261 7463  lly rerun a batc
+00001f60: 6820 7468 6174 2077 6173 2061 6c72 6561  h that was alrea
+00001f70: 6479 2072 756e 2028 6569 7468 6572 206c  dy run (either l
+00001f80: 6f63 616c 6c79 206f 7220 6f6e 2074 6865  ocally or on the
+00001f90: 2063 6c75 7374 6572 292e 0a0a 4166 7465   cluster)...Afte
+00001fa0: 7220 796f 7527 7665 206c 6f67 6765 6420  r you've logged 
+00001fb0: 696e 746f 205b 6369 7472 6f73 2e69 6f5d  into [citros.io]
+00001fc0: 2863 6974 726f 732e 696f 292c 2063 6c69  (citros.io), cli
+00001fd0: 636b 2074 6865 2060 5369 6d75 6c61 7469  ck the `Simulati
+00001fe0: 6f6e 2052 756e 7360 2074 6162 3a0a 215b  on Runs` tab:.![
+00001ff0: 7369 6d5f 7275 6e73 5d28 696d 672f 7369  sim_runs](img/si
+00002000: 6d5f 7275 6e73 2e70 6e67 2022 5369 6d75  m_runs.png "Simu
+00002010: 6c61 7469 6f6e 2052 756e 7322 2920 200a  lation Runs")  .
+00002020: 0a61 6e64 206f 6e20 7468 6520 6c69 7374  .and on the list
+00002030: 2069 7465 6d20 636f 7272 6573 706f 6e64   item correspond
+00002040: 696e 6720 746f 2074 6865 2062 6174 6368  ing to the batch
+00002050: 2079 6f75 2764 206c 696b 6520 746f 2072   you'd like to r
+00002060: 756e 2c20 636c 6963 6b20 7468 6520 7468  un, click the th
+00002070: 7265 6520 7665 7274 6963 616c 2064 6f74  ree vertical dot
+00002080: 7320 6f6e 2074 6865 2072 6967 6874 2061  s on the right a
+00002090: 6e64 2074 6865 6e20 636c 6963 6b20 6e61  nd then click na
+000020a0: 7669 6761 7465 206f 6e20 7468 6520 736d  vigate on the sm
+000020b0: 616c 6c20 636f 6e74 6578 7420 6d65 6e75  all context menu
+000020c0: 2074 6861 7420 6f70 656e 732e 2054 6869   that opens. Thi
+000020d0: 7320 7769 6c6c 2074 616b 6520 796f 7520  s will take you 
+000020e0: 746f 2074 6865 206c 6973 7420 6f66 2073  to the list of s
+000020f0: 696d 756c 6174 696f 6e20 7275 6e73 2066  imulation runs f
+00002100: 6f72 2074 6865 2062 6174 6368 2079 6f75  or the batch you
+00002110: 2073 656c 6563 7465 643a 0a21 5b62 6174   selected:.![bat
+00002120: 6368 5f72 756e 735d 2869 6d67 2f62 6174  ch_runs](img/bat
+00002130: 6368 5f72 756e 732e 706e 6720 2242 6174  ch_runs.png "Bat
+00002140: 6368 2052 756e 7322 290a 0a75 6e64 6572  ch Runs")..under
+00002150: 2074 6865 2060 5369 6d75 6c61 7469 6f6e   the `Simulation
+00002160: 2052 756e 7360 2068 6561 6469 6e67 2c20   Runs` heading, 
+00002170: 796f 7520 6172 6520 7072 6573 656e 7465  you are presente
+00002180: 6420 7769 7468 2073 6f6d 6520 6d65 7461  d with some meta
+00002190: 6461 7461 2066 6f72 2074 6869 7320 6261  data for this ba
+000021a0: 7463 6820 696e 2074 6865 2066 6f6c 6c6f  tch in the follo
+000021b0: 7769 6e67 2066 6f72 6d61 743a 0a0a 2020  wing format:..  
+000021c0: 2020 4461 7368 626f 6172 6420 2d20 5072    Dashboard - Pr
+000021d0: 6f6a 6563 744c 6973 7420 2d20 3c70 726f  ojectList - <pro
+000021e0: 6a65 6374 5f6e 616d 653e 202d 203c 7369  ject_name> - <si
+000021f0: 6d75 6c61 7469 6f6e 5f69 643e 202d 203c  mulation_id> - <
+00002200: 6261 7463 685f 6964 3e0a 0a63 6f70 7920  batch_id>..copy 
+00002210: 7468 6520 7468 6520 6261 7463 6820 6964  the the batch id
+00002220: 2c20 616e 6420 696e 2074 6865 2063 6f6d  , and in the com
+00002230: 6d61 6e64 2d6c 696e 653a 0a0a 2020 2020  mand-line:..    
+00002240: 6369 7472 6f73 2072 756e 203c 6261 7463  citros run <batc
+00002250: 685f 6964 3e20 3c73 696d 5f72 756e 5f69  h_id> <sim_run_i
+00002260: 643e 0a0a 7768 6572 6520 603c 7369 6d5f  d>..where `<sim_
+00002270: 7275 6e5f 6964 3e60 2069 7320 7468 6520  run_id>` is the 
+00002280: 287a 6572 6f2d 6261 7365 6429 2072 756e  (zero-based) run
+00002290: 2069 6e64 6578 2028 6e6f 7420 746f 2062   index (not to b
+000022a0: 6520 636f 6e66 7573 6564 2077 6974 6820  e confused with 
+000022b0: 6073 696d 756c 6174 696f 6e5f 6964 6029  `simulation_id`)
+000022c0: 2e20 4966 2069 7420 6973 206e 6f74 2073  . If it is not s
+000022d0: 7065 6369 6669 6564 2c20 7468 6520 656e  pecified, the en
+000022e0: 7469 7265 2062 6174 6368 2069 7320 6578  tire batch is ex
+000022f0: 6563 7574 6564 2e20 4578 616d 706c 653a  ecuted. Example:
+00002300: 0a0a 2020 2020 6369 7472 6f73 2072 756e  ..    citros run
+00002310: 2062 6431 3735 6139 332d 3432 3334 2d34   bd175a93-4234-4
+00002320: 3234 342d 3934 3264 2d30 6232 6139 3832  244-942d-0b2a982
+00002330: 6334 3635 6620 300a 0a23 2320 7570 6c6f  c465f 0..## uplo
+00002340: 6164 5f62 6167 0a65 7870 6572 696d 656e  ad_bag.experimen
+00002350: 7461 6c2e 0a0a 7570 6c6f 6164 2062 6167  tal...upload bag
+00002360: 2074 6f20 6369 7472 6f73 2e0a 2323 2073   to citros..## s
+00002370: 7472 6573 730a 6578 7065 7269 6d65 6e74  tress.experiment
+00002380: 616c 2e0a 0a73 7472 6573 7320 7465 7374  al...stress test
+00002390: 2074 6865 2073 7973 7465 6d2e 0a23 2320   the system..## 
+000023a0: 646f 636b 6572 2d6c 6f67 696e 0a6c 6f67  docker-login.log
+000023b0: 696e 2074 6f20 646f 636b 6572 2d68 7562  in to docker-hub
+000023c0: 0a23 2320 646f 636b 6572 0a42 7569 6c64  .## docker.Build
+000023d0: 7320 7468 6520 7072 6f6a 6563 742e 0a    s the project..
```

### Comparing `citros-23.22.2/bin/citros` & `citros-23.23.1/bin/citros`

 * *Files 20% similar despite different names*

```diff
@@ -3,163 +3,254 @@
 from citros import Citros, __version__ as citros_version
 import argparse
 from getpass import getpass
 import os
 import sys        
 import traceback
 from decouple import config
-import json
+
+from InquirerPy import prompt
+from prompt_toolkit.validation import Validator, ValidationError
+
+from launch import LaunchService 
+from citros.launches import generate_launch_description  
+
+# in seconds
+DEFAULT_SIMULATION_TIMEOUT = 10*60
+
+
+class NumberValidator(Validator):
+    """
+    small helper class for validating user input during an interactive session.
+    """
+    def validate(self, document):
+        try:
+            int(document.text)
+        except ValueError:
+            raise ValidationError(message="Please enter a number",
+                                  cursor_position=len(document.text))
+
+
 
 def print_citros():
     print ("""
 ==============================================
  ██████╗██╗████████╗██████╗  ██████╗ ███████╗
 ██╔════╝██║╚══██╔══╝██╔══██╗██╔═══██╗██╔════╝
 ██║     ██║   ██║   ██████╔╝██║   ██║███████╗
 ██║     ██║   ██║   ██╔══██╗██║   ██║╚════██║
 ╚██████╗██║   ██║   ██║  ██║╚██████╔╝███████║
  ╚═════╝╚═╝   ╚═╝   ╚═╝  ╚═╝ ╚═════╝ ╚══════╝
 ==============================================
 CITROS CLI tool for interaction with the CITROS system. V[{citros_version}]
     """)
 
+
+def generate_question(type, name, message, choices=None, validator=None, filter=None):
+    if type not in ["list", "raw_list", "expand", "confirm",
+                    "check_box", "input", "password", "editor"]:
+        print("question type not supported.")
+        return {}
+
+    if type == "list":
+        if not choices:
+            print("Nothing to choose from.")
+            return {}
+        return {
+            "type": type,
+            "name": name,
+            "message": message,
+            "choices": choices
+        }
+    elif type == "input":
+        return {
+            f"type":type,
+            f"name":name,
+            f"message": message,
+            f"validate": validator,
+            f"filter": filter
+        }
+    else:
+        raise NotImplementedError()
+
+
 def login(args, argv): 
     with Citros() as citros:       
-        username, password = args.username, args.password        
+        username, password, key = args.username, args.password, args.key
+
+        if key:
+            success = citros.authenticate_with_key(key)
+            if success:
+                pass
+                #print("User authenticated.")
+            return
+
         if not citros.isAuthenticated() and (args.username is None or args.password is None):        
             username = input("email: ")        
             password = getpass()            
         resp = citros.login(username, password) 
         if resp:
             print("User logged in.")
         else:
             print("Failed to log in. Please try again.")
 
-
-def authenticate(args, argv):
-    with Citros() as citros:   
-        key = args.key
-        if not key:
-            print("Please provide a valid key.")
-        else:
-            try:
-                success = citros.authenticate_with_key(key)
-                if success:
-                    print("Authenticated!")
-            except Exception as e:
-                print(f"\nAuthentication failed.\n{e}")
-    
     
 def logout(args, argv):
     with Citros() as citros: 
         citros.logout() 
         print("User logged out.")
 
 
 def sync_project(args, argv):             
     with Citros() as citros:  
         if not citros.isAuthenticated():
             print("sync_project: please log in first!")
             return
+        
         project_data = citros.parser_ros2.parse(args.dir, args.name, args.ws)
-        # print("sync_project:project: ", json.dumps(project_data, indent=2))
         citros.integration.sync_project(project_data)
 
 
-def run_simulation(args, argv):    
-    print_citros()       
+def list_project(args, argv):
+    with Citros() as citros:  
+        if not citros.isAuthenticated():
+            print("list_project: please log in first!")
+            return
         
-    with Citros() as citros:    
-        if args.key:
-            loggedin = citros.authenticate_with_key(args.key)
+        if args.names:
+            for proj in citros.query_projects():
+                print(proj)
+        else:
+            ids, names = citros.query_simulations(args.project)
+            for id,name in zip(ids,names):
+                print(f"{name}\t{id}")
+
+
+def run(args, argv):
+    """
+    :param args.simulation_id:
+    :param args.batch_id:
+    :param args.run_id:
+    :param args.remote:
+    :param args.timeout:
+    :param args.key:
+    :param args.completions:
+    """
+    print_citros()       
+
+    sim_id, batch_id, run_id = args.simulation_id, args.batch_id, args.run_id
+    remote, timeout, key, completions = args.remote, args.timeout, args.key, args.completions
+
+    with Citros() as citros:
+        if key:
+            loggedin = citros.authenticate_with_key(key)
             if not loggedin:
-                sys.exit("run_ros2_project.authenticate_with_key: please log in first!") 
+                sys.exit("run.authenticate_with_key: please log in first!") 
         
         if not citros.isAuthenticated():
-            sys.exit("run_simulation: please log in first!")      
+            sys.exit("run: please log in first!")
+
+        if batch_id:
+            run_simulation_by_batch(citros, batch_id, run_id, timeout)
+        elif sim_id:
+            run_simulation(citros, sim_id, completions, timeout, remote)
+        else:
+            proj_name = os.path.abspath(".").split("/")[-1]
+            run_simulation_interactively(citros, proj_name, completions, timeout, remote)
+
+        # sys.exit(0)
             
-        # create new batch for this simulation
-        batch_run_id = citros.batch.create_manual_batch(args.simulation_id, args.completions)
-        print(f"created new batch_run_id: {batch_run_id}")
-        batch = citros.batch.get_batch(batch_run_id)
-        run_batch(batch, batch_run_id, 10*60)
-    sys.exit(0)
+
+def run_simulation_interactively(citros : Citros, proj_name, completions, timeout, remote):
+    proj_names = citros.query_projects()
+    if proj_name in proj_names:
+        sim_ids, sim_names = citros.query_simulations(proj_name)
+
+        if not sim_names:
+            print(f"There are currently no simulations associated with project {proj_name}. \
+                    Please login to citros.io and create at least one simulation for your project.")
+            return
+        
+        names_and_ids = [name + '   ' + id for name, id in zip(sim_names, sim_ids)]
+        sim_name_and_id_q = generate_question("list", "sim_name_and_id", 
+                                              "Please choose the simulation you wish to run", names_and_ids )
+        #completions_q = generate_question("input", "completions", "Please enter number of completions:",
+        #                                  NumberValidator, lambda val: int(val))
+        answers = prompt([sim_name_and_id_q])  # use default style
+        sim_name_and_id = answers.get("sim_name_and_id")
+        idx = names_and_ids.index(sim_name_and_id)
+
+        run_simulation(citros, sim_ids[idx], completions, timeout, remote)
+
+    else:
+        print(f"Your project `{proj_name}` is not known to citros. Please run `citros sync` first.")
+
+
+def run_simulation(citros : Citros, sim_id, completions, timeout, remote):      
+    # create a new batch for this simulation
+    isManual = not remote
+    where = "locally" if isManual else "on Citros cluster"
+    batch_id = citros.batch.create_manual_batch(sim_id, completions, isManual)
+    citros.log.info(f"created new batch_run_id: {batch_id}. Running {where}.")
+    if isManual:
+        batch = citros.batch.get_batch(batch_id)
+        run_batch(batch, batch_id, timeout)
     
     
 def run_batch(batch, batch_run_id, timeout):
     completions = 0
     try:
         completions = int(batch["batchRun"]["completions"])
     except Exception as e:
         print(e)
     print(f" + running batch [{batch_run_id}], repeating simulations: [{completions}]")
     for sid in range(0, completions):
         try:
-            run_simulation_run(batch_run_id, sid, timeout)                        
+            single_simulation_run(batch_run_id, sid, timeout)                        
             time.sleep(1)
         except Exception as e:
             print("------------------------")   
             print (e)
             traceback.print_exc()
             print("------------------------")
             continue
     print(f" - Finished [{batch_run_id}] batch.")    
 
 
-def run_simulation_run(batch_run_id, sid, timeout):    
-    print(f" + + running simulation [{sid}]")
-    from launch import LaunchService 
-    from citros.launches import generate_launch_description    
+def single_simulation_run(batch_id, sid, timeout):    
+    print(f" + + running simulation [{sid}]")  
     
-    # create a new instance so that a new logger will be created and mapped
-    # according to batch_run_id, simulation_run_id. Very inelegant.
+    # create a new instance of citros so that a new logger will be created 
+    # and mapped according to batch_id, simulation_run_id. Very inelegant.
     # TODO: find a simple way to map the loggers without instantiating Citros. 
-    with Citros(batch_run_id, sid) as citros:
+    with Citros(batch_id, sid) as citros:
         launch_description = generate_launch_description(citros, str(timeout))
         if launch_description is None:
             sys.exit(f'Couldn\'t run sid:[{sid}]. Something went wrong, probably with connection to CITROS. ')    
         #launch_service = LaunchService(debug=True)
         launch_service = LaunchService()
         launch_service.include_launch_description(launch_description)
         ret = launch_service.run()    
         print(f" - - Finished simulation sid = [{sid}] with return code [{ret}].")    
     
 
-def run_ros2_project(args, argv):  
-    """
-    args.batch_run_id
-    args.sid
-    args.timeout
-    """
-    print_citros()
-    
-    with Citros() as citros: 
-        if args.key:
-            logedin = citros.authenticate_with_key(args.key)
-            if not logedin:
-                sys.exit("run_ros2_project.authenticate_with_key: please log in first!")            
-            
-        if not citros.isAuthenticated():
-            sys.exit("run_ros2_project: please log in first!")             
-        
-        # k8s indexed batch job is passing the index with JOB_COMPLETION_INDEX env variable.
-        if args.sid == "JOB_COMPLETION_INDEX":
-            args.sid = config("JOB_COMPLETION_INDEX", "bad-value-from-k8s")
-            print(f"got JOB_COMPLETION_INDEX={args.sid} from k8s.")
-        
-        if (args.sid == ''):
-            # run batch... 
-            print(f"running batch [{args.batch_run_id}]")
-            batch = citros.batch.get_batch(args.batch_run_id)
-            run_batch(batch, args.batch_run_id, str(args.timeout))
-            sys.exit(0)        
-        
-        print("running simulation...")
-        run_simulation_run(args.batch_run_id, args.sid, str(args.timeout))
-    sys.exit(0)
+def run_simulation_by_batch(citros : Citros, batch_id, run_id, timeout):
+    # k8s indexed batch job is passing the index with JOB_COMPLETION_INDEX env variable.
+    if run_id == "JOB_COMPLETION_INDEX":
+        run_id = config("JOB_COMPLETION_INDEX", "bad-value-from-k8s")
+        print(f"got JOB_COMPLETION_INDEX={run_id} from k8s.")
+    
+    if (run_id == ''):
+        print(f"running batch [{batch_id}]")
+        batch = citros.batch.get_batch(batch_id)
+        run_batch(batch, batch_id, str(timeout))
+        return       
+    else:    
+        print(f"running a single simulation run from batch [{batch_id}]")
+        single_simulation_run(batch_id, run_id, str(timeout))
 
 
 # experimental:
 def load_params(args, argv):
     with Citros() as citros: 
         if not citros.isAuthenticated():
             print("load_params: please log in first!")
@@ -190,17 +281,14 @@
         
         # print( 'echo ' + google_access_token + ' | docker login -u oauth2accesstoken --password-stdin https://europe-west2-docker.pkg.dev')
         os.system('echo ' + google_access_token + ' | docker login -u oauth2accesstoken --password-stdin https://us-central1-docker.pkg.dev')                        
 
 
 def docker(args, argv):
     # TODO: login to docker first
-    # print(args, argv)
-    import os
-    # print('docker ' + ' '.join(argv))
     os.system('docker ' + ' '.join(argv))
 
 
 def stress_user_db(args, argv):
     """
     args.runs - how many query's to send,
     args.sleep - how much sleep between sends. 
@@ -214,15 +302,14 @@
         print(f"sending {args.runs} log messages.")
         for i in range(1, int(args.runs) + 1):
             # print(f"sending {i} message.")
             citros.events.creating("72311c81-5992-431a-9373-81aa2bdb3fe1", "2", "vova", "stress test", "")
             # citros.log.debug(f"{i} - sending message.")
             if float(args.sleep) > 0:
                 time.sleep(float(args.sleep))    
-        citros.close()
     print("Done.")    
 
 
 
 def main():    
     parser = argparse.ArgumentParser(
         prog='CITROS ROS parser',
@@ -250,95 +337,80 @@
     
     subparsers = parser.add_subparsers(title="commands", help="citros commands", dest='command', required=True)
 
     # -----------------------------------------
     build_parser = subparsers.add_parser("login", help="log in to citros")
     build_parser.add_argument("-username", default=None, help="username")
     build_parser.add_argument("-password", default=None, help="password")
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
+    build_parser.add_argument("-k", "--key", default=None, help="authentication key")
     build_parser.set_defaults(func=login)
     
     # -----------------------------------------
-    build_parser = subparsers.add_parser("authenticate", help="log in to citros using key")
-    build_parser.add_argument("key", help="The key provided by citros system.")
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
-    build_parser.set_defaults(func=authenticate)
-    
-    # -----------------------------------------
-    build_parser = subparsers.add_parser("logout", help="log out of the system")   
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api") 
+    build_parser = subparsers.add_parser("logout", help="log out of the system")
     build_parser.set_defaults(func=logout)
     
     # -----------------------------------------
     current_folder_name = os.path.abspath(".").split("/")[-1]
     
     build_parser = subparsers.add_parser("sync", help="sync the ros project to citros")
     build_parser.add_argument("-dir", default=".", help="The working dir of the project")
     build_parser.add_argument("-name", default=current_folder_name, help="The project name of the project")
     build_parser.add_argument('-w','--ws', action='append', default=[""], help='workspaces list')
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
-    
     build_parser.set_defaults(func=sync_project)
 
+    # -----------------------------------------
+    build_parser = subparsers.add_parser("list", help="lists project names, simulation IDs or batch IDs.")
+    build_parser.add_argument("-p", "--project", default=current_folder_name, help="The project name whose simulations ids will be printed.")
+    build_parser.add_argument("-n", "--names", action="store_true", help="if used, list all available project names.")
+    build_parser.set_defaults(func=list_project)
+
     # experimental
     # -----------------------------------------
     build_parser = subparsers.add_parser("params", help="generating parameters to the project")
     build_parser.add_argument("batch_run_id", help="Batch run id")
-    build_parser.add_argument("sid", help="simulation run id")    
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
+    build_parser.add_argument("sid", help="simulation run id")
     build_parser.set_defaults(func=load_params)
         
     # -----------------------------------------
-    # runs the [batch_run, simulation_run]
-    build_parser = subparsers.add_parser("run", help="run ros2 project")
-    build_parser.add_argument("batch_run_id", help="Batch run id")
-    build_parser.add_argument("sid", nargs='?', default='', help="simulation run id")    
-    build_parser.add_argument("-timeout", default=60*60, help="simulation timeout")    
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
-    build_parser.add_argument("--key", help="jwt ket of the user")
-    build_parser.set_defaults(func=run_ros2_project)
-    
-    # -----------------------------------------
-    build_parser = subparsers.add_parser("run_simulation", help="create new batch and run it")
-    build_parser.add_argument("simulation_id", help="Simulation run id")
-    build_parser.add_argument("completions", default=1, help="number of times to run the simulation")
-    build_parser.add_argument("-timeout", default=60*60, help="simulation timeout")
-    build_parser.add_argument("--key", help="jwt ket of the user")
-    build_parser.set_defaults(func=run_simulation)
+    build_parser = subparsers.add_parser("run", help="run a simulation")
+    #build_parser.add_argument("-n", "--name", default=current_folder_name, help="The project name of the project")
+    build_parser.add_argument("-s", "--simulation_id", nargs='?', default=None, help="Simulation id")
+    build_parser.add_argument("-b", "--batch_id", nargs='?', default=None, help="Batch id")
+    build_parser.add_argument("-i", "--run_id", nargs='?', default='', help="run id")
+    build_parser.add_argument("-c", "--completions", nargs='?', default=1, help="number of times to run the simulation")
+    build_parser.add_argument("-t", "--timeout", nargs='?', default=DEFAULT_SIMULATION_TIMEOUT, help="simulation timeout")
+    build_parser.add_argument("-k", "--key", nargs='?', default=None, help="jwt key of the user")
+    build_parser.add_argument("-r", "--remote", action='store_true', help="simulation timeout")
+    build_parser.set_defaults(func=run)
      
     # experimental
     # -----------------------------------------
-    # runs the [batch_run, simulation_run]
     build_parser = subparsers.add_parser("upload_bag", help="upload bag to citros")
     build_parser.add_argument("bag", help="bag file")
     build_parser.add_argument("batch_run_id", help="Batch run id")
-    build_parser.add_argument("sid", help="simulation run id")    
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")    
+    build_parser.add_argument("sid", help="simulation run id")  
     build_parser.set_defaults(func=upload_bag)
     
     # experimental
     # -----------------------------------------
-    # runs the [batch_run, simulation_run]
     build_parser = subparsers.add_parser("stress", help="stress test the system")
     build_parser.add_argument("--batch_run_id", help="Batch run id")
     build_parser.add_argument("--sid", help="simulation run id")
     build_parser.add_argument("--runs", default=100,help="how many runs to perform")
-    build_parser.add_argument("--sleep", default=0.0, help="how much sleep between runs")  
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")       
+    build_parser.add_argument("--sleep", default=0.0, help="how much sleep between runs")      
     build_parser.set_defaults(func=stress_user_db)
     
     # -----------------------------------------
     build_parser = subparsers.add_parser("docker-login", help="Builds the project")
     build_parser.set_defaults(func=docker_login)
     
     build_parser = subparsers.add_parser("docker", help="Builds the project")
     build_parser.add_argument("-d", default="Dockerfile", help="The docker to build")
-    build_parser.add_argument("--url", default="https://db.citros.dev:5555", help="entry point for citros gql api")
     build_parser.set_defaults(func=docker)
 
-    # args = parser.parse_args()
     args, argv = parser.parse_known_args()
     
     args.func(args, argv)     
 
+
 if __name__ == "__main__":
     main()
```

### Comparing `citros-23.22.2/citros/__init__.py` & `citros-23.23.1/citros/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/citros.py` & `citros-23.23.1/citros/citros.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,38 +1,46 @@
 import os
-import yaml
-## ENV
+
 from decouple import config
 import traceback
 import jwt
-import time
+import json
+import traceback
 
-## Postgres
-# import psycopg2
-# from psycopg2 import Error
 ## graphQL
 from gql import Client, gql
 from gql.transport.exceptions import TransportQueryError
 from gql.transport.requests import RequestsHTTPTransport
 
+import requests 
+
 from .citros_events import citros_events
 from .citros_integration import citros_integration
 from .citros_utils import citros_utils
 from .citros_batch import citros_batch
 from .citros_bag import citros_bag
 from .parsers import parser_ros2
 from .citros_params import citros_params
 from .logger import get_logger
 
 
 class Citros:
+    """
+    The Citros class implements the frontend of the Citros CLI.
+    It must instantiated within a `with` block in order to prevent 
+    resource leaks and unexpected behavior.
+    """
     def __init__(self, batch_run_id=None, simulation_run_id=None):    
-        # if self.init: # init only once. 
-        #     return
-        # self.init = True
+        """
+        Initialize Citros instance.
+
+        Args:
+        batch_run_id: An optional ID for a batch run.
+        simulation_run_id: An optional ID for a simulation run.
+        """
         
         self.CONFIG_DIR = ".citros"
                     
         self._user = None
         # do not access directly, only via get/set token.
         self._jwt_token = None
         
@@ -41,202 +49,264 @@
         self._token_changed = False
         
         # for logger
         self.batch_run_id = batch_run_id
         self.simulation_run_id = simulation_run_id    
         
         self.CITROS_DOMAIN = config("CITROS_DOMAIN", "https://citros.io")
-        print(f"--- using self.CITROS_DOMAIN = {self.CITROS_DOMAIN}")
+        # print(f"--- using self.CITROS_DOMAIN = {self.CITROS_DOMAIN}")
         
         self.CITROS_ENTRYPOINT = f"{self.CITROS_DOMAIN}/api/graphql"
         self.CITROS_LOGS = f"{self.CITROS_DOMAIN}/api/logs"        
         self.CITROS_GTOKEN = f"{self.CITROS_DOMAIN}/api/gtoken" 
         self.CITROS_HEALTH_CHECK = f"{self.CITROS_DOMAIN}/api/check" 
-        
-        
-        # TODO: fix this! how to make it beautiful?s
+          
         self.log = None
         self.listener = None
         self.log, self.listener = get_logger(__name__, self.sync_logs, self.batch_run_id, self.simulation_run_id)
         
-        
-        ########################################################################
-        ###     Citros components
-        ########################################################################
+        self._init_components()
+    
+
+    def _init_components(self):
         self.events = citros_events(self)        
         self.parser_ros2 = parser_ros2(self.log)
         self.integration = citros_integration(self)        
         self.params = citros_params(self)
         self.utils = citros_utils(self)
         self.bag = citros_bag(self)
         self.batch = citros_batch(self)
-    
+
+
+    def handle_exceptions(self, e):
+        """
+        Handles exceptions and logs them.
+
+        Args:
+        e: Exception to handle.
+        """
+        stack_trace = traceback.format_exception(type(e), e, e.__traceback__)
+        stack_trace_str = "".join(stack_trace)
+        self.log.exception(stack_trace_str)
+
 
     def __enter__(self):
+        """
+        Returns the Citros instance. This allows the class to be used in a `with` statement.
+        """
         return self
 
 
     def __exit__(self, exc_type, exc_val, exc_tb):
+        """
+        Stops the log listener and handles exceptions.
+
+        Args:
+        exc_type: The type of exception.
+        exc_val: The exception instance.
+        exc_tb: A traceback object encapsulating the call stack at the point 
+                where the exception originally occurred.
+        """
         if exc_type is not None:
-            # Handle the exception here...
-            pass
+            self.handle_exceptions(exc_val)
 
         # Stop the log listener in order to flush the queue.
         # If you don't call this before your application exits, there may 
         # be some records still left on the queue, which won't be processed.
-        self.listener.stop()
+        if self.listener:     
+            self.listener.stop()
 
 
-    def close(self):                
-        if self.listener:         
-            self.listener.stop()    
-                    
     def _remove_token(self):
+        """
+        Removes the JWT token.
+        """
         self._set_token(None)
-        
+
+
+    def _validate_token(self, token):
+        """
+        Validates the JWT token.
+
+        Args:
+        token: JWT token to validate.
+
+        Returns:
+        Boolean indicating if the token is valid.
+        """
+        # TODO: Implement token validation (may be None!)
+        return True
+
+
     def _set_token(self, jwt_token):
-        #TODO: check token validity
-        # print(f"jwt_token [{jwt_token}]")
-        if not jwt_token or jwt_token == '':
+        """
+        Sets the JWT token.
+
+        Args:
+        jwt_token: JWT token to set.
+        """
+        if not self._validate_token(jwt_token):
+            self.log.error("Invalid JWT token.")
+            return
+
+        if not jwt_token or jwt_token.strip() == '':
             self._jwt_token = None
             self._token_changed = True
             try:
                 os.remove(f"{self.CONFIG_DIR}/auth")
-                return
             except FileNotFoundError as e:
-                return # its ok that there is no file.                
+                pass # its ok that there is no file.                
             except Exception as e:
-                self.log.exception(e)       
-                traceback.print_exc()
+                self.handle_exceptions(e)
             return    
             
-        # create DIR if not exists
         if not os.path.isdir(self.CONFIG_DIR):
             os.makedirs(self.CONFIG_DIR)
             
         try:
             with open(f"{self.CONFIG_DIR}/auth", mode='w') as file:            
-                file.write(jwt_token)                  
-        except FileNotFoundError as e:
-            self.log.exception(e)
-            traceback.print_exc()
+                file.write(jwt_token)      
         except Exception as e:
-            self.log.exception(e)
-            traceback.print_exc()
+            self.handle_exceptions(e)
         finally:
             self._jwt_token = jwt_token
             self._token_changed = True                        
         
         return self._jwt_token
-    
+
+
     def _get_token(self):
+        """
+        Gets the JWT token.
+        """
         try:
             if self._jwt_token:
                 return self._jwt_token
             
             with open(f"{self.CONFIG_DIR}/auth", mode='r') as file:            
                 self._jwt_token = file.read()
                 self._token_changed = True
         except FileNotFoundError as e:
             # Key file wasn't found. assuming the user is not logged in...
             self._jwt_token = None
             return None
         except Exception as e:
-            self.log.exception(e)
-            traceback.print_exc()
+            self.handle_exceptions(e)
         
-        if self._jwt_token == '':
-            print("ERROR: self._jwt_token is empty, removing. ")
+        if not self._validate_token(self._jwt_token):
+            self.log.error("JWT token is invalid, removing.")
             self._remove_token()
-        # TODO: check token is valid. if not remove token!
+
         return self._jwt_token
     
-    ###########################
-    # Public
-    ###########################
-
+    ################################# Public #################################
+    
     def logout(self):
-        """Logs out of CiTROS
         """
-        #self.log.info("User logging out...")
-        #time.sleep(5) # wait till the PGHandler is done. TODO: fix this.
-
+        Logs out of CiTROS
+        """
         self._remove_token()
         self._user = None
         
     
     def isAuthenticated(self):
-        """returns the authentication status
+        """
+        returns the authentication status
 
         Returns:
             boolean: True if the user is logged in. 
         """        
         return self._get_token() is not None
-    
+
+
     def checkStatus(self):
+        """
+        Checks the current status of the user authentication
+
+        Returns:
+            boolean: True if the user is authenticated and health check passes. 
+        """ 
         if not self.isAuthenticated():
             print("User is not logged in. please log in first.")
             return False
-
-        import requests      
+     
         try:
             resp = requests.post(self.CITROS_HEALTH_CHECK, headers={
                 "Authorization": f"Bearer {self._get_token()}"
             })                
             if resp.status_code == 200 and resp.text == "OK":
                 return True
-        except Exception as err:
-            print("[ERROR] cant get access token at this moment...")
-            print(err)
-            return False
+            else:
+                self.log.error(f"Health check failed with status code {resp.status_code} and response {resp.text}")
+        except requests.exceptions.RequestException as err:
+            print("Can't get access token at this moment...")
+            self.handle_exceptions(err)
+            
         return False
-    
+
+
     def authenticate_with_key(self, key):
-        """Login to CiTROS using a key
+        """
+        Login to CiTROS using a key.
 
         Args:
-            key (string): a key generated by CiTROS system.
-        """        
+            key (str): a key generated by CiTROS system.
+
+        Returns:
+            bool: True if the login attempt was successful, False otherwise.
+        """   
         self.logout()
         
         query = """
             mutation auth($key: AuthenticateKeyInput!){
                 authenticateKey(input: $key){
                     results {
                     _role
                     fail
                     message
                     }
                 }
             }
-            """        
-        result = self.gql_execute(query, variable_values={ "key": {"jwtToken": key}})
+            """
+        try:  
+            result = self.gql_execute(query, variable_values={ "key": {"jwtToken": key}})
+            
+            if result is None or "authenticateKey" not in result:
+                self.log.error("Error during authentication: No response from server.")
+                return False
+
+            if not result["authenticateKey"]["results"][0]["fail"]:
+                token = key
+            else:
+                self.log.error("ERROR during authentication: unrecognized authentication key.")
+                token = None
+                return False
+            
+            self._set_token(token)
+            self.log.info("User authenticated.")
+            return True
         
-        # print("login result", result)
-        if not result["authenticateKey"]["results"][0]["fail"]:
-            token = key
-        else:
-            print("ERROR: failed to log in. resp", result)
+        except Exception as ex:
+            self.log.error("Authentication failed - exception was thrown.")
             token = None
-        
-        if token:
-            self._set_token(token)
-            self.log.info("Authenticated!")            
-        else:
-            self.log.error(f"ERROR during authentication attempt: wrong username or password.")
+            self.handle_exceptions(ex)
             return False
-        return True
-        
+
+
     def login(self, email, password):
-        """_summary_
+        """
+        Login to CiTROS using an email and password
 
         Args:
-            email (string): the user email 
-            password (string): the users password
-        """                
+            email (str): the user email 
+            password (str): the user's password
+
+        Returns:
+            bool: True if the login attempt was successful, False otherwise.
+        """                  
         if self.isAuthenticated():
             return True
         
         query = """
             mutation AuthenticateUser($email: String!, $password: String!) {
                 authenticate(input: {
                     email: $email, 
@@ -246,49 +316,52 @@
                 }
             }
             """        
         result = self.gql_execute(query, variable_values={
             "email": email,
             "password": password
         })
-        # print("login result", result)
-        if result:
-            token = result["authenticate"]["jwt"]
-        else:
-            print("ERROR: failed to log in. resp: ", result)
-            token = None
+
+        if result is None or 'authenticate' not in result or 'jwt' not in result['authenticate']:
+            self.log.error("Failed to log in. Response: " + result)
             return False
+
+        token = result["authenticate"]["jwt"]
         
         try:
-            # bug fix. addede audience as it didnt work in some cases. 
-            decoded = jwt.decode(token, options={"verify_signature": False}, audience="postgraphile")        
-            # print("decoded: ", decoded)
-        except Exception as err:     
-            print("ERROR: failed to log in. token: ", token) 
-            self.log.exception(err)        
-            traceback.print_exc()
+            # bug fix. added audience as it didn't work in some cases. 
+            decoded = jwt.decode(token, options={"verify_signature": False}, audience="postgraphile")
+        except jwt.exceptions.DecodeError as err:
+            self.log.error("Failed to log in. token: " + token) 
+            self.handle_exceptions(err)
             return False
         
         if token and decoded["role"] != "citros_anonymous":
             self._set_token(token)
-            self.log.info("Authenticated!")
+            self.log.info("User authenticated.")
+            return True
         else:
-            print(f"ERROR during authentication attempt: wrong username or password for [{email}]")
-            self.log.error(f"ERROR during authentication attempt: wrong username or password for [{email}]")
+            self.log.error(f"Authentication attempt failed: wrong username or password for [{email}]")
             return False
-        return True
-            
+
+
     def getUser(self):
-        """returns the currently logged in user with all his data
+        """
+        Returns the currently logged in user with all their data from CiTROS.
+
+        This includes their ID, username, role ID and name, and their
+        organization's ID, name, and domain prefix.
 
         Returns:
-            user: all user data from CiTROS
-        """        
+            dict: The user data, or None if the user is not logged in or an
+                  error occurred.
+        """           
         if self._user:
             return self._user
+        
         query = """
             query getCurrentUser {
                 currentUser {  
                     id        
                     username        
                     role{
                         id
@@ -298,126 +371,218 @@
                         id 
                         name
                         domainPrefix
                     }                    
                 }
             }  
             """
+        
         try:
-            result = self.gql_execute(query)            
-            self._user = result["currentUser"]    
+            result = self.gql_execute(query)
+            if result is None or 'currentUser' not in result:
+                self.log.error("Error during getUser: No response or unexpected response format from server.")
+                self._user = None
+            else:
+                self._user = result["currentUser"]
         except Exception as e:
+            self.handle_exceptions(e)
             self.logout()
-            self._user = None
+
         return self._user
     
-    ###########################
-    # Docker
-    ###########################    
+    ################################# Docker #################################
+    
     def get_access_token(self):
+        """
+        Fetches an access token if the user is authenticated.
+
+        Returns:
+            str: The access token, or None if the user is not authenticated or an error occurred.
+        """
         if not self.isAuthenticated():
             print("user is not logged in. please log in first.")
             return 
         
         rest_data = None
-        import requests      
+             
         try:
             resp = requests.post(self.CITROS_GTOKEN, headers={
                 "Authorization": f"Bearer {self._get_token()}"
-            })          
+            })
+            resp.raise_for_status()     
             rest_data = resp.json()
-        except Exception as err:
-            print("[ERROR] cant get access token at this moment...")
-            print(err)
-            return    
-        
-        # print(rest_data)
+        except requests.HTTPError as ex:
+            self.log.error("HTTP error occurred during get_access_token")
+            self.handle_exceptions(ex)
+            return
+        except requests.RequestException as ex:
+            self.log.error("A network error occurred during get_access_token")
+            self.handle_exceptions(ex)
+            return
+        except json.JSONDecodeError as ex:
+            self.log.error("Failed to decode JSON response during get_access_token")
+            self.handle_exceptions(ex)
+            return
         
-        # token = rest_data["id_token"]
         try:
-            # token = rest_data
             token = rest_data["access_token"]            
             expires_in = rest_data["expires_in"]
             token_type = rest_data["token_type"]
-        except KeyError as err:
+        except KeyError as ex:
+            self.log.error("Failed to fetch access token, expected key not found in response.")
+            self.handle_exceptions(ex)
             return None
         return token
             
-    ###########################
-    # GraphQL
-    ###########################             
-    def _get_transport(self):                            
+    ################################# GraphQL #################################
+       
+    def _get_transport(self):
+        """
+        Obtain transport with authorization if user is authenticated.
+        """                      
         transport = RequestsHTTPTransport(
             url=self.CITROS_ENTRYPOINT,
             verify=True,
             retries=3            
         )     
         # create GQL client for user or for anonymous user. 
         if self.isAuthenticated():
             transport.headers = {
                 "Authorization": f"Bearer {self._get_token()}"
             }
         return transport
 
+
     def _get_gql_client(self):
+        """
+        Obtain GraphQL client.
+        """
         if self._gql_client and not self._token_changed:
             return self._gql_client
         # https://gql.readthedocs.io/en/v3.0.0a6/intro.html
         transport = self._get_transport()
         self._gql_client = Client(transport=transport, fetch_schema_from_transport=False)
         self._token_changed = False
         return self._gql_client
-        
+
+
     def gql_execute(self, query, variable_values=None):
-        """_summary_
+        """
+        Execute a GraphQL query.
 
         Args:
             query (gql): gql query
             variable_values (dict, optional): variables for the gql query. Defaults to None.
 
         Returns:
+            dict: Result of the executed query.
         """
         
         gql_query = gql(query)
         try:
             return self._get_gql_client().execute(gql_query, variable_values=variable_values)
-        except TransportQueryError as err:                    
-            print("TransportQueryError: Error while querying: query=",query, " variable_values=",variable_values)
-            self.log.exception(err) 
-            traceback.print_exc()
-                 
-            if err.errors[0].get('errcode', '') == "23503":                
-                self.logout()            
+        except TransportQueryError as ex:                    
+            self.log.error(f"Error while querying: query={query} variable_values={variable_values}")
+            self.handle_exceptions(ex)     
+            if ex.errors[0].get('errcode', '') == "23503":                
+                self.logout()
         except Exception as e:    
-            print("Exception: Error while querying: query=",query, " variable_values=",variable_values)
-            self.log.exception(e)
-            traceback.print_exc()
+            self.log.error(f"Error while querying: query={query} variable_values={variable_values}")
+            self.handle_exceptions(ex)
                            
         return None
     
-    ###########################
-    # CITROS sync
-    ###########################
-    def sync_logs(self, request_json):
+    ############################### CITROS sync ###############################
+
+    def sync_logs(self, log_content):
+        """Synchronizes logs with the CiTROS system.
+
+        Args:
+            log_content (json): The log data to be synchronized.
+
+        Returns:
+            bool: True if the synchronization was successful, False otherwise.
+        """
         if not self.isAuthenticated():
-            print("User is unauthenticated. please login first!")
+            # print("User is unauthenticated. please login first!")
             return
-        
-        import requests     
+           
         try:           
-            resp = requests.post(self.CITROS_LOGS, 
-                              json=request_json, 
-                              headers={"Authorization": f"Bearer {self._get_token()}"}
-                            )         
+            resp = requests.post(
+                self.CITROS_LOGS, 
+                json=log_content, 
+                headers={"Authorization": f"Bearer {self._get_token()}"}
+            )      
+
             if resp.status_code != 200:
-                print(f"Error from sync_logs: {resp.status_code}: {resp.reason}", resp)
-                # print("sync_logs", self.CITROS_LOGS, request_json)
+                self.log.error(f"Error from sync_logs: {resp.status_code}: {resp.reason}")
                 return False
-        except Exception as e:
-            print(f"Error from sync_logs: {e}", resp)
-            # print("sync_logs", self.CITROS_LOGS, request_json)
+        except requests.RequestException as e:
+            self.log.error(f"Error from sync_logs. log content = {log_content}")
+            self.handle_exceptions(e)
             return False
         
         return True
     
+    ############################### CITROS list ###############################
+    
+    def query_projects(self):
+        """
+        Queries the names of all projects in the CiTROS system.
+
+        Returns:
+            list: A list of project names, or an empty list if no projects are found.
+        """
+        query = """
+            query projects {
+                              projectsList(orderBy: CREATED_AT_DESC) {
+                                name
+                              }
+                            }
+            """
+        try:
+            data = self.gql_execute(query)
+        except Exception as e:
+            self.handle_exceptions(e)
+            self.logout()
         
-   
+        if not data or not data.get("projectsList"):
+            self.log.info("No projects found.")
+            return []
+
+        project_list = [d["name"] for d in data["projectsList"]]
+        return project_list
+
+    
+    def query_simulations(self, proj_name):
+        """Queries the IDs of all simulations in a specified project.
+
+        Args:
+            proj_name (str): The name of the project.
+
+        Returns:
+            list: A list of simulation IDs, or an empty list if no simulations are found.
+        """
+        query = """
+        query sim_ids($name: String = "") {
+                              projectsList(orderBy: CREATED_AT_DESC, condition: {name: $name}) {
+                                name
+                                simulationsList(orderBy: CREATED_AT_ASC) {
+                                  id
+                                  name
+                                }
+                              }
+                            }
+        """
+        try:
+            data = self.gql_execute(query, variable_values={"name": proj_name})
+        except Exception as e:
+            self.handle_exceptions(e)
+            self.logout()
+
+        if not data or not data.get("projectsList") or not data["projectsList"][0].get("simulationsList"):
+            print(f"No simulations found for project {proj_name}.")
+            return []
+
+        sim_ids = [d["id"] for d in data["projectsList"][0]["simulationsList"]]
+        sim_names = [d["name"] for d in data["projectsList"][0]["simulationsList"]]
+        return sim_ids, sim_names
```

### Comparing `citros-23.22.2/citros/citros_bag.py` & `citros-23.23.1/citros/citros_bag.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,21 +2,20 @@
 from decouple import config
 from pathlib import Path
 import traceback
 import datetime 
 import json
 import yaml
 import os
+import requests   
+import psycopg2
+import glob
 
-# from .rosbag import BagReader
 from .rosbag import BagReaderSQL
 
-###########################
-#           BAGd
-###########################  
 class citros_bag():
     def __init__(self, citros):     
         self.citros = citros
         self.log = citros.log 
         
         self.BUCKET = 'citros_bags'
         self.CITROS_BAG_TOKEN = f"{citros.CITROS_DOMAIN}/api/bag/token"  
@@ -24,47 +23,48 @@
         self.CITROS_DATA_HOST = config("CITROS_DATA_HOST", None)
         self.CITROS_DATA_PORT = config("CITROS_DATA_PORT", "5432")
         self.CITROS_DATA_DATABASE = config("CITROS_DATA_DATABASE", "postgres")
         self.CITROS_DATA_USERNAME = config("CITROS_DATA_USERNAME", "citros_anonymous")
         self.CITROS_DATA_PASSWORD = config("CITROS_DATA_PASSWORD", "citros_anonymous")
         
         self.CONFIG_FOLDER = config("CONFIG_FOLDER", 'tmp/config')
-        # if not self.CITROS_DATA_HOST:
-        #     raise Exception("env variable CITROS_DATA_HOST is None, the simulation will not be able to upload the data to DB.")            
+
     
-    # get token to upload the bag to GCP bucket.
     def get_bag_access_token(self):
+        """
+        get token to upload the bag to GCP bucket.
+        """
         if not self.citros.isAuthenticated():
             self.log.error("User is not logged in. please log in first.")
             return None
         
         rest_data = None
-        import requests      
+           
         try:
             resp = requests.post(self.CITROS_BAG_TOKEN, headers={
                 "Authorization": f"Bearer {self.citros._get_token()}"
             })
             if resp.status_code == 404:      
                 self.log.error("cant find [{self.CITROS_BAG_TOKEN}] url.")
                 return 
             rest_data = resp.json()
         except Exception as err:
             self.log.error("Cant get access token at this moment... google json file may be corrupt (sa-api-secret).")
             self.log.error(err)
             return    
                                 
         try:
-            # token = rest_data
             token = rest_data["access_token"]            
             expires_in = rest_data["expires_in"]
             token_type = rest_data["token_type"]
         except KeyError as err:
             return None
         return token
     
+
     def emit(self, path_to_bag, batch_run_id, simulation_run_id, option='google'):       
         my_file = Path(path_to_bag)
         if not my_file.is_file():
             self.log.error(f"Bag file {path_to_bag} doesn't exists.")
             return False, f"Bag file {path_to_bag} doesn't exists.", None
                     
         path_to_metadata = "/".join(path_to_bag.split("/")[:-1]) +"/metadata.yaml"           
@@ -73,19 +73,20 @@
         
         # TODO: if  bag is 3db -> sqlite
         # TODO: if  bag is mcap -> mcap
         # TODO: log in between!
         # TODO: fix event logs for ros... after bad is not done! 
         return self.sync_bag_pgdb(batch_run_id, simulation_run_id, path_to_metadata, path_to_bag)
     
-    ################################################################################################
-    ### sync BAG to Postgres DB
-    ################################################################################################
-    def sync_bag_pgdb(self, batch_run_id, simulation_run_id, path_to_metadata, path_to_bag):        
-        import psycopg2
+    ######################### sync BAG to Postgres DB #########################
+
+    def sync_bag_pgdb(self, batch_run_id, simulation_run_id, path_to_metadata, path_to_bag):  
+        """
+        sync BAG to Postgres DB.
+        """      
         self.log.debug("------------------------------------------------------------------------------------")
         self.log.debug(f"uploading bag to PGDB")
         
         connection = None
         # get data-token from citros to access data DB.             
         user = self.citros.getUser()      
         
@@ -93,52 +94,56 @@
             error_text = f"Error at sync_bag, failed to get user from CITROS."
             self.log.error(error_text)                                 
             return False, error_text, None
         
         if not self.CITROS_DATA_HOST:
             raise Exception(f"[{datetime.datetime.now()}] ENV variable [CITROS_DATA_HOST] is None, the simulation will not be able to upload the data to DB.")            
         
-        connection = psycopg2.connect(user=user["username"],
-                                    password=user["id"],
-                                    host=self.CITROS_DATA_HOST,
-                                    port=self.CITROS_DATA_PORT,
-                                    database=self.CITROS_DATA_DATABASE)
+        try:
+            connection = psycopg2.connect(user=user["username"],
+                                        password=user["id"],
+                                        host=self.CITROS_DATA_HOST,
+                                        port=self.CITROS_DATA_PORT,
+                                        database=self.CITROS_DATA_DATABASE)
+        except psycopg2.OperationalError as e:
+            self.log.error("Unable to connect to the database. Check your config!")
+            self.log.error(e)
+            return False, "Unable to connect to the database. Check your config!", None
+
         cursor = connection.cursor()
         postgres_insert_query = f""" 
             insert into data_bucket."{batch_run_id}"
             (sid, rid, time, topic, type, data)
             values (%(sid)s, %(rid)s, %(time)s, %(topic)s, %(type)s, %(data)s);
         """
         
         try:                                       
             #####################
             # Uploads configs    
             #####################
-            import glob
             rid_counter = 0
             self.log.debug(f"uploading config")
             for config_file in glob.glob(self.CONFIG_FOLDER + "/*"):                
                 with open(f"{config_file}", 'r') as file:                                                     
                     config_dict = yaml.load(file, Loader=yaml.FullLoader) 
                     self.log.debug(f"uploading config [{config_file}]")
                     
                     record_to_insert = {
                         "sid": simulation_run_id,
                         "rid": rid_counter,
                         "time": 0,
                         "topic": '/config',
-                        "type": 'params',
+                        "type": config_file,
                         # "type": config_file.split('.')[0],
                         "data": json.dumps(config_dict)
                     }
                     rid_counter = rid_counter + 1
                     
                     cursor.execute(postgres_insert_query, record_to_insert)                                                        
                     connection.commit()                
-                      
             
             #####################
             # Uploads metadata
             #####################
             self.log.debug(f" + uploading metadata")
             with open(path_to_metadata, 'r') as file:                                                     
                 metadata_dict = yaml.load(file, Loader=yaml.FullLoader) 
@@ -149,68 +154,56 @@
                     "rid": 0,
                     "time": 0,
                     "topic": '/metadata',
                     "type": 'metadata',
                     "data": json.dumps(metadata_dict)
                 }
                 
-                # self.log.debug("metadata record_to_insert:", record_to_insert)
-                # record_to_insert = (simulation_run_id, 0, 0, '/metadata', 'metadata', json.dumps(metadata_dict))                
-                # self.log.debug(postgres_insert_query, record_to_insert)
-                
                 cursor.execute(postgres_insert_query, record_to_insert)                                                        
                 connection.commit()                                 
             
             #####################
             # Uploading data
             #####################  
             self.log.debug(f" +++ uploading bag to PG")
             bagReader = BagReaderSQL()
             total_size = 0
             for buffer in bagReader.read_messages(path_to_bag, simulation_run_id):
-                # self.log.debug(f" + read_messages")
                 size = buffer.seek(0, os.SEEK_END)
                 size = buffer.tell()
                 total_size = total_size + size
                 buffer.seek(0)                
                 self.log.debug(f" \tinserting buffer size: { (size / 1024 ) / 1024 } MB")
                 if size == 0:
                     continue
                 cursor.execute(f'SET search_path TO data_bucket')
                 try:           
                     cursor.copy_from(buffer, batch_run_id, sep=chr(0x1E), null="", columns=['sid', 'rid', 'time', 'topic', 'type', 'data'])                
                 except (Exception, psycopg2.Error) as error:
                     buffer.seek(0)                      
                     self.log.error(f" Failed to insert record into table, aboring uploading to PG DB.", error) 
-                    # self.log.error(traceback.format_exc())
                     self.log.exception(error)     
-                    # self.log.debug("===============================================================================================")
-                    # self.log.debug(buffer.getvalue())
-                    # self.log.debug("===============================================================================================")
                     return False, "got exception from pgdb", str(error)
-                # buffer.truncate(0)
-                # buffer.seek(0)
-                # buffer.close()
+                
                 connection.commit()
             self.log.debug(f" --- done uploading to PG")
             return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}] to Postgres. [size: {(total_size / 1024)/1024} MB]", None
         except (Exception, psycopg2.Error) as error:
             self.log.exception(f" Failed to insert record into table, aboring uploading to PG DB.", error) 
             self.log.exception(traceback.format_exc())
             return False, "got exception from pgdb", str(error)
         finally:
             # closing database connection.
             if connection:
                 cursor.close()
                 connection.close()
                 self.log.debug(f"PostgreSQL connection is closed")  
                 
-    ################################################################################################
-    ### sync BAG to Google Bucket
-    ################################################################################################
+    ######################## sync BAG to Google Bucket ########################
+
     def sync_bag_google_bucket(self, batch_run_id, simulation_run_id, path_to_metadata, path_to_bag):
         self.log.debug("------------------------------------------------------------------------------------")
         self.log.debug("uploading bag to google bucket")
         if not self.citros.isAuthenticated():
             self.log.debug("not authenticated. please login first.")
             return False, "not authenticated. please login first." , None       
         
@@ -220,53 +213,48 @@
         bag_file_name = path_to_bag.split('/')[-1]            
         data_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={tenant + "/" + batch_run_id + "/sid-" + simulation_run_id + "/" + bag_file_name}'        
         
         metadata_name = path_to_metadata.split('/')[-1]  
         metadata_url = f'https://storage.googleapis.com/upload/storage/v1/b/{self.BUCKET}/o?uploadType=media&name={tenant + "/" + batch_run_id + "/sid-" + simulation_run_id + "/" + metadata_name}'        
 
         google_token = self.get_bag_access_token()
-        # self.log.debug("google_token", google_token)
         if google_token is None:
             error_text = f"[ERROR] at sync_bag, failed to get google token from CITROS."
             self.log.error(error_text)                                  
             return False, error_text, None  
-        
-        import requests  
+
+        headers = {
+        "Authorization": f"Bearer {google_token}",
+        "Content-Type": "application/octet-stream"
+        }
+
+        def upload_file(url, path_to_file):
+            with open(path_to_file, 'rb') as data:
+                try:
+                    resp = requests.post(url, data=data, headers=headers)
+                    resp.raise_for_status()
+                except requests.exceptions.HTTPError as err:
+                    self.log.error(f"HTTP error occurred: {err}")
+                    return False
+                except Exception as err:
+                    self.log.error(f"An error occurred: {err}")
+                    return False
+                else:
+                    return resp
+
         # uploading metadata first, assuming much smaller file. 
-        with open(path_to_metadata, 'rb') as data:
-            # metadata = yaml.safe_load(data)
-            metadata_resp = requests.post(metadata_url,
-                                data=data,
-                                headers={
-                                    "Authorization": f"Bearer {google_token}",
-                                    "Content-Type" : "application/octet-stream"
-                                }
-                            ) 
-        if metadata_resp.status_code != 200:                        
-            error_text = f"[ERROR] from sync_bag: [{metadata_resp.status_code}]:[{metadata_resp.reason}]"
-            self.log.error(error_text)
-            return False, error_text, None  
-        
+        metadata_resp = upload_file(metadata_url, path_to_metadata)
+        if not metadata_resp:
+            error_text = f"[ERROR] from sync_bag: failed to upload metadata."
+            return False, error_text, None
+
         self.log.info(f"done updating metadata to: [{batch_run_id}],[{simulation_run_id}] - [{metadata_resp.text}]")
         
-        # uploading the bag
-        with open(path_to_bag, 'rb') as data:            
-            bag_resp = requests.post(data_url,
-                                data=data,
-                                headers={
-                                    "Authorization": f"Bearer {google_token}",
-                                    "Content-Type" : "application/octet-stream"
-                                }
-                            ) 
-            # self.log.debug("bag_resp", bag_resp)
-            
-        if bag_resp.status_code != 200:                        
-            error_text = f"[ERROR] from sync_bag: [{bag_resp.status_code}]:[{bag_resp.reason}]"
-            self.log.error(error_text)            
-            # self.log.debug("sync_bag", CITROS_BAG, request_json)
-            return False, error_text, None  
-        
-        # self.log.debug("resp", json.loads(bag_resp.text))
+        bag_resp = upload_file(data_url, path_to_bag)
+        if not bag_resp:
+            error_text = f"[ERROR] from sync_bag: failed to upload bag file."
+            return False, error_text, None
         
-        self.log.info(f"done updating bag to: [{batch_run_id}],[{simulation_run_id}] - [{bag_resp.text}] ")        
+        self.log.info(f"done updating bag to: [{batch_run_id}],[{simulation_run_id}] - [{bag_resp.text}] ")
+
         return True, f"success, uploaded [{path_to_metadata}],[{path_to_bag}]", bag_resp.text
```

### Comparing `citros-23.22.2/citros/citros_batch.py` & `citros-23.23.1/citros/citros_batch.py`

 * *Files 24% similar despite different names*

```diff
@@ -24,30 +24,35 @@
                 }
             }            
         }
         """
         result = self.citros.gql_execute(query, variable_values={"batchRunId": batch_run_id})
         return result
     
-    def create_manual_batch(self, simulation_id, completions):
+    def create_manual_batch(self, simulation_id, completions, isManual):
         query = """
-        mutation createBatch($simulationId: UUID!, $completions: Int) {
-        createBatchRun(input: {             
-            batchRun: {
-                simulationId: $simulationId,
-                completions: $completions,
-                parallelism: 0,
-                trigger: MANUAL,
-                isManual: true
-                }
-            }){
-                batchRun {
-                id
-                }
-            } 
-        }
+        mutation createBatch($simulationId: UUID!, $completions: Int, $isManual: Boolean = true, $trigger: TriggerType = MANUAL) {
+                      createBatchRun(
+                        input: {
+                            batchRun: {
+                                simulationId: $simulationId, 
+                                completions: $completions, 
+                                parallelism: 0, 
+                                trigger: $trigger, 
+                                isManual: $isManual}}
+                      ) {
+                        batchRun {
+                          id
+                        }
+                      }
+                    }
+
         """ 
-        result = self.citros.gql_execute(query, variable_values={"simulationId": simulation_id, "completions": int(completions)})        
+        trigger = "MANUAL" if isManual else "CLI"
+        result = self.citros.gql_execute(query, variable_values={"simulationId": simulation_id, 
+                                                                 "completions": int(completions),
+                                                                 "isManual" : isManual,
+                                                                 "trigger" : trigger})
         return result["createBatchRun"]["batchRun"]["id"]
```

### Comparing `citros-23.22.2/citros/citros_events.py` & `citros-23.23.1/citros/citros_events.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # from __future__ import absolute_import
 import atexit
 import json
-import os
 import threading
-from functools import partial
-import sys
-import logging
 import datetime 
+import requests
 
 def setInterval(interval):
     """
     :param interval: 
     """
     def decorator(function):
         """
@@ -33,220 +30,246 @@
             t.start()
             return stopped
 
         return wrapper
 
     return decorator
 
+
 class citros_events():    
-    """Will emit events to the CiTROS server. 
+    """
+    Handles event emission to the CiTROS server. 
     
+    This class collects events and periodically sends them to the CiTROS server.
+    It supports different types of events representing different stages in the lifecycle
+    of a simulation.
     """
     def __init__(self, citros):
         self.citros = citros        
         
         self.timer = None
         self.events = []
         self.timer = self._flushAndRepeatTimer()
         atexit.register(self._stopFlushTimer)
         
         self.CITROS_EVENTS = f"{self.citros.CITROS_DOMAIN}/api/events"    
         
         self.seq = 0
+        self._events_lock = threading.Lock()
+
 
     @setInterval(5)
     def _flushAndRepeatTimer(self):        
         self.flush()
 
+
     def _stopFlushTimer(self):        
         self.timer.set()
         self.flush()   
     
+
     def flush(self, current_batch=None):   
-        """Sends all the events in current_batch to the Citros server.
+        """
+        Sends all the events in current_batch to the Citros server.
+        If current_batch is None, will try to send all the events from self.events
 
         :param current_batch:  (Default value = None)
-        if current_batch is None, will try to send all the events from self.events
         """
         if not self.citros.isAuthenticated():
             return
-        if current_batch is None:
-            self.events, current_batch = [], self.events        
+        
+        # protect from the main thread running emit()
+        with self._events_lock:
+            if current_batch is None:
+                self.events, current_batch = [], self.events 
                     
         if len(current_batch) == 0:
             return
         
         request_json = {
             "events": current_batch
         }
         
         resp = self.sync_events(request_json)   
         if not resp and current_batch is not None:
-            # retry on fail.            
-            self.events = current_batch + self.events
+            # retry on fail.
+            # protect from the main thread running emit()
+            with self._events_lock: 
+                self.events = current_batch + self.events
         
+
     def sync_events(self, request_json):
+        """
+        Synchronize (upload) the given batch of events with the Citros server.
+        """
         if not self.citros.isAuthenticated():
             print("User is unauthenticated. please login first!")
             return
         
-        import requests
         try:  
             resp = requests.post(self.CITROS_EVENTS, 
-                              json=request_json, 
-                              headers={"Authorization": f"Bearer {self.citros._get_token()}"}
-                            )              
+                                 json=request_json, 
+                                 headers={"Authorization": f"Bearer {self.citros._get_token()}"}
+                                )              
             if resp.status_code != 200:
-                print(f"Error from sync_events: [{self.CITROS_EVENTS}], {resp.status_code}: {resp.reason}", resp)
-                # print("sync_events", self.CITROS_EVENTS, request_json)
+                self.citros.log.error(f"sync_events: [{self.CITROS_EVENTS}], {resp.status_code}: {resp.reason} \nresponse: {resp}")
                 return False   
-        except Exception as e:
-            print(f"Error from sync_events: [{self.CITROS_EVENTS}], {e}")
+        except requests.exceptions.RequestException as e:
+            self.citros.log.error(f"Error from sync_events: [{self.CITROS_EVENTS}]")
+            self.citros.handle_exceptions(e)
             return False
+        
         return True
     
     
-    
-    
-    
-    
-    
     def emit(self, batch_run_id, sid, event_type, tag, message, metadata):
         """
+        Appends an event to the event list, to be later synched with Citros.
 
         :param batch_run_id: batch run id
         :param sid: sequence-id of the simulation 
         :param event: event type
         :param tag: tag - can be any string
         :param message: a message for the event
         :param metadata: some dict object containing metadata.
-        
         """
         try:
-            if type(metadata) == dict:
+            if isinstance(metadata, dict):
                 metadata = json.dumps(metadata)
         except Exception as e:
-            print(e)
+            self.citros.handle_exceptions(e)
                                     
         event = {
             "batch_run_id":batch_run_id, 
             "sid": sid, 
             "event":event_type, 
             "tag":tag, 
             "message":message,
             "metadata":metadata,
             "created": datetime.datetime.now().isoformat(),
             "seq": self.seq
         }
+
         self.seq = self.seq + 1
-        self.events.append(event)
+
+        # protect from the thread running flush()
+        with self._events_lock:
+            self.events.append(event)
     
+
     def schedule(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
+        Sends event of type SCHEDULE to CiTROS
 
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "SCHEDULE", tag, message, metadata)
         
+
     def creating(self, batch_run_id, sid, tag="", message="", metadata=None):
-        """Sends event of type CREATING to CiTROS
+        """
+        Sends event of type CREATING to CiTROS
 
         :param batch_run_id: batch run id
         :param sid: sequence-id of the simulation         
         :param tag: tag - can be any string
         :param message: a message for the event
         :param metadata: some dict object containing metadata.
-
         """
         self.emit(batch_run_id, sid, "CREATING", tag, message, metadata)
     
+
     def init(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
+        Sends event of type INIT to CiTROS
 
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "INIT", tag, message, metadata)
           
+
     def starting(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
-
+        Sends event of type STARTING to CiTROS
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "STARTING",tag, message, metadata)
                   
+
     def running(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
-
+        Sends event of type RUNNING to CiTROS
+        
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "RUNNING", tag, message, metadata)
     
+
     def terminating(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
+        Sends event of type TERMINATING to CiTROS
 
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "TERMINATING", tag, message, metadata)
     
+
     def stopping(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
+        Sends event of type STOPPING to CiTROS
 
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "STOPPING", tag, message, metadata)        
         
+
     def done(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
+        Sends event of type DONE to CiTROS
 
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "DONE", tag, message, metadata)
     
+    
     def error(self, batch_run_id, sid, tag="", message="", metadata=None):
         """
+        Sends event of type ERROR to CiTROS
 
         :param batch_run_id: 
         :param sid: 
         :param tag:  (Default value = "")
         :param message:  (Default value = "")
         :param metadata:  (Default value = None)
-
         """
         self.emit(batch_run_id, sid, "ERROR", tag, message, metadata)
```

### Comparing `citros-23.22.2/citros/citros_integration.py` & `citros-23.23.1/citros/citros_integration.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 from gql import Client, gql
 from gql.transport.requests import RequestsHTTPTransport
 import json
 import os
 
 class citros_integration():
-    """citros_integration class has all the functionality to integrate the project to CiTROS"""
+    """
+    citros_integration class has all the functionality to integrate the project to CiTROS
+    """
     def __init__(self, citros) -> None:
-        # Select your transport with a defined url endpoint        
+        """
+        :param citros: Citros object
+        """     
         self.citros = citros
         self.log = citros.log
         self.proj_jason_path = ".citros/project.json"
 
+
     def uploadParam(self, param, node_id):    
         """
+        Upload a parameter to Citros.
 
-        :param param: 
-        :param node_id: 
-        """
-        # print("uploadParam for node_id: ", node_id)      
+        :param param: Parameter dictionary
+        :param node_id: Node identifier
+        :return: Parameter ID
+        """   
         query = """
         mutation UpsertRosNodeParameter($node_id: UUID!, $name: String!, $description: String!, $value: String!, $parameterType: ParameterType) {
             upsertRosNodeParameter(
                 where: {rosNodeId: $node_id, name: $name }
                 input: {rosNodeParameter: {rosNodeId: $node_id, name: $name, description: $description, parameterType: $parameterType, value: $value}}                
             ) {
                 rosNodeParameter {                    
@@ -38,27 +44,27 @@
         if param["parameterType"] == 'LIST':
             print('*********************************************************')
             print(f'*** ERROR: parameterType {param["parameterType"]} not supported. passing. ****')
             print('*********************************************************')
             return
         
         result = self.citros.gql_execute(query, variable_values=param)
-        # print(result)
         param_id = result["upsertRosNodeParameter"]["rosNodeParameter"]["id"]
         print(" - - - param_id", param_id)
         return param_id 
     
+
     def uploadNode(self, node, package_id):      
         """
+        Upload a node to Citros.
 
-        :param node: 
-        :param package_id: 
-
+        :param node: Node dictionary
+        :param package_id: Package identifier
+        :return: Node ID
         """
-        # print("uploadNode for package_id: ", package_id)  
         query = """
         mutation UpsertRosNode($package_id: UUID!, $name: String!, $path: String!) {
             upsertRosNode(
                 where: {
                     name: $name,
                 }
                 input: {rosNode: {packageId: $package_id, name: $name, path: $path}}
@@ -69,62 +75,64 @@
             }
         }
         """
         
         node["package_id"] = package_id
         result = self.citros.gql_execute(query, variable_values=node)
         
-        node_id = result["upsertRosNode"]["rosNode"]["id"]
+        node_id = result.get("upsertRosNode", {}).get("rosNode", {}).get("id")
         print(f" - - node: {node['name']} [{node_id}]")
         
         print(" - - - parameters: ")
-        for parameter in node["parameters"]:
+        for parameter in node.get("parameters", []):
             parameter_id = self.uploadParam(parameter, node_id)            
     
         return node_id  
     
+
     def uploadLaunch(self, launch, package_id):        
         """
+        Upload a launch to Citros.
 
-        :param launch: 
-        :param package_id: 
-
-        """
-        # print("uploadLaunch for package_id: ", package_id)        
+        :param launch: The launch details.
+        :param package_id: The package ID for the launch.
+        :return: The launch ID.
+        """       
         query = """
         mutation upsertLaunch($data: UpsertLaunchInput!){
             upsertLaunch(input:$data) {
                 launch{
                 id
                 name
                 }
             }
         }
         """
         
         print("Launch: ")
-        launch["packageId"] = package_id                
+        launch["packageId"] = package_id           
         result = self.citros.gql_execute(query, variable_values={
             "data":{
                 "launch":launch
             }
         })
-        # print("result", result)
-        launch_id = result["upsertLaunch"]["launch"]["id"]
+
+        launch_id = result.get("upsertLaunch", {}).get("launch", {}).get("id")
         print(" - launch_id", launch_id)
         return launch_id  
-        
+    
+
     def uploadPackage(self, package, project_id):
         """
+        Upload a package to Citros.
 
-        :param package: 
-        :param project_id: 
-
+        :param package: The package details.
+        :param project_id: The project ID for the package.
+        :return: The package ID.
         """
-        # print("uploadPackage for project_id: ", project_id)
         query = """
         mutation UpsertRosPackage(
             $projectId: UUID!, 
             $name: String!,
             $cover: String!,
             $description: String!,
             $git: String!,
@@ -157,31 +165,33 @@
                 }
             }
         }
         """
         
         package["projectId"] = project_id
         result = self.citros.gql_execute(query, variable_values=package)
-        # print(result)
-        package_id = result["upsertRosPackage"]["rosPackage"]["id"]        
+
+        package_id = result.get("upsertRosPackage", {}).get("rosPackage", {}).get("id")
         print(f" - package: {package['name']} [{package_id}]")
                 
-        for node in package["nodes"]:
+        for node in package.get("nodes", []):
             node_id = self.uploadNode(node, package_id)            
                                 
-        for launch in package["launches"]:
+        for launch in package.get("launches", []):
             launch_id = self.uploadLaunch(launch, package_id)             
             
         return package_id        
     
+
     def sync_project(self, project):
         """
+        Synchronize a project with Citros.
 
-        :param project: 
-
+        :param project: The project details.
+        :return: The project ID.
         """
         if not self.citros.isAuthenticated():                                
             self.log.error("Cant sync unauthenticated user. please log in first.")
             return
         
         partial_upsert = False
         
@@ -242,24 +252,21 @@
                 }) {
                     project {                                            
                         id
                     }                    
                 }
             }
             """
-        # print("Project: ")
+        
         print("-------------------sync_project-------------------")     
         project["userId"] = self.citros.getUser().get("id")
-        # print("user_id", self.citros.user.get("id"))
-        # print("user", self.citros.user)
         result = self.citros.gql_execute(query, variable_values=project)
-        # print("result:", result)
-        project_id = result["upsertProject"]["project"]["id"]   
+
+        project_id = result.get("upsertProject", {}).get("project", {}).get("id")
         print(f"project_id: {project['name']} [{project_id}]")         
                 
-        # print("Packages: ")
-        for package in project["packages"]:
+        for package in project.get("packages", []):
             package_id = self.uploadPackage(package, project_id)
         print("----------------------DONE------------------------")               
         
         return project_id
```

### Comparing `citros-23.22.2/citros/citros_params.py` & `citros-23.23.1/citros/citros_params.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,21 +1,23 @@
-# from pkg_resources import Distribution
-from soupsieve import match
 import yaml
 import json
+import os
+import numpy as np
 from pathlib import Path
 from decouple import config
+from ament_index_python.packages import get_package_share_directory
+
 
 class citros_params():
     def __init__(self, citros):
         self.citros = citros
         self.log = citros.log
-        
         self.CONFIG_FOLDER = config("CONFIG_FOLDER", 'tmp/config')
     
+    
     def _get_params(self, batch_run_id, sid=""):
         query = """
         query getParametersFromBatchRun($batchRunId: UUID!, $sid: String!){
             batchRun(id:$batchRunId){
                 id                
                 simulation {
                 project {
@@ -55,98 +57,72 @@
                 metadata
             }
         }
         """
         result = self.citros.gql_execute(query, variable_values={"batchRunId": batch_run_id, "sid": sid})        
         return result
    
+
     def _coercion(self, value, type):
         if type == "FLOAT":
             return float(value)
         if type == "INT":
             return int(float(value))
         return value
         
+    
     def _eval_distribution(self, parameter_setting):
-        import numpy as np
-
         distribution_type = parameter_setting["distType"]
-        param1 = parameter_setting["param1"]
-        param1Type = parameter_setting["param1Type"]
-        param1 = self._coercion(param1, param1Type)
-        param2 = parameter_setting["param2"]
-        param2Type = parameter_setting["param2Type"]
-        param2 = self._coercion(param2, param2Type)
-        
-        if distribution_type == "NORMAL":                            
-            return np.random.normal(param1, param2)
-        
-        if distribution_type == "EXPONENTIAL":                            
-            return np.random.exponential(param1)
-        
-        if distribution_type == "LAPLACE":                 
-            return np.random.laplace(param1, param2)
-        
-        if distribution_type == "POISSON":                            
-            return np.random.poisson(param1)
-        
-        if distribution_type == "POWER":                            
-            return np.random.power(param1)
-                
-        if distribution_type == "UNIFORM":                 
-            return np.random.uniform(param1, param2)
-           
-        if distribution_type == "ZIPF":                            
-            return np.random.zipf(param1)   
-        
-        if distribution_type == "VONMISES":                 
-            return np.random.vonmises(param1, param2)
-          
-        if distribution_type == "RAYLEIGH":                            
-            return np.random.rayleigh(param1)   
-        
-        if distribution_type == "FLOAT":
-            value = self._coercion(param1, param1Type)
-            return value
-        
-        if distribution_type == "STRING":                            
-            return param1
-              
-        self.log.error(f"Error: {distribution_type} is not supported.")        
+        param1 = self._coercion(parameter_setting["param1"], parameter_setting["param1Type"])
+        param2 = self._coercion(parameter_setting["param2"], parameter_setting["param2Type"])
+
+        distribution_mapping = {
+                "NORMAL": lambda: np.random.normal(param1, param2),
+                "EXPONENTIAL": lambda: np.random.exponential(param1),
+                "LAPLACE": lambda: np.random.laplace(param1, param2),
+                "POISSON": lambda: np.random.poisson(param1),
+                "POWER": lambda: np.random.power(param1),
+                "UNIFORM": lambda: np.random.uniform(param1, param2),
+                "ZIPF": lambda: np.random.zipf(param1),
+                "VONMISES": lambda: np.random.vonmises(param1, param2),
+                "RAYLEIGH": lambda: np.random.rayleigh(param1),
+                "FLOAT": lambda: self._coercion(param1, parameter_setting["param1Type"]),
+                "STRING": lambda: param1,
+        }
+        try:
+                return distribution_mapping[distribution_type]()
+        except KeyError:
+                self.log.error(f"Error: {distribution_type} is not supported.")   
         
+    
     def get_config(self, batch_run_id, sid=""):
         data = self._get_params(batch_run_id, sid)
         if not data:
-            self.log.error("Didnt get any data from GQL.")
-            print("Didnt get any data from GQL.")  
+            self.log.error("Did not get any data from GQL.")
             return 
-        # self.log.debug(json.dumps(data, indent=4))
         
-        # in case sid is provided, and there was already a run with this sid. load original config to run it again.
+        # in case sid is provided, and there was already a run with this sid. 
+        # load original config to run it again.
         reloaded_parameters = None
-        if len(data["simulationEventsList"]) > 0:
+        if data["simulationEventsList"]:
             reloaded_parameters = json.loads(data["simulationEventsList"][0]["metadata"])
-            self.log.info(f"Reloaded config from allready used [batch_run_id-sid] [{batch_run_id}-{sid}]")  
-            # print(f"Reloaded config from allready used [batch_run_id-sid] [{batch_run_id}-{sid}]")
+            self.log.info(f"Reloaded config from already used [batch_run_id-sid] [{batch_run_id}-{sid}]")
             return reloaded_parameters
             
         if data["batchRun"]["simulation"] is None:
             self.log.error("ERROR! Cant get parameters from CiTROS. There is no simulation attached to batch.")  
             return     
               
-        # users parametre setup
-        parameter_settings_list = data["batchRun"]["simulation"]["parameterSetup"]["parameterSettingsList"]        
-        paramValues = {} 
-        for ps in parameter_settings_list:
-            try:
-                paramValues[str(ps["nodeParameterId"])] = self._eval_distribution(ps)
-            except Exception as e:
-                self.log.error(f"Error in _eval_distribution, parameter_settings_list: [{json.dumps(ps, indent=4)}]")
-                # self.log.excption(e)
-                raise e
+        # users parameter setup
+        parameter_settings_list = data["batchRun"]["simulation"]["parameterSetup"]["parameterSettingsList"]
+        try:
+            paramValues = {str(ps["nodeParameterId"]): self._eval_distribution(ps) for ps in parameter_settings_list}
+        except Exception as e:
+            self.log.error(f"Error in _eval_distribution, parameter_settings_list")
+            raise e
         
         # load defaults from ros nodes. 
         ros_packages_list = data["batchRun"]["simulation"]["project"]["rosPackagesList"]
         config = {}   
         for package in ros_packages_list:
             config[package["name"]] = {}
             for node in package["rosNodesByPackageIdList"]:                
@@ -157,78 +133,73 @@
                     value = self._coercion(parameter['value'], parameter['parameterType'])
                     paramValue = paramValues.get(str(parameter["id"]))
                     if paramValue:
                         value = paramValue
                     config[package["name"]][node["name"]]["ros__parameters"][parameter['name']] = value                                                             
         return config   
     
-    def save_config(self, config):        
-        import os
-        try:
-            # print("creating path: ", self.CONFIG_FOLDER)
-            os.makedirs(self.CONFIG_FOLDER)
-        except FileExistsError:
-            # directory already exists
-            pass
+
+    def save_config(self, config):     
+        Path(self.CONFIG_FOLDER).mkdir(exist_ok=True, parents=True)
                 
-        from ament_index_python.packages import get_package_share_directory
         for package_name, citros_config in config.items():     
-            self.log.debug(f"Saving config for [{package_name}]")                               
+            self.log.debug(f"Saving config for [{package_name}]")
+
             # TODO: add other method to get the package path
             path_to_package = None
             try:
-                path_to_package = get_package_share_directory(package_name) # get the path to the package install directory - the project must be sourced for it to work            
+                # get the path to the package install directory - the project must be sourced for it to work 
+                path_to_package = get_package_share_directory(package_name)            
             except Exception as e:
                 self.log.exception(e)
                 continue                
 
             if not path_to_package:
                 continue
                 
             path = f"{path_to_package}/config/"    
             
             # check if folder exists
             if not Path(path).exists():
                 self.log.debug(f"No config file {path} exits for pack:{package_name}. passing.") 
                 continue
                                                 
-            # path = f"install/{package_name}/share/{package_name}/config/"
             Path(path).mkdir(parents=True, exist_ok=True)
             path = path + "params.yaml"
             
-            # check if file exists?
+            # check if file exists
             if not Path(path).exists():
-                self.log.debug(f"No config file {path} exits for pack:{package_name}. passing.") 
+                self.log.debug(f"No config file {path} exits for package: {package_name}. passing.") 
                 continue
             
-            # self.log.debug(f"Loading default config from {path}") 
             with open(path, "r") as stream:
                 try:    
                     default_config = yaml.safe_load(stream)
                 except yaml.YAMLError as exc:
-                    print(exc)
-            
-            # self.log.debug(f"Merging configuration files.") 
-            merged_config = {key: value for (key, value) in (list(default_config.items()) + list(citros_config.items()))}
+                    self.log.exception(exc)
             
-            # self.log.debug(f"config file for {package_name}:")
+            merged_config = {**default_config, **citros_config}
             self.log.debug(json.dumps(merged_config, indent=4))
             
             with open(path, 'w') as file:
                 yaml.dump(merged_config, file)  
                 
             # save for metadata
             with open(f"{self.CONFIG_FOLDER}/{package_name}.yaml", 'w') as file:                                     
                 yaml.dump(merged_config, file)         
     
-    def init_params(self, batch_run_id, sid):                
+
+    def init_params(self, batch_run_id, sid):
+        """
+        Fetches parameters from CITROS, saves them to files, and returns the config.
+        """          
         self.log.info("Getting parameters from CITROS.") 
         config = self.get_config(batch_run_id, sid)
         if not config:
-            # if there is no config, cant init anything...
-            self.log.warning("If there is no config, cant init anything...") 
+            self.log.warning("There is no config, can't init anything...") 
             return
+        
         self.log.debug("Saving parameters to files. ")        
         self.save_config(config)     
         self.log.debug("Done saving config files.")                    
         return config
```

### Comparing `citros-23.22.2/citros/citros_utils.py` & `citros-23.23.1/citros/citros_utils.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/launches/__init__.py` & `citros-23.23.1/citros/launches/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/launches/launch.py` & `citros-23.23.1/citros/launches/launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import shutil
 from datetime import datetime
 from typing import cast
 from ament_index_python.packages import get_package_share_directory
 from launch import LaunchDescription, Event
 from launch.actions import EmitEvent, ExecuteProcess, IncludeLaunchDescription, DeclareLaunchArgument, OpaqueFunction, RegisterEventHandler, LogInfo, TimerAction
 from launch.launch_description_sources import PythonLaunchDescriptionSource
 from launch_ros.actions import Node
@@ -12,15 +13,25 @@
 from launch.events import Shutdown, process
 from launch.actions import SetLaunchConfiguration
 from citros import Citros
 
 ################################
 # Entrypoint        
 ################################
-def generate_launch_description(citros : Citros, timeout):  
+def generate_launch_description(citros : Citros, timeout):
+    """
+    Generates a ROS2 LaunchDescription for a simulation run.
+
+    Args:
+        citros (Citros): An instance of Citros class which manages interaction with the CiTROS service.
+        timeout (int): The time limit for the simulation run.
+
+    Returns:
+        launch.LaunchDescription: A launch description that ROS2 can execute.
+    """
     batch_run_id = str(citros.batch_run_id)    
     simulation_run_id = str(citros.simulation_run_id)    
     timeout = str(timeout)    
     
     citros.log.debug("+ generate_launch_description()")
     citros.log.debug(f"batch_run_id: {batch_run_id}")
     citros.log.debug(f"simulation_run_id: {simulation_run_id}")
@@ -29,17 +40,16 @@
     resp = citros.checkStatus()
     if not resp:        
         return 
     
     citros.log.debug("Health-check: OK")
     citros.events.init(batch_run_id=batch_run_id, sid=simulation_run_id, tag="INIT", message="updated config", metadata=None)
 
-    ld = LaunchDescription([
-        LogInfo(msg='CITROS launch file!')
-    ])
+    ld = LaunchDescription([LogInfo(msg='CITROS launch file!')])
+
     ld.add_action(SetLaunchConfiguration('batch_run_id', batch_run_id))
     ld.add_action(SetLaunchConfiguration('simulation_run_id', simulation_run_id))
 
     batch = citros.batch.get_batch(batch_run_id) 
     
     if not batch["batchRun"]:
         citros.log.error(f"unknown batch id [{batch_run_id}]")
@@ -83,15 +93,14 @@
         ),   
         default_value=str(60*60*24*7),   
     ))
 
     ################################
     # RECORDING BAG Proccess 
     ################################ 
-    import shutil
     bag_folder = 'tmp/bag' 
     bag_name = 'bag_0.db3'  # default to sqlite3
 
     # delete folder if exists
     try:
         shutil.rmtree(bag_folder)
     except Exception as e:
```

### Comparing `citros-23.22.2/citros/logger/__init__.py` & `citros-23.23.1/citros/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/logger/logger.py` & `citros-23.23.1/citros/logger/logger.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/logger/logger_pg_handler.py` & `citros-23.23.1/citros/logger/logger_pg_handler.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/parsers/__init__.py` & `citros-23.23.1/citros/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/parsers/parser_ros2.py` & `citros-23.23.1/citros/parsers/parser_ros2.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,145 +1,184 @@
-from pygments import highlight, lexers, formatters
-from bson import ObjectId
 import glob
-import json
 import yaml
 import subprocess
 import os
 import ast
+import re
+
+import xml.etree.ElementTree as ET
 
 from .parser_base import parser_base
 
 
 class parser_ros2(parser_base):
-    def __init__(self, logging) -> None:                                
-        self.log = logging
-        
+    """
+    Class to parse ROS2 package files (XML, CMakeLists.txt, setup.py etc).
+    """  
+
+    def __init__(self, logger) -> None:                                
+        self.log = logger
         self.project = None
 
+    ################################ Any lang #################################
 
-    def print(self, json_data):
-        formatted_json = json.dumps(json_data, indent=4, default=str)
-        self.log.info(formatted_json)
-        # colorful_json = highlight(bytes(formatted_json, 'UTF-8'), lexers.JsonLexer(), formatters.TerminalFormatter())
-        # self.log.debug(colorful_json)
+    def parse_xml(self, package_path):
+        """
+        Parse an XML file in the given package path.
 
+        :param package_path: Path of the package.
+        """  
+        path_to_package_xml = os.path.join(package_path, "package.xml")
+        if not os.path.exists(path_to_package_xml):
+            self.log.error(f"File not found: {path_to_package_xml}")
+            return {}
 
-    # Any lang
-    def parse_xml(self, package_path):    
-        import xml.etree.ElementTree as ET
-        path_to_package_xml = f"{package_path}/package.xml"                
-        tree = ET.parse(path_to_package_xml)
-        root = tree.getroot()
+        try:
+            tree = ET.parse(path_to_package_xml)
+            root = tree.getroot()
+        except ET.ParseError as ex:
+            self.log.exception(f"parsing error while trying to parse: {path_to_package_xml}")
+            return {}
+        
+        package_name = root.find("name")
+        version = root.find("version")
+        maintainer = root.find("maintainer")
+        maintainer_email = maintainer.attrib["email"] if maintainer is not None else ""
+        description = root.find("description")
+        license = root.find("license")
+        export = root.find("export")
+        build_type = export.find("build_type") if export is not None else None
         
         return {
             "package_xml": path_to_package_xml,
-            
-            "package_name": root.find("name").text,
-            "version": root.find("version").text,
-            "maintainer": root.find("maintainer").text,
-            "maintainer_email": root.find("maintainer").attrib["email"],
-            "description": root.find("description").text,
-            "license": root.find("license").text,
+            "package_name": package_name.text if package_name is not None else "",
+            "version": version.text if version is not None else "",
+            "maintainer": maintainer.text if maintainer is not None else "",
+            "maintainer_email": maintainer_email,
+            "description": description.text if description is not None else "",
+            "license": license.text if license is not None else "",
             "nodes": [],
-            "build_type": root.find("export").find("build_type").text,
+            "build_type": build_type.text if build_type is not None else None
         }
     
+    ################################# C / CPP #################################
 
-    ########################################### C / CPP ###########################################
+    def parse_makefile(self, package_path):
+        """
+        Parse a CMakeLists.txt file in the given package path.
+
+        :param package_path: Path of the package.
+        """
+        path_to_cmake = os.path.join(package_path, "CMakeLists.txt")
+        if not os.path.exists(path_to_cmake):
+            self.log.error(f"File not found: {path_to_cmake}")
+            return {} 
 
-    def parse_makefile(self, package_path):        
-        import re
-        path_to_cmake = f"{package_path}/CMakeLists.txt"        
-        f = open(path_to_cmake, "r")
-        package_py_content = f.read()          
-        # nodes_list = re.search("(?<=install\(TARGETS)($[\S\s]*)(?=DESTINATION)", package_py_content)
+        with open(path_to_cmake, "r") as f:
+            package_py_content = f.read() 
+ 
         matches = re.finditer(r"install\(TARGETS([\S\s]*?)DESTINATION", package_py_content, re.MULTILINE)
         
-        #(?<=install\(TARGETS)($[\S\s]*)(?=^\))
+        found_matches = False
         nodes = []
-        for matchNum, match in enumerate(matches, start=1):
-            matches = match.groups()[0].split("\n")            
+        for match in matches:
+            found_matches = True
+            matches = match.groups()[0].split()
+            if len(matches) == 0:
+                self.log.error(f"{path_to_cmake} is not formatted correctly: no targets in 'install' command.")
+                raise ValueError(f"{path_to_cmake} is not formatted correctly: no targets in 'install' command.")
+               
             for n in matches:   
                 node = n.strip()                     
                 if node == "":
                     continue             
                 if node[0] == "#":
                     continue                
                 nodes.append({                                    
                     "name": node,
                     "entry_point": "",                    
                     "path": "",
                     "parameters": []
-                })        
+                })  
+
+        if not found_matches:
+            self.log.error(f"{path_to_cmake} is not formatted correctly: no 'install' command found.")
+            raise ValueError(f"{path_to_cmake} is not formatted correctly: no 'install' command found.")
+
         return {
             "cmake": path_to_cmake,
             "nodes": nodes 
         }               
     
-
-    ########################################### Python ###########################################
+    ################################# Python ##################################
  
-    def extract_contents(self, node, global_scope):
+    def _extract_contents(self, node, global_scope):
         """
         Recursive helper function for parsing a variety of objects such as lists, function calls etc.
         Does not handle every case, such as nested functions etc. Returns None on failure.
         """
         if isinstance(node, ast.Str):
             return node.s
         elif isinstance(node, ast.Num):
             return node.n
         elif isinstance(node, ast.Name):
             return global_scope.get(node.id)
         elif isinstance(node, ast.List):
-            return [self.extract_contents(item, global_scope) for item in node.elts]
+            return [self._extract_contents(item, global_scope) for item in node.elts]
         elif isinstance(node, ast.Tuple):
-            return tuple(self.extract_contents(item, global_scope) for item in node.elts)
+            return tuple(self._extract_contents(item, global_scope) for item in node.elts)
         elif isinstance(node, ast.Dict):
-            return {self.extract_contents(key, global_scope): self.extract_contents(value, global_scope)
+            return {self._extract_contents(key, global_scope): self._extract_contents(value, global_scope)
                     for key, value in zip(node.keys, node.values)}
         elif isinstance(node, ast.BinOp):
-            return self.extract_contents(node.left, global_scope) + self.extract_contents(node.right, global_scope)
+            return self._extract_contents(node.left, global_scope) + self._extract_contents(node.right, global_scope)
         elif isinstance(node, ast.Call):
-            pos_args = tuple(self.extract_contents(arg, global_scope) for arg in node.args)
-            kw_args = tuple(f"{kw.arg}={self.extract_contents(kw.value, global_scope)}" for kw in node.keywords)
+            pos_args = tuple(self._extract_contents(arg, global_scope) for arg in node.args)
+            kw_args = tuple(f"{kw.arg}={self._extract_contents(kw.value, global_scope)}" for kw in node.keywords)
             if isinstance(node.func, ast.Name):
                 return f"{node.func.id}{pos_args+kw_args}"
             elif isinstance(node.func, ast.Attribute):
                 return f"{node.func.attr}{pos_args+kw_args}"
         elif isinstance(node, ast.Constant):
             return node.s
         else:
             return None
     
 
-    def extract_setup_parameters(self, tree, global_scope):
+    def _extract_setup_parameters(self, tree, global_scope):
+        """
+        Returns a dictionary containing the parameters in the `setup` function, 
+        by extracting them from the given syntax tree.
+        """
         for node in ast.walk(tree):
             if isinstance(node, ast.Call) and isinstance(node.func, ast.Name) and node.func.id == 'setup':
                 parameters = {}
                 for keyword in node.keywords:
                     parameter_name = keyword.arg
-                    parameter_value = self.extract_contents(keyword.value, global_scope)
+                    parameter_value = self._extract_contents(keyword.value, global_scope)
                     parameters[parameter_name] = parameter_value
                 return parameters
     
         return None
     
 
-    def populate_global_scope(self, tree):
+    def _populate_global_scope(self, tree):
+        """
+        Returns a dictionary containing variables defined globally in the given syntax tree.
+        """
         global_scope = {}
         for node in tree.body:
             if isinstance(node, ast.Assign) and len(node.targets) == 1 and isinstance(node.targets[0], ast.Name):
                 target_name = node.targets[0].id
-                target_value = self.extract_contents(node.value, global_scope)
+                target_value = self._extract_contents(node.value, global_scope)
                 global_scope[target_name] = target_value
         return global_scope
 
 
-    def parse_entry_point(self, ep):
+    def _parse_entry_point(self, ep):
         """
         Example of expected entrypoint format:
         analytic_dynamics = cannon_analytic.analytic_dynamics:main
         """
         try:
             node_name = ep.split('=')[0].strip()
             entry_point = ep.split('=')[1].strip()
@@ -148,42 +187,46 @@
             self.log.error(f"Failed to parse entry point {ep}")
             return None,None,None
 
         return node_name, entry_point, file_name 
 
 
     def parse_setup_py(self, package_path):
-        
-        path_to_setup = f"{package_path}/setup.py"  
+        """
+        Parse a setup.py file in the given package path.
+
+        :param package_path: Path of the package.
+        """
+        path_to_setup = os.path.join(package_path, "setup.py")  
 
         try:
             with open(path_to_setup, 'r') as f:
                 source = f.read()
         except FileNotFoundError as e:
             self.log.error(f"Failed to find {path_to_setup}")
             return {}
 
         tree = ast.parse(source)
-        global_scope = self.populate_global_scope(tree)
-        parameters = self.extract_setup_parameters(tree, global_scope)
+        global_scope = self._populate_global_scope(tree)
+        parameters = self._extract_setup_parameters(tree, global_scope)
 
         if not parameters:
             self.log.error("Failed to parse setup.py")
             return {}
 
         # possibly loop over the list of entry points if there is more than one.
-        node_name, entry_point, file_name = self.parse_entry_point(parameters['entry_points']['console_scripts'][0])
+        node_name, entry_point, file_name = self._parse_entry_point(parameters['entry_points']['console_scripts'][0])
 
-        package_name = package_path.split("/")[-1]
+        package_name = package_path.split(os.path.sep)[-1]
             
         nodes = []
         nodes.append({                
             "name": node_name,
             "entry_point": entry_point,                
-            "path": f"{package_path}/{package_name}/{file_name}",
+            "path": os.path.join(package_path, package_name, file_name),
             "parameters": []
         })
 
         return {
             "setup_py": path_to_setup,
             
             "package_name": package_name,
@@ -191,16 +234,15 @@
             "maintainer": parameters["maintainer"],
             "maintainer_email": parameters["maintainer_email"],
             "description": parameters["description"],
             "license": parameters["license"],
             "nodes": nodes
         }
     
-
-    ########################################### Project ###########################################
+    ################################# Project #################################
 
     def get_file_hierarchy(self, root_dir, file_list):
         """
         Returns the file hierarchy of the given directory, and the contents of the given files.
 
         Args:
             root_dir: full path to the directory in question.
@@ -249,32 +291,35 @@
                     else:
                         with open(file_path, 'r') as file:
                             file_contents.append(file.read())
 
         return hierarchy, file_contents
 
 
-    def get_project_packages(self, project_path, workspace=""):                
+    def get_project_packages(self, project_path, workspace=""):
+        """
+        Collects packages metadata (nodes, parameters etc.)
+        """              
         self.log.debug(f" + get_project_packages {project_path}/{workspace}")
         
-        package_paths = glob.glob(f"{project_path}/src/*")                
+        package_paths = glob.glob(os.path.join(project_path, "src", "*"))                
         if workspace != "":
-            package_paths = glob.glob(f"{project_path}/{workspace}/src/*") + package_paths            
+            package_paths = glob.glob(os.path.join(project_path, workspace, "src","*")) + package_paths        
         
+        # Exclude ROS2 system packages
         package_paths = [p for p in package_paths if 'ros2.' not in p]
         
         packages = []
         for package_path in package_paths:            
-            # package_py = f"{'/'.join(package_path.split('/')[:-1])}/setup.py"
             self.log.debug(f"package_path: {package_path}")
             
             parsed_data = None     
             try:
                 parsed_data = self.parse_xml(package_path)
-            except Exception as e:
+            except ET.ParseError as e:
                 print(f"{package_path} doesn't contain xml, probably not a package. skipping.")
                 continue
             
             if parsed_data["build_type"] == "ament_python":                
                 temp = self.parse_setup_py(package_path)
                 parsed_data["nodes"] = temp["nodes"]                
                 parsed_data["setup_py"] = temp["setup_py"]
@@ -285,105 +330,111 @@
                 parsed_data["cmake"] = temp["cmake"]                
                 
             else:
                 self.log.exception(f"Method {parsed_data['build_type']} not allowed")
                 raise Exception(f"Method {parsed_data['build_type']} not allowed")
 
             node_parameters = {}
-            try:
-                path_to_config =  f"{package_path}/config/params.yaml"            
+            path_to_config =  os.path.join(package_path, "config","params.yaml")            
+            if os.path.exists(path_to_config):
                 with open(path_to_config, 'r') as config_file:
-                    config = yaml.full_load(config_file)                    
+                    try:
+                        config = yaml.safe_load(config_file)
+                    except yaml.YAMLError as ye:
+                        self.log.exception(f"Error parsing params.yaml in package {package_path}: {ye}")
+                        raise ye       
                     
                 for node_name, val in config.items():
-                    par_dict = val["ros__parameters"]                    
+                    par_dict = val.get("ros__parameters", {})                 
                     node_parameters[node_name] = []
                     for key, val in par_dict.items():
                         node_parameters[node_name].append({                            
                             "name":key,
                             "parameterType": type(val).__name__, # TODO: Fix type
                             "value": val,
                             "description": "Parameter loaded from config.yaml",                            
                         })
-                for node in parsed_data["nodes"]:
-                    # print(f"adding parameters to [{node['name']}] node")                
-                    node["parameters"] = node_parameters.get(node["name"], [])                    
-            except Exception as e:
-                self.log.exception(e)
+                for node in parsed_data["nodes"]:               
+                    node["parameters"] = node_parameters.get(node["name"], [])  
+                              
+            else:
+                self.log.info(f"no parameters.yaml file for package {package_path}")
 
-            packages.append({
-                # "id": uuid.uuid4(),                
+            packages.append({               
                 "name": parsed_data["package_name"],
                 "cover": "",
                 "path": package_path,
                 "setup_py": parsed_data.get("setup_py", ""),
-                "package_xml": parsed_data.get("package_xml"),
-                "maintainer": parsed_data.get("maintainer"),
-                "maintainer_email" : parsed_data.get("maintainer_email"),
-                "description": parsed_data.get("description"),
-                "license": parsed_data.get("license"),
+                "package_xml": parsed_data.get("package_xml", ""),
+                "maintainer": parsed_data.get("maintainer", ""),
+                "maintainer_email" : parsed_data.get("maintainer_email", ""),
+                "description": parsed_data.get("description", ""),
+                "license": parsed_data.get("license", ""),
 
-                "readme": f"{package_path}/README.md",
+                "readme": f"{package_path}{os.path.sep}README.md",
                 "git": "", #TODO
                 
                 "launches": self.get_project_launch_files(package_path),
-                "nodes": parsed_data.get("nodes"),                
+                "nodes": parsed_data.get("nodes", []),
             })
+            
         return packages
 
 
     def get_project_launch_files(self, package_path, workspace=""):
-        #TODO: check if done. 
-        launch_paths = glob.glob(f"{package_path}/launch/*.py")
+        """
+        Collects all the *.launch.py files in the 'launch' directory.
+        """
+        launch_paths = glob.glob(os.path.join(package_path, "launch", "*.py"))
         if workspace != "":
-            launch_paths + glob.glob(f"{package_path}/{workspace}/src/*.py")
+            launch_paths + glob.glob(os.path.join(package_path, workspace, "src", "*.py"))
         
         launch_paths = [p for p in launch_paths if 'ros2.' not in p]
         
         launch_files = []
         for launch_path in launch_paths:
             launch_files.append({                
-                "name": launch_path.split("/")[-1],
+                "name": launch_path.split(os.path.sep)[-1],
                 "path": launch_path,
 
                 # "tags": [],
                 "description": "",                
             })
         return launch_files
 
 
     def get_git_remote_url(self, project_path):
         """
         Assumption: The user is using github as the remote backup, and the name of the remote is 'origin'.
         """
         try:
-            command = 'echo $REMOTE_CONTAINERS'
-            result = subprocess.check_output(command, shell=True, executable='/bin/bash').decode().strip()
-            if result == "true":
-                self.log.info("Inside devcontainer. Cannot communicate with github.")
+            if os.environ.get('REMOTE_CONTAINERS', '') == "true":
+                self.log.info("Inside devcontainer. Cannot communicate with GitHub.")
                 return ""
 
-            os.chdir(project_path)
-            result = subprocess.run(["git", "remote", "get-url", "origin"], capture_output=True, text=True).stdout.strip()
+            result = subprocess.run(["git", "-C", project_path, "remote", "get-url", "origin"], capture_output=True, text=True).stdout.strip()
         except Exception as e:
             self.log.exception(e)
             return ""
         
         # sanity check
         if result.startswith("git@github.com:") and result.endswith(".git"):
             return result
         else:
             self.log.error("Could not obtain git remote url for path " + project_path)
             return ""
         
 
     def get_git_local_hash(self, project_path):
-        os.chdir(project_path)
-        result = subprocess.run(["git", "rev-parse", "HEAD"], capture_output=True, text=True)
-        result = result.stdout.strip()
+        try:
+            result = subprocess.run(["git", "-C", project_path, "rev-parse", "HEAD"], capture_output=True, text=True)
+            result = result.stdout.strip()
+        except Exception as e:
+            self.log.exception(e)
+            return None
 
         # sanity check
         if len(result) == 40:
             return result
         else:
             self.log.error("Could not obtain git hash for local path " + project_path)
             return None
@@ -395,53 +446,63 @@
 
 
     def get_file_content(self, path):
         try:
             with open(path, 'r') as f:
                 content = f.read()
             return content
-        except FileNotFoundError as e:
-            self.log.error(f"could not find file {path}")
+        except Exception as e:
+            self.log.error(f"could not open file {path}")
             return ""        
     
 
-    def parse(self, project_path, project_name, workspaces=["", "ros_ws"]):       
+    def _setup_project(self, project_name, project_path):
+        self.project = {                          
+            "cover": "",
+            "name": project_name,
+            "image": project_name,
+            "tags": [],
+            "is_active": True,
+            "description": "",                 
+            "git": self.get_git_remote_url(project_path), 
+            "path": project_path,    
+                            
+            "packages": None,                
+            "launches": None,
+
+            "readme": None,
+            "license":None
+        }
+
+
+    def parse(self, project_path, project_name, workspaces=["", "ros_ws"]):
+        """
+        parse the project with the given name under the given path.
+
+        Returns:
+        a dictionary holding all metadata for the project.
+        """    
         packages = []
         launches = []
 
         # remove duplicates
         workspaces = list(set(workspaces))
 
         # remove non-existing workspaces
-        workspaces = [ws for ws in workspaces if os.path.isdir(f"./{ws}")]
+        workspaces = [ws for ws in workspaces if os.path.isdir(os.path.join(".",ws))]
         
         for w in workspaces:
             packages = packages + self.get_project_packages(project_path, workspace=w)
             launches = launches + self.get_project_launch_files(project_path, workspace=w)
                         
         if not self.project:
-            self.project = {                          
-                "cover": "",
-                "name": project_name,
-                "image": project_name,
-                "tags": [],
-                "is_active": True,
-                "description": "",                 
-                "git": self.get_git_remote_url(project_path), 
-                "path": project_path,    
-                                
-                "packages": None,                
-                "launches": None,
-
-                "readme": None,
-                "license":None
-            }
-        
+            self._setup_project(project_name, project_path)
+    
         self.project["description"] = self.get_project_description(project_path)
         self.project["packages"] = packages
         self.project["launches"] = launches
-        self.project["readme"] = self.get_file_content(f"{project_path}/README.md")
-        self.project["license"] = self.get_file_content(f"{project_path}/LICENSE")
+        self.project["readme"] = self.get_file_content(os.path.join(project_path, "README.md"))
+        self.project["license"] = self.get_file_content(os.path.join(project_path,"LICENSE"))
         
         return self.project
```

### Comparing `citros-23.22.2/citros/rosbag/__init__.py` & `citros-23.23.1/citros/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/rosbag/reader_base.py` & `citros-23.23.1/citros/rosbag/reader_base.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/rosbag/reader_mcap.py` & `citros-23.23.1/citros/rosbag/reader_mcap.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros/rosbag/reader_sqlite.py` & `citros-23.23.1/citros/rosbag/reader_sqlite.py`

 * *Files identical despite different names*

### Comparing `citros-23.22.2/citros.egg-info/PKG-INFO` & `citros-23.23.1/citros.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: citros
-Version: 23.22.2
+Version: 23.23.1
 Summary: A cli entrypoint for the citros system.
 Home-page: http://pypi.python.org/pypi/citros_cli/
 Author: vovacooper
 Author-email: vova@lulav.space
 License: LICENSE.txt
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -56,14 +56,25 @@
 
     Install the package from the current directory, directly to a global bin folder 
 
         python3 -m pip install .
     
     (should be done before uploading to PyPI, to make sure the installation is working properly).
 
+4. Env
+
+| ENV | Description | used in |
+| --- | --- | --- |
+| `CITROS_DOMAIN` | the main domain, default is `citros.io` | all packages |
+| `CITROS_DATA_HOST` | host of the playground PGDB, default comes from simulation job env (citros_worker) and is: `shared-playground-postgresql.ns-citros-shared`. used for uploading BAG. | citros_bag |
+| `CITROS_DATA_PORT` | the port of PGDB, default `5432` | citros_bag |
+| `CITROS_DATA_DATABASE` | the database to access inside PGDB. default comes from simulation job env (citros_worker) and is: `domain_prefix`. used for uploading BAG. | citros_bag |
+| `CITROS_DATA_USERNAME` | the username to access PGDB, default `citros_anonymous`. the username is the username from citros.  | citros_bag |
+| `CITROS_DATA_PASSWORD` | the password to access PGDB, default `citros_anonymous`. the password is the id of the user in `citros.user` table.  | citros_bag |
+
 # CLI API commands:
 
 ## login
 Login to CITROS.
 
 After entering the command, you will be prompted for your email (the username) and password.
```

### Comparing `citros-23.22.2/citros.egg-info/SOURCES.txt` & `citros-23.23.1/citros.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -24,9 +24,10 @@
 citros/parsers/__init__.py
 citros/parsers/parser_base.py
 citros/parsers/parser_ros2.py
 citros/rosbag/__init__.py
 citros/rosbag/reader_base.py
 citros/rosbag/reader_mcap.py
 citros/rosbag/reader_sqlite.py
-tests/test_parse_ros_project.py
-tests/test_uplosd_to_server.py
+tests/test_parse_makefile.py
+tests/test_parse_setup_py.py
+tests/test_parse_xml.py
```

### Comparing `citros-23.22.2/setup.py` & `citros-23.23.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,11 +46,13 @@
         'python-decouple',
         'requests_toolbelt',
         'soupsieve',
         'bs4',
         'zipp',
         'pyjwt',
         'psycopg2-binary',
-        'urllib3>=1.26'
+        'urllib3>=1.26',
+        'InquirerPy',
+        'faker'
     ],
     py_modules=['citros', 'citros_meta']
 )
```

