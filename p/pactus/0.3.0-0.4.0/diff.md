# Comparing `tmp/pactus-0.3.0.tar.gz` & `tmp/pactus-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/pactus/pactus/dist/.tmp-nfx43jlq/pactus-0.3.0.tar", last modified: Sat Apr  8 22:05:00 2023, max compression
+DOS/MBR boot sector; partition 1 : ID=0x86, active 0xf6, start-CHS (0x1e4,39,44), end-CHS (0x8,17,20), startsector 4091241006, 3650289469 sectors; partition 2 : ID=0xc8, active 0xcc, start-CHS (0x1c,129,10), end-CHS (0x11,25,31), startsector 3353880728, 1122530999 sectors; partition 3 : ID=0x28, active 0xe6, start-CHS (0x2a3,30,51), end-CHS (0x1b,112,60), startsector 3991417312, 1677054193 sectors
```

## Comparing `pactus-0.3.0.tar` & `pactus-0.4.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.643139 pactus-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-04-08 22:04:36.000000 pactus-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-04-08 22:05:00.643139 pactus-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      617 2023-04-08 22:04:36.000000 pactus-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.639140 pactus-0.3.0/pactus/
--rw-r--r--   0 runner    (1001) docker     (122)      513 2023-04-08 22:04:45.000000 pactus-0.3.0/pactus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/config.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.639140 pactus-0.3.0/pactus/dataset/
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/dataset/_utils.py
--rw-r--r--   0 runner    (1001) docker     (122)    10775 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/dataset/dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.643139 pactus-0.3.0/pactus/models/
--rw-r--r--   0 runner    (1001) docker     (122)      870 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/decision_tree_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     8800 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/evaluation_comparison.py
--rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/kneighbors_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     5137 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/lstm_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/random_forest_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/svm_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     2883 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/transformer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8591 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1762 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/xgboost_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     4898 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/zoom_transformer_model.py
--rw-r--r--   0 runner    (1001) docker     (122)     1719 2023-04-08 22:04:36.000000 pactus-0.3.0/pactus/models/zoomletizer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-08 22:05:00.639140 pactus-0.3.0/pactus.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2463 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      738 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      139 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-08 22:05:00.000000 pactus-0.3.0/pactus.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-04-08 22:04:45.000000 pactus-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-08 22:05:00.643139 pactus-0.3.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 19:30:57.767287 pactus-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1065 2023-06-08 19:30:33.000000 pactus-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-08 19:30:57.767287 pactus-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2041 2023-06-08 19:30:33.000000 pactus-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 19:30:57.763287 pactus-0.4.0/pactus/
+-rw-r--r--   0 runner    (1001) docker     (122)      513 2023-06-08 19:30:42.000000 pactus-0.4.0/pactus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1020 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 19:30:57.767287 pactus-0.4.0/pactus/dataset/
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4494 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/dataset/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13013 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/dataset/dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 19:30:57.767287 pactus-0.4.0/pactus/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1221 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/decision_tree_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8800 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/evaluation_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1222 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/kneighbors_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5866 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/lstm_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1688 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1219 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/random_forest_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1172 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/svm_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2883 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9359 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/transformer_model.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1802 2023-06-08 19:30:33.000000 pactus-0.4.0/pactus/models/xgboost_model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 19:30:57.767287 pactus-0.4.0/pactus.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3887 2023-06-08 19:30:57.000000 pactus-0.4.0/pactus.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      698 2023-06-08 19:30:57.000000 pactus-0.4.0/pactus.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-06-08 19:30:57.000000 pactus-0.4.0/pactus.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-06-08 19:30:57.000000 pactus-0.4.0/pactus.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-06-08 19:30:57.000000 pactus-0.4.0/pactus.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1871 2023-06-08 19:30:42.000000 pactus-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-06-08 19:30:57.767287 pactus-0.4.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-08 19:30:57.767287 pactus-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     2294 2023-06-08 19:30:33.000000 pactus-0.4.0/tests/test_data.py
```

### Comparing `pactus-0.3.0/LICENSE` & `pactus-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/__init__.py` & `pactus-0.4.0/pactus/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from yupi import DiffMethod, Trajectory, WindowType
 from yupi.core import featurizers
 
 from pactus.dataset import Dataset
 from pactus.models import Evaluation, EvaluationComparison
 
