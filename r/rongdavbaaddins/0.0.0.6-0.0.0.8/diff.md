# Comparing `tmp/rongdavbaaddins-0.0.0.6.tar.gz` & `tmp/rongdavbaaddins-0.0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rongdavbaaddins-0.0.0.6.tar", last modified: Thu Jun  8 02:23:43 2023, max compression
+gzip compressed data, was "rongdavbaaddins-0.0.0.8.tar", last modified: Thu Jun  8 02:52:59 2023, max compression
```

## Comparing `rongdavbaaddins-0.0.0.6.tar` & `rongdavbaaddins-0.0.0.8.tar`

### file list

```diff
@@ -1,55 +1,63 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.191861 rongdavbaaddins-0.0.0.6/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.6/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.6/MANIFEST.in
--rw-rw-rw-   0        0        0      409 2023-06-08 02:23:43.191861 rongdavbaaddins-0.0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.018964 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/
--rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Excel.officeUI
--rw-rw-rw-   0        0        0   107702 2023-06-07 08:07:55.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/RDaddins.xlam
--rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Vbalog.pyd
--rw-rw-rw-   0        0        0      812 2023-06-07 02:06:12.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Vbalogpy.py
--rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/__init__.py
--rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/getNumber.pyd
--rw-rw-rw-   0        0        0      384 2023-06-07 01:55:36.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/getNumberpy.py
--rw-rw-rw-   0        0        0    41984 2023-06-07 01:54:22.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/minusFunction.pyd
-drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.075858 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/
--rw-rw-rw-   0        0        0    90160 2023-06-08 02:07:36.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/__init__.py
--rw-rw-rw-   0        0        0    30117 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_common.py
--rw-rw-rw-   0        0        0    15475 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_compat.py
--rw-rw-rw-   0        0        0    19220 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psaix.py
--rw-rw-rw-   0        0        0    32696 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psbsd.py
--rw-rw-rw-   0        0        0    89178 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pslinux.py
--rw-rw-rw-   0        0        0    16818 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psosx.py
--rw-rw-rw-   0        0        0     8477 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psposix.py
--rw-rw-rw-   0        0        0    26213 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pssunos.py
--rw-rw-rw-   0        0        0    78336 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psutil_windows.pyd
--rw-rw-rw-   0        0        0    38545 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pswindows.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.164850 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/
--rw-rw-rw-   0        0        0    61064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/__init__.py
--rw-rw-rw-   0        0        0      308 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/__main__.py
--rw-rw-rw-   0        0        0    11554 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/runner.py
--rw-rw-rw-   0        0        0     4630 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_aix.py
--rw-rw-rw-   0        0        0    21638 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_bsd.py
--rw-rw-rw-   0        0        0    21458 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_connections.py
--rw-rw-rw-   0        0        0    28501 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_contracts.py
--rw-rw-rw-   0        0        0    97598 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_linux.py
--rw-rw-rw-   0        0        0    15520 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_memleaks.py
--rw-rw-rw-   0        0        0    35604 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_misc.py
--rw-rw-rw-   0        0        0     6791 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_osx.py
--rw-rw-rw-   0        0        0    17487 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_posix.py
--rw-rw-rw-   0        0        0    64702 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_process.py
--rw-rw-rw-   0        0        0     1379 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_sunos.py
--rw-rw-rw-   0        0        0    36812 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_system.py
--rw-rw-rw-   0        0        0    15064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_testutils.py
--rw-rw-rw-   0        0        0    12576 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_unicode.py
--rw-rw-rw-   0        0        0    36065 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_windows.py
--rw-rw-rw-   0        0        0   125952 2023-06-08 02:22:53.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/rongdaVbaAddins.pyd
--rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/vbaLogin.pyd
--rw-rw-rw-   0        0        0      156 2023-06-07 01:12:56.000000 rongdavbaaddins-0.0.0.6/rongdaVbaAddins/vbaloginpy.py
-drwxrwxrwx   0        0        0        0 2023-06-08 02:23:43.185817 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/
--rw-rw-rw-   0        0        0      409 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1712 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-06-08 02:23:42.000000 rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      136 2023-06-08 02:23:43.194807 rongdavbaaddins-0.0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1023 2023-06-08 02:21:52.000000 rongdavbaaddins-0.0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.375619 rongdavbaaddins-0.0.0.8/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 rongdavbaaddins-0.0.0.8/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 rongdavbaaddins-0.0.0.8/MANIFEST.in
+-rw-rw-rw-   0        0        0      409 2023-06-08 02:52:59.376606 rongdavbaaddins-0.0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 rongdavbaaddins-0.0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.190605 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/
+-rw-rw-rw-   0        0        0    15227 2023-06-02 06:14:22.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Excel.officeUI
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.205613 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:12.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/__init__.py
+-rw-rw-rw-   0        0        0    41472 2023-06-01 02:58:27.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/minusFunction.pyd
+-rw-rw-rw-   0        0        0      204 2023-06-01 03:01:41.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Function/minusFunctionpy.py
+-rw-rw-rw-   0        0        0   107702 2023-06-07 08:07:55.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/RDaddins.xlam
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.213601 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/
+-rw-rw-rw-   0        0        0        0 2023-06-08 02:38:04.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/__init__.py
+-rw-rw-rw-   0        0        0     3281 2023-06-07 05:42:04.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
+-rw-rw-rw-   0        0        0    54784 2023-05-31 09:26:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Vbalog.pyd
+-rw-rw-rw-   0        0        0      999 2023-06-07 09:28:00.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Vbalogpy.py
+-rw-rw-rw-   0        0        0        0 2023-06-01 01:46:56.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/__init__.py
+-rw-rw-rw-   0        0        0    48640 2023-06-08 01:57:00.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/getNumber.pyd
+-rw-rw-rw-   0        0        0      372 2023-06-08 01:57:56.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/getNumberpy.py
+-rw-rw-rw-   0        0        0    41984 2023-06-08 01:39:24.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/minusFunction.pyd
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.263605 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/
+-rw-rw-rw-   0        0        0    90160 2023-06-08 02:07:36.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/__init__.py
+-rw-rw-rw-   0        0        0    30117 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_common.py
+-rw-rw-rw-   0        0        0    15475 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_compat.py
+-rw-rw-rw-   0        0        0    19253 2023-06-08 02:39:18.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psaix.py
+-rw-rw-rw-   0        0        0    32729 2023-06-08 02:40:14.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psbsd.py
+-rw-rw-rw-   0        0        0    89211 2023-06-08 02:49:21.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pslinux.py
+-rw-rw-rw-   0        0        0    16851 2023-06-08 02:40:14.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psosx.py
+-rw-rw-rw-   0        0        0     8477 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psposix.py
+-rw-rw-rw-   0        0        0    26246 2023-06-08 02:40:14.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pssunos.py
+-rw-rw-rw-   0        0        0    78336 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psutil_windows.pyd
+-rw-rw-rw-   0        0        0    38545 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pswindows.py
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.353603 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/
+-rw-rw-rw-   0        0        0    61064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/__init__.py
+-rw-rw-rw-   0        0        0      308 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/__main__.py
+-rw-rw-rw-   0        0        0    11554 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/runner.py
+-rw-rw-rw-   0        0        0     4630 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_aix.py
+-rw-rw-rw-   0        0        0    21638 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_bsd.py
+-rw-rw-rw-   0        0        0    21458 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_connections.py
+-rw-rw-rw-   0        0        0    28501 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_contracts.py
+-rw-rw-rw-   0        0        0    97598 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_linux.py
+-rw-rw-rw-   0        0        0    15520 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_memleaks.py
+-rw-rw-rw-   0        0        0    35604 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_misc.py
+-rw-rw-rw-   0        0        0     6791 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_osx.py
+-rw-rw-rw-   0        0        0    17487 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_posix.py
+-rw-rw-rw-   0        0        0    64702 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_process.py
+-rw-rw-rw-   0        0        0     1379 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_sunos.py
+-rw-rw-rw-   0        0        0    36812 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_system.py
+-rw-rw-rw-   0        0        0    15064 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_testutils.py
+-rw-rw-rw-   0        0        0    12576 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_unicode.py
+-rw-rw-rw-   0        0        0    36065 2023-06-02 01:19:30.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_windows.py
+-rw-rw-rw-   0        0        0   125952 2023-06-08 02:52:28.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/rongdaVbaAddins.pyd
+-rw-rw-rw-   0        0        0    69632 2023-05-31 09:26:36.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/vbaLogin.pyd
+-rw-rw-rw-   0        0        0      289 2023-06-07 09:28:00.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/vbaloginpy.py
+-rw-rw-rw-   0        0        0    27804 2023-06-07 02:50:03.000000 rongdavbaaddins-0.0.0.8/rongdaVbaAddins/文件处理类模板.xlsx
+drwxrwxrwx   0        0        0        0 2023-06-08 02:52:59.371604 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/
+-rw-rw-rw-   0        0        0      409 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1950 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 02:52:59.000000 rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      136 2023-06-08 02:52:59.378607 rongdavbaaddins-0.0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0     1024 2023-06-08 02:52:44.000000 rongdavbaaddins-0.0.0.8/setup.py
```

### Comparing `rongdavbaaddins-0.0.0.6/LICENSE.txt` & `rongdavbaaddins-0.0.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Excel.officeUI` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Excel.officeUI`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/RDaddins.xlam` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/RDaddins.xlam`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/Vbalogpy.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/Vbalogpy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,18 @@
-from Vbalog import FunctionLog
-from minusFunction import minusFunction
+import traceback
+
+try:
+    from Vbalog import FunctionLog
+    from minusFunction import minusFunction
+except
+    try:
+        from .Vbalog import FunctionLog
+        from .minusFunction import minusFunction
+    except:
+        traceback.print_exc()
 import sys, datetime
 if __name__ == "__main__":
     FuncitonId = sys.argv[1]
     token = sys.argv[2]
     useNumber = sys.argv[3]
     details = sys.argv[4]
     functionName = sys.argv[5]
