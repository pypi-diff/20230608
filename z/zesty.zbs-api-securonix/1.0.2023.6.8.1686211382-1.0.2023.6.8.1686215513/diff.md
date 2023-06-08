# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.6.8.1686211382.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.6.8.1686215513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.8.1686211382.tar", last modified: Thu Jun  8 08:03:02 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.8.1686215513.tar", last modified: Thu Jun  8 09:11:53 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382.tar` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    14360 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3683 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     8818 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7367 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    16027 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    14309 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16027 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    14309 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-06-08 09:04:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-08 09:11:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.6.8.1686211382
+Version: 1.0.2023.6.8.1686215513
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/README.md` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/setup.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/actions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/BlockDevice.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,18 +22,18 @@
             map: str = None,
             iops_stats: Dict[str, int] = None,
             parent: str = None,
             unlock_ts: int = 0,
             volume_id: str = None,
             volume_type: str = None,
             device: str = None,
-            btrfs_size: int = None
+            btrfs_size: int = None,
             extendable: bool = True,
             removable: bool = True
-            ):
+    ):
         """
         Block Device class doc:
         :param size: Size of the device in Bytes
         :param btrfs_dev_id: ID of the device inside the BTRFS structure
         :param cloud_vendor: Cloud vendor (AWS/Azure/GCP)
         :param created: Device creation date
         :param dev_usage: How much of the device is in use (in Bytes)
@@ -101,8 +101,7 @@
             return obj
 
     def serialize(self) -> dict:
         return self.as_dict()
 
     def __repr__(self) -> str:
         return str(self.as_dict())
-
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/EbsVolume.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/FileSystem.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/InstancesTags.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/ManagedFS.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/ManagedFS.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/protocol.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.6.8.1686211382
+Version: 1.0.2023.6.8.1686215513
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686215513/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

