# Comparing `tmp/eotdl-cli-2023.5.9.post4.tar.gz` & `tmp/eotdl-cli-2023.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl-cli-2023.5.9.post4.tar", max compression
+gzip compressed data, was "eotdl-cli-2023.6.8.tar", max compression
```

## Comparing `eotdl-cli-2023.5.9.post4.tar` & `eotdl-cli-2023.6.8.tar`

### file list

```diff
@@ -1,29 +1,31 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post4/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.5.9.post4/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post4/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     2125 2023-05-09 15:21:02.804320 eotdl-cli-2023.5.9.post4/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl-cli-2023.5.9.post4/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     7709 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      932 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      820 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
--rw-r--r--   0        0        0      837 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
--rw-r--r--   0        0        0      421 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0      148 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1842 2023-05-09 15:05:12.940722 eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      604 2023-05-09 15:31:07.174517 eotdl-cli-2023.5.9.post4/pyproject.toml
--rw-r--r--   0        0        0     1041 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post4/setup.py
--rw-r--r--   0        0        0      699 1970-01-01 00:00:00.000000 eotdl-cli-2023.5.9.post4/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl-cli-2023.6.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl-cli-2023.6.8/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl-cli-2023.6.8/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1598 2023-05-23 12:10:19.220001 eotdl-cli-2023.6.8/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      367 2023-05-23 10:31:57.663189 eotdl-cli-2023.6.8/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl-cli-2023.6.8/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     9594 2023-06-08 14:47:32.367190 eotdl-cli-2023.6.8/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl-cli-2023.6.8/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      763 2023-05-23 12:06:36.471211 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      932 2023-05-09 15:05:12.940722 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0     1375 2023-06-08 14:44:02.846956 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py
+-rw-r--r--   0        0        0      927 2023-05-16 10:10:52.296818 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py
+-rw-r--r--   0        0        0      421 2023-05-09 15:05:12.940722 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0      940 2023-05-23 11:36:06.764258 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/UpdateDataset.py
+-rw-r--r--   0        0        0      168 2023-05-16 10:10:52.296818 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     2168 2023-05-23 12:06:38.803219 eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      235 2023-05-23 11:05:01.073388 eotdl-cli-2023.6.8/eotdl_cli/src/utils.py
+-rw-r--r--   0        0        0      601 2023-06-08 15:06:34.445545 eotdl-cli-2023.6.8/pyproject.toml
+-rw-r--r--   0        0        0     1035 1970-01-01 00:00:00.000000 eotdl-cli-2023.6.8/setup.py
+-rw-r--r--   0        0        0      693 1970-01-01 00:00:00.000000 eotdl-cli-2023.6.8/PKG-INFO
```

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/commands/auth.py` & `eotdl-cli-2023.6.8/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/commands/datasets.py` & `eotdl-cli-2023.6.8/eotdl_cli/commands/datasets.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import typer
 from src.usecases.datasets import (
     retrieve_datasets,
     download_dataset,
-    # ingest_dataset,
+    update_dataset,
     ingest_large_dataset,
     ingest_large_dataset_parallel,
 )
 from src.usecases.auth import auth
 from typing import Optional
 
 app = typer.Typer()
@@ -27,65 +27,55 @@
     Download a dataset
 
     name: Name of the dataset
     path: Path to download the dataset to
     """
     try:
         user = auth()
-        dst_path = download_dataset(name, path, user)
+        dst_path = download_dataset(name, path, user, typer.echo)
         typer.echo(f"Dataset {name} downloaded to {dst_path}")
     except Exception as e:
         typer.echo(e)
 
 
-# @app.command()
-# def ingest(path: str):
-#     """
-#     Ingest a dataset
-
-#     path: Path to dataset to ingest
-#     """
-#     try:
-#         user = auth()
-#         name = typer.prompt("Dataset name")
-#         description = typer.prompt("Description")
-#         # confirm
-#         typer.confirm(f"Is the data correct?", abort=True)
-#         ingest_dataset(name, description, path, user, typer.echo)
-#         typer.echo(f"Dataset {name} ingested")
-#     except Exception as e:
-#         typer.echo(e)
-
-
 @app.command()
 def ingest(
     path: str,
-    n: Optional[str] = None,
-    d: Optional[str] = None,
-    p: Optional[bool] = False,
+    name: str,
+    # p: Optional[int] = 0,
 ):
     """
     Ingest a dataset
 
     path: Path to dataset to ingest
     n: Name of the dataset
-    d: Description of the dataset
-    p: Parallel ingest
     """
     try:
         user = auth()
-        name = n or typer.prompt("Dataset name")
-        description = d or typer.prompt("Description")
-        # confirm
-        if not n or not d:
-            typer.confirm(f"Is the data correct?", abort=True)
-        if p:
-            ingest_large_dataset_parallel(name, description, path, user, typer.echo)
-        else:
-            ingest_large_dataset(name, description, path, user, typer.echo)
+        # ingest_large_dataset_parallel(name, path, user, p, typer.echo)
+        ingest_large_dataset(name, path, user, typer.echo)
         typer.echo(f"Dataset {name} ingested")
     except Exception as e:
         typer.echo(e)
 
 
+@app.command()
+def update(
+    name: str,
+    path: str,
+):
+    """
+    Update a dataset
+
+    name: Name of the dataset
+    path: Path to dataset to ingest
+    """
+    try:
+        user = auth()
+        update_dataset(name, path, user, typer.echo)
+        typer.echo(f"Dataset {name} updated")
+    except Exception as e:
+        typer.echo(e)
+
+
 if __name__ == "__main__":
     app()
```

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/APIRepo.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/repos/APIRepo.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import requests
 from tqdm import tqdm
 from pathlib import Path
 import os
 from concurrent.futures import ThreadPoolExecutor
 import time
