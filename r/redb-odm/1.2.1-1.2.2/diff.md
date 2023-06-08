# Comparing `tmp/redb-odm-1.2.1.tar.gz` & `tmp/redb-odm-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redb-odm-1.2.1.tar", last modified: Sun May 21 01:19:03 2023, max compression
+gzip compressed data, was "redb-odm-1.2.2.tar", last modified: Thu Jun  8 18:15:57 2023, max compression
```

## Comparing `redb-odm-1.2.1.tar` & `redb-odm-1.2.2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 01:18:47.000000 redb-odm-1.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-21 01:19:03.058179 redb-odm-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 01:18:47.000000 redb-odm-1.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.054179 redb-odm-1.2.1/redb/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.054179 redb-odm-1.2.1/redb/behaviors/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/behaviors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7885 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/behaviors/i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/behaviors/soft_deletion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.054179 redb-odm-1.2.1/redb/core/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16207 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/core/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/core/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/redb/interface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/interface/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/redb/json_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/json_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/json_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/json_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/json_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/redb/migo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/migo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/migo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/migo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/migo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/redb/mongo_system/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/mongo_system/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/mongo_system/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/mongo_system/collection.py
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-05-21 01:18:47.000000 redb-odm-1.2.1/redb/mongo_system/database.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/redb_odm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-21 01:19:03.000000 redb-odm-1.2.1/redb_odm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-05-21 01:19:03.000000 redb-odm-1.2.1/redb_odm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:19:03.000000 redb-odm-1.2.1/redb_odm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-05-21 01:19:03.000000 redb-odm-1.2.1/redb_odm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 01:19:03.000000 redb-odm-1.2.1/redb_odm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-21 01:18:47.000000 redb-odm-1.2.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-21 01:18:47.000000 redb-odm-1.2.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-21 01:18:47.000000 redb-odm-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 01:19:03.058179 redb-odm-1.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-21 01:18:47.000000 redb-odm-1.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:19:03.058179 redb-odm-1.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_bson_objs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_hashing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_i_remember.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_json_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     8572 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_mongo_system.py
--rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_return_cls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-21 01:18:47.000000 redb-odm-1.2.1/tests/test_soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.255736 redb-odm-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-08 18:15:38.000000 redb-odm-1.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 18:15:57.255736 redb-odm-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-08 18:15:38.000000 redb-odm-1.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.243736 redb-odm-1.2.2/redb/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.247736 redb-odm-1.2.2/redb/behaviors/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/behaviors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/behaviors/i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/behaviors/soft_deletion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.247736 redb-odm-1.2.2/redb/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6838 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16621 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3005 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/interface/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/json_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9263 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1374 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/json_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/migo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1654 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11715 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/migo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb/mongo_system/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6017 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-08 18:15:38.000000 redb-odm-1.2.2/redb/mongo_system/database.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.251736 redb-odm-1.2.2/redb_odm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 18:15:57.000000 redb-odm-1.2.2/redb_odm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-08 18:15:38.000000 redb-odm-1.2.2/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-08 18:15:38.000000 redb-odm-1.2.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-08 18:15:38.000000 redb-odm-1.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 18:15:57.255736 redb-odm-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-06-08 18:15:38.000000 redb-odm-1.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 18:15:57.255736 redb-odm-1.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_bson_objs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_hashing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5326 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_i_remember.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_json_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8216 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_mongo_system.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_return_cls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_soft_deletion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-06-08 18:15:38.000000 redb-odm-1.2.2/tests/test_unique_constraints.py
```

### Comparing `redb-odm-1.2.1/redb/behaviors/i_remember.py` & `redb-odm-1.2.2/redb/behaviors/i_remember.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
         out = super().dict(*args, **kwargs)
         return out
 
     @classmethod
     def get_hashable_fields(cls) -> list[ClassField]:
         all_fields = super().get_hashable_fields()