-__version__ = "0.3.0"
+__version__ = "0.4.0"
 
 __all__ = [
     "Dataset",
     "Evaluation",
     "EvaluationComparison",
     "featurizers",
 ]
```

### Comparing `pactus-0.3.0/pactus/config.py` & `pactus-0.4.0/pactus/config.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/dataset/_utils.py` & `pactus-0.4.0/pactus/dataset/_utils.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/dataset/dataset.py` & `pactus-0.4.0/pactus/dataset/dataset.py`

 * *Files 17% similar despite different names*

```diff
@@ -19,25 +19,38 @@
 REPO_URL = "https://github.com/yupidevs/trajectory-datasets"
 
 
 class Data:
     """
     Structure that groups the trajectories and labels along with some
     useful methods to work with the set of them.
+
+    Parameters
+    ----------
+    trajs: List[Trajectory]
+        A list that contains a subset of the dataset trajectories.
+    labels: List[Any]
+        A list that contains the label of each trajectory from the subset.
+    dataset_name: str
+        Name of the dataset where the trajectories come from. If not provided,
+        it will be set to "custom".
     """
 
     def __init__(
-        self, dataset: Dataset, trajs: List[Trajectory], labels: List[Any]
+        self,
+        trajs: List[Trajectory],
+        labels: List[Any],
+        dataset_name: str = "custom",
     ) -> None:
-        self.dataset = dataset
         self.trajs = trajs
         self.labels = labels
         self.label_counts = Counter(labels)
         self.feats = None
         self.last_featurizer = None
+        self.dataset_name = dataset_name
 
     @property
     def classes(self) -> List[Any]:
         """Classes present in the dataset."""
         return list(self.label_counts.keys())
 
     def __len__(self) -> int:
@@ -66,41 +79,78 @@
     def take(
         self,
         size: Union[float, int],
         stratify: bool = True,
         shuffle: bool = True,
         random_state: Union[int, None] = None,
     ) -> Data:
-        """Takes a subset of the dataset."""
+        """
+        Takes a subset of the dataset.
+        
+        Parameters
+        ----------
+        size : Union[float, int]
+            If float, it should be between 0 and 1 and it will be interpreted
+            as the proportion of the dataset to be taken. If int, it should be
+            between 0 and the dataset size and it will be interpreted as the
+            number of trajectories to be taken.
+        stratify : bool, optional
+            If True, the dataset will be stratified by the labels, by default
+            True.
+        shuffle : bool, optional
+            If True, the dataset will be shuffled before taking the subset,
+            by default True.
+        random_state : Union[int, None], optional
+            Random state to be used, by default None.
+        
+        Returns
+        -------
+        Data
+            A new Data object with the subset of the dataset.
+        """
         if isinstance(size, int):
             assert 0 < size < len(self), "size should be within 0 and len(self)"
             size /= len(self)
 
         ans, _ = self.split(
             size, stratify=stratify, shuffle=shuffle, random_state=random_state
         )
         return ans
 
-    def cut(self, size: Union[float, int]):
+    def cut(self, size: Union[float, int]) -> Tuple[Data, Data]:
         """
         Similar to split, but without shuffle, stratify, etc. Just slices the
         dataset into two parts.
+
+        Parameters
+        ----------
+        size : Union[float, int]
+            If float, it should be between 0 and 1 and it will be interpreted
+            as the proportion of the dataset to be taken. If int, it should be
+            between 0 and the dataset size and it will be interpreted as the
+            number of trajectories to be taken.
+        
+        Returns
+        -------
+        Tuple[Data, Data]
+            A tuple with two Data objects, the first one with the first part
+            of the cut and the second one with the second part.
         """
         if isinstance(size, float):
             assert 0 < size < 1, "size should be within 0 and 1 if float"
             size = int(len(self) * size)
         else:
             assert (
                 0 < size < len(self)
             ), "size should be within 0 and the dataset size if int"
 
         left, right = self.trajs[:size], self.trajs[size:]
         left_labels, right_labels = self.labels[:size], self.labels[size:]
