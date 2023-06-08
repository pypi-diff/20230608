# Comparing `tmp/automation_file-0.0.3.tar.gz` & `tmp/automation_file-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automation_file-0.0.3.tar", last modified: Mon May 29 02:44:13 2023, max compression
+gzip compressed data, was "automation_file-0.0.4.tar", last modified: Thu Jun  8 08:35:14 2023, max compression
```

## Comparing `automation_file-0.0.3.tar` & `automation_file-0.0.4.tar`

### file list

```diff
@@ -1,34 +1,57 @@
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.487630 automation_file-0.0.3/
--rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     1372 2023-05-29 02:44:13.486629 automation_file-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      749 2023-05-29 01:54:01.000000 automation_file-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.437231 automation_file-0.0.3/automation_file.egg-info/
--rw-rw-rw-   0        0        0     1372 2023-05-29 02:44:13.000000 automation_file-0.0.3/automation_file.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      747 2023-05-29 02:44:13.000000 automation_file-0.0.3/automation_file.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-29 02:44:13.000000 automation_file-0.0.3/automation_file.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-05-29 02:44:13.000000 automation_file-0.0.3/automation_file.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.442052 automation_file-0.0.3/file_automation/
--rw-rw-rw-   0        0        0      732 2023-05-29 02:35:20.000000 automation_file-0.0.3/file_automation/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.447779 automation_file-0.0.3/file_automation/local/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.3/file_automation/local/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.453775 automation_file-0.0.3/file_automation/local/dir/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.3/file_automation/local/dir/__init__.py
--rw-rw-rw-   0        0        0     1230 2023-05-19 07:13:21.000000 automation_file-0.0.3/file_automation/local/dir/dir_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.459773 automation_file-0.0.3/file_automation/local/file/
--rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.3/file_automation/local/file/__init__.py
--rw-rw-rw-   0        0        0     2205 2023-05-19 06:44:49.000000 automation_file-0.0.3/file_automation/local/file/file_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.465268 automation_file-0.0.3/file_automation/local/zip/
--rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.3/file_automation/local/zip/__init__.py
--rw-rw-rw-   0        0        0     2383 2023-05-19 09:53:23.000000 automation_file-0.0.3/file_automation/local/zip/zip_process.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.469271 automation_file-0.0.3/file_automation/remote/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.3/file_automation/remote/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.472139 automation_file-0.0.3/file_automation/remote/google_drive/
--rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.3/file_automation/remote/google_drive/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.475147 automation_file-0.0.3/file_automation/utils/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.3/file_automation/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-29 02:44:13.483393 automation_file-0.0.3/file_automation/utils/exception/
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.3/file_automation/utils/exception/__init__.py
--rw-rw-rw-   0        0        0        0 2023-05-18 07:59:25.000000 automation_file-0.0.3/file_automation/utils/exception/exception_tags.py
--rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file-0.0.3/file_automation/utils/exception/exceptions.py
--rw-rw-rw-   0        0        0      873 2023-05-29 02:42:10.000000 automation_file-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-29 02:44:13.488631 automation_file-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.456562 automation_file-0.0.4/
+-rw-rw-rw-   0        0        0     1085 2023-05-18 06:36:21.000000 automation_file-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1302 2023-06-08 08:35:14.455556 automation_file-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      679 2023-05-30 06:22:36.000000 automation_file-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.354603 automation_file-0.0.4/automation_file.egg-info/
+-rw-rw-rw-   0        0        0     1302 2023-06-08 08:35:14.000000 automation_file-0.0.4/automation_file.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1618 2023-06-08 08:35:14.000000 automation_file-0.0.4/automation_file.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-08 08:35:14.000000 automation_file-0.0.4/automation_file.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       79 2023-06-08 08:35:14.000000 automation_file-0.0.4/automation_file.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-06-08 08:35:14.000000 automation_file-0.0.4/automation_file.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.359606 automation_file-0.0.4/file_automation/
+-rw-rw-rw-   0        0        0      835 2023-06-05 01:25:45.000000 automation_file-0.0.4/file_automation/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.362604 automation_file-0.0.4/file_automation/local/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:02.000000 automation_file-0.0.4/file_automation/local/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.370859 automation_file-0.0.4/file_automation/local/dir/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:51.000000 automation_file-0.0.4/file_automation/local/dir/__init__.py
+-rw-rw-rw-   0        0        0     2135 2023-06-08 06:26:10.000000 automation_file-0.0.4/file_automation/local/dir/dir_process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.377404 automation_file-0.0.4/file_automation/local/file/
+-rw-rw-rw-   0        0        0        0 2023-05-18 06:38:46.000000 automation_file-0.0.4/file_automation/local/file/__init__.py
+-rw-rw-rw-   0        0        0     3716 2023-06-08 06:40:19.000000 automation_file-0.0.4/file_automation/local/file/file_process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.383621 automation_file-0.0.4/file_automation/local/zip/
+-rw-rw-rw-   0        0        0        0 2023-05-19 07:24:05.000000 automation_file-0.0.4/file_automation/local/zip/__init__.py
+-rw-rw-rw-   0        0        0     3626 2023-06-08 07:15:08.000000 automation_file-0.0.4/file_automation/local/zip/zip_process.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.386778 automation_file-0.0.4/file_automation/remote/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:15.000000 automation_file-0.0.4/file_automation/remote/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.391755 automation_file-0.0.4/file_automation/remote/google_drive/
+-rw-rw-rw-   0        0        0        0 2023-05-29 02:05:24.000000 automation_file-0.0.4/file_automation/remote/google_drive/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.397910 automation_file-0.0.4/file_automation/remote/google_drive/delete/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/remote/google_drive/delete/__init__.py
+-rw-rw-rw-   0        0        0      648 2023-06-08 07:37:31.000000 automation_file-0.0.4/file_automation/remote/google_drive/delete/delete_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.404270 automation_file-0.0.4/file_automation/remote/google_drive/dir/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/remote/google_drive/dir/__init__.py
+-rw-rw-rw-   0        0        0      876 2023-06-08 07:41:43.000000 automation_file-0.0.4/file_automation/remote/google_drive/dir/folder_manager.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.410277 automation_file-0.0.4/file_automation/remote/google_drive/download/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/remote/google_drive/download/__init__.py
+-rw-rw-rw-   0        0        0     2139 2023-06-08 07:46:57.000000 automation_file-0.0.4/file_automation/remote/google_drive/download/download_file.py
+-rw-rw-rw-   0        0        0     2200 2023-06-08 08:10:58.000000 automation_file-0.0.4/file_automation/remote/google_drive/driver_instance.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.418919 automation_file-0.0.4/file_automation/remote/google_drive/search/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/remote/google_drive/search/__init__.py
+-rw-rw-rw-   0        0        0     2308 2023-06-08 07:49:23.000000 automation_file-0.0.4/file_automation/remote/google_drive/search/search_drive.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.425117 automation_file-0.0.4/file_automation/remote/google_drive/share/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/remote/google_drive/share/__init__.py
+-rw-rw-rw-   0        0        0     2524 2023-06-08 07:55:10.000000 automation_file-0.0.4/file_automation/remote/google_drive/share/share_file.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.432654 automation_file-0.0.4/file_automation/remote/google_drive/upload/
+-rw-rw-rw-   0        0        0        0 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/remote/google_drive/upload/__init__.py
+-rw-rw-rw-   0        0        0     3823 2023-06-08 08:10:58.000000 automation_file-0.0.4/file_automation/remote/google_drive/upload/upload_to_driver.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.435655 automation_file-0.0.4/file_automation/utils/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:01.000000 automation_file-0.0.4/file_automation/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.445556 automation_file-0.0.4/file_automation/utils/exception/
+-rw-rw-rw-   0        0        0        0 2023-05-18 07:59:15.000000 automation_file-0.0.4/file_automation/utils/exception/__init__.py
+-rw-rw-rw-   0        0        0       46 2023-06-05 01:25:46.000000 automation_file-0.0.4/file_automation/utils/exception/exception_tags.py
+-rw-rw-rw-   0        0        0      165 2023-05-19 07:56:11.000000 automation_file-0.0.4/file_automation/utils/exception/exceptions.py
+drwxrwxrwx   0        0        0        0 2023-06-08 08:35:14.452548 automation_file-0.0.4/file_automation/utils/logging/
+-rw-rw-rw-   0        0        0        0 2023-06-08 03:44:59.000000 automation_file-0.0.4/file_automation/utils/logging/__init__.py
+-rw-rw-rw-   0        0        0      372 2023-06-08 05:31:05.000000 automation_file-0.0.4/file_automation/utils/logging/loggin_instance.py
+-rw-rw-rw-   0        0        0     1004 2023-06-08 08:34:52.000000 automation_file-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-08 08:35:14.456562 automation_file-0.0.4/setup.cfg
```

### Comparing `automation_file-0.0.3/LICENSE` & `automation_file-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `automation_file-0.0.3/automation_file.egg-info/SOURCES.txt` & `automation_file-0.0.4/automation_file.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,37 @@
 LICENSE
 README.md
 pyproject.toml
 automation_file.egg-info/PKG-INFO
 automation_file.egg-info/SOURCES.txt
 automation_file.egg-info/dependency_links.txt
+automation_file.egg-info/requires.txt
 automation_file.egg-info/top_level.txt
 file_automation/__init__.py
 file_automation/local/__init__.py
 file_automation/local/dir/__init__.py
 file_automation/local/dir/dir_process.py
 file_automation/local/file/__init__.py
 file_automation/local/file/file_process.py
 file_automation/local/zip/__init__.py
 file_automation/local/zip/zip_process.py
 file_automation/remote/__init__.py
 file_automation/remote/google_drive/__init__.py
+file_automation/remote/google_drive/driver_instance.py
+file_automation/remote/google_drive/delete/__init__.py
+file_automation/remote/google_drive/delete/delete_manager.py
+file_automation/remote/google_drive/dir/__init__.py
+file_automation/remote/google_drive/dir/folder_manager.py
+file_automation/remote/google_drive/download/__init__.py
+file_automation/remote/google_drive/download/download_file.py
+file_automation/remote/google_drive/search/__init__.py
+file_automation/remote/google_drive/search/search_drive.py
+file_automation/remote/google_drive/share/__init__.py
+file_automation/remote/google_drive/share/share_file.py
+file_automation/remote/google_drive/upload/__init__.py
+file_automation/remote/google_drive/upload/upload_to_driver.py
 file_automation/utils/__init__.py
 file_automation/utils/exception/__init__.py
 file_automation/utils/exception/exception_tags.py
-file_automation/utils/exception/exceptions.py
+file_automation/utils/exception/exceptions.py
+file_automation/utils/logging/__init__.py
+file_automation/utils/logging/loggin_instance.py
```

### Comparing `automation_file-0.0.3/file_automation/__init__.py` & `automation_file-0.0.4/file_automation/__init__.py`

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

### Comparing `automation_file-0.0.3/file_automation/local/zip/zip_process.py` & `automation_file-0.0.4/file_automation/local/zip/zip_process.py`

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

### Comparing `automation_file-0.0.3/pyproject.toml` & `automation_file-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,28 @@
 # This is dev version
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "automation_file"
-version = "0.0.3"
+version = "0.0.4"
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