-        return list(filter(lambda x: x.model_field.name in HISTORY_FIELDS, all_fields))
+        return list(filter(lambda x: x.model_field.name not in HISTORY_FIELDS, all_fields))
 
     @classmethod
     def historical_find_one(
         cls: Type[T],
         filter: OptionalDocumentData = None,
         fields: IncludeColumns = None,
         skip: int = 0,
@@ -231,12 +231,12 @@
 
         new_history = referenced_doc.dict(
             ignored_history_fields=False,
             exclude={"id"},
             exclude_none=True,
         )
         new_history["version"] = version
-        new_history["retired_by"] = user_info.dict()
+        new_history["retired_by"] = user_info.dict() if hasattr(user_info, "dict") else str(user_info)
         new_history["retired_at"] = pytz.UTC.localize(datetime.utcnow()).isoformat()
         new_history["ref_id"] = referenced_doc.id
         new_history["_id"] = f"{referenced_doc.id}_v{version}"
         return new_history
```

### Comparing `redb-odm-1.2.1/redb/behaviors/soft_deletion.py` & `redb-odm-1.2.2/redb/behaviors/soft_deletion.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/core/base.py` & `redb-odm-1.2.2/redb/core/base.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/core/document.py` & `redb-odm-1.2.2/redb/core/document.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from datetime import datetime
 from typing import Any, Dict, Sequence, Type, TypeAlias, TypeVar, Union, cast
 
 import pytz
 from pymongo.errors import DuplicateKeyError
-
 from redb.interface.errors import (
     CannotUpdateIdentifyingField,
     UniqueConstraintViolation,
 )
 from redb.interface.fields import (
     CompoundIndex,
     DBRef,
@@ -174,15 +173,17 @@
         data = _format_document_data(self)
         try:
             return collection.insert_one(
                 cls=self.__class__,
                 data=data,
             )
         except DuplicateKeyError as e:
-            raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"], collection_name=self.collection_name()
+            )
 
     @classmethod
     def insert_one(
         cls: Type[T],
         data: DocumentData,
     ) -> InsertOneResult:
         _validate_fields(cls, data)
@@ -191,15 +192,17 @@
         data = _format_document_data(data)
         try:
             return collection.insert_one(
                 cls=cls,
                 data=data,
             )
         except DuplicateKeyError as e:
-            raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"], collection_name=cls.collection_name()
+            )
 
     @classmethod
     def insert_vectors(
         cls: Type[T],
         data: Dict[str, list[Any]],
     ) -> InsertManyResult:
         collection = Document._get_collection(cls)
@@ -209,15 +212,17 @@
         instances = [{key: data[key][i] for key in keys} for i in range(values_size)]
         try:
             return collection.insert_many(
                 cls=cls,
                 data=instances,
             )
         except DuplicateKeyError as e:
-            raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"], collection_name=cls.collection_name()
+            )
 
     @classmethod
     def insert_many(
         cls: Type[T],
         data: Sequence[DocumentData],
     ) -> InsertManyResult:
         for val in data:
@@ -227,15 +232,17 @@
         try:
             result = collection.insert_many(
                 cls=cls,
                 data=data,
             )
             return result
         except DuplicateKeyError as e:
-            raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"], collection_name=cls.collection_name()
+            )
 
     def replace(
         self: T,
         replacement: DocumentData,
         upsert: bool = False,
         allow_new_fields: bool = False,
     ) -> ReplaceOneResult:
@@ -339,15 +346,17 @@
             )
             collection.update_one(
                 cls=cls,
                 filter=filter,
                 update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
             )
         except DuplicateKeyError as e:
-            raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"], collection_name=cls.collection_name()
+            )
         return result
 
     @classmethod
     def update_many(
         cls: Type[T],
         filter: DocumentData,
         update: DocumentData,
@@ -378,15 +387,17 @@
             )
             collection.update_many(
                 cls=cls,
                 filter=filter,
                 update={"$set": {"updated_at": datetime.now(pytz.UTC).isoformat()}},
             )
         except DuplicateKeyError as e:
