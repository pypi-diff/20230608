# Comparing `tmp/xgo-pythonlib-0.1.1.tar.gz` & `tmp/xgo-pythonlib-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xgo-pythonlib-0.1.1.tar", last modified: Wed Jun  7 11:52:29 2023, max compression
+gzip compressed data, was "xgo-pythonlib-0.1.2.tar", last modified: Wed Jun  7 11:54:54 2023, max compression
```

## Comparing `xgo-pythonlib-0.1.1.tar` & `xgo-pythonlib-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 11:52:29.782727 xgo-pythonlib-0.1.1/
--rw-rw-rw-   0        0        0     1563 2023-06-07 11:52:29.781726 xgo-pythonlib-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      936 2023-06-07 11:42:17.000000 xgo-pythonlib-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-07 11:52:29.782727 xgo-pythonlib-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     3684 2023-06-07 11:52:22.000000 xgo-pythonlib-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:52:29.771690 xgo-pythonlib-0.1.1/xgo_pythonlib.egg-info/
--rw-rw-rw-   0        0        0     1563 2023-06-07 11:52:29.000000 xgo-pythonlib-0.1.1/xgo_pythonlib.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      289 2023-06-07 11:52:29.000000 xgo-pythonlib-0.1.1/xgo_pythonlib.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 11:52:29.000000 xgo-pythonlib-0.1.1/xgo_pythonlib.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-06-07 11:52:29.000000 xgo-pythonlib-0.1.1/xgo_pythonlib.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-07 11:52:29.774690 xgo-pythonlib-0.1.1/xgoedu/
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.1/xgoedu/__init__.py
--rw-rw-rw-   0        0        0    33489 2023-06-07 11:44:09.000000 xgo-pythonlib-0.1.1/xgoedu/xgoedu.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:52:29.774690 xgo-pythonlib-0.1.1/xgolib/
--rw-rw-rw-   0        0        0    24818 2023-06-07 11:52:08.000000 xgo-pythonlib-0.1.1/xgolib/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-07 11:52:29.780726 xgo-pythonlib-0.1.1/xgoscreen/
--rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.1/xgoscreen/LCD_2inch.py
--rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.1/xgoscreen/__init__.py
--rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.1/xgoscreen/lcdconfig.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:54.625440 xgo-pythonlib-0.1.2/
+-rw-rw-rw-   0        0        0     1563 2023-06-07 11:54:54.624438 xgo-pythonlib-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      936 2023-06-07 11:42:17.000000 xgo-pythonlib-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-07 11:54:54.625440 xgo-pythonlib-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     3684 2023-06-07 11:54:43.000000 xgo-pythonlib-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:54.615131 xgo-pythonlib-0.1.2/xgo_pythonlib.egg-info/
+-rw-rw-rw-   0        0        0     1563 2023-06-07 11:54:54.000000 xgo-pythonlib-0.1.2/xgo_pythonlib.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      272 2023-06-07 11:54:54.000000 xgo-pythonlib-0.1.2/xgo_pythonlib.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-07 11:54:54.000000 xgo-pythonlib-0.1.2/xgo_pythonlib.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-06-07 11:54:54.000000 xgo-pythonlib-0.1.2/xgo_pythonlib.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:54.617421 xgo-pythonlib-0.1.2/xgoedu/
+-rw-rw-rw-   0        0        0    33489 2023-06-07 11:54:24.000000 xgo-pythonlib-0.1.2/xgoedu/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:54.619429 xgo-pythonlib-0.1.2/xgolib/
+-rw-rw-rw-   0        0        0    24818 2023-06-07 11:52:08.000000 xgo-pythonlib-0.1.2/xgolib/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-07 11:54:54.623438 xgo-pythonlib-0.1.2/xgoscreen/
+-rw-rw-rw-   0        0        0     5339 2023-06-07 11:44:32.000000 xgo-pythonlib-0.1.2/xgoscreen/LCD_2inch.py
+-rw-rw-rw-   0        0        0        0 2023-06-06 11:56:39.000000 xgo-pythonlib-0.1.2/xgoscreen/__init__.py
+-rw-rw-rw-   0        0        0     2214 2023-06-06 01:30:25.000000 xgo-pythonlib-0.1.2/xgoscreen/lcdconfig.py
```

### Comparing `xgo-pythonlib-0.1.1/PKG-INFO` & `xgo-pythonlib-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.1.1/README.md` & `xgo-pythonlib-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.1/setup.py` & `xgo-pythonlib-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 NAME = 'xgo-pythonlib'
 DESCRIPTION = 'PythonLib for XGO2-DOG'
 URL = 'https://github.com/Xgorobot/XGO-PythonLib'
 EMAIL = 'hello@xgorobot.com'
 AUTHOR = 'luwudynamics'
 REQUIRES_PYTHON = '>=3.6.0'
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
 ]
 
 # What packages are optional?
```

### Comparing `xgo-pythonlib-0.1.1/xgo_pythonlib.egg-info/PKG-INFO` & `xgo-pythonlib-0.1.2/xgo_pythonlib.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xgo-pythonlib
-Version: 0.1.1
+Version: 0.1.2
 Summary: PythonLib for XGO2-DOG
 Home-page: https://github.com/Xgorobot/XGO-PythonLib
 Author: luwudynamics
 Author-email: hello@xgorobot.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `xgo-pythonlib-0.1.1/xgoedu/xgoedu.py` & `xgo-pythonlib-0.1.2/xgoedu/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.1/xgolib/__init__.py` & `xgo-pythonlib-0.1.2/xgolib/__init__.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.1/xgoscreen/LCD_2inch.py` & `xgo-pythonlib-0.1.2/xgoscreen/LCD_2inch.py`

 * *Files identical despite different names*

### Comparing `xgo-pythonlib-0.1.1/xgoscreen/lcdconfig.py` & `xgo-pythonlib-0.1.2/xgoscreen/lcdconfig.py`

 * *Files identical despite different names*