-        left_d = Data(self.dataset, left, left_labels)
-        right_d = Data(self.dataset, right, right_labels)
+        left_d = Data(left, left_labels)
+        right_d = Data(right, right_labels)
         return left_d, right_d
 
     def split(
         self,
         train_size: Union[float, int] = 0.8,
         stratify: bool = True,
         shuffle: bool = True,
@@ -143,16 +193,16 @@
             self.labels,
             train_size=train_size,
             stratify=self.labels if stratify else None,
             random_state=random_state,
             shuffle=shuffle,
         )
 
-        train_data = Data(self.dataset, x_train, y_train)
-        test_data = Data(self.dataset, x_test, y_test)
+        train_data = Data(x_train, y_train)
+        test_data = Data(x_test, y_test)
         return train_data, test_data
 
     def map(self, func: Callable[[Trajectory, Any], Tuple[Trajectory, Any]]) -> Data:
         """
         Applies a function to each trajectory and label pair.
 
         Usefull to apply some preprocessing to the trajectories
@@ -169,15 +219,15 @@
             A new Data object with the results of the function.
         """
         trajs, labels = [], []
         for traj, label in zip(self.trajs, self.labels):
             traj, label = func(traj, label)
             trajs.append(traj)
             labels.append(label)
-        return Data(self.dataset, trajs, labels)
+        return Data(trajs, labels)
 
     def filter(self, func: Callable[[Trajectory, Any], bool]) -> Data:
         """
         Filters the dataset based on a function.
 
         Parameters
         ----------
@@ -191,49 +241,61 @@
         """
         trajs, labels = [], []
         for traj, label in zip(self.trajs, self.labels):
             if func(traj, label):
                 trajs.append(traj)
                 labels.append(label)
         logging.info("Filtered %d of %d trajectories", len(trajs), len(self))
-        return Data(self.dataset, trajs, labels)
+        return Data(trajs, labels)
 
 
 class Dataset(Data):
-    """Wraps the data with some general properties that describes a full dataset"""
+    """
+    Wraps the data with some general properties that describes a full dataset
 
-    _last_tag = None
+    Parameters
+    ----------
+    name : str
+        Name of the dataset.
+    trajs: List[Trajectory]
+        A list that contains the dataset trajectories.
+    labels: List[Any]
+        A list that contains the label of each trajectory.
+    version: int
+        Dataset version.
+    """
+
+    _last_tag: Union[str, None] = None
 
     def __init__(
         self,
         name: str,
         trajs: List[Trajectory],
         labels: List[Any],
         version: int = 0,
     ):
         self.name = name
         self.version = version
         self.trajs = trajs
         self.labels = labels
-        super().__init__(self, trajs, labels)
+        super().__init__(trajs, labels, dataset_name=name)
 
     def __len__(self):
         return len(self.trajs)
 
     @staticmethod
     def _from_json(name: str, data: dict) -> Dataset:
         assert "trajs" in data, "trajs not found in dataset"
         assert "labels" in data, "labels not found in dataset"
-        assert "version" in data, "version not found in dataset"
         trajs = [JSONSerializer.from_json(traj) for traj in data["trajs"]]
         return Dataset(
             name=name,
             trajs=trajs,
             labels=data["labels"],
-            version=data["version"],
+            version=data.get("version", 0),
         )
 
     @staticmethod
     def _get_dataset_url(name: str) -> str:
         tag = Dataset._last_tag
         if tag is None:
             g_cmd = Git()
@@ -248,15 +310,15 @@
         url = Dataset._get_dataset_url(name)
         raw_dir = _get_path(config.DS_DIR, name)
         yupi_data_file = raw_dir / f"{name}.json"
 
         if not force and yupi_data_file.exists():
             with open(yupi_data_file, "r", encoding="utf-8") as yupi_fd:
                 data = json.load(yupi_fd)
-                if "trajs" in data and "labels" in data and "version" in data:
+                if "trajs" in data and "labels" in data:
                     return Dataset._from_json(name, data)
             logging.warning("Invalid dataset file, downloading again")
 
         download_dataset(url, name)
         return Dataset.from_file(yupi_data_file, name)
 
     @staticmethod