-            raise UniqueConstraintViolation(dup_keys=e.details["keyValue"])
+            raise UniqueConstraintViolation(
+                dup_keys=e.details["keyValue"], collection_name=cls.collection_name()
+            )
 
         return result
 
     def delete(self: T) -> DeleteOneResult:
         collection = Document._get_collection(self.__class__)
         filter = _format_document_data(self)
         return collection.delete_one(
```

### Comparing `redb-odm-1.2.1/redb/core/instance.py` & `redb-odm-1.2.2/redb/core/instance.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/core/transaction.py` & `redb-odm-1.2.2/redb/core/transaction.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/core/utils.py` & `redb-odm-1.2.2/redb/core/utils.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/interface/client.py` & `redb-odm-1.2.2/redb/interface/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/interface/collection.py` & `redb-odm-1.2.2/redb/interface/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/interface/configs.py` & `redb-odm-1.2.2/redb/interface/configs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/interface/database.py` & `redb-odm-1.2.2/redb/interface/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/interface/errors.py` & `redb-odm-1.2.2/redb/interface/errors.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 class REDBError(Exception):
     """Base class for all REDB errors."""
 
+    def __init__(self, *args: object, collection_name: str = "") -> None:
+        super().__init__(*args)
+        self.collection_name = collection_name
+
     pass
 
 
 class DocumentNotFound(REDBError):
     pass
 
 
 class CannotUpdateIdentifyingField(REDBError):
     pass
 
 
 class UniqueConstraintViolation(REDBError):
-    """Raised when an insert or update fails due to a duplicate key error."""
-
     def __init__(
         self, *args: object, dup_keys: dict, collection_name: str = ""
     ) -> None:
         if collection_name:
             msg = f"Duplicate key at collection {collection_name} on: {dup_keys}"
         else:
             msg = f"Duplicate key error on: {dup_keys}"
-        super().__init__(msg, *args)
+        super().__init__(msg, *args, collection_name=collection_name)
+        self.dup_keys = [dup_keys]
```

### Comparing `redb-odm-1.2.1/redb/interface/fields.py` & `redb-odm-1.2.2/redb/interface/fields.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/interface/results.py` & `redb-odm-1.2.2/redb/interface/results.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/json_system/client.py` & `redb-odm-1.2.2/redb/json_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/json_system/collection.py` & `redb-odm-1.2.2/redb/json_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/json_system/database.py` & `redb-odm-1.2.2/redb/json_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/migo_system/client.py` & `redb-odm-1.2.2/redb/migo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/migo_system/collection.py` & `redb-odm-1.2.2/redb/migo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/migo_system/database.py` & `redb-odm-1.2.2/redb/migo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/mongo_system/client.py` & `redb-odm-1.2.2/redb/mongo_system/client.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/mongo_system/collection.py` & `redb-odm-1.2.2/redb/mongo_system/collection.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb/mongo_system/database.py` & `redb-odm-1.2.2/redb/mongo_system/database.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/redb_odm.egg-info/SOURCES.txt` & `redb-odm-1.2.2/redb_odm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -40,8 +40,9 @@
 redb_odm.egg-info/top_level.txt
 tests/test_bson_objs.py
 tests/test_hashing.py
 tests/test_i_remember.py
 tests/test_json_client.py
 tests/test_mongo_system.py
 tests/test_return_cls.py
-tests/test_soft_deletion.py
+tests/test_soft_deletion.py
+tests/test_unique_constraints.py
```

### Comparing `redb-odm-1.2.1/setup.py` & `redb-odm-1.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/tests/test_bson_objs.py` & `redb-odm-1.2.2/tests/test_bson_objs.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/tests/test_hashing.py` & `redb-odm-1.2.2/tests/test_hashing.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/tests/test_i_remember.py` & `redb-odm-1.2.2/tests/test_i_remember.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/tests/test_json_client.py` & `redb-odm-1.2.2/tests/test_json_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,35 +13,35 @@
         model="ai",
         text="Some data.",
         vector=[1, 2],
         source_url="www",
     )
 
 
-def test_insert_one(collection_path: Path, embedding: Embedding):
+def test_insert_one(json_client, collection_path: Path, embedding: Embedding):
     # Ignored while we do not have a Mongo instance to run agains
     # with transaction(collection_class=Embedding, config=MongoConfig(database_uri="mongodb://localhost:27017/", default_database="teia"), database_name="another") as embedding:
     #     embedding.insert_one(data=d)
     #     assert not (collection_path / f"{d.id}.json").is_file()
     Embedding.insert_one(embedding)
     assert (collection_path / f"{embedding.id}.json").is_file()
     json_path = collection_path / f"{embedding.id}.json"
     other = read_json(json_path)
     remove_document(collection_path, embedding.id)
     assert other == embedding
 
 
-def test_find_by_id(collection_path: Path, embedding: Embedding):
+def test_find_by_id(json_client, collection_path: Path, embedding: Embedding):
     Embedding.insert_one(embedding)
     found_instance = Embedding.find_one(filter=dict(_id=embedding.id))
     remove_document(collection_path, embedding.id)
     assert found_instance == embedding
 
 
