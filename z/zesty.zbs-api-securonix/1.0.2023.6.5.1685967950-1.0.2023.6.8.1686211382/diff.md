# Comparing `tmp/zesty.zbs-api-securonix-1.0.2023.6.5.1685967950.tar.gz` & `tmp/zesty.zbs-api-securonix-1.0.2023.6.8.1686211382.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.5.1685967950.tar", last modified: Mon Jun  5 12:25:51 2023, max compression
+gzip compressed data, was "dist/zesty.zbs-api-securonix-1.0.2023.6.8.1686211382.tar", last modified: Thu Jun  8 08:03:02 2023, max compression
```

## Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950.tar` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/
--rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/README.md
--rw-r--r--   0 root         (0) root         (0)       60 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13458 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/actions.py
--rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/cloud_vendors.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/
--rw-rw-rw-   0 root         (0) root         (0)     3326 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/BlockDevice.py
--rw-rw-rw-   0 root         (0) root         (0)     7404 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/EbsVolume.py
--rw-rw-rw-   0 root         (0) root         (0)     7245 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/FileSystem.py
--rw-rw-rw-   0 root         (0) root         (0)     1879 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/InstancesTags.py
--rw-rw-rw-   0 root         (0) root         (0)    10693 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/ManagedFS.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/Usage.py
--rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/agent_report.py
--rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/cpu_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/disk_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/hf_interface.py
--rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/mem_mon.py
--rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/network_mon.py
--rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/overview.py
--rw-rw-rw-   0 root         (0) root         (0)    12497 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/protocol.py
--rw-rw-rw-   0 root         (0) root         (0)     7202 2023-06-05 12:24:46.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/step_instructions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1175 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      674 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-05 12:25:51.000000 zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/
+-rw-rw-rw-   0 root         (0) root         (0)      239 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      748 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/README.md
+-rw-r--r--   0 root         (0) root         (0)       60 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)      882 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    14360 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/actions.py
+-rw-rw-rw-   0 root         (0) root         (0)      268 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/cloud_vendors.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/
+-rw-rw-rw-   0 root         (0) root         (0)     3683 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/BlockDevice.py
+-rw-rw-rw-   0 root         (0) root         (0)     8818 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/EbsVolume.py
+-rw-rw-rw-   0 root         (0) root         (0)     7367 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/FileSystem.py
+-rw-rw-rw-   0 root         (0) root         (0)     2588 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/InstancesTags.py
+-rw-rw-rw-   0 root         (0) root         (0)    16027 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/ManagedFS.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/Usage.py
+-rw-rw-rw-   0 root         (0) root         (0)     1228 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/agent_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      873 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/cpu_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1154 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/disk_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     2738 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/hf_interface.py
+-rw-rw-rw-   0 root         (0) root         (0)      447 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/mem_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)      444 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/network_mon.py
+-rw-rw-rw-   0 root         (0) root         (0)     1935 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/overview.py
+-rw-rw-rw-   0 root         (0) root         (0)    14309 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/protocol.py
+-rw-rw-rw-   0 root         (0) root         (0)     7202 2023-06-08 08:01:53.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/step_instructions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1175 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      674 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-08 08:03:02.000000 zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/top_level.txt
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.6.5.1685967950
+Version: 1.0.2023.6.8.1686211382
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/README.md` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/README.md`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/setup.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/setup.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/actions.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/actions.py`

 * *Files 7% similar despite different names*

```diff
@@ -115,14 +115,19 @@
             "ZBSAgentReceiver 'remove_disk' is abstract, please implement a concrete per OD receiver")
 
     @abstractmethod
     def balance_ebs_structure(self, data: ZBSActionData, action_id) -> None:
         raise NotImplementedError(
             "ZBSAgentReceiver 'balance_ebs_structure' is abstract, please implement a concrete per OD receiver")
 