```

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/__init__.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/__init__.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_common.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_common.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_compat.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_compat.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psaix.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psaix.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,16 +12,19 @@
 import re
 import subprocess
 import sys
 from collections import namedtuple
 
 from . import _common
 from . import _psposix
-from . import _psutil_aix as cext
-from . import _psutil_posix as cext_posix
+try:
+    from . import _psutil_aix as cext
+    from . import _psutil_posix as cext_posix
+except:
+    pass
 from ._common import NIC_DUPLEX_FULL
 from ._common import NIC_DUPLEX_HALF
 from ._common import NIC_DUPLEX_UNKNOWN
 from ._common import AccessDenied
 from ._common import NoSuchProcess
 from ._common import ZombieProcess
 from ._common import conn_to_ntuple
```

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psbsd.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psbsd.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,16 +10,19 @@
 import os
 import xml.etree.ElementTree as ET
 from collections import defaultdict
 from collections import namedtuple
 
 from . import _common
 from . import _psposix
-from . import _psutil_bsd as cext
-from . import _psutil_posix as cext_posix
+try:
+    from . import _psutil_bsd as cext
+    from . import _psutil_posix as cext_posix
+except:
+    pass
 from ._common import FREEBSD
 from ._common import NETBSD
 from ._common import OPENBSD
 from ._common import AccessDenied
 from ._common import NoSuchProcess
 from ._common import ZombieProcess
 from ._common import conn_tmap
