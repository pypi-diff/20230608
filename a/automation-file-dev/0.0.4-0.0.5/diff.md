# Comparing `tmp/automation_file_dev-0.0.4.tar.gz` & `tmp/automation_file_dev-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file_dev-0.0.4.tar", last modified: Mon May 29 02:35:41 2023, max compression
+gzip compressed data, was "automation_file_dev-0.0.5.tar", last modified: Thu Jun  8 08:17:56 2023, max compression
```

## Comparing `automation_file_dev-0.0.4.tar` & `automation_file_dev-0.0.5.tar`

### file list

```diff
@@ -1,34 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:41.004395 automation_file_dev-0.0.4/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.4/LICENSE
--rw-rw-rw-   0        0        0     1376 2023-05-29 02:35:41.003391 automation_file_dev-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-05-29 01:54:01.000000 automation_file_dev-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.953323 automation_file_dev-0.0.4/automation_file_dev.egg-info/
--rw-rw-rw-   0        0        0     1376 2023-05-29 02:35:40.000000 automation_file_dev-0.0.4/automation_file_dev.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      763 2023-05-29 02:35:40.000000 automation_file_dev-0.0.4/automation_file_dev.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 02:35:40.000000 automation_file_dev-0.0.4/automation_file_dev.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-29 02:35:40.000000 automation_file_dev-0.0.4/automation_file_dev.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.960149 automation_file_dev-0.0.4/file_automation/
--rw-rw-rw-   0        0        0      732 2023-05-29 02:35:20.000000 automation_file_dev-0.0.4/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.962449 automation_file_dev-0.0.4/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.4/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.968996 automation_file_dev-0.0.4/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.4/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-05-19 07:13:21.000000 automation_file_dev-0.0.4/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.975003 automation_file_dev-0.0.4/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.4/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-05-19 06:44:49.000000 automation_file_dev-0.0.4/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.982170 automation_file_dev-0.0.4/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.4/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-05-19 09:53:23.000000 automation_file_dev-0.0.4/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.985178 automation_file_dev-0.0.4/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.4/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.989261 automation_file_dev-0.0.4/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.4/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:40.991270 automation_file_dev-0.0.4/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.4/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:35:41.000299 automation_file_dev-0.0.4/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.4/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:25.000000 automation_file_dev-0.0.4/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file_dev-0.0.4/file_automation/utils/exception/exceptions.py
--rw-rw-rw-   0        0        0      877 2023-05-29 02:35:20.000000 automation_file_dev-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 02:35:41.004395 automation_file_dev-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.861891 automation_file_dev-0.0.5/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file_dev-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0     1306 2023-06-08 08:17:56.860885 automation_file_dev-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file_dev-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.704589 automation_file_dev-0.0.5/automation_file_dev.egg-info/
+-rw-rw-rw-   0        0        0     1306 2023-06-08 08:17:56.000000 automation_file_dev-0.0.5/automation_file_dev.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1638 2023-06-08 08:17:56.000000 automation_file_dev-0.0.5/automation_file_dev.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 08:17:56.000000 automation_file_dev-0.0.5/automation_file_dev.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-08 08:17:56.000000 automation_file_dev-0.0.5/automation_file_dev.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 08:17:56.000000 automation_file_dev-0.0.5/automation_file_dev.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.714080 automation_file_dev-0.0.5/file_automation/
+-rw-rw-rw-   0        0        0      835 2023-06-05 01:25:45.000000 automation_file_dev-0.0.5/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.718089 automation_file_dev-0.0.5/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file_dev-0.0.5/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.724717 automation_file_dev-0.0.5/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file_dev-0.0.5/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file_dev-0.0.5/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.738231 automation_file_dev-0.0.5/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file_dev-0.0.5/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file_dev-0.0.5/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.750331 automation_file_dev-0.0.5/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file_dev-0.0.5/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file_dev-0.0.5/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.755495 automation_file_dev-0.0.5/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file_dev-0.0.5/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.764713 automation_file_dev-0.0.5/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.773024 automation_file_dev-0.0.5/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.785349 automation_file_dev-0.0.5/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.794746 automation_file_dev-0.0.5/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2200 2023-06-08 08:10:58.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.806035 automation_file_dev-0.0.5/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.820141 automation_file_dev-0.0.5/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.830805 automation_file_dev-0.0.5/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file_dev-0.0.5/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.834463 automation_file_dev-0.0.5/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file_dev-0.0.5/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.846614 automation_file_dev-0.0.5/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file_dev-0.0.5/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-06-05 01:25:46.000000 automation_file_dev-0.0.5/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file_dev-0.0.5/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:17:56.857116 automation_file_dev-0.0.5/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file_dev-0.0.5/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file_dev-0.0.5/file_automation/utils/logging/loggin_instance.py
+-rw-rw-rw-   0        0        0     1008 2023-06-08 08:17:20.000000 automation_file_dev-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 08:17:56.863412 automation_file_dev-0.0.5/setup.cfg
```

### Comparing `automation_file_dev-0.0.4/LICENSE` & `automation_file_dev-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file_dev-0.0.4/PKG-INFO` & `automation_file_dev-0.0.5/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: automation_file_dev
-Version: 0.0.4
+Version: 0.0.5
 Author-email: JE-Chen <zenmailman@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/JE-Chen/Integration-testing-environment
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
@@ -19,40 +19,29 @@
 
 ### Documentation
 
 * TODO
 
 ---
 > Project Kanban \
