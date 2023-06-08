# Comparing `tmp/baysalt_christmas-0.1.7.5.tar.gz` & `tmp/baysalt_christmas-0.1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baysalt_christmas-0.1.7.5.tar", last modified: Tue Jun  6 09:11:06 2023, max compression
+gzip compressed data, was "baysalt_christmas-0.1.7.6.tar", last modified: Thu Jun  8 02:22:41 2023, max compression
```

## Comparing `baysalt_christmas-0.1.7.5.tar` & `baysalt_christmas-0.1.7.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.855027 baysalt_christmas-0.1.7.5/
--rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.5/.DS_Store
--rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.5/MANIFEST.in
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-06 09:11:06.854866 baysalt_christmas-0.1.7.5/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.5/README.md
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.848504 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/
--rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/PKG-INFO
--rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/SOURCES.txt
--rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/dependency_links.txt
--rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/requires.txt
--rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-06 09:11:06.000000 baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/top_level.txt
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.850903 baysalt_christmas-0.1.7.5/christmas/
--rw-r--r--   0 christmas   (501) staff       (20)    20844 2023-05-25 08:49:22.000000 baysalt_christmas-0.1.7.5/christmas/Blogging.py
--rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.5/christmas/S_DateTime.py
--rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.5/christmas/__init__.py
--rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.5/christmas/commonCode.py
--rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.5/christmas/cprintf.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.853590 baysalt_christmas-0.1.7.5/christmas/mncPy/
--rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/.gitignore
--rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/LICENSE
--rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__init__.py
-drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-06 09:11:06.854434 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/
--rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/common.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc
--rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/common.py
--rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.5/christmas/mncPy/compress.py
--rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.5/christmas/processBar.py
--rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.5/christmas/read_conf.py
--rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.5/christmas/server_info.py
--rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.5/run_twine.py
--rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-06 09:11:06.855071 baysalt_christmas-0.1.7.5/setup.cfg
--rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-06 09:11:05.000000 baysalt_christmas-0.1.7.5/setup.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.559088 baysalt_christmas-0.1.7.6/
+-rw-r--r--   0 christmas   (501) staff       (20)    10244 2023-05-18 11:12:41.000000 baysalt_christmas-0.1.7.6/.DS_Store
+-rw-r--r--   0 christmas   (501) staff       (20)      117 2023-03-25 19:22:27.000000 baysalt_christmas-0.1.7.6/MANIFEST.in
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-08 02:22:41.558935 baysalt_christmas-0.1.7.6/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)     3732 2023-03-29 03:30:38.000000 baysalt_christmas-0.1.7.6/README.md
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.548994 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/
+-rw-r--r--   0 christmas   (501) staff       (20)     4095 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/PKG-INFO
+-rw-r--r--   0 christmas   (501) staff       (20)      729 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/SOURCES.txt
+-rw-r--r--   0 christmas   (501) staff       (20)        1 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/dependency_links.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       30 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/requires.txt
+-rw-r--r--   0 christmas   (501) staff       (20)       10 2023-06-08 02:22:41.000000 baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/top_level.txt
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.552525 baysalt_christmas-0.1.7.6/christmas/
+-rw-r--r--   0 christmas   (501) staff       (20)    21061 2023-06-08 02:22:25.000000 baysalt_christmas-0.1.7.6/christmas/Blogging.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1895 2023-03-25 02:55:02.000000 baysalt_christmas-0.1.7.6/christmas/S_DateTime.py
+-rw-r--r--   0 christmas   (501) staff       (20)      445 2023-04-23 12:43:18.000000 baysalt_christmas-0.1.7.6/christmas/__init__.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4676 2023-05-17 09:02:10.000000 baysalt_christmas-0.1.7.6/christmas/commonCode.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1638 2023-04-12 07:23:55.000000 baysalt_christmas-0.1.7.6/christmas/cprintf.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.557653 baysalt_christmas-0.1.7.6/christmas/mncPy/
+-rw-r--r--   0 christmas   (501) staff       (20)     1203 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/.gitignore
+-rw-r--r--   0 christmas   (501) staff       (20)    35149 2023-03-03 04:53:20.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/LICENSE
+-rw-r--r--   0 christmas   (501) staff       (20)      239 2023-03-03 08:53:41.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__init__.py
+drwxr-xr-x   0 christmas   (501) staff       (20)        0 2023-06-08 02:22:41.558569 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/
+-rw-r--r--   0 christmas   (501) staff       (20)      228 2023-03-26 18:28:05.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     8964 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)     3411 2023-04-08 09:55:17.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc
+-rw-r--r--   0 christmas   (501) staff       (20)    12920 2023-03-09 13:49:40.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/common.py
+-rw-r--r--   0 christmas   (501) staff       (20)     4347 2023-03-09 14:00:22.000000 baysalt_christmas-0.1.7.6/christmas/mncPy/compress.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3554 2023-03-29 02:58:20.000000 baysalt_christmas-0.1.7.6/christmas/processBar.py
+-rw-r--r--   0 christmas   (501) staff       (20)     3473 2023-04-13 06:21:12.000000 baysalt_christmas-0.1.7.6/christmas/read_conf.py
+-rw-r--r--   0 christmas   (501) staff       (20)     1506 2022-12-07 09:44:40.000000 baysalt_christmas-0.1.7.6/christmas/server_info.py
+-rw-r--r--   0 christmas   (501) staff       (20)      456 2023-03-25 18:44:30.000000 baysalt_christmas-0.1.7.6/run_twine.py
+-rw-r--r--   0 christmas   (501) staff       (20)       38 2023-06-08 02:22:41.559146 baysalt_christmas-0.1.7.6/setup.cfg
+-rw-r--r--   0 christmas   (501) staff       (20)      796 2023-06-08 02:22:36.000000 baysalt_christmas-0.1.7.6/setup.py
```

### Comparing `baysalt_christmas-0.1.7.5/.DS_Store` & `baysalt_christmas-0.1.7.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/PKG-INFO` & `baysalt_christmas-0.1.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt_christmas
-Version: 0.1.7.5
+Version: 0.1.7.6
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.5/README.md` & `baysalt_christmas-0.1.7.6/README.md`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/PKG-INFO` & `baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baysalt-christmas
-Version: 0.1.7.5
+Version: 0.1.7.6
 Summary: Some simple tools for Christmas
 Author: Christmas
 Author-email: 273519355@qq.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `baysalt_christmas-0.1.7.5/baysalt_christmas.egg-info/SOURCES.txt` & `baysalt_christmas-0.1.7.6/baysalt_christmas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/Blogging.py` & `baysalt_christmas-0.1.7.6/christmas/Blogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,14 +51,23 @@
                  _switch_print_log=True,  # 是否打印日志
                  _switch_write_debug_log=False,  # 是否写入单独的debug日志
                  _switch_write_info_log=False,  # 是否写入单独的info日志
                  _switch_write_warning_log=False,  # 是否写入单独的warning日志
                  _switch_write_error_log=False,  # 是否写入单独的error日志
                  _switch_write_critical_log=False):  # 是否写入单独的critical日志
         