+import multiprocessing
 
 
 class APIRepo:
     def __init__(self, url=os.getenv("EOTDL_API_URL", "https://api.eotdl.com/")):
         self.url = url
 
     def login(self):
@@ -34,185 +35,231 @@
         headers = {"Authorization": "Bearer " + id_token}
         if path is None:
             path = str(Path.home()) + "/.etodl/datasets"
             os.makedirs(path, exist_ok=True)
         with requests.get(url, headers=headers, stream=True) as r:
             r.raise_for_status()
             total_size = int(r.headers.get("content-length", 0))
-            block_size = 1024  # 1 Kibibyte
-            progress_bar = tqdm(total=total_size, unit="iB", unit_scale=True)
+            block_size = 1024 * 1024 * 10
+            progress_bar = tqdm(
+                total=total_size, unit="iB", unit_scale=True, unit_divisor=1024
+            )
             filename = r.headers.get("content-disposition").split("filename=")[1][1:-1]
             path = f"{path}/{filename}"
             with open(path, "wb") as f:
                 for chunk in r.iter_content(block_size):
                     progress_bar.update(len(chunk))
-                    f.write(chunk)
+                    if chunk:
+                        f.write(chunk)
             progress_bar.close()
             return path
 
-    def ingest_dataset(self, name, description, path, id_token):
-        # Not sure this will work with large datasets, need to test
-        url = self.url + "datasets"
-        headers = {"Authorization": "Bearer " + id_token}
-        files = {"file": open(path, "rb")}
-        data = {"name": name, "description": description}
-        response = requests.post(url, headers=headers, files=files, data=data)
-        if response.status_code == 200:
-            return response.json(), None
-        return None, response.json()["detail"]
-
     def read_in_chunks(self, file_object, CHUNK_SIZE):
         while True:
             data = file_object.read(CHUNK_SIZE)
             if not data:
                 break
             yield data
 