-> https://github.com/orgs/Intergration-Automation-Testing/projects/2 \
-> FileAutomation is used to manager files and dirs.
+> https://github.com/orgs/Integration-Automation/projects/2/views/1
+> * FileAutomation is used to manager files and dirs.
+> * Easily file automation.
+> * Automatically backup.
+> * Automatically download from Google Drive.
+> * Automatically upload to Google Drive.
+> * Automatically zip and unzip file.
+> * Automatically manager specify file.
+> * OS Independent.
+> * Remote automation support.
+> * Project & Template support.
+> * Detailed log file.
+> * Scheduler.
 
 
----
-### Features
-* Process multi file.
-  * copy file.
-  * copy specify extension file.
-  * copy all file to dir.
-  * rename file.
-  * remove file.
-* Process multi dir.
-  * copy dir.
-  * remove dir.
-  * rename dir.
-  * create dir.
-* Process zip files.
-  * zip a dir.
-  * zip a file.
-  * read zip file.
-  * unzip file on zip.
-  * un zip all file on zip.
-  * show zip info.
-  * show file on zip info.
-
 ## install
 > pip install automation_file
 
 ## Requires
 > python 3.8 or later
 
 ### Architecture Diagram
```

### Comparing `automation_file_dev-0.0.4/file_automation/__init__.py` & `automation_file_dev-0.0.5/file_automation/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from file_automation.local.file.file_process import copy_file, remove_file, rename_file, copy_specify_extension_file, \
     copy_all_file_to_dir
 from file_automation.local.dir.dir_process import copy_dir, rename_dir, create_dir, remove_dir_tree
 from file_automation.local.zip.zip_process import zip_dir, zip_file, zip_info, zip_file_info, set_zip_password, \
     read_zip_file, unzip_file, unzip_all
 
+from file_automation.remote.google_drive.driver_instance import driver_instance
+
 __all__ = [
     "copy_file", "rename_file", "remove_file", "copy_all_file_to_dir", "copy_specify_extension_file",
     "copy_dir", "create_dir", "copy_specify_extension_file", "remove_dir_tree",
     "zip_dir", "zip_file", "zip_info", "zip_file_info", "set_zip_password", "unzip_file", "read_zip_file",
-    "unzip_all"
+    "unzip_all", "driver_instance",
 ]
```

### Comparing `automation_file_dev-0.0.4/file_automation/local/zip/zip_process.py` & `automation_file_dev-0.0.5/file_automation/local/zip/zip_process.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,69 +1,102 @@
-import sys
 import zipfile
 from pathlib import Path
 from shutil import make_archive
 from typing import List
 
 from file_automation.utils.exception.exceptions import ZIPGetWrongFileException
+from file_automation.utils.logging.loggin_instance import file_automation_logger
 
 
 def zip_dir(dir_we_want_to_zip: str, zip_name: str):
     make_archive(root_dir=dir_we_want_to_zip, base_name=zip_name, format="zip")
