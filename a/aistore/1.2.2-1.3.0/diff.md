# Comparing `tmp/aistore-1.2.2.tar.gz` & `tmp/aistore-1.3.0.tar.gz`

## Comparing `aistore-1.2.2.tar` & `aistore-1.3.0.tar`

### file list

```diff
@@ -1,44 +1,48 @@
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/__init__.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/client.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/common_requirements
--rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/__init__.py
--rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/botocore.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/botocore_patch/botocore_requirements
--rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/README.md
--rw-r--r--   0        0        0      181 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/__init__.py
--rw-r--r--   0        0        0     5827 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/aisio.py
--rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/dataset.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/dev_requirements
--rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/pytorch/utils.py
--rw-r--r--   0        0        0     5511 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/README.md
--rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/__init__.py
--rw-r--r--   0        0        0    26239 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/bucket.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/client.py
--rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/cluster.py
--rw-r--r--   0        0        0     1939 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/const.py
--rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/errors.py
--rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/etl.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/etl_const.py
--rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/etl_templates.py
--rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/job.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/list_object_flag.py
--rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/namespace.py
--rw-r--r--   0        0        0     8204 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object.py
--rw-r--r--   0        0        0     2524 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object_attributes.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object_iterator.py
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/object_reader.py
--rw-r--r--   0        0        0     2457 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/request_client.py
--rw-r--r--   0        0        0    10465 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/types.py
--rw-r--r--   0        0        0     4156 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/utils.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/__init__.py
--rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_collection.py
--rw-r--r--   0        0        0    11271 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_group.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_names.py
--rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_range.py
--rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.2.2/aistore/sdk/multiobj/object_template.py
--rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.2.2/LICENSE
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.2.2/.gitignore
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.2.2/README.md
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 aistore-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     2110 2020-02-02 00:00:00.000000 aistore-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0      183 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/__init__.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/client.py
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/common_requirements
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/version.py
+-rw-r--r--   0        0        0     1462 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/__init__.py
+-rw-r--r--   0        0        0     3531 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/botocore.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/botocore_patch/botocore_requirements
+-rw-r--r--   0        0        0     4349 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/README.md
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/__init__.py
+-rw-r--r--   0        0        0     6978 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/aisio.py
+-rw-r--r--   0        0        0     2002 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/dataset.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/dev_requirements
+-rw-r--r--   0        0        0     2073 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/pytorch/utils.py
+-rw-r--r--   0        0        0     5656 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/README.md
+-rw-r--r--   0        0        0      180 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/__init__.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/ais_source.py
+-rw-r--r--   0        0        0    26977 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/bucket.py
+-rw-r--r--   0        0        0     3140 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/client.py
+-rw-r--r--   0        0        0     5233 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/cluster.py
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/const.py
+-rw-r--r--   0        0        0     3652 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/dsort.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/dsort_types.py
+-rw-r--r--   0        0        0     2521 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/errors.py
+-rw-r--r--   0        0        0     7285 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/etl.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/etl_const.py
+-rw-r--r--   0        0        0     3439 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/etl_templates.py
+-rw-r--r--   0        0        0     9114 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/job.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/list_object_flag.py
+-rw-r--r--   0        0        0      415 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/namespace.py
+-rw-r--r--   0        0        0     9082 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object.py
+-rw-r--r--   0        0        0     2538 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object_attributes.py
+-rw-r--r--   0        0        0     1329 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object_iterator.py
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/object_reader.py
+-rw-r--r--   0        0        0     3302 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/request_client.py
+-rw-r--r--   0        0        0    11137 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/types.py
+-rw-r--r--   0        0        0     4856 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/utils.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/__init__.py
+-rw-r--r--   0        0        0      549 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_collection.py
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_group.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_names.py
+-rw-r--r--   0        0        0     3235 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_range.py
+-rw-r--r--   0        0        0      724 2020-02-02 00:00:00.000000 aistore-1.3.0/aistore/sdk/multiobj/object_template.py
+-rw-r--r--   0        0        0     1075 2020-02-02 00:00:00.000000 aistore-1.3.0/LICENSE
+-rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 aistore-1.3.0/.gitignore
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 aistore-1.3.0/README.md
+-rw-r--r--   0        0        0     1703 2020-02-02 00:00:00.000000 aistore-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2141 2020-02-02 00:00:00.000000 aistore-1.3.0/PKG-INFO
```

