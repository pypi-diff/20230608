# Comparing `tmp/dare_datasets-0.1.5.tar.gz` & `tmp/dare_datasets-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dare_datasets-0.1.5.tar", max compression
+gzip compressed data, was "dare_datasets-0.1.7.tar", max compression
```

## Comparing `dare_datasets-0.1.5.tar` & `dare_datasets-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      178 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/README.md
--rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/__init__.py
--rw-r--r--   0        0        0     2310 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/dataset_abc.py
--rw-r--r--   0        0        0     1427 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/qr2t_benchmark.py
--rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/utils/__init__.py
--rw-r--r--   0        0        0      459 2023-05-27 09:16:11.245474 dare_datasets-0.1.5/dare_datasets/utils/downloader.py
--rw-r--r--   0        0        0      588 2023-05-27 09:22:09.076489 dare_datasets-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 dare_datasets-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0      989 2023-06-08 11:08:35.634718 dare_datasets-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.7/dare_datasets/__init__.py
+-rw-r--r--   0        0        0     2483 2023-06-08 11:08:35.634718 dare_datasets-0.1.7/dare_datasets/dataset_abc.py
+-rw-r--r--   0        0        0     1886 2023-06-08 11:08:35.634718 dare_datasets-0.1.7/dare_datasets/iris.py
+-rw-r--r--   0        0        0     1318 2023-06-08 11:08:35.634718 dare_datasets-0.1.7/dare_datasets/qr2t_benchmark.py
+-rw-r--r--   0        0        0        0 2023-05-27 09:16:11.245474 dare_datasets-0.1.7/dare_datasets/utils/__init__.py
+-rw-r--r--   0        0        0      459 2023-05-27 09:16:11.245474 dare_datasets-0.1.7/dare_datasets/utils/downloader.py
+-rw-r--r--   0        0        0      831 2023-06-08 11:45:05.322270 dare_datasets-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1646 1970-01-01 00:00:00.000000 dare_datasets-0.1.7/PKG-INFO
```

### Comparing `dare_datasets-0.1.5/dare_datasets/dataset_abc.py` & `dare_datasets-0.1.7/dare_datasets/dataset_abc.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 from abc import ABC, abstractmethod
-
-# Url of the FOLDER of the dataset in Google Drive. The folder must be publicly available.
-GDRIVE_URL = ""
+from pathlib import Path
 
 
 class Dataset(ABC):
     """
     Set of methods that every dataset should implement.
 
     Apart from these methods the class can
     implement whichever other method is considered needed e.g. different versions of the dataset.
     """
-    @abstractmethod
-    def __init__(self, cache_dir: str | None = '~/.cache/dare-datasets/') -> None:
+    def __init__(self, dataset_name: str, cache_dir: str | None) -> None:
         """
         Initializer chooses the cache directory where the dataset will be downloaded or retrieved.
         Note the dataset is not yet downloaded.
 
         Args:
+            dataset_name: Name of the dataset.
             cache_dir: Folder where the dataset will be downloaded or retrieved from.
         """
-        pass
+        self.data = None
+        self.cache_dir = cache_dir if cache_dir is not None else str(Path.home()) + '/.cache/dare-datasets/'
+        self.dataset_name = dataset_name
+        self.dataset_folder = self.cache_dir + dataset_name + "/"
 
     @abstractmethod
     def _init_data(self):
         """
         Loads the dataset from disk. If the dataset is not available on disk, it is downloaded and saved in cache.
         """
         pass
@@ -55,15 +56,15 @@
                  "test":[]
             }
         ```
         """
         pass
 
     @abstractmethod
-    def get_processed(self):
+    def get_processed(self, **kwargs):
         """
         Returns the processed data of the dataset on whichever format we consider default.
         If many processed versions are available, the one we consider default should be the one returned.
         Structure (if not applicable it is not enforced):
         ```python
             {
                  "train":[],
```

### Comparing `dare_datasets-0.1.5/dare_datasets/qr2t_benchmark.py` & `dare_datasets-0.1.7/dare_datasets/qr2t_benchmark.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,27 +8,25 @@
 from dare_datasets.utils.downloader import get_file_from_gdrive
 
 GDRIVE_URL = "https://drive.google.com/drive/folders/1LCD4gObeX-PBxkNYNuZxSmrTBvzEK095?usp=sharing"
 DATASET_NAME = "QR2T_Benchmark"
 
 
 class QR2TBenchmark(Dataset):
-    def __init__(self, cache_dir: typing.Optional[str] = f'{Path.home()}/.cache/dare-datasets/') -> None:
-        self.data = None
-        self.cache_dir = cache_dir
-        self.dataset_folder = cache_dir + DATASET_NAME + "/"
+    def __init__(self, cache_dir: typing.Optional[str] = None) -> None:
+        super().__init__(DATASET_NAME, cache_dir)
 
     def get_info(self) -> dict[str, str]:
         return {
             "name": "QR2T Benchmark",
             "description": "QR2T Benchmark is an extension of the Spider dataset for the QR2T task.",
             "url": GDRIVE_URL,
             "original_url": "-",
             "formats": ["json"],
-            "dataset_folder": self.dataset_folder if self.data is not None else "NOT_YET_DOWNLOADED"
+            "dataset_folder": self.dataset_folder if self.data is not None else "NOT_YET_LOADED"
         }
 
     def _init_data(self):
         get_file_from_gdrive(url=GDRIVE_URL, cache_dir=self.cache_dir, folder_name=DATASET_NAME)
 
         self.data = {}
         for file in glob.glob(self.dataset_folder + "*"):
```