+    @abstractmethod
+    def start_migration(self, data: ZBSActionData, action_id, account_id=None) -> None:
+        raise NotImplementedError(
+            "ZBSAgentReceiver 'start_migration' is abstract, please implement a concrete per OD receiver")
+
 
 class SpecialInstructions(ISpecialInstructions):
     """
     Constructor for special instructions with optional parameters:
     * dev_id: identify the device for the filesystem to which the action is attached
     * size: specify the capacity for a new device or the additional capacity when extending a device
     * sub_actions: when an action implements multiple actions, specify a dictionary:
@@ -354,14 +359,30 @@
         except AttributeError as ex:
             print("Failed to execute command '{}': error is '{}'".format(self.get_action_type(), ex))
 
     class Factory:
         def create(self, uuid): return BalanceEBSStructureAction(uuid=uuid)
 
 
+class MigrationStartAction(ZBSAction):
+    """
+    Migration Start Action.
+    The purpose of this action is to get a BE request to start a migration action for a mount point
+    Returns: if migration started successfully or failed with the error
+    """
+
+    def execute(self, account_id):
+        try:
+            return self.receiver.start_migration(self.get_special_instructions(), self.get_action_id(), account_id)
+        except AttributeError as ex:
+            print("Failed to execute command '{}': error is '{}'".format(self.get_action_type(), ex))
+
+    class Factory:
+        def create(self, uuid): return MigrationStartAction(uuid=uuid)
+
 class ZBSActionFactory:
     actions = {}
 
     @staticmethod
     def create_action(action_type, uuid=None):
         if action_type not in ZBSActionFactory.actions:
             action_class = ZBSAction.subclasses.get(action_type)
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/BlockDevice.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/BlockDevice.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,17 @@
             iops_stats: Dict[str, int] = None,
             parent: str = None,
             unlock_ts: int = 0,
             volume_id: str = None,
             volume_type: str = None,
             device: str = None,
             btrfs_size: int = None
-    ):
+            extendable: bool = True,
+            removable: bool = True
+            ):
         """
         Block Device class doc:
         :param size: Size of the device in Bytes
         :param btrfs_dev_id: ID of the device inside the BTRFS structure
         :param cloud_vendor: Cloud vendor (AWS/Azure/GCP)
         :param created: Device creation date
         :param dev_usage: How much of the device is in use (in Bytes)
@@ -41,14 +43,16 @@
         :param iops_stats: Dict with IOPS statistics
         :param parent: If it's a partition so this one represent the parent device
         :param unlock_ts: TS when the device will be ready to be extended again
         :param volume_id: Device ID
         :param volume_type: Type of the device in the cloud
         :param device: Device mount slot from the cloud
         :param btrfs_size: The usable size for the filesystem in bytes