### Comparing `aistore-1.2.2/aistore/botocore_patch/README.md` & `aistore-1.3.0/aistore/botocore_patch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/botocore_patch/botocore.py` & `aistore-1.3.0/aistore/botocore_patch/botocore.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/pytorch/README.md` & `aistore-1.3.0/aistore/pytorch/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/pytorch/aisio.py` & `aistore-1.3.0/aistore/pytorch/aisio.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """
 AIS IO Datapipe
 Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 """
 
-from typing import Iterator, Tuple
+from typing import Iterator, Tuple, List
 
+from torch.utils.data.dataset import T_co
 from torchdata.datapipes import functional_datapipe
 
 from torchdata.datapipes.iter import IterDataPipe
 from torchdata.datapipes.utils import StreamWrapper
 
+from aistore.sdk.ais_source import AISSource
+
 try:
     from aistore.sdk import Client
     from aistore.pytorch.utils import parse_url, unparse_url
 
     HAS_AIS = True
 except ImportError:
     HAS_AIS = False
@@ -144,7 +147,33 @@
                 .object(obj_name=obj_name)
                 .get(etl_name=self.etl_name)
                 .raw()
             )
 
     def __len__(self) -> int:
         return len(self.source_datapipe)
+
+
+@functional_datapipe("ais_list_sources")
+class AISSourceLister(IterDataPipe[str]):
+    def __init__(self, ais_sources: List[AISSource], prefix="", etl_name=None):
+        """
+        Iterable DataPipe over the full URLs for each of the provided AIS source object types
+
+        Args:
+            ais_sources (List[AISSource]): List of types implementing the AISSource interface: Bucket, ObjectGroup,
+             Object, etc.
+            prefix (str, optional): Filter results to only include objects with names starting with this prefix
+            etl_name (str, optional): Pre-existing ETL on AIS to apply to all selected objects on the cluster side
+        """
+        _assert_aistore()
+        self.sources = ais_sources
+        self.prefix = prefix
+        self.etl_name = etl_name
+
+    def __getitem__(self, index) -> T_co:
+        raise NotImplementedError
+
+    def __iter__(self) -> Iterator[T_co]:
+        for source in self.sources:
+            for url in source.list_urls(prefix=self.prefix, etl_name=self.etl_name):
+                yield url
```

### Comparing `aistore-1.2.2/aistore/pytorch/dataset.py` & `aistore-1.3.0/aistore/pytorch/dataset.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/pytorch/utils.py` & `aistore-1.3.0/aistore/pytorch/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     """
     samples = []
     for url in urls_list:
         provider, bck_name, path = parse_url(url)
         objects = client.bucket(bck_name=bck_name, provider=provider).list_objects(
             prefix=path
         )
-        for obj_info in objects.get_entries():
+        for obj_info in objects.entries:
             samples.append(
                 {"provider": provider, "bck_name": bck_name, "object": obj_info.name}
             )
     return samples
 
 
 def unparse_url(provider: str, bck_name: str, obj_name: str) -> str:
```

### Comparing `aistore-1.2.2/aistore/sdk/README.md` & `aistore-1.3.0/aistore/sdk/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -97,14 +97,15 @@
 |--|--|
 |[api.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/client.py)|Contains `Client` class, which has methods for making HTTP requests to an AIStore server. Includes factory constructors for `Bucket`, `Cluster`, and `Job` classes.|
 |[cluster.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/cluster.py)|Contains `Cluster` class that represents a cluster bound to a client and contains all cluster-related operations, including checking the cluster's health and retrieving vital cluster information.|
 |[bucket.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/bucket.py)|Contains `Bucket` class that represents a bucket in an AIS cluster and contains all bucket-related operations, including (but not limited to) creating, deleting, evicting, renaming, copying.|
 |[object.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/object.py)|Contains class `Object` that represents an object belonging to a bucket in an AIS cluster, and contains all object-related operations, including (but not limited to) retreiving, adding and deleting objects.|
 |[object_group.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/object_group.py)|Contains class `ObjectGroup`, representing a collection of objects belonging to a bucket in an AIS cluster. Includes all multi-object operations such as deleting, evicting, prefetching, copying, and transforming objects.|
 |[job.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/job.py)|Contains class `Job` and all job-related operations.|
