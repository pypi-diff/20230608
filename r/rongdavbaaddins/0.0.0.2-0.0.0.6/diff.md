# Comparing `tmp/rongdavbaaddins-0.0.0.2.tar.gz` & `tmp/rongdavbaaddins-0.0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.0.2.tar", last modified: Fri Jun  2 08:20:42 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.0.6.tar", last modified: Thu Jun  8 02:23:43 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.0.2.tar` & `rongdavbaaddins-0.0.0.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.389924 rongdavbaaddins-0.0.0.2/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0      397 2023-06-02 08:20:42.389924 rongdavbaaddins-0.0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.329888 rongdavbaaddins-0.0.0.2/rongdavbaaddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/Excel.officeUI
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/Vbalog.pyd
--rw-rw-rw-   0        0        0     1041 2023-05-29 08:29:49.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/__init__.py
--rw-rw-rw-   0        0        0     2596 2023-06-01 06:14:19.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/getNumber.py
--rw-rw-rw-   0        0        0      368 2023-05-31 09:29:33.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/getNumberpy.py
--rw-rw-rw-   0        0        0     2076 2023-06-01 02:55:54.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/minusFunction.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.355890 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/
--rw-rw-rw-   0        0        0    90081 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/__init__.py
--rw-rw-rw-   0        0        0    30117 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_common.py
--rw-rw-rw-   0        0        0    15475 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_compat.py
--rw-rw-rw-   0        0        0    19220 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psaix.py
--rw-rw-rw-   0        0        0    32696 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psbsd.py
--rw-rw-rw-   0        0        0    89178 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pslinux.py
--rw-rw-rw-   0        0        0    16818 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psosx.py
--rw-rw-rw-   0        0        0     8477 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psposix.py
--rw-rw-rw-   0        0        0    26213 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pssunos.py
--rw-rw-rw-   0        0        0    78336 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psutil_windows.pyd
--rw-rw-rw-   0        0        0    38545 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pswindows.py
-drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.387888 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/
--rw-rw-rw-   0        0        0    61064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/__init__.py
--rw-rw-rw-   0        0        0      308 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/__main__.py
--rw-rw-rw-   0        0        0    11554 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/runner.py
--rw-rw-rw-   0        0        0     4630 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_aix.py
--rw-rw-rw-   0        0        0    21638 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_bsd.py
--rw-rw-rw-   0        0        0    21458 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_connections.py
--rw-rw-rw-   0        0        0    28501 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_contracts.py
--rw-rw-rw-   0        0        0    97598 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_linux.py
--rw-rw-rw-   0        0        0    15520 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_memleaks.py
--rw-rw-rw-   0        0        0    35604 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_misc.py
--rw-rw-rw-   0        0        0     6791 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_osx.py
--rw-rw-rw-   0        0        0    17487 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_posix.py
--rw-rw-rw-   0        0        0    64702 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_process.py
--rw-rw-rw-   0        0        0     1379 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_sunos.py
--rw-rw-rw-   0        0        0    36812 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_system.py
--rw-rw-rw-   0        0        0    15064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_testutils.py
--rw-rw-rw-   0        0        0    12576 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_unicode.py
--rw-rw-rw-   0        0        0    36065 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_windows.py
--rw-rw-rw-   0        0        0    10397 2023-06-02 06:35:19.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/rongdaVbaAddins.py
--rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      156 2023-05-29 09:14:34.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/vbaloginpy.py
--rw-rw-rw-   0        0        0    26574 2023-06-01 06:58:31.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins/荣大工具箱.xlam
-drwxrwxrwx   0        0        0        0 2023-06-02 08:20:42.335885 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      397 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1716 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-02 08:20:42.000000 rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-02 08:20:42.391887 rongdavbaaddins-0.0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1003 2023-06-02 08:20:11.000000 rongdavbaaddins-0.0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.191861 rongdavbaaddins-0.0.0.6/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.6/MANIFEST.in
+-rw-rw-rw-   0        0        0      409 2023-06-08 02:23:43.191861 rongdavbaaddins-0.0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.018964 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Excel.officeUI
+-rw-rw-rw-   0        0        0   107702 2023-06-07 08:07:55.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/RDaddins.xlam
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0      812 2023-06-07 02:06:12.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      384 2023-06-07 01:55:36.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-07 01:54:22.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/minusFunction.pyd
+drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.075858 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/
+-rw-rw-rw-   0        0        0    90160 2023-06-08 02:07:36.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/__init__.py
+-rw-rw-rw-   0        0        0    30117 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_common.py
+-rw-rw-rw-   0        0        0    15475 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_compat.py
+-rw-rw-rw-   0        0        0    19220 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psaix.py
+-rw-rw-rw-   0        0        0    32696 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psbsd.py
+-rw-rw-rw-   0        0        0    89178 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pslinux.py
+-rw-rw-rw-   0        0        0    16818 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psosx.py
+-rw-rw-rw-   0        0        0     8477 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psposix.py
+-rw-rw-rw-   0        0        0    26213 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pssunos.py
+-rw-rw-rw-   0        0        0    78336 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psutil_windows.pyd
+-rw-rw-rw-   0        0        0    38545 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pswindows.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.164850 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/
+-rw-rw-rw-   0        0        0    61064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/__main__.py
+-rw-rw-rw-   0        0        0    11554 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/runner.py
+-rw-rw-rw-   0        0        0     4630 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_aix.py
+-rw-rw-rw-   0        0        0    21638 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_bsd.py
+-rw-rw-rw-   0        0        0    21458 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_connections.py
+-rw-rw-rw-   0        0        0    28501 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_contracts.py
+-rw-rw-rw-   0        0        0    97598 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_linux.py
+-rw-rw-rw-   0        0        0    15520 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_memleaks.py
+-rw-rw-rw-   0        0        0    35604 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_misc.py
+-rw-rw-rw-   0        0        0     6791 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_osx.py
+-rw-rw-rw-   0        0        0    17487 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_posix.py
+-rw-rw-rw-   0        0        0    64702 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_process.py
+-rw-rw-rw-   0        0        0     1379 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_sunos.py
+-rw-rw-rw-   0        0        0    36812 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_system.py
+-rw-rw-rw-   0        0        0    15064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_testutils.py
+-rw-rw-rw-   0        0        0    12576 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_unicode.py
+-rw-rw-rw-   0        0        0    36065 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_windows.py
+-rw-rw-rw-   0        0        0   125952 2023-06-08 02:22:53.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/rongdaVbaAddins.pyd
+-rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      156 2023-06-07 01:12:56.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/vbaloginpy.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.185817 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1712 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-08 02:23:43.194807 rongdavbaaddins-0.0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1023 2023-06-08 02:21:52.000000 rongdavbaaddins-0.0.0.6/setup.py
```

### Comparing `rongdavbaaddins-0.0.0.2/LICENSE.txt` & `rongdavbaaddins-0.0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/Excel.officeUI` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/__init__.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,16 +16,19 @@
  - NetBSD
  - Sun Solaris
  - AIX
 
 Works with Python versions 2.7 and 3.4+.
 """
 
-from __future__ import division
 
+
+from __future__ import division
+import sys, os
+sys.path.append(os.path.dirname(os.path.abspath(__file__)))
 import collections
 import contextlib
 import datetime
 import functools
 import os
 import signal
 import subprocess
```

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_common.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_common.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_compat.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_compat.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psaix.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psaix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psbsd.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psbsd.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pslinux.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pslinux.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psosx.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psosx.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_psposix.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psposix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pssunos.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pssunos.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/_pswindows.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pswindows.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/__init__.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/runner.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/runner.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_aix.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_aix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_bsd.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_bsd.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_connections.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_contracts.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_linux.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_linux.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_memleaks.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_memleaks.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_misc.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_osx.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_osx.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_posix.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_process.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_sunos.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_sunos.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_system.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_testutils.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_unicode.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins/psutil/tests/test_windows.py` & `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.2/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 LICENSE.txt
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
-rongdavbaaddins/Excel.officeUI
-rongdavbaaddins/Vbalog.pyd
-rongdavbaaddins/Vbalogpy.py
-rongdavbaaddins/__init__.py
-rongdavbaaddins/getNumber.py
-rongdavbaaddins/getNumberpy.py
-rongdavbaaddins/minusFunction.py
-rongdavbaaddins/rongdaVbaAddins.py
-rongdavbaaddins/vbaLogin.pyd
-rongdavbaaddins/vbaloginpy.py
-rongdavbaaddins/荣大工具箱.xlam
+rongdaVbaAddins/Excel.officeUI
+rongdaVbaAddins/RDaddins.xlam
+rongdaVbaAddins/Vbalog.pyd
+rongdaVbaAddins/Vbalogpy.py
+rongdaVbaAddins/__init__.py
+rongdaVbaAddins/getNumber.pyd
+rongdaVbaAddins/getNumberpy.py
+rongdaVbaAddins/minusFunction.pyd
+rongdaVbaAddins/rongdaVbaAddins.pyd
+rongdaVbaAddins/vbaLogin.pyd
+rongdaVbaAddins/vbaloginpy.py
+rongdaVbaAddins/psutil/__init__.py
+rongdaVbaAddins/psutil/_common.py
+rongdaVbaAddins/psutil/_compat.py
+rongdaVbaAddins/psutil/_psaix.py
+rongdaVbaAddins/psutil/_psbsd.py
+rongdaVbaAddins/psutil/_pslinux.py
+rongdaVbaAddins/psutil/_psosx.py
+rongdaVbaAddins/psutil/_psposix.py
+rongdaVbaAddins/psutil/_pssunos.py
+rongdaVbaAddins/psutil/_psutil_windows.pyd
+rongdaVbaAddins/psutil/_pswindows.py
+rongdaVbaAddins/psutil/tests/__init__.py
+rongdaVbaAddins/psutil/tests/__main__.py
+rongdaVbaAddins/psutil/tests/runner.py
+rongdaVbaAddins/psutil/tests/test_aix.py
+rongdaVbaAddins/psutil/tests/test_bsd.py
+rongdaVbaAddins/psutil/tests/test_connections.py
+rongdaVbaAddins/psutil/tests/test_contracts.py
+rongdaVbaAddins/psutil/tests/test_linux.py
+rongdaVbaAddins/psutil/tests/test_memleaks.py
+rongdaVbaAddins/psutil/tests/test_misc.py
+rongdaVbaAddins/psutil/tests/test_osx.py
+rongdaVbaAddins/psutil/tests/test_posix.py
+rongdaVbaAddins/psutil/tests/test_process.py
+rongdaVbaAddins/psutil/tests/test_sunos.py
+rongdaVbaAddins/psutil/tests/test_system.py
+rongdaVbaAddins/psutil/tests/test_testutils.py
+rongdaVbaAddins/psutil/tests/test_unicode.py
+rongdaVbaAddins/psutil/tests/test_windows.py
 rongdavbaaddins.egg-info/PKG-INFO
 rongdavbaaddins.egg-info/SOURCES.txt
 rongdavbaaddins.egg-info/dependency_links.txt