-def test_insert_vectors(collection_path: Path):
+def test_insert_vectors(json_client, collection_path: Path):
     data = dict(
         _id=["a", "b", "c"],
         kb_name=["KB5", "KB6", "KB7"],
         model=["ai", "ai", "ai"],
         text=["Some data 5", "Some data 6", "Some data 7"],
         vector=[[1, 3], [2, 4], [3, 5]],
         source_url=["ww5", "ww6", "ww7"],
@@ -63,56 +63,56 @@
         remove_document(collection_path, other.id)
         # Make both timestamps be the same because they are being generated on object instantiation
         original.created_at = other.created_at
         original.updated_at = other.updated_at
         assert original == other
 
 
-def test_count_documents(collection_path: Path, embedding: Embedding):
+def test_count_documents(json_client, collection_path: Path, embedding: Embedding):
     doc_count = Embedding.count_documents()
     assert doc_count == 0
     Embedding.insert_one(embedding)
     doc_count = Embedding.count_documents()
     try:
         assert doc_count == 1
     finally:
         remove_document(collection_path, embedding.id)
 
 
-def test_replace_one(collection_path: Path, embedding: Embedding):
+def test_replace_one(json_client, collection_path: Path, embedding: Embedding):
     Embedding.insert_one(embedding)
     replacement = Embedding(
         kb_name="KB_REPLACED",
         model="replaced",
         text="Some replaced data.",
         vector=[114, 101, 112, 108, 97, 99, 101, 100],
         source_url="www.replaced",
     )
     Embedding.replace_one(embedding, replacement)
     other = read_json(collection_path / f"{replacement.id}.json")
     remove_document(collection_path, replacement.id)
     assert replacement == other
 
 
-def test_update_one(collection_path: Path, embedding: Embedding):
+def test_update_one(json_client, collection_path: Path, embedding: Embedding):
     Embedding.insert_one(embedding)
     Embedding.update_one(embedding, update={"vector": [1, 2, 3]})
     expected = embedding.dict()
     expected["vector"] = [1, 2, 3]
     other = read_json(collection_path / f"{embedding.id}.json")
     remove_document(collection_path, embedding.id)
     for key, value in expected.items():
         if key == "updated_at":
             continue
 
         assert key in other
         assert value == other[key]
 
 
-def test_delete_one(collection_path: Path, embedding: Embedding):
+def test_delete_one(json_client, collection_path: Path, embedding: Embedding):
     try:
         Embedding.insert_one(embedding)
     except:
         pass
     Embedding.delete_one(embedding)
     with pytest.raises(AssertionError):
         assert (collection_path / f"{embedding.id}.json").is_file()
```

### Comparing `redb-odm-1.2.1/tests/test_mongo_system.py` & `redb-odm-1.2.2/tests/test_mongo_system.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,37 +1,24 @@
 import os
 from pathlib import Path
 
 import dotenv
 import pytest
-from redb.core import RedB
-from redb.interface.configs import MongoConfig
 from redb.interface.errors import DocumentNotFound
 from redb.interface.fields import Direction, SortColumn
 
 from .utils import Embedding, RussianDog
 
 dotenv.load_dotenv()
 
 
 class TestmongoSystem:
-    @pytest.fixture()
-    def client_path(self):
-        return Path("/tmp/")
 
     @pytest.fixture(scope="class", autouse=True)
-    def client(self):
-        RedB.setup(
-            MongoConfig(
-                database_uri=os.environ["MONGODB_URI"],
-            )
-        )
-
-    @pytest.fixture(scope="class", autouse=True)
-    def clean_db(self, client):
+    def clean_db(self):
         RussianDog.delete_many({})
         Embedding.delete_many({})
         yield
         RussianDog.delete_many({})
         Embedding.delete_many({})
 
     def test_insert_one(self):
@@ -42,14 +29,15 @@
             vector=[1, 2],
             source_url="www",
         )
         emb_id = Embedding.insert_one(emb)
         response = Embedding.find_one({"_id": emb_id.inserted_id})
         assert emb == response
 
+
     def test_find_one(self):
         vladmir = RussianDog(
             name="Vladimir",
             age=2,
             breed="Siberian Husky",
             color="Gray",
             is_good_boy=True,
```

### Comparing `redb-odm-1.2.1/tests/test_return_cls.py` & `redb-odm-1.2.2/tests/test_return_cls.py`

 * *Files identical despite different names*

### Comparing `redb-odm-1.2.1/tests/test_soft_deletion.py` & `redb-odm-1.2.2/tests/test_soft_deletion.py`

 * *Files identical despite different names*

