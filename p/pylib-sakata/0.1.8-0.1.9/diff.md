# Comparing `tmp/pylib-sakata-0.1.8.tar.gz` & `tmp/pylib-sakata-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylib-sakata-0.1.8.tar", last modified: Wed Jul 20 03:31:31 2022, max compression
+gzip compressed data, was "pylib-sakata-0.1.9.tar", last modified: Wed Jul 20 09:00:00 2022, max compression
```

## Comparing `pylib-sakata-0.1.8.tar` & `pylib-sakata-0.1.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2022-07-20 03:31:31.881965 pylib-sakata-0.1.8/
--rw-rw-rw-   0        0        0     1091 2022-04-29 12:07:38.000000 pylib-sakata-0.1.8/LICENSE
--rw-rw-rw-   0        0        0    62397 2022-07-20 03:31:31.881965 pylib-sakata-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0    62057 2022-07-20 03:30:50.000000 pylib-sakata-0.1.8/README.md
--rw-rw-rw-   0        0        0       42 2022-07-20 03:31:31.881965 pylib-sakata-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      576 2022-07-20 03:30:32.000000 pylib-sakata-0.1.8/setup.py
-drwxrwxrwx   0        0        0        0 2022-07-20 03:31:31.821966 pylib-sakata-0.1.8/src/
-drwxrwxrwx   0        0        0        0 2022-07-20 03:31:31.859964 pylib-sakata-0.1.8/src/pylib_sakata/
--rw-rw-rw-   0        0        0        0 2022-04-29 12:07:38.000000 pylib-sakata-0.1.8/src/pylib_sakata/__init__.py
--rw-rw-rw-   0        0        0    31529 2022-07-20 03:26:55.000000 pylib-sakata-0.1.8/src/pylib_sakata/ctrl.py
--rw-rw-rw-   0        0        0     8614 2022-05-22 12:50:33.000000 pylib-sakata-0.1.8/src/pylib_sakata/fft.py
--rw-rw-rw-   0        0        0      331 2022-04-29 12:07:38.000000 pylib-sakata-0.1.8/src/pylib_sakata/init.py
--rw-rw-rw-   0        0        0    11243 2022-05-28 17:38:19.000000 pylib-sakata-0.1.8/src/pylib_sakata/kinema.py
--rw-rw-rw-   0        0        0     3475 2022-05-02 05:12:25.000000 pylib-sakata-0.1.8/src/pylib_sakata/meas.py
--rw-rw-rw-   0        0        0     7485 2022-05-20 15:32:05.000000 pylib-sakata-0.1.8/src/pylib_sakata/plot.py
--rw-rw-rw-   0        0        0     2405 2022-04-29 12:07:38.000000 pylib-sakata-0.1.8/src/pylib_sakata/traj.py
-drwxrwxrwx   0        0        0        0 2022-07-20 03:31:31.879964 pylib-sakata-0.1.8/src/pylib_sakata.egg-info/
--rw-rw-rw-   0        0        0    62397 2022-07-20 03:31:31.000000 pylib-sakata-0.1.8/src/pylib_sakata.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2022-07-20 03:31:31.000000 pylib-sakata-0.1.8/src/pylib_sakata.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-20 03:31:31.000000 pylib-sakata-0.1.8/src/pylib_sakata.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2022-07-20 03:31:31.000000 pylib-sakata-0.1.8/src/pylib_sakata.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.221379 pylib-sakata-0.1.9/
+-rw-rw-rw-   0        0        0     1091 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0    62397 2022-07-20 09:00:00.220378 pylib-sakata-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0    62057 2022-07-20 08:59:27.000000 pylib-sakata-0.1.9/README.md
+-rw-rw-rw-   0        0        0       42 2022-07-20 09:00:00.221379 pylib-sakata-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      576 2022-07-20 08:59:48.000000 pylib-sakata-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.161379 pylib-sakata-0.1.9/src/
+drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.203379 pylib-sakata-0.1.9/src/pylib_sakata/
+-rw-rw-rw-   0        0        0        0 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/src/pylib_sakata/__init__.py
+-rw-rw-rw-   0        0        0    32607 2022-07-20 08:57:06.000000 pylib-sakata-0.1.9/src/pylib_sakata/ctrl.py
+-rw-rw-rw-   0        0        0     8614 2022-05-22 12:50:33.000000 pylib-sakata-0.1.9/src/pylib_sakata/fft.py
+-rw-rw-rw-   0        0        0      331 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/src/pylib_sakata/init.py
+-rw-rw-rw-   0        0        0    11243 2022-05-28 17:38:19.000000 pylib-sakata-0.1.9/src/pylib_sakata/kinema.py
+-rw-rw-rw-   0        0        0     3475 2022-05-02 05:12:25.000000 pylib-sakata-0.1.9/src/pylib_sakata/meas.py
+-rw-rw-rw-   0        0        0     7485 2022-05-20 15:32:05.000000 pylib-sakata-0.1.9/src/pylib_sakata/plot.py
+-rw-rw-rw-   0        0        0     2405 2022-04-29 12:07:38.000000 pylib-sakata-0.1.9/src/pylib_sakata/traj.py
+drwxrwxrwx   0        0        0        0 2022-07-20 09:00:00.219377 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/
+-rw-rw-rw-   0        0        0    62397 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2022-07-20 09:00:00.000000 pylib-sakata-0.1.9/src/pylib_sakata.egg-info/top_level.txt
```

### Comparing `pylib-sakata-0.1.8/LICENSE` & `pylib-sakata-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.8/PKG-INFO` & `pylib-sakata-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pylib-sakata
-Version: 0.1.8
+Version: 0.1.9
 Summary: Control system design and analysis package
 Home-page: https://github.com/Koichi-Sakata/pylib_sakata
 Author: Koichi Sakata
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-pylib-sakata User's Manual version-0.1.8
+pylib-sakata User's Manual version-0.1.9
 ===
 
 <!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
 
 <!-- code_chunk_output -->
 