@@ -266,53 +328,58 @@
         with open(_path, "r", encoding="utf-8") as yupi_fd:
             data = json.load(yupi_fd)
             return Dataset._from_json(name, data)
 
     @staticmethod
     def geolife(redownload: bool = False) -> Dataset:
         """Loads the geolife dataset"""
-        return Dataset._from_url("geolife", force=redownload)
+        return Dataset.get("geolife", redownload=redownload)
 
     @staticmethod
     def animals(redownload: bool = False) -> Dataset:
         """Loads the animals dataset"""
-        return Dataset._from_url("animals", force=redownload)
+        return Dataset.get("animals", redownload=redownload)
 
     @staticmethod
     def mnist_stroke(redownload: bool = False) -> Dataset:
         """Loads the mnist_stroke dataset"""
-        return Dataset._from_url("mnist_stroke", force=redownload)
+        return Dataset.get("mnist_stroke", redownload=redownload)
 
     @staticmethod
     def hurdat2(redownload: bool = False) -> Dataset:
         """Loads the hurdat2 dataset"""
-        return Dataset._from_url("hurdat2", force=redownload)
+        return Dataset.get("hurdat2", redownload=redownload)
 
     @staticmethod
     def cma_bst(redownload: bool = False) -> Dataset:
         """Loads the cma_bst dataset"""
-        return Dataset._from_url("cma_bst", force=redownload)
+        return Dataset.get("cma_bst", redownload=redownload)
 
     @staticmethod
     def uci_gotrack(redownload: bool = False) -> Dataset:
         """Loads the uci_gotrack dataset"""
-        return Dataset._from_url("uci_gotrack", force=redownload)
+        return Dataset.get("uci_gotrack", redownload=redownload)
 
     @staticmethod
     def uci_movement_libras(redownload: bool = False) -> Dataset:
         """Loads the uci_movement_libras dataset"""
-        return Dataset._from_url("uci_movement_libras", force=redownload)
+        return Dataset.get("uci_movement_libras", redownload=redownload)
 
     @staticmethod
     def uci_pen_digits(redownload: bool = False) -> Dataset:
         """Loads the uci_pen_digits dataset"""
-        return Dataset._from_url("uci_pen_digits", force=redownload)
+        return Dataset.get("uci_pen_digits", redownload=redownload)
 
     @staticmethod
     def uci_characters(redownload: bool = False) -> Dataset:
         """Loads the uci_characters dataset"""
-        return Dataset._from_url("uci_characters", force=redownload)
+        return Dataset.get("uci_characters", redownload=redownload)
 
     @staticmethod
-    def stochastic_models(redownload: bool = False) -> Dataset:
-        """Loads the stochastic models dataset"""
-        return Dataset._from_url("stochastic_models", force=redownload)
+    def diffusive_particles(redownload: bool = False) -> Dataset:
+        """Loads the diffusive particles dataset"""
+        return Dataset.get("diffusive_particles", redownload=redownload)
+    
+    @staticmethod
+    def get(dataset_name: str, redownload: bool = False) -> Dataset:
+        """Loads a dataset from the trajectory-dataset repository"""
+        return Dataset._from_url(dataset_name, force=redownload)
```

### Comparing `pactus-0.3.0/pactus/models/__init__.py` & `pactus-0.4.0/pactus/models/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,22 +4,20 @@
 from pactus.models.kneighbors_model import KNeighborsModel
 from pactus.models.lstm_model import LSTMModel
 from pactus.models.model import Model
 from pactus.models.random_forest_model import RandomForestModel
 from pactus.models.svm_model import SVMModel
 from pactus.models.transformer_model import TransformerModel
 from pactus.models.xgboost_model import XGBoostModel
-from pactus.models.zoom_transformer_model import ZoomTransformerModel
 
 __all__ = [
+    "Model",
     "DecisionTreeModel",
     "Evaluation",
     "EvaluationComparison",
     "KNeighborsModel",
-    "Model",
     "RandomForestModel",
     "SVMModel",
     "TransformerModel",
-    "ZoomTransformerModel",
     "XGBoostModel",
     "LSTMModel",
 ]