+        self.CRITICAL = 50
+        self.FATAL = self.CRITICAL
+        self.ERROR = 40
+        self.WARNING = 30
+        self.WARN = self.WARNING
+        self.INFO = 20
+        self.DEBUG = 10
+        self.NOTSET = 0
+
         self.loger_name = _loger_name  # 日志记录器名称
         self.logfile_name = _log_filename  # 日志文件名
         self.switch_write_all_log = _switch_write_all_log  # 是否写入全部日志
         self.switch_write_error_plus_log = _switch_write_error_plus_log  # 是否写入错误日志
         self.switch_print_log = _switch_print_log  # 是否打印日志
         self.switch_write_debug_log = _switch_write_debug_log  # 是否写入单独的debug日志
         self.switch_write_info_log = _switch_write_info_log  # 是否写入单独的info日志
```

### Comparing `baysalt_christmas-0.1.7.5/christmas/S_DateTime.py` & `baysalt_christmas-0.1.7.6/christmas/S_DateTime.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/commonCode.py` & `baysalt_christmas-0.1.7.6/christmas/commonCode.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/cprintf.py` & `baysalt_christmas-0.1.7.6/christmas/cprintf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/mncPy/.gitignore` & `baysalt_christmas-0.1.7.6/christmas/mncPy/.gitignore`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/mncPy/LICENSE` & `baysalt_christmas-0.1.7.6/christmas/mncPy/LICENSE`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/common.cpython-39.pyc` & `baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/common.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/mncPy/__pycache__/compress.cpython-39.pyc` & `baysalt_christmas-0.1.7.6/christmas/mncPy/__pycache__/compress.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/mncPy/common.py` & `baysalt_christmas-0.1.7.6/christmas/mncPy/common.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/mncPy/compress.py` & `baysalt_christmas-0.1.7.6/christmas/mncPy/compress.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/processBar.py` & `baysalt_christmas-0.1.7.6/christmas/processBar.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/read_conf.py` & `baysalt_christmas-0.1.7.6/christmas/read_conf.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/christmas/server_info.py` & `baysalt_christmas-0.1.7.6/christmas/server_info.py`

 * *Files identical despite different names*

### Comparing `baysalt_christmas-0.1.7.5/setup.py` & `baysalt_christmas-0.1.7.6/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
     name="baysalt_christmas",
-    version="0.1.7.5",
+    version="0.1.7.6",
     author="Christmas",
     author_email="273519355@qq.com",
     description="Some simple tools for Christmas",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     include_package_data=True,
```