```

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pslinux.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pslinux.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,16 +19,19 @@
 import traceback
 import warnings
 from collections import defaultdict
 from collections import namedtuple
 
 from . import _common
 from . import _psposix
-from . import _psutil_linux as cext
-from . import _psutil_posix as cext_posix
+try:
+    from . import _psutil_linux as cext
+    from . import _psutil_posix as cext_posix
+except:
+    pass
 from ._common import NIC_DUPLEX_FULL
 from ._common import NIC_DUPLEX_HALF
 from ._common import NIC_DUPLEX_UNKNOWN
 from ._common import AccessDenied
 from ._common import NoSuchProcess
 from ._common import ZombieProcess
 from ._common import bcat
```

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psosx.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psosx.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,16 +7,19 @@
 import errno
 import functools
 import os
 from collections import namedtuple
 
 from . import _common
 from . import _psposix
-from . import _psutil_osx as cext
-from . import _psutil_posix as cext_posix
+try:
+    from . import _psutil_osx as cext
+    from . import _psutil_posix as cext_posix
+except:
+    pass
 from ._common import AccessDenied
 from ._common import NoSuchProcess
 from ._common import ZombieProcess
 from ._common import conn_tmap
 from ._common import conn_to_ntuple
 from ._common import isfile_strict
 from ._common import memoize_when_activated
