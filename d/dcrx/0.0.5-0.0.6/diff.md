# Comparing `tmp/dcrx-0.0.5.tar.gz` & `tmp/dcrx-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcrx-0.0.5.tar", last modified: Wed Jun  7 19:02:44 2023, max compression
+gzip compressed data, was "dcrx-0.0.6.tar", last modified: Thu Jun  8 01:32:36 2023, max compression
```

## Comparing `dcrx-0.0.5.tar` & `dcrx-0.0.6.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.431843 dcrx-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-07 19:02:41.000000 dcrx-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-07 19:02:44.431843 dcrx-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-07 19:02:41.000000 dcrx-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx/
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8316 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/image.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx/layers/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      511 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/arg.py
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/cmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/copy.py
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/expose.py
--rw-r--r--   0 runner    (1001) docker     (123)      500 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/healthcheck.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/label.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx/layers/mount_types/
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/bind_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/cache_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/secret_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/ssh_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/mount_types/tmpfs_mount.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/run.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/user.py
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/volume.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/layers/workdir.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.431843 dcrx-0.0.5/dcrx/memory_file/
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/memory_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-06-07 19:02:41.000000 dcrx-0.0.5/dcrx/memory_file/memory_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:02:44.427842 dcrx-0.0.5/dcrx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-07 19:02:44.000000 dcrx-0.0.5/dcrx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:02:44.431843 dcrx-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-07 19:02:41.000000 dcrx-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:32:36.711921 dcrx-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-08 01:32:33.000000 dcrx-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-08 01:32:36.711921 dcrx-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-06-08 01:32:33.000000 dcrx-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:32:36.707921 dcrx-0.0.6/dcrx/
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8639 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/image.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:32:36.711921 dcrx-0.0.6/dcrx/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/arg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/cmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/copy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      410 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/expose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/healthcheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/label.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:32:36.711921 dcrx-0.0.6/dcrx/layers/mount_types/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/mount_types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/mount_types/bind_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/mount_types/cache_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/mount_types/secret_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/mount_types/ssh_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/mount_types/tmpfs_mount.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/layers/workdir.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:32:36.711921 dcrx-0.0.6/dcrx/memory_file/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/memory_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-06-08 01:32:33.000000 dcrx-0.0.6/dcrx/memory_file/memory_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 01:32:36.707921 dcrx-0.0.6/dcrx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4990 2023-06-08 01:32:36.000000 dcrx-0.0.6/dcrx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-08 01:32:36.000000 dcrx-0.0.6/dcrx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 01:32:36.000000 dcrx-0.0.6/dcrx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-08 01:32:36.000000 dcrx-0.0.6/dcrx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-08 01:32:36.000000 dcrx-0.0.6/dcrx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 01:32:36.711921 dcrx-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-06-08 01:32:33.000000 dcrx-0.0.6/setup.py
```

### Comparing `dcrx-0.0.5/LICENSE` & `dcrx-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/PKG-INFO` & `dcrx-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for typesafe, programmatic generation of Docker images via SQL-builder like API.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-0.0.5/README.md` & `dcrx-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/dcrx/image.py` & `dcrx-0.0.6/dcrx/image.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-import io
+import os
 import tarfile
 import pathlib
 from typing import (
     List, 
     Union, 
     Optional,
     Callable,
@@ -38,19 +38,26 @@
 
 class Image:
 
     def __init__(
         self,
         name: str,
         tag: str="latest",
-        registry: str=None
+        registry: str=None,
+        filename: str=None
     ) -> None:
         self.name = name
         self.tag = tag
         self.files: List[str] = []
+
+        if filename is None:
+            stub = name.replace('/', '.')
+            filename = f'Dockerfile.{stub}'
+
+        self.filename = filename
         
         self.registry = registry
         self.layers: List[
             Union[
                 Arg,
                 Cmd,
                 Copy,
@@ -89,18 +96,22 @@
         return f'{self.name}:{self.tag}'
 
     def to_string(self) -> str:
         return '\n\n'.join([
             layer.to_string() for layer in self.layers
         ])
     
-    def to_context(self) -> io.BytesIO:
+    def to_context(self) -> MemoryFile:
+
+        if os.path.exists(self.filename) is False:
+            self.to_file()
 
         image_file = MemoryFile(
-            self.to_string().encode()
+            self.to_string().encode(),
+            name=self.filename
         )
 
         image_file.seek(0)
 
         tar_file_number = image_file.file_number + 1
 
         tar_file = MemoryFile(
@@ -110,16 +121,15 @@
 
         context = tarfile.open(
             fileobj=tar_file, 
             mode='w'
         )
 
         image_file_info = context.gettarinfo(
-            fileobj=image_file, 
-            arcname='Dockefile'
+            fileobj=image_file
         )
 
         context.addfile(
             image_file_info, 
             image_file
         )
 
@@ -135,24 +145,25 @@
                 context.addfile(info, context_file)
 
         context.close()
         tar_file.seek(0)
 
         return tar_file
     
-    def to_file(
-        self,
-        path: str
-    ):
-        self.files.append(path)
+    def to_file(self):
+        self.files.append(self.filename)
 
-        with open(path, 'w') as dockerfile:
+        with open(self.filename, 'w') as dockerfile:
             dockerfile.write(
                 self.to_string()
             )
+
+    def clear(self):
+        os.remove(self.filename)
+        self.layers.clear()
     
     def add(
         self,
         source: str,
         destination: str,
         user_id: Optional[str]=None,
         group_id: Optional[str]=None,
```

### Comparing `dcrx-0.0.5/dcrx/layers/add.py` & `dcrx-0.0.6/dcrx/layers/add.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 from pydantic import (
     BaseModel,
     StrictStr,
     StrictBool,
     constr
 )
 
-from typing import Union, Optional
+from typing import Literal, Optional
 
 class Add(BaseModel):
+    layer_type: Literal["add"]="add"
     source: StrictStr
     destination: StrictStr
     user_id: Optional[StrictStr]
     group_id: Optional[StrictStr]
     permissions: Optional[constr(max_length=4, regex='^[0-9]*$')]
     checksum: Optional[StrictStr]
     link: StrictBool=False
```

### Comparing `dcrx-0.0.5/dcrx/layers/copy.py` & `dcrx-0.0.6/dcrx/layers/copy.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,18 +3,19 @@
     FilePath,
     DirectoryPath,
     StrictStr,
     StrictBool,
     constr
 )
 
-from typing import Union, Optional
+from typing import Union, Optional, Literal
 
 
 class Copy(BaseModel):
+    layer_type: Literal["copy"]="copy"
     source: Union[FilePath, DirectoryPath]
     destination: StrictStr
     user_id: Optional[StrictStr]
     group_id: Optional[StrictStr]
     permissions: Optional[constr(max_length=4, regex='^[0-9]*$')]
     from_source: Optional[StrictStr]
     link: StrictBool=False
```

### Comparing `dcrx-0.0.5/dcrx/layers/mount_types/bind_mount.py` & `dcrx-0.0.6/dcrx/layers/mount_types/bind_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/dcrx/layers/mount_types/cache_mount.py` & `dcrx-0.0.6/dcrx/layers/mount_types/cache_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/dcrx/layers/mount_types/secret_mount.py` & `dcrx-0.0.6/dcrx/layers/mount_types/secret_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/dcrx/layers/mount_types/ssh_mount.py` & `dcrx-0.0.6/dcrx/layers/mount_types/ssh_mount.py`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/dcrx/layers/run.py` & `dcrx-0.0.6/dcrx/layers/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     SecretMount,
     SSHMount,
     TMPFSMount
 )
 
 
 class Run(BaseModel):
+    layer_type: Literal["run"]="run"
     command: StrictStr
     mount: Optional[Union[BindMount, CacheMount, SecretMount, SSHMount, TMPFSMount]]
     network: Optional[Literal["default", "host", "none"]]
     security: Optional[Literal["insecure", "sandbox"]]
 
     def to_string(self) -> str:
```

### Comparing `dcrx-0.0.5/dcrx.egg-info/PKG-INFO` & `dcrx-0.0.6/dcrx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dcrx
-Version: 0.0.5
+Version: 0.0.6
 Summary: A library for typesafe, programmatic generation of Docker images via SQL-builder like API.
 Home-page: https://github.com/scorbettUM/dcrx
 Author: Sean Corbett
 Author-email: sean.corbett@umontana.edu
 Keywords: pypi,cicd,python,setup,docker,infra,devops
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dcrx-0.0.5/dcrx.egg-info/SOURCES.txt` & `dcrx-0.0.6/dcrx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dcrx-0.0.5/setup.py` & `dcrx-0.0.6/setup.py`

 * *Files identical despite different names*