```

### Comparing `pactus-0.3.0/pactus/models/decision_tree_model.py` & `pactus-0.4.0/pactus/models/decision_tree_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/models/evaluation.py` & `pactus-0.4.0/pactus/models/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
     @staticmethod
     def from_data(
         data: Data,
         predictions: List[Any],
         model_summary: dict,
     ) -> Evaluation:
         return Evaluation(
-            dataset_name=data.dataset.name,
+            dataset_name=data.dataset_name,
             trajs_ids=[traj.traj_id for traj in data.trajs if traj.traj_id is not None],
             y_true=data.labels,
             y_pred=predictions,
             model_summary=model_summary,
         )
 
     def _conf_matrix_perc(self) -> np.ndarray:
```

### Comparing `pactus-0.3.0/pactus/models/evaluation_comparison.py` & `pactus-0.4.0/pactus/models/evaluation_comparison.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
             model = evaluation.model_summary["name"]
             self.evals_by_model[model] = self.evals_by_model.get(model, []) + [
                 evaluation
             ]
 
         self.evals_by_dataset: Dict[str, List[Evaluation]] = {}
         for evaluation in self.evals:
-            ds_name = evaluation.dataset.name
+            ds_name = evaluation.dataset_name
             self.evals_by_dataset[ds_name] = self.evals_by_dataset.get(ds_name, []) + [
                 evaluation
             ]
 
     def to_latex(self) -> str:
         rows = []
         for model, evaluations in self.evals_by_model.items():
```

### Comparing `pactus-0.3.0/pactus/models/kneighbors_model.py` & `pactus-0.4.0/pactus/models/kneighbors_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/models/lstm_model.py` & `pactus-0.4.0/pactus/models/lstm_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,20 @@
+import datetime
 import logging
+import time
 from pathlib import Path
 from typing import Any, List, Tuple, Union
 
 import numpy as np
+import tensorflow as tf
 from sklearn.preprocessing import LabelEncoder
 from tensorflow import keras
-from tensorflow.keras import layers
 from yupi import Trajectory
 
+from pactus import Dataset
 from pactus import config as cfg
 from pactus.dataset import Data
 from pactus.models.evaluation import Evaluation
 from pactus.models.model import Model
 
 NAME = "lstm"
 
@@ -26,21 +29,24 @@
     def __init__(
         self,
         units: Union[List[int], None] = None,
         masking_value: Union[int, None] = None,
         loss="sparse_categorical_crossentropy",
         optimizer="rmsprop",
         metrics=None,
+        random_state: Union[int, None] = None,
         **kwargs,
     ):
         super().__init__(NAME)
         self.masking_value = cfg.MASK_VALUE if masking_value is None else masking_value
         self.encoder: Union[LabelEncoder, None] = None
+        self.dataset: Union[Dataset, None] = None
         self.model: keras.Secuential
         self.max_len = 0
+        self.random_state = random_state
         metrics = ["accuracy"] if metrics is None else metrics
         self.units = [128, 64] if units is None else units
         kwargs.update(dict(loss=loss, optimizer=optimizer, metrics=metrics))
         self.compile_args = kwargs
         self.set_summary(**self.compile_args)
 
     def _get_x_data(self, max_len: int, trajs: List[Trajectory]) -> np.ndarray:
@@ -59,61 +65,74 @@
             _X[i, :top, -1] = traj.t
         return _X
 
     def _get_model(self, input_shape, n_classes):
         max_len, traj_dim = input_shape
         model = keras.Sequential()
         model.add(
-            layers.Masking(
-                mask_value=self.masking_value, input_shape=(max_len, traj_dim)
+            keras.layers.Masking(
+                mask_value=self.masking_value,
+                input_shape=(max_len, traj_dim),
             )
         )
         for units_val in self.units:
             model.add(
-                layers.LSTM(
+                keras.layers.LSTM(
                     units_val,
                     input_shape=(max_len, traj_dim),
                     return_sequences=True,
                 )
             )
         model.add(
-            layers.Bidirectional(
-                layers.LSTM(32, input_shape=(max_len, traj_dim)), merge_mode="ave"
+            keras.layers.Bidirectional(
+                keras.layers.LSTM(32, input_shape=(max_len, traj_dim)),
+                merge_mode="ave",
             )
         )
-        model.add(layers.Dense(15, activation="relu"))
-        model.add(layers.Dense(n_classes, activation="softmax"))
+        model.add(keras.layers.Dense(15, activation="relu"))
+        model.add(keras.layers.Dense(n_classes, activation="softmax"))
         model.compile(**self.compile_args)
         return model
 
     def _prepare_data(self, data: Data) -> Tuple[np.ndarray, np.ndarray]:
+        assert self.dataset is not None, "Dataset is not set"
+
         self.encoder = LabelEncoder()
         self.encoder.fit(data.labels)
         encoded_labels = self.encoder.transform(data.labels)
         y_data = np.array(encoded_labels)
 
-        self.max_len = max(map(len, data.dataset.trajs))
+        self.max_len = max(map(len, self.dataset.trajs))
         x_data = self._get_x_data(self.max_len, data.trajs)
         return x_data, y_data
 
     def train(
         self,
         data: Data,
+        dataset: Dataset,
         cross_validation=0,
         epochs=10,
         batch_size=None,
         validation_split=None,
         callbacks: Union[list, None] = None,
         checkpoint: Union[keras.callbacks.ModelCheckpoint, None] = None,
     ):
+        if self.random_state is not None:
+            tf.keras.utils.set_random_seed(self.random_state)
+            logging.warning(
+                f"Custom seed provided for {self.name} model. This "
+                "calls 'tf.keras.utils.set_random_seed' which sets a global "
+                "random state on python, numpy and tensorflow."
+            )
         if cross_validation != 0:
             logging.warning("Cross validation is not supported yet for lstm")
         self.set_summary(epochs=epochs, validation_split=validation_split)
         callbacks = DEFAULT_CALLBACKS.copy() if callbacks is None else callbacks
         model_path = None
+        self.dataset = dataset
         if checkpoint is not None:
             callbacks.append(checkpoint)
             if Path(checkpoint.filepath).exists():
                 logging.info("Loading model from checkpoint %s", checkpoint.filepath)
                 model_path = checkpoint.filepath
         x_train, y_train = self._prepare_data(data)
         self.model = (
```

### Comparing `pactus-0.3.0/pactus/models/model.py` & `pactus-0.4.0/pactus/models/model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/models/random_forest_model.py` & `pactus-0.4.0/pactus/models/random_forest_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/models/svm_model.py` & `pactus-0.4.0/pactus/models/svm_model.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/models/transformer.py` & `pactus-0.4.0/pactus/models/transformer.py`

 * *Files identical despite different names*

### Comparing `pactus-0.3.0/pactus/models/transformer_model.py` & `pactus-0.4.0/pactus/models/transformer_model.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 import logging
 from pathlib import Path
 from typing import Any, List, Tuple, Union
 
 import numpy as np
+import tensorflow as tf
 from sklearn.model_selection import KFold
 from sklearn.preprocessing import LabelEncoder
 from tensorflow import keras
 
 import pactus.config as cfg
+from pactus import Dataset
 from pactus.dataset import Data
 from pactus.models import Model
 from pactus.models.evaluation import Evaluation
 from pactus.models.transformer import TransformerBlock, build_model
 
 NAME = "transformer_model"
 DEFAULT_OPTIMIZER = keras.optimizers.Adam(learning_rate=1e-2)
@@ -34,17 +36,17 @@
         dropout: float = 0.25,
         loss="categorical_crossentropy",
         optimizer=None,
         metrics=None,
         max_traj_len: int = -1,
         skip_long_trajs: bool = False,
         mask_value=cfg.MASK_VALUE,
-        name=NAME,
+        random_state: Union[int, None] = None,
     ):
-        super().__init__(name)
+        super().__init__(NAME)
         self.head_size = head_size
         self.num_heads = num_heads
         self.ff_dim = ff_dim
         self.num_transformer_blocks = num_transformer_blocks
         self.mlp_units = [128] if mlp_units is None else mlp_units
         self.mlp_dropout = mlp_dropout
         self.dropout = dropout
@@ -53,14 +55,16 @@
         self.optimizer = DEFAULT_OPTIMIZER if optimizer is None else optimizer
         self.metrics = ["accuracy"] if metrics is None else metrics
         self.max_traj_len = max_traj_len
         self.skip_long_trajs = skip_long_trajs
         self.mask_value = mask_value
         self.encoder: Union[LabelEncoder, None] = None
         self.labels: Union[List[Any], None] = None
+        self.original_data: Union[Data, None] = None
+        self.random_state: Union[int, None] = random_state
         self.set_summary(
             head_size=self.head_size,
             num_heads=self.num_heads,
             ff_dim=self.ff_dim,
             num_transformer_blocks=self.num_transformer_blocks,
             mlp_units=self.mlp_units,
             mlp_dropout=self.mlp_dropout,
@@ -71,29 +75,38 @@
             max_traj_len=self.max_traj_len,
             skip_long_trajs=self.skip_long_trajs,
         )
 
     def train(
         self,
         data: Data,
+        original_data: Data,
         cross_validation: int = 0,
         epochs: int = 10,
         validation_split: float = 0.2,
         batch_size: int = 32,
         callbacks: Union[list, None] = None,
         checkpoint: Union[keras.callbacks.ModelCheckpoint, None] = None,
     ):
+        if self.random_state is not None:
+            tf.keras.utils.set_random_seed(self.random_state)
+            logging.warning(
+                f"Custom seed provided for {self.name} model. This "
+                "calls 'tf.keras.utils.set_random_seed' which sets a global "
+                "random state on python, numpy and tensorflow."
+            )
         self.set_summary(
             cross_validation=cross_validation,
             epochs=epochs,
             validation_split=validation_split,
             batch_size=batch_size,
         )
         self.encoder = None
         self.labels = data.labels
+        self.original_data = original_data
         x_train, y_train = self._get_input_data(data)
         n_classes = len(data.classes)
         input_shape = x_train.shape[1:]
         callbacks = DEFAULT_CALLBACKS.copy() if callbacks is None else callbacks
         model_path = None
         if checkpoint is not None:
             callbacks.append(checkpoint)
@@ -162,23 +175,23 @@
         return self.model.predict(x_data)
 
     def _get_model(
         self, n_classes: int, input_shape: tuple, mask: Any = None
     ) -> keras.Model:
         model = build_model(
             n_classes,
-            input_shape,
+            input_shape=input_shape,
             head_size=self.head_size,
             num_heads=self.num_heads,
             ff_dim=self.ff_dim,
             num_transformer_blocks=self.num_transformer_blocks,
             mlp_units=self.mlp_units,
             mlp_dropout=self.mlp_dropout,
             dropout=self.dropout,
-            mask=mask,
+            # mask=mask, # FIXME: using mask is causing input shapes issues
         )
         model.compile(
             loss=self.loss,
             optimizer=self.optimizer,
             metrics=self.metrics,
         )
         return model
@@ -204,16 +217,18 @@
         classes = np.zeros((len(encoded_labels), len(self.encoder.classes_)))
         for i, label in enumerate(encoded_labels):
             classes[i][label] = 1
         return classes
 
     def _extract_raw_data(self, data: Data) -> np.ndarray:
         """Extracts the raw data from the yupi trajectories"""
+        assert self.original_data is not None, "Original data must be set"
+
         trajs = data.trajs
-        max_len = np.max([len(traj) for traj in data.dataset.trajs])
+        max_len = np.max([len(traj) for traj in self.original_data.trajs])
         if self.max_traj_len > 0:
             max_len = self.max_traj_len
         raw_data = [np.hstack((traj.r, np.reshape(traj.t, (-1, 1)))) for traj in trajs]
         if self.skip_long_trajs:
             raw_data = [traj for traj in raw_data if traj.shape[0] <= max_len]
         assert len(raw_data) > 0, "No trajectories to train on"
         all_raw_data = np.zeros((len(raw_data), max_len, 3))
```

### Comparing `pactus-0.3.0/pactus/models/xgboost_model.py` & `pactus-0.4.0/pactus/models/xgboost_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,12 +39,13 @@
         self.grid = GridSearchCV(self.model, {}, cv=cross_validation, verbose=3)
         classes = self._encode_labels(data)
         self.grid.fit(x_data, classes)
 
     def predict(self, data: Data) -> List[Any]:
         x_data = data.featurize(self.featurizer)
         predicted = self.grid.predict(x_data)
+        assert self.encoder is not None
         return self.encoder.inverse_transform(predicted)
 
     def predict_single(self, traj: Trajectory) -> Any:
         """Predicts the label of a single trajectory."""
         return self.grid.predict([traj])[0]
```

### Comparing `pactus-0.3.0/pactus.egg-info/SOURCES.txt` & `pactus-0.4.0/pactus.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 README.md
 pyproject.toml
+setup.cfg
 pactus/__init__.py
 pactus/config.py
 pactus.egg-info/PKG-INFO
 pactus.egg-info/SOURCES.txt
 pactus.egg-info/dependency_links.txt
 pactus.egg-info/requires.txt
 pactus.egg-info/top_level.txt
@@ -19,9 +20,8 @@
 pactus/models/lstm_model.py
 pactus/models/model.py
 pactus/models/random_forest_model.py
 pactus/models/svm_model.py
 pactus/models/transformer.py
 pactus/models/transformer_model.py
 pactus/models/xgboost_model.py
-pactus/models/zoom_transformer_model.py
-pactus/models/zoomletizer.py
+tests/test_data.py
```

### Comparing `pactus-0.3.0/pyproject.toml` & `pactus-0.4.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,63 +1,93 @@
 [project]
 name = "pactus"
-version = "0.3.0"
+version = "0.4.0"
 description = "Framework to evaluate Trajectory Classification Algorithms"
 readme = "README.md"
 authors = [
     { name = "Jorge Morgado Vega", email = "jorge.morgadov@gmail.com" },
     { name = "Gustavo Viera-López", email = "gvieralopez@gmail.com" },
     { name = "Alfredo Reyes", email = "areyes@fisica.uh.cu" },
 ]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["trajectory", "classification"]
+keywords = ["trajectory",
+    "classification"]
 dependencies = [
     "numpy >= 1.20.0",
     "yupi >= 0.11.2",
     "tensorflow >= 2.9.1",
     "scikit-learn >= 1.1.1",
     "xgboost >= 1.7.4",
     "GitPython >= 3.1.29"
 ]
 requires-python = ">=3.8"
 
+[options]
+packages = [
+    { name = "pactus", include = true },
+]
+
 [project.optional-dependencies]
-dev = ["black", "pylint", "bumpver", "isort", "pytest"]
+dev = [
+    "mypy",
+    "black",
+    "pylint",
+    "bumpver",
+    "isort",
+    "pytest",
+    "tensor-annotations-tensorflow-stubs"
+]
 
 [project.urls]
 Homepage = "https://github.com/yupidevs/pactus"
 
 [tool.isort]
 profile = "black"
 known_first_party = ["pactus"]
 
 [tool.black]
-target-version = ["py37"]
+target-version = ["py38"]
 
 [tool.pylint."MESSAGES CONTROL"]
 max-line-length = 88
 
 [tool.bumpver]
-current_version = "0.3.0"
+current_version = "0.4.0"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
 "pyproject.toml" = [
     'current_version = "{version}"',
     'version = "{version}"',
 ]
 "pactus/__init__.py" = [
     '__version__ = "{version}"',
 ]
+"docs/source/conf.py" = [
+    'release = "{version}"',
+]
 
 [build-system]
-requires      = ["setuptools>=61.0.0", "wheel"]
+requires      = ["setuptools>=61.0.0",
+    "wheel"]
 build-backend = "setuptools.build_meta"
 
+[tool.mypy]
+python_version = "3.8"
+exclude = [
+    "docs",
+]
+
+[[tool.mypy.overrides]]
+module = [
+    "yupi.*",
+    "sklearn.*",
+]
+ignore_missing_imports = true
```