-rongdavbaaddins.egg-info/top_level.txt
-rongdavbaaddins/psutil/__init__.py
-rongdavbaaddins/psutil/_common.py
-rongdavbaaddins/psutil/_compat.py
-rongdavbaaddins/psutil/_psaix.py
-rongdavbaaddins/psutil/_psbsd.py
-rongdavbaaddins/psutil/_pslinux.py
-rongdavbaaddins/psutil/_psosx.py
-rongdavbaaddins/psutil/_psposix.py
-rongdavbaaddins/psutil/_pssunos.py
-rongdavbaaddins/psutil/_psutil_windows.pyd
-rongdavbaaddins/psutil/_pswindows.py
-rongdavbaaddins/psutil/tests/__init__.py
-rongdavbaaddins/psutil/tests/__main__.py
-rongdavbaaddins/psutil/tests/runner.py
-rongdavbaaddins/psutil/tests/test_aix.py
-rongdavbaaddins/psutil/tests/test_bsd.py
-rongdavbaaddins/psutil/tests/test_connections.py
-rongdavbaaddins/psutil/tests/test_contracts.py
-rongdavbaaddins/psutil/tests/test_linux.py
-rongdavbaaddins/psutil/tests/test_memleaks.py
-rongdavbaaddins/psutil/tests/test_misc.py
-rongdavbaaddins/psutil/tests/test_osx.py
-rongdavbaaddins/psutil/tests/test_posix.py
-rongdavbaaddins/psutil/tests/test_process.py
-rongdavbaaddins/psutil/tests/test_sunos.py
-rongdavbaaddins/psutil/tests/test_system.py
-rongdavbaaddins/psutil/tests/test_testutils.py
-rongdavbaaddins/psutil/tests/test_unicode.py
-rongdavbaaddins/psutil/tests/test_windows.py
+rongdavbaaddins.egg-info/top_level.txt
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `rongdavbaaddins-0.0.0.2/setup.py` & `rongdavbaaddins-0.0.0.6/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.2"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.6"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
     author="wangweidong",
     author_email="17891967090@163.com",
-    description='创建文件夹',
+    description='荣大工具箱-Excel插件',
     long_description_content_type="text/markdown",
     url='https://alidocs.dingtalk.com/i/p/4oJRz0VRJyvmLZMydy0mV7WvjQn7MG89',
     long_description=open('README.md', encoding="utf-8").read(),
     python_requires=">=3.8",
     install_requires=get_install_requires(),
 
     packages=find_packages(),
     # license = '',
     classifiers=[
         'Programming Language :: Python',
 
     ],
     # 包含的类型
-    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm', '*.xlam', '*.officeUI']},  # 这个很重要
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm', '*.xlam', '*.officeUI','.xlsx']},  # 这个很重要
     include_package_data=True  # 也选上
 
 )
```