-- [pylib-sakata User's Manual version-0.1.8](#pylib-sakata-users-manual-version-018)
+- [pylib-sakata User's Manual version-0.1.9](#pylib-sakata-users-manual-version-019)
 - [1. Introduction](#1-introduction)
 - [2. Environment Setup](#2-environment-setup)
   - [2.1. Installation of Python](#21-installation-of-python)
   - [2.2. Installation  of required Python libraries](#22-installation--of-required-python-libraries)
   - [2.3. Installation of pylib-sakata](#23-installation-of-pylib-sakata)
   - [2.4. Installation of IDE for Python](#24-installation-of-ide-for-python)
     - [2.4.1. Visual Studio Code (VSCode)](#241-visual-studio-code-vscode)
```

### Comparing `pylib-sakata-0.1.8/README.md` & `pylib-sakata-0.1.9/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-pylib-sakata User's Manual version-0.1.8
+pylib-sakata User's Manual version-0.1.9
 ===
 
 <!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
 
 <!-- code_chunk_output -->
 
-- [pylib-sakata User's Manual version-0.1.8](#pylib-sakata-users-manual-version-018)
+- [pylib-sakata User's Manual version-0.1.9](#pylib-sakata-users-manual-version-019)
 - [1. Introduction](#1-introduction)
 - [2. Environment Setup](#2-environment-setup)
   - [2.1. Installation of Python](#21-installation-of-python)
   - [2.2. Installation  of required Python libraries](#22-installation--of-required-python-libraries)
   - [2.3. Installation of pylib-sakata](#23-installation-of-pylib-sakata)
   - [2.4. Installation of IDE for Python](#24-installation-of-ide-for-python)
     - [2.4.1. Visual Studio Code (VSCode)](#241-visual-studio-code-vscode)
```

### Comparing `pylib-sakata-0.1.8/setup.py` & `pylib-sakata-0.1.9/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pylib-sakata",
-    version="0.1.8",
+    version="0.1.9",
     author="Koichi Sakata",
     author_email="",
     description="Control system design and analysis package",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Koichi-Sakata/pylib_sakata",
     package_dir={"": "src"},
```

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata/ctrl.py` & `pylib-sakata-0.1.9/src/pylib_sakata/ctrl.py`

 * *Files 2% similar despite different names*

```diff
@@ -702,28 +702,47 @@
 
 
 def makeprmset(path='.'):
     path_cpp = path + '/gval_ctrlprm.cpp'
     f = open(path_cpp, 'w')
     f.write('#include "TcPch.h"\n')
     f.write('#pragma hdrstop\n')
-    f.write('#include "head_common.h"\n\n')
+    f.write('#include "head_ctrlprm.h"\n\n')
 
     path_h = path + '/head_ctrlprm.h'
     f = open(path_h, 'w')
     f.write('#ifndef _HEAD_CTRLPRM_\n')
-    f.write('#define _HEAD_CTRLPRM_\n')
-    f.write('\n\n#endif\n')
+    f.write('#define _HEAD_CTRLPRM_\n\n')
+    f.write('typedef struct {\n')
+    f.write('	double	dA[2];\n')
+    f.write('	double	dB[2];\n')
+    f.write('	double	dInPre;\n')
+    f.write('	double	dOutPre;\n')
+    f.write('} TF1_INF;						// 1st order TF information\n\n')
+    f.write('typedef struct {\n')
+    f.write('	double	dA[3];\n')
+    f.write('	double	dB[3];\n')
+    f.write('	double	dInPre[2];\n')
+    f.write('	double	dOutPre[2];\n')
+    f.write('} TF2_INF;						// 2nd order TF information\n\n')
+    f.write('typedef struct {\n')
+    f.write('	double	dA[4];\n')
+    f.write('	double	dB[4];\n')
+    f.write('	double	dInPre[3];\n')
+    f.write('	double	dOutPre[3];\n')
+    f.write('} TF3_INF;						// 3rd order TF information\n\n')
+    f.write('#endif\n')
 
 
 def defprmset(tfz, prmSetName, path='.', mode='a'):
     if type(tfz).__module__ != 'numpy':
         num = tfz.num[0][0]
         den = tfz.den[0][0]
-
+        if len(den) - len(num) > 0:
+            num = np.concatenate([np.zeros(len(den) - len(num)), num])
         path_cpp = path + '/gval_ctrlprm.cpp'
         f = open(path_cpp, mode)
         f.write('\n')
         if len(den) == 2:
             f.write('TF1_INF	')
             f.write(prmSetName)
             f.write(' = {\n')
@@ -816,14 +835,16 @@
             elif len(den) == 4:
                 f.write('TF3_INF	')
                 f.write(prmSetName)
                 f.write(' = {\n')
             for i in range(len(tfz)):
                 num = tfz[i].num[0][0]
                 den = tfz[i].den[0][0]
+                if len(den) - len(num) > 0:
+                    num = np.concatenate([np.zeros(len(den) - len(num)), num])
                 f.write('	{\n')
                 f.write('		{ ')
                 for k in range(len(den)):
                     f.write(str(den[k]))
                     if k != len(den) - 1:
                         f.write(', ')
                 f.write(' },\n')
@@ -883,14 +904,16 @@
                 f.write(prmSetName)
                 f.write(' = {\n')
             for i in range(len(tfz)):
                 f.write('	{\n')
                 for j in range(len(tfz[i])):
                     num = tfz[i][j].num[0][0]
                     den = tfz[i][j].den[0][0]
+                    if len(den) - len(num) > 0:
+                        num = np.concatenate([np.zeros(len(den) - len(num)), num])
                     f.write('		{\n')
                     f.write('			{ ')
                     for k in range(len(den)):
                         f.write(str(den[k]))
                         if k != len(den) - 1:
                             f.write(', ')
                     f.write(' },\n')
```

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata/fft.py` & `pylib-sakata-0.1.9/src/pylib_sakata/fft.py`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata/kinema.py` & `pylib-sakata-0.1.9/src/pylib_sakata/kinema.py`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata/meas.py` & `pylib-sakata-0.1.9/src/pylib_sakata/meas.py`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata/plot.py` & `pylib-sakata-0.1.9/src/pylib_sakata/plot.py`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata/traj.py` & `pylib-sakata-0.1.9/src/pylib_sakata/traj.py`

 * *Files identical despite different names*

### Comparing `pylib-sakata-0.1.8/src/pylib_sakata.egg-info/PKG-INFO` & `pylib-sakata-0.1.9/src/pylib_sakata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: pylib-sakata
-Version: 0.1.8
+Version: 0.1.9
 Summary: Control system design and analysis package
 Home-page: https://github.com/Koichi-Sakata/pylib_sakata
 Author: Koichi Sakata
 Author-email: 
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-pylib-sakata User's Manual version-0.1.8
+pylib-sakata User's Manual version-0.1.9
 ===
 
 <!-- @import "[TOC]" {cmd="toc" depthFrom=1 depthTo=6 orderedList=false} -->
 
 <!-- code_chunk_output -->
 
-- [pylib-sakata User's Manual version-0.1.8](#pylib-sakata-users-manual-version-018)
+- [pylib-sakata User's Manual version-0.1.9](#pylib-sakata-users-manual-version-019)
 - [1. Introduction](#1-introduction)
 - [2. Environment Setup](#2-environment-setup)
   - [2.1. Installation of Python](#21-installation-of-python)
   - [2.2. Installation  of required Python libraries](#22-installation--of-required-python-libraries)
   - [2.3. Installation of pylib-sakata](#23-installation-of-pylib-sakata)
   - [2.4. Installation of IDE for Python](#24-installation-of-ide-for-python)
     - [2.4.1. Visual Studio Code (VSCode)](#241-visual-studio-code-vscode)
```

