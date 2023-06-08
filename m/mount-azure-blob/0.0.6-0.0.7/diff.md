# Comparing `tmp/mount_azure_blob-0.0.6.tar.gz` & `tmp/mount_azure_blob-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mount_azure_blob-0.0.6.tar", last modified: Thu Jun  8 05:39:59 2023, max compression
+gzip compressed data, was "mount_azure_blob-0.0.7.tar", last modified: Thu Jun  8 05:52:01 2023, max compression
```

## Comparing `mount_azure_blob-0.0.6.tar` & `mount_azure_blob-0.0.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-08 05:39:48.000000 mount_azure_blob-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 05:39:59.000000 mount_azure_blob-0.0.6/mount_azure_blob.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3603 2023-06-08 05:39:48.000000 mount_azure_blob-0.0.6/mount_azure_blob.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 05:39:59.908059 mount_azure_blob-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 05:39:48.000000 mount_azure_blob-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:52:01.393192 mount_azure_blob-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 05:52:01.393192 mount_azure_blob-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-08 05:51:49.000000 mount_azure_blob-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 05:52:01.393192 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-08 05:52:01.000000 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-06-08 05:52:01.000000 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:52:01.000000 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 05:52:01.000000 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-08 05:52:01.000000 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-08 05:52:01.000000 mount_azure_blob-0.0.7/mount_azure_blob.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-06-08 05:51:49.000000 mount_azure_blob-0.0.7/mount_azure_blob.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 05:52:01.393192 mount_azure_blob-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-08 05:51:49.000000 mount_azure_blob-0.0.7/setup.py
```

### Comparing `mount_azure_blob-0.0.6/PKG-INFO` & `mount_azure_blob-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mount_azure_blob
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mount Azure blob storage in google colab.
 Home-page: https://github.com/lkarjun/mount-azure-blob-storage/
 Author: Lalkrishna
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Mount Azure Blob Storage in Colab
```

### Comparing `mount_azure_blob-0.0.6/README.md` & `mount_azure_blob-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `mount_azure_blob-0.0.6/mount_azure_blob.egg-info/PKG-INFO` & `mount_azure_blob-0.0.7/mount_azure_blob.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mount-azure-blob
-Version: 0.0.6
+Version: 0.0.7
 Summary: Mount Azure blob storage in google colab.
 Home-page: https://github.com/lkarjun/mount-azure-blob-storage/
 Author: Lalkrishna
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Mount Azure Blob Storage in Colab
```

### Comparing `mount_azure_blob-0.0.6/mount_azure_blob.py` & `mount_azure_blob-0.0.7/mount_azure_blob.py`

 * *Files 3% similar despite different names*

```diff
@@ -33,36 +33,40 @@
     print(f"Config created file={config_export_path}...")
 
 
 def _mount_storage_helper(
     mount_path, account_name=None, account_key=None, container_name=None, config_file=None
 ):
     print("\nMounting azure blob storage (blobfuse v1)...")
+    rm_config = False
     if config_file is None:
+        rm_config = True
         config_file = "fuse_connection.cfg"
         with open(config_file, "w") as f:
             content = f"""accountName {account_name}\naccountKey {account_key}\ncontainerName {container_name}"""
             f.write(content)
     print("Installing Dependencies...")
     install_dependenices()
 
     command = f"""
         chmod 600 fuse_connection.cfg
         mkdir {mount_path}
         sudo blobfuse {mount_path} --tmp-path=/mnt/resource/blobfusetmp  --config-file={config_file} -o attr_timeout=240 -o entry_timeout=240 -o negative_timeout=120
-        rm fuse_connection.cfg
       """
     
     try:
         output = subprocess.check_output(command, shell=True)
     except subprocess.CalledProcessError as e:
         output = e.output.decode()
         print("\nFailed to Mount Blob Storage...\n")
         print(str(e))
 
+    if rm_config:
+        os.remove(config_file)
+
     print("Successfully Mounted...")
 
 
 def _mount_storage__widget_helper(
     btn: widgets.Button,
     accountName: widgets.Text, 
     accountKey: widgets.Text,
```