+    file_automation_logger.info(f"Dir to zip: {dir_we_want_to_zip}, zip file name: {zip_name}")
 
 
 def zip_file(zip_file_path: str, file: [str, List[str]]):
     current_zip = zipfile.ZipFile(zip_file_path, mode="w")
     if isinstance(file, str):
         file_name = Path(file)
         current_zip.write(file, file_name.name)
+        file_automation_logger.info(
+            f"Write file: {file_name} to zip: {current_zip}"
+        )
     else:
         if isinstance(file, list):
             for writeable in file:
                 file_name = Path(writeable)
                 current_zip.write(writeable, file_name.name)
+                file_automation_logger.info(
+                    f"Write file: {writeable} to zip: {current_zip}"
+                )
         else:
-            print(repr(ZIPGetWrongFileException), file=sys.stderr)
+            file_automation_logger.error(
+                repr(ZIPGetWrongFileException))
     current_zip.close()
 
 
 def read_zip_file(zip_file_path: str, file_name: str, password: [str, None] = None):
     current_zip = zipfile.ZipFile(zip_file_path, mode="r")
-    data = None
     with current_zip.open(name=file_name, mode="r", pwd=password, force_zip64=True) as read_file:
         data = read_file.read()
     current_zip.close()
+    file_automation_logger.info(
+        f"Read zip file: {zip_file_path}"
+    )
     return data
 
 
 def unzip_file(zip_file_path: str, extract_member, extract_path: [str, None] = None, password: [str, None] = None):
     current_zip = zipfile.ZipFile(zip_file_path, mode="r")
     current_zip.extract(member=extract_member, path=extract_path, pwd=password)
+    file_automation_logger.info(
+        f"Unzip file: {zip_file_path}, "
+        f"extract member: {extract_member}, "
+        f"extract path: {extract_path}, "
+        f"password: {password}"
+    )
     current_zip.close()
 
 
 def unzip_all(
         zip_file_path: str, extract_member: [str, None] = None,
         extract_path: [str, None] = None, password: [str, None] = None):
     current_zip = zipfile.ZipFile(zip_file_path, mode="r")
     current_zip.extractall(members=extract_member, path=extract_path, pwd=password)
+    file_automation_logger.info(
+        f"Unzip file: {zip_file_path}, "
+        f"extract member: {extract_member}, "
+        f"extract path: {extract_path}, "
+        f"password: {password}"
+    )
     current_zip.close()
 
 
 def zip_info(zip_file_path: str):
     current_zip = zipfile.ZipFile(zip_file_path, mode="r")
     info_list = current_zip.infolist()
     current_zip.close()
+    file_automation_logger.info(
+        f"Show zip info: {zip_file_path}"
+    )
     return info_list
 
 
 def zip_file_info(zip_file_path: str):
     current_zip = zipfile.ZipFile(zip_file_path, mode="r")
     name_list = current_zip.namelist()
     current_zip.close()
+    file_automation_logger.info(
+        f"Show zip file info: {zip_file_path}"
+    )
     return name_list
 
 
 def set_zip_password(zip_file_path: str, password: bytes):
     current_zip = zipfile.ZipFile(zip_file_path)
     current_zip.setpassword(pwd=password)
     current_zip.close()
+    file_automation_logger.info(
+        f"Set zip file password, "
+        f"zip file: {zip_file_path}, "
+        f"zup password: {password}"
+    )
```

### Comparing `automation_file_dev-0.0.4/pyproject.toml` & `automation_file_dev-0.0.5/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file_dev"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
     { name = "JE-Chen", email = "zenmailman@gmail.com" },
 ]
 description = ""
 readme = { file = "README.md", content-type = "text/markdown" }
 requires-python = ">=3.8"
 license = { text = "MIT" }
+dependencies = [
+    "google-api-python-client",
+    "google-auth-httplib2",
+    "google-auth-oauthlib",
+    "APScheduler"
+]
 classifiers = [
     "Programming Language :: Python :: 3.7",
     "Development Status :: 2 - Pre-Alpha",
     "Environment :: Win32 (MS Windows)",
     "Environment :: MacOS X",
     "Environment :: X11 Applications",
     "License :: OSI Approved :: MIT License",
```