+        :param extendable: Whether ZestyDisk Handsfree logic is allowed to extend the device
+        :param removable: Whether ZestyDisk Handsfree logic is allowed to remove the device from the filesystem
         """
         # Init empty dict here instead of passing as default value
         iops_stats = {} if iops_stats is None else iops_stats
 
         self.size = size
         self.cloud_vendor = cloud_vendor
         try:
@@ -74,14 +78,16 @@
         if not unlock_ts:
             self.unlock_ts = 0
         else:
             self.unlock_ts = unlock_ts
 
         self.volume_type = volume_type
         self.btrfs_size = btrfs_size
+        self.extendable = extendable
+        self.removable = removable
     
     def as_dict(self) -> dict:
         return_dict = json.loads(json.dumps(self, default=self.object_dumper))
         return {k: v for k, v in return_dict.items() if v is not None}
 
     @staticmethod
     def object_dumper(obj) -> dict:
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/EbsVolume.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/EbsVolume.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from typing import Dict, Union
 
 from sqlalchemy.orm import Session, sessionmaker, Query
-from sqlalchemy.sql.elements import or_
+from sqlalchemy.sql.elements import or_, Label
+
+from .InstancesTags import InstancesTags
 
 try:
-    from sqlalchemy import Column, engine, case, func, cast, String
+    from sqlalchemy import Column, engine, case, func, cast, String, text
     from sqlalchemy.ext.declarative import declarative_base
     from sqlalchemy.dialects.postgresql import BOOLEAN, FLOAT, INTEGER, BIGINT, \
         JSON, TIMESTAMP, VARCHAR
 except ImportError:
     raise ImportError("sqlalchemy is required by zesty.zbs-api but needs to be vendored separately. Add postgres-utils to your project's requirements that depend on zbs-api.")
 
-try:
-    from zesty.models.InstancesTags import InstancesTags
-except ImportError:
-    from src.models.InstancesTags import InstancesTags
 
 Base = declarative_base()
 
 
 class EbsVolume(Base):
     # TODO: Move this model into our Alembic system
     # when a modification of this model is needed.
@@ -44,14 +42,17 @@
     monthly_cost = Column(FLOAT, default=0)
     is_unused_resource = Column(INTEGER, default=0)
     unused_since = Column(VARCHAR)
     agent_installed = Column(BOOLEAN, default=False)
     _zbs_supported_os = Column(INTEGER)
     potential_savings = Column(FLOAT, default=0)
 
+    # dict for custom_order_by class method
+    col_to_actual_sorting_col = {"instance_tags": "instance_tags_keys"}
+
     def __init__(
             self,
             volume_aws_schema: Dict,
             account_uuid: str = None):
         if account_uuid:
             self.account_uuid = account_uuid
         else:
@@ -82,77 +83,95 @@
         self.potential_savings = volume_aws_schema.get("potential_savings", 0)
 
     def __repr__(self):
         return f"{self.__tablename__}:{self.volume_id}"
 
     @classmethod
     def instance_id_filter(cls, query: Query, value: str):
+        val = f'%{value}%'
         query = query.filter(
             case((or_(cls.attached_to == None, func.json_array_length(cls.attached_to) == 0), False),
-                 else_=func.jsonb(cls.attached_to).op('?')(value)))
+                 else_=cast(cls.attached_to, String).ilike(val)))
         return query
 
     @classmethod
     def instance_name_filter(cls, query: Query, value: str):
-        session = query.session
-        subq = session.query(InstancesTags.instance_name)
-        query = query.filter(
-            cast(func.array(subq.scalar_subquery().where(func.jsonb(cls.attached_to).op('?')(InstancesTags.instance_id))), String)
-            .regexp_replace(r'[\{\}"]', '', 'g') == value)
+        subq = query.session.query(InstancesTags.instance_name)
+        val = '%{}%'.format(value.replace("%", "\\%"))
+        query = query.filter((subq.scalar_subquery().where(
+            (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (
+                cls.account_id == InstancesTags.account_id))).ilike(val))
         return query
 
     @classmethod
     def instance_tags_filter(cls, query: Query, value: str):
         session = query.session
         subq = session.query(InstancesTags.instance_tags)
 
         python_types_to_pg = {int: BIGINT, float: FLOAT, bool: BOOLEAN}
         for key_val in value:
             key = key_val.get('key')
             val = key_val.get('value')
             if key is not None and val is not None:
                 if not isinstance(val, str):
                     query = query.filter(cast(cast(func.jsonb(subq.scalar_subquery().where(
-                        func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id)).op('->')(key), String), python_types_to_pg[type(val)]) == val)
+                        (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (cls.account_id == InstancesTags.account_id)).op('->')(key)), String), python_types_to_pg[type(val)]) == val)
                 else:
-                    val = f'"{val}"'
+                    val = f'%{val}%'
                     query = query.filter(cast(func.jsonb(subq.scalar_subquery().where(
-                        func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id)).op('->')(key), String) == val)
+                        (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (cls.account_id == InstancesTags.account_id)).op('->')(key)), String).ilike(val))
             elif key is not None:
                 query = query.filter(func.jsonb(subq.scalar_subquery().where(
-                        func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id)).op('?')(key))
+                        (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (cls.account_id == InstancesTags.account_id))).op('?')(key))
             elif val is not None:
-                if isinstance(val, str) or isinstance(val, bool):
-                    val = f'"{val}"'
-                query = query.filter(cast(subq.scalar_subquery().where(
-                        func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id), String)
-                                     .regexp_replace(r'.+\: (' + str(val) + r')[,\s}].*', "\\1") == f"{val}")
+                if isinstance(val, str):
+                    query = query.filter(cast(subq.scalar_subquery().where(
+                            (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (cls.account_id == InstancesTags.account_id)), String)
+                                         .regexp_replace(r'.+\: "[^"]*(' + str(val) + r')[^"]*"[,\s}].*', "\\1") == f"{val}")
+                else:
+                    if isinstance(val, bool):
+                        val = f'"{val}"'
+                    query = query.filter(cast(subq.scalar_subquery().where(
+                            (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) & (cls.account_id == InstancesTags.account_id)), String)
+                                         .regexp_replace(r'.+\: (' + str(val) + r')[,\s}].*', "\\1") == f"{val}")
         return query
 
     # Custom query
     @classmethod
     def custom_query(cls, session: Union[Session, sessionmaker]) -> Query:
         q = session.query(cls)
-        subq = session.query(InstancesTags.instance_name)
         subq_2 = session.query(func.json_object_keys(InstancesTags.instance_tags))
         subq_3 = session.query(InstancesTags.instance_tags)
 
+        instance_name_clause = "regexp_replace(cast(array((select instances_tags.instance_name from instances_tags " \
+                               "inner join json_array_elements(disks.attached_to) as attached_to_set " \
+                               "on instances_tags.instance_id = replace(cast(attached_to_set.value as varchar), '\"', '') " \
+                               "and instances_tags.account_id = disks.account_id)) as varchar), '[\\{\\}\"]', '', 'g')"
+
         q = q.add_columns(case((or_(cls.attached_to == None, func.json_array_length(cls.attached_to) == 0), ''),
                                else_=cast(cls.attached_to, String).regexp_replace(r'[\[\]"]', '', 'g'))
                           .label("instance_id"),
-                          cast(func.array(subq.scalar_subquery().where(func.jsonb(cls.attached_to).op('?')(InstancesTags.instance_id))), String).regexp_replace(r'[\{\}"]', '', 'g')
-                          .label("instance_name"),
-                          func.array(subq_2.scalar_subquery().where(func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id))
+                          Label('instance_name', text(instance_name_clause)),
+                          func.array(subq_2.scalar_subquery().where(
+                              (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) &
+                              (cls.account_id == InstancesTags.account_id)))
                           .label('instance_tags_keys'),
-                          subq_3.scalar_subquery().where(func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id)
-                          .label('instance_tags')
-                          )
+                          subq_3.scalar_subquery().where(
+                              (func.jsonb(cls.attached_to).op('->>')(0) == InstancesTags.instance_id) &
+                              (cls.account_id == InstancesTags.account_id))
+                          .label('instance_tags'))
 
         return q
 
+    @classmethod
+    def custom_order_by(cls, sorting_column: str, sorting_order: str) -> str:
+        actual_sorting_column = cls.col_to_actual_sorting_col.get(sorting_column, sorting_column)
+
+        return f"{actual_sorting_column} {sorting_order}"
+
     def get_volume_id(self):
         return self.volume_id
 
     def as_dict(self):
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/FileSystem.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/FileSystem.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,14 +76,15 @@
             autoupdate_last_execution_time: str = None,
             statvfs_raw_data: Dict[str, str] = None,
             pvc_id: str = None,
             mount_options: list = None,
             leading_device: str = None,
             policies: Dict[str, dict] = None,
             instance_tags: Dict[str, str] = None,
+            is_manageable: bool = False, #related migration
             is_emr: bool = False
             ):
 
         # Initialize empty dict not as default arg
         existing_actions = {} if existing_actions is None else existing_actions
         devices = {} if devices is None else devices
         inodes = {} if inodes is None else inodes
@@ -159,14 +160,15 @@
         self.autoupdate_last_execution_time = autoupdate_last_execution_time
         self.statvfs_raw_data = statvfs_raw_data
         self.pvc_id = pvc_id
         self.mount_options = mount_options
         self.leading_device = leading_device
         self.policies = policies
         self.instance_tags = instance_tags
+        self.is_manageable = is_manageable #related migration
         self.is_emr = is_emr
 
     @staticmethod
     def init_devices(devices: Dict[str, BlockDevice]):
         if not devices:
             return {}
         else:
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/InstancesTags.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/InstancesTags.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,63 @@
+import json
 import time
+from datetime import datetime
 from typing import Dict, Union
 
+from .ManagedFS import Base, BaseMixin
+
 try:
-    from sqlalchemy import Column, engine, cast, String, case, func, or_, select, text, PrimaryKeyConstraint
+    from sqlalchemy import (Column, PrimaryKeyConstraint, String, case, cast,
+                            engine, func, or_, select, text)
+    from sqlalchemy.dialects.postgresql import (BIGINT, BOOLEAN, FLOAT, JSON,
+                                                VARCHAR)
     from sqlalchemy.ext.declarative import declarative_base
-    from sqlalchemy.orm import aliased, Session, sessionmaker
-    from sqlalchemy.dialects.postgresql import BIGINT, BOOLEAN, FLOAT, \
-        JSON, VARCHAR
-    from sqlalchemy.orm import Query
+    from sqlalchemy.orm import Query, Session, aliased, sessionmaker
 except ImportError:
-    raise ImportError("sqlalchemy is required by zesty.zbs-api but needs to be vendored separately. Add postgres-utils to your project's requirements that depend on zbs-api.")
-
-Base = declarative_base()
+    raise ImportError(
+        "sqlalchemy is required by zesty.zbs-api but needs to be vendored separately. Add postgres-utils to your project's requirements that depend on zbs-api.")
 
 
-class InstancesTags(Base):
+class InstancesTags(BaseMixin, Base):
     __tablename__ = "instances_tags"
 
     instance_id = Column(VARCHAR, primary_key=True)
     account_id = Column(VARCHAR, index=True, default=None)
     account_uuid = Column(VARCHAR, index=True, default=None)
     instance_name = Column(VARCHAR, default=None)
     instance_tags = Column(JSON, default=None)
+    expired_at = Column(BIGINT, default=None)
 
     __table_args__ = (
         PrimaryKeyConstraint('instance_id', name='instances_tags_pkey'),)
 
     def __init__(
             self,
             instance_id: str,
             account_id: str = None,
             account_uuid: str = None,
             instance_name: str = None,
-            instance_tags: dict = None
-            ):
-        self.instance_id = instance_id,
+            instance_tags: dict = None,
+            expired_at: int = None
+    ):
+        self.instance_id = instance_id
         self.account_id = account_id
         self.account_uuid = account_uuid
         self.instance_name = instance_name
         self.instance_tags = instance_tags
+        self.expired_at = expired_at or int(datetime.utcnow().timestamp()) + 3 * 3600
+
+    def __eq__(self, other) -> bool:
+        return self.__hash__() == other.__hash__()
+
+    def __hash__(self) -> int:
+        return hash(''.join(map(lambda c: getattr(self, c.name) or '',
+                                filter(lambda c: c.name not in ['instance_tags', 'expired_at', 'created_at', 'updated_at'],
+                                       self.__table__.columns))) +
+                    json.dumps(self.instance_tags))
 
     def __repr__(self) -> str:
         return f"{self.__tablename__}:{self.instance_id}"
 
     def asdict(self) -> dict:
         return {c.name: getattr(self, c.name) for c in self.__table__.columns}
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/Usage.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/Usage.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/agent_report.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/agent_report.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/cpu_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/cpu_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/disk_mon.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/disk_mon.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/hf_interface.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/hf_interface.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/models/overview.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/models/overview.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/protocol.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/protocol.py`

 * *Files 8% similar despite different names*

```diff
@@ -399,7 +399,60 @@
             self.stage = stage
             self.version = version
             self.api_key = api_key
             self.api_base = api_base
 
         def create(self): return SyncMachineActions(stage=self.stage, version=self.version, api_key=self.api_key,
                                                     api_base=self.api_base)
+
+
+class MigrationStartActionCompleted(Request):
+    message = {}
+
+    def build_url(self):
+        if self.api_is_private_endpoint:
+            return '{}{}'.format(self.api_base, "/post-migration-start-action-complete")
+        else:
+            return '{}{}'.format(self.api_base, cfg.migration_start_action_completed_ep)
+
+    def set_data(self, account_id, fs_id, action_id, mount_path, volume_id, region, cloud_vendor, dev_path, exit_code,
+                 error):
+        self.message = {
+            "account_id": account_id,
+            "fs_id": fs_id,
+            "action_id": action_id,
+            "mount_path": mount_path,
+            "volume_id": volume_id,
+            "region": region,
+            "cloud_vendor": cloud_vendor,
+            "dev_path": dev_path,
+            "exit_code": exit_code,
+            "error": error
+        }
+
+    class Response:
+        raw_data = None
+        status_code = None
+        success = None
+        message = None
+
+        def __init__(self, res):
+            self.status_code = res.status_code
+            self.raw_data = res.json()
+            self.success = self.raw_data.get('Success')
+            self.message = self.raw_data.get('message')
+
+    class Factory:
+        stage = None
+        version = None
+        api_key = None
+        api_base = None
+
+        def __init__(self, stage, version, api_key, api_base: str = DEFAULT_BASE_URL):
+            self.stage = stage
+            self.version = version
+            self.api_key = api_key
+            self.api_base = api_base
+
+        def create(self): return MigrationStartActionCompleted(stage=self.stage, version=self.version,
+                                                               api_key=self.api_key,
+                                                               api_base=self.api_base)
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/src/step_instructions.py` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/src/step_instructions.py`

 * *Files identical despite different names*

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/PKG-INFO` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zesty.zbs-api-securonix
-Version: 1.0.2023.6.5.1685967950
+Version: 1.0.2023.6.8.1686211382
 Summary: Zesty Disk API
 Home-page: https://github.com/javatechy/dokr
 Author: Zesty.co
 Author-email: rnd@cloudvisor.co
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `zesty.zbs-api-securonix-1.0.2023.6.5.1685967950/zesty.zbs_api_securonix.egg-info/SOURCES.txt` & `zesty.zbs-api-securonix-1.0.2023.6.8.1686211382/zesty.zbs_api_securonix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