```

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_psposix.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_psposix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pssunos.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pssunos.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,16 +11,19 @@
 import subprocess
 import sys
 from collections import namedtuple
 from socket import AF_INET
 
 from . import _common
 from . import _psposix
-from . import _psutil_posix as cext_posix
-from . import _psutil_sunos as cext
+try:
+    from . import _psutil_posix as cext_posix
+    from . import _psutil_sunos as cext
+except:
+    pass
 from ._common import AF_INET6
 from ._common import AccessDenied
 from ._common import NoSuchProcess
 from ._common import ZombieProcess
 from ._common import debug
 from ._common import get_procfs_path
 from ._common import isfile_strict
```

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/_pswindows.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/_pswindows.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/__init__.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/runner.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/runner.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_aix.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_aix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_bsd.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_bsd.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_connections.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_connections.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_contracts.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_contracts.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_linux.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_linux.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_memleaks.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_memleaks.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_misc.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_osx.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_osx.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_posix.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_posix.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_process.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_sunos.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_sunos.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_system.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_system.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_testutils.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_testutils.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_unicode.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_unicode.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdaVbaAddins/psutil/tests/test_windows.py` & `rongdavbaaddins-0.0.0.8/rongdaVbaAddins/psutil/tests/test_windows.py`

 * *Files identical despite different names*

### Comparing `rongdavbaaddins-0.0.0.6/rongdavbaaddins.egg-info/SOURCES.txt` & `rongdavbaaddins-0.0.0.8/rongdavbaaddins.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,14 +10,20 @@
 rongdaVbaAddins/__init__.py
 rongdaVbaAddins/getNumber.pyd
 rongdaVbaAddins/getNumberpy.py
 rongdaVbaAddins/minusFunction.pyd
 rongdaVbaAddins/rongdaVbaAddins.pyd
 rongdaVbaAddins/vbaLogin.pyd
 rongdaVbaAddins/vbaloginpy.py
+rongdaVbaAddins/文件处理类模板.xlsx
+rongdaVbaAddins/Function/__init__.py
+rongdaVbaAddins/Function/minusFunction.pyd
+rongdaVbaAddins/Function/minusFunctionpy.py
+rongdaVbaAddins/Ui/__init__.py
+rongdaVbaAddins/Ui/rongdaVbaAddinsUi.py
 rongdaVbaAddins/psutil/__init__.py
 rongdaVbaAddins/psutil/_common.py
 rongdaVbaAddins/psutil/_compat.py
 rongdaVbaAddins/psutil/_psaix.py
 rongdaVbaAddins/psutil/_psbsd.py
 rongdaVbaAddins/psutil/_pslinux.py
 rongdaVbaAddins/psutil/_psosx.py
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `rongdavbaaddins-0.0.0.6/setup.py` & `rongdavbaaddins-0.0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
 MINOR = 0
 PATCH = 0
-VERSION = f"{MAJOR}.{MINOR}.{PATCH}.6"
+VERSION = f"{MAJOR}.{MINOR}.{PATCH}.8"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "rongdavbaaddins",
     version=VERSION,
@@ -26,11 +26,11 @@
     packages=find_packages(),
     # license = '',
     classifiers=[
         'Programming Language :: Python',
 
     ],
     # 包含的类型
-    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm', '*.xlam', '*.officeUI','.xlsx']},  # 这个很重要
+    package_data={'': ['*.csv', '*.txt', '.toml', "*.pyd", '*.exe', '*.db', '*.xlsm', '*.xlam', '*.officeUI','*.xlsx']},  # 这个很重要
     include_package_data=True  # 也选上
 
 )
```