+|[dsort.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/dsort.py)|Contains class `Dsort` and all dsort-related operations.|
 |[etl.py](https://github.com/NVIDIA/aistore/blob/master/python/aistore/sdk/etl.py)|Contains class `Etl` and all ETL-related operations.|
 
 For more information on SDK usage, refer to the [SDK reference documentation](https://aiatscale.org/docs/python_sdk.md) or see the examples [here](https://github.com/NVIDIA/aistore/blob/master/python/examples/sdk/).
 
 
 ## References
```

### Comparing `aistore-1.2.2/aistore/sdk/bucket.py` & `aistore-1.3.0/aistore/sdk/bucket.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 # Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 #
 
 from __future__ import annotations  # pylint: disable=unused-variable
 
 import logging
 from pathlib import Path
-from typing import Dict, List, NewType
+from typing import Dict, List, NewType, Iterable
 import requests
 
+from aistore.sdk.ais_source import AISSource
 from aistore.sdk.etl_const import DEFAULT_ETL_TIMEOUT
 from aistore.sdk.object_iterator import ObjectIterator
 from aistore.sdk.const import (
     ACT_COPY_BCK,
     ACT_CREATE_BCK,
     ACT_DESTROY_BCK,
     ACT_ETL_BCK,
@@ -25,14 +26,16 @@
     HTTP_METHOD_POST,
     PROVIDER_AIS,
     QPARAM_BCK_TO,
     QPARAM_KEEP_REMOTE,
     QPARAM_NAMESPACE,
     QPARAM_PROVIDER,
     URL_PATH_BUCKETS,
+    HEADER_ACCEPT,
+    MSGPACK_CONTENT_TYPE,
 )
 
 from aistore.sdk.errors import (
     InvalidBckProvider,
     ErrBckAlreadyExists,
     ErrBckNotFound,
 )
@@ -53,15 +56,15 @@
 from aistore.sdk.list_object_flag import ListObjectFlag
 from aistore.sdk.utils import validate_directory, get_file_size
 
 Header = NewType("Header", requests.structures.CaseInsensitiveDict)
 
 
 # pylint: disable=unused-variable,too-many-public-methods
-class Bucket:
+class Bucket(AISSource):
     """
     A class representing a bucket that contains user data.
 
     Args:
         client (RequestClient): Client for interfacing with AIS cluster
         name (str): name of bucket
         provider (str, optional): Provider of bucket (one of "ais", "aws", "gcp", ...), defaults to "ais"
@@ -104,14 +107,27 @@
         return self._name
 
     @property
     def namespace(self) -> Namespace:
         """The namespace for this bucket."""
         return self._namespace
 
+    def list_urls(self, prefix: str = "", etl_name: str = None) -> Iterable[str]:
+        """
+            Get an iterator of full URLs to every object in this bucket matching the prefix
+        Args:
+            prefix (str, optional): Limit objects selected by a given string prefix
+            etl_name (str, optional): ETL to include in URLs
+
+        Returns:
+            Iterator of all object URLs matching the prefix
+        """
+        for entry in self.list_objects_iter(prefix=prefix, props="name"):
+            yield self.object(entry.name).get_url(etl_name=etl_name)
+
     def create(self, exist_ok=False):
         """
         Creates a bucket in AIStore cluster.
         Can only create a bucket for AIS provider on localized cluster. Remote cloud buckets do not support creation.
 
         Args:
             exist_ok (bool, optional): Ignore error if the cluster already contains this bucket
@@ -327,18 +343,20 @@
             target=target,
         ).as_dict()
         action = ActionMsg(action=ACT_LIST, value=value).dict()
 
         bucket_list = self.client.request_deserialize(
             HTTP_METHOD_GET,
             path=f"{URL_PATH_BUCKETS}/{ self.name }",
+            headers={HEADER_ACCEPT: MSGPACK_CONTENT_TYPE},
             res_model=BucketList,
             json=action,
             params=self.qparam,
         )
+
         for entry in bucket_list.entries:
             entry.object = self.object(entry.name)
         return bucket_list
 
     def list_objects_iter(
         self,
         prefix: str = "",
@@ -436,16 +454,16 @@
                 page_size=page_size,
                 uuid=uuid,
                 continuation_token=continuation_token,
                 flags=flags,
                 target=target,
             )
             if obj_list:
-                obj_list = obj_list + resp.get_entries()
-            obj_list = obj_list or resp.get_entries()
+                obj_list = obj_list + resp.entries
+            obj_list = obj_list or resp.entries
             if resp.continuation_token == "":
                 break
             continuation_token = resp.continuation_token
             uuid = resp.uuid
         return obj_list
 
     # pylint: disable=too-many-arguments
```

### Comparing `aistore-1.2.2/aistore/sdk/client.py` & `aistore-1.3.0/aistore/sdk/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from __future__ import annotations  # pylint: disable=unused-variable
 
 from aistore.sdk.bucket import Bucket
 from aistore.sdk.const import (
     PROVIDER_AIS,
 )
 from aistore.sdk.cluster import Cluster
+from aistore.sdk.dsort import Dsort
 from aistore.sdk.request_client import RequestClient
 from aistore.sdk.types import Namespace
 from aistore.sdk.job import Job
 from aistore.sdk.etl import Etl
 
 
 # pylint: disable=unused-variable
@@ -82,7 +83,21 @@
         Args:
             etl_name (str): Name of the ETL
 
         Returns:
             The ETL object created.
         """
         return Etl(client=self._request_client, name=etl_name)
+
+    def dsort(self, dsort_id: str = ""):
+        """
+        Factory constructor for dSort object.
+        Contains APIs related to AIStore dSort operations.
+        Does not make any HTTP request, only instantiates a dSort object.
+
+        Args:
+            dsort_id: ID of the dSort job
+
+        Returns:
+            dSort object created
+        """
+        return Dsort(client=self._request_client, dsort_id=dsort_id)
```

### Comparing `aistore-1.2.2/aistore/sdk/cluster.py` & `aistore-1.3.0/aistore/sdk/cluster.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/const.py` & `aistore-1.3.0/aistore/sdk/const.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,41 @@
 #
 # Copyright (c) 2021-2023, NVIDIA CORPORATION. All rights reserved.
 #
 
+HEADERS_KW = "headers"
+# Standard Header Keys
+HEADER_ACCEPT = "Accept"
+HEADER_USER_AGENT = "User-Agent"
+HEADER_CONTENT_TYPE = "Content-Type"
+HEADER_CONTENT_LENGTH = "Content-Length"
+# Standard Header Values
+USER_AGENT_BASE = "ais/python"
+JSON_CONTENT_TYPE = "application/json"
+MSGPACK_CONTENT_TYPE = "application/msgpack"
+# AIS Headers
+AIS_CHECKSUM_TYPE = "ais-checksum-type"
+AIS_CHECKSUM_VALUE = "ais-checksum-value"
+AIS_ACCESS_TIME = "ais-atime"
+AIS_VERSION = "ais-version"
+AIS_CUSTOM_MD = "ais-custom-md"
+
+
 # URL Params
 # See api/apc/query.go
 QPARAM_WHAT = "what"
 QPARAM_ETL_NAME = "etl_name"
 QPARAM_PROVIDER = "provider"
 QPARAM_BCK_TO = "bck_to"
 QPARAM_KEEP_REMOTE = "keep_bck_md"
 QPARAM_ARCHPATH = "archpath"
 QPARAM_FORCE = "frc"
 QPARAM_PRIMARY_READY_REB = "prr"
 QPARAM_NAMESPACE = "namespace"
+DSORT_UUID = "uuid"
 
 # URL Param values
 # See api/apc/query.go
 WHAT_SMAP = "smap"
 WHAT_ONE_XACT_STATUS = "status"
 WHAT_ALL_XACT_STATUS = "status_all"
 WHAT_ALL_RUNNING_STATUS = "running_all"
@@ -25,14 +44,16 @@
 # URL paths
 URL_PATH_CLUSTER = "cluster"
 URL_PATH_BUCKETS = "buckets"
 URL_PATH_OBJECTS = "objects"
 URL_PATH_HEALTH = "health"
 URL_PATH_DAEMON = "daemon"
 URL_PATH_ETL = "etl"
+URL_PATH_DSORT = "sort"
+DSORT_ABORT = "abort"
 
 # Bucket providers
 # See api/apc/provider.go
 PROVIDER_AIS = "ais"
 PROVIDER_AMAZON = "aws"
 PROVIDER_AZURE = "azure"
 PROVIDER_GOOGLE = "gcp"
@@ -62,21 +83,14 @@
 ACT_PREFETCH_OBJECTS = "prefetch-listrange"
 ACT_COPY_OBJECTS = "copy-listrange"
 ACT_TRANSFORM_OBJECTS = "etl-listrange"
 ACT_ARCHIVE_OBJECTS = "archive"
 # Job actions
 ACT_START = "start"
 
-# Headers
-CONTENT_LENGTH = "content-length"
-AIS_CHECKSUM_TYPE = "ais-checksum-type"
-AIS_CHECKSUM_VALUE = "ais-checksum-value"
-AIS_ACCESS_TIME = "ais-atime"
-AIS_VERSION = "ais-version"
-AIS_CUSTOM_MD = "ais-custom-md"
-
 # Defaults
 DEFAULT_CHUNK_SIZE = 32768
 DEFAULT_JOB_WAIT_TIMEOUT = 300
+DEFAULT_DSORT_WAIT_TIMEOUT = 300
 
 # ENCODING
 UTF_ENCODING = "utf-8"
```

### Comparing `aistore-1.2.2/aistore/sdk/errors.py` & `aistore-1.3.0/aistore/sdk/errors.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/etl.py` & `aistore-1.3.0/aistore/sdk/etl.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/etl_const.py` & `aistore-1.3.0/aistore/sdk/etl_const.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/etl_templates.py` & `aistore-1.3.0/aistore/sdk/etl_templates.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/job.py` & `aistore-1.3.0/aistore/sdk/job.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/list_object_flag.py` & `aistore-1.3.0/aistore/sdk/list_object_flag.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/object.py` & `aistore-1.3.0/aistore/sdk/object.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #
 # Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 #
 from io import BufferedWriter
-from typing import NewType
+from typing import NewType, Iterable
+
 import requests
 
+from aistore.sdk.ais_source import AISSource
 from aistore.sdk.const import (
     DEFAULT_CHUNK_SIZE,
     HTTP_METHOD_DELETE,
     HTTP_METHOD_GET,
     HTTP_METHOD_HEAD,
     HTTP_METHOD_PUT,
     QPARAM_ARCHPATH,
@@ -22,15 +24,15 @@
 from aistore.sdk.types import ActionMsg, PromoteAPIArgs
 from aistore.sdk.utils import read_file_bytes, validate_file
 
 Header = NewType("Header", requests.structures.CaseInsensitiveDict)
 
 
 # pylint: disable=consider-using-with,unused-variable
-class Object:
+class Object(AISSource):
     """
     A class representing an object of a bucket bound to a client.
 
     Args:
         bucket (Bucket): Bucket to which this object belongs
         name (str): name of object
 
@@ -38,25 +40,29 @@
 
     def __init__(self, bucket: "Bucket", name: str):
         self._bucket = bucket
         self._client = bucket.client
         self._bck_name = bucket.name
         self._qparams = bucket.qparam
         self._name = name
+        self._object_path = f"{URL_PATH_OBJECTS}/{ self._bck_name}/{ self.name }"
 
     @property
     def bucket(self):
         """Bucket containing this object"""
         return self._bucket
 
     @property
     def name(self):
         """Name of this object"""
         return self._name
 
+    def list_urls(self, prefix: str = "", etl_name: str = None) -> Iterable[str]:
+        yield self.get_url(etl_name=etl_name)
+
     def head(self) -> Header:
         """
         Requests object properties.
 
         Returns:
             Response header with the object properties.
 
@@ -65,15 +71,15 @@
             requests.ConnectionError: Connection error
             requests.ConnectionTimeout: Timed out connecting to AIStore
             requests.ReadTimeout: Timed out waiting response from AIStore
             requests.exceptions.HTTPError(404): The object does not exist
         """
         return self._client.request(
             HTTP_METHOD_HEAD,
-            path=f"{URL_PATH_OBJECTS}/{ self._bck_name}/{ self.name }",
+            path=self._object_path,
             params=self._qparams,
         ).headers
 
     def get(
         self,
         archpath: str = "",
         chunk_size: int = DEFAULT_CHUNK_SIZE,
@@ -102,27 +108,47 @@
         """
         params = self._qparams.copy()
         params[QPARAM_ARCHPATH] = archpath
         if etl_name:
             params[QPARAM_ETL_NAME] = etl_name
         resp = self._client.request(
             HTTP_METHOD_GET,
-            path=f"{URL_PATH_OBJECTS}/{ self._bck_name }/{ self.name }",
+            path=self._object_path,
             params=params,
             stream=True,
         )
         obj_reader = ObjectReader(
             stream=resp,
             response_headers=resp.headers,
             chunk_size=chunk_size,
         )
         if writer:
             writer.writelines(obj_reader)
         return obj_reader
 
+    def get_url(self, archpath: str = "", etl_name: str = None):
+        """
+        Get the full url to the object including base url and any query parameters
+
+        Args:
+            archpath (str, optional): If the object is an archive, use `archpath` to extract a single file
+                from the archive
+            etl_name (str, optional): Transforms an object based on ETL with etl_name
+
+        Returns:
+            Full URL to get object
+
+        """
+        params = self._qparams.copy()
+        if archpath:
+            params[QPARAM_ARCHPATH] = archpath
+        if etl_name:
+            params[QPARAM_ETL_NAME] = etl_name
+        return self._client.get_full_url(self._object_path, params)
+
     def put_content(self, content: bytes) -> Header:
         """
         Puts bytes as an object to a bucket in AIS storage.
 
         Args:
             content (bytes): Bytes to put as an object.
 
@@ -222,10 +248,10 @@
             requests.ConnectionError: Connection error
             requests.ConnectionTimeout: Timed out connecting to AIStore
             requests.ReadTimeout: Timed out waiting response from AIStore
             requests.exceptions.HTTPError(404): The object does not exist
         """
         self._client.request(
             HTTP_METHOD_DELETE,
-            path=f"{URL_PATH_OBJECTS}/{ self._bck_name }/{ self.name }",
+            path=self._object_path,
             params=self._qparams,
         )
```

### Comparing `aistore-1.2.2/aistore/sdk/object_attributes.py` & `aistore-1.3.0/aistore/sdk/object_attributes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from typing import Dict
 
 from requests.structures import CaseInsensitiveDict
 
 from aistore.sdk.const import (
-    CONTENT_LENGTH,
+    HEADER_CONTENT_LENGTH,
     AIS_CHECKSUM_TYPE,
     AIS_CHECKSUM_VALUE,
     AIS_ACCESS_TIME,
     AIS_VERSION,
     AIS_CUSTOM_MD,
 )
 
@@ -25,15 +25,15 @@
         self.response_headers = response_headers
 
     @property
     def size(self) -> int:
         """
         Size of object content
         """
-        return int(self.response_headers.get(CONTENT_LENGTH, 0))
+        return int(self.response_headers.get(HEADER_CONTENT_LENGTH, 0))
 
     @property
     def checksum_type(self) -> str:
         """
         Type of checksum, e.g. xxhash or md5
         """
         return self.response_headers.get(AIS_CHECKSUM_TYPE, "")
```

### Comparing `aistore-1.2.2/aistore/sdk/object_iterator.py` & `aistore-1.3.0/aistore/sdk/object_iterator.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,14 @@
     def __next__(self) -> BucketEntry:
         # Iterator is exhausted.
         if len(self._fetched) == 0 and self._token == "" and self._uuid != "":
             raise StopIteration
         # Read the next page of objects.
         if len(self._fetched) == 0:
             resp = self._list_objects(uuid=self._uuid, token=self._token)
-            self._fetched = resp.get_entries()
+            self._fetched = resp.entries
             self._uuid = resp.uuid
             self._token = resp.continuation_token
             # Empty page and token mean no more objects left.
             if len(self._fetched) == 0 and self._token == "":
                 raise StopIteration
         return self._fetched.pop(0)
```

### Comparing `aistore-1.2.2/aistore/sdk/object_reader.py` & `aistore-1.3.0/aistore/sdk/object_reader.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/request_client.py` & `aistore-1.3.0/aistore/sdk/request_client.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 #
 # Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 #
+from urllib.parse import urljoin, urlencode
+from typing import TypeVar, Type, Any, Dict
 
-from urllib.parse import urljoin
-from typing import TypeVar, Type
-
-from pydantic.tools import parse_raw_as
 import requests
 
-from aistore.sdk.utils import handle_errors
+from aistore.sdk.const import (
+    JSON_CONTENT_TYPE,
+    HEADER_USER_AGENT,
+    USER_AGENT_BASE,
+    HEADER_CONTENT_TYPE,
+    HEADERS_KW,
+)
+from aistore.sdk.utils import handle_errors, decode_response
+from aistore.version import __version__ as sdk_version
 
 T = TypeVar("T")
 
 
 # pylint: disable=unused-variable
 class RequestClient:
     """
@@ -52,34 +58,55 @@
         self, method: str, path: str, res_model: Type[T], **kwargs
     ) -> T:
         """
         Make a request to the AIS cluster and deserialize the response to a defined type
         Args:
             method (str): HTTP method, e.g. POST, GET, PUT, DELETE
             path (str): URL path to call
-            res_model Type[T]: Resulting type to which the response should be deserialized
+            res_model (Type[T]): Resulting type to which the response should be deserialized
             **kwargs (optional): Optional keyword arguments to pass with the call to request
 
         Returns:
             Parsed result of the call to the API, as res_model
         """
         resp = self.request(method, path, **kwargs)
-        return parse_raw_as(res_model, resp.text)
+        return decode_response(res_model, resp)
 
     def request(self, method: str, path: str, **kwargs) -> requests.Response:
         """
         Make a request to the AIS cluster
         Args:
             method (str): HTTP method, e.g. POST, GET, PUT, DELETE
             path (str): URL path to call
             **kwargs (optional): Optional keyword arguments to pass with the call to request
 
         Returns:
             Raw response from the API
         """
         url = f"{self._base_url}/{path.lstrip('/')}"
+        if HEADERS_KW not in kwargs:
+            kwargs[HEADERS_KW] = {}
+        headers = kwargs.get(HEADERS_KW, {})
+        headers[HEADER_CONTENT_TYPE] = JSON_CONTENT_TYPE
+        headers[HEADER_USER_AGENT] = f"{USER_AGENT_BASE}/{sdk_version}"
         resp = self._session.request(
-            method, url, headers={"Accept": "application/json"}, **kwargs
+            method,
+            url,
+            **kwargs,
         )
         if resp.status_code < 200 or resp.status_code >= 300:
             handle_errors(resp)
         return resp
+
+    def get_full_url(self, path: str, params: Dict[str, Any]):
+        """
+        Get the full URL to the path on the cluster with the parameters given
+
+        Args:
+            path: Path on the cluster
+            params: Query parameters to include
+
+        Returns:
+            URL including cluster base url and parameters
+
+        """
+        return f"{self._base_url}/{path.lstrip('/')}?{urlencode(params)}"
```

### Comparing `aistore-1.2.2/aistore/sdk/types.py` & `aistore-1.3.0/aistore/sdk/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 #
 
 from __future__ import annotations  # pylint: disable=unused-variable
 import base64
 
 from typing import Any, Mapping, List, Optional, Dict
 
+import msgspec
 from pydantic import BaseModel, validator
 
 from aistore.sdk.namespace import Namespace
 from aistore.sdk.const import PROVIDER_AIS
 from aistore.sdk.list_object_flag import ListObjectFlag
 
 
@@ -59,56 +60,101 @@
     pmap: Mapping[str, Snode]
     proxy_si: Snode
     version: int = 0
     uuid: str = ""
     creation_time: str = ""
 
 
-class BucketEntry(BaseModel):
+class BucketEntry(msgspec.Struct):
     """
     Represents a single entry in a bucket -- an object
+    See cmn/objlist.go/LsoEntry
     """
 
-    name: str
-    size: int = 0
-    checksum: str = ""
-    atime: str = ""
-    version: str = ""
-    target_url: str = ""
-    copies: int = 0
-    flags: int = 0
-    object: "Object" = None
+    n: str
+    cs: str = ""
+    a: str = ""
+    v: str = ""
+    t: str = ""
+    s: int = 0
+    c: int = 0
+    f: int = 0
+    object: Any = None
+
+    @property
+    def name(self):
+        return self.n
+
+    @property
+    def checksum(self):
+        return self.cs
+
+    @property
+    def atime(self):
+        return self.a
+
+    @property
+    def version(self):
+        return self.v
+
+    @property
+    def location(self):
+        return self.t
+
+    @property
+    def size(self):
+        return self.s
+
+    @property
+    def copies(self):
+        return self.c
+
+    @property
+    def flags(self):
+        return self.f
 
     def is_cached(self):
         return (self.flags & (1 << 6)) != 0
 
     def is_ok(self):
         return (self.flags & ((1 << 5) - 1)) == 0
 
 
-class BucketList(BaseModel):
+class BucketList(msgspec.Struct):
     """
     Represents the response when getting a list of bucket items, containing a list of BucketEntry objects
     """
 
-    uuid: str
-    entries: Optional[List[BucketEntry]] = []
-    continuation_token: str
-    flags: int
+    UUID: str
+    ContinuationToken: str
+    Flags: int
+    Entries: List[BucketEntry] = None
+
+    @property
+    def uuid(self):
+        return self.UUID
+
+    @property
+    def continuation_token(self):
+        return self.ContinuationToken
+
+    @property
+    def flags(self):
+        return self.Flags
+
+    @property
+    def entries(self):
+        return [] if self.Entries is None else self.Entries
 
     def get_entries(self):
+        """
+        Deprecated -- use entries property
+        """
         return self.entries
 
-    # pylint: disable=no-self-argument
-    @validator("entries")
-    def set_entries(cls, entries):
-        if entries is None:
-            entries = []
-        return entries
-
 
 class BucketModel(BaseModel):
     """
     Represents the response from the API containing bucket info
     """
 
     name: str
```

### Comparing `aistore-1.2.2/aistore/sdk/utils.py` & `aistore-1.3.0/aistore/sdk/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 #
 # Copyright (c) 2022-2023, NVIDIA CORPORATION. All rights reserved.
 #
 from pathlib import Path
-from typing import Iterator
+from typing import Iterator, Type, TypeVar
 
 import braceexpand
 import humanize
+
+from msgspec import msgpack
 import pydantic.tools
 import requests
-from pydantic import BaseModel
+from pydantic import BaseModel, parse_raw_as
+from requests import Response
 
-from aistore.sdk.const import UTF_ENCODING
+from aistore.sdk.const import UTF_ENCODING, HEADER_CONTENT_TYPE, MSGPACK_CONTENT_TYPE
 from aistore.sdk.errors import (
     AISError,
     ErrBckNotFound,
     ErrRemoteBckNotFound,
     ErrBckAlreadyExists,
     ErrETLAlreadyExists,
 )
 
+T = TypeVar("T")
+
 
 class HttpError(BaseModel):
     """
     Represents the errors returned by the API
     """
 
     status: int
@@ -152,7 +157,25 @@
     Returns:
         Iterator of brace expansion output
 
     """
     # pylint: disable = fixme
     # TODO Build custom expansion to validate consistent with cmn/cos/template.go TemplateRange
     return braceexpand.braceexpand(template)
+
+
+def decode_response(
+    res_model: Type[T],
+    resp: Response,
+) -> T:
+    """
+    Parse response content from the cluster into a Python class,
+     decoding with msgpack depending on content type in header
+
+    Args:
+        res_model (Type[T]): Resulting type to which the response should be deserialized
+        resp (Response): Response from the AIS cluster
+
+    """
+    if resp.headers.get(HEADER_CONTENT_TYPE) == MSGPACK_CONTENT_TYPE:
+        return msgpack.decode(resp.content, type=res_model)
+    return parse_raw_as(res_model, resp.text)
```

### Comparing `aistore-1.2.2/aistore/sdk/multiobj/object_collection.py` & `aistore-1.3.0/aistore/sdk/multiobj/object_collection.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/multiobj/object_group.py` & `aistore-1.3.0/aistore/sdk/multiobj/object_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #
 # Copyright (c) 2023, NVIDIA CORPORATION. All rights reserved.
 #
 import logging
-from typing import List
+from typing import List, Iterable
 
+from aistore.sdk.ais_source import AISSource
 from aistore.sdk.const import (
     HTTP_METHOD_DELETE,
     HTTP_METHOD_POST,
     HTTP_METHOD_PUT,
     ACT_DELETE_OBJECTS,
     ACT_PREFETCH_OBJECTS,
     ACT_EVICT_OBJECTS,
@@ -25,29 +26,29 @@
     TransformBckMsg,
     TCBckMsg,
     ArchiveMultiObj,
 )
 
 
 # pylint: disable=unused-variable
-class ObjectGroup:
+class ObjectGroup(AISSource):
     """
     A class representing multiple objects within the same bucket. Only one of obj_names, obj_range, or obj_template
      should be provided.
 
     Args:
         bck (Bucket): Bucket the objects belong to
         obj_names (list[str], optional): List of object names to include in this collection
         obj_range (ObjectRange, optional): Range defining which object names in the bucket should be included
         obj_template (str, optional): String argument to pass as template value directly to api
     """
 
     def __init__(
         self,
-        bck,
+        bck: "Bucket",
         obj_names: list = None,
         obj_range: ObjectRange = None,
         obj_template: str = None,
     ):
         self.bck = bck
         num_args = sum(
             1 if x is not None else 0 for x in [obj_names, obj_range, obj_template]
@@ -62,14 +63,27 @@
         if obj_range:
             self._obj_collection = obj_range
         elif obj_names:
             self._obj_collection = ObjectNames(obj_names)
         else:
             self._obj_collection = ObjectTemplate(obj_template)
 
+    def list_urls(self, prefix: str = "", etl_name: str = None) -> Iterable[str]:
+        """
+            Get an iterator of the full URL for every object in this group
+        Args:
+            prefix (str, optional): Limit objects selected by a given string prefix
+            etl_name (str, optional): ETL to include in URLs
+
+        Returns:
+            Iterator of all object URLs in the group
+        """
+        for obj_name in self._obj_collection:
+            yield self.bck.object(obj_name).get_url(etl_name=etl_name)
+
     def delete(self):
         """
         Deletes a list or range of objects in a bucket
 
         Raises:
             aistore.sdk.errors.AISError: All other types of errors with AIStore
             requests.ConnectionError: Connection error
```

### Comparing `aistore-1.2.2/aistore/sdk/multiobj/object_names.py` & `aistore-1.3.0/aistore/sdk/multiobj/object_names.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/multiobj/object_range.py` & `aistore-1.3.0/aistore/sdk/multiobj/object_range.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/aistore/sdk/multiobj/object_template.py` & `aistore-1.3.0/aistore/sdk/multiobj/object_template.py`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/LICENSE` & `aistore-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/.gitignore` & `aistore-1.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/README.md` & `aistore-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `aistore-1.2.2/pyproject.toml` & `aistore-1.3.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -9,17 +9,20 @@
 "../LICENSE" = "LICENSE"
 
 [tool.pytest.ini_options]
 markers = [
     "etl: marks tests as using etl and therefore requiring k8s cluster",
 ]
 
+[tool.hatch.version]
+path = "aistore/version.py"
+
 [project]
 name = "aistore"
-version = "1.2.2"
+dynamic = ["version"]
 authors = [
   { name="AIStore Team", email="ais@exchange.nvidia.com" },
 ]
 description = "A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {text = "MIT License"}
@@ -35,15 +38,16 @@
 
 dependencies = [
     "requests",
     "packaging",
     "pydantic==1.9.0",
     "cloudpickle==2.2.0",
     "humanize>=4.6.0",
-    "braceexpand>=0.1.7"
+    "braceexpand>=0.1.7",
+    "msgspec>=0.15.1"
 ]
 
 keywords = [
     "AIStore",
     "Artificial Intelligence",
     "Object Storage",
     "Deep Learning",
```

### Comparing `aistore-1.2.2/PKG-INFO` & `aistore-1.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aistore
-Version: 1.2.2
+Version: 1.3.0
 Summary: A (growing) set of client-side APIs to access and utilize clusters, buckets, and objects on AIStore.
 Project-URL: Homepage, https://aiatscale.org
 Project-URL: Download, https://github.com/NVIDIA/aistore/tags
 Project-URL: Documentation, https://aiatscale.org/docs/
 Project-URL: Release notes, https://github.com/NVIDIA/aistore/releases/
 Project-URL: Source, https://github.com/NVIDIA/aistore/
 Author-email: AIStore Team <ais@exchange.nvidia.com>
@@ -17,14 +17,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: braceexpand>=0.1.7
 Requires-Dist: cloudpickle==2.2.0
 Requires-Dist: humanize>=4.6.0
+Requires-Dist: msgspec>=0.15.1
 Requires-Dist: packaging
 Requires-Dist: pydantic==1.9.0
 Requires-Dist: requests
 Provides-Extra: botocore
 Requires-Dist: wrapt; extra == 'botocore'
 Provides-Extra: pytorch
 Requires-Dist: torch; extra == 'pytorch'
```

