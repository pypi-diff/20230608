# Comparing `tmp/mount_azure_blob-0.0.5.tar.gz` & `tmp/mount_azure_blob-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mount_azure_blob-0.0.5.tar", last modified: Mon Apr  3 06:08:33 2023, max compression
+gzip compressed data, was "mount_azure_blob-0.0.6.tar", last modified: Thu Jun  8 05:39:59 2023, max compression
```

## Comparing `mount_azure_blob-0.0.5.tar` & `mount_azure_blob-0.0.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:08:33.554694 mount_azure_blob-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-03 06:08:33.550694 mount_azure_blob-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-03 06:08:09.000000 mount_azure_blob-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 06:08:33.550694 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-04-03 06:08:33.000000 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-04-03 06:08:33.000000 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:08:33.000000 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 06:08:33.000000 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-03 06:08:33.000000 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-03 06:08:33.000000 mount_azure_blob-0.0.5/mount_azure_blob.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-04-03 06:08:09.000000 mount_azure_blob-0.0.5/mount_azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 06:08:33.554694 mount_azure_blob-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-03 06:08:09.000000 mount_azure_blob-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-08 05:39:48.000000 mount_azure_blob-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-08 05:39:48.000000 mount_azure_blob-0.0.6/mount_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 05:39:48.000000 mount_azure_blob-0.0.6/setup.py
```

### Comparing `mount_azure_blob-0.0.5/PKG-INFO` & `mount_azure_blob-0.0.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mount_azure_blob
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mount Azure blob storage in google colab.
 Home-page: https://github.com/lkarjun/mount-azure-blob-storage/
 Author: Lalkrishna
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Mount Azure Blob Storage in Colab
@@ -22,17 +22,17 @@
 ### Approch 2
 ```
 from mount_azure_blob import mount_storage
 mount_storage(mount_path="blob-storage", config_file="path-to-.env-file")
 ```
 #### sample ```config_file``` / ```.env```
 ```
-account_name="..."
-account_key="..."
-container_name="..."
+accountName ...
+accountKey ...
+containerName ...
 ```
 output: 
 
 ![image](https://user-images.githubusercontent.com/58617251/222144492-88eebbfa-4e91-48c6-acec-950f2bf7b799.png)
 
 ### After mount
 ![image](https://user-images.githubusercontent.com/58617251/222145707-28b625a6-a1f0-479c-9748-e7ad69a18fa3.png)
```

### Comparing `mount_azure_blob-0.0.5/README.md` & `mount_azure_blob-0.0.6/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 ### Approch 2
 ```
 from mount_azure_blob import mount_storage
 mount_storage(mount_path="blob-storage", config_file="path-to-.env-file")
 ```
 #### sample ```config_file``` / ```.env```
 ```
-account_name="..."
-account_key="..."
-container_name="..."
+accountName ...
+accountKey ...
+containerName ...
 ```
 output: 
 
 ![image](https://user-images.githubusercontent.com/58617251/222144492-88eebbfa-4e91-48c6-acec-950f2bf7b799.png)
 
 ### After mount
 ![image](https://user-images.githubusercontent.com/58617251/222145707-28b625a6-a1f0-479c-9748-e7ad69a18fa3.png)
```

### Comparing `mount_azure_blob-0.0.5/mount_azure_blob.egg-info/PKG-INFO` & `mount_azure_blob-0.0.6/mount_azure_blob.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mount-azure-blob
-Version: 0.0.5
+Version: 0.0.6
 Summary: Mount Azure blob storage in google colab.
 Home-page: https://github.com/lkarjun/mount-azure-blob-storage/
 Author: Lalkrishna
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Mount Azure Blob Storage in Colab
@@ -22,17 +22,17 @@
 ### Approch 2
 ```
 from mount_azure_blob import mount_storage
 mount_storage(mount_path="blob-storage", config_file="path-to-.env-file")
 ```
 #### sample ```config_file``` / ```.env```
 ```
-account_name="..."
-account_key="..."
-container_name="..."
+accountName ...
+accountKey ...
+containerName ...
 ```
 output: 
 
 ![image](https://user-images.githubusercontent.com/58617251/222144492-88eebbfa-4e91-48c6-acec-950f2bf7b799.png)
 
 ### After mount
 ![image](https://user-images.githubusercontent.com/58617251/222145707-28b625a6-a1f0-479c-9748-e7ad69a18fa3.png)
```

