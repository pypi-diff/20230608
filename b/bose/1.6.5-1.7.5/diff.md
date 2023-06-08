# Comparing `tmp/bose-1.6.5.tar.gz` & `tmp/bose-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bose-1.6.5.tar", last modified: Thu May 25 17:03:10 2023, max compression
+gzip compressed data, was "bose-1.7.5.tar", last modified: Thu Jun  8 13:08:27 2023, max compression
```

## Comparing `bose-1.6.5.tar` & `bose-1.7.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 17:03:10.789121 bose-1.6.5/
--rw-rw-rw-   0        0        0    14240 2023-05-25 17:03:10.791120 bose-1.6.5/PKG-INFO
--rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-1.6.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-25 17:03:10.788127 bose-1.6.5/bose/
--rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.6.5/bose/__init__.py
--rw-rw-rw-   0        0        0      652 2023-05-25 17:01:27.624054 bose-1.6.5/bose/analytics.py
--rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.6.5/bose/base_data.py
--rw-rw-rw-   0        0        0     5070 2023-05-25 16:54:25.377864 bose-1.6.5/bose/base_task.py
--rw-rw-rw-   0        0        0     9039 2023-05-22 11:25:15.734584 bose-1.6.5/bose/boss_driver.py
--rw-rw-rw-   0        0        0     9051 2023-05-22 11:25:15.732590 bose-1.6.5/bose/boss_undetected_driver.py
--rw-rw-rw-   0        0        0     7295 2023-05-13 11:28:17.686088 bose-1.6.5/bose/create_driver.py
--rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.6.5/bose/download_driver.py
--rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.6.5/bose/local_storage.py
--rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.6.5/bose/local_storage_driver.py
--rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.6.5/bose/opponent.py
--rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.6.5/bose/output.py
--rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.6.5/bose/task_info.py
--rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.6.5/bose/temp_mail.py
--rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.6.5/bose/user_agent.py
--rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.6.5/bose/utils.py
--rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.6.5/bose/wait.py
--rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.6.5/bose/window_size.py
--rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.6.5/setup.cfg
--rw-rw-rw-   0        0        0     2329 2023-05-25 17:02:57.205292 bose-1.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-08 13:08:27.870110 bose-1.7.5/
+-rw-rw-rw-   0        0        0    14240 2023-06-08 13:08:27.871113 bose-1.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10461 2023-05-24 16:36:27.405231 bose-1.7.5/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-08 13:08:27.869114 bose-1.7.5/bose/
+-rw-rw-rw-   0        0        0      340 2023-05-13 11:28:45.126433 bose-1.7.5/bose/__init__.py
+-rw-rw-rw-   0        0        0      652 2023-05-25 17:01:27.624054 bose-1.7.5/bose/analytics.py
+-rw-rw-rw-   0        0        0     3657 2023-05-10 09:24:37.900794 bose-1.7.5/bose/base_data.py
+-rw-rw-rw-   0        0        0     5070 2023-05-25 16:54:25.377864 bose-1.7.5/bose/base_task.py
+-rw-rw-rw-   0        0        0     9039 2023-05-22 11:25:15.734584 bose-1.7.5/bose/boss_driver.py
+-rw-rw-rw-   0        0        0     9051 2023-05-22 11:25:15.732590 bose-1.7.5/bose/boss_undetected_driver.py
+-rw-rw-rw-   0        0        0     7295 2023-06-08 13:07:56.570819 bose-1.7.5/bose/create_driver.py
+-rw-rw-rw-   0        0        0     1391 2023-05-10 10:36:24.892682 bose-1.7.5/bose/download_driver.py
+-rw-rw-rw-   0        0        0     3185 2023-05-18 07:50:25.651854 bose-1.7.5/bose/local_storage.py
+-rw-rw-rw-   0        0        0     1728 2023-05-09 15:44:16.700182 bose-1.7.5/bose/local_storage_driver.py
+-rw-rw-rw-   0        0        0       80 2023-05-09 06:14:41.273740 bose-1.7.5/bose/opponent.py
+-rw-rw-rw-   0        0        0     3187 2023-05-15 09:11:34.318135 bose-1.7.5/bose/output.py
+-rw-rw-rw-   0        0        0     1650 2023-05-13 11:28:17.687091 bose-1.7.5/bose/task_info.py
+-rw-rw-rw-   0        0        0     3977 2023-05-13 13:31:08.141431 bose-1.7.5/bose/temp_mail.py
+-rw-rw-rw-   0        0        0     7361 2023-05-10 09:24:37.900794 bose-1.7.5/bose/user_agent.py
+-rw-rw-rw-   0        0        0     6050 2023-05-10 10:34:20.625623 bose-1.7.5/bose/utils.py
+-rw-rw-rw-   0        0        0       60 2023-05-09 06:15:17.436327 bose-1.7.5/bose/wait.py
+-rw-rw-rw-   0        0        0     1203 2023-05-09 07:09:28.075948 bose-1.7.5/bose/window_size.py
+-rw-rw-rw-   0        0        0       40 2022-10-28 11:26:12.145036 bose-1.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     2329 2023-06-08 13:07:20.397716 bose-1.7.5/setup.py
```

### Comparing `bose-1.6.5/PKG-INFO` & `bose-1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: bose
-Version: 1.6.5
+Version: 1.7.5
 Summary: The Ultimate Web Scraping Framework
 Home-page: UNKNOWN
 Author: Chetan Jain
 Author-email: chetan@omkar.cloud
 License: MIT
 Description: 🚀 Introducing ✨ Bose Framework - The Swiss Army Knife for Bot Developers 🤖
         =============================================================================
```

### Comparing `bose-1.6.5/README.rst` & `bose-1.7.5/README.rst`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/analytics.py` & `bose-1.7.5/bose/analytics.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/base_data.py` & `bose-1.7.5/bose/base_data.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/base_task.py` & `bose-1.7.5/bose/base_task.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/boss_driver.py` & `bose-1.7.5/bose/boss_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/boss_undetected_driver.py` & `bose-1.7.5/bose/boss_undetected_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/create_driver.py` & `bose-1.7.5/bose/create_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/download_driver.py` & `bose-1.7.5/bose/download_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/local_storage.py` & `bose-1.7.5/bose/local_storage.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/local_storage_driver.py` & `bose-1.7.5/bose/local_storage_driver.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/output.py` & `bose-1.7.5/bose/output.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/task_info.py` & `bose-1.7.5/bose/task_info.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/temp_mail.py` & `bose-1.7.5/bose/temp_mail.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/user_agent.py` & `bose-1.7.5/bose/user_agent.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/utils.py` & `bose-1.7.5/bose/utils.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/bose/window_size.py` & `bose-1.7.5/bose/window_size.py`

 * *Files identical despite different names*

### Comparing `bose-1.6.5/setup.py` & `bose-1.7.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from distutils.core import setup
 
 
 install_requires = [
     "requests",
     "chromedriver-autoinstaller==0.4.0",
-    "selenium>=4.0.0",
+    "selenium==4.5.0",
     "undetected_chromedriver>=3.4.6",
     "openpyxl>=3.0.3",
     "beautifulsoup4>=4.11.2",
 
 ]
 extras_require = {}
 cpython_dependencies = [
@@ -21,15 +21,15 @@
     except:
       return None
     
 
 setup(
     name='bose',
     packages=['bose'],
-    version='1.6.5',
+    version='1.7.5',
     license='MIT',
     project_urls={
         "Documentation": "https://omkar.cloud/bose/docs/",
         "Source": "https://github.com/omkarcloud/boss",
         "Tracker": "https://github.com/omkarcloud/boss/issues",
     },
```