-    def parallel_upload(
-        self,
-        content_size,
-        chunk_size,
-        content_path,
-        url,
-        id_token,
-        upload_id,
-        dataset_id,
-        total_chunks,
-    ):
-        # Create thread pool executor
-        executor = ThreadPoolExecutor()
-
-        # Divide file into chunks and create tasks for each chunk
-        offset = 0
-        tasks = []
-        while offset < content_size:
-            chunk_end = min(offset + chunk_size, content_size)
-            tasks.append((offset, chunk_end, str(offset // chunk_size + 1)))
-            offset = chunk_end
-
-        # Define the function that will upload each chunk
-        def upload_chunk(start, end, part):
-            # print(f"Uploading chunk {start} - {end}", part)
-            with open(content_path, "rb") as f:
-                f.seek(start)
-                chunk = f.read(end - start)
-            # headers["Part-Number"] = part
-            response = requests.post(
-                url,
-                files={"file": chunk},
-                headers={
-                    "Authorization": "Bearer " + id_token,
-                    "Upload-Id": upload_id,
-                    "Dataset-Id": dataset_id,
-                    "Part-Number": part,
-                },
-            )
-            if response.status_code != 200:
-                print(f"Failed to upload chunk {start} - {end}")
-            return response
-
-        # Submit each task to the executor
-        with tqdm(total=total_chunks) as pbar:
-            futures = []
-            for task in tasks:
-                future = executor.submit(upload_chunk, *task)
-                future.add_done_callback(lambda p: pbar.update())
-                futures.append(future)
-
-            # Wait for all tasks to complete
-            for future in futures:
-                future.result()
-
-    def prepare_large_upload(self, name, description, path, id_token):
-        # first call to get upload id
-        url = self.url + "datasets/chunk?name=" + name + "&description=" + description
+    def prepare_large_upload(self, name, id_token, checksum):
+        url = self.url + "datasets/chunk?name=" + name + "&checksum=" + checksum
         response = requests.get(url, headers={"Authorization": "Bearer " + id_token})
         if response.status_code != 200:
-            return None, response.json()["detail"]
+            raise Exception(response.json()["detail"])
         data = response.json()
-        dataset_id, upload_id = data["dataset_id"], data["upload_id"]
+        dataset_id, upload_id, parts = (
+            data["dataset_id"],
+            data["upload_id"],
+            data["parts"] if "parts" in data else [],
+        )
+        return dataset_id, upload_id, parts
+
+    def ingest_large_dataset(
+        self, path, chunk_size, upload_id, dataset_id, id_token, parts
+    ):
         content_path = os.path.abspath(path)
         content_size = os.stat(content_path).st_size
-        url = self.url + "datasets/chunk"
-        chunk_size = 1024 * 1024 * 5  # 5 MiB
         total_chunks = content_size // chunk_size
-        return (
-            content_size,
-            chunk_size,
-            content_path,
-            url,
-            upload_id,
-            dataset_id,
-            total_chunks,
+        url = self.url + "datasets/chunk"
+        headers = {
+            "Authorization": "Bearer " + id_token,
+            "Upload-Id": upload_id,
+            "Dataset-Id": dataset_id,
+        }
+        # upload chunks sequentially
+        pbar = tqdm(
+            self.read_in_chunks(open(content_path, "rb"), chunk_size),
+            total=total_chunks,
         )
+        index = 0
+        for chunk in pbar:
+            part = index // chunk_size + 1
+            offset = index + len(chunk)
+            index = offset
+            if part not in parts:
+                headers["Part-Number"] = str(part)
+                file = {"file": chunk}
+                r = requests.post(url, files=file, headers=headers)
+                if r.status_code != 200:
+                    return None, r.json()["detail"]
+            pbar.set_description(
+                "{:.2f}/{:.2f} MB".format(
+                    offset / 1024 / 1024, content_size / 1024 / 1024
+                )
+            )
+        pbar.close()
 
-    def complete_upload(self, name, description, id_token, upload_id, dataset_id):
+    def complete_upload(self, name, id_token, upload_id, dataset_id, checksum):
         url = self.url + "datasets/complete"
         r = requests.post(
             url,
-            json={"name": name, "description": description},
+            json={"name": name, "checksum": checksum},
             headers={
                 "Authorization": "Bearer " + id_token,
                 "Upload-Id": upload_id,
                 "Dataset-Id": dataset_id,
             },
         )
+        if r.status_code != 200:
+            return None, r.json()["detail"]
         return r.json(), None
 
-    def ingest_large_dataset(self, name, description, path, id_token):
-        (
-            content_size,
-            chunk_size,
-            content_path,
-            url,
-            upload_id,
-            dataset_id,
-            total_chunks,
-        ) = self.prepare_large_upload(name, description, path, id_token)
+    def update_dataset(self, name, path, id_token, checksum):
+        # check that dataset exists
+        data, error = self.retrieve_dataset(name)
+        if error:
+            return None, error
+        # first call to get upload id
+        dataset_id = data["id"]
+        url = self.url + f"datasets/chunk/{dataset_id}?checksum={checksum}"
+        response = requests.get(url, headers={"Authorization": "Bearer " + id_token})
+        if response.status_code != 200:
+            return None, response.json()["detail"]
+        data = response.json()
+        _, upload_id, parts = data["dataset_id"], data["upload_id"], data["parts"]
+        # assert dataset_id is None
+        content_path = os.path.abspath(path)
+        content_size = os.stat(content_path).st_size
+        url = self.url + "datasets/chunk"
+        chunk_size = 1024 * 1024 * 10  # 10 MiB
+        total_chunks = content_size // chunk_size
         headers = {
             "Authorization": "Bearer " + id_token,
             "Upload-Id": upload_id,
             "Dataset-Id": dataset_id,
         }
         # upload chunks sequentially
         pbar = tqdm(
             self.read_in_chunks(open(content_path, "rb"), chunk_size),
             total=total_chunks,
         )
         index = 0
         for chunk in pbar:
             offset = index + len(chunk)
-            headers["Part-Number"] = str(index // chunk_size + 1)
+            part = index // chunk_size + 1
             index = offset
-            file = {"file": chunk}
-            r = requests.post(url, files=file, headers=headers)
-            if r.status_code != 200:
-                return None, r.json()["detail"]
+            if part not in parts:
+                headers["Part-Number"] = str(part)
+                file = {"file": chunk}
+                r = requests.post(url, files=file, headers=headers)
+                if r.status_code != 200:
+                    return None, r.json()["detail"]
             pbar.set_description(
                 "{:.2f}/{:.2f} MB".format(
                     offset / 1024 / 1024, content_size / 1024 / 1024
                 )
             )
         pbar.close()
-        return self.complete_upload(name, description, id_token, upload_id, dataset_id)
-
-    def ingest_large_dataset_parallel(self, name, description, path, id_token):
-        (
-            content_size,
-            chunk_size,
-            content_path,
-            url,
-            upload_id,
-            dataset_id,
-            total_chunks,
-        ) = self.prepare_large_upload(name, description, path, id_token)
-        self.parallel_upload(
-            content_size,
-            chunk_size,
-            content_path,
+        # complete upload
+        url = self.url + "datasets/complete"
+        r = requests.post(
             url,
-            id_token,
-            upload_id,
-            dataset_id,
-            total_chunks,
+            json={"checksum": checksum},
+            headers={
+                "Authorization": "Bearer " + id_token,
+                "Upload-Id": upload_id,
+                "Dataset-Id": dataset_id,
+            },
         )
-        return self.complete_upload(name, description, id_token, upload_id, dataset_id)
+        if r.status_code != 200:
+            return None, r.json()["detail"]
+        return r.json(), None
+
+    # def parallel_upload(
+    #     self,
+    #     content_size,
+    #     chunk_size,
+    #     content_path,
+    #     url,
+    #     id_token,
+    #     upload_id,
+    #     dataset_id,
+    #     total_chunks,
+    #     threads,
+    # ):
+    #     # Create thread pool executor
+    #     max_workers = threads if threads > 0 else multiprocessing.cpu_count()
+    #     executor = ThreadPoolExecutor(max_workers=max_workers)
+
+    #     # Divide file into chunks and create tasks for each chunk
+    #     offset = 0
+    #     tasks = []
+    #     while offset < content_size:
+    #         chunk_end = min(offset + chunk_size, content_size)
+    #         tasks.append((offset, chunk_end, str(offset // chunk_size + 1)))
+    #         offset = chunk_end
+
+    #     # Define the function that will upload each chunk
+    #     def upload_chunk(start, end, part):
+    #         # print(f"Uploading chunk {start} - {end}", part)
+    #         with open(content_path, "rb") as f:
+    #             f.seek(start)
+    #             chunk = f.read(end - start)
+    #         # headers["Part-Number"] = part
+    #         response = requests.post(
+    #             url,
+    #             files={"file": chunk},
+    #             headers={
+    #                 "Authorization": "Bearer " + id_token,
+    #                 "Upload-Id": upload_id,
+    #                 "Dataset-Id": dataset_id,
+    #                 "Part-Number": part,
+    #             },
+    #         )
+    #         if response.status_code != 200:
+    #             print(f"Failed to upload chunk {start} - {end}")
+    #         return response
+
+    #     # Submit each task to the executor
+    #     with tqdm(total=total_chunks) as pbar:
+    #         futures = []
+    #         for task in tasks:
+    #             future = executor.submit(upload_chunk, *task)
+    #             future.add_done_callback(lambda p: pbar.update())
+    #             futures.append(future)
+
+    #         # Wait for all tasks to complete
+    #         for future in futures:
+    #             future.result()
+
+    # def ingest_large_dataset_parallel(self, name, description, path, id_token, threads):
+    #     (
+    #         content_size,
+    #         chunk_size,
+    #         content_path,
+    #         url,
+    #         upload_id,
+    #         dataset_id,
+    #         total_chunks,
+    #     ) = self.prepare_large_upload(name, description, path, id_token)
+    #     self.parallel_upload(
+    #         content_size,
+    #         chunk_size,
+    #         content_path,
+    #         url,
+    #         id_token,
+    #         upload_id,
+    #         dataset_id,
+    #         total_chunks,
+    #         threads,
+    #     )
+    #     return self.complete_upload(name, description, id_token, upload_id, dataset_id)
```

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/repos/AuthRepo.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/auth/main.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDataset.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 from pydantic import BaseModel
 
 
-class IngestLargeDataset:
+class IngestLargeDatasetParallel:
     def __init__(self, repo, logger):
         self.repo = repo
         self.logger = logger
 
     class Inputs(BaseModel):
         name: str
         description: str
         path: str = None
         user: dict
+        threads: int = 0
 
     class Outputs(BaseModel):
         dataset: dict
 
     def __call__(self, inputs: Inputs) -> Outputs:
         # allow only zip files
         if not inputs.path.endswith(".zip"):
             raise Exception("Only zip files are allowed")
         self.logger("Ingesting dataset...")
-        data, error = self.repo.ingest_large_dataset(
-            inputs.name, inputs.description, inputs.path, inputs.user["id_token"]
+        data, error = self.repo.ingest_large_dataset_parallel(
+            inputs.name,
+            inputs.description,
+            inputs.path,
+            inputs.user["id_token"],
+            inputs.threads,
         )
         if error:
             raise Exception(error)
         self.logger("Done")
         return self.Outputs(dataset=data)
```

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/IngestLargeDatasetParallel.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/DownloadDataset.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,29 +1,27 @@
 from pydantic import BaseModel
+from src.utils import calculate_checksum
 
 
-class IngestLargeDatasetParallel:
+class DownloadDataset:
     def __init__(self, repo, logger):
         self.repo = repo
         self.logger = logger
 
     class Inputs(BaseModel):
-        name: str
-        description: str
+        dataset: str
         path: str = None
         user: dict
+        checksum: str
 
     class Outputs(BaseModel):
-        dataset: dict
+        dst_path: str
 
     def __call__(self, inputs: Inputs) -> Outputs:
-        # allow only zip files
-        if not inputs.path.endswith(".zip"):
-            raise Exception("Only zip files are allowed")
-        self.logger("Ingesting dataset...")
-        data, error = self.repo.ingest_large_dataset_parallel(
-            inputs.name, inputs.description, inputs.path, inputs.user["id_token"]
+        dst_path = self.repo.download_dataset(
+            inputs.dataset, inputs.user["id_token"], inputs.path
         )
-        if error:
-            raise Exception(error)
-        self.logger("Done")
-        return self.Outputs(dataset=data)
+        checksum = calculate_checksum(dst_path)
+        self.logger(f"Checksum: {checksum}")
+        if inputs.checksum != checksum:
+            self.logger("Checksums do not match")
+        return self.Outputs(dst_path=dst_path)
```

### Comparing `eotdl-cli-2023.5.9.post4/eotdl_cli/src/usecases/datasets/main.py` & `eotdl-cli-2023.6.8/eotdl_cli/src/usecases/datasets/main.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from ...repos import APIRepo
 from .RetrieveDatasets import RetrieveDatasets
 from .RetrieveDataset import RetrieveDataset
 from .DownloadDataset import DownloadDataset
 from .IngestDataset import IngestDataset
 from .IngestLargeDataset import IngestLargeDataset
 from .IngestLargeDatasetParallel import IngestLargeDatasetParallel
+from .UpdateDataset import UpdateDataset
 
 
 def retrieve_datasets():
     api_repo = APIRepo()
     retrieve = RetrieveDatasets(api_repo)
     inputs = retrieve.Inputs()
     outputs = retrieve(inputs)
@@ -19,38 +20,52 @@
     api_repo = APIRepo()
     retrieve = RetrieveDataset(api_repo)
     inputs = retrieve.Inputs(name=name)
     outputs = retrieve(inputs)
     return outputs.dataset
 
 
-def download_dataset(name, path, user):
-    dataset_id = retrieve_dataset(name)["id"]
-    api_repo = APIRepo()
-    download = DownloadDataset(api_repo)
-    inputs = download.Inputs(dataset=dataset_id, path=path, user=user)
+def download_dataset(name, path, user, logger):
+    dataset = retrieve_dataset(name)
+    dataset_id = dataset["id"]
+    checksum = dataset["checksum"]
+    api_repo = APIRepo()
+    download = DownloadDataset(api_repo, logger)
+    inputs = download.Inputs(
+        dataset=dataset_id, checksum=checksum, path=path, user=user
+    )
     outputs = download(inputs)
     return outputs.dst_path
 
 
 def ingest_dataset(name, description, path, user, logger):
     api_repo = APIRepo()
-    ingest = IngestDataset(api_repo, logger)
+    ingest = IngestDataset(
+        api_repo,
+    )
     inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
 
 
-def ingest_large_dataset(name, description, path, user, logger):
+def ingest_large_dataset(name, path, user, logger):
     api_repo = APIRepo()
     ingest = IngestLargeDataset(api_repo, logger)
-    inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+    inputs = ingest.Inputs(name=name, path=path, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
 
 
-def ingest_large_dataset_parallel(name, description, path, user, logger):
+def ingest_large_dataset_parallel(name, path, user, p, logger):
     api_repo = APIRepo()
     ingest = IngestLargeDatasetParallel(api_repo, logger)
-    inputs = ingest.Inputs(name=name, description=description, path=path, user=user)
+    inputs = ingest.Inputs(name=name, path=path, user=user, threads=p)
+    outputs = ingest(inputs)
+    return outputs.dataset
+
+
+def update_dataset(name, path, user, logger):
+    api_repo = APIRepo()
+    ingest = UpdateDataset(api_repo, logger)
+    inputs = ingest.Inputs(name=name, path=path, user=user)
     outputs = ingest(inputs)
     return outputs.dataset
```

### Comparing `eotdl-cli-2023.5.9.post4/pyproject.toml` & `eotdl-cli-2023.6.8/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.05.09-4"
+version = "2023.06.08"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
@@ -14,15 +14,14 @@
 python = "^3.8"
 typer = {extras = ["all"], version = "^0.7.0"}
 requests = "^2.28.2"
 pydantic = "^1.10.6"
 tqdm = "^4.65.0"
 pyjwt = "^2.6.0"
 
-
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
 pytest-watch = "^4.2.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `eotdl-cli-2023.5.9.post4/setup.py` & `eotdl-cli-2023.6.8/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  'typer[all]>=0.7.0,<0.8.0']
 
 entry_points = \
 {'console_scripts': ['eotdl-cli = eotdl_cli.main:app']}
 
 setup_kwargs = {
     'name': 'eotdl-cli',
-    'version': '2023.5.9.post4',
+    'version': '2023.6.8',
     'description': '',
     'long_description': '# eotdl-cli\n\nThis is the CLI for EOTDL.\n\n',
     'author': 'EarthPulse',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `eotdl-cli-2023.5.9.post4/PKG-INFO` & `eotdl-cli-2023.6.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.5.9.post4
+Version: 2023.6.8
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

